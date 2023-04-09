# Comparing `tmp/property-lister-1.5.tar.gz` & `tmp/property-lister-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "property-lister-1.5.tar", last modified: Wed Mar 29 15:27:42 2023, max compression
+gzip compressed data, was "property-lister-1.6.tar", last modified: Sun Apr  9 10:22:10 2023, max compression
```

## Comparing `property-lister-1.5.tar` & `property-lister-1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:27:42.610374 property-lister-1.5/
--rwxrwx---   0 root         (0) root         (0)     1090 2023-03-29 15:27:15.000000 property-lister-1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2614 2023-03-29 15:27:42.610374 property-lister-1.5/PKG-INFO
--rwxrwx---   0 root         (0) root         (0)     2229 2023-03-29 15:27:15.000000 property-lister-1.5/README.md
--rwxrwx---   0 root         (0) root         (0)      728 2023-03-29 15:27:15.000000 property-lister-1.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-29 15:27:42.610374 property-lister-1.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:27:42.610374 property-lister-1.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:27:42.610374 property-lister-1.5/src/property_lister/
--rwxrwx---   0 root         (0) root         (0)        0 2023-03-29 15:27:15.000000 property-lister-1.5/src/property_lister/__init__.py
--rwxrwx---   0 root         (0) root         (0)     8892 2023-03-29 15:27:15.000000 property-lister-1.5/src/property_lister/property_lister.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:27:42.610374 property-lister-1.5/src/property_lister.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2614 2023-03-29 15:27:42.000000 property-lister-1.5/src/property_lister.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2023-03-29 15:27:42.000000 property-lister-1.5/src/property_lister.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 15:27:42.000000 property-lister-1.5/src/property_lister.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-29 15:27:42.000000 property-lister-1.5/src/property_lister.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-29 15:27:42.000000 property-lister-1.5/src/property_lister.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-03-29 15:27:42.000000 property-lister-1.5/src/property_lister.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 10:22:10.452973 property-lister-1.6/
+-rwxrwx---   0 root         (0) root         (0)     1090 2023-04-08 16:38:41.000000 property-lister-1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2614 2023-04-09 10:22:10.448971 property-lister-1.6/PKG-INFO
+-rwxrwx---   0 root         (0) root         (0)     2229 2023-04-08 16:40:20.000000 property-lister-1.6/README.md
+-rwxrwx---   0 root         (0) root         (0)      728 2023-04-08 16:40:03.000000 property-lister-1.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 10:22:10.452973 property-lister-1.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 10:22:10.448971 property-lister-1.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 10:22:10.448971 property-lister-1.6/src/property_lister/
+-rwxrwx---   0 root         (0) root         (0)        0 2023-04-08 16:38:41.000000 property-lister-1.6/src/property_lister/__init__.py
+-rwxrwx---   0 root         (0) root         (0)     9038 2023-04-09 10:21:14.000000 property-lister-1.6/src/property_lister/property_lister.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 10:22:10.448971 property-lister-1.6/src/property_lister.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2614 2023-04-09 10:22:10.000000 property-lister-1.6/src/property_lister.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2023-04-09 10:22:10.000000 property-lister-1.6/src/property_lister.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 10:22:10.000000 property-lister-1.6/src/property_lister.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-09 10:22:10.000000 property-lister-1.6/src/property_lister.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-09 10:22:10.000000 property-lister-1.6/src/property_lister.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-09 10:22:10.000000 property-lister-1.6/src/property_lister.egg-info/top_level.txt
```

### Comparing `property-lister-1.5/LICENSE` & `property-lister-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `property-lister-1.5/PKG-INFO` & `property-lister-1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: property-lister
-Version: 1.5
+Version: 1.6
 Summary: Extract property list files from an SQLite unencrypted database file.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/property-lister
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -41,15 +41,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/property-lister && cd property-lister
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/property_lister-1.5-py3-none-any.whl
+python3 -m pip install dist/property_lister-1.6-py3-none-any.whl
 ```
 
 ## Extract Property List Files
 
 ```fundamental
 scp root@192.168.1.10:/var/mobile/Containers/Data/Application/YYY...YYY/Library/Caches/com.someapp.dev/Cache.db ./
 
@@ -57,15 +57,15 @@
 ```
 
 Check my other project on how to [find files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#3-search-for-files-and-directories) and on how to [extract sensitive data from files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#4-inspect-files).
 
 ## Usage
 
 ```fundamental
-Property Lister v1.5 ( github.com/ivan-sincek/property-lister )
+Property Lister v1.6 ( github.com/ivan-sincek/property-lister )
 
 --- Extract from an SQLite unencrypted database file ---
 Usage:   property-lister -db database -o out
 Example: property-lister -db Cache.db -o results
 
 --- Extract from a property list file ---
 Usage:   property-lister -pl property-list -o out
```

### Comparing `property-lister-1.5/README.md` & `property-lister-1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/property-lister && cd property-lister
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/property_lister-1.5-py3-none-any.whl
+python3 -m pip install dist/property_lister-1.6-py3-none-any.whl
 ```
 
 ## Extract Property List Files
 
 ```fundamental
 scp root@192.168.1.10:/var/mobile/Containers/Data/Application/YYY...YYY/Library/Caches/com.someapp.dev/Cache.db ./
 
@@ -44,15 +44,15 @@
 ```
 
 Check my other project on how to [find files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#3-search-for-files-and-directories) and on how to [extract sensitive data from files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#4-inspect-files).
 
 ## Usage
 
 ```fundamental
-Property Lister v1.5 ( github.com/ivan-sincek/property-lister )
+Property Lister v1.6 ( github.com/ivan-sincek/property-lister )
 
 --- Extract from an SQLite unencrypted database file ---
 Usage:   property-lister -db database -o out
 Example: property-lister -db Cache.db -o results
 
 --- Extract from a property list file ---
 Usage:   property-lister -pl property-list -o out
```

### Comparing `property-lister-1.5/pyproject.toml` & `property-lister-1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "property-lister"
-version = "1.5"
+version = "1.6"
 authors = [{ name = "Ivan Sincek" }]
 description = "Extract property list files from an SQLite unencrypted database file."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `property-lister-1.5/src/property_lister/property_lister.py` & `property-lister-1.6/src/property_lister/property_lister.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 start = datetime.datetime.now()
 
 # -------------------------- INFO --------------------------
 
 def basic():
 	global proceed
 	proceed = False
-	print("Property Lister v1.5 ( github.com/ivan-sincek/property-lister )")
+	print("Property Lister v1.6 ( github.com/ivan-sincek/property-lister )")
 	print("")
 	print("--- Extract from an SQLite unencrypted database file ---")
 	print("Usage:   property-lister -db database -o out")
 	print("Example: property-lister -db Cache.db -o results")
 	print("")
 	print("--- Extract from a property list file ---")
 	print("Usage:   property-lister -pl property-list -o out")
@@ -156,17 +156,23 @@
 
 # ------------------ GLOBAL VARIABLES END ------------------
 
 # ----------------------- TASK BEGIN -----------------------
 
 def read_database(file):
 	tmp = ""
-	with sqlite3.connect(file) as db:
+	db = None
+	try:
+		db = sqlite3.connect(file)
 		tmp = ("").join(db.iterdump())
-	db.close()
+	except sqlite3.DatabaseError:
+		pass
+	finally:
+		if db:
+			db.close()
 	return tmp
 
 # database --> full path (external)
 def dump(database, out):
 	for db in database:
 		count = 0
 		data = read_database(db)
@@ -204,15 +210,15 @@
 		data = None
 		with open(file, "rb") as stream:
 			data = plistlib.load(stream)
 		stream.close()
 		if data:
 			open(file, "wb").write(plistlib.dumps(data, fmt = plistlib.FMT_XML))
 			os.rename(file, file.rsplit(".", 1)[0] + ext["xml"])
-	except (plistlib.InvalidFileException):
+	except plistlib.InvalidFileException:
 		pass
 
 def main():
 	argc = len(sys.argv) - 1
 
 	if argc == 0:
 		advanced()
@@ -222,24 +228,24 @@
 		elif sys.argv[1] == "--help":
 			advanced()
 		else:
 			error("Incorrect usage", True)
 	elif argc % 2 == 0 and argc <= len(args) * 2:
 		for i in range(1, argc, 2):
 			validate(sys.argv[i], sys.argv[i + 1])
-		if not ((args["database"] and args["out"]) or (args["plist"] and args["out"])) or (args["database"] and args["plist"]) or not check(argc, args):
+		if not ((args["database"] is not None and args["out"] is not None) or (args["plist"] is not None and args["out"] is not None)) or (args["database"] is not None and args["plist"] is not None) or not check(argc, args):
 			error("Missing a mandatory option (-db, -o)")
 			error("Missing a mandatory option (-pl, -o)", True)
 	else:
 		error("Incorrect usage", True)
 
 	if proceed and check_directory(args["out"]):
 		print("######################################################################")
 		print("#                                                                    #")
-		print("#                        Property Lister v1.5                        #")
+		print("#                        Property Lister v1.6                        #")
 		print("#                                   by Ivan Sincek                   #")
 		print("#                                                                    #")
 		print("# Extract and convert property list files.                           #")
 		print("# GitHub repository at github.com/ivan-sincek/property-lister.       #")
 		print("# Feel free to donate bitcoin at 1BrZM6T7G9RN8vbabnfXu4M6Lpgztq6Y14. #")
 		print("#                                                                    #")
 		print("######################################################################")
```

### Comparing `property-lister-1.5/src/property_lister.egg-info/PKG-INFO` & `property-lister-1.6/src/property_lister.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: property-lister
-Version: 1.5
+Version: 1.6
 Summary: Extract property list files from an SQLite unencrypted database file.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/property-lister
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -41,15 +41,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/property-lister && cd property-lister
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/property_lister-1.5-py3-none-any.whl
+python3 -m pip install dist/property_lister-1.6-py3-none-any.whl
 ```
 
 ## Extract Property List Files
 
 ```fundamental
 scp root@192.168.1.10:/var/mobile/Containers/Data/Application/YYY...YYY/Library/Caches/com.someapp.dev/Cache.db ./
 
@@ -57,15 +57,15 @@
 ```
 
 Check my other project on how to [find files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#3-search-for-files-and-directories) and on how to [extract sensitive data from files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#4-inspect-files).
 
 ## Usage
 
 ```fundamental
-Property Lister v1.5 ( github.com/ivan-sincek/property-lister )
+Property Lister v1.6 ( github.com/ivan-sincek/property-lister )
 
 --- Extract from an SQLite unencrypted database file ---
 Usage:   property-lister -db database -o out
 Example: property-lister -db Cache.db -o results
 
 --- Extract from a property list file ---
 Usage:   property-lister -pl property-list -o out
```

