# Comparing `tmp/sqlite-history-0.1.tar.gz` & `tmp/sqlite-history-0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlite-history-0.1.tar", last modified: Sun Apr  9 05:09:50 2023, max compression
+gzip compressed data, was "sqlite-history-0.1a0.tar", last modified: Sun Apr  9 01:26:40 2023, max compression
```

## Comparing `sqlite-history-0.1.tar` & `sqlite-history-0.1a0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:09:50.165363 sqlite-history-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 05:09:29.000000 sqlite-history-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-09 05:09:50.165363 sqlite-history-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-04-09 05:09:29.000000 sqlite-history-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 05:09:50.165363 sqlite-history-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-09 05:09:29.000000 sqlite-history-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:09:50.165363 sqlite-history-0.1/sqlite_history/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-09 05:09:29.000000 sqlite-history-0.1/sqlite_history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-09 05:09:29.000000 sqlite-history-0.1/sqlite_history/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-09 05:09:29.000000 sqlite-history-0.1/sqlite_history/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-09 05:09:29.000000 sqlite-history-0.1/sqlite_history/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:09:50.165363 sqlite-history-0.1/sqlite_history.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-09 05:09:50.000000 sqlite-history-0.1/sqlite_history.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-09 05:09:50.000000 sqlite-history-0.1/sqlite_history.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 05:09:50.000000 sqlite-history-0.1/sqlite_history.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-09 05:09:50.000000 sqlite-history-0.1/sqlite_history.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-09 05:09:50.000000 sqlite-history-0.1/sqlite_history.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:09:50.165363 sqlite-history-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-09 05:09:29.000000 sqlite-history-0.1/tests/test_sqlite_history.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:26:40.515200 sqlite-history-0.1a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 01:26:13.000000 sqlite-history-0.1a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-09 01:26:40.515200 sqlite-history-0.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-09 01:26:13.000000 sqlite-history-0.1a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 01:26:40.515200 sqlite-history-0.1a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-09 01:26:13.000000 sqlite-history-0.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:26:40.511200 sqlite-history-0.1a0/sqlite_history/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-09 01:26:13.000000 sqlite-history-0.1a0/sqlite_history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-09 01:26:13.000000 sqlite-history-0.1a0/sqlite_history/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-09 01:26:13.000000 sqlite-history-0.1a0/sqlite_history/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:26:40.511200 sqlite-history-0.1a0/sqlite_history.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-09 01:26:40.000000 sqlite-history-0.1a0/sqlite_history.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-09 01:26:40.000000 sqlite-history-0.1a0/sqlite_history.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 01:26:40.000000 sqlite-history-0.1a0/sqlite_history.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-09 01:26:40.000000 sqlite-history-0.1a0/sqlite_history.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-09 01:26:40.000000 sqlite-history-0.1a0/sqlite_history.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:26:40.515200 sqlite-history-0.1a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-09 01:26:13.000000 sqlite-history-0.1a0/tests/test_sqlite_history.py
```

### Comparing `sqlite-history-0.1/LICENSE` & `sqlite-history-0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite-history-0.1/setup.py` & `sqlite-history-0.1a0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.1"
+VERSION = "0.1a0"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -24,10 +24,10 @@
         "CI": "https://github.com/simonw/sqlite-history/actions",
         "Changelog": "https://github.com/simonw/sqlite-history/releases",
     },
     license="Apache License, Version 2.0",
     version=VERSION,
     packages=["sqlite_history"],
     install_requires=[],
-    extras_require={"test": ["pytest", "sqlite-utils", "cogapp"]},
+    extras_require={"test": ["pytest", "sqlite-utils"]},
     python_requires=">=3.7",
 )
```

### Comparing `sqlite-history-0.1/sqlite_history/cli.py` & `sqlite-history-0.1a0/sqlite_history/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,75 +16,53 @@
         )
         if cursor.fetchone():
             print(f"History table {history_table_name} already exists - skipping.")
             continue
         configure_history(db, table)
 
 
-def all_regular_tables(database_path):
-    """'Regular' excludes FTS and related tables."""
+def get_all_table_names(database_path):
     conn = sqlite3.connect(database_path)
     cursor = conn.cursor()
-    hidden_tables = [
-        r[0]
-        for r in (
-            cursor.execute(
-                """
-            SELECT NAME FROM sqlite_master
-            WHERE type = 'table'
-            AND (
-                sql LIKE '%VIRTUAL TABLE%USING FTS%'
-            ) OR name IN ('sqlite_stat1', 'sqlite_stat2', 'sqlite_stat3', 'sqlite_stat4')
-        """
-            )
-        ).fetchall()
-    ]
-    hidden_tables_copy = hidden_tables[:]
-    regular_tables = []
-    for row in cursor.execute(
-        "SELECT name FROM sqlite_master WHERE type='table';"
-    ).fetchall():
-        table_name = row[0]
-        should_be_hidden = any(
-            table_name.startswith(hidden_table) for hidden_table in hidden_tables_copy
-        )
-        if not should_be_hidden:
-            regular_tables.append(table_name)
-    return regular_tables
+    cursor.execute(
+        "SELECT name FROM sqlite_master WHERE type='table' and sql not like '%virtual table%';"
+    )
+    return [table[0] for table in cursor.fetchall()]
 
 
-def run(test_args=None):
+def run():
     parser = argparse.ArgumentParser(
         description="Configure sqlite-history triggers for one or more tables."
     )
 
     parser.add_argument("database_path", help="Path to the SQLite database file.")
     parser.add_argument(
         "tables", nargs="*", help="One or more table names to configure."
     )
     parser.add_argument(
         "--all", action="store_true", help="Configure for all tables in the database."
     )
 
-    if test_args:
-        args = parser.parse_args(test_args)
-    else:
-        args = parser.parse_args()
+    args = parser.parse_args()
 
     if args.all:
-        args.tables = all_regular_tables(args.database_path)
+        args.tables = get_all_table_names(args.database_path)
     elif len(args.tables) == 0:
         parser.error(
             "No tables provided. Please provide table names or use --all flag."
         )
 
     # Error if database_path doesn't exist
     if not os.path.exists(args.database_path):
         parser.error("Database file does not exist.")
 
     # Error if any of the tables don't exist
-    all_table_names = all_regular_tables(args.database_path)
+    all_table_names = get_all_table_names(args.database_path)
     missing_tables = [table for table in args.tables if table not in all_table_names]
     if missing_tables:
         parser.error("The following tables do not exist: " + ", ".join(missing_tables))
 
     configure_triggers(args.database_path, args.tables)
+
+
+if __name__ == "__main__":
+    run()
```

