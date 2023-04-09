# Comparing `tmp/ssoss-0.3.15.tar.gz` & `tmp/ssoss-0.3.16.tar.gz`

## Comparing `ssoss-0.3.15.tar` & `ssoss-0.3.16.tar`

### file list

```diff
@@ -1,25 +1,34 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ssoss-0.3.15/requirements.in
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ssoss-0.3.15/requirements.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ssoss-0.3.15/.idea/.gitignore
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 ssoss-0.3.15/.idea/Traffic Signal Sight Distance Checks.iml
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 ssoss-0.3.15/.idea/misc.xml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 ssoss-0.3.15/.idea/modules.xml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 ssoss-0.3.15/.idea/toolchains.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ssoss-0.3.15/.idea/vcs.xml
--rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 ssoss-0.3.15/.idea/workspace.xml
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 ssoss-0.3.15/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ssoss-0.3.15/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 ssoss-0.3.15/src/ssoss/__init__.py
--rw-r--r--   0        0        0    27184 2020-02-02 00:00:00.000000 ssoss-0.3.15/src/ssoss/dynamic_road_object.py
--rw-r--r--   0        0        0    10759 2020-02-02 00:00:00.000000 ssoss-0.3.15/src/ssoss/motion_road_object.py
--rw-r--r--   0        0        0    18209 2020-02-02 00:00:00.000000 ssoss-0.3.15/src/ssoss/process_road_objects.py
--rw-r--r--   0        0        0    17468 2020-02-02 00:00:00.000000 ssoss-0.3.15/src/ssoss/process_video.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 ssoss-0.3.15/src/ssoss/ssoss_cli.py
--rw-r--r--   0        0        0     4362 2020-02-02 00:00:00.000000 ssoss-0.3.15/src/ssoss/ssoss_gui.py
--rw-r--r--   0        0        0     8542 2020-02-02 00:00:00.000000 ssoss-0.3.15/src/ssoss/static_road_object.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ssoss-0.3.15/tests/__init__.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 ssoss-0.3.15/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 ssoss-0.3.15/LICENSE.txt
--rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 ssoss-0.3.15/README.md
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ssoss-0.3.15/pyproject.toml
--rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 ssoss-0.3.15/PKG-INFO
+-rwxr-xr-x   0        0        0     1064 2020-02-02 00:00:00.000000 ssoss-0.3.16/build.spec
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ssoss-0.3.16/requirements.in
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ssoss-0.3.16/requirements.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ssoss-0.3.16/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ssoss-0.3.16/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ssoss-0.3.16/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ssoss-0.3.16/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ssoss-0.3.16/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 ssoss-0.3.16/src/ssoss/__init__.py
+-rw-r--r--   0        0        0    27184 2020-02-02 00:00:00.000000 ssoss-0.3.16/src/ssoss/dynamic_road_object.py
+-rw-r--r--   0        0        0    10759 2020-02-02 00:00:00.000000 ssoss-0.3.16/src/ssoss/motion_road_object.py
+-rw-r--r--   0        0        0    18339 2020-02-02 00:00:00.000000 ssoss-0.3.16/src/ssoss/process_road_objects.py
+-rw-r--r--   0        0        0    17928 2020-02-02 00:00:00.000000 ssoss-0.3.16/src/ssoss/process_video.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 ssoss-0.3.16/src/ssoss/ssoss_cli.py
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 ssoss-0.3.16/src/ssoss/ssoss_gui.py
+-rw-r--r--   0        0        0     8847 2020-02-02 00:00:00.000000 ssoss-0.3.16/src/ssoss/static_road_object.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ssoss-0.3.16/src/ssoss/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ssoss-0.3.16/src/ssoss/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ssoss-0.3.16/src/ssoss/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ssoss-0.3.16/src/ssoss/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ssoss-0.3.16/src/ssoss/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ssoss-0.3.16/tests/__init__.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 ssoss-0.3.16/tests/test_static_road_object.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ssoss-0.3.16/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ssoss-0.3.16/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ssoss-0.3.16/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ssoss-0.3.16/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 ssoss-0.3.16/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ssoss-0.3.16/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 ssoss-0.3.16/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 ssoss-0.3.16/LICENSE.txt
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 ssoss-0.3.16/README.md
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ssoss-0.3.16/pyproject.toml
+-rw-r--r--   0        0        0     6007 2020-02-02 00:00:00.000000 ssoss-0.3.16/PKG-INFO
```

### Comparing `ssoss-0.3.15/requirements.txt` & `ssoss-0.3.16/requirements.txt`

 * *Files identical despite different names*

### Comparing `ssoss-0.3.15/src/ssoss/dynamic_road_object.py` & `ssoss-0.3.16/src/ssoss/dynamic_road_object.py`

 * *Files identical despite different names*

### Comparing `ssoss-0.3.15/src/ssoss/motion_road_object.py` & `ssoss-0.3.16/src/ssoss/motion_road_object.py`

 * *Files identical despite different names*

### Comparing `ssoss-0.3.15/src/ssoss/process_road_objects.py` & `ssoss-0.3.16/src/ssoss/process_road_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,22 +32,22 @@
         :gpx_filepath: as string, full directory and filename of gpx file
         """
 
         self.intersection_listDF = None
         self.intersection_load = None
         self.date_format = "%m-%d-%Y--%H-%M-%S.%f-%Z"
         self.pretty_datetime_format = "%y-%m-%d %H:%M:%S"
-
         self.in_gpx_dir_path = Path(gpx_filestring).parent
         self.in_dir_path = self.in_gpx_dir_path
         self.out_dir_path = Path(self.in_dir_path, "/out/") #  self.in_dir_path / "out/"
         self.out_dir_path.parent.mkdir(exist_ok=True, parents=True)
 
         # init variables
-        self.intersection_filename = Path(signals_filestring)
+        if signals_filestring:
+            self.intersection_filename = Path(signals_filestring)
         self.gpx_filename = Path(gpx_filestring).stem
         self.pickle_file = ''
         self.gpx_file = ''
         self.csv_file = None
         self.gpxDF = ''
         self.gpx_listDF = None
         self.gDF_pickle_file = None
@@ -57,18 +57,19 @@
 
         self.intersection_approaches = 0
 
         # scafold directory structure if not present
         gpx_video_dir = self.in_gpx_dir_path
         p = Path(str(gpx_video_dir))
 
+        if signals_filestring:
+            all_intersections_df = self.load_intersection_csv(self.intersection_filename)
+        if self.gpx_filename:
+            gpx_df = self.load_gpx_to_obj_df(self.gpx_filename, use_pickle=False)
 
-        all_intersections_df = self.load_intersection_csv(self.intersection_filename)
-        gpx_df = self.load_gpx_to_obj_df(self.gpx_filename, use_pickle=False)
-        self.gpx_summary()
 
     @staticmethod
     def speed_calc(point1, point2, t1, t2) -> float:
         """
         Calculates Meters Per Second speed between two point and time objects
         """
         # dist = geo.distance(point1.latitude, point1.longitude, point2.latitude, point2.longitude)
@@ -251,17 +252,18 @@
                     )
                     pt_count += 1
 
         self.gpx_listDF = pd.DataFrame(gpx_load)
         #self.gpx_listDF.to_pickle(self.pickle_file)
         #self.gpx_listDF.to_csv(self.csv_file)
         print(
-            f"Processed {pt_count} points of GPX file."
+            f"Processing {pt_count} points of GPX file."
         )
-        self.update_gpx_points()
+        if self.intersection_listDF is not None:
+            self.update_gpx_points()
         self.gpx_summary()
         return self.gpx_listDF
 
     def update_gpx_points(self):
         """
         updates gpx_prev_point and gpx_next_point as objects after the initial points
         are loaded
```

### Comparing `ssoss-0.3.15/src/ssoss/process_video.py` & `ssoss-0.3.16/src/ssoss/process_video.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 
         self.fps = self.get_fps()
         self.frame_count = self.get_frame_count()
         self.duration = self.get_duration()
         self.start_time = 0
         self.capture = ""
 
-        self.vid_summary()
+
+        self.vid_summary(vid_summary=True)
 
     def set_start_utc(self, video_start_time):
         self.start_time = video_start_time
         return None
 
     def get_start_timestamp(self):
         return self.start_time
@@ -67,15 +68,15 @@
         elapsed_time = frame / self.fps
         if type(ts) is float:
             start_time = ts - elapsed_time
         else:
             t_temp = (dateutil.parser.isoparse(ts))  #  isoparse parses ISO-8601 datetime string into datetime.datetime
             start_time = t_temp.replace(tzinfo=timezone.utc).timestamp() - elapsed_time
         self.set_start_utc(start_time)
-        self.vid_summary(sync=True)
+        self.vid_summary(vid_summary=False, sync=True)
         return None
 
     def create_pic_list_from_zip(self, i_desc_timestamps):
         """returns sight distance description text and frame of video to extract as 2 lists"""
         intersection_desc = []
         frames = []
         prev_frame = 0
@@ -90,15 +91,15 @@
                 if int(frame_of_video) > int(prev_frame):
                     intersection_desc.append(filename_description[sd_item])
                     frames.append(int(frame_of_video))
                 prev_frame = frame_of_video
 
         return intersection_desc, frames
 
-    def extract_sightings(self, desc_timestamps, project, gen_gif=False):
+    def extract_sightings(self, desc_timestamps, project, label_img=True, gen_gif=False):
         """
         extract sighting images from video based on description and timestamp zip
 
         desc_timestamps: sorted list of tuples (filename description, timestamp of sight distance)
         project: instance of ProcessRoadObjects() class
         """
 
@@ -138,15 +139,16 @@
                     capture.release()
                     break
                 i += 1
             if i > extract_frames[-1]:
                 break
         capture.release()
 
-        self.img_overlay_info_box(self.video_filename, project)
+        if label_img:
+            self.img_overlay_info_box(self.video_filename, project)
         if gen_gif:
             self.generate_gif(desc_timestamps, project)
 
     #  TODO: convert to start_sec, start_min=0, end_sec, end_min=0, folder="")
     def extract_frames_between(self, start_sec, end_sec):
         """ helper function to extract frames from video during a specific time period to estimate offset
             between gpx and video
@@ -319,20 +321,20 @@
             return str(round(size, 2)) + ' Bytes'
 
     def get_filesize(self):
         # get the file size
         file_byte = os.path.getsize(self.video_filepath)
         return self.sizeConvert(file_byte)
 
-    def vid_summary(self, sync=False):
+    def vid_summary(self, vid_summary, sync=False):
         #  display values
         width = 70
         title = "VIDEO SUMMARY"
         symbol = "="
-        sync_title = "Sync Start Time"
+        sync_title = "VIDEO SYNCHRONIZATION SUMMARY"
 
         vid_file = cv2.VideoCapture(str(self.video_filepath))
         if vid_file.isOpened():
             # get vcap property
             vid_width = vid_file.get(cv2.CAP_PROP_FRAME_WIDTH)  # float `width`
             vid_height = vid_file.get(cv2.CAP_PROP_FRAME_HEIGHT)  # float `height`
 
@@ -340,32 +342,31 @@
                 {symbol * width}
                 {" " * (int(width/2)-int(len(title)/2))}{title}
                 {symbol * width}
                 # Video File: {str(self.video_filepath)}
                 # Video File Size: {self.get_filesize()}
                 # Resolution (w x h): {vid_width} x {vid_height} ({round((vid_width * vid_height)/(1*10**6),1)}MP)
                 # Frames Per Second: {self.fps}
-                # Total Number of Frames: {self.frame_count}
+                # Total Number of Frames: {self.frame_count:,}
                 # Total Duration: {self.hr_min_sec(self.get_duration())}
                 {symbol * width}
                 """
 
         sync_time = f"""
                     {symbol * width}
                     {" " * (int(width/2)-int(len(sync_title)/2))}{sync_title}
                     {symbol * width}
                     # Start Time: {datetime.fromtimestamp(self.start_time, tz=None)}
                     # End Time:   {datetime.fromtimestamp(self.start_time + self.get_duration(), tz=None)}
                     {symbol * width}
                     """
-
-        if not sync:
+        if vid_summary:
             print(summary)
-        else:
-            print(sync)
+        if sync:
+            print(sync_time)
 
 
     @staticmethod
     def find_font_scale(label, max_width):
         font_scl = 0.1
         textsize_x, textsize_y = cv2.getTextSize(label, cv2.FONT_HERSHEY_PLAIN, font_scl, 1)[0]
         if textsize_x < max_width:
@@ -387,53 +388,56 @@
 
         alpha = 1  # Transparency factor.
         text_font = cv2.FONT_HERSHEY_PLAIN
         font_thickness = 1
 
         img_dir_string = str(img_path)
         label_img_dir_string = str(label_img_path)
+        pattern_criteria = ['*.[0-3]-*.jpg','[!.]*']
 
-        pathlist = Path(img_dir_string).rglob('*.[0-3]-*.jpg') #  filter for images where * is wildcard
+        #  filter for images where * is wildcard and don't include hidden (.*) files
+        pathlist = [f for f in Path(img_dir_string).rglob('*.[0-3]-*.jpg') if not str(f).startswith(".")]
         for file in pathlist:
-            filename = str(Path(file).name)
-            img_path = img_dir_string + "/" + filename
-            img = cv2.imread(img_path)
-            overlay = img.copy()
-
-            label_img_name = str(Path(label_img_path, filename))
-
-            # get img dimensions
-            img_height, img_width, channels = img.shape
-            rect_h = int(img_height * 0.05)
-            rect_w = img_width
-            rect_y = img_height-rect_h
-
-            # build label
-            sro_id = int(filename.split(".")[0])
-            b_index = int((filename.rsplit(".")[1])[0:1])
-            distance = 0
-            ts = float(filename.split("-")[-1].replace(".jpg", ""))
-            label = ro_info.intersection_frame_description(sro_id, b_index, distance, ts, desc_type="label")
-            font_scale = self.find_font_scale(label, rect_w)
-            textsize_x, textsize_y = cv2.getTextSize(label, text_font,  font_scale, font_thickness)[0]
-            text_y = int((img_height - rect_h/2.0)+textsize_y/2.0)
+            if not str(file.stem).startswith("."):
+                filename = str(Path(file).name)
+                img_path = img_dir_string + "/" + filename
+                img = cv2.imread(img_path)
+                overlay = img.copy()
+
+                label_img_name = str(Path(label_img_path, filename))
+
+                # get img dimensions
+                img_height, img_width, channels = img.shape
+                rect_h = int(img_height * 0.05)
+                rect_w = img_width
+                rect_y = img_height-rect_h
+
+                # build label
+                sro_id = int(filename.split(".")[0])
+                b_index = int((filename.rsplit(".")[1])[0:1])
+                distance = 0
+                ts = float(filename.split("-")[-1].replace(".jpg", ""))
+                label = ro_info.intersection_frame_description(sro_id, b_index, distance, ts, desc_type="label")
+                font_scale = self.find_font_scale(label, rect_w)
+                textsize_x, textsize_y = cv2.getTextSize(label, text_font,  font_scale, font_thickness)[0]
+                text_y = int((img_height - rect_h/2.0)+textsize_y/2.0)
 
-            if textsize_x <= rect_w:
-                text_x = int((rect_w-textsize_x)/2.0)
-            else:
-                text_x = 0
-                label = label[0:rect_w]
+                if textsize_x <= rect_w:
+                    text_x = int((rect_w-textsize_x)/2.0)
+                else:
+                    text_x = 0
+                    label = label[0:rect_w]
 
-            # (x,y))
-            """
-            0,0                                                              img_width,0
-            
-            
-            
-            0, img_height - img_height*5%             img_width, img_height - img_height*5%
-            
-            0,img_height                                             img_width, img_height
-            """
-            cv2.rectangle(overlay, pt1=(0, img_height), pt2=(rect_w, rect_y), color=(255, 255, 255), thickness=-1)
-            img_new = cv2.addWeighted(overlay, alpha, img, 1-alpha, 0)
-            cv2.putText(img_new, label, (text_x, text_y), text_font, font_scale, (0, 0, 0), 2)
-            cv2.imwrite(label_img_name, img_new)
+                # (x,y))
+                """
+                0,0                                                              img_width,0
+                
+                
+                
+                0, img_height - img_height*5%             img_width, img_height - img_height*5%
+                
+                0,img_height                                             img_width, img_height
+                """
+                cv2.rectangle(overlay, pt1=(0, img_height), pt2=(rect_w, rect_y), color=(255, 255, 255), thickness=-1)
+                img_new = cv2.addWeighted(overlay, alpha, img, 1-alpha, 0)
+                cv2.putText(img_new, label, (text_x, text_y), text_font, font_scale, (0, 0, 0), 2)
+                cv2.imwrite(label_img_name, img_new)
```

### Comparing `ssoss-0.3.15/src/ssoss/ssoss_cli.py` & `ssoss-0.3.16/src/ssoss/ssoss_cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,34 @@
 import argparse
 import process_road_objects
 import process_video
 
 
+def args_static_obj_gpx_video(static_obj="", gpx_file="", video_file="",
+                              vid_sync=("",""), frame_extract=("",""), extra_out=(True, False)):
+    sightings = ""
+    if static_obj and gpx_file:
+        project = process_road_objects.ProcessRoadObjects(gpx_file.name, static_obj.name)
+        sightings = project.intersection_checks()
+    elif static_obj:
+        process_road_objects.ProcessRoadObjects("", static_obj.name)
+    elif gpx_file:
+        process_road_objects.ProcessRoadObjects(gpx_file.name, "")
+
+    if video_file:
+        video = process_video.ProcessVideo(video_file.name)
+        if vid_sync[0] and vid_sync[1]:
+            video.sync(int(vid_sync[0]), vid_sync[1])
+            if sightings:
+                video.extract_sightings(sightings, project, label_img=extra_out[0], gen_gif=extra_out[1])
+        elif frame_extract[0] and frame_extract[1]:
+            print("extracting frames...")
+            video.extract_frames_between(frame_extract[0], frame_extract[1])
+
+
 def main():
     parser = argparse.ArgumentParser(
     prog="Safe Sightings of Signs and Signals",
     description="A Python tool to verify visible traffic signs and signals using GPX and Video files")
 
     gpx_group = parser.add_argument_group(
         "Static Objects and GPX Input",
@@ -41,47 +63,44 @@
     # Video file arguments
     video_group.add_argument("-v", "--video_file",
                             metavar="Video File",
                             help="Video file to process",
                             type=argparse.FileType('r')
                             )
 
-
-
-    # extract frames based on video frame and timestamp
-
     # extract frames based on start and end time of video
     video_extract_group.add_argument("-fxs", "--frame_extract_start", help="Start extract frames in video (seconds)", type=int, nargs=1)
     video_extract_group.add_argument("-fxe", "--frame_extract_end", help="End Extract frames in video (seconds)",
                                     type=int, nargs=1)
 
     video_sync_group.add_argument("-sf", "--sync_frame", help="Sync Frame number for video. Sync with timestamp also", type=int)
     video_sync_group.add_argument("-st", "--sync_timestamp", help="2. Sync Timestamp ('2022-10-24T14:21:54.988Z') for video. Sync with frame number also", type=str)
 
-    video_sync_group.add_argument("--labelbox", help="Include descriptive label on bottom of image", action="store_false")
-    video_sync_group.add_argument("--gif", help="Generate GIF of Sight Distance", action="store_false")
-
-    args = parser.parse_args()
+    video_sync_group.add_argument("--labelbox", help="Include descriptive label on bottom of image", action="store_true")
+    video_sync_group.add_argument("--gif", help="Generate GIF of Sight Distance", action="store_true")
 
-    if args.gpx_file and args.static_objects:
-        project = process_road_objects.ProcessRoadObjects(args.gpx_file.name, args.static_objects.name)
-        sightings = project.intersection_checks()
 
-    if args.video_file is not None:
-        video = process_video.ProcessVideo(args.video_file.name)
-        if args.sync_frame and args.sync_timestamp:
-            print(args.sync_frame)
-            print(args.sync_timestamp)
-            video.sync(int(args.sync_frame), args.sync_timestamp)
-            if args.static_objects and args.gpx_file:
-                video.extract_sightings(sightings, project, gen_gif=args.gif)
-        elif args.frame_extract_start and args.frame_extract_end:
-            video.extract_frames_between(args.frame_extract_start[0], args.frame_extract_end[0])
+    # process args depending on filled in values
+    args = parser.parse_args()
 
+    sync_input = ("", "")
+    frames = ("", "")
+    if args.sync_frame and args.sync_timestamp:
+        sync_input = (args.sync_frame, args.sync_timestamp)
+    if args.frame_extract_start and args.frame_extract_end:
+        frames = (args.frame_extract_start[0], args.frame_extract_end[0])
+    if args.labelbox and args.gif:
+        label_and_gif = (args.labelbox, args.gif)
+    elif args.labelbox:
+        label_and_gif = (args.labelbox, False)
+    elif args.gif:
+        label_and_gif = (False, args.gif)
+    else:
+        label_and_gif = (True, False)
+
+    args_static_obj_gpx_video(args.static_objects, args.gpx_file,
+                              args.video_file,
+                              sync_input, frames, label_and_gif)
 
 
 if __name__ == "__main__":
-    main()
-
-
-
-
+    main()
```

### Comparing `ssoss-0.3.15/src/ssoss/ssoss_gui.py` & `ssoss-0.3.16/src/ssoss/ssoss_gui.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 from gooey import Gooey, GooeyParser
-
+from ssoss_cli import *
 
 import process_road_objects
 import process_video
 
 
 @Gooey(program_name="Safe Sightings of Signs and Signals") #  , tabbed_groups=True
 def main():
@@ -53,43 +53,45 @@
                             help="Video file to process",
                             type=argparse.FileType('r'),
                             widget="FileChooser",
                             gooey_options={'wildcard': "All files (*.*)|*.*",
                                         'message': "Select Video File"})
 
 
-
-    # extract frames based on video frame and timestamp
-
     # extract frames based on start and end time of video
     video_extract_group.add_argument("-fxs", "--frame_extract_start", metavar="A. Start Frame Extract", help="Start extract frames in video (seconds)", type=int, nargs=1)
     video_extract_group.add_argument("-fxe", "--frame_extract_end", metavar="B. End Frame Extract", help="End Extract frames in video (seconds)",
                                     type=int, nargs=1)
 
     video_sync_group.add_argument("-sf", "--sync_frame", metavar="1. Sync Frame", help="Sync Frame number for video. Sync with timestamp also", type=int)
     video_sync_group.add_argument("-st", "--sync_timestamp", metavar="2. Sync Timestamp", help="2. Sync Timestamp ('2022-10-24T14:21:54.988Z') for video. Sync with frame number also", type=str)
 
     video_sync_group.add_argument("-lb", "--labelbox", metavar="Overlay Image Label", help="Include descriptive label on bottom of image", action="store_true", default=True)
-    video_sync_group.add_argument("-g", "--gif", metavar="Create Animated GIF", help="Generate GIF of Sight Distance", action="store_true", default=False)
+    video_sync_group.add_argument("-gif", "--gif", metavar="Create Animated GIF", help="Generate GIF of Sight Distance", action="store_true", default=False)
 
     args = parser.parse_args()
 
-    if args.gpx_file and args.static_objects:
-        project = process_road_objects.ProcessRoadObjects(args.gpx_file.name, args.static_objects.name)
-        sightings = project.intersection_checks()
-
-    if args.video_file is not None:
-        video = process_video.ProcessVideo(args.video_file.name)
-        if args.sync_frame and args.sync_timestamp:
-            video.sync(float(args.sync_frame), args.sync_timestamp)
-            if args.static_objects and args.gpx_file:
-                video.extract_sightings(sightings, project)
-        elif args.frame_extract_start and args.frame_extract_end:
-            video.extract_frames_between(args.frame_extract_start[0], args.frame_extract_end[0])
-
+    sync_input = ("", "")
+    frames = ("", "")
+    if args.sync_frame and args.sync_timestamp:
+        sync_input = (args.sync_frame, args.sync_timestamp)
+    if args.frame_extract_start and args.frame_extract_end:
+        frames = (args.frame_extract_start[0], args.frame_extract_end[0])
+    if args.labelbox and args.gif:
+        label_and_gif = (args.labelbox, args.gif)
+    elif args.labelbox:
+        label_and_gif = (args.labelbox, False)
+    elif args.gif:
+        label_and_gif = (False, args.gif)
+    else:
+        label_and_gif = (True, False)
+
+    args_static_obj_gpx_video(args.static_objects, args.gpx_file,
+                                        args.video_file,
+                                        sync_input, frames, label_and_gif)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ssoss-0.3.15/src/ssoss/static_road_object.py` & `ssoss-0.3.16/src/ssoss/static_road_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # !/usr/bin/env python
 # coding: utf-8
 
 import math
-import geopy
-import geopy.distance
+import geopy, geopy.distance
 
 
 class StaticRoadObject:
 
     def __init__(self, id_num: int, name: str, obj_type: type,
                  ctr_pt: geopy.Point, spd_sd: dict):
         """initializes values related to static road objects
@@ -83,15 +82,15 @@
         :param stop_bar_sb: tuple of two geopy Points (both with (lat,lon)) for SB approach stop bar*
         :param stop_bar_wb: tuple of two geopy Points (both with (lat,lon)) for WB approach stop bar*
 
         *Note: left point (inside lane) is [0] in tuple, right point (right turn lane) is [1] in tuple
 
         """
 
-        self.stop_bar = None
+        self.stop_bar = None  # why is this here?
         self.spd = spd
         self.ctr_pnt = ctr_pnt
         self.bearing = bearing
         self.spd_sd = {
             -999: 0,
             20: 175,
             25: 215,
@@ -208,35 +207,39 @@
 
         :param dynamic_pt: geopy point object of dynamic object
         :param direction: index for heading of dynamic object
         :return: distance in feet as float from dynamic point to stop bar of approaching intersection
         """
 
         # length of stop bar
-        a = geopy.distance.distance(self.stop_bar_d[direction][0],
+        if self.stop_bar_d[direction][0] is False or self.stop_bar_d[direction][1] is False:
+            dist_to_ctr = geopy.distance.distance(self.pt, dynamic_pt).ft
+            return dist_to_ctr
+        else:
+            a = geopy.distance.distance(self.stop_bar_d[direction][0],
                                     self.stop_bar_d[direction][1]).ft
 
         # if length of stop bar is zero, use center of intersection point.
-        if a <= 0 or self.stop_bar is None:
-            dis_to_ctr = geopy.distance.distance(self.pt, dynamic_pt).ft
-            return dis_to_ctr
-        else:
-            # distance from dynamic point to inside lane stop bar point
-            b = geopy.distance.distance(self.stop_bar[direction][0], dynamic_pt).ft
-            # distance from dynamic point to outside lane stop bar point
-            c = geopy.distance.distance(self.stop_bar[direction][1], dynamic_pt).ft
-
-        # calculate perpendicular distance between stop bar and dynamic object
-        if a is not None and b is not None and c is not None:
-            s = (a + b + c) / 2
-            dis_to_sb = 2. * math.sqrt(abs(s * (s - a) * (s - b) *
-                                           (s - c))) / a
-            return dis_to_sb
-        else:
-            return 0
+            if a <= 0 or self.stop_bar_d is None:
+                dist_to_ctr = geopy.distance.distance(self.pt, dynamic_pt).ft
+                return dist_to_ctr
+            else:
+                # distance from dynamic point to inside lane stop bar point
+                b = geopy.distance.distance(self.stop_bar_d[direction][0], dynamic_pt).ft
+                # distance from dynamic point to outside lane stop bar point
+                c = geopy.distance.distance(self.stop_bar_d[direction][1], dynamic_pt).ft
+
+            # calculate perpendicular distance between stop bar and dynamic object
+            if a is not None and b is not None and c is not None:
+                s = (a + b + c) / 2
+                dist_to_sb = 2. * math.sqrt(abs(s * (s - a) * (s - b) *
+                                               (s - c))) / a
+                return dist_to_sb
+            else:
+                return 0
 
 
 def main():
     print("Initialize and Load Static Road Object File")
     print("Copy CSV file into ./in/ folder, where ./ is the current directory")
```

### Comparing `ssoss-0.3.15/LICENSE.txt` & `ssoss-0.3.16/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssoss-0.3.15/README.md` & `ssoss-0.3.16/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Safe Sightings of Signs and Signals (SSOSS)
 
-SSOSS is a Python package that helps you verify if traffic signs and signals are visible or obstructed. This is a 
-streamlined and repeatable process to monitor signs and signals along any roadway using a simple input file (.CSV) as well as
-GPS recorded data file (.GPX) and a synchronized recorded video file.
+SSOSS is a software tool that automates the difficult aspects of verifying if traffic signs and signals are visible or obstructed on a roadway network. This is a 
+streamlined and repeatable process to monitor signs and signals along any roadway using a simple input file (.CSV), GPS recorded data file (.GPX) and a synchronized recorded video file.
 
 ## Features
 * Video Synchronization Helper Tools: Python methods are provided to export the video frames and help to synchronize the video file.
 * Automated data processing: The SSOSS scripts uses a combination of GPS and video data to extract images of traffic signals and/or roadway signs.
 * Image Labeling and animated GIF image tools: Python functions are included to label images or create an animated GIF from multiple images 
 
 ## Requirements
@@ -21,38 +20,42 @@
 ## Usage
 To use the SSOSS program, 
 1. Setup the necessary input files in A and B. 
 2. Follow the data processing commands in Part C. Jupyter Notebook available as example
 
 ### A. Input Files
 Data related to the static road objects (signs and traffic signals) need to be saved in a CSV file for used in processing.
-The intersection CSV file has the following format (as a minimum)
+The intersection CSV file has the following format (as a minimum):
 
 ID, Streetname 1, Streetname 2, Center_Latitude, Center_Longitude, Posted Speed (MPH) of NB Approach, Posted Speed (MPH) of EB Approach, 
 Posted Speed (MPH) of SB Approach, Posted Speed (MPH) of WB Approach, NB Approach Compass Heading, EB Approach Compass Heading,
 SB Approach Compass Heading, WB Approach Compass Heading
 
 ### B. Data Collection
 Collect data simultaneously:
 1. GPX recording
    a. Use GPX Version 1.0 with logging every second
 2. Video Recording
    a. Record at 5 Megapixel resolution or more
    b. Record at 30 frames per second or higher
 
-### C. Data Processing
-See example notebooks (coming soon)
-#### File Setup
-Save Signal .CSV to:
-./in/
+### C. Data Processing: Argparse Command Line
+```Shell
+(ssoss_virtual_env) python ssoss_cli.py -h
+```
+
+#### Basic Usage
+```Shell
+(ssoss_virtual_env) python ssoss_cli.py --static_objects signals.csv --gpx_file drive.gpx --video_file vid.mov 
+                                        --sync_frame 456 --sync_timestamp 2022-10-24T14:21:54.32Z
+```
+
 
-Save GPX and Video files to:
-./in/gpx_video/
 
-#### Example Usage
+#### Python Notebook
 
 ```python
     import ssoss as ss
 
 signals_csv = "signal"  # .csv is omitted
 gpx_file = "drive_1"  # .gpx is omitted
 
@@ -69,38 +72,34 @@
 
 #### Sync GPX & Video Process
 Synchronizing the GPX file and the video could be one of the largest sources of error. The ProcessVideo Class has
 a helper function to perform a accurate synchronization time. The extract_frames_between method can export all the 
 video frames between two time vales. When looking at the GPX points, the approximate video time can be estimated 
 and all the frames can be extracted. This method is:
 
-```python
-        video.extract_frames_between(start_sec=20, end_sec=40)
+```Shell
+        (ssoss_virtual_env) python ssoss_cli.py -video_file vid.mov --frame_extract_start 4 --frame_extract_end 6
 ```
 
 Check the printed logs to see the saved output location. Default is:
-./out/frames/[video filename]/###.jpg
+./out/[video filename]/frames/###.jpg
 where ### is the frame number of the image.
 
 Use the frame number and the GPX recorded time to line up the best point to synchronize the video using the Sync method.
-```python
-         video.sync(frame = 200, timestamp="2022-10-24T16:45:54.988Z")
-```
 
 ## Documentation
-### Jupter Notebook Examples
-coming soon
+
 ### Helper Function: GIF Creator
 Create a gif from multiple images around the sight distance location. This can be helpful if the lens is out of focus
 at an extracted frame, or just more context before and after a sight distance is needed.
 
 ```python
         video.extract_sightings(sightings, signal_project, gen_gif=True)
 ```
-Saves .gif file in ./out/frames/ [video filename] /gif/
+Saves .gif file in ./out/[video filename]/gif/
 
 ### Heuristic
 
 For Each GPX Point:
 * What are the closest & approaching intersections
   * Based on compass heading of moving vehicle and input data (.csv), which approach leg is vehicle on?
     * What is the approach speed of that approach leg, and look up sight distance for that speed
```

### Comparing `ssoss-0.3.15/pyproject.toml` & `ssoss-0.3.16/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ssoss"
-version = "0.3.15"
+version = "0.3.16"
 authors = [
   { name="Matt Redmond", email="mr2742@gmail.com" },
 ]
 description = "Safe Sightings of Signs and Signals Package"
 keywords = ["traffic signals","sight distance", "gpx", "video"]
 dynamic = ["dependencies"]
 readme = "README.md"
```

### Comparing `ssoss-0.3.15/PKG-INFO` & `ssoss-0.3.16/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssoss
-Version: 0.3.15
+Version: 0.3.16
 Summary: Safe Sightings of Signs and Signals Package
 Project-URL: Homepage, https://github.com/swerty24/ssoss
 Project-URL: Bug Tracker, https://github.com/swerty24/ssoss/issues
 Author-email: Matt Redmond <mr2742@gmail.com>
 License-File: LICENSE.txt
 Keywords: gpx,sight distance,traffic signals,video
 Classifier: License :: OSI Approved :: MIT License
@@ -24,17 +24,16 @@
 Requires-Dist: pytz==2022.4
 Requires-Dist: six==1.15.0
 Requires-Dist: tqdm==4.64.1
 Description-Content-Type: text/markdown
 
 # Safe Sightings of Signs and Signals (SSOSS)
 
-SSOSS is a Python package that helps you verify if traffic signs and signals are visible or obstructed. This is a 
-streamlined and repeatable process to monitor signs and signals along any roadway using a simple input file (.CSV) as well as
-GPS recorded data file (.GPX) and a synchronized recorded video file.
+SSOSS is a software tool that automates the difficult aspects of verifying if traffic signs and signals are visible or obstructed on a roadway network. This is a 
+streamlined and repeatable process to monitor signs and signals along any roadway using a simple input file (.CSV), GPS recorded data file (.GPX) and a synchronized recorded video file.
 
 ## Features
 * Video Synchronization Helper Tools: Python methods are provided to export the video frames and help to synchronize the video file.
 * Automated data processing: The SSOSS scripts uses a combination of GPS and video data to extract images of traffic signals and/or roadway signs.
 * Image Labeling and animated GIF image tools: Python functions are included to label images or create an animated GIF from multiple images 
 
 ## Requirements
@@ -49,38 +48,42 @@
 ## Usage
 To use the SSOSS program, 
 1. Setup the necessary input files in A and B. 
 2. Follow the data processing commands in Part C. Jupyter Notebook available as example
 
 ### A. Input Files
 Data related to the static road objects (signs and traffic signals) need to be saved in a CSV file for used in processing.
-The intersection CSV file has the following format (as a minimum)
+The intersection CSV file has the following format (as a minimum):
 
 ID, Streetname 1, Streetname 2, Center_Latitude, Center_Longitude, Posted Speed (MPH) of NB Approach, Posted Speed (MPH) of EB Approach, 
 Posted Speed (MPH) of SB Approach, Posted Speed (MPH) of WB Approach, NB Approach Compass Heading, EB Approach Compass Heading,
 SB Approach Compass Heading, WB Approach Compass Heading
 
 ### B. Data Collection
 Collect data simultaneously:
 1. GPX recording
    a. Use GPX Version 1.0 with logging every second
 2. Video Recording
    a. Record at 5 Megapixel resolution or more
    b. Record at 30 frames per second or higher
 
-### C. Data Processing
-See example notebooks (coming soon)
-#### File Setup
-Save Signal .CSV to:
-./in/
+### C. Data Processing: Argparse Command Line
+```Shell
+(ssoss_virtual_env) python ssoss_cli.py -h
+```
+
+#### Basic Usage
+```Shell
+(ssoss_virtual_env) python ssoss_cli.py --static_objects signals.csv --gpx_file drive.gpx --video_file vid.mov 
+                                        --sync_frame 456 --sync_timestamp 2022-10-24T14:21:54.32Z
+```
+
 
-Save GPX and Video files to:
-./in/gpx_video/
 
-#### Example Usage
+#### Python Notebook
 
 ```python
     import ssoss as ss
 
 signals_csv = "signal"  # .csv is omitted
 gpx_file = "drive_1"  # .gpx is omitted
 
@@ -97,38 +100,34 @@
 
 #### Sync GPX & Video Process
 Synchronizing the GPX file and the video could be one of the largest sources of error. The ProcessVideo Class has
 a helper function to perform a accurate synchronization time. The extract_frames_between method can export all the 
 video frames between two time vales. When looking at the GPX points, the approximate video time can be estimated 
 and all the frames can be extracted. This method is:
 
-```python
-        video.extract_frames_between(start_sec=20, end_sec=40)
+```Shell
+        (ssoss_virtual_env) python ssoss_cli.py -video_file vid.mov --frame_extract_start 4 --frame_extract_end 6
 ```
 
 Check the printed logs to see the saved output location. Default is:
-./out/frames/[video filename]/###.jpg
+./out/[video filename]/frames/###.jpg
 where ### is the frame number of the image.
 
 Use the frame number and the GPX recorded time to line up the best point to synchronize the video using the Sync method.
-```python
-         video.sync(frame = 200, timestamp="2022-10-24T16:45:54.988Z")
-```
 
 ## Documentation
-### Jupter Notebook Examples
-coming soon
+
 ### Helper Function: GIF Creator
 Create a gif from multiple images around the sight distance location. This can be helpful if the lens is out of focus
 at an extracted frame, or just more context before and after a sight distance is needed.
 
 ```python
         video.extract_sightings(sightings, signal_project, gen_gif=True)
 ```
-Saves .gif file in ./out/frames/ [video filename] /gif/
+Saves .gif file in ./out/[video filename]/gif/
 
 ### Heuristic
 
 For Each GPX Point:
 * What are the closest & approaching intersections
   * Based on compass heading of moving vehicle and input data (.csv), which approach leg is vehicle on?
     * What is the approach speed of that approach leg, and look up sight distance for that speed
```

