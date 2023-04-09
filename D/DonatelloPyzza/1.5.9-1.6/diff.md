# Comparing `tmp/donatellopyzza-1.5.9.tar.gz` & `tmp/donatellopyzza-1.6.tar.gz`

## Comparing `donatellopyzza-1.5.9.tar` & `donatellopyzza-1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/__init__.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/assessor.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/envBuilder.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/game.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/main.py
--rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/mazeGenerator.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/turtleAgent.py
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/data/environments/assessment_maze.png
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/data/environments/assessment_maze.txt
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/data/environments/hard_maze.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/data/environments/maze.txt
--rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/data/environments/test.png
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/data/environments/test.txt
--rw-r--r--   0        0        0    40100 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/data/images/pizza.png
--rw-r--r--   0        0        0     8849 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/data/images/turtle.png
--rw-r--r--   0        0        0    22725 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/data/images/turtle_small.png
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/grid/agent.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/grid/careTaker.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/grid/constants.py
--rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/grid/grid.py
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/grid/gui.py
--rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/grid/map.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/grid/memento.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/grid/orientation.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/grid/originator.py
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/grid/parser.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/grid/square.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/donatellopyzza/grid/turn.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/LICENSE
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/README.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/pyproject.toml
--rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 donatellopyzza-1.5.9/PKG-INFO
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/__init__.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/assessor.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/envBuilder.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/game.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/main.py
+-rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/mazeGenerator.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/turtleAgent.py
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/data/environments/assessment_maze.png
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/data/environments/assessment_maze.txt
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/data/environments/hard_maze.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/data/environments/maze.txt
+-rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/data/environments/test.png
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/data/environments/test.txt
+-rw-r--r--   0        0        0    40100 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/data/images/pizza.png
+-rw-r--r--   0        0        0     8849 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/data/images/turtle.png
+-rw-r--r--   0        0        0    22725 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/data/images/turtle_small.png
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/grid/agent.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/grid/careTaker.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/grid/constants.py
+-rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/grid/grid.py
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/grid/gui.py
+-rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/grid/map.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/grid/memento.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/grid/orientation.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/grid/originator.py
+-rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/grid/parser.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/grid/square.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 donatellopyzza-1.6/donatellopyzza/grid/turn.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 donatellopyzza-1.6/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 donatellopyzza-1.6/LICENSE
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 donatellopyzza-1.6/README.md
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 donatellopyzza-1.6/pyproject.toml
+-rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 donatellopyzza-1.6/PKG-INFO
```

### Comparing `donatellopyzza-1.5.9/donatellopyzza/assessor.py` & `donatellopyzza-1.6/donatellopyzza/assessor.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.9/donatellopyzza/envBuilder.py` & `donatellopyzza-1.6/donatellopyzza/envBuilder.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.9/donatellopyzza/game.py` & `donatellopyzza-1.6/donatellopyzza/game.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.9/donatellopyzza/main.py` & `donatellopyzza-1.6/donatellopyzza/main.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.9/donatellopyzza/mazeGenerator.py` & `donatellopyzza-1.6/donatellopyzza/mazeGenerator.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.9/donatellopyzza/data/environments/assessment_maze.png` & `donatellopyzza-1.6/donatellopyzza/data/environments/assessment_maze.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.9/donatellopyzza/data/environments/test.png` & `donatellopyzza-1.6/donatellopyzza/data/environments/test.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.9/donatellopyzza/data/images/pizza.png` & `donatellopyzza-1.6/donatellopyzza/data/images/pizza.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.9/donatellopyzza/data/images/turtle.png` & `donatellopyzza-1.6/donatellopyzza/data/images/turtle.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.9/donatellopyzza/data/images/turtle_small.png` & `donatellopyzza-1.6/donatellopyzza/data/images/turtle_small.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.9/donatellopyzza/grid/agent.py` & `donatellopyzza-1.6/donatellopyzza/grid/agent.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.9/donatellopyzza/grid/grid.py` & `donatellopyzza-1.6/donatellopyzza/grid/grid.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.9/donatellopyzza/grid/gui.py` & `donatellopyzza-1.6/donatellopyzza/grid/gui.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.9/donatellopyzza/grid/map.py` & `donatellopyzza-1.6/donatellopyzza/grid/map.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.9/donatellopyzza/grid/parser.py` & `donatellopyzza-1.6/donatellopyzza/grid/parser.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.9/donatellopyzza/grid/square.py` & `donatellopyzza-1.6/donatellopyzza/grid/square.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.9/LICENSE` & `donatellopyzza-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.5.9/README.md` & `donatellopyzza-1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -91,14 +91,17 @@
 For more details, you can find several complete examples of the game loop in the `examples` folder on the github repository of this project.
 
 Have fun!
 
 
 ## What's new
 
+
+- 2023-04-09 (v1.6)
+    Integration of an algorithm assessment class. Allows to evaluate automatically a solution on several mazes
 - 2023-04-07 (v1.5)
     Integration of a maze generator from Alexandru Văleanu (https://github.com/AlexandruValeanu/Mazify)
 - 2023-01-17 (v1.2)
     Initial release
 
 
 ## Roadmap
```

### Comparing `donatellopyzza-1.5.9/pyproject.toml` & `donatellopyzza-1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "DonatelloPyzza"
-version = "1.5.9"
+version = "1.6"
 authors = [
   { name="Mickaël Bettinelli", email="mickael.bettinelli@univ-smb.fr" },
 ]
 description = "A simple grid environment to learn Python"
 readme = "README.md"
 requires-python = ">=3.1"
 classifiers = [
```

### Comparing `donatellopyzza-1.5.9/PKG-INFO` & `donatellopyzza-1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DonatelloPyzza
-Version: 1.5.9
+Version: 1.6
 Summary: A simple grid environment to learn Python
 Project-URL: Homepage, https://github.com/MilowB/Donatello
 Project-URL: Bug Tracker, https://github.com/MilowB/Donatello/pulls
 Author-email: Mickaël Bettinelli <mickael.bettinelli@univ-smb.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -105,14 +105,17 @@
 For more details, you can find several complete examples of the game loop in the `examples` folder on the github repository of this project.
 
 Have fun!
 
 
 ## What's new
 
+
+- 2023-04-09 (v1.6)
+    Integration of an algorithm assessment class. Allows to evaluate automatically a solution on several mazes
 - 2023-04-07 (v1.5)
     Integration of a maze generator from Alexandru Văleanu (https://github.com/AlexandruValeanu/Mazify)
 - 2023-01-17 (v1.2)
     Initial release
 
 
 ## Roadmap
```

