# Comparing `tmp/pytranscoder-ffmpeg-2.2.5.tar.gz` & `tmp/pytranscoder-ffmpeg-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytranscoder-ffmpeg-2.2.5.tar", last modified: Fri Jan 27 04:13:12 2023, max compression
+gzip compressed data, was "pytranscoder-ffmpeg-2.2.6.tar", last modified: Sun Apr  9 17:36:30 2023, max compression
```

## Comparing `pytranscoder-ffmpeg-2.2.5.tar` & `pytranscoder-ffmpeg-2.2.6.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 marshallsmith   (501) _lpoperator   (100)        0 2023-01-27 04:13:12.719814 pytranscoder-ffmpeg-2.2.5/
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)    14467 2023-01-27 04:04:39.000000 pytranscoder-ffmpeg-2.2.5/Cluster.md
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)    35149 2019-03-25 22:56:14.000000 pytranscoder-ffmpeg-2.2.5/LICENSE
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)    29333 2023-01-27 04:13:12.719665 pytranscoder-ffmpeg-2.2.5/PKG-INFO
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)    28502 2023-01-27 04:04:24.000000 pytranscoder-ffmpeg-2.2.5/README.md
-drwxr-xr-x   0 marshallsmith   (501) _lpoperator   (100)        0 2023-01-27 04:13:12.717265 pytranscoder-ffmpeg-2.2.5/config-samples/
--rwx------   0 marshallsmith   (501) _lpoperator   (100)     5239 2022-08-26 02:08:03.000000 pytranscoder-ffmpeg-2.2.5/config-samples/cluster-sample.yml
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)     2392 2022-08-26 02:08:03.000000 pytranscoder-ffmpeg-2.2.5/config-samples/simple.yml
--rwx------   0 marshallsmith   (501) _lpoperator   (100)     9941 2022-08-26 02:08:03.000000 pytranscoder-ffmpeg-2.2.5/config-samples/transcode-sample2.yml
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)     9012 2023-01-27 04:04:39.000000 pytranscoder-ffmpeg-2.2.5/config-samples/transcode.yml
-drwxr-xr-x   0 marshallsmith   (501) _lpoperator   (100)        0 2023-01-27 04:13:12.718730 pytranscoder-ffmpeg-2.2.5/pytranscoder/
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)      240 2023-01-27 04:04:39.000000 pytranscoder-ffmpeg-2.2.5/pytranscoder/__init__.py
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)       59 2019-03-05 22:29:59.000000 pytranscoder-ffmpeg-2.2.5/pytranscoder/__main__.py
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)     5251 2023-01-27 04:04:39.000000 pytranscoder-ffmpeg-2.2.5/pytranscoder/agent.py
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)    43134 2023-01-27 04:04:39.000000 pytranscoder-ffmpeg-2.2.5/pytranscoder/cluster.py
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)     5079 2022-12-17 01:01:38.000000 pytranscoder-ffmpeg-2.2.5/pytranscoder/config.py
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)     4833 2023-01-27 04:04:39.000000 pytranscoder-ffmpeg-2.2.5/pytranscoder/ffmpeg.py
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)    13013 2022-09-23 00:26:49.000000 pytranscoder-ffmpeg-2.2.5/pytranscoder/media.py
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)     2623 2023-01-27 04:04:39.000000 pytranscoder-ffmpeg-2.2.5/pytranscoder/processor.py
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)     6594 2022-08-26 02:09:24.000000 pytranscoder-ffmpeg-2.2.5/pytranscoder/profile.py
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)     2736 2020-09-24 20:58:58.000000 pytranscoder-ffmpeg-2.2.5/pytranscoder/rule.py
--rwxr-xr-x   0 marshallsmith   (501) _lpoperator   (100)    18776 2023-01-27 04:04:39.000000 pytranscoder-ffmpeg-2.2.5/pytranscoder/transcode.py
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)     2214 2020-09-24 20:58:58.000000 pytranscoder-ffmpeg-2.2.5/pytranscoder/utils.py
-drwxr-xr-x   0 marshallsmith   (501) _lpoperator   (100)        0 2023-01-27 04:13:12.719481 pytranscoder-ffmpeg-2.2.5/pytranscoder_ffmpeg.egg-info/
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)    29333 2023-01-27 04:13:12.000000 pytranscoder-ffmpeg-2.2.5/pytranscoder_ffmpeg.egg-info/PKG-INFO
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)      706 2023-01-27 04:13:12.000000 pytranscoder-ffmpeg-2.2.5/pytranscoder_ffmpeg.egg-info/SOURCES.txt
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)        1 2023-01-27 04:13:12.000000 pytranscoder-ffmpeg-2.2.5/pytranscoder_ffmpeg.egg-info/dependency_links.txt
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)       61 2023-01-27 04:13:12.000000 pytranscoder-ffmpeg-2.2.5/pytranscoder_ffmpeg.egg-info/entry_points.txt
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)       20 2023-01-27 04:13:12.000000 pytranscoder-ffmpeg-2.2.5/pytranscoder_ffmpeg.egg-info/requires.txt
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)       13 2023-01-27 04:13:12.000000 pytranscoder-ffmpeg-2.2.5/pytranscoder_ffmpeg.egg-info/top_level.txt
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)       38 2023-01-27 04:13:12.719849 pytranscoder-ffmpeg-2.2.5/setup.cfg
--rw-r--r--   0 marshallsmith   (501) _lpoperator   (100)     1739 2022-08-26 02:19:40.000000 pytranscoder-ffmpeg-2.2.5/setup.py
+drwxr-xr-x   0 mark      (1026) users      (100)        0 2023-04-09 17:36:30.765936 pytranscoder-ffmpeg-2.2.6/
+-rw-r--r--   0 mark      (1026) users      (100)    14467 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/Cluster.md
+-rw-r--r--   0 mark      (1026) users      (100)    35149 2019-03-25 22:56:14.000000 pytranscoder-ffmpeg-2.2.6/LICENSE
+-rw-r--r--   0 mark      (1026) users      (100)    28729 2023-04-09 17:36:30.765936 pytranscoder-ffmpeg-2.2.6/PKG-INFO
+-rw-r--r--   0 mark      (1026) users      (100)    27861 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/README.md
+drwxr-xr-x   0 mark      (1026) users      (100)        0 2023-04-09 17:36:30.765936 pytranscoder-ffmpeg-2.2.6/config-samples/
+-rwxr-xr-x   0 mark      (1026) users      (100)     5239 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/config-samples/cluster-sample.yml
+-rw-r--r--   0 mark      (1026) users      (100)     2392 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/config-samples/simple.yml
+-rwxr-xr-x   0 mark      (1026) users      (100)     9941 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/config-samples/transcode-sample2.yml
+-rw-r--r--   0 mark      (1026) users      (100)     9013 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/config-samples/transcode.yml
+drwxr-xr-x   0 mark      (1026) users      (100)        0 2023-04-09 17:36:30.765936 pytranscoder-ffmpeg-2.2.6/pytranscoder/
+-rw-r--r--   0 mark      (1026) users      (100)      240 2023-04-09 17:00:24.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/__init__.py
+-rw-r--r--   0 mark      (1026) users      (100)       59 2019-03-05 22:29:59.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/__main__.py
+-rw-r--r--   0 mark      (1026) users      (100)     5251 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/agent.py
+-rw-r--r--   0 mark      (1026) users      (100)    41615 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/cluster.py
+-rw-r--r--   0 mark      (1026) users      (100)     3945 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/config.py
+-rw-r--r--   0 mark      (1026) users      (100)     5077 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/ffmpeg.py
+-rw-r--r--   0 mark      (1026) users      (100)    13121 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/media.py
+-rw-r--r--   0 mark      (1026) users      (100)     2623 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/processor.py
+-rw-r--r--   0 mark      (1026) users      (100)    10176 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/profile.py
+-rw-r--r--   0 mark      (1026) users      (100)     2736 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/rule.py
+-rw-r--r--   0 mark      (1026) users      (100)     3741 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/template.py
+-rwxr-xr-x   0 mark      (1026) users      (100)    19074 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/transcode.py
+-rw-r--r--   0 mark      (1026) users      (100)     2218 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/utils.py
+drwxr-xr-x   0 mark      (1026) users      (100)        0 2023-04-09 17:36:30.765936 pytranscoder-ffmpeg-2.2.6/pytranscoder_ffmpeg.egg-info/
+-rw-r--r--   0 mark      (1026) users      (100)    28729 2023-04-09 17:36:30.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder_ffmpeg.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1026) users      (100)      731 2023-04-09 17:36:30.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder_ffmpeg.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1026) users      (100)        1 2023-04-09 17:36:30.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder_ffmpeg.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1026) users      (100)       62 2023-04-09 17:36:30.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder_ffmpeg.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1026) users      (100)       20 2023-04-09 17:36:30.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder_ffmpeg.egg-info/requires.txt
+-rw-r--r--   0 mark      (1026) users      (100)       13 2023-04-09 17:36:30.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder_ffmpeg.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1026) users      (100)       38 2023-04-09 17:36:30.765936 pytranscoder-ffmpeg-2.2.6/setup.cfg
+-rw-r--r--   0 mark      (1026) users      (100)     1739 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/setup.py
```

### Comparing `pytranscoder-ffmpeg-2.2.5/Cluster.md` & `pytranscoder-ffmpeg-2.2.6/Cluster.md`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.5/LICENSE` & `pytranscoder-ffmpeg-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.5/PKG-INFO` & `pytranscoder-ffmpeg-2.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: pytranscoder-ffmpeg
-Version: 2.2.5
+Version: 2.2.6
 Summary: A ffmpeg workflow manager for transcoding
 Home-page: https://github.com/mlsmithjr/transcoder
 Author: Marshall L Smith Jr
 Author-email: marshallsmithjr@gmail.com
+License: UNKNOWN
 Keywords: ffmpeg qsv cuda encode transcode
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
 Classifier: Topic :: Multimedia :: Video :: Conversion
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
@@ -24,21 +26,19 @@
 for automation.
 
 [Read The Docs](https://pytranscoder.readthedocs.io/en/latest/)
 
 
 #### News
 
-**Coming soon** - agent mode!
-That's right.  Due to a few issues around Windows 11 security and WSL2 networking changes I'm adding an agent to this tool so that you can skip the convoluted setup of ssh and exposing network shares on Windows 11.  This is in testing now and will be released after I update the docs.  What this means is you can run pytranscoder in 'agent' mode on any Windows machine without setting up ssh key sharing, hacking the registry to make OpenSSH see network shares, and setting up a proxy to make WSL2 allow ssh address resolution.  You can then use any Windows box as a transcoding agent apart from your main hub.  Of course, the agent will work on linux and macos too.
+**Coming soon**
 
-
-Pytranscoder now supports better profiles.  Existing ones are backward-compatible unless you try to use mixings.
-The mixin feature allows you to create pieces of profiles and combine them into another profile on the commandline at runtime.
-This negates the need to create many unique permutations of a profile just for simple variances.
+Version 3 will include an alternate means of configuring your setup.  Let's face it, all that YAML is confusing.
+The new version will use templating and be far simpler and very much smaller -- all my converted profiles fit on one screen now.
+Existing profile support will remain indefinitely for users with more complicated setups, but templates will appeal more to most users.
 
 
 #### What it is
 This script is intended to help automate transcoding for people encoding lots of video.
 It is more than a wrapper - it is a workflow and job manager.
 
 There are 2 modes: **local** and **clustered**.  Local mode is the most common usage and is for running this script on the same machine where it is installed.  Cluster mode turns pytranscoder into a remote encoding manager.  In this mode it delegates and manages encode jobs running on multiple hosts.  This requires more advanced configuration and is documented separately in [Cluster.md](https://github.com/mlsmithjr/transcoder/blob/master/Cluster.md)
@@ -569,7 +569,9 @@
     hevc_cuda:
       output_options: -c:v hevc_nvenc -profile:v main
       threshold: 18
       extension: ".mkv"
 ```
 Since _output_options_ is a simple string rather than list, pytranscoder doesn't know how to merge them so it doesn't try.  The child values always wins.  So this profile will produce undesirable results because the parent options weren't merged.  Convert both back to lists and it will work again.
 
+
+
```

### Comparing `pytranscoder-ffmpeg-2.2.5/README.md` & `pytranscoder-ffmpeg-2.2.6/pytranscoder_ffmpeg.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,44 @@
+Metadata-Version: 2.1
+Name: pytranscoder-ffmpeg
+Version: 2.2.6
+Summary: A ffmpeg workflow manager for transcoding
+Home-page: https://github.com/mlsmithjr/transcoder
+Author: Marshall L Smith Jr
+Author-email: marshallsmithjr@gmail.com
+License: UNKNOWN
+Keywords: ffmpeg qsv cuda encode transcode
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Environment :: Console
+Classifier: Topic :: Multimedia :: Video :: Conversion
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## pytranscoder
 Python wrapper for ffmpeg for batch, concurrent, or clustered transcoding using defined profiles and optional rules engine
 for automation.
 
 [Read The Docs](https://pytranscoder.readthedocs.io/en/latest/)
 
 
 #### News
 
-**Coming soon** - agent mode!
-That's right.  Due to a few issues around Windows 11 security and WSL2 networking changes I'm adding an agent to this tool so that you can skip the convoluted setup of ssh and exposing network shares on Windows 11.  This is in testing now and will be released after I update the docs.  What this means is you can run pytranscoder in 'agent' mode on any Windows machine without setting up ssh key sharing, hacking the registry to make OpenSSH see network shares, and setting up a proxy to make WSL2 allow ssh address resolution.  You can then use any Windows box as a transcoding agent apart from your main hub.  Of course, the agent will work on linux and macos too.
-
+**Coming soon**
 
-Pytranscoder now supports better profiles.  Existing ones are backward-compatible unless you try to use mixings.
-The mixin feature allows you to create pieces of profiles and combine them into another profile on the commandline at runtime.
-This negates the need to create many unique permutations of a profile just for simple variances.
+Version 3 will include an alternate means of configuring your setup.  Let's face it, all that YAML is confusing.
+The new version will use templating and be far simpler and very much smaller -- all my converted profiles fit on one screen now.
+Existing profile support will remain indefinitely for users with more complicated setups, but templates will appeal more to most users.
 
 
 #### What it is
 This script is intended to help automate transcoding for people encoding lots of video.
 It is more than a wrapper - it is a workflow and job manager.
 
 There are 2 modes: **local** and **clustered**.  Local mode is the most common usage and is for running this script on the same machine where it is installed.  Cluster mode turns pytranscoder into a remote encoding manager.  In this mode it delegates and manages encode jobs running on multiple hosts.  This requires more advanced configuration and is documented separately in [Cluster.md](https://github.com/mlsmithjr/transcoder/blob/master/Cluster.md)
@@ -548,7 +569,9 @@
     hevc_cuda:
       output_options: -c:v hevc_nvenc -profile:v main
       threshold: 18
       extension: ".mkv"
 ```
 Since _output_options_ is a simple string rather than list, pytranscoder doesn't know how to merge them so it doesn't try.  The child values always wins.  So this profile will produce undesirable results because the parent options weren't merged.  Convert both back to lists and it will work again.
 
+
+
```

### Comparing `pytranscoder-ffmpeg-2.2.5/config-samples/cluster-sample.yml` & `pytranscoder-ffmpeg-2.2.6/config-samples/cluster-sample.yml`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.5/config-samples/simple.yml` & `pytranscoder-ffmpeg-2.2.6/config-samples/simple.yml`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.5/config-samples/transcode-sample2.yml` & `pytranscoder-ffmpeg-2.2.6/config-samples/transcode-sample2.yml`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.5/config-samples/transcode.yml` & `pytranscoder-ffmpeg-2.2.6/config-samples/transcode.yml`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         - "-b:v 7M"
         - "-profile:v main"
         - "-maxrate:v 7M"
         - "-c:v hevc_nvenc"
         - "-preset slow"
         - "-pix_fmt yuv420p"
 
-  hevc_cuda
+  hevc_cuda:
     include: "base cuda"
     output_options_video:
       - "-b:v 4000K"
     output_options_audio:
       - "-c:a ac3"
       - "-b:a 768k"
     queue: 'cuda'
```

### Comparing `pytranscoder-ffmpeg-2.2.5/pytranscoder/agent.py` & `pytranscoder-ffmpeg-2.2.6/pytranscoder/agent.py`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.5/pytranscoder/cluster.py` & `pytranscoder-ffmpeg-2.2.6/pytranscoder/cluster.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 import pytranscoder
 
 from pytranscoder import verbose
 from pytranscoder.config import ConfigFile
 from pytranscoder.ffmpeg import FFmpeg
 from pytranscoder.media import MediaInfo
-from pytranscoder.profile import Profile
+from pytranscoder.profile import Directives
 from pytranscoder.utils import filter_threshold, get_local_os_type, calculate_progress, run
 
 
 class RemoteHostProperties:
     name: str
     props: Dict
 
@@ -127,24 +127,29 @@
             print('\n'.join(msg))
             return False
         return True
 
 
 class EncodeJob:
     """One file to be encoded"""
-    inpath:     str
+    inpath: str
     media_info: MediaInfo
-    profile_name: str
+    directive_name: str
 
-    def __init__(self, inpath: str, info: MediaInfo, profile_name: str, mixins: List[str]):
+    def __init__(self, inpath: str, info: MediaInfo, directive: Directives, mixins: Optional[List[str]]):
         self.inpath = os.path.abspath(inpath)
         self.media_info = info
-        self.profile_name = profile_name
+        self.directive = directive
         self.mixins = mixins
 
+    def should_abort(self, pct_comp) -> bool:
+        if self.directive.threshold_check() < 100:
+            return self.directive.threshold_check() <= pct_comp < self.directive.threshold()
+        return False
+
 
 class ManagedHost(Thread):
     """
         Base thread class for all remote host types.
     """
 
     def __init__(self, hostname, props, queue, cluster):
@@ -213,17 +218,17 @@
             self.log(crayons.yellow(f'Host at address {addr} cannot be reached - skipped'))
             return False
         return True
 
     def ssh_test_ok(self):
         try:
             remote_cmd = 'dir' if self.props.is_windows() else 'ls'
-            #remote_cmd = 'ls'
+            # remote_cmd = 'ls'
             sshtest = subprocess.run([*self.ssh_cmd(), remote_cmd], stdout=subprocess.PIPE, stderr=subprocess.PIPE,
-                                     shell=False, timeout=5)
+                                     shell=False, timeout=10)
             if sshtest.returncode != 0:
                 self.log('ssh test failed with the following output: ' + str(sshtest.stderr))
                 return False
             return True
         except subprocess.TimeoutExpired:
             return False
 
@@ -234,23 +239,23 @@
         p = subprocess.run(*args)
         if self._manager.verbose:
             self.log(' '.join(*args))
             if p.returncode != 0:
                 self.log(p.stderr)
         return p
 
-    def match_profile(self, job: EncodeJob, name: str) -> Optional[Profile]:
-        if job.profile_name is None:
-            rule = self.configfile.match_rule(job.media_info, restrict_profiles=self.props.profiles)
-            if rule is None:
-                self.log(crayons.yellow(
-                    f'Failed to match rule/profile for host {name} for file {job.inpath} - skipped'))
-                return None
-            job.profile_name = rule.profile
-        return self._manager.profiles[job.profile_name]
+    # def match_profile(self, job: EncodeJob, name: str) -> Optional[Profile]:
+    #     if job.directive_name is None:
+    #         rule = self.configfile.match_rule(job.media_info, restrict_profiles=self.props.profiles)
+    #         if rule is None:
+    #             self.log(crayons.yellow(
+    #                 f'Failed to match rule/profile for host {name} for file {job.inpath} - skipped'))
+    #             return None
+    #         job.directive_name = rule.profile
+    #     return self._manager.profiles[job.directive_name]
 
     def terminate(self):
         pass
 
 
 class AgentManagedHost(ManagedHost):
     """Implementation of a agent host worker thread"""
@@ -276,71 +281,58 @@
     def go(self):
 
         while not self.queue.empty():
             try:
                 job: EncodeJob = self.queue.get()
                 inpath = job.inpath
 
-
-                #
-                # Got to do the rule matching again.
-                # This time we narrow down the available profiles based on host definition
-                #
-                if pytranscoder.verbose:
-                    self.log('matching ' + inpath)
-
-                _profile: Profile = self.match_profile(job, self.name)
-                if _profile is None:
-                    continue
-
                 #
                 # build command line
                 #
 
-                oinput = _profile.input_options.as_shell_params()
-                ooutput = self._manager.config.output_from_profile(_profile, job.mixins)
-
                 remote_inpath = inpath
 
-                if job.media_info.is_multistream() and self.configfile.automap and _profile.automap:
-                    ooutput = ooutput + job.media_info.ffmpeg_streams(_profile)
-                cmd = [self.props.ffmpeg_path, '-y', *oinput, '-i', '{FILENAME}', *ooutput]
+                stream_map = []
+                if job.media_info.is_multistream() and self._manager.config.automap:
+                    stream_map = job.directive.stream_map(job.media_info.stream, job.media_info.audio,
+                                                          job.media_info.subtitle)
+
+                cmd = [self.props.ffmpeg_path, '-y', *job.directive.input_options_list(), '-i', '{FILENAME}',
+                       *job.directive.output_options_list(self._manager.config, job.mixins), *stream_map]
 
                 #
                 # display useful information
                 #
                 self.lock.acquire()
                 try:
                     print('-' * 40)
                     print(f'Host     : {self.hostname} (agent)')
                     print('Filename : ' + crayons.green(os.path.basename(remote_inpath)))
-                    print(f'Profile  : {_profile.name}')
+                    print(f'Directive: {job.directive.name()}')
                     print('Command  : ' + ' '.join(cmd) + '\n')
                 finally:
                     self.lock.release()
 
                 if pytranscoder.dry_run:
                     continue
 
                 basename = os.path.basename(job.inpath)
 
                 def log_callback(stats):
                     pct_done, pct_comp = calculate_progress(job.media_info, stats)
-                    pytranscoder.status_queue.put({ 'host': self.hostname,
-                                                    'file': basename,
-                                                    'speed': stats['speed'],
-                                                    'comp': pct_comp,
-                                                    'done': pct_done})
-
-                    if _profile.threshold_check < 100:
-                        if pct_done >= _profile.threshold_check and pct_comp < _profile.threshold:
-                            # compression goal (threshold) not met, kill the job and waste no more time...
-                            self.log(f'Encoding of {basename} cancelled and skipped due to threshold not met')
-                            return True
-                    # continue
+                    pytranscoder.status_queue.put({'host': self.hostname,
+                                                   'file': basename,
+                                                   'speed': stats['speed'],
+                                                   'comp': pct_comp,
+                                                   'done': pct_done})
+
+                    if job.should_abort(pct_done):
+                        # compression goal (threshold) not met, kill the job and waste no more time...
+                        self.log(f'Encoding of {basename} cancelled and skipped due to threshold not met')
+                        return True
                     return False
 
                 #
                 # Send to agent
                 #
                 s = socket.socket()
 
@@ -454,51 +446,42 @@
                 #
                 # Convert escaped spaces back to normal. Typical for bash to escape spaces and special characters
                 # in filenames.
                 #
                 inpath = inpath.replace('\\ ', ' ')
 
                 #
-                # Got to do the rule matching again.
-                # This time we narrow down the available profiles based on host definition
-                #
-                _profile: Profile = self.match_profile(job, self.name)
-                if _profile is None:
-                    continue
-
-                #
                 # calculate full input and output paths
                 #
                 remote_working_dir = self.props.working_dir
                 remote_inpath = os.path.join(remote_working_dir, os.path.basename(inpath))
                 remote_outpath = os.path.join(remote_working_dir, os.path.basename(inpath) + '.tmp')
 
                 #
                 # build remote commandline
                 #
-                oinput = _profile.input_options.as_shell_params()
-                ooutput = self._manager.config.output_from_profile(_profile, job.mixins)
-#                ooutput = _profile.output_options.as_shell_params()
-
-                if job.media_info.is_multistream() and self.configfile.automap and _profile.automap:
-                    ooutput = ooutput + job.media_info.ffmpeg_streams(_profile)
-                cmd = ['-y', *oinput, '-i', self.converted_path(remote_inpath),
-                       *ooutput, self.converted_path(remote_outpath)]
-
+                stream_map = []
+                if job.media_info.is_multistream() and self._manager.config.automap:
+                    stream_map = job.directive.stream_map(job.media_info.stream, job.media_info.audio,
+                                                          job.media_info.subtitle)
+
+                cmd = ['-y', *job.directive.input_options_list(), '-i', self.converted_path(remote_inpath),
+                       *job.directive.output_options_list(self._manager.config, job.mixins), *stream_map,
+                       self.converted_path(remote_outpath)]
                 cli = [*ssh_cmd, *cmd]
 
                 #
                 # display useful information
                 #
                 self.lock.acquire()  # used to synchronize threads so multiple threads don't create a jumble of output
                 try:
                     print('-' * 40)
                     print(f'Host     : {self.hostname} (streaming)')
                     print('Filename : ' + crayons.green(os.path.basename(remote_inpath)))
-                    print(f'Profile  : {job.profile_name}')
+                    print(f'Directive: {job.directive.name()}')
                     print('ssh      : ' + ' '.join(cli) + '\n')
                 finally:
                     self.lock.release()
 
                 if pytranscoder.dry_run:
                     continue
 
@@ -520,38 +503,35 @@
                         self.log(output)
                     continue
 
                 basename = os.path.basename(job.inpath)
 
                 def log_callback(stats):
                     pct_done, pct_comp = calculate_progress(job.media_info, stats)
-                    pytranscoder.status_queue.put({ 'host': self.hostname,
-                                                    'file': basename,
-                                                    'speed': stats['speed'],
-                                                    'comp': pct_comp,
-                                                    'done': pct_done})
-#                    self.log(f'{basename}: speed: {stats["speed"]}x, comp: {pct_comp}%, done: {pct_done:3}%')
-                    if _profile.threshold_check < 100:
-                        if pct_done >= _profile.threshold_check and pct_comp < _profile.threshold:
-                            # compression goal (threshold) not met, kill the job and waste no more time...
-                            self.log(f'Encoding of {basename} cancelled and skipped due to threshold not met')
-                            return True
-                    # continue
+                    pytranscoder.status_queue.put({'host': self.hostname,
+                                                   'file': basename,
+                                                   'speed': stats['speed'],
+                                                   'comp': pct_comp,
+                                                   'done': pct_done})
+                    if job.should_abort(pct_done):
+                        # compression goal (threshold) not met, kill the job and waste no more time...
+                        self.log(f'Encoding of {basename} cancelled and skipped due to threshold not met')
+                        return True
                     return False
 
                 #
                 # Start remote
                 #
                 job_start = datetime.datetime.now()
                 code = self.ffmpeg.run_remote(self._manager.ssh, self.props.user, self.props.ip, cmd, log_callback)
                 job_stop = datetime.datetime.now()
 
-#                if code != 0:
-#                    self.log(crayons.red('Unknown error encoding on remote'))
-#                    continue
+                #                if code != 0:
+                #                    self.log(crayons.red('Unknown error encoding on remote'))
+                #                    continue
 
                 #
                 # copy results back to local
                 #
                 retrieved_copy_name = os.path.join(gettempdir(), os.path.basename(remote_outpath))
                 cmd = ['scp', self.props.user + '@' + self.props.ip + ':' + remote_outpath, retrieved_copy_name]
                 self.log(' '.join(cmd))
@@ -564,15 +544,15 @@
                 if code is None:
                     # was vetoed by threshold checker, clean up
                     self.complete(inpath, (job_stop - job_start).seconds)
                     os.remove(retrieved_copy_name)
                     continue
 
                 if code == 0:
-                    if not filter_threshold(_profile, inpath, retrieved_copy_name):
+                    if not filter_threshold(job.directive, inpath, retrieved_copy_name):
                         self.log(
                             f'Transcoded file {inpath} did not meet minimum savings threshold, skipped')
                         self.complete(inpath, (job_stop - job_start).seconds)
                         os.remove(retrieved_copy_name)
                         continue
                     self.complete(inpath, (job_stop - job_start).seconds)
 
@@ -586,21 +566,23 @@
                 elif code is not None:
                     self.log(crayons.red(f'error during remote transcode of {inpath}'))
                     self.log(f' Did not complete normally: {self.ffmpeg.last_command}')
                     self.log(f'Output can be found in {self.ffmpeg.log_path}')
 
                 # self.log(f'Removing temporary media copies from {remote_working_dir}')
                 if self.props.is_windows():
-#                    remote_outpath = self.converted_path(remote_outpath)
-#                    remote_inpath = self.converted_path(remote_inpath)
+                    #                    remote_outpath = self.converted_path(remote_outpath)
+                    #                    remote_inpath = self.converted_path(remote_inpath)
+                    remote_outpath = remote_outpath.replace("/", "\\")
+                    remote_inpath = remote_inpath.replace("/", "\\")
                     if get_local_os_type() == "linux":
                         remote_outpath = remote_outpath.replace(r"\\", "\\")
                         remote_inpath = remote_inpath.replace(r"\\", "\\")
-                    self.run_process([*ssh_cmd, f'del {remote_outpath}'])
-                    self.run_process([*ssh_cmd, f'del {remote_inpath}'])
+                    self.run_process([*ssh_cmd, f'del "{remote_outpath}"'])
+                    self.run_process([*ssh_cmd, f'del "{remote_inpath}"'])
                 else:
                     self.run_process([*ssh_cmd, f'"rm {remote_outpath}"'])
                     self.run_process([*ssh_cmd, f'"rm {remote_inpath}"'])
 
             finally:
                 self.queue.task_done()
 
@@ -627,86 +609,71 @@
     def go(self):
 
         while not self.queue.empty():
             try:
                 job: EncodeJob = self.queue.get()
                 inpath = job.inpath
 
-
-                #
-                # Got to do the rule matching again.
-                # This time we narrow down the available profiles based on host definition
-                #
-                if pytranscoder.verbose:
-                    self.log('matching ' + inpath)
-
-                _profile: Profile = self.match_profile(job, self.name)
-                if _profile is None:
-                    continue
-
                 #
                 # calculate paths
                 #
-                outpath = inpath[0:inpath.rfind('.')] + _profile.extension + '.tmp'
+                outpath = inpath[0:inpath.rfind('.')] + job.directive.extension() + '.tmp'
                 remote_inpath = inpath
                 remote_outpath = outpath
                 if self.props.has_path_subst:
                     #
                     # fix the input path to match what the remote machine expects
                     #
                     remote_inpath, remote_outpath = self.props.substitute_paths(inpath, outpath)
 
                 #
                 # build command line
                 #
-
-                oinput = _profile.input_options.as_shell_params()
-                ooutput = self._manager.config.output_from_profile(_profile, job.mixins)
-#                ooutput = _profile.output_options.as_shell_params()
-
                 remote_inpath = self.converted_path(remote_inpath)
                 remote_outpath = self.converted_path(remote_outpath)
 
-                if job.media_info.is_multistream() and self.configfile.automap and _profile.automap:
-                    ooutput = ooutput + job.media_info.ffmpeg_streams(_profile)
-                cmd = ['-y', *oinput, '-i', f'"{remote_inpath}"', *ooutput, f'"{remote_outpath}"']
+                stream_map = []
+                if job.media_info.is_multistream() and self._manager.config.automap:
+                    stream_map = job.directive.stream_map(job.media_info.stream, job.media_info.audio,
+                                                          job.media_info.subtitle)
+                cmd = ['-y', *job.directive.input_options_list(), '-i', f'"{remote_inpath}"',
+                       *job.directive.output_options_list(self._manager.config, job.mixins), *stream_map,
+                       f'"{remote_outpath}"']
 
                 #
                 # display useful information
                 #
                 self.lock.acquire()
                 try:
                     print('-' * 40)
                     print(f'Host     : {self.hostname} (mounted)')
                     print('Filename : ' + crayons.green(os.path.basename(remote_inpath)))
-                    print(f'Profile  : {_profile.name}')
+
+                    print(f'Directive: {job.directive.name()}')
                     print('ssh      : ' + ' '.join(cmd) + '\n')
                 finally:
                     self.lock.release()
 
                 if pytranscoder.dry_run:
                     continue
 
                 basename = os.path.basename(job.inpath)
 
                 def log_callback(stats):
                     pct_done, pct_comp = calculate_progress(job.media_info, stats)
-                    pytranscoder.status_queue.put({ 'host': self.hostname,
-                                                    'file': basename,
-                                                    'speed': stats['speed'],
-                                                    'comp': pct_comp,
-                                                    'done': pct_done})
-
-#                    self.log(f'{basename}: speed: {stats["speed"]}x, comp: {pct_comp}%, done: {pct_done:3}%')
-                    if _profile.threshold_check < 100:
-                        if pct_done >= _profile.threshold_check and pct_comp < _profile.threshold:
-                            # compression goal (threshold) not met, kill the job and waste no more time...
-                            self.log(f'Encoding of {basename} cancelled and skipped due to threshold not met')
-                            return True
-                    # continue
+                    pytranscoder.status_queue.put({'host': self.hostname,
+                                                   'file': basename,
+                                                   'speed': stats['speed'],
+                                                   'comp': pct_comp,
+                                                   'done': pct_done})
+
+                    if job.should_abort(pct_done):
+                        # compression goal (threshold) not met, kill the job and waste no more time...
+                        self.log(f'Encoding of {basename} cancelled and skipped due to threshold not met')
+                        return True
                     return False
 
                 #
                 # Start remote
                 #
                 job_start = datetime.datetime.now()
                 code = self.ffmpeg.run_remote(self._manager.ssh, self.props.user, self.props.ip, cmd, log_callback)
@@ -718,15 +685,15 @@
                 if code is None:
                     # was vetoed by threshold checker, clean up
                     self.complete(inpath, (job_stop - job_start).seconds)
                     os.remove(outpath)
                     continue
 
                 if code == 0:
-                    if not filter_threshold(_profile, inpath, outpath):
+                    if not filter_threshold(job.directive, inpath, outpath):
                         self.log(
                             f'Transcoded file {inpath} did not meet minimum savings threshold, skipped')
                         self.complete(inpath, (job_stop - job_start).seconds)
                         os.remove(outpath)
                         continue
 
                     if not pytranscoder.keep_source:
@@ -775,74 +742,62 @@
 
         while not self.queue.empty():
             try:
                 job: EncodeJob = self.queue.get()
                 inpath = job.inpath
 
                 #
-                # Got to do the rule matching again.
-                # This time we narrow down the available profiles based on host definition
-                #
-                if pytranscoder.verbose:
-                    self.log('matching ' + inpath)
-
-                _profile: Profile = self.match_profile(job, self.name)
-                if _profile is None:
-                    continue
-                #
                 # calculate paths
                 #
-                outpath = inpath[0:inpath.rfind('.')] + _profile.extension + '.tmp'
+                outpath = inpath[0:inpath.rfind('.')] + job.directive.extension() + '.tmp'
 
                 #
                 # build command line
                 #
-                oinput = _profile.input_options.as_shell_params()
-                ooutput = self._manager.config.output_from_profile(_profile, job.mixins)
-#                ooutput = _profile.output_options.as_shell_params()
-
                 remote_inpath = self.converted_path(inpath)
                 remote_outpath = self.converted_path(outpath)
 
-                if job.media_info.is_multistream() and self.configfile.automap and _profile.automap:
-                    ooutput = ooutput + job.media_info.ffmpeg_streams(_profile)
-                cli = ['-y', *oinput, '-i', remote_inpath, *ooutput, remote_outpath]
+                stream_map = []
+                if job.media_info.is_multistream() and self._manager.config.automap:
+                    stream_map = job.directive.stream_map(job.media_info.stream, job.media_info.audio,
+                                                          job.media_info.subtitle)
+                cli = ['-y', *job.directive.input_options_list(), '-i', remote_inpath,
+                       *job.directive.output_options_list(self._manager.config, job.mixins), *stream_map,
+                       remote_outpath]
 
                 #
                 # display useful information
                 #
                 self.lock.acquire()  # used to synchronize threads so multiple threads don't create a jumble of output
                 try:
                     print('-' * 40)
                     print(f'Host     : {self.hostname} (local)')
                     print('Filename : ' + crayons.green(os.path.basename(remote_inpath)))
-                    print(f'Profile  : {_profile.name}')
+                    print(f'Directive: {job.directive.name()}')
                     print('ffmpeg   : ' + ' '.join(cli) + '\n')
                 finally:
                     self.lock.release()
 
                 if pytranscoder.dry_run:
                     continue
 
                 basename = os.path.basename(job.inpath)
 
                 def log_callback(stats):
                     pct_done, pct_comp = calculate_progress(job.media_info, stats)
-                    pytranscoder.status_queue.put({ 'host': 'local',
-                                                    'file': basename,
-                                                    'speed': stats['speed'],
-                                                    'comp': pct_comp,
-                                                    'done': pct_done})
-
-#                    self.log(f'{basename}: speed: {stats["speed"]}x, comp: {pct_comp}%, done: {pct_done:3}%')
-                    if _profile.threshold_check < 100:
-                        if pct_done >= _profile.threshold_check and pct_comp < _profile.threshold:
-                            # compression goal (threshold) not met, kill the job and waste no more time...
-                            self.log(f'Encoding of {basename} cancelled and skipped due to threshold not met')
-                            return True
+                    pytranscoder.status_queue.put({'host': 'local',
+                                                   'file': basename,
+                                                   'speed': stats['speed'],
+                                                   'comp': pct_comp,
+                                                   'done': pct_done})
+
+                    if job.should_abort(pct_done):
+                        # compression goal (threshold) not met, kill the job and waste no more time...
+                        self.log(f'Encoding of {basename} cancelled and skipped due to threshold not met')
+                        return True
                     return False
 
                 #
                 # Start process
                 #
                 job_start = datetime.datetime.now()
                 code = self.ffmpeg.run(cli, log_callback)
@@ -854,15 +809,15 @@
                 if code is None:
                     # was vetoed by threshold checker, clean up
                     self.complete(inpath, (job_stop - job_start).seconds)
                     os.remove(outpath)
                     continue
 
                 if code == 0:
-                    if not filter_threshold(_profile, inpath, outpath):
+                    if not filter_threshold(job.directive, inpath, outpath):
                         self.log(
                             f'Transcoded file {inpath} did not meet minimum savings threshold, skipped')
                         self.complete(inpath, (job_stop - job_start).seconds)
                         os.remove(outpath)
                         continue
 
                     if not pytranscoder.keep_source:
@@ -887,15 +842,15 @@
             finally:
                 self.queue.task_done()
 
 
 class Cluster(Thread):
     """Thread to create host threads and wait for their completion."""
 
-    terminal_lock:  Lock = Lock()       # class-level
+    terminal_lock: Lock = Lock()  # class-level
 
     def __init__(self, name, configs: Dict, config: ConfigFile, ssh: str):
         """
         :param name:        Cluster name, used only for thread naming
         :param configs:     The "clusters" section of the global config
         :param config:      The full configuration object
         :param ssh:         Path to local ssh
@@ -970,15 +925,15 @@
                         if not _h.validate_settings():
                             sys.exit(1)
                         self.hosts.append(_h)
 
             else:
                 print(crayons.red(f'Unknown cluster host type "{hosttype}" - skipping'))
 
-    def enqueue(self, file, forced_profile: Optional[str]) -> (str, Optional[EncodeJob]):
+    def enqueue(self, file, forced_directive: Optional[str]) -> (str, Optional[EncodeJob]):
         """Add a media file to this cluster queue.
            This is different than in local mode in that we only care about handling skips here.
            The profile will be selected once a host is assigned to the work
         """
 
         path = os.path.abspath(file)  # convert to full path so that rule filtering can work
         if pytranscoder.verbose:
@@ -986,46 +941,50 @@
 
         media_info = self.ffmpeg.fetch_details(path)
 
         if media_info is None:
             print(crayons.red(f'File not found: {path}'))
             return None, None
         if media_info.valid:
+            directive = None
 
             if pytranscoder.verbose:
                 print(str(media_info))
 
-            if forced_profile is None:
+            if forced_directive is None:
                 #
                 # just interested in SKIP rule matches and queue designations here
                 #
 
-                profile = None
                 rule = self.config.match_rule(media_info)
                 if rule is None:
                     print(crayons.yellow(f'No matching profile found - skipped'))
                     return None, None
                 if rule.is_skip():
                     basename = os.path.basename(path)
                     print(f'{basename}: Skipping due to profile rule - {rule.name}')
                     return None, None
-                profile = self.profiles[rule.profile]
+                directive = self.directives[rule.profile]
             else:
-                profile = self.profiles[forced_profile]
+                if forced_directive in self.directives:
+                    directive = self.directives[forced_directive]
+                else:
+                    print(f"{forced_directive} not found")
+                    return None, None
 
             if pytranscoder.verbose:
-                print(f"Matched to profile {profile.name}")
+                print(f"Matched to profile {directive.name()}")
 
             # not short circuited by a skip rule, add to appropriate queue
-            queue_name = profile.queue_name if profile.queue_name is not None else '_default'
+            queue_name = directive.queue_name() if directive.queue_name() is not None else '_default'
             if queue_name not in self.queues:
                 print(crayons.red('Error: ') +
-                      f'Queue "{queue_name}" referenced in profile "{profile.name}" not defined in any host')
+                      f'Queue "{queue_name}" referenced in "{directive.name()}" not defined in any host')
                 exit(1)
-            job = EncodeJob(file, media_info, profile.name, None)
+            job = EncodeJob(file, media_info, directive, None)
             self.queues[queue_name].put(job)
             return queue_name, job
         return None, None
 
     def testrun(self):
         for host in self.hosts:
             host.testrun()
@@ -1046,16 +1005,16 @@
             self.completed.extend(host.completed)
 
     def terminate(self):
         for host in self.hosts:
             host.terminate()
 
     @property
-    def profiles(self):
-        return self.config.profiles
+    def directives(self):
+        return self.config.directives
 
 
 def manage_clusters(files, config: ConfigFile, testing=False) -> List:
     """Main entry point for setup and execution of all clusters
 
         There is one thread per cluster, and each cluster manages multiple hosts, each having their own thread.
     """
@@ -1112,11 +1071,11 @@
                 for _, cluster in clusters.items():
                     if cluster.is_alive():
                         busy = True
 
         #
         # wait for each cluster thread to complete
         #
-#        for _, cluster in clusters.items():
-#            cluster.join()
-#            completed.extend(cluster.completed)
+    #        for _, cluster in clusters.items():
+    #            cluster.join()
+    #            completed.extend(cluster.completed)
     return completed
```

### Comparing `pytranscoder-ffmpeg-2.2.5/pytranscoder/ffmpeg.py` & `pytranscoder-ffmpeg-2.2.6/pytranscoder/ffmpeg.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,25 +81,34 @@
                         hh, mm, ss = info['time'].split(':')
                         ss = ss.split('.')[0]
                         info['time'] = (int(hh) * 3600) + (int(mm) * 60) + int(ss)
                         yield info
 
         if proc.returncode == 0:
             # if we got here then everything went fine, so remove the transaction log
-            os.remove(str(self.log_path))
+            try:
+                os.remove(str(self.log_path))
+            except Exception:
+                pass
             self.log_path = None
 
     def monitor_agent(self, sock):
         diff = datetime.timedelta(seconds=self.monitor_interval)
         event = datetime.datetime.now() + diff
         while True:
             c = sock.recv(1024).decode()
             if c.startswith("DONE|") or c.startswith("ERR|"):
                 print("Transcode complete, receiving results..")
                 # found end of processing marker
+                try:
+                    os.remove(str(self.log_path))
+                    self.log_path = None
+                except Exception:
+                    pass
+
                 yield c
 
             sock.send(bytes("ACK!".encode()))
             line = c
 
             match = status_re.match(line)
             if match is not None and len(match.groups()) >= 5:
```

### Comparing `pytranscoder-ffmpeg-2.2.5/pytranscoder/media.py` & `pytranscoder-ffmpeg-2.2.6/pytranscoder/media.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,84 +37,84 @@
 
     def __str__(self):
         runtime = "{:0>8}".format(str(timedelta(seconds=self.runtime)))
         audios = [a['stream'] + ':' + a['lang'] + ':' + a['format'] + ':' + a['default'] for a in self.audio]
         audio = '(' + ','.join(audios) + ')'
         subs = [s['stream'] + ':' + s['lang'] + ':' + s['default'] for s in self.subtitle]
         sub = '(' + ','.join(subs) + ')'
-        buf = f"MediaInfo: {self.path}, {self.filesize_mb}mb, {self.fps} fps, cs={self.colorspace}, {self.res_width}x{self.res_height}, {runtime}, c:v={self.vcodec}, audio={audio}, sub={sub}"
+        buf = f"{self.path}, {self.filesize_mb}mb, {self.fps} fps, {self.res_width}x{self.res_height}, {runtime}, {self.vcodec}, audio={audio}, sub={sub}"
         return buf
 
     def is_multistream(self) -> bool:
         return len(self.audio) > 1 or len(self.subtitle) > 1
 
-    def _map_streams(self, stream_type: str, streams: List, excludes: list, includes: list, defl: str) -> list:
-        if excludes is None:
-            excludes = []
-        if not includes:
-            includes = None
-        seq_list = list()
-        mapped = list()
-        default_reassign = False
-        for s in streams:
-            stream_lang = s.get('lang', 'none')
-            #
-            # includes take precedence over excludes
-            #
-            if includes is not None and stream_lang not in includes:
-                if s.get('default', None) is not None:
-                    default_reassign = True
-                continue
-
-            if stream_lang in excludes:
-                if s.get('default', None) is not None:
-                    default_reassign = True
-                continue
-
-            # if we got here, map the stream
-            mapped.append(s)
-            seq = s['stream']
-            seq_list.append('-map')
-            seq_list.append(f'0:{seq}')
-
-        if default_reassign:
-            if defl is None:
-                print('Warning: A default stream will be removed but no default language specified to replace it')
-            else:
-                for i, s in enumerate(mapped):
-                    if s.get('lang', None) == defl:
-                        seq_list.append(f'-disposition:{stream_type}:{i}')
-                        seq_list.append('default')
-        return seq_list
-
-    def ffmpeg_streams(self, profile: Profile) -> list:
-        excl_audio = profile.excluded_audio()
-        excl_subtitle = profile.excluded_subtitles()
-        incl_audio = profile.included_audio()
-        incl_subtitle = profile.included_subtitles()
-
-        defl_audio = profile.default_audio()
-        defl_subtitle = profile.default_subtitle()
-
-        if excl_audio is None:
-            excl_audio = []
-        if excl_subtitle is None:
-            excl_subtitle = []
-        #
-        # if no inclusions or exclusions just map everything
-        #
-        if len(incl_audio) == 0 and len(excl_audio) == 0 and len(incl_subtitle) == 0 and len(excl_subtitle) == 0:
-            return ['-map', '0']
-
-        seq_list = list()
-        seq_list.append('-map')
-        seq_list.append(f'0:{self.stream}')
-        audio_streams = self._map_streams("a", self.audio, excl_audio, incl_audio, defl_audio)
-        subtitle_streams = self._map_streams("s", self.subtitle, excl_subtitle, incl_subtitle, defl_subtitle)
-        return seq_list + audio_streams + subtitle_streams
+    # def _map_streams(self, stream_type: str, streams: List, excludes: list, includes: list, defl: str) -> list:
+    #     if excludes is None:
+    #         excludes = []
+    #     if not includes:
+    #         includes = None
+    #     seq_list = list()
+    #     mapped = list()
+    #     default_reassign = False
+    #     for s in streams:
+    #         stream_lang = s.get('lang', 'none')
+    #         #
+    #         # includes take precedence over excludes
+    #         #
+    #         if includes is not None and stream_lang not in includes:
+    #             if s.get('default', None) is not None:
+    #                 default_reassign = True
+    #             continue
+    #
+    #         if stream_lang in excludes:
+    #             if s.get('default', None) is not None:
+    #                 default_reassign = True
+    #             continue
+    #
+    #         # if we got here, map the stream
+    #         mapped.append(s)
+    #         seq = s['stream']
+    #         seq_list.append('-map')
+    #         seq_list.append(f'0:{seq}')
+    #
+    #     if default_reassign:
+    #         if defl is None:
+    #             print('Warning: A default stream will be removed but no default language specified to replace it')
+    #         else:
+    #             for i, s in enumerate(mapped):
+    #                 if s.get('lang', None) == defl:
+    #                     seq_list.append(f'-disposition:{stream_type}:{i}')
+    #                     seq_list.append('default')
+    #     return seq_list
+    #
+    # def stream_map(self, profile: Profile) -> list:
+    #     excl_audio = profile.excluded_audio()
+    #     excl_subtitle = profile.excluded_subtitles()
+    #     incl_audio = profile.included_audio()
+    #     incl_subtitle = profile.included_subtitles()
+    #
+    #     defl_audio = profile.default_audio()
+    #     defl_subtitle = profile.default_subtitle()
+    #
+    #     if excl_audio is None:
+    #         excl_audio = []
+    #     if excl_subtitle is None:
+    #         excl_subtitle = []
+    #     #
+    #     # if no inclusions or exclusions just map everything
+    #     #
+    #     if len(incl_audio) == 0 and len(excl_audio) == 0 and len(incl_subtitle) == 0 and len(excl_subtitle) == 0:
+    #         return ['-map', '0']
+    #
+    #     seq_list = list()
+    #     seq_list.append('-map')
+    #     seq_list.append(f'0:{self.stream}')
+    #     audio_streams = self._map_streams("a", self.audio, excl_audio, incl_audio, defl_audio)
+    #     subtitle_streams = self._map_streams("s", self.subtitle, excl_subtitle, incl_subtitle, defl_subtitle)
+    #     return seq_list + audio_streams + subtitle_streams
 
     def eval_numeric(self, rulename: str, pred: str, value: str) -> bool:
         attr = self.__dict__.get(pred, None)
         if attr is None:
             print(f'Error: Rule "{rulename}" unknown attribute: {pred} ')
             raise ValueError(value)
```

### Comparing `pytranscoder-ffmpeg-2.2.5/pytranscoder/processor.py` & `pytranscoder-ffmpeg-2.2.6/pytranscoder/processor.py`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.5/pytranscoder/rule.py` & `pytranscoder-ffmpeg-2.2.6/pytranscoder/rule.py`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.5/pytranscoder/transcode.py` & `pytranscoder-ffmpeg-2.2.6/pytranscoder/transcode.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,26 +15,27 @@
 
 from pytranscoder import __version__
 from pytranscoder.agent import Agent
 from pytranscoder.cluster import manage_clusters
 from pytranscoder.config import ConfigFile
 from pytranscoder.ffmpeg import FFmpeg
 from pytranscoder.media import MediaInfo
-from pytranscoder.profile import Profile
+from pytranscoder.profile import Profile, Directives
+from pytranscoder.template import Template
 from pytranscoder.utils import filter_threshold, files_from_file, calculate_progress, dump_stats
 
 DEFAULT_CONFIG = os.path.expanduser('~/.transcode.yml')
 
 
 class LocalJob:
     """One file with matched profile to be encoded"""
 
-    def __init__(self, inpath: str, profile: Profile, mixins: List[str], info: MediaInfo):
+    def __init__(self, inpath: str, directives: Directives, mixins: List[str], info: MediaInfo):
         self.inpath = Path(os.path.abspath(inpath))
-        self.profile = profile
+        self.directives = directives
         self.info = info
         self.mixins = mixins
 
 
 class QueueThread(Thread):
     """One transcoding thread associated to a queue"""
 
@@ -71,41 +72,37 @@
         self.lock.release()
 
     def go(self):
 
         while not self.queue.empty():
             try:
                 job: LocalJob = self.queue.get()
-                input_opt = job.profile.input_options.as_shell_params()
-                output_opt = self.config.output_from_profile(job.profile, job.mixins)
 
                 fls = False
                 if self.config.fls_path():
                     # lets write output to local storage, for efficiency
-                    outpath = PurePath(self.config.fls_path(), job.inpath.with_suffix(job.profile.extension).name)
+                    outpath = PurePath(self.config.fls_path(), job.inpath.with_suffix(job.directives.extension()).name)
                     fls = True
                 else:
-                    outpath = job.inpath.with_suffix(job.profile.extension + '.tmp')
+                    outpath = job.inpath.with_suffix(job.directives.extension() + '.tmp')
 
-                #
-                # check if we need to exclude any streams
-                #
-                if job.info.is_multistream() and self.config.automap and job.profile.automap:
-                    output_opt = output_opt + job.info.ffmpeg_streams(job.profile)
-                cli = ['-y', *input_opt, '-i', str(job.inpath), *output_opt, str(outpath)]
+                stream_map = []
+                if job.info.is_multistream() and self.config.automap:
+                    stream_map = job.directives.stream_map(job.info.stream, job.info.audio, job.info.subtitle)
+                cli = ['-y', *job.directives.input_options_list(), '-i', str(job.inpath), *job.directives.output_options_list(self.config, job.mixins), *stream_map, str(outpath)]
 
                 #
                 # display useful information
                 #
                 self.lock.acquire()  # used to synchronize threads so multiple threads don't create a jumble of output
                 try:
                     print('-' * 40)
-                    print('Filename : ' + crayons.green(os.path.basename(str(job.inpath))))
-                    print(f'Profile  : {job.profile.name}')
-                    print('{:<6}   : '.format(job.profile.processor) + ' '.join(cli) + '\n')
+                    print( 'Filename : ' + crayons.green(os.path.basename(str(job.inpath))))
+                    print(f'Directive: {job.directives.name()}')
+                    print( 'ffmpeg   :' + ' '.join(cli) + '\n')
                 finally:
                     self.lock.release()
 
                 if pytranscoder.dry_run:
                     continue
 
                 basename = job.inpath.name
@@ -113,45 +110,44 @@
                 def log_callback(stats):
                     pct_done, pct_comp = calculate_progress(job.info, stats)
                     pytranscoder.status_queue.put({ 'host': 'local',
                                                     'file': basename,
                                                     'speed': stats['speed'],
                                                     'comp': pct_comp,
                                                     'done': pct_done})
-                    #self.log(f'{basename}: speed: {stats["speed"]}x, comp: {pct_comp}%, done: {pct_done:3}%')
-                    if job.profile.threshold_check < 100:
-                        if pct_done >= job.profile.threshold_check and pct_comp < job.profile.threshold:
+                    if job.directives.threshold_check() < 100:
+                        if pct_done >= job.directives.threshold_check() and pct_comp < job.directives.threshold():
                             # compression goal (threshold) not met, kill the job and waste no more time...
                             self.log(f'Encoding of {basename} cancelled and skipped due to threshold not met')
                             return True
                     return False
 
                 job_start = datetime.datetime.now()
                 code = self.ffmpeg.run(cli, log_callback)
                 job_stop = datetime.datetime.now()
                 elapsed = job_stop - job_start
 
                 if code == 0:
-                    if not filter_threshold(job.profile, str(job.inpath), outpath):
+                    if not filter_threshold(job.directives, str(job.inpath), outpath):
                         # oops, this transcode didn't do so well, lets keep the original and scrap this attempt
                         self.log(f'Transcoded file {job.inpath} did not meet minimum savings threshold, skipped')
                         self.complete(job.inpath, (job_stop - job_start).seconds)
                         os.unlink(str(outpath))
                         continue
 
                     self.complete(job.inpath, elapsed.seconds)
                     if not pytranscoder.keep_source:
                         if pytranscoder.verbose:
                             self.log(f'replacing {job.inpath} with {outpath}')
                         job.inpath.unlink()
 
                         if fls:
-                            shutil.move(outpath, job.inpath.with_suffix(job.profile.extension))
+                            shutil.move(outpath, job.inpath.with_suffix(job.directives.extension()))
                         else:
-                            outpath.rename(job.inpath.with_suffix(job.profile.extension))
+                            outpath.rename(job.inpath.with_suffix(job.directives.extension()))
 
                         self.log(crayons.green(f'Finished {job.inpath}'))
                     else:
                         self.log(crayons.yellow(f'Finished {outpath}, original file unchanged'))
                 elif code is not None:
                     self.log(f' Did not complete normally: {self.ffmpeg.last_command}')
                     self.log(f'Output can be found in {self.ffmpeg.log_path}')
@@ -226,79 +222,79 @@
         # wait for all queues to drain and all jobs to complete
 #        for _, queue in self.queues.items():
 #            queue.join()
 
     def enqueue_files(self, files: list):
         """Add requested files to the appropriate queue
 
-        :param files: list of (path,profile) tuples
+        :param files: list of (path,directives) tuples
         :return:
         """
         ffmpeg = FFmpeg(self.configfile.ffmpeg_path)
-        for path, forced_profile, mixins in files:
+        for path, forced_directive, mixins in files:
             #
             # do some prechecks...
             #
-            if forced_profile is not None and not self.configfile.has_profile(forced_profile):
-                print(f'profile "{forced_profile}" referenced from command line not found')
+            if forced_directive is not None and not self.configfile.has_directive(forced_directive):
+                print(f'"{forced_directive}" referenced from command line not found')
                 sys.exit(1)
 
             if len(path) == 0:
                 continue
 
             if not os.path.isfile(path):
                 print(crayons.red('file not found, skipping: ' + path))
                 continue
 
-            if forced_profile:
-                the_profile = self.configfile.get_profile(forced_profile)
+            if forced_directive:
+                the_profile = self.configfile.get_directive(forced_directive)
 
             media_info = ffmpeg.fetch_details(path)
 
             if media_info is None:
                 print(crayons.red(f'File not found: {path}'))
                 continue
 
             if media_info.valid:
 
                 if pytranscoder.verbose:
                     print(str(media_info))
 
-                if forced_profile is None:
+                if forced_directive is None:
                     rule = self.configfile.match_rule(media_info)
                     if rule is None:
-                        print(crayons.green(os.path.basename(path)), crayons.yellow(f'No matching profile found - skipped'))
+                        print(crayons.green(os.path.basename(path)), crayons.yellow(f'No matching profile or template found - skipped'))
                         continue
                     if rule.is_skip():
                         print(crayons.green(os.path.basename(path)), f'SKIPPED ({rule.name})')
                         self.complete.append((path, 0))
                         continue
-                    profile_name = rule.profile
+                    directive_name = rule.profile
                 else:
                     #
                     # looks good, add this file to the thread queue
                     #
-                    profile_name = forced_profile
+                    directive_name = forced_directive
 
-                the_profile = self.configfile.get_profile(profile_name)
-                qname = the_profile.queue_name
+                the_directive = self.configfile.get_directive(directive_name)
+                qname = the_directive.queue_name()
                 if pytranscoder.verbose:
-                    print('Matched with profile {profile_name}')
+                    print('Matched with {the_directive}')
                 if qname is not None:
-                    if not self.configfile.has_queue(the_profile.queue_name):
+                    if not self.configfile.has_queue(the_directive.queue_name()):
                         print(crayons.red(
-                            f'Profile "{profile_name}" indicated queue "{qname}" that has not been defined')
+                            f'Profile "{the_directive}" indicated queue "{qname}" that has not been defined')
                         )
                         sys.exit(1)
                     else:
-                        self.queues[qname].put(LocalJob(path, the_profile, mixins, media_info))
+                        self.queues[qname].put(LocalJob(path, the_directive, mixins, media_info))
                         if pytranscoder.verbose:
                             print('Added to queue {qname}')
                 else:
-                    self.queues['_default_'].put(LocalJob(path, the_profile, mixins, media_info))
+                    self.queues['_default_'].put(LocalJob(path, the_directive, mixins, media_info))
 
 
 def cleanup_queuefile(queue_path: str, completed: Set):
     if not pytranscoder.dry_run and queue_path is not None:
         # pick up any newly added files
         files = set(files_from_file(queue_path))
         # subtract out the ones we've completed
@@ -349,23 +345,26 @@
         print('  --dry-run  Run without actually transcoding or modifying anything, useful to test rules and profiles')
         print('  -v         Verbose output, helpful in debugging profiles and rules')
         print(
             '  -k         Keep source files after transcoding. If used, the transcoded file will have the same '
             'name and .tmp extension')
         print('  -y <file>  Full path to configuration file.  Default is ~/.transcode.yml')
         print('  -p         profile to use. If used with --from-file, applies to all listed media in <filename>')
+        print('  -t         template to use, simpler alternative to profiles')
         print('  -m         Add mixins to profile. Separate multiples with a comma')
+        print('  --agent    Start in agent mode on a host and listen for transcode requests from other pytranscoder.')
         print('\n** PyPi Repo: https://pypi.org/project/pytranscoder-ffmpeg/')
         print('** Read the docs at https://pytranscoder.readthedocs.io/en/latest/')
         sys.exit(0)
 
     install_sigint_handler()
 
     files = list()
     profile = None
+    template = None
     mixins = None
     queue_path = None
     agent_mode = False
     cluster = None
     configfile: Optional[ConfigFile] = None
     host_override = None
     if len(sys.argv) > 1:
@@ -379,14 +378,17 @@
                 if cluster is None:
                     files.extend([(f, profile) for f in tmpfiles])
                 else:
                     files.extend([(f, cluster) for f in tmpfiles])
             elif sys.argv[arg] == '-p':                 # specific profile
                 profile = sys.argv[arg + 1]
                 arg += 1
+            elif sys.argv[arg] == '-t':                 # specific template
+                template = sys.argv[arg + 1]
+                arg += 1
             elif sys.argv[arg] == '-y':                 # specify yaml config file
                 arg += 1
                 configfile = ConfigFile(sys.argv[arg])
             elif sys.argv[arg] == '-k':                 # keep original
                 pytranscoder.keep_source = True
             elif sys.argv[arg] == '--dry-run':
                 pytranscoder.dry_run = True
@@ -407,17 +409,17 @@
             else:
                 if os.name == "nt":
                     expanded_files: List = glob.glob(sys.argv[arg])     # handle wildcards in Windows
                 else:
                     expanded_files = [sys.argv[arg]]
                 for f in expanded_files:
                     if cluster is None:
-                        files.append((f, profile, mixins))
+                        files.append((f, profile or template, mixins))
                     else:
-                        files.append((f, cluster, profile, mixins))
+                        files.append((f, cluster, profile or template, mixins))
             arg += 1
 
     if agent_mode:
         agent = Agent()
         agent.run()
         sys.exit(0)
 
@@ -432,17 +434,17 @@
     if len(files) == 0 and queue_path is None and configfile.default_queue_file is not None:
         #
         # load from list of files
         #
         tmpfiles = files_from_file(configfile.default_queue_file)
         queue_path = configfile.default_queue_file
         if cluster is None:
-            files.extend([(f, profile, mixins) for f in tmpfiles])
+            files.extend([(f, profile or template, mixins) for f in tmpfiles])
         else:
-            files.extend([(f, cluster, profile) for f in tmpfiles])
+            files.extend([(f, cluster, profile or template) for f in tmpfiles])
 
     if len(files) == 0:
         print(crayons.yellow(f'Nothing to do'))
         sys.exit(0)
 
     if cluster is not None:
         if host_override is not None:
```

### Comparing `pytranscoder-ffmpeg-2.2.5/pytranscoder/utils.py` & `pytranscoder-ffmpeg-2.2.6/pytranscoder/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 
 import math
 import os
 import platform
 import subprocess
-from typing import Dict, List
+from typing import Dict
 
 import pytranscoder
 from pytranscoder.media import MediaInfo
-from pytranscoder.profile import Profile
+from pytranscoder.profile import Directives
 
 
-def filter_threshold(profile: Profile, inpath, outpath):
-    if profile.threshold > 0:
+def filter_threshold(profile: Directives, inpath, outpath):
+    if profile.threshold() > 0:
         orig_size = os.path.getsize(inpath)
         new_size = os.path.getsize(outpath)
-        return is_exceeded_threshold(profile.threshold, orig_size, new_size)
+        return is_exceeded_threshold(profile.threshold(), orig_size, new_size)
     return True
 
 
 def is_exceeded_threshold(pct_threshold: int, orig_size: int, new_size: int) -> bool:
     pct_savings = 100 - math.floor((new_size * 100) / orig_size)
     if pct_savings < pct_threshold:
         return False
```

### Comparing `pytranscoder-ffmpeg-2.2.5/pytranscoder_ffmpeg.egg-info/PKG-INFO` & `pytranscoder-ffmpeg-2.2.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,21 @@
-Metadata-Version: 2.1
-Name: pytranscoder-ffmpeg
-Version: 2.2.5
-Summary: A ffmpeg workflow manager for transcoding
-Home-page: https://github.com/mlsmithjr/transcoder
-Author: Marshall L Smith Jr
-Author-email: marshallsmithjr@gmail.com
-Keywords: ffmpeg qsv cuda encode transcode
-Classifier: Programming Language :: Python :: 3
-Classifier: Environment :: Console
-Classifier: Topic :: Multimedia :: Video :: Conversion
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## pytranscoder
 Python wrapper for ffmpeg for batch, concurrent, or clustered transcoding using defined profiles and optional rules engine
 for automation.
 
 [Read The Docs](https://pytranscoder.readthedocs.io/en/latest/)
 
 
 #### News
 
-**Coming soon** - agent mode!
-That's right.  Due to a few issues around Windows 11 security and WSL2 networking changes I'm adding an agent to this tool so that you can skip the convoluted setup of ssh and exposing network shares on Windows 11.  This is in testing now and will be released after I update the docs.  What this means is you can run pytranscoder in 'agent' mode on any Windows machine without setting up ssh key sharing, hacking the registry to make OpenSSH see network shares, and setting up a proxy to make WSL2 allow ssh address resolution.  You can then use any Windows box as a transcoding agent apart from your main hub.  Of course, the agent will work on linux and macos too.
-
+**Coming soon**
 
-Pytranscoder now supports better profiles.  Existing ones are backward-compatible unless you try to use mixings.
-The mixin feature allows you to create pieces of profiles and combine them into another profile on the commandline at runtime.
-This negates the need to create many unique permutations of a profile just for simple variances.
+Version 3 will include an alternate means of configuring your setup.  Let's face it, all that YAML is confusing.
+The new version will use templating and be far simpler and very much smaller -- all my converted profiles fit on one screen now.
+Existing profile support will remain indefinitely for users with more complicated setups, but templates will appeal more to most users.
 
 
 #### What it is
 This script is intended to help automate transcoding for people encoding lots of video.
 It is more than a wrapper - it is a workflow and job manager.
 
 There are 2 modes: **local** and **clustered**.  Local mode is the most common usage and is for running this script on the same machine where it is installed.  Cluster mode turns pytranscoder into a remote encoding manager.  In this mode it delegates and manages encode jobs running on multiple hosts.  This requires more advanced configuration and is documented separately in [Cluster.md](https://github.com/mlsmithjr/transcoder/blob/master/Cluster.md)
```

### Comparing `pytranscoder-ffmpeg-2.2.5/pytranscoder_ffmpeg.egg-info/SOURCES.txt` & `pytranscoder-ffmpeg-2.2.6/pytranscoder_ffmpeg.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 pytranscoder/cluster.py
 pytranscoder/config.py
 pytranscoder/ffmpeg.py
 pytranscoder/media.py
 pytranscoder/processor.py
 pytranscoder/profile.py
 pytranscoder/rule.py
+pytranscoder/template.py
 pytranscoder/transcode.py
 pytranscoder/utils.py
 pytranscoder_ffmpeg.egg-info/PKG-INFO
 pytranscoder_ffmpeg.egg-info/SOURCES.txt
 pytranscoder_ffmpeg.egg-info/dependency_links.txt
 pytranscoder_ffmpeg.egg-info/entry_points.txt
 pytranscoder_ffmpeg.egg-info/requires.txt
```

### Comparing `pytranscoder-ffmpeg-2.2.5/setup.py` & `pytranscoder-ffmpeg-2.2.6/setup.py`

 * *Files identical despite different names*

