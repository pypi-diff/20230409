# Comparing `tmp/pioreactor_logs2slack-0.1.1-py3-none-any.whl.zip` & `tmp/pioreactor_logs2slack-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,9 @@
-Zip file size: 4863 bytes, number of entries: 9
--rw-r--r--  2.0 unx     2025 b- defN 22-Sep-22 15:23 pioreactor_logs2slack/__init__.py
--rw-r--r--  2.0 unx       46 b- defN 21-Oct-11 15:06 pioreactor_logs2slack/additional_config.ini
--rw-r--r--  2.0 unx      160 b- defN 22-Aug-24 16:09 pioreactor_logs2slack/ui/contrib/jobs/logs2slack.yaml
--rw-r--r--  2.0 unx     1079 b- defN 22-Sep-22 15:26 pioreactor_logs2slack-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2194 b- defN 22-Sep-22 15:26 pioreactor_logs2slack-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Sep-22 15:26 pioreactor_logs2slack-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 22-Sep-22 15:26 pioreactor_logs2slack-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 22-Sep-22 15:26 pioreactor_logs2slack-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      862 b- defN 22-Sep-22 15:26 pioreactor_logs2slack-0.1.1.dist-info/RECORD
-9 files, 6547 bytes uncompressed, 3333 bytes compressed:  49.1%
+Zip file size: 4275 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     2121 b- defN 23-Apr-09 00:00 pioreactor_logs2slack/__init__.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-Apr-09 00:01 pioreactor_logs2slack-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2187 b- defN 23-Apr-09 00:01 pioreactor_logs2slack-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 00:01 pioreactor_logs2slack-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 23-Apr-09 00:01 pioreactor_logs2slack-0.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-09 00:01 pioreactor_logs2slack-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      655 b- defN 23-Apr-09 00:01 pioreactor_logs2slack-0.1.2.dist-info/RECORD
+7 files, 6223 bytes uncompressed, 3089 bytes compressed:  50.4%
```

## zipnote {}

```diff
@@ -1,28 +1,22 @@
 Filename: pioreactor_logs2slack/__init__.py
 Comment: 
 
-Filename: pioreactor_logs2slack/additional_config.ini
+Filename: pioreactor_logs2slack-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: pioreactor_logs2slack/ui/contrib/jobs/logs2slack.yaml
+Filename: pioreactor_logs2slack-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: pioreactor_logs2slack-0.1.1.dist-info/LICENSE
+Filename: pioreactor_logs2slack-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: pioreactor_logs2slack-0.1.1.dist-info/METADATA
+Filename: pioreactor_logs2slack-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pioreactor_logs2slack-0.1.1.dist-info/WHEEL
+Filename: pioreactor_logs2slack-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pioreactor_logs2slack-0.1.1.dist-info/entry_points.txt
-Comment: 
-
-Filename: pioreactor_logs2slack-0.1.1.dist-info/top_level.txt
-Comment: 
-
-Filename: pioreactor_logs2slack-0.1.1.dist-info/RECORD
+Filename: pioreactor_logs2slack-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pioreactor_logs2slack/__init__.py

```diff
@@ -1,59 +1,60 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import json
 import logging
+
 import click
-from requests import post
-from pioreactor.background_jobs.base import BackgroundJob
+from pioreactor.background_jobs.base import BackgroundJobContrib
 from pioreactor.config import config
-from pioreactor.whoami import get_unit_name, get_latest_experiment_name
+from pioreactor.mureq import post
+from pioreactor.whoami import get_latest_experiment_name
+from pioreactor.whoami import get_unit_name
 
 
-class Logs2Slack(BackgroundJob):
-    job_name="logs2slack"
+class Logs2Slack(BackgroundJobContrib):
+    job_name = "logs2slack"
 
     def __init__(self, unit, experiment):
         super(Logs2Slack, self).__init__(
-            unit=unit, experiment=experiment
+            unit=unit, experiment=experiment, source="pioreactor_logs2slack"
         )
         self.slack_webhook_url = config.get("logs2slack", "slack_webhook_url")
         if not self.slack_webhook_url:
             self.logger.error("[logs2slack] slack_webhook_url is not defined in your config.ini.")
             raise ValueError("[logs2slack] slack_webhook_url is not defined in your config.ini.")
 
         self.log_level = config.get("logs2slack", "log_level", fallback="INFO")
         self.start_passive_listeners()
 
     def publish_to_slack(self, msg):
         payload = json.loads(msg.payload)
 
         # check to see if we should allow the logs based on the level.
-        if getattr(logging, self.log_level) > getattr(logging, payload['level']):
+        if getattr(logging, self.log_level) > getattr(logging, payload["level"]):
             return
-        elif payload['task'] == self.job_name:
+        elif payload["task"] == self.job_name:
             # avoid an infinite loop, https://github.com/Pioreactor/pioreactor-logs2slack/issues/2
             return
 
         slack_msg = f"[{payload['level']}] [{self.unit}] [{payload['task']}] {payload['message']}"
         encoded_json = json.dumps({"text": slack_msg}).encode("utf-8")
 
         r = post(
-            self.slack_webhook_url, data=encoded_json,
-            headers={'Content-Type': 'application/json'}
+            self.slack_webhook_url, data=encoded_json, headers={"Content-Type": "application/json"}
         )
 
         r.raise_for_status()
 
     def start_passive_listeners(self):
         self.subscribe_and_callback(self.publish_to_slack, f"pioreactor/{self.unit}/+/logs/+")
 
 
 @click.command(name="logs2slack")
 def click_logs2slack():
     """
     turn on logging to Slack
     """
 
-    lg = Logs2Slack(
-        unit=get_unit_name(), experiment=get_latest_experiment_name()
-    )
+    lg = Logs2Slack(unit=get_unit_name(), experiment=get_latest_experiment_name())
     lg.block_until_disconnected()
```

## Comparing `pioreactor_logs2slack-0.1.1.dist-info/LICENSE` & `pioreactor_logs2slack-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pioreactor_logs2slack-0.1.1.dist-info/METADATA` & `pioreactor_logs2slack-0.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pioreactor-logs2slack
-Version: 0.1.1
+Version: 0.1.2
 Summary: Push logs generated by Pioreactors to your Slack workspace
 Home-page: https://github.com/Pioreactor/pioreactor-logs2slack
 Author: Cam Davidson Pilon
 Author-email: cam@pioreactor.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -46,14 +46,7 @@
 ```
 
 Add your webhook URL from step 6. here. Click "Save". You can also change the level of logs to report, see [Python logging levels](https://docs.python.org/3/library/logging.html#logging-levels).
 
 3. In the "Pioreactors" page, you should see "Logs2Slack" as an activity now. You can start this activity like you would any other activity. Go ahead and start it.
 
 4. In your dedicated Slack channel, you should start to see logs arrive!
-
-
-
-
-
-
-
```

## Comparing `pioreactor_logs2slack-0.1.1.dist-info/RECORD` & `pioreactor_logs2slack-0.1.2.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-pioreactor_logs2slack/__init__.py,sha256=aoSmMbCW6YkvU7FH4D8HsxveOj_n8uCq0lBB4na6qf0,2025
-pioreactor_logs2slack/additional_config.ini,sha256=VNHRyohY-tUJ4UWLUSEB3oi87Svh84Nv5KS4DLm5VOk,46
-pioreactor_logs2slack/ui/contrib/jobs/logs2slack.yaml,sha256=8f2tdcw-DgVo-sOQBSynXgRRIXxp26qchmrIXqXtQSk,160
-pioreactor_logs2slack-0.1.1.dist-info/LICENSE,sha256=RTnFva3sXKEPtRcFEvpWgg6NqscwpXrZ0ckNz9x2tlo,1079
-pioreactor_logs2slack-0.1.1.dist-info/METADATA,sha256=IcpF9wkM9GXCYv9mD59VNZ-zqMII-Mta_C0Mxdpocpk,2194
-pioreactor_logs2slack-0.1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pioreactor_logs2slack-0.1.1.dist-info/entry_points.txt,sha256=UGc-TQ_kF5mFe9hPOtoJl-Nc-14P99vkQtdLVEkuocQ,67
-pioreactor_logs2slack-0.1.1.dist-info/top_level.txt,sha256=2QWckvgdEg9ZQN1M279uoBBHPt582EgfduegCyBid44,22
-pioreactor_logs2slack-0.1.1.dist-info/RECORD,,
+pioreactor_logs2slack/__init__.py,sha256=_roeHvN9O5eKznYjOpAuPY0G8i1o9m5F_x6JQ4l247o,2121
+pioreactor_logs2slack-0.1.2.dist-info/LICENSE,sha256=RTnFva3sXKEPtRcFEvpWgg6NqscwpXrZ0ckNz9x2tlo,1079
+pioreactor_logs2slack-0.1.2.dist-info/METADATA,sha256=EGOmnyp_yp98Tq2Sgo3UkKk2xdcoKJBQPCHRM5wN5zQ,2187
+pioreactor_logs2slack-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pioreactor_logs2slack-0.1.2.dist-info/entry_points.txt,sha256=UGc-TQ_kF5mFe9hPOtoJl-Nc-14P99vkQtdLVEkuocQ,67
+pioreactor_logs2slack-0.1.2.dist-info/top_level.txt,sha256=2QWckvgdEg9ZQN1M279uoBBHPt582EgfduegCyBid44,22
+pioreactor_logs2slack-0.1.2.dist-info/RECORD,,
```

