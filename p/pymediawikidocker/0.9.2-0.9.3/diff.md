# Comparing `tmp/pymediawikidocker-0.9.2.tar.gz` & `tmp/pymediawikidocker-0.9.3.tar.gz`

## Comparing `pymediawikidocker-0.9.2.tar` & `pymediawikidocker-0.9.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/.pydevproject
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/.DS_Store
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/__init__.py
--rw-r--r--   0        0        0     9673 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/config.py
--rw-r--r--   0        0        0    22762 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/docker.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/html_table.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/logger.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/mariadb.py
--rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/mw.py
--rw-r--r--   0        0        0     8314 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/mwcluster.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/version.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/webscrape.py
--rw-r--r--   0        0        0    11593 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/extensions.json
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/addCronTabEntry.sh
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/addSysopUser.sh
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/initdb.sh
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/installExtensions.sh
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/mwCompose.yml
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/mwDockerfile
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/mwLocalSettings.php
--rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/mwLocalSettings127.php
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/mwLocalSettings131.php
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/mwLocalSettings135.php
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/mwLocalSettings136.php
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/mwLocalSettings137.php
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/mwLocalSettings138.php
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/mwLocalSettings139.php
--rw-r--r--   0        0        0    56849 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/mwWiki127.sql
--rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/mwWiki131.sql
--rw-r--r--   0        0        0    64022 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/mwWiki135.sql
--rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/mwWiki136.sql
--rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/mwWiki137.sql
--rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/mwWiki138.sql
--rw-r--r--   0        0        0    64483 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/mwWiki139.sql
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/phpinfo.php
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/plantuml.sh
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/startRunJobs.sh
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/update.sh
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/mwdocker/resources/templates/upload.ini
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/scripts/install
--rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/tests/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/tests/basetest.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/tests/test_config.py
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/tests/test_extensions.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/tests/test_html_tables.py
--rw-r--r--   0        0        0     9690 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/tests/test_install.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/LICENSE
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/README.md
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/.pydevproject
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/.DS_Store
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/__init__.py
+-rw-r--r--   0        0        0     9673 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/config.py
+-rw-r--r--   0        0        0    23246 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/docker.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/html_table.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/logger.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/mariadb.py
+-rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/mw.py
+-rw-r--r--   0        0        0     8314 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/mwcluster.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/version.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/webscrape.py
+-rw-r--r--   0        0        0    11593 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/extensions.json
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/addCronTabEntry.sh
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/addSysopUser.sh
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/initdb.sh
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/installExtensions.sh
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwCompose.yml
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwDockerfile
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings.php
+-rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings127.php
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings131.php
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings135.php
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings136.php
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings137.php
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings138.php
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings139.php
+-rw-r--r--   0        0        0    56849 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki127.sql
+-rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki131.sql
+-rw-r--r--   0        0        0    64022 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki135.sql
+-rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki136.sql
+-rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki137.sql
+-rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki138.sql
+-rw-r--r--   0        0        0    64483 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki139.sql
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/phpinfo.php
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/plantuml.sh
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/startRunJobs.sh
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/update.sh
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/upload.ini
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/scripts/install
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/tests/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/tests/basetest.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/tests/test_config.py
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/tests/test_extensions.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/tests/test_html_tables.py
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/tests/test_install.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/LICENSE
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/README.md
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/PKG-INFO
```

### Comparing `pymediawikidocker-0.9.2/.github/workflows/build.yml` & `pymediawikidocker-0.9.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/.github/workflows/upload-to-pypi.yml` & `pymediawikidocker-0.9.3/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/.DS_Store` & `pymediawikidocker-0.9.3/mwdocker/.DS_Store`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/config.py` & `pymediawikidocker-0.9.3/mwdocker/config.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/docker.py` & `pymediawikidocker-0.9.3/mwdocker/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,32 @@
         Returns:
             bool: True if the container is not None
         """
         ok=self.container.state.running
         msg=f"mediawiki {self.kind} container {self.name}"
         return Logger.check_and_log(msg, ok) 
     
+    def getHostPort(self,local_port:int=80)->int:
+        """
+        get the host port for the given local port
+        
+        Args:
+            local_port(int): the local port to get the mapping for
+            
+        Returns:
+            int: the  host port or None
+        """
+        host_port=None
+        pb_dict=self.container.host_config.port_bindings
+        p_local=f"{local_port}/tcp"
+        if p_local in pb_dict:
+            pb=pb_dict[p_local][0]
+            host_port=pb.host_port
+        return host_port
+    
 @dataclass
 class DBStatus():
     """
     the Database Status
     """
     attempts: int
     max_tries: int
@@ -151,30 +169,28 @@
         if not mw:
             print("mediawiki container missing")
             exitCode=1
         if  not db:
             print("database container missing")
             exitCode=1
         if mw and db and mw.check() and db.check():
-            pb_dict=mw.container.host_config.port_bindings
-            p80="80/tcp"
-            if p80 in pb_dict:
-                pb=pb_dict[p80][0]
-                host_port=pb.host_port
+            host_port=mw.getHostPort(80)
+            if host_port:
                 Logger.check_and_log_equal(f"port binding",host_port,"expected  port",str(self.config.port))
                 url=self.config.url
                 # fix url to local port
+                # @TODO isn't this superfluous / has no effect ...?
                 url=url.replace(str(self.config.port),host_port)
                 version_url=f"{url}/index.php/Special:Version"
                 
                 ok=self.checkWiki(version_url)
                 if not ok:
                     exitCode=1
             else:
-                self.log(f"port binding {p80} missing",False)
+                self.log(f"port binding for port 80 missing",False)
                 exitCode=1
             pass
         return exitCode
     
     def checkWiki(self,version_url:str)->bool:
         """
         check this wiki against the content of the given version_url
```

### Comparing `pymediawikidocker-0.9.2/mwdocker/html_table.py` & `pymediawikidocker-0.9.3/mwdocker/html_table.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/logger.py` & `pymediawikidocker-0.9.3/mwdocker/logger.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/mariadb.py` & `pymediawikidocker-0.9.3/mwdocker/mariadb.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/mw.py` & `pymediawikidocker-0.9.3/mwdocker/mw.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/mwcluster.py` & `pymediawikidocker-0.9.3/mwdocker/mwcluster.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/version.py` & `pymediawikidocker-0.9.3/mwdocker/version.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/webscrape.py` & `pymediawikidocker-0.9.3/mwdocker/webscrape.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/resources/extensions.json` & `pymediawikidocker-0.9.3/mwdocker/resources/extensions.json`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/resources/templates/mwCompose.yml` & `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwCompose.yml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/resources/templates/mwDockerfile` & `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwDockerfile`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/resources/templates/mwLocalSettings.php` & `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/resources/templates/mwLocalSettings127.php` & `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings127.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/resources/templates/mwLocalSettings131.php` & `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings131.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/resources/templates/mwLocalSettings135.php` & `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings135.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/resources/templates/mwLocalSettings136.php` & `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings136.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/resources/templates/mwLocalSettings137.php` & `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings137.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/resources/templates/mwLocalSettings138.php` & `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings138.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/resources/templates/mwLocalSettings139.php` & `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings139.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/resources/templates/mwWiki127.sql` & `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki127.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/resources/templates/mwWiki131.sql` & `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki131.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/resources/templates/mwWiki135.sql` & `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki135.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/resources/templates/mwWiki136.sql` & `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki136.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/resources/templates/mwWiki137.sql` & `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki137.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/resources/templates/mwWiki138.sql` & `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki138.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/resources/templates/mwWiki139.sql` & `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki139.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/mwdocker/resources/templates/plantuml.sh` & `pymediawikidocker-0.9.3/mwdocker/resources/templates/plantuml.sh`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/tests/basetest.py` & `pymediawikidocker-0.9.3/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/tests/test_config.py` & `pymediawikidocker-0.9.3/tests/test_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -47,8 +47,20 @@
         args = parser.parse_args(argv)
         mwClusterConfig.fromArgs(args)
         mwd=dataclasses.asdict(mwClusterConfig)
         debug=self.debug
         #debug=True
         if debug:
             print(json.dumps(mwd,indent=2))
-        self.assertEqual("https",mwClusterConfig.prot)
+        self.assertEqual("https",mwClusterConfig.prot)
+        
+    def test_random_password(self):
+        """
+        test the random password generation
+        """
+        config=MwClusterConfig()
+        for length,chars in [(11,15),(13,18),(15,20)]:
+            rp=config.random_password(length)
+            debug=self.debug
+            if debug:
+                print(f"{length} bytes:{len(rp)} chars:{rp}")
+            self.assertEqual(chars,len(rp))
```

### Comparing `pymediawikidocker-0.9.2/tests/test_extensions.py` & `pymediawikidocker-0.9.3/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/tests/test_html_tables.py` & `pymediawikidocker-0.9.3/tests/test_html_tables.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/tests/test_install.py` & `pymediawikidocker-0.9.3/tests/test_install.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,14 +132,31 @@
             self.assertTrue(dbStatus.ok)
             userCountRecords=mwApp.sqlQuery("select count(*) from user;")
             print(userCountRecords)
         mwCluster.close()
         exitCode=mwCluster.check()
         self.assertEqual(0,exitCode)
         
+    def testPortBindingAccess(self):
+        """
+        https://github.com/WolfgangFahl/pymediawikidocker/issues/48
+        
+        refactor port binding access 
+        """    
+        mwCluster=self.getMwCluster(withGenerate=False)
+        apps=mwCluster.apps.values()
+        for mwApp in apps:
+            self.assertTrue(mwApp.dbContainer is not None)
+            self.assertTrue(mwApp.mwContainer is not None)
+            browser_port=mwApp.mwContainer.getHostPort(80)
+            sql_port=mwApp.dbContainer.getHostPort(3306)
+            self.assertEqual(str(browser_port),str(mwApp.config.port))
+            self.assertEqual(str(sql_port),str(mwApp.config.sqlPort))
+            pass
+        
     def testSocketGetHostname(self):
         """
         test for https://github.com/python/cpython/issues/79345
         """
         debug=self.debug
         #debug=True
         for i,hostname in enumerate([socket.gethostname(),socket.getfqdn()]):
@@ -223,14 +240,15 @@
         test the wikiUser handling
         '''
         mwCluster=self.getMwCluster()
         for mwApp in mwCluster.apps.values():
             wikiUser=mwApp.createWikiUser(store=False)
             if self.debug:
                 print(wikiUser)
+            self.assertEqual(wikiUser.wikiId,mwApp.config.container_base_name)
             pass
         
     def testMwClusterCommandLine(self):
         '''
         test the mwCluster Command Line
         '''
         for argv,expected in [
```

### Comparing `pymediawikidocker-0.9.2/.gitignore` & `pymediawikidocker-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/LICENSE` & `pymediawikidocker-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/README.md` & `pymediawikidocker-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/pyproject.toml` & `pymediawikidocker-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.2/PKG-INFO` & `pymediawikidocker-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymediawikidocker
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python controlled (semantic) mediawiki docker application cluster installation
 Project-URL: Home, https://github.com/WolfgangFahl/pymediawikidocker
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/pymediawikidocker
 Project-URL: Source, https://github.com/WolfgangFahl/pymediawikidocker
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License: Apache-2.0
```

