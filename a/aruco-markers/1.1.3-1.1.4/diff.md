# Comparing `tmp/aruco_markers-1.1.3.tar.gz` & `tmp/aruco_markers-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aruco_markers-1.1.3.tar", last modified: Wed Apr  5 08:45:10 2023, max compression
+gzip compressed data, was "aruco_markers-1.1.4.tar", last modified: Sun Apr  9 13:52:29 2023, max compression
```

## Comparing `aruco_markers-1.1.3.tar` & `aruco_markers-1.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-05 08:45:10.133535 aruco_markers-1.1.3/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    11357 2023-03-24 18:40:46.000000 aruco_markers-1.1.3/LICENSE
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    14281 2023-04-05 08:45:10.133535 aruco_markers-1.1.3/PKG-INFO
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    13445 2023-04-05 08:43:44.000000 aruco_markers-1.1.3/README.md
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-05 08:45:10.133535 aruco_markers-1.1.3/aruco_markers/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      292 2023-03-28 15:07:01.000000 aruco_markers-1.1.3/aruco_markers/__init__.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    17158 2023-04-03 12:14:19.000000 aruco_markers-1.1.3/aruco_markers/calibrate.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     4251 2023-04-04 15:30:29.000000 aruco_markers-1.1.3/aruco_markers/camera.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     7993 2023-04-03 12:43:30.000000 aruco_markers-1.1.3/aruco_markers/detect.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    11467 2023-04-05 08:22:29.000000 aruco_markers-1.1.3/aruco_markers/main.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     6058 2023-04-05 08:22:24.000000 aruco_markers-1.1.3/aruco_markers/marker.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      426 2023-03-28 16:11:35.000000 aruco_markers-1.1.3/aruco_markers/utils.py
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-05 08:45:10.133535 aruco_markers-1.1.3/aruco_markers.egg-info/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    14281 2023-04-05 08:45:10.000000 aruco_markers-1.1.3/aruco_markers.egg-info/PKG-INFO
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      435 2023-04-05 08:45:10.000000 aruco_markers-1.1.3/aruco_markers.egg-info/SOURCES.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)        1 2023-04-05 08:45:10.000000 aruco_markers-1.1.3/aruco_markers.egg-info/dependency_links.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       50 2023-04-05 08:45:10.000000 aruco_markers-1.1.3/aruco_markers.egg-info/entry_points.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       61 2023-04-05 08:45:10.000000 aruco_markers-1.1.3/aruco_markers.egg-info/requires.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       14 2023-04-05 08:45:10.000000 aruco_markers-1.1.3/aruco_markers.egg-info/top_level.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      783 2023-04-05 08:27:27.000000 aruco_markers-1.1.3/pyproject.toml
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       38 2023-04-05 08:45:10.133535 aruco_markers-1.1.3/setup.cfg
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     1096 2023-04-05 08:27:21.000000 aruco_markers-1.1.3/setup.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-09 13:52:29.863731 aruco_markers-1.1.4/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    11357 2023-03-24 18:40:46.000000 aruco_markers-1.1.4/LICENSE
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    14896 2023-04-09 13:52:29.863731 aruco_markers-1.1.4/PKG-INFO
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    14060 2023-04-09 13:51:07.000000 aruco_markers-1.1.4/README.md
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-09 13:52:29.863731 aruco_markers-1.1.4/aruco_markers/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      332 2023-04-09 13:44:31.000000 aruco_markers-1.1.4/aruco_markers/__init__.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    17158 2023-04-07 11:30:34.000000 aruco_markers-1.1.4/aruco_markers/calibrate.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     7714 2023-04-09 13:44:31.000000 aruco_markers-1.1.4/aruco_markers/camera.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     7834 2023-04-07 11:30:34.000000 aruco_markers-1.1.4/aruco_markers/detect.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    13056 2023-04-09 13:44:31.000000 aruco_markers-1.1.4/aruco_markers/main.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     6058 2023-04-07 11:30:34.000000 aruco_markers-1.1.4/aruco_markers/marker.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      426 2023-04-07 11:30:34.000000 aruco_markers-1.1.4/aruco_markers/utils.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-09 13:52:29.863731 aruco_markers-1.1.4/aruco_markers.egg-info/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    14896 2023-04-09 13:52:29.000000 aruco_markers-1.1.4/aruco_markers.egg-info/PKG-INFO
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      435 2023-04-09 13:52:29.000000 aruco_markers-1.1.4/aruco_markers.egg-info/SOURCES.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)        1 2023-04-09 13:52:29.000000 aruco_markers-1.1.4/aruco_markers.egg-info/dependency_links.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       50 2023-04-09 13:52:29.000000 aruco_markers-1.1.4/aruco_markers.egg-info/entry_points.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       61 2023-04-09 13:52:29.000000 aruco_markers-1.1.4/aruco_markers.egg-info/requires.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       14 2023-04-09 13:52:29.000000 aruco_markers-1.1.4/aruco_markers.egg-info/top_level.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      783 2023-04-09 13:39:41.000000 aruco_markers-1.1.4/pyproject.toml
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       38 2023-04-09 13:52:29.863731 aruco_markers-1.1.4/setup.cfg
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     1096 2023-04-09 13:39:36.000000 aruco_markers-1.1.4/setup.py
```

### Comparing `aruco_markers-1.1.3/LICENSE` & `aruco_markers-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aruco_markers-1.1.3/PKG-INFO` & `aruco_markers-1.1.4/aruco_markers.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aruco_markers
-Version: 1.1.3
+Name: aruco-markers
+Version: 1.1.4
 Summary:  A compact Python package for handling ArUCo markers.
 Home-page: https://github.com/cmower/aruco_markers
 Author: Christopher E. Mower
 Author-email: "Christopher E. Mower" <christopher.mower@kcl.ac.uk>
 License: Apache License 2.0
 Project-URL: Homepage, https://cmower.github.io/aruco_markers/
 Project-URL: Documentation, https://cmower.github.io/aruco_markers/
@@ -282,14 +282,33 @@
 ```
 $ aruco detect --dict DICT_4X4_50 --markerindex 0
 ```
 
 *Note*, the marker I use in this example has a length of 5cm.
 This information is required if you want to use the pose estimation.
 
+## Server
+
+You can run a server that will broadcast images to a UDP network.
+Simply run the following
+
+```
+$ aruco server
+```
+
+Several listeners can recieve the feeds from this server.
+The information flow is as follows.
+
+<p align="center">
+  <img src="https://raw.githubusercontent.com/cmower/aruco_markers/master/doc/image/server-overview.png" width="60%" align="center">
+</p>
+
+To see this in action try running the example script [example/server_listener.py](https://github.com/cmower/aruco_markers/blob/master/example/server_listener.py).
+**Note**, this script can be run multiple times in separate terminals.
+
 # Marker pose estimation
 
 If you opt for the `aruco_markers` package, you can use the command line interface to produce tags and calibrate cameras.
 However, if you require additional features, you can customize the class/method structure available in the library.
 Several methods are provided to that enable you to easily load camera parameters, and estimate marker poses.
 
 Please see the [example](example/ros1_tf_publisher.py), that shows how to implement a simple pose estimator into ROS.
```

### Comparing `aruco_markers-1.1.3/README.md` & `aruco_markers-1.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,33 @@
 ```
 $ aruco detect --dict DICT_4X4_50 --markerindex 0
 ```
 
 *Note*, the marker I use in this example has a length of 5cm.
 This information is required if you want to use the pose estimation.
 
+## Server
+
+You can run a server that will broadcast images to a UDP network.
+Simply run the following
+
+```
+$ aruco server
+```
+
+Several listeners can recieve the feeds from this server.
+The information flow is as follows.
+
+<p align="center">
+  <img src="https://raw.githubusercontent.com/cmower/aruco_markers/master/doc/image/server-overview.png" width="60%" align="center">
+</p>
+
+To see this in action try running the example script [example/server_listener.py](https://github.com/cmower/aruco_markers/blob/master/example/server_listener.py).
+**Note**, this script can be run multiple times in separate terminals.
+
 # Marker pose estimation
 
 If you opt for the `aruco_markers` package, you can use the command line interface to produce tags and calibrate cameras.
 However, if you require additional features, you can customize the class/method structure available in the library.
 Several methods are provided to that enable you to easily load camera parameters, and estimate marker poses.
 
 Please see the [example](example/ros1_tf_publisher.py), that shows how to implement a simple pose estimator into ROS.
```

### Comparing `aruco_markers-1.1.3/aruco_markers/calibrate.py` & `aruco_markers-1.1.4/aruco_markers/calibrate.py`

 * *Files identical despite different names*

### Comparing `aruco_markers-1.1.3/aruco_markers/detect.py` & `aruco_markers-1.1.4/aruco_markers/detect.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,18 +40,14 @@
     def transform(self) -> np.ndarray:
         """! Homogenous transformation matrix representing the pose."""
         T = np.eye(4)
         T[:3, :3] = self.rotation.as_matrix()
         T[:3, 3] = self.translation
         return T
 
-    def add_translation_offset(self, offset_translation: Union[List[float], np.ndarray]):
-        self.translation += np.asarray(offset_translation)
-        
-
     def to_ros_msg(self) -> Transform:
         """! Converts the pose to a geometry_msg/Transform ROS message. This method is only available when ROS is installed on your system."""
         assert ROS_AVAILABLE, "ROS not found (perhaps you didn't source it?)"
         tf = Transform()
         tf.translation.x = self.translation[0]
         tf.translation.y = self.translation[1]
         tf.translation.z = self.translation[2]
```

### Comparing `aruco_markers-1.1.3/aruco_markers/main.py` & `aruco_markers-1.1.4/aruco_markers/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import sys
 import argparse
 from collections import OrderedDict
 
 from .marker import Marker
-from .camera import cvCamera
+from .camera import cvCamera, CameraViewer, ServerCameraViewerCallback, UDPSenderServer
 from .calibrate import collect_data, calibrate, Checkerboard
 from .detect import detect_poses_from_camera, DetectSingleMarkerPoseFromCameraCallback
 
 #
 # Helper variables/methods for setting up documentation
 #
 
 command_descr = OrderedDict()
 command_descr["collect"] = "Collect data with checkerboard to calibrate a camera."
 command_descr["calibrate"] = "Calibrate a camera."
 command_descr["generate"] = "Generate marker tags."
 command_descr["detect"] = "Detect marker poses from camera feed."
+command_descr["server"] = "Start a camera server."
 
 longest_cmd_name = max(command_descr, key=lambda k: len(k))
 len_longest_cmd_name = len(longest_cmd_name)
 
 doc_main = """usage: aruco COMMAND [OPTIONS]
 
 Available commands
@@ -408,25 +409,80 @@
     callback = DetectSingleMarkerPoseFromCameraCallback(
         camera, args.dict, args.markerindex
     )
 
     detect_poses_from_camera(camera, callback, args.reportduration)
 
 
+def server_main(argv):
+    # Setup argument parser
+    parser = init_argparser("server")
+
+    cameraindex_param_default = 0
+    parser.add_argument(
+        "-c",
+        "--cameraindex",
+        type=int,
+        default=cameraindex_param_default,
+        help=helptxt(
+            "Camera index.",
+            "This corresponds to /dev/videoN where N is the camera index.",
+            default=cameraindex_param_default,
+        ),
+    )
+
+    compressionquality_param_default = 80
+    parser.add_argument(
+        "-q",
+        "--compressionquality",
+        type=int,
+        default=compressionquality_param_default,
+        help=helptxt(
+            "Quality of the compression, in range 0 to 100.",
+            default=compressionquality_param_default,
+        ),
+    )
+
+    args = parser.parse_args(argv)
+
+    # Setup camera
+    camera = cvCamera(args.cameraindex)
+
+    # Setup server and callback
+    assert 0 <= args.compressionquality <= 100, (
+        f"Compression quality argument outside of allowed range. "
+        + "Got '{args.compressionquality}' expected in range 0 to 100."
+    )
+    sender_server = UDPSenderServer()
+    callback = ServerCameraViewerCallback(
+        sender_server, compression_quality=args.compressionquality
+    )
+
+    # Start camera viewer
+    viewer = CameraViewer("server", camera, callback)
+    try:
+        viewer.spin()
+    except KeyboardInterrupt:
+        pass
+    finally:
+        viewer.close()
+
+
 #
 # Main entry point
 #
 
 
 def main():
     cmd_main_map = {
         "generate": generate_main,
         "collect": collect_main,
         "calibrate": calibrate_main,
         "detect": detect_main,
+        "server": server_main,
     }
 
     # Get command and arguments
     try:
         cmd = sys.argv[1]
     except IndexError:
         print("\033[91m" + "[ERROR] unable to parse command line input" + "\033[0m")
```

### Comparing `aruco_markers-1.1.3/aruco_markers/marker.py` & `aruco_markers-1.1.4/aruco_markers/marker.py`

 * *Files identical despite different names*

### Comparing `aruco_markers-1.1.3/aruco_markers.egg-info/PKG-INFO` & `aruco_markers-1.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aruco-markers
-Version: 1.1.3
+Name: aruco_markers
+Version: 1.1.4
 Summary:  A compact Python package for handling ArUCo markers.
 Home-page: https://github.com/cmower/aruco_markers
 Author: Christopher E. Mower
 Author-email: "Christopher E. Mower" <christopher.mower@kcl.ac.uk>
 License: Apache License 2.0
 Project-URL: Homepage, https://cmower.github.io/aruco_markers/
 Project-URL: Documentation, https://cmower.github.io/aruco_markers/
@@ -282,14 +282,33 @@
 ```
 $ aruco detect --dict DICT_4X4_50 --markerindex 0
 ```
 
 *Note*, the marker I use in this example has a length of 5cm.
 This information is required if you want to use the pose estimation.
 
+## Server
+
+You can run a server that will broadcast images to a UDP network.
+Simply run the following
+
+```
+$ aruco server
+```
+
+Several listeners can recieve the feeds from this server.
+The information flow is as follows.
+
+<p align="center">
+  <img src="https://raw.githubusercontent.com/cmower/aruco_markers/master/doc/image/server-overview.png" width="60%" align="center">
+</p>
+
+To see this in action try running the example script [example/server_listener.py](https://github.com/cmower/aruco_markers/blob/master/example/server_listener.py).
+**Note**, this script can be run multiple times in separate terminals.
+
 # Marker pose estimation
 
 If you opt for the `aruco_markers` package, you can use the command line interface to produce tags and calibrate cameras.
 However, if you require additional features, you can customize the class/method structure available in the library.
 Several methods are provided to that enable you to easily load camera parameters, and estimate marker poses.
 
 Please see the [example](example/ros1_tf_publisher.py), that shows how to implement a simple pose estimator into ROS.
```

### Comparing `aruco_markers-1.1.3/pyproject.toml` & `aruco_markers-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aruco_markers"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="Christopher E. Mower", email="christopher.mower@kcl.ac.uk" },
 ]
 description = " A compact Python package for handling ArUCo markers."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aruco_markers-1.1.3/setup.py` & `aruco_markers-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setup(
     name="aruco_markers",
     description="A compact Python package for handling ArUCo markers.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="1.1.3",
+    version="1.1.4",
     author="Christopher E. Mower",
     author_email="christopher.mower@kcl.ac.uk",
     url="https://github.com/cmower/aruco_markers",
     packages=["aruco_markers"],
     license="Apache License 2.0",
     entry_points={
         "console_scripts": [
```

