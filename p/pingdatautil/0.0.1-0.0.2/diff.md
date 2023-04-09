# Comparing `tmp/pingdatautil-0.0.1.tar.gz` & `tmp/pingdatautil-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pingdatautil-0.0.1.tar", last modified: Sun Apr  2 16:02:49 2023, max compression
+gzip compressed data, was "pingdatautil-0.0.2.tar", last modified: Sun Apr  9 11:00:54 2023, max compression
```

## Comparing `pingdatautil-0.0.1.tar` & `pingdatautil-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 16:02:49.078290 pingdatautil-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-04-02 15:02:53.000000 pingdatautil-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      231 2023-04-02 15:26:23.000000 pingdatautil-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      142 2023-04-02 16:02:49.078290 pingdatautil-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-04-02 15:02:53.000000 pingdatautil-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-02 16:02:49.068288 pingdatautil-0.0.1/pingdatautil/
--rw-rw-rw-   0        0        0     2294 2023-04-02 15:51:17.000000 pingdatautil-0.0.1/pingdatautil/EngineHelper.py
--rw-rw-rw-   0        0        0     2291 2023-04-02 15:47:17.000000 pingdatautil-0.0.1/pingdatautil/LineNotify.py
--rw-rw-rw-   0        0        0     4087 2023-04-02 15:47:31.000000 pingdatautil-0.0.1/pingdatautil/Logger.py
--rw-rw-rw-   0        0        0     3982 2023-04-02 15:58:25.000000 pingdatautil-0.0.1/pingdatautil/ODBCHelper.py
--rw-rw-rw-   0        0        0      140 2023-04-02 15:43:43.000000 pingdatautil-0.0.1/pingdatautil/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 16:02:49.078290 pingdatautil-0.0.1/pingdatautil.egg-info/
--rw-rw-rw-   0        0        0      142 2023-04-02 16:02:48.000000 pingdatautil-0.0.1/pingdatautil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-04-02 16:02:49.000000 pingdatautil-0.0.1/pingdatautil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 16:02:48.000000 pingdatautil-0.0.1/pingdatautil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-02 16:02:48.000000 pingdatautil-0.0.1/pingdatautil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-02 16:02:49.078290 pingdatautil-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      213 2023-04-02 15:29:12.000000 pingdatautil-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-02 16:02:49.078290 pingdatautil-0.0.1/test/
--rw-rw-rw-   0        0        0      447 2023-04-02 15:59:38.000000 pingdatautil-0.0.1/test/test1.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:00:54.501476 pingdatautil-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-04-02 15:02:53.000000 pingdatautil-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      231 2023-04-02 15:26:23.000000 pingdatautil-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      142 2023-04-09 11:00:54.501476 pingdatautil-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-04-02 15:02:53.000000 pingdatautil-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 11:00:54.487476 pingdatautil-0.0.2/pingdatautil/
+-rw-rw-rw-   0        0        0     6939 2023-04-02 17:34:55.000000 pingdatautil-0.0.2/pingdatautil/AzureStorage.py
+-rw-rw-rw-   0        0        0     6272 2023-04-09 09:04:38.000000 pingdatautil-0.0.2/pingdatautil/DataConnection.py
+-rw-rw-rw-   0        0        0    20872 2023-04-09 10:39:11.000000 pingdatautil-0.0.2/pingdatautil/DataExport.py
+-rw-rw-rw-   0        0        0     2294 2023-04-02 15:51:17.000000 pingdatautil-0.0.2/pingdatautil/EngineHelper.py
+-rw-rw-rw-   0        0        0     7118 2023-04-09 10:55:36.000000 pingdatautil-0.0.2/pingdatautil/ExcelFormatter.py
+-rw-rw-rw-   0        0        0     6294 2023-04-02 16:21:41.000000 pingdatautil-0.0.2/pingdatautil/GoogleDrive.py
+-rw-rw-rw-   0        0        0     5602 2023-04-02 16:20:58.000000 pingdatautil-0.0.2/pingdatautil/GoogleSheet.py
+-rw-rw-rw-   0        0        0    22769 2023-04-07 07:52:34.000000 pingdatautil-0.0.2/pingdatautil/HyperClass.py
+-rw-rw-rw-   0        0        0     8710 2023-04-02 17:03:36.000000 pingdatautil-0.0.2/pingdatautil/JDBCExport.py
+-rw-rw-rw-   0        0        0     4187 2023-04-02 16:59:49.000000 pingdatautil-0.0.2/pingdatautil/JDBCHelper.py
+-rw-rw-rw-   0        0        0     2291 2023-04-02 15:47:17.000000 pingdatautil-0.0.2/pingdatautil/LineNotify.py
+-rw-rw-rw-   0        0        0     4087 2023-04-02 15:47:31.000000 pingdatautil-0.0.2/pingdatautil/Logger.py
+-rw-rw-rw-   0        0        0    15750 2023-04-02 16:44:54.000000 pingdatautil-0.0.2/pingdatautil/ODBCExport.py
+-rw-rw-rw-   0        0        0     3756 2023-04-09 08:31:37.000000 pingdatautil-0.0.2/pingdatautil/ODBCHelper.py
+-rw-rw-rw-   0        0        0      524 2023-04-09 08:49:40.000000 pingdatautil-0.0.2/pingdatautil/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:00:54.491476 pingdatautil-0.0.2/pingdatautil.egg-info/
+-rw-rw-rw-   0        0        0      142 2023-04-09 11:00:54.000000 pingdatautil-0.0.2/pingdatautil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2023-04-09 11:00:54.000000 pingdatautil-0.0.2/pingdatautil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 11:00:54.000000 pingdatautil-0.0.2/pingdatautil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-09 11:00:54.000000 pingdatautil-0.0.2/pingdatautil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 11:00:54.501476 pingdatautil-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      213 2023-04-09 11:00:06.000000 pingdatautil-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:00:54.500475 pingdatautil-0.0.2/test/
+-rw-rw-rw-   0        0        0      903 2023-04-09 08:49:13.000000 pingdatautil-0.0.2/test/test-data-connection.py
+-rw-rw-rw-   0        0        0      503 2023-04-09 09:58:44.000000 pingdatautil-0.0.2/test/test-data-export-2.py
+-rw-rw-rw-   0        0        0     1246 2023-04-09 09:55:34.000000 pingdatautil-0.0.2/test/test-data-export.py
+-rw-rw-rw-   0        0        0      542 2023-04-09 10:56:13.000000 pingdatautil-0.0.2/test/test-excel-format.py
+-rw-rw-rw-   0        0        0      414 2023-04-07 07:38:37.000000 pingdatautil-0.0.2/test/test-hyper1.py
+-rw-rw-rw-   0        0        0      958 2023-04-02 17:22:59.000000 pingdatautil-0.0.2/test/test-hyper2.py
+-rw-rw-rw-   0        0        0      756 2023-04-05 07:30:16.000000 pingdatautil-0.0.2/test/test1.py
+-rw-rw-rw-   0        0        0      356 2023-04-07 02:52:52.000000 pingdatautil-0.0.2/test/test1a.py
+-rw-rw-rw-   0        0        0      779 2023-04-03 04:07:43.000000 pingdatautil-0.0.2/test/test2.py
+-rw-rw-rw-   0        0        0     1375 2023-04-02 17:35:00.000000 pingdatautil-0.0.2/test/test3.py
+-rw-rw-rw-   0        0        0      276 2023-04-05 07:30:30.000000 pingdatautil-0.0.2/test/test4.py
```

### Comparing `pingdatautil-0.0.1/LICENSE` & `pingdatautil-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.1/pingdatautil/EngineHelper.py` & `pingdatautil-0.0.2/pingdatautil/EngineHelper.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.1/pingdatautil/LineNotify.py` & `pingdatautil-0.0.2/pingdatautil/LineNotify.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.1/pingdatautil/Logger.py` & `pingdatautil-0.0.2/pingdatautil/Logger.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.1/pingdatautil/ODBCHelper.py` & `pingdatautil-0.0.2/pingdatautil/ODBCHelper.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,14 +66,21 @@
             self.conn = pyodbc.connect(self.connection_string)
             self.log("Connect to database successfully.")
         except Exception as e:
             self.log("Cannot connect to database", "ERROR")
             self.log(str(e), "ERROR")
             sys.exit(-1)
 
+    def close(self):
+        self.conn.close()
+
+    #########################
+    ### HELPER FUNCTION ###
+    #########################
+
     def count_records(self, sql_command):
         self.log(f"Count records using: {sql_command}")
         try:
             cursor = self.conn.cursor()
             cursor.execute(sql_command)
             row = cursor.fetchone()
             cnt = row[0]
@@ -116,22 +123,7 @@
                 self.log(F"{str(row)}")
             cursor.close()
         except Exception as e:
             self.log(F"{str(e)}", "ERROR")
             cursor.close()
         txt = self.timer_stop()
         return txt
-
-    def close(self):
-        self.conn.close()
-
-
-if __name__ == "__main__":
-    o = ODBCHelper()
-    cs = (
-        F"DRIVER=ODBC Driver 17 for SQL Server;"
-        F"SERVER=localhost;PORT=1433;"
-        F"DATABASE=TEST;UID=sa;PWD=P@ssw0rd;"
-    )
-    o.connect(cs)
-    o.execute_full("SELECT TOP 10 * FROM bnk48_member", with_result=True)
-    o.close()
```

