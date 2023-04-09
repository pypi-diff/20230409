# Comparing `tmp/pymediawikidocker-0.9.3.tar.gz` & `tmp/pymediawikidocker-0.9.4.tar.gz`

## Comparing `pymediawikidocker-0.9.3.tar` & `pymediawikidocker-0.9.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/.pydevproject
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/.DS_Store
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/__init__.py
--rw-r--r--   0        0        0     9673 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/config.py
--rw-r--r--   0        0        0    23246 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/docker.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/html_table.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/logger.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/mariadb.py
--rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/mw.py
--rw-r--r--   0        0        0     8314 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/mwcluster.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/version.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/webscrape.py
--rw-r--r--   0        0        0    11593 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/extensions.json
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/addCronTabEntry.sh
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/addSysopUser.sh
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/initdb.sh
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/installExtensions.sh
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwCompose.yml
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwDockerfile
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings.php
--rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings127.php
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings131.php
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings135.php
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings136.php
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings137.php
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings138.php
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings139.php
--rw-r--r--   0        0        0    56849 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki127.sql
--rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki131.sql
--rw-r--r--   0        0        0    64022 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki135.sql
--rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki136.sql
--rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki137.sql
--rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki138.sql
--rw-r--r--   0        0        0    64483 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki139.sql
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/phpinfo.php
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/plantuml.sh
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/startRunJobs.sh
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/update.sh
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/mwdocker/resources/templates/upload.ini
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/scripts/install
--rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/tests/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/tests/basetest.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/tests/test_config.py
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/tests/test_extensions.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/tests/test_html_tables.py
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/tests/test_install.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/LICENSE
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/README.md
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/.pydevproject
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/.DS_Store
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/__init__.py
+-rw-r--r--   0        0        0     9834 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/config.py
+-rw-r--r--   0        0        0    23246 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/docker.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/html_table.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/logger.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/mariadb.py
+-rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/mw.py
+-rw-r--r--   0        0        0     8471 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/mwcluster.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/version.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/webscrape.py
+-rw-r--r--   0        0        0    11593 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/extensions.json
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/addCronTabEntry.sh
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/addSysopUser.sh
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/initdb.sh
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/installExtensions.sh
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwCompose.yml
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwDockerfile
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings.php
+-rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings127.php
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings131.php
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings135.php
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings136.php
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings137.php
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings138.php
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings139.php
+-rw-r--r--   0        0        0    56849 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki127.sql
+-rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki131.sql
+-rw-r--r--   0        0        0    64022 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki135.sql
+-rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki136.sql
+-rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki137.sql
+-rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki138.sql
+-rw-r--r--   0        0        0    64483 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki139.sql
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/phpinfo.php
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/plantuml.sh
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/startRunJobs.sh
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/update.sh
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/upload.ini
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/scripts/install
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/tests/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/tests/basetest.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/tests/test_config.py
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/tests/test_extensions.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/tests/test_html_tables.py
+-rw-r--r--   0        0        0    10738 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/tests/test_install.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/LICENSE
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/README.md
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/PKG-INFO
```

### Comparing `pymediawikidocker-0.9.3/.github/workflows/build.yml` & `pymediawikidocker-0.9.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/.github/workflows/upload-to-pypi.yml` & `pymediawikidocker-0.9.4/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/.DS_Store` & `pymediawikidocker-0.9.4/mwdocker/.DS_Store`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/config.py` & `pymediawikidocker-0.9.4/mwdocker/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,19 @@
         self.fullVersion=f"MediaWiki {self.version}"
         self.underscoreVersion=self.version.replace(".","_")
         self.shortVersion=self.getShortVersion()
         self.base_url=f"{self.prot}://{self.host}"
         self.url=f"{self.base_url}{self.script_path}:{self.port}"
         if not self.container_base_name:
             self.container_base_name=f"{self.prefix}-{self.shortVersion}"
-            
+          
+    def reset_container_base_name(self,container_base_name:str=None):
+        self.container_base_name=container_base_name
+        self.__post_init__()
+          
     def as_dict(self)->dict:
         """
         return my fields as a dict
         dataclasses to dict conversion convenienc and information hiding
         
         Returns:
             dict: my fields in dict format
```

### Comparing `pymediawikidocker-0.9.3/mwdocker/docker.py` & `pymediawikidocker-0.9.4/mwdocker/docker.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/html_table.py` & `pymediawikidocker-0.9.4/mwdocker/html_table.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/logger.py` & `pymediawikidocker-0.9.4/mwdocker/logger.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/mariadb.py` & `pymediawikidocker-0.9.4/mwdocker/mariadb.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/mw.py` & `pymediawikidocker-0.9.4/mwdocker/mw.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/mwcluster.py` & `pymediawikidocker-0.9.4/mwdocker/mwcluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Created on 2021-08-06
 @author: wf
 '''
 import dataclasses
 from mwdocker.docker import DockerApplication
 from mwdocker.version import Version
 from mwdocker.config import MwClusterConfig
+from mwdocker.logger import Logger
 import sys
 from argparse import ArgumentParser
 from argparse import ArgumentDefaultsHelpFormatter
-from mwdocker.logger import Logger
 import webbrowser
 import traceback
 
 class MediaWikiCluster(object):
     '''
     a cluster of mediawiki docker Applications
     '''
@@ -40,16 +40,17 @@
         Args:
             home(str): the home path to use for the docker configuration files
             withGenerate(bool): if True generate the config files
             
         Returns:
             dict(str): a dict of apps by version
         '''  
+        app_count=len(self.config.versions)
         for i,version in enumerate(self.config.versions):
-            mwApp=self.getDockerApplication(i,version,home)
+            mwApp=self.getDockerApplication(i,app_count,version,home)
             if withGenerate:
                 mwApp.generateAll(overwrite=self.config.forceRebuild)
             self.apps[version]=mwApp    
         return self.apps
         
     def checkDocker(self)->int: 
         """
@@ -100,23 +101,20 @@
             int: exitCode - 0 if ok 1 if failed
         """
         exitCode=self.checkDocker()  
         if exitCode>0: return exitCode
         for i,version in enumerate(self.config.versions):
             mwApp=self.apps[version]
             mw,db=mwApp.getContainers()
-            if mw and db:
-                l_str="found"
-            else:
-                l_str="missing"
-            msg=f"{i+1}:{version} {l_str}"
-            print(msg)
+            config=mwApp.config
+            ok=mw and db
+            msg=f"{i+1}:{config.container_base_name} {config.fullVersion}"
+            Logger.check_and_log(msg, ok)
         return exitCode
         
-        
     def check(self)->int:
         """
         check the composer applications
         
         Returns:
             int: exitCode - 0 if ok 1 if failed
         """         
@@ -133,35 +131,37 @@
     def close(self):
         """
         close my apps
         """
         for mwApp in self.apps.values():
             mwApp.close()
             
-    def getDockerApplication(self,i:int,version:str,home:str=None):
+    def getDockerApplication(self,i:int,count:int,version:str,home:str=None):
         '''
         get the docker application for the given version index and version
         
         Args:
             i(int): the index of the version
+            count(int): total number of Docker applications in this cluster
             version(str): the mediawiki version to use
         
         Returns:
             DockerApplication: the docker application
         '''
         # please note that we are using the subclass MwClusterConfig here although
         # we only need the superclass MwConfig - we let inheritance work here for us but
         # have to ignore the superfluous fields
         appConfig=dataclasses.replace(self.config)
         appConfig.extensionMap=self.config.extensionMap.copy()
         appConfig.version=version
         appConfig.port=self.config.basePort+i
         appConfig.sqlPort=self.config.sqlPort+i   
         # let post_init create a new container_base_name
-        appConfig.container_base_name=None
+        if count>1:
+            appConfig.container_base_name=None
         appConfig.__post_init__()            
         mwApp=DockerApplication(config=appConfig,home=home)
         return mwApp
 
 DEBUG=False
 
 def main(argv=None): # IGNORE:C0111
```

### Comparing `pymediawikidocker-0.9.3/mwdocker/version.py` & `pymediawikidocker-0.9.4/mwdocker/version.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/webscrape.py` & `pymediawikidocker-0.9.4/mwdocker/webscrape.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/resources/extensions.json` & `pymediawikidocker-0.9.4/mwdocker/resources/extensions.json`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwCompose.yml` & `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwCompose.yml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwDockerfile` & `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwDockerfile`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings.php` & `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings127.php` & `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings127.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings131.php` & `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings131.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings135.php` & `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings135.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings136.php` & `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings136.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings137.php` & `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings137.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings138.php` & `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings138.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwLocalSettings139.php` & `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings139.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki127.sql` & `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki127.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki131.sql` & `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki131.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki135.sql` & `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki135.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki136.sql` & `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki136.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki137.sql` & `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki137.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki138.sql` & `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki138.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/resources/templates/mwWiki139.sql` & `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki139.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/mwdocker/resources/templates/plantuml.sh` & `pymediawikidocker-0.9.4/mwdocker/resources/templates/plantuml.sh`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/tests/basetest.py` & `pymediawikidocker-0.9.4/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/tests/test_config.py` & `pymediawikidocker-0.9.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/tests/test_extensions.py` & `pymediawikidocker-0.9.4/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/tests/test_html_tables.py` & `pymediawikidocker-0.9.4/tests/test_html_tables.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/tests/test_install.py` & `pymediawikidocker-0.9.4/tests/test_install.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,41 +202,48 @@
         '''
         version="1.27.7"
         args=["--versionList",version,
             "--prefix","rqotest",
             "--basePort","9481",
             "--sqlBasePort","10307"]
         self.printCommand("--down -f",args)
+        forceRebuild=True
         mwCluster=self.getMwCluster(args,createApps=False)
         mwCluster.config.addExtensions(["MagicNoCache"])
-        apps=mwCluster.createApps(withGenerate=True)
+        mwCluster.config.forceRebuild=forceRebuild
+        mwCluster.config.reset_container_base_name()
+        apps=mwCluster.createApps(withGenerate=forceRebuild)
         app=apps[version]
-        app.start(forceRebuild=True)
+        app.start(forceRebuild=forceRebuild)
         exitCode=mwCluster.check()
         self.assertEqual(0,exitCode)
         
     def testInstallationWithMissingLocalSettingsTemplate(self):
         '''
         test a cluster with no LocalSettingsTemplate available
         '''
         version="1.36.0"
         args=["--versionList",version,
-            "--prefix","mittest"
+            "--prefix","mittest",
+            "--container_name","mittest",
+            "-f"
         ]
+        debug=self.debug
+        debug=True
         try:
             mwCluster=self.getMwCluster(args,createApps=True)
             mwCluster.start()
             exitCode=mwCluster.check()
             self.assertEqual(0,exitCode)
         except Exception as ex:
             ex_msg=str(ex)
-            if self.debug:
-                print(ex_msg)
+            if debug:
+                print(f"exception: {ex_msg}")
             #self.assertTrue()
-            self.assertTrue("code 14" in ex_msg)
+            self.assertTrue("code 14" in ex_msg,ex_msg)
             pass
            
     def testWikiUser(self):
         '''
         test the wikiUser handling
         '''
         mwCluster=self.getMwCluster()
```

### Comparing `pymediawikidocker-0.9.3/.gitignore` & `pymediawikidocker-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/LICENSE` & `pymediawikidocker-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/README.md` & `pymediawikidocker-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/pyproject.toml` & `pymediawikidocker-0.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.3/PKG-INFO` & `pymediawikidocker-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymediawikidocker
-Version: 0.9.3
+Version: 0.9.4
 Summary: Python controlled (semantic) mediawiki docker application cluster installation
 Project-URL: Home, https://github.com/WolfgangFahl/pymediawikidocker
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/pymediawikidocker
 Project-URL: Source, https://github.com/WolfgangFahl/pymediawikidocker
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License: Apache-2.0
```

