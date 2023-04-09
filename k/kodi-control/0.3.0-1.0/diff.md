# Comparing `tmp/kodi-control-0.3.0.tar.gz` & `tmp/kodi-control-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodi-control-0.3.0.tar", last modified: Mon Aug 30 00:05:10 2021, max compression
+gzip compressed data, was "kodi-control-1.0.tar", last modified: Sun Apr  9 05:18:12 2023, max compression
```

## Comparing `kodi-control-0.3.0.tar` & `kodi-control-1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ken       (1000) ken       (1001)        0 2021-08-30 00:05:10.213302 kodi-control-0.3.0/
--rw-rw-r--   0 ken       (1000) ken       (1001)     7185 2021-08-30 00:05:10.213302 kodi-control-0.3.0/PKG-INFO
--rw-rw-r--   0 ken       (1000) ken       (1001)     5450 2021-08-30 00:01:33.000000 kodi-control-0.3.0/README.rst
--rwxrwxr-x   0 ken       (1000) ken       (1001)    16373 2021-08-30 00:01:33.000000 kodi-control-0.3.0/kodi-control
-drwxrwxr-x   0 ken       (1000) ken       (1001)        0 2021-08-30 00:05:10.213302 kodi-control-0.3.0/kodi_control.egg-info/
--rw-rw-r--   0 ken       (1000) ken       (1001)     7185 2021-08-30 00:05:10.000000 kodi-control-0.3.0/kodi_control.egg-info/PKG-INFO
--rw-rw-r--   0 ken       (1000) ken       (1001)      211 2021-08-30 00:05:10.000000 kodi-control-0.3.0/kodi_control.egg-info/SOURCES.txt
--rw-rw-r--   0 ken       (1000) ken       (1001)        1 2021-08-30 00:05:10.000000 kodi-control-0.3.0/kodi_control.egg-info/dependency_links.txt
--rw-rw-r--   0 ken       (1000) ken       (1001)       50 2021-08-30 00:05:10.000000 kodi-control-0.3.0/kodi_control.egg-info/requires.txt
--rw-rw-r--   0 ken       (1000) ken       (1001)        1 2021-08-30 00:05:10.000000 kodi-control-0.3.0/kodi_control.egg-info/top_level.txt
--rw-rw-r--   0 ken       (1000) ken       (1001)       38 2021-08-30 00:05:10.213302 kodi-control-0.3.0/setup.cfg
--rw-rw-r--   0 ken       (1000) ken       (1001)      983 2021-08-30 00:01:33.000000 kodi-control-0.3.0/setup.py
+drwx------   0 ken       (1000) ken       (1001)        0 2023-04-09 05:18:12.473833 kodi-control-1.0/
+-rw-------   0 ken       (1000) ken       (1001)     6160 2023-04-09 05:18:12.473833 kodi-control-1.0/PKG-INFO
+-rw-rw-r--   0 ken       (1000) ken       (1001)     5448 2023-04-09 05:13:36.000000 kodi-control-1.0/README.rst
+-rwxrwxr-x   0 ken       (1000) ken       (1001)    16071 2023-04-09 05:13:36.000000 kodi-control-1.0/kodi-control
+drwx------   0 ken       (1000) ken       (1001)        0 2023-04-09 05:18:12.473833 kodi-control-1.0/kodi_control.egg-info/
+-rw-------   0 ken       (1000) ken       (1001)     6160 2023-04-09 05:18:12.000000 kodi-control-1.0/kodi_control.egg-info/PKG-INFO
+-rw-------   0 ken       (1000) ken       (1001)      211 2023-04-09 05:18:12.000000 kodi-control-1.0/kodi_control.egg-info/SOURCES.txt
+-rw-------   0 ken       (1000) ken       (1001)        1 2023-04-09 05:18:12.000000 kodi-control-1.0/kodi_control.egg-info/dependency_links.txt
+-rw-------   0 ken       (1000) ken       (1001)       56 2023-04-09 05:18:12.000000 kodi-control-1.0/kodi_control.egg-info/requires.txt
+-rw-------   0 ken       (1000) ken       (1001)        1 2023-04-09 05:18:12.000000 kodi-control-1.0/kodi_control.egg-info/top_level.txt
+-rw-------   0 ken       (1000) ken       (1001)       38 2023-04-09 05:18:12.473833 kodi-control-1.0/setup.cfg
+-rw-rw-r--   0 ken       (1000) ken       (1001)     1087 2023-04-09 05:13:36.000000 kodi-control-1.0/setup.py
```

### Comparing `kodi-control-0.3.0/PKG-INFO` & `kodi-control-1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,152 +1,151 @@
 Metadata-Version: 2.1
 Name: kodi-control
-Version: 0.3.0
+Version: 1.0
 Summary: interactive tty-based remote control for Kodi
-Home-page: UNKNOWN
-License: UNKNOWN
-Description: Kodi Control — Interactive TTY-based remote control for Kodi
-        ============================================================
-        
-        .. image:: https://pepy.tech/badge/kodi-control/month
-            :target: https://pepy.tech/project/kodi-control
-        
-        .. ignore:
-        
-            ..  image:: https://github.com/KenKundert/kodi-control/actions/workflows/build.yaml/badge.svg
-                :target: https://github.com/KenKundert/kodi-control/actions/workflows/build.yaml
-        
-            .. image:: https://coveralls.io/repos/github/KenKundert/kodi-control/badge.svg?branch=master
-                :target: https://coveralls.io/github/KenKundert/kodi-control?branch=master
-        
-        .. image:: https://img.shields.io/pypi/v/kodi-control.svg
-            :target: https://pypi.python.org/pypi/kodi-control
-        
-        .. image:: https://img.shields.io/pypi/pyversions/kodi-control.svg
-            :target: https://pypi.python.org/pypi/kodi-control/
-        
-        :Author: Ken Kundert
-        :Version: 0.3.0
-        :Released: 2021-08-29
-        
-        *Kodi Control* can be used to control a running instance of *Kodi* from 
-        a terminal.  You can use it to interactively control the app and the players by 
-        opening a terminal and typing individual characters to perform various actions.
-        
-        Getting Started
-        ---------------
-        
-        Install using::
-        
-            pip3 install --user kodi-control
-        
-        Then, you need to create a file containing the settings.  In 
-        ~/.config/kodi-control/settings.nt (a `NestedText <https://nestedtext.org>`_ 
-        file) that takes the following form::
-        
-            hostname: localhost
-            port: 8080
-            username: kodi
-            password: password
-        
-        All the values are optional with the defaults shown (except for password which 
-        is empty by default).
-        
-        Before using *Kodi Control* you must first enable the JSONRPC over HTTP 
-        interface.  To do so, open *Kodi* and navigate to *Settings* → *Services* 
-        → *Control* and enable "Allow remote control via HTTP".  While there you can add 
-        a username and password if desired.  Do not enable SSL.
-        
-        You can run *Kodi Control* on a host different from the one that runs *Kodi*, 
-        you just need to give the hostname for the machine that is running *Kodi*, and 
-        of course that machine must be accessible over the network from the machine 
-        running *Kodi Control*.  In this case, some functionality, such as volume 
-        control and starting and killing *Kodi*, is not available.  Alternately, *Kodi* 
-        can be run locally (best with two screens) or you can open an SSH terminal and 
-        run *Kodi Control* on the *Kodi* host.  In this case all functionality is 
-        available.  To control a remote *Kodi* while using an SSH terminal, you must 
-        specify the name of your display in your ``settings.nt`` file.  The typical 
-        value is ``:0`` or ``:0``, but you can examine your DISPLAY environment variable 
-        and specify whatever it contains::
-        
-            display: :0
-        
-        However you choose to do it, you would start *Kodi Control* in a terminal::
-        
-            > kodi-control
-            Enter desired actions, use 'q' to terminate.
-        
-            Navigation Keys:
-                BS: go back                h: move left
-                ENT: select                j: move down
-                ESC: go to to home screen  k: move up
-                H: go to to home screen    l: move right
-                c: context menu
-        
-            Player Keys:
-                 : toggle play/pause     7: go to 70%             i: show info
-                0: go to 0%              8: go to 80%             n: toggle navigation
-                1: go to 10%             9: go to 90%             p: toggle play/pause
-                2: go to 20%             P: toggle player on top  s: go to start
-                3: go to 30%             T: show subtitles        t: hide subtitles
-                4: go to 40%             b: skip backward         x: stop player
-                5: go to 50%             e: go to end
-                6: go to 60%             f: skip forward
-        
-            Sound Keys:
-                M: temporary mute  m: toggle mute
-                d: volume down     u: volume up
-        
-            Kodi Keys:
-                ': enter text  K: kill kodi   S: start kodi
-        
-        As it starts, it immediately prints a list of available actions.  Then you 
-        simply type individual characters to run the desired action.
-        
-        The temporary mute action (``M``) engages mute for settable number of seconds.  
-        This can be used to turn off the sound during commercials.  Once engaged you 
-        will see a count down with the sound being re-enabled when the count reaches 0.  
-        During the interim all input is ignore except ``ctrl-C`` which immediately 
-        terminates the count-down and immediately re-activates the sound.  You can 
-        specify the duration of the temporary mute with the following setting::
-        
-            temporary mute duration: 30
-        
-        You can specify the path to the *Kodi* executable in your settings file::
-        
-            kodi: kodi-standalone
-        
-        ``kodi`` holds the command used to start *Kodi*.  It can be just the command 
-        name, in which case it must be on your path, or it can be the full path to the 
-        command.  By default it is simply *kodi*.
-        
-        Older versions of *Kodi* have a bug that interferes with proper operation of 
-        forward seeks of less than 60 seconds.  *Kodi Control* works around this issue 
-        if you specify the version number of *Kodi* in the settings file::
-        
-            kodi version: 18.7
-        
-        Currently, the workaround is disabled if the version is 19 or later.
-        
-        If you have any trouble, you can enable the log file and examine it for clues.  
-        To enable the log file, add the following to your settings file::
-        
-            log: yes
-        
-        The log file can then be found at ``~/.local/share/kodi-control/log``.
-        
-        Feel free to post questions or bug report to `GitHub Issues 
-        <https://github.com/KenKundert/kodi-control/issues>`_.
-        
 Keywords: kodi
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+
+Kodi Control — Interactive TTY-based remote control for Kodi
+============================================================
+
+.. image:: https://pepy.tech/badge/kodi-control/month
+    :target: https://pepy.tech/project/kodi-control
+
+.. ignore:
+
+    ..  image:: https://github.com/KenKundert/kodi-control/actions/workflows/build.yaml/badge.svg
+        :target: https://github.com/KenKundert/kodi-control/actions/workflows/build.yaml
+
+    .. image:: https://coveralls.io/repos/github/KenKundert/kodi-control/badge.svg?branch=master
+        :target: https://coveralls.io/github/KenKundert/kodi-control?branch=master
+
+.. image:: https://img.shields.io/pypi/v/kodi-control.svg
+    :target: https://pypi.python.org/pypi/kodi-control
+
+.. image:: https://img.shields.io/pypi/pyversions/kodi-control.svg
+    :target: https://pypi.python.org/pypi/kodi-control/
+
+:Author: Ken Kundert
+:Version: 1.0
+:Released: 2023-04-08
+
+*Kodi Control* can be used to control a running instance of *Kodi* from 
+a terminal.  You can use it to interactively control the app and the players by 
+opening a terminal and typing individual characters to perform various actions.
+
+Getting Started
+---------------
+
+Install using::
+
+    pip3 install --user kodi-control
+
+Then, you need to create a file containing the settings.  In 
+~/.config/kodi-control/settings.nt (a `NestedText <https://nestedtext.org>`_ 
+file) that takes the following form::
+
+    hostname: localhost
+    port: 8080
+    username: kodi
+    password: password
+
+All the values are optional with the defaults shown (except for password which 
+is empty by default).
+
+Before using *Kodi Control* you must first enable the JSONRPC over HTTP 
+interface.  To do so, open *Kodi* and navigate to *Settings* → *Services* 
+→ *Control* and enable "Allow remote control via HTTP".  While there you can add 
+a username and password if desired.  Do not enable SSL.
+
+You can run *Kodi Control* on a host different from the one that runs *Kodi*, 
+you just need to give the hostname for the machine that is running *Kodi*, and 
+of course that machine must be accessible over the network from the machine 
+running *Kodi Control*.  In this case, some functionality, such as volume 
+control and starting and killing *Kodi*, is not available.  Alternately, *Kodi* 
+can be run locally (best with two screens) or you can open an SSH terminal and 
+run *Kodi Control* on the *Kodi* host.  In this case all functionality is 
+available.  To control a remote *Kodi* while using an SSH terminal, you must 
+specify the name of your display in your ``settings.nt`` file.  The typical 
+value is ``:0`` or ``:0``, but you can examine your DISPLAY environment variable 
+and specify whatever it contains::
+
+    display: :0
+
+However you choose to do it, you would start *Kodi Control* in a terminal::
+
+    > kodi-control
+    Enter desired actions, use 'q' to terminate.
+
+    Navigation Keys:
+        BS: go back                h: move left
+        ENT: select                j: move down
+        ESC: go to to home screen  k: move up
+        H: go to to home screen    l: move right
+        c: context menu
+
+    Player Keys:
+         : toggle play/pause     7: go to 70%             i: show info
+        0: go to 0%              8: go to 80%             n: toggle navigation
+        1: go to 10%             9: go to 90%             p: toggle play/pause
+        2: go to 20%             P: toggle player on top  s: go to start
+        3: go to 30%             T: show subtitles        t: hide subtitles
+        4: go to 40%             b: skip backward         x: stop player
+        5: go to 50%             e: go to end
+        6: go to 60%             f: skip forward
+
+    Sound Keys:
+        M: temporary mute  m: toggle mute
+        d: volume down     u: volume up
+
+    Kodi Keys:
+        ': enter text  K: kill kodi   S: start kodi
+
+As it starts, it immediately prints a list of available actions.  Then you 
+simply type individual characters to run the desired action.
+
+The temporary mute action (``M``) engages mute for settable number of seconds.  
+This can be used to turn off the sound during commercials.  Once engaged you 
+will see a count down with the sound being re-enabled when the count reaches 0.  
+During the interim all input is ignore except ``ctrl-C`` which immediately 
+terminates the count-down and immediately re-activates the sound.  You can 
+specify the duration of the temporary mute with the following setting::
+
+    temporary mute duration: 30
+
+You can specify the path to the *Kodi* executable in your settings file::
+
+    kodi: kodi-standalone
+
+``kodi`` holds the command used to start *Kodi*.  It can be just the command 
+name, in which case it must be on your path, or it can be the full path to the 
+command.  By default it is simply *kodi*.
+
+Older versions of *Kodi* have a bug that interferes with proper operation of 
+forward seeks of less than 60 seconds.  *Kodi Control* works around this issue 
+if you specify the version number of *Kodi* in the settings file::
+
+    kodi version: 18.7
+
+Currently, the workaround is disabled if the version is 19 or later.
+
+If you have any trouble, you can enable the log file and examine it for clues.  
+To enable the log file, add the following to your settings file::
+
+    log: yes
+
+The log file can then be found at ``~/.local/share/kodi-control/log``.
+
+Feel free to post questions or bug report to `GitHub Issues 
+<https://github.com/KenKundert/kodi-control/issues>`_.
```

### Comparing `kodi-control-0.3.0/README.rst` & `kodi-control-1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 .. image:: https://img.shields.io/pypi/v/kodi-control.svg
     :target: https://pypi.python.org/pypi/kodi-control
 
 .. image:: https://img.shields.io/pypi/pyversions/kodi-control.svg
     :target: https://pypi.python.org/pypi/kodi-control/
 
 :Author: Ken Kundert
-:Version: 0.3.0
-:Released: 2021-08-29
+:Version: 1.0
+:Released: 2023-04-08
 
 *Kodi Control* can be used to control a running instance of *Kodi* from 
 a terminal.  You can use it to interactively control the app and the players by 
 opening a terminal and typing individual characters to perform various actions.
 
 Getting Started
 ---------------
```

### Comparing `kodi-control-0.3.0/kodi-control` & `kodi-control-1.0/kodi-control`

 * *Files 4% similar despite different names*

```diff
@@ -206,84 +206,77 @@
 
 # ToggleMuteAction {{{2
 class ToggleMuteAction(Action):
 
     def run(self):
         mute()
 
+
 # TemporaryMuteAction {{{2
 class TemporaryMuteAction(Action):
 
     def __init__(self, keys=None, desc=None):
         super().__init__(keys, desc)
 
     def run(self):
         def show(text=''):
             sys.stdout.write('\033[2K\r' + str(text))
             sys.stdout.flush()
 
         mute('1')
         try:
-            display('ctrl-c to cancel.')
             for i in range(temporary_mute_duration, 0, -1):
-                show(i)
+                show(f"ctrl-C to cancel — {i}")
                 sleep(1)
         except KeyboardInterrupt:
             pass
+        show('                      ')
         show()
         mute('0')
 
+
 # VolumeAction {{{2
 class VolumeAction(Action):
     def __init__(self, keys, desc, direction, percent=5):
         super().__init__(keys, desc)
         assert direction in ['+', '-']
         self.direction = direction
         self.percent = percent
 
     def run(self):
-        for sink in get_audio_sinks():
-            Run(f'pactl set-sink-mute {sink} 0', modes='soeW')
-            Run(f'pactl set-sink-volume {sink} {self.direction}{self.percent}%', modes='soeW')
+        Run(f'wpctl set-volume @DEFAULT_AUDIO_SINK@ 1%{self.direction}', modes='soeW')
+
 
 # StartPlayerAction {{{2
 class StartPlayerAction(Action):
     def __init__(self, keys, desc):
         super().__init__(keys, desc)
 
     def run(self):
         Start(kodi_exe, modes='sOEW')
 
+
 # KillPlayerAction {{{2
 class KillPlayerAction(Action):
     def __init__(self, keys, desc):
         super().__init__(keys, desc)
 
     def run(self):
         Run(f'killall {kodi_bin}', modes='soeW')
 
 
 # Utility Functions {{{1
-# get_audio_sinks() {{{2
-def get_audio_sinks():
-    pactl = Run('pactl list sinks', modes='sOeW1')
-    return [
-        l.partition('#')[-1]
-        for l in pactl.stdout.splitlines()
-        if l.startswith('Sink #')
-    ]
-
 # mute() {{{2
 def mute(action=None):
     if not action:
         action = 'toggle'
     assert action in ['0', '1', 'toggle']
-    log(f'muting each available sink:')
-    for sink in get_audio_sinks():
-        Run(f'pactl set-sink-mute {sink} {action}', modes='sOMW')
+    log(f'muting: {action}')
+    Run(f'wpctl set-mute @DEFAULT_AUDIO_SOURCE@ {action}', modes='sOMW')
+
 
 # getch() {{{2
 def getch():
     fd = sys.stdin.fileno()
     old_settings = termios.tcgetattr(fd)
     try:
         tty.setraw(sys.stdin.fileno())
@@ -322,17 +315,16 @@
         for key in keys:
             if key in self.known_keys:
                 error('duplicate key.', culprit=key)
             self.known_keys.add(key)
 
 
 # Globals {{{1
-__version__ = '0.3.0'
-__released__ = '2021-08-29'
-
+__version__ = '1.0'
+__released__ = '2023-04-08'
 
 
 # scale factor {{{2
 class RepeatedKey:
     def __init__(self):
         self.reset()
 
@@ -444,20 +436,20 @@
 all_actions = {}
 for category, actions in categorized_actions.items():
     available = {k:a for a in actions for k in a.keys}
     all_actions.update(available)
     available_actions.extend([
         f'\n{category}:',
         columns(
-            '{}: {}'.format(k, available[k].desc) for k in sorted(available)
+            ('{}: {}'.format(k, available[k].desc) for k in sorted(available)),
+            min_col_width=26, pagewidth=95,
         )
     ])
 available_actions = '\n'.join(available_actions)
 
-
 # Main {{{1
 # read command line {{{2
 cmdline = docopt(__doc__.format(actions=available_actions), version=__version__)
 
 # set up logging to ~/.local/share/kodi-control/log {{{2
 shlib_set_prefs(use_inform=True, log_cmd=True)
 inform = Inform()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kodi-control-0.3.0/kodi_control.egg-info/PKG-INFO` & `kodi-control-1.0/kodi_control.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,152 +1,151 @@
 Metadata-Version: 2.1
 Name: kodi-control
-Version: 0.3.0
+Version: 1.0
 Summary: interactive tty-based remote control for Kodi
-Home-page: UNKNOWN
-License: UNKNOWN
-Description: Kodi Control — Interactive TTY-based remote control for Kodi
-        ============================================================
-        
-        .. image:: https://pepy.tech/badge/kodi-control/month
-            :target: https://pepy.tech/project/kodi-control
-        
-        .. ignore:
-        
-            ..  image:: https://github.com/KenKundert/kodi-control/actions/workflows/build.yaml/badge.svg
-                :target: https://github.com/KenKundert/kodi-control/actions/workflows/build.yaml
-        
-            .. image:: https://coveralls.io/repos/github/KenKundert/kodi-control/badge.svg?branch=master
-                :target: https://coveralls.io/github/KenKundert/kodi-control?branch=master
-        
-        .. image:: https://img.shields.io/pypi/v/kodi-control.svg
-            :target: https://pypi.python.org/pypi/kodi-control
-        
-        .. image:: https://img.shields.io/pypi/pyversions/kodi-control.svg
-            :target: https://pypi.python.org/pypi/kodi-control/
-        
-        :Author: Ken Kundert
-        :Version: 0.3.0
-        :Released: 2021-08-29
-        
-        *Kodi Control* can be used to control a running instance of *Kodi* from 
-        a terminal.  You can use it to interactively control the app and the players by 
-        opening a terminal and typing individual characters to perform various actions.
-        
-        Getting Started
-        ---------------
-        
-        Install using::
-        
-            pip3 install --user kodi-control
-        
-        Then, you need to create a file containing the settings.  In 
-        ~/.config/kodi-control/settings.nt (a `NestedText <https://nestedtext.org>`_ 
-        file) that takes the following form::
-        
-            hostname: localhost
-            port: 8080
-            username: kodi
-            password: password
-        
-        All the values are optional with the defaults shown (except for password which 
-        is empty by default).
-        
-        Before using *Kodi Control* you must first enable the JSONRPC over HTTP 
-        interface.  To do so, open *Kodi* and navigate to *Settings* → *Services* 
-        → *Control* and enable "Allow remote control via HTTP".  While there you can add 
-        a username and password if desired.  Do not enable SSL.
-        
-        You can run *Kodi Control* on a host different from the one that runs *Kodi*, 
-        you just need to give the hostname for the machine that is running *Kodi*, and 
-        of course that machine must be accessible over the network from the machine 
-        running *Kodi Control*.  In this case, some functionality, such as volume 
-        control and starting and killing *Kodi*, is not available.  Alternately, *Kodi* 
-        can be run locally (best with two screens) or you can open an SSH terminal and 
-        run *Kodi Control* on the *Kodi* host.  In this case all functionality is 
-        available.  To control a remote *Kodi* while using an SSH terminal, you must 
-        specify the name of your display in your ``settings.nt`` file.  The typical 
-        value is ``:0`` or ``:0``, but you can examine your DISPLAY environment variable 
-        and specify whatever it contains::
-        
-            display: :0
-        
-        However you choose to do it, you would start *Kodi Control* in a terminal::
-        
-            > kodi-control
-            Enter desired actions, use 'q' to terminate.
-        
-            Navigation Keys:
-                BS: go back                h: move left
-                ENT: select                j: move down
-                ESC: go to to home screen  k: move up
-                H: go to to home screen    l: move right
-                c: context menu
-        
-            Player Keys:
-                 : toggle play/pause     7: go to 70%             i: show info
-                0: go to 0%              8: go to 80%             n: toggle navigation
-                1: go to 10%             9: go to 90%             p: toggle play/pause
-                2: go to 20%             P: toggle player on top  s: go to start
-                3: go to 30%             T: show subtitles        t: hide subtitles
-                4: go to 40%             b: skip backward         x: stop player
-                5: go to 50%             e: go to end
-                6: go to 60%             f: skip forward
-        
-            Sound Keys:
-                M: temporary mute  m: toggle mute
-                d: volume down     u: volume up
-        
-            Kodi Keys:
-                ': enter text  K: kill kodi   S: start kodi
-        
-        As it starts, it immediately prints a list of available actions.  Then you 
-        simply type individual characters to run the desired action.
-        
-        The temporary mute action (``M``) engages mute for settable number of seconds.  
-        This can be used to turn off the sound during commercials.  Once engaged you 
-        will see a count down with the sound being re-enabled when the count reaches 0.  
-        During the interim all input is ignore except ``ctrl-C`` which immediately 
-        terminates the count-down and immediately re-activates the sound.  You can 
-        specify the duration of the temporary mute with the following setting::
-        
-            temporary mute duration: 30
-        
-        You can specify the path to the *Kodi* executable in your settings file::
-        
-            kodi: kodi-standalone
-        
-        ``kodi`` holds the command used to start *Kodi*.  It can be just the command 
-        name, in which case it must be on your path, or it can be the full path to the 
-        command.  By default it is simply *kodi*.
-        
-        Older versions of *Kodi* have a bug that interferes with proper operation of 
-        forward seeks of less than 60 seconds.  *Kodi Control* works around this issue 
-        if you specify the version number of *Kodi* in the settings file::
-        
-            kodi version: 18.7
-        
-        Currently, the workaround is disabled if the version is 19 or later.
-        
-        If you have any trouble, you can enable the log file and examine it for clues.  
-        To enable the log file, add the following to your settings file::
-        
-            log: yes
-        
-        The log file can then be found at ``~/.local/share/kodi-control/log``.
-        
-        Feel free to post questions or bug report to `GitHub Issues 
-        <https://github.com/KenKundert/kodi-control/issues>`_.
-        
 Keywords: kodi
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+
+Kodi Control — Interactive TTY-based remote control for Kodi
+============================================================
+
+.. image:: https://pepy.tech/badge/kodi-control/month
+    :target: https://pepy.tech/project/kodi-control
+
+.. ignore:
+
+    ..  image:: https://github.com/KenKundert/kodi-control/actions/workflows/build.yaml/badge.svg
+        :target: https://github.com/KenKundert/kodi-control/actions/workflows/build.yaml
+
+    .. image:: https://coveralls.io/repos/github/KenKundert/kodi-control/badge.svg?branch=master
+        :target: https://coveralls.io/github/KenKundert/kodi-control?branch=master
+
+.. image:: https://img.shields.io/pypi/v/kodi-control.svg
+    :target: https://pypi.python.org/pypi/kodi-control
+
+.. image:: https://img.shields.io/pypi/pyversions/kodi-control.svg
+    :target: https://pypi.python.org/pypi/kodi-control/
+
+:Author: Ken Kundert
+:Version: 1.0
+:Released: 2023-04-08
+
+*Kodi Control* can be used to control a running instance of *Kodi* from 
+a terminal.  You can use it to interactively control the app and the players by 
+opening a terminal and typing individual characters to perform various actions.
+
+Getting Started
+---------------
+
+Install using::
+
+    pip3 install --user kodi-control
+
+Then, you need to create a file containing the settings.  In 
+~/.config/kodi-control/settings.nt (a `NestedText <https://nestedtext.org>`_ 
+file) that takes the following form::
+
+    hostname: localhost
+    port: 8080
+    username: kodi
+    password: password
+
+All the values are optional with the defaults shown (except for password which 
+is empty by default).
+
+Before using *Kodi Control* you must first enable the JSONRPC over HTTP 
+interface.  To do so, open *Kodi* and navigate to *Settings* → *Services* 
+→ *Control* and enable "Allow remote control via HTTP".  While there you can add 
+a username and password if desired.  Do not enable SSL.
+
+You can run *Kodi Control* on a host different from the one that runs *Kodi*, 
+you just need to give the hostname for the machine that is running *Kodi*, and 
+of course that machine must be accessible over the network from the machine 
+running *Kodi Control*.  In this case, some functionality, such as volume 
+control and starting and killing *Kodi*, is not available.  Alternately, *Kodi* 
+can be run locally (best with two screens) or you can open an SSH terminal and 
+run *Kodi Control* on the *Kodi* host.  In this case all functionality is 
+available.  To control a remote *Kodi* while using an SSH terminal, you must 
+specify the name of your display in your ``settings.nt`` file.  The typical 
+value is ``:0`` or ``:0``, but you can examine your DISPLAY environment variable 
+and specify whatever it contains::
+
+    display: :0
+
+However you choose to do it, you would start *Kodi Control* in a terminal::
+
+    > kodi-control
+    Enter desired actions, use 'q' to terminate.
+
+    Navigation Keys:
+        BS: go back                h: move left
+        ENT: select                j: move down
+        ESC: go to to home screen  k: move up
+        H: go to to home screen    l: move right
+        c: context menu
+
+    Player Keys:
+         : toggle play/pause     7: go to 70%             i: show info
+        0: go to 0%              8: go to 80%             n: toggle navigation
+        1: go to 10%             9: go to 90%             p: toggle play/pause
+        2: go to 20%             P: toggle player on top  s: go to start
+        3: go to 30%             T: show subtitles        t: hide subtitles
+        4: go to 40%             b: skip backward         x: stop player
+        5: go to 50%             e: go to end
+        6: go to 60%             f: skip forward
+
+    Sound Keys:
+        M: temporary mute  m: toggle mute
+        d: volume down     u: volume up
+
+    Kodi Keys:
+        ': enter text  K: kill kodi   S: start kodi
+
+As it starts, it immediately prints a list of available actions.  Then you 
+simply type individual characters to run the desired action.
+
+The temporary mute action (``M``) engages mute for settable number of seconds.  
+This can be used to turn off the sound during commercials.  Once engaged you 
+will see a count down with the sound being re-enabled when the count reaches 0.  
+During the interim all input is ignore except ``ctrl-C`` which immediately 
+terminates the count-down and immediately re-activates the sound.  You can 
+specify the duration of the temporary mute with the following setting::
+
+    temporary mute duration: 30
+
+You can specify the path to the *Kodi* executable in your settings file::
+
+    kodi: kodi-standalone
+
+``kodi`` holds the command used to start *Kodi*.  It can be just the command 
+name, in which case it must be on your path, or it can be the full path to the 
+command.  By default it is simply *kodi*.
+
+Older versions of *Kodi* have a bug that interferes with proper operation of 
+forward seeks of less than 60 seconds.  *Kodi Control* works around this issue 
+if you specify the version number of *Kodi* in the settings file::
+
+    kodi version: 18.7
+
+Currently, the workaround is disabled if the version is 19 or later.
+
+If you have any trouble, you can enable the log file and examine it for clues.  
+To enable the log file, add the following to your settings file::
+
+    log: yes
+
+The log file can then be found at ``~/.local/share/kodi-control/log``.
+
+Feel free to post questions or bug report to `GitHub Issues 
+<https://github.com/KenKundert/kodi-control/issues>`_.
```

