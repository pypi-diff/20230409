# Comparing `tmp/qt_colored_logger-0.3.0.tar.gz` & `tmp/qt_colored_logger-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qt_colored_logger-0.3.0.tar", last modified: Wed Apr  5 15:00:03 2023, max compression
+gzip compressed data, was "qt_colored_logger-0.4.0.tar", last modified: Sun Apr  9 16:56:53 2023, max compression
```

## Comparing `qt_colored_logger-0.3.0.tar` & `qt_colored_logger-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 15:00:03.656013 qt_colored_logger-0.3.0/
--rw-rw-rw-   0        0        0    11357 2023-03-13 14:04:00.000000 qt_colored_logger-0.3.0/LICENSE
--rw-rw-rw-   0        0        0    37972 2023-04-05 15:00:03.657014 qt_colored_logger-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    37204 2023-04-05 14:57:21.000000 qt_colored_logger-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 15:00:03.598014 qt_colored_logger-0.3.0/qt_colored_logger/
--rw-rw-rw-   0        0        0     1749 2023-04-05 14:57:21.000000 qt_colored_logger-0.3.0/qt_colored_logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 15:00:03.633015 qt_colored_logger-0.3.0/qt_colored_logger/_basic/
--rw-rw-rw-   0        0        0     1700 2023-04-05 10:50:01.000000 qt_colored_logger-0.3.0/qt_colored_logger/_basic/__init__.py
--rw-rw-rw-   0        0        0     6833 2023-04-05 10:45:27.000000 qt_colored_logger-0.3.0/qt_colored_logger/_basic/_basic_logger.py
--rw-rw-rw-   0        0        0     2030 2023-04-05 10:50:01.000000 qt_colored_logger-0.3.0/qt_colored_logger/_basic/_exceptions.py
--rw-rw-rw-   0        0        0     1732 2023-03-31 13:07:44.000000 qt_colored_logger-0.3.0/qt_colored_logger/_basic/_patterns.py
--rw-rw-rw-   0        0        0    39395 2023-04-05 12:38:32.000000 qt_colored_logger-0.3.0/qt_colored_logger/colored_logger.py
--rw-rw-rw-   0        0        0    37351 2023-04-05 14:17:48.000000 qt_colored_logger-0.3.0/qt_colored_logger/html_colored_logger.py
-drwxrwxrwx   0        0        0        0 2023-04-05 15:00:03.645015 qt_colored_logger-0.3.0/qt_colored_logger/src/
--rw-rw-rw-   0        0        0     1740 2023-04-01 18:46:09.000000 qt_colored_logger-0.3.0/qt_colored_logger/src/__init__.py
--rw-rw-rw-   0        0        0     6132 2023-04-01 10:33:48.000000 qt_colored_logger-0.3.0/qt_colored_logger/src/ansi_format.py
--rw-rw-rw-   0        0        0    10245 2023-04-01 18:46:02.000000 qt_colored_logger-0.3.0/qt_colored_logger/src/color_picker.py
--rw-rw-rw-   0        0        0     1940 2023-04-05 10:06:34.000000 qt_colored_logger-0.3.0/qt_colored_logger/test.py
-drwxrwxrwx   0        0        0        0 2023-04-05 15:00:03.608011 qt_colored_logger-0.3.0/qt_colored_logger.egg-info/
--rw-rw-rw-   0        0        0    37972 2023-04-05 15:00:03.000000 qt_colored_logger-0.3.0/qt_colored_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      599 2023-04-05 15:00:03.000000 qt_colored_logger-0.3.0/qt_colored_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 15:00:03.000000 qt_colored_logger-0.3.0/qt_colored_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-05 15:00:03.000000 qt_colored_logger-0.3.0/qt_colored_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-05 15:00:03.658014 qt_colored_logger-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2818 2023-04-05 14:57:21.000000 qt_colored_logger-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:56:53.221768 qt_colored_logger-0.4.0/
+-rw-rw-rw-   0        0        0    11357 2023-03-13 14:04:00.000000 qt_colored_logger-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     9691 2023-04-09 16:56:53.221768 qt_colored_logger-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8898 2023-04-09 10:07:36.000000 qt_colored_logger-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 16:56:53.129109 qt_colored_logger-0.4.0/qt_colored_logger/
+-rw-rw-rw-   0        0        0      811 2023-04-09 16:19:08.000000 qt_colored_logger-0.4.0/qt_colored_logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:56:53.161114 qt_colored_logger-0.4.0/qt_colored_logger/basic/
+-rw-rw-rw-   0        0        0      812 2023-04-08 15:53:12.000000 qt_colored_logger-0.4.0/qt_colored_logger/basic/__init__.py
+-rw-rw-rw-   0        0        0     5893 2023-04-08 15:53:12.000000 qt_colored_logger-0.4.0/qt_colored_logger/basic/basic_logger.py
+-rw-rw-rw-   0        0        0     1126 2023-04-08 15:53:12.000000 qt_colored_logger-0.4.0/qt_colored_logger/basic/exceptions.py
+-rw-rw-rw-   0        0        0      848 2023-04-08 15:17:18.000000 qt_colored_logger-0.4.0/qt_colored_logger/basic/patterns.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:56:53.178009 qt_colored_logger-0.4.0/qt_colored_logger/logger/
+-rw-rw-rw-   0        0        0      739 2023-04-08 15:53:12.000000 qt_colored_logger-0.4.0/qt_colored_logger/logger/__init__.py
+-rw-rw-rw-   0        0        0    39641 2023-04-09 09:07:44.000000 qt_colored_logger-0.4.0/qt_colored_logger/logger/colored_logger.py
+-rw-rw-rw-   0        0        0    37471 2023-04-09 09:14:39.000000 qt_colored_logger-0.4.0/qt_colored_logger/logger/html_colored_logger.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:56:53.195121 qt_colored_logger-0.4.0/qt_colored_logger/src/
+-rw-rw-rw-   0        0        0      866 2023-04-08 15:58:27.000000 qt_colored_logger-0.4.0/qt_colored_logger/src/__init__.py
+-rw-rw-rw-   0        0        0     4758 2023-04-08 15:58:27.000000 qt_colored_logger-0.4.0/qt_colored_logger/src/ansi_format.py
+-rw-rw-rw-   0        0        0     8957 2023-04-08 15:58:27.000000 qt_colored_logger-0.4.0/qt_colored_logger/src/color_picker.py
+-rw-rw-rw-   0        0        0     1677 2023-04-07 12:17:31.000000 qt_colored_logger-0.4.0/qt_colored_logger/src/~log_environment.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:56:53.219767 qt_colored_logger-0.4.0/qt_colored_logger/text/
+-rw-rw-rw-   0        0        0      720 2023-04-08 16:15:43.000000 qt_colored_logger-0.4.0/qt_colored_logger/text/__init__.py
+-rw-rw-rw-   0        0        0     5881 2023-04-09 09:04:41.000000 qt_colored_logger-0.4.0/qt_colored_logger/text/text_buffer.py
+-rw-rw-rw-   0        0        0     4822 2023-04-07 12:21:55.000000 qt_colored_logger-0.4.0/qt_colored_logger/text/~animation.py
+-rw-rw-rw-   0        0        0     1704 2023-04-07 12:17:31.000000 qt_colored_logger-0.4.0/qt_colored_logger/text/~icon_set.py
+-rw-rw-rw-   0        0        0    14432 2021-01-12 12:58:45.000000 qt_colored_logger-0.4.0/qt_colored_logger/~~logger~~.py
+-rw-rw-rw-   0        0        0     7482 2021-01-12 12:58:45.000000 qt_colored_logger-0.4.0/qt_colored_logger/~~utils~~.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:56:53.140826 qt_colored_logger-0.4.0/qt_colored_logger.egg-info/
+-rw-rw-rw-   0        0        0     9691 2023-04-09 16:56:52.000000 qt_colored_logger-0.4.0/qt_colored_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      868 2023-04-09 16:56:53.000000 qt_colored_logger-0.4.0/qt_colored_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 16:56:52.000000 qt_colored_logger-0.4.0/qt_colored_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-09 16:56:52.000000 qt_colored_logger-0.4.0/qt_colored_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 16:56:53.222767 qt_colored_logger-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2920 2023-04-09 16:39:19.000000 qt_colored_logger-0.4.0/setup.py
```

### Comparing `qt_colored_logger-0.3.0/LICENSE` & `qt_colored_logger-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qt_colored_logger-0.3.0/qt_colored_logger/__init__.py` & `qt_colored_logger-0.4.0/qt_colored_logger/text/~icon_set.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-# ##########################   Qt_Colored-logger   ########################### #
-# ---------------------------------------------------------------------------- #
-#                                                                              #
-# Copyright © 2023 Kalynovsky Valentin. All rights reserved.                   #
-#                                                                              #
-# Licensed under the Apache License, Version 2.0 (the "License");              #
-# you may not use this file except in compliance with the License.             #
-# You may obtain a copy of the License at                                      #
-#                                                                              #
-#     http://www.apache.org/licenses/LICENSE-2.0                               #
-#                                                                              #
-# Unless required by applicable law or agreed to in writing, software          #
-# distributed under the License is distributed on an "AS IS" BASIS,            #
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.     #
-# See the License for the specific language governing permissions and          #
-# limitations under the License.                                               #
-#                                                                              #
-# ---------------------------------------------------------------------------- #
-# ############################################################################ #
-
-from .colored_logger import Logger
-from .html_colored_logger import LoggerQ
-
-__authot__ = "Kalynovsky 'Nakama3942' Valentin"
-__version__ = "0.3.0"
-__email__ = "nakama3942@gmail.com"
+# ##########################   Qt_Colored-logger   ########################### #
+# ---------------------------------------------------------------------------- #
+#                                                                              #
+# Copyright © 2023 Kalynovsky Valentin. All rights reserved.                   #
+#                                                                              #
+# Licensed under the Apache License, Version 2.0 (the "License");              #
+# you may not use this file except in compliance with the License.             #
+# You may obtain a copy of the License at                                      #
+#                                                                              #
+#     http://www.apache.org/licenses/LICENSE-2.0                               #
+#                                                                              #
+# Unless required by applicable law or agreed to in writing, software          #
+# distributed under the License is distributed on an "AS IS" BASIS,            #
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.     #
+# See the License for the specific language governing permissions and          #
+# limitations under the License.                                               #
+#                                                                              #
+# ---------------------------------------------------------------------------- #
+# ############################################################################ #
+
+class IconSet:
+    info = 'ℹ'
+    success = '✔'
+    fail = '✘'
+    warning = '!'
+    error = '☠'
+    critical = '☠'
+    process = '⧗'
+    time = '◴'
```

### Comparing `qt_colored_logger-0.3.0/qt_colored_logger/colored_logger.py` & `qt_colored_logger-0.4.0/qt_colored_logger/logger/colored_logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# ##########################   Qt_Colored-logger   ########################### #
-# ---------------------------------------------------------------------------- #
-#                                                                              #
-# Copyright © 2023 Kalynovsky Valentin. All rights reserved.                   #
-#                                                                              #
-# Licensed under the Apache License, Version 2.0 (the "License");              #
-# you may not use this file except in compliance with the License.             #
-# You may obtain a copy of the License at                                      #
-#                                                                              #
-#     http://www.apache.org/licenses/LICENSE-2.0                               #
-#                                                                              #
-# Unless required by applicable law or agreed to in writing, software          #
-# distributed under the License is distributed on an "AS IS" BASIS,            #
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.     #
-# See the License for the specific language governing permissions and          #
-# limitations under the License.                                               #
-#                                                                              #
-# ---------------------------------------------------------------------------- #
-# ############################################################################ #
+"""
+A module with the implementation of a standard (console) logger.
+\n
+Copyright © 2023 Kalynovsky Valentin. All rights reserved.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
+from qt_colored_logger.basic.basic_logger import BasicLogger
+from qt_colored_logger.basic.exceptions import ColorException, CombinationException
+from qt_colored_logger.src.color_picker import AnsiColor, Dec2Ansi
+from qt_colored_logger.text.text_buffer import TextBuffer
 
-from qt_colored_logger._basic import _Singleton, _BasicLogger, ColorException, CombinationException
-from qt_colored_logger.src import AnsiColor, Dec2Ansi
-
-class Logger(_Singleton, _BasicLogger):
+class Logger(BasicLogger):
 	"""
 	The Logger class is a class that implements the functionality
 	of logging the work of software in different directions.\n
 	It has a color output of information, settings for the operation of the log.
 	Only one class object can be created!!!\n
 	Implements the output of the following information:\n
 	1) Record creation time;
@@ -52,26 +52,28 @@
 	16) `FAIL`
 	"""
 
 	def __init__(
 			self,
 			*,
 			program_name: str = "Unknown",
+			text_buffer: TextBuffer = TextBuffer(),
 			global_background: bool = False,
 			time: bool = True,
 			status: bool = True,
 			status_message: bool = True,
 			status_type: bool = True,
 			message: bool = True
 	):
 		super().__init__(program_name, time, status, status_message, status_type, message)
+		self._buffer = text_buffer
 		self._AnsiColorSet: dict = {}
 		self._ansi_color_set_init()
 		self.global_background = global_background
-		print(self._initial_log())  # todo Перенести в буфер
+		self._initial_log()
 
 	def _ansi_color_set_init(self):
 		"""
 		Sets the colors of the logger.
 		"""
 		self._AnsiColorSet['INITIAL_COLOR'] = [AnsiColor('GOLD', "foreground"), AnsiColor('INDIGO', "foreground")]
 		self._AnsiColorSet['INITIAL_BACKGROUND'] = ["", AnsiColor('GOLD', "background")]
@@ -188,20 +190,21 @@
 		self._AnsiColorSet['FAIL_MESSAGE'] = [AnsiColor('DARKRED', "foreground"), AnsiColor('DARKYELLOW', "foreground")]
 		self._AnsiColorSet['FAIL_BACKGROUND'] = ["", AnsiColor('DARKRED', "background")]
 
 	def _initial_log(self):
 		"""
 		Displays initialized information.
 		"""
-		return self._initialized_data(  # todo return заменить на buffer
+		self._buffer << self._initialized_data(
 			[
 				self._AnsiColorSet['INITIAL_COLOR'][self.global_background],
 				self._AnsiColorSet['INITIAL_BACKGROUND'][self.global_background]
 			]
 		)
+		self._buffer.update_console()
 
 	def set_color(self, *, logger_color_name: str, color_value: list[int, int, int], foreground: bool = True, background: bool = False):
 		"""
 		A method that sets the ANSI escape code color code in the color table of the logger.
 		May throw a ColorException if the given color is not in the table.
 		The logger color table stores the following keys: see README.md/Data/"Logger Color Chart".\n
 		Boolean flags: If foreground is set to True, then the color of the foreground text will change
@@ -224,458 +227,482 @@
 				self._AnsiColorSet[logger_color_name][1] = Dec2Ansi(color_value, "foreground")
 			elif not background and foreground:
 				self._AnsiColorSet[logger_color_name][0] = Dec2Ansi(color_value, "foreground")
 			else:
 				raise CombinationException("False-False combination of foreground-background flags not possible")
 		else:
 			raise ColorException("This color is not in the dictionary")
+    
+	def get_buffer(self):
+		"""
+		Usually, before creating a logger, you need to create a text buffer
+		and pass it to the constructor. But if this has not been done, the buffer
+		is created directly in the logger. And to get it (for example, to save
+		the buffer to a file), this method was implemented. It returns a buffer.
 
-	def DEBUG(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None) -> str:
+		:return: a text buffer object
+		"""
+		return self._buffer
+
+	def DEBUG(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None):
 		"""
 		Debugging information logging:
 		Can be used to log entry any information while debugging an application.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param invert: Display entry with invert font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_entry(
+		self._buffer << self._assemble_entry(
 			[
 				self._AnsiColorSet['DEBUG_TIME'][background],
 				self._AnsiColorSet['DEBUG_STATUS'][background],
 				self._AnsiColorSet['DEBUG_STATUS_MESSAGE'][background],
 				self._AnsiColorSet['TYPE_DEBUG'][background],
 				self._AnsiColorSet['DEBUG_MESSAGE'][background],
 				self._AnsiColorSet['DEBUG_BACKGROUND'][background],
 			], status_message_text, "%DEBUG", message_text, bold, italic, invert
 		)
+		self._buffer.update_console()
 
-	def DEBUG_PERFORMANCE(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None) -> str:
+	def DEBUG_PERFORMANCE(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None):
 		"""
 		Performance debugging information logging:
 		Can be used to log entry the execution time of operations or other
 		performance information while the application is being debugged.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param invert: Display entry with invert font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_entry(
+		self._buffer << self._assemble_entry(
 			[
 				self._AnsiColorSet['DEBUG_PERFORMANCE_TIME'][background],
 				self._AnsiColorSet['DEBUG_PERFORMANCE_STATUS'][background],
 				self._AnsiColorSet['DEBUG_PERFORMANCE_STATUS_MESSAGE'][background],
 				self._AnsiColorSet['TYPE_DEBUG_PERFORMANCE'][background],
 				self._AnsiColorSet['DEBUG_PERFORMANCE_MESSAGE'][background],
 				self._AnsiColorSet['DEBUG_PERFORMANCE_BACKGROUND'][background],
 			], status_message_text, "%DEBUG PERFORMANCE", message_text, bold, italic, invert
 		)
+		self._buffer.update_console()
 
-	def PERFORMANCE(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None) -> str:
+	def PERFORMANCE(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None):
 		"""
 		Performance information logging:
 		Can be used to log entry the execution time of operations or
 		other application performance information.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param invert: Display entry with invert font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_entry(
+		self._buffer << self._assemble_entry(
 			[
 				self._AnsiColorSet['PERFORMANCE_TIME'][background],
 				self._AnsiColorSet['PERFORMANCE_STATUS'][background],
 				self._AnsiColorSet['PERFORMANCE_STATUS_MESSAGE'][background],
 				self._AnsiColorSet['TYPE_PERFORMANCE'][background],
 				self._AnsiColorSet['PERFORMANCE_MESSAGE'][background],
 				self._AnsiColorSet['PERFORMANCE_BACKGROUND'][background],
 			], status_message_text, "%PERFORMANCE", message_text, bold, italic, invert
 		)
+		self._buffer.update_console()
 
-	def EVENT(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None) -> str:
+	def EVENT(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None):
 		"""
 		Event information logging:
 		Can be used to log entry specific events in the application,
 		such as button presses or mouse cursor movements.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param invert: Display entry with invert font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_entry(
+		self._buffer << self._assemble_entry(
 			[
 				self._AnsiColorSet['EVENT_TIME'][background],
 				self._AnsiColorSet['EVENT_STATUS'][background],
 				self._AnsiColorSet['EVENT_STATUS_MESSAGE'][background],
 				self._AnsiColorSet['TYPE_EVENT'][background],
 				self._AnsiColorSet['EVENT_MESSAGE'][background],
 				self._AnsiColorSet['EVENT_BACKGROUND'][background],
 			], status_message_text, "~EVENT", message_text, bold, italic, invert
 		)
+		self._buffer.update_console()
 
-	def AUDIT(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None) -> str:
+	def AUDIT(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None):
 		"""
 		Audit information logging:
 		Can be used to log entry changes in the system, such as creating or
 		deleting users, as well as changes in security settings.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param invert: Display entry with invert font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_entry(
+		self._buffer << self._assemble_entry(
 			[
 				self._AnsiColorSet['AUDIT_TIME'][background],
 				self._AnsiColorSet['AUDIT_STATUS'][background],
 				self._AnsiColorSet['AUDIT_STATUS_MESSAGE'][background],
 				self._AnsiColorSet['TYPE_AUDIT'][background],
 				self._AnsiColorSet['AUDIT_MESSAGE'][background],
 				self._AnsiColorSet['AUDIT_BACKGROUND'][background],
 			], status_message_text, "~AUDIT", message_text, bold, italic, invert
 		)
+		self._buffer.update_console()
 
-	def METRICS(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None) -> str:
+	def METRICS(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None):
 		"""
 		Metrics information logging:
 		Can be used to log entry metrics to track application performance and identify issues.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param invert: Display entry with invert font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_entry(
+		self._buffer << self._assemble_entry(
 			[
 				self._AnsiColorSet['METRICS_TIME'][background],
 				self._AnsiColorSet['METRICS_STATUS'][background],
 				self._AnsiColorSet['METRICS_STATUS_MESSAGE'][background],
 				self._AnsiColorSet['TYPE_METRICS'][background],
 				self._AnsiColorSet['METRICS_MESSAGE'][background],
 				self._AnsiColorSet['METRICS_BACKGROUND'][background],
 			], status_message_text, "~METRICS", message_text, bold, italic, invert
 		)
+		self._buffer.update_console()
 
-	def USER(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None) -> str:
+	def USER(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None):
 		"""
 		User information logging:
 		Can be used to log entry custom logs to store additional information
 		that may be useful for diagnosing problems.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param invert: Display entry with invert font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_entry(
+		self._buffer << self._assemble_entry(
 			[
 				self._AnsiColorSet['USER_TIME'][background],
 				self._AnsiColorSet['USER_STATUS'][background],
 				self._AnsiColorSet['USER_STATUS_MESSAGE'][background],
 				self._AnsiColorSet['TYPE_USER'][background],
 				self._AnsiColorSet['USER_MESSAGE'][background],
 				self._AnsiColorSet['USER_BACKGROUND'][background],
 			], status_message_text, "~USER", message_text, bold, italic, invert
 		)
+		self._buffer.update_console()
 
-	def MESSAGE(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None) -> str:
+	def MESSAGE(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None):
 		"""
 		Message information logging:
 		Can be used for the usual output of ordinary messages about the program's operation.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param invert: Display entry with invert font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_entry(
+		self._buffer << self._assemble_entry(
 			[
 				self._AnsiColorSet['MESSAGE_TIME'][background],
 				self._AnsiColorSet['MESSAGE_STATUS'][background],
 				self._AnsiColorSet['MESSAGE_STATUS_MESSAGE'][background],
 				self._AnsiColorSet['TYPE_MESSAGE'][background],
 				self._AnsiColorSet['MESSAGE_MESSAGE'][background],
 				self._AnsiColorSet['MESSAGE_BACKGROUND'][background],
 			], status_message_text, "@MESSAGE", message_text, bold, italic, invert
 		)
+		self._buffer.update_console()
 
-	def INFO(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None) -> str:
+	def INFO(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None):
 		"""
 		Default information logging:
 		Can be used to log entry messages with specific content about the operation of the program.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param invert: Display entry with invert font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_entry(
+		self._buffer << self._assemble_entry(
 			[
 				self._AnsiColorSet['INFO_TIME'][background],
 				self._AnsiColorSet['INFO_STATUS'][background],
 				self._AnsiColorSet['INFO_STATUS_MESSAGE'][background],
 				self._AnsiColorSet['TYPE_INFO'][background],
 				self._AnsiColorSet['INFO_MESSAGE'][background],
 				self._AnsiColorSet['INFO_BACKGROUND'][background],
 			], status_message_text, "@INFO", message_text, bold, italic, invert
 		)
+		self._buffer.update_console()
 
-	def NOTICE(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None) -> str:
+	def NOTICE(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = None):
 		"""
 		Notice information logging:
 		Can be used to flag important events that might be missed with a normal logging level.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param invert: Display entry with invert font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_entry(
+		self._buffer << self._assemble_entry(
 			[
 				self._AnsiColorSet['NOTICE_TIME'][background],
 				self._AnsiColorSet['NOTICE_STATUS'][background],
 				self._AnsiColorSet['NOTICE_STATUS_MESSAGE'][background],
 				self._AnsiColorSet['TYPE_NOTICE'][background],
 				self._AnsiColorSet['NOTICE_MESSAGE'][background],
 				self._AnsiColorSet['NOTICE_BACKGROUND'][background],
 			], status_message_text, "@NOTICE", message_text, bold, italic, invert
 		)
+		self._buffer.update_console()
 
-	def WARNING(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = True) -> str:
+	def WARNING(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = True):
 		"""
 		Warning information logging:
 		Can be used to log entry warnings that the program may work with unpredictable results.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param invert: Display entry with invert font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
-		return self._assemble_entry(
+		self._buffer << self._assemble_entry(
 			[
 				self._AnsiColorSet['WARNING_TIME'][local_background],
 				self._AnsiColorSet['WARNING_STATUS'][local_background],
 				self._AnsiColorSet['WARNING_STATUS_MESSAGE'][local_background],
 				self._AnsiColorSet['TYPE_WARNING'][local_background],
 				self._AnsiColorSet['WARNING_MESSAGE'][local_background],
 				self._AnsiColorSet['WARNING_BACKGROUND'][local_background],
 			], status_message_text, "!WARNING", message_text, bold, italic, invert
 		)
+		self._buffer.update_console()
 
-	def ERROR(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = True) -> str:
+	def ERROR(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = True):
 		"""
 		Error information logging:
 		Used to log entry errors and crashes in the program.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param invert: Display entry with invert font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
-		return self._assemble_entry(
+		self._buffer << self._assemble_entry(
 			[
 				self._AnsiColorSet['ERROR_TIME'][local_background],
 				self._AnsiColorSet['ERROR_STATUS'][local_background],
 				self._AnsiColorSet['ERROR_STATUS_MESSAGE'][local_background],
 				self._AnsiColorSet['TYPE_ERROR'][local_background],
 				self._AnsiColorSet['ERROR_MESSAGE'][local_background],
 				self._AnsiColorSet['ERROR_BACKGROUND'][local_background],
 			], status_message_text, "!!ERROR", message_text, bold, italic, invert
 		)
+		self._buffer.update_console()
 
-	def CRITICAL(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = True, italic: bool = False, invert: bool = False, local_background: bool = True) -> str:
+	def CRITICAL(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = True, italic: bool = False, invert: bool = False, local_background: bool = True):
 		"""
 		Critical error information logging:
 		Used to log entry for critical and unpredictable program failures.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param invert: Display entry with invert font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
-		return self._assemble_entry(
+		self._buffer << self._assemble_entry(
 			[
 				self._AnsiColorSet['CRITICAL_TIME'][local_background],
 				self._AnsiColorSet['CRITICAL_STATUS'][local_background],
 				self._AnsiColorSet['CRITICAL_STATUS_MESSAGE'][local_background],
 				self._AnsiColorSet['TYPE_CRITICAL'][local_background],
 				self._AnsiColorSet['CRITICAL_MESSAGE'][local_background],
 				self._AnsiColorSet['CRITICAL_BACKGROUND'][local_background],
 			], status_message_text, "!!!@CRITICAL", message_text, bold, italic, invert
 		)
+		self._buffer.update_console()
 
-	def START_PROCESS(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = True) -> str:
+	def START_PROCESS(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = True):
 		"""
 		Stub.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param invert: Display entry with invert font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
-		# return self._assemble_entry(
+		# self._buffer << self._assemble_entry(
 		# 	[
 		# 		self._AnsiColorSet['PROGRESS_TIME'][local_background],
 		# 		self._AnsiColorSet['PROGRESS_STATUS'][local_background],
 		# 		self._AnsiColorSet['PROGRESS_STATUS_MESSAGE'][local_background],
 		# 		self._AnsiColorSet['TYPE_PROGRESS'][local_background],
 		# 		self._AnsiColorSet['PROGRESS_MESSAGE'][local_background],
 		# 		self._AnsiColorSet['PROGRESS_BACKGROUND'][local_background],
 		# 	], status_message_text, "&PROGRESS [*******.............] - 37%", message_text, bold, italic, invert
 		# )
+		# self._buffer.update_console()
 		pass
 		# Must run on a thread
 
-	def STOP_PROCESS(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = True) -> str:
+	def STOP_PROCESS(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, invert: bool = False, local_background: bool = True):
 		"""
 		Stub.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param invert: Display entry with invert font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		pass
 		# Make transition to SUCCESS or FAIL
 
-	def SUCCESS(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = True, invert: bool = False, local_background: bool = True) -> str:
+	def SUCCESS(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = True, invert: bool = False, local_background: bool = True):
 		"""
 		Success information logging:
 		Used to log entry a message about the success of the process.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param invert: Display entry with invert font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
-		return self._assemble_entry(
+		self._buffer << self._assemble_entry(
 			[
 				self._AnsiColorSet['SUCCESS_TIME'][local_background],
 				self._AnsiColorSet['SUCCESS_STATUS'][local_background],
 				self._AnsiColorSet['SUCCESS_STATUS_MESSAGE'][local_background],
 				self._AnsiColorSet['TYPE_SUCCESS'][local_background],
 				self._AnsiColorSet['SUCCESS_MESSAGE'][local_background],
 				self._AnsiColorSet['SUCCESS_BACKGROUND'][local_background],
 			], status_message_text, "&SUCCESS", message_text, bold, italic, invert
 		)
+		self._buffer.update_console()
 
-	def FAIL(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = True, invert: bool = False, local_background: bool = True) -> str:
+	def FAIL(self, *, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = True, invert: bool = False, local_background: bool = True):
 		"""
 		Fail information logging:
 		Used to log entry a message about the failed execution of the process.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param invert: Display entry with invert font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
-		return self._assemble_entry(
+		self._buffer << self._assemble_entry(
 			[
 				self._AnsiColorSet['FAIL_TIME'][local_background],
 				self._AnsiColorSet['FAIL_STATUS'][local_background],
 				self._AnsiColorSet['FAIL_STATUS_MESSAGE'][local_background],
 				self._AnsiColorSet['TYPE_FAIL'][local_background],
 				self._AnsiColorSet['FAIL_MESSAGE'][local_background],
 				self._AnsiColorSet['FAIL_BACKGROUND'][local_background],
 			], status_message_text, "&FAIL", message_text, bold, italic, invert
 		)
-
+		self._buffer.update_console()
 
 # Test
 if __name__ == "__main__":
-	logger = Logger(program_name="WiretappingScaner")
-	print(logger.DEBUG(message_text="Debug data"))
-	print(logger.DEBUG(message_text="Debug data", bold=True))
-	print(logger.DEBUG(message_text="Debug data", italic=True))
-	print(logger.DEBUG(message_text="Debug data", bold=True, italic=True))
-
-
-
-
-	print(logger.DEBUG(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.DEBUG_PERFORMANCE(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.PERFORMANCE(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.EVENT(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
+	buf = TextBuffer(115)
+	logger = Logger(program_name="WiretappingScaner", text_buffer=buf)
+	logger.DEBUG(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.DEBUG_PERFORMANCE(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.PERFORMANCE(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.EVENT(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
 	logger.global_background = True
-	print(logger.AUDIT(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.METRICS(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
+	logger.AUDIT(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.METRICS(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
 	logger.time = False
-	print(logger.USER(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.MESSAGE(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
+	logger.USER(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.MESSAGE(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
 	logger.status_type = False
-	print(logger.INFO(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.NOTICE(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.WARNING(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.ERROR(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.CRITICAL(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	# print(logger.START_PROCESS(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.SUCCESS(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.FAIL(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
+	logger.INFO(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message Test message Test message Test message Test message Test message Test message Test message Test message Test message Test message Test message Test message Test message Test message Test message")
+	logger.NOTICE(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	buf.replace(7, "7")
+	logger.WARNING(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.ERROR(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.CRITICAL(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	# logger.START_PROCESS(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.SUCCESS(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.FAIL(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
 	# print(logger.FAIL(status_message_text="33", message_text="34", invert=True))
+	buf << "55"
+	buf.insert(3, "150")
+	logger.INFO(status_message_text="Test text", message_text="Entrying was successful!", bold=True)
+	buf >> "buf"
 
 	# logger.timeEnabled(False)
 	# print(logger.DEBUG(status_message_text="1", message_text="2"))
```

### Comparing `qt_colored_logger-0.3.0/qt_colored_logger/html_colored_logger.py` & `qt_colored_logger-0.4.0/qt_colored_logger/logger/html_colored_logger.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# ##########################   Qt_Colored-logger   ########################### #
-# ---------------------------------------------------------------------------- #
-#                                                                              #
-# Copyright © 2023 Kalynovsky Valentin. All rights reserved.                   #
-#                                                                              #
-# Licensed under the Apache License, Version 2.0 (the "License");              #
-# you may not use this file except in compliance with the License.             #
-# You may obtain a copy of the License at                                      #
-#                                                                              #
-#     http://www.apache.org/licenses/LICENSE-2.0                               #
-#                                                                              #
-# Unless required by applicable law or agreed to in writing, software          #
-# distributed under the License is distributed on an "AS IS" BASIS,            #
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.     #
-# See the License for the specific language governing permissions and          #
-# limitations under the License.                                               #
-#                                                                              #
-# ---------------------------------------------------------------------------- #
-# ############################################################################ #
+"""
+A module with the implementation of a Qt (HTML) logger.
+\n
+Copyright © 2023 Kalynovsky Valentin. All rights reserved.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
 
 # The idea is taken here:
 # https://github.com/Nakama3942/WiretappingScanner/commit/da5e0e71681b9e1462d5bba5438fc8b1fde8142e
 
-from qt_colored_logger._basic import _Singleton, _BasicLogger, ColorException, CombinationException
-from qt_colored_logger.src import HexColor, Dec2Hex
+from qt_colored_logger.basic.basic_logger import BasicLogger
+from qt_colored_logger.basic.exceptions import ColorException, CombinationException
+from qt_colored_logger.src.color_picker import HexColor, Dec2Hex
+from qt_colored_logger.text.text_buffer import BasicTextBuffer
 
-class LoggerQ(_Singleton, _BasicLogger):
+class LoggerQ(BasicLogger):
 	"""
 	The LoggerQ class is a class that implements the functionality
 	of logging the work of software in different directions.\n
 	It has a color output of information, settings for the operation of the log.
 	Only one class object can be created!!!\n
 	Implements the output of the following information:\n
 	1) Record creation time;
@@ -56,26 +56,28 @@
 	\nAttention: This class in the log entry does not support color inversion!
 	"""
 
 	def __init__(
 			self,
 			*,
 			program_name: str = "Unknown",
+			text_buffer: BasicTextBuffer = BasicTextBuffer(),
 			global_background: bool = False,
 			time: bool = True,
 			status: bool = True,
 			status_message: bool = True,
 			status_type: bool = True,
 			message: bool = True
 	):
 		super().__init__(program_name, time, status, status_message, status_type, message)
+		self._buffer = text_buffer
 		self._HtmlColorSet: dict = {}
 		self._html_color_set_init()
 		self.global_background = global_background
-		# print(self._initial_log())  # todo Перенести в буфер
+		self._initial_log()
 
 	def _html_color_set_init(self):
 		"""
 		Sets the colors of the logger.
 		"""
 		self._HtmlColorSet['INITIAL_COLOR'] = [HexColor('GOLD'), HexColor('INDIGO')]
 		self._HtmlColorSet['INITIAL_BACKGROUND'] = ["", HexColor('GOLD')]
@@ -192,15 +194,16 @@
 		self._HtmlColorSet['FAIL_MESSAGE'] = [HexColor('DARKRED'), HexColor('DARKYELLOW')]
 		self._HtmlColorSet['FAIL_BACKGROUND'] = ["", HexColor('DARKRED')]
 
 	def _initial_log(self):
 		"""
 		Displays initialized information.
 		"""
-		return self._html_initialized_data(  # todo return заменить на buffer
+		self._buffer << "<body style='background-color: #000000; color: #ffffff;'>"
+		self._buffer << self._html_initialized_data(
 			[
 				self._HtmlColorSet['INITIAL_COLOR'][self.global_background],
 				self._HtmlColorSet['INITIAL_BACKGROUND'][self.global_background]
 			]
 		)
 
 	def set_hex_color(self, *, logger_color_name: str, hex_color_value: str, foreground: bool = True, background: bool = False):
@@ -222,16 +225,18 @@
 		:param background: Change background color?
 		"""
 		if logger_color_name in _HtmlColorSet:
 			if background and not foreground:
 				self._HtmlColorSet[logger_color_name][1] = hex_color_value
 			elif background and foreground:
 				self._HtmlColorSet[logger_color_name][1] = hex_color_value
-			else:
+			elif not background and foreground:
 				self._HtmlColorSet[logger_color_name][0] = hex_color_value
+			else:
+				raise CombinationException("False-False combination of foreground-background flags not possible")
 		else:
 			raise ColorException("This color is not in the dictionary")
 
 	def set_color(self, *, logger_color_name: str, color_value: list[int, int, int], foreground: bool = True, background: bool = False):
 		"""
 		A method that sets the decimal RGB list color code in the color table of the logger.
 		May throw a ColorException if the given color is not in the table.
@@ -250,442 +255,458 @@
 		:param background: Change background color?
 		"""
 		if logger_color_name in self._HtmlColorSet:
 			if background and not foreground:
 				self._HtmlColorSet[logger_color_name][1] = Dec2Hex(color_value)
 			elif background and foreground:
 				self._HtmlColorSet[logger_color_name][1] = Dec2Hex(color_value)
-			else:
+			elif not background and foreground:
 				self._HtmlColorSet[logger_color_name][0] = Dec2Hex(color_value)
+			else:
+				raise CombinationException("False-False combination of foreground-background flags not possible")
 		else:
 			raise ColorException("This color is not in the dictionary")
 
-	def DEBUG(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> str:
+	def get_buffer(self):
+		"""
+		Usually, before creating a logger, you need to create a text buffer
+		and pass it to the constructor. But if this has not been done, the buffer
+		is created directly in the logger. And to get it (for example, to save
+		the buffer to a file), this method was implemented. It returns a buffer.
+
+		:return: a text buffer object
+		"""
+		return self._buffer
+
+	def DEBUG(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> None:
 		"""
 		Debugging information logging:
 		Can be used to log entry any information while debugging an application.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_html_entry(
+		self._buffer << self._assemble_html_entry(
 			[
 				self._HtmlColorSet['DEBUG_TIME'][background],
 				self._HtmlColorSet['DEBUG_STATUS'][background],
 				self._HtmlColorSet['DEBUG_STATUS_MESSAGE'][background],
 				self._HtmlColorSet['TYPE_DEBUG'][background],
 				self._HtmlColorSet['DEBUG_MESSAGE'][background],
 				self._HtmlColorSet['DEBUG_BACKGROUND'][background],
 			], status_message_text, "%DEBUG", message_text, bold, italic
 		)
 
-	def DEBUG_PERFORMANCE(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> str:
+	def DEBUG_PERFORMANCE(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> None:
 		"""
 		Performance debugging information logging:
 		Can be used to log entry the execution time of operations or other
 		performance information while the application is being debugged.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_html_entry(
+		self._buffer << self._assemble_html_entry(
 			[
 				self._HtmlColorSet['DEBUG_PERFORMANCE_TIME'][background],
 				self._HtmlColorSet['DEBUG_PERFORMANCE_STATUS'][background],
 				self._HtmlColorSet['DEBUG_PERFORMANCE_STATUS_MESSAGE'][background],
 				self._HtmlColorSet['TYPE_DEBUG_PERFORMANCE'][background],
 				self._HtmlColorSet['DEBUG_PERFORMANCE_MESSAGE'][background],
 				self._HtmlColorSet['DEBUG_PERFORMANCE_BACKGROUND'][background],
 			], status_message_text, "%DEBUG PERFORMANCE", message_text, bold, italic
 		)
 
-	def PERFORMANCE(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> str:
+	def PERFORMANCE(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> None:
 		"""
 		Performance information logging:
 		Can be used to log entry the execution time of operations or
 		other application performance information.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_html_entry(
+		self._buffer << self._assemble_html_entry(
 			[
 				self._HtmlColorSet['PERFORMANCE_TIME'][background],
 				self._HtmlColorSet['PERFORMANCE_STATUS'][background],
 				self._HtmlColorSet['PERFORMANCE_STATUS_MESSAGE'][background],
 				self._HtmlColorSet['TYPE_PERFORMANCE'][background],
 				self._HtmlColorSet['PERFORMANCE_MESSAGE'][background],
 				self._HtmlColorSet['PERFORMANCE_BACKGROUND'][background],
 			], status_message_text, "%PERFORMANCE", message_text, bold, italic
 		)
 
-	def EVENT(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> str:
+	def EVENT(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> None:
 		"""
 		Event information logging:
 		Can be used to log entry specific events in the application,
 		such as button presses or mouse cursor movements.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_html_entry(
+		self._buffer << self._assemble_html_entry(
 			[
 				self._HtmlColorSet['EVENT_TIME'][background],
 				self._HtmlColorSet['EVENT_STATUS'][background],
 				self._HtmlColorSet['EVENT_STATUS_MESSAGE'][background],
 				self._HtmlColorSet['TYPE_EVENT'][background],
 				self._HtmlColorSet['EVENT_MESSAGE'][background],
 				self._HtmlColorSet['EVENT_BACKGROUND'][background],
 			], status_message_text, "~EVENT", message_text, bold, italic
 		)
 
-	def AUDIT(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> str:
+	def AUDIT(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> None:
 		"""
 		Audit information logging:
 		Can be used to log entry changes in the system, such as creating or
 		deleting users, as well as changes in security settings.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_html_entry(
+		self._buffer << self._assemble_html_entry(
 			[
 				self._HtmlColorSet['AUDIT_TIME'][background],
 				self._HtmlColorSet['AUDIT_STATUS'][background],
 				self._HtmlColorSet['AUDIT_STATUS_MESSAGE'][background],
 				self._HtmlColorSet['TYPE_AUDIT'][background],
 				self._HtmlColorSet['AUDIT_MESSAGE'][background],
 				self._HtmlColorSet['AUDIT_BACKGROUND'][background],
 			], status_message_text, "~AUDIT", message_text, bold, italic
 		)
 
-	def METRICS(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> str:
+	def METRICS(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> None:
 		"""
 		Metrics information logging:
 		Can be used to log entry metrics to track application performance and identify issues.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_html_entry(
+		self._buffer << self._assemble_html_entry(
 			[
 				self._HtmlColorSet['METRICS_TIME'][background],
 				self._HtmlColorSet['METRICS_STATUS'][background],
 				self._HtmlColorSet['METRICS_STATUS_MESSAGE'][background],
 				self._HtmlColorSet['TYPE_METRICS'][background],
 				self._HtmlColorSet['METRICS_MESSAGE'][background],
 				self._HtmlColorSet['METRICS_BACKGROUND'][background],
 			], status_message_text, "~METRICS", message_text, bold, italic
 		)
 
-	def USER(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> str:
+	def USER(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> None:
 		"""
 		User information logging:
 		Can be used to log entry custom logs to store additional information
 		that may be useful for diagnosing problems.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_html_entry(
+		self._buffer << self._assemble_html_entry(
 			[
 				self._HtmlColorSet['USER_TIME'][background],
 				self._HtmlColorSet['USER_STATUS'][background],
 				self._HtmlColorSet['USER_STATUS_MESSAGE'][background],
 				self._HtmlColorSet['TYPE_USER'][background],
 				self._HtmlColorSet['USER_MESSAGE'][background],
 				self._HtmlColorSet['USER_BACKGROUND'][background],
 			], status_message_text, "~USER", message_text, bold, italic
 		)
 
-	def MESSAGE(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> str:
+	def MESSAGE(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> None:
 		"""
 		Message information logging:
 		Can be used for the usual output of ordinary messages about the program's operation.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_html_entry(
+		self._buffer << self._assemble_html_entry(
 			[
 				self._HtmlColorSet['MESSAGE_TIME'][background],
 				self._HtmlColorSet['MESSAGE_STATUS'][background],
 				self._HtmlColorSet['MESSAGE_STATUS_MESSAGE'][background],
 				self._HtmlColorSet['TYPE_MESSAGE'][background],
 				self._HtmlColorSet['MESSAGE_MESSAGE'][background],
 				self._HtmlColorSet['MESSAGE_BACKGROUND'][background],
 			], status_message_text, "@MESSAGE", message_text, bold, italic
 		)
 
-	def INFO(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> str:
+	def INFO(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> None:
 		"""
 		Default information logging:
 		Can be used to log entry messages with specific content about the operation of the program.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_html_entry(
+		self._buffer << self._assemble_html_entry(
 			[
 				self._HtmlColorSet['INFO_TIME'][background],
 				self._HtmlColorSet['INFO_STATUS'][background],
 				self._HtmlColorSet['INFO_STATUS_MESSAGE'][background],
 				self._HtmlColorSet['TYPE_INFO'][background],
 				self._HtmlColorSet['INFO_MESSAGE'][background],
 				self._HtmlColorSet['INFO_BACKGROUND'][background],
 			], status_message_text, "@INFO", message_text, bold, italic
 		)
 
-	def NOTICE(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> str:
+	def NOTICE(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = None) -> None:
 		"""
 		Notice information logging:
 		Can be used to flag important events that might be missed with a normal logging level.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		background = local_background if local_background is not None else self.global_background
-		return self._assemble_html_entry(
+		self._buffer << self._assemble_html_entry(
 			[
 				self._HtmlColorSet['NOTICE_TIME'][background],
 				self._HtmlColorSet['NOTICE_STATUS'][background],
 				self._HtmlColorSet['NOTICE_STATUS_MESSAGE'][background],
 				self._HtmlColorSet['TYPE_NOTICE'][background],
 				self._HtmlColorSet['NOTICE_MESSAGE'][background],
 				self._HtmlColorSet['NOTICE_BACKGROUND'][background],
 			], status_message_text, "@NOTICE", message_text, bold, italic
 		)
 
-	def WARNING(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = True) -> str:
+	def WARNING(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = True) -> None:
 		"""
 		Warning information logging:
 		Can be used to log entry warnings that the program may work with unpredictable results.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
-		return self._assemble_html_entry(
+		self._buffer << self._assemble_html_entry(
 			[
 				self._HtmlColorSet['WARNING_TIME'][local_background],
 				self._HtmlColorSet['WARNING_STATUS'][local_background],
 				self._HtmlColorSet['WARNING_STATUS_MESSAGE'][local_background],
 				self._HtmlColorSet['TYPE_WARNING'][local_background],
 				self._HtmlColorSet['WARNING_MESSAGE'][local_background],
 				self._HtmlColorSet['WARNING_BACKGROUND'][local_background],
 			], status_message_text, "!WARNING", message_text, bold, italic
 		)
 
-	def ERROR(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = True) -> str:
+	def ERROR(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = True) -> None:
 		"""
 		Error information logging:
 		Used to log entry errors and crashes in the program.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
-		return self._assemble_html_entry(
+		self._buffer << self._assemble_html_entry(
 			[
 				self._HtmlColorSet['ERROR_TIME'][local_background],
 				self._HtmlColorSet['ERROR_STATUS'][local_background],
 				self._HtmlColorSet['ERROR_STATUS_MESSAGE'][local_background],
 				self._HtmlColorSet['TYPE_ERROR'][local_background],
 				self._HtmlColorSet['ERROR_MESSAGE'][local_background],
 				self._HtmlColorSet['ERROR_BACKGROUND'][local_background],
 			], status_message_text, "!!ERROR", message_text, bold, italic
 		)
 
-	def CRITICAL(self, status_message_text: str = "...", message_text: str = "...", bold: bool = True, italic: bool = False, local_background: bool = True) -> str:
+	def CRITICAL(self, status_message_text: str = "...", message_text: str = "...", bold: bool = True, italic: bool = False, local_background: bool = True) -> None:
 		"""
 		Critical error information logging:
 		Used to log entry for critical and unpredictable program failures.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
-		return self._assemble_html_entry(
+		self._buffer << self._assemble_html_entry(
 			[
 				self._HtmlColorSet['CRITICAL_TIME'][local_background],
 				self._HtmlColorSet['CRITICAL_STATUS'][local_background],
 				self._HtmlColorSet['CRITICAL_STATUS_MESSAGE'][local_background],
 				self._HtmlColorSet['TYPE_CRITICAL'][local_background],
 				self._HtmlColorSet['CRITICAL_MESSAGE'][local_background],
 				self._HtmlColorSet['CRITICAL_BACKGROUND'][local_background],
 			], status_message_text, "!!!@CRITICAL", message_text, bold, italic
 		)
 
-	def START_PROCESS(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = True) -> str:
+	def START_PROCESS(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = True) -> None:
 		"""
 		Stub.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
-		# return self._assemble_html_entry(
+		# self._buffer << self._assemble_html_entry(
 		# 	[
 		# 		self._HtmlColorSet['PROGRESS_TIME'][local_background],
 		# 		self._HtmlColorSet['PROGRESS_STATUS'][local_background],
 		# 		self._HtmlColorSet['PROGRESS_STATUS_MESSAGE'][local_background],
 		# 		self._HtmlColorSet['TYPE_PROGRESS'][local_background],
 		# 		self._HtmlColorSet['PROGRESS_MESSAGE'][local_background],
 		# 		self._HtmlColorSet['PROGRESS_BACKGROUND'][local_background],
 		# 	], status_message_text, "&PROGRESS [*******.............] - 37%", message_text, bold, italic
 		# )
 		pass
 		# Must run on a thread
 
-	def STOP_PROCESS(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = True) -> str:
+	def STOP_PROCESS(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = False, local_background: bool = True) -> None:
 		"""
 		Stub.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
 		pass
 		# Make transition to SUCCESS or FAIL
 
-	def SUCCESS(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = True, local_background: bool = True) -> str:
+	def SUCCESS(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = True, local_background: bool = True) -> None:
 		"""
 		Success information logging:
 		Used to log entry a message about the success of the process.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
-		return self._assemble_html_entry(
+		self._buffer << self._assemble_html_entry(
 			[
 				self._HtmlColorSet['SUCCESS_TIME'][local_background],
 				self._HtmlColorSet['SUCCESS_STATUS'][local_background],
 				self._HtmlColorSet['SUCCESS_STATUS_MESSAGE'][local_background],
 				self._HtmlColorSet['TYPE_SUCCESS'][local_background],
 				self._HtmlColorSet['SUCCESS_MESSAGE'][local_background],
 				self._HtmlColorSet['SUCCESS_BACKGROUND'][local_background],
 			], status_message_text, "&SUCCESS", message_text, bold, italic
 		)
 
-	def FAIL(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = True, local_background: bool = True) -> str:
+	def FAIL(self, status_message_text: str = "...", message_text: str = "...", bold: bool = False, italic: bool = True, local_background: bool = True) -> None:
 		"""
 		Fail information logging:
 		Used to log entry a message about the failed execution of the process.
 
 		:param status_message_text: Log entry status message
 		:param message_text: Log entry message
 		:param bold: Display entry with bold font?
 		:param italic: Display entry with italic font?
 		:param local_background: Display entry with background?
 		:return: the generated log entry string
 		"""
-		return self._assemble_html_entry(
+		self._buffer << self._assemble_html_entry(
 			[
 				self._HtmlColorSet['FAIL_TIME'][local_background],
 				self._HtmlColorSet['FAIL_STATUS'][local_background],
 				self._HtmlColorSet['FAIL_STATUS_MESSAGE'][local_background],
 				self._HtmlColorSet['TYPE_FAIL'][local_background],
 				self._HtmlColorSet['FAIL_MESSAGE'][local_background],
 				self._HtmlColorSet['FAIL_BACKGROUND'][local_background],
 			], status_message_text, "&FAIL", message_text, bold, italic
 		)
 
-
 # Test
 if __name__ == "__main__":
-	logger = LoggerQ(program_name="Test")
-	print(logger._initial_log())
-	print(logger.DEBUG(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.DEBUG_PERFORMANCE(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.PERFORMANCE(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.EVENT(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
+	buf = BasicTextBuffer()
+	logger = LoggerQ(program_name="Test", text_buffer=buf)
+	logger.DEBUG(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.DEBUG_PERFORMANCE(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.PERFORMANCE(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.EVENT(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
 	# logger.global_background = True
-	print(logger.AUDIT(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.METRICS(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
+	logger.AUDIT(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.METRICS(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
 	# logger.time = False
-	print(logger.USER(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.MESSAGE(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
+	logger.USER(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.MESSAGE(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
 	# logger.status_type = False
-	print(logger.INFO(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.NOTICE(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.WARNING(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.ERROR(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.CRITICAL(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	# print(logger.START_PROCESS(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.SUCCESS(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	print(logger.FAIL(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message"))
-	# print(logger.FAIL(status_message_text="33", message_text="34", invert=True))
+	logger.INFO(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.NOTICE(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.WARNING(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.ERROR(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.CRITICAL(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	# logger.START_PROCESS(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.SUCCESS(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	logger.FAIL(status_message_text="Test text", message_text="Test message Test message Test message Test message Test message")
+	# print(logger.FAIL(status_message_text="33", message_text="34", invert=True)
+
+	buf.insert(3, "150<br>")
+	buf >> "2.html"
+	print('\n'.join(buf.get_data()))
 
 	# logger2 = LoggerQ()
 	# print(logger.ID)
 	# print(logger2.ID)
 	# logger.ID = 10
 	# print(logger.ID)
 	# print(logger2.ID)
```

### Comparing `qt_colored_logger-0.3.0/qt_colored_logger/src/color_picker.py` & `qt_colored_logger-0.4.0/qt_colored_logger/src/color_picker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-# ##########################   Qt_Colored-logger   ########################### #
-# ---------------------------------------------------------------------------- #
-#                                                                              #
-# Copyright © 2023 Kalynovsky Valentin. All rights reserved.                   #
-#                                                                              #
-# Licensed under the Apache License, Version 2.0 (the "License");              #
-# you may not use this file except in compliance with the License.             #
-# You may obtain a copy of the License at                                      #
-#                                                                              #
-#     http://www.apache.org/licenses/LICENSE-2.0                               #
-#                                                                              #
-# Unless required by applicable law or agreed to in writing, software          #
-# distributed under the License is distributed on an "AS IS" BASIS,            #
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.     #
-# See the License for the specific language governing permissions and          #
-# limitations under the License.                                               #
-#                                                                              #
-# ---------------------------------------------------------------------------- #
-# ############################################################################ #
+"""
+Module with implementation of colors and their formatter functions.
+\n
+Copyright © 2023 Kalynovsky Valentin. All rights reserved.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
 
-from qt_colored_logger.src import GetAnsiFormat
+from qt_colored_logger.basic.exceptions import ColorException
+from qt_colored_logger.src.ansi_format import GetAnsiFormat
 
 ColorPicker = {
 	# Color table
 	# Original: https://en.wikipedia.org/wiki/Web_colors
 	# Red
 	'MAROON': [128, 0, 0],
 	'DARKRED': [139, 0, 0],
@@ -182,15 +181,14 @@
 
 	:param color_name: Color name
 	:return: Decimal color value
 	"""
 	if color_name in ColorPicker:
 		return ColorPicker[color_name]
 	else:
-		from qt_colored_logger._basic import ColorException
 		raise ColorException("This color is not in the dictionary")
 
 def HexColor(color_name: str) -> str:
 	"""
 	Returns a hexadecimal color value.
 
 	:param color_name: Color name
@@ -288,20 +286,7 @@
 	:return: Hexadecimal color value
 	"""
 	return '{:02x}{:02x}{:02x}'.format(
 		int(ansi_color.split(';')[2]),
 		int(ansi_color.split(';')[3]),
 		int(ansi_color.split(';')[4][:-1])
 	)
-
-# Test
-if __name__ == "__main__":
-	print(DecColor('GREEN'))
-	print(HexColor('GREEN'))
-	print(f"{AnsiColor('GREEN', 'foreground')}Test string")
-
-	print(Dec2Hex([100, 200, 255]))
-	print(Dec2Ansi([100, 200, 255], "foreground").replace('\033', '3'))
-	print(Hex2Dec('7080ea'))
-	print(Hex2Ansi('7080ea', "foreground").replace('\033', '3'))
-	print(Ansi2Dec('\033[38;2;15;19;250m'))
-	print(Ansi2Hex('\033[38;2;15;19;250m'))
```

### Comparing `qt_colored_logger-0.3.0/setup.py` & `qt_colored_logger-0.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,37 +25,40 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name="qt_colored_logger",
-    version="0.3.0",
+    version="0.4.0",
 
     author="Kalynovsky 'Nakama3942' Valentin",
     author_email="nakama3942@gmail.com",
 
     description="Powerful functional logger with support for qt programming",
     long_description=readme,
     long_description_content_type="text/markdown",
 
     url="https://github.com/Nakama3942/qt_colored_logger",
 
     license="Apache License, Version 2.0, see LICENSE file",
 
     packages=[
         'qt_colored_logger',
+        'qt_colored_logger.text',
         'qt_colored_logger.src',
-        'qt_colored_logger._basic'
+        'qt_colored_logger.logger',
+        'qt_colored_logger.basic'
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.11",
         "Topic :: System :: Logging",
     ],
     project_urls={
         'Releases': 'https://github.com/Nakama3942/qt_colored_logger/releases',
     },
+    python_requires='>=3.11',
 )
```

