# Comparing `tmp/hurdat2parser-2.11.tar.gz` & `tmp/hurdat2parser-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\ksgta\Documents\GitHub\hurdat2parser\upload_for2p11\dist\tmpktita0x_\hurdat2parser-2.11.tar", last modified: Sat Jun  4 03:41:25 2022, max compression
+gzip compressed data, was "hurdat2parser-2.2.tar", last modified: Sun Apr  9 01:27:04 2023, max compression
```

## Comparing `hurdat2parser-2.11.tar` & `hurdat2parser-2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-06-04 03:41:25.000000 hurdat2parser-2.11/
--rw-rw-rw-   0        0        0     1115 2022-06-04 03:27:15.000000 hurdat2parser-2.11/LICENSE.txt
--rw-rw-rw-   0        0        0    23131 2022-06-04 03:41:25.000000 hurdat2parser-2.11/PKG-INFO
--rw-rw-rw-   0        0        0    22537 2022-06-04 03:23:48.000000 hurdat2parser-2.11/README.md
-drwxrwxrwx   0        0        0        0 2022-06-04 03:41:25.000000 hurdat2parser-2.11/hurdat2parser/
--rw-rw-rw-   0        0        0    51764 2022-06-02 23:02:24.000000 hurdat2parser-2.11/hurdat2parser/__init__.py
--rw-rw-rw-   0        0        0     3804 2022-05-31 23:33:50.000000 hurdat2parser-2.11/hurdat2parser/_aliases.py
--rw-rw-rw-   0        0        0    59218 2022-06-02 23:27:29.000000 hurdat2parser-2.11/hurdat2parser/_calculations.py
--rw-rw-rw-   0        0        0     2436 2021-10-04 15:04:24.000000 hurdat2parser-2.11/hurdat2parser/_future.py
--rw-rw-rw-   0        0        0   366145 2021-10-05 01:22:34.000000 hurdat2parser-2.11/hurdat2parser/_maps.py
--rw-rw-rw-   0        0        0    33766 2022-06-02 10:05:45.000000 hurdat2parser-2.11/hurdat2parser/_reports.py
-drwxrwxrwx   0        0        0        0 2022-06-04 03:41:25.000000 hurdat2parser-2.11/hurdat2parser.egg-info/
--rw-rw-rw-   0        0        0    23131 2022-06-04 03:41:23.000000 hurdat2parser-2.11/hurdat2parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2022-06-04 03:41:25.000000 hurdat2parser-2.11/hurdat2parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-04 03:41:23.000000 hurdat2parser-2.11/hurdat2parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-06-04 03:41:19.000000 hurdat2parser-2.11/hurdat2parser.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2022-06-04 03:41:24.000000 hurdat2parser-2.11/hurdat2parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-06-04 03:41:24.000000 hurdat2parser-2.11/hurdat2parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-04-22 04:30:17.000000 hurdat2parser-2.11/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-06-04 03:41:25.000000 hurdat2parser-2.11/setup.cfg
--rw-rw-rw-   0        0        0      899 2022-06-04 03:27:41.000000 hurdat2parser-2.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 01:27:04.086099 hurdat2parser-2.2/
+-rw-rw-rw-   0        0        0     1115 2023-04-09 01:19:53.000000 hurdat2parser-2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    33455 2023-04-09 01:27:04.086099 hurdat2parser-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    32862 2023-04-09 01:14:18.000000 hurdat2parser-2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 01:27:04.014084 hurdat2parser-2.2/hurdat2parser/
+-rw-rw-rw-   0        0        0    57354 2023-04-07 05:04:47.000000 hurdat2parser-2.2/hurdat2parser/__init__.py
+-rw-rw-rw-   0        0        0     7088 2023-02-28 07:16:47.000000 hurdat2parser-2.2/hurdat2parser/_aliases.py
+-rw-rw-rw-   0        0        0    80092 2023-02-26 03:51:21.000000 hurdat2parser-2.2/hurdat2parser/_calculations.py
+-rw-rw-rw-   0        0        0    14830 2023-02-24 08:17:51.000000 hurdat2parser-2.2/hurdat2parser/_future.py
+-rw-rw-rw-   0        0        0   163453 2022-07-18 22:48:06.000000 hurdat2parser-2.2/hurdat2parser/_maps.py
+-rw-rw-rw-   0        0        0    37465 2023-03-02 07:25:50.000000 hurdat2parser-2.2/hurdat2parser/_reports.py
+drwxrwxrwx   0        0        0        0 2023-04-09 01:27:04.086099 hurdat2parser-2.2/hurdat2parser.egg-info/
+-rw-rw-rw-   0        0        0    33455 2023-04-09 01:27:03.000000 hurdat2parser-2.2/hurdat2parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-04-09 01:27:03.000000 hurdat2parser-2.2/hurdat2parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 01:27:03.000000 hurdat2parser-2.2/hurdat2parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-09 01:27:02.000000 hurdat2parser-2.2/hurdat2parser.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2023-04-09 01:27:03.000000 hurdat2parser-2.2/hurdat2parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-09 01:27:03.000000 hurdat2parser-2.2/hurdat2parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-04-22 04:30:18.000000 hurdat2parser-2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-09 01:27:04.086099 hurdat2parser-2.2/setup.cfg
+-rw-rw-rw-   0        0        0      898 2023-04-09 01:21:06.000000 hurdat2parser-2.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hurdat2parser-2.11/LICENSE.txt` & `hurdat2parser-2.2/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-hurdat2parser 2.11, Copyright (c) 2019-2022 Kyle S. Gentry
+hurdat2parser 2.2, Copyright (c) 2019-2023, Kyle S. Gentry
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `hurdat2parser-2.11/PKG-INFO` & `hurdat2parser-2.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,101 +1,176 @@
 Metadata-Version: 2.1
 Name: hurdat2parser
-Version: 2.11
+Version: 2.2
 Summary: Interpret Hurricane Data contained in HURDAT2
 Home-page: http://github.com/ksgwxfan/hurdat2parser
 Author: Kyle S. Gentry
 Author-email: KyleSGentry@outlook.com
 License: MIT
 Keywords: hurricane hurdat2 meteorology weather
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# hurdat2parser -- v2.11
+# hurdat2parser -- v2.2
 ---
-### *Interpreting the HURDAT2 Tropical Cyclone Dataset using Python*
+### *Interpreting the Hurdat2 Tropical Cyclone Dataset using Python*
 
 Hurdat2 ([https://www.nhc.noaa.gov/data/#hurdat](https://www.nhc.noaa.gov/data/#hurdat)) is a collection of records from individual Tropical Cyclones. The two primary Hurdat2 records are for the Atlantic (since 1850) and East/Central-Pacific Oceans (since 1949).
 
 The purpose of this module is to provide a quick way to analyze the Hurdat2 datasets. It includes methods for retrieving, inspecting, ranking, or even exporting data for seasons, individual storms, or climatological eras.
 
-This release is primarily a "patch" in response to the newest release of the Hurdat2 database (official inclusion of data from the 2021 season). A new variable has been introduced, and this release accommodates it. But all previous versions of `hurdat2parser` will not be compatible with this and (likely) future Hurdat2 databases. But this (`2.11`) and all future versions of this program will be backward compatible to previous versions of the database.
-
 PyPI Link: [https://pypi.org/project/hurdat2parser/](https://pypi.org/project/hurdat2parser/)
 
 ## Contents
-* [Changes/Fixes in this Version (2.11)](#changes-in-this-version-211)
+* [Changes/Fixes in this Version (2.2)](#changes-in-this-version-22)
 * [Requirements, Installation, and getting the data](#installation)
 * [Importing the module](#importing-the-module)
+* [Example Calls](#example-calls)
 * [Hurdat2 Object Structure](#hurdat2-object-structure)
 * [Methods &amp; Attributes](#methods-and-attributes)
 * [Note on Landfall Data](#landfall-data)
+* [Future/Under-Development/Unreleased Methods](#access-to-future-methods)
 * [Roadmap](#roadmap)
 * [Credits](#credits)
 * [Copyright/License](#copyright)
 
-## Changes in this Version (2.11)
-- Patched to enable compatibility with the May 2022 release of the Hurdat2 database
-- Added a `TCRecordEntry` variable called `wind_radii` (the new variable included in the May 2022 Hurdat2 release. There may be some future potential in expanding the use of this variable, but its availability is currently limited to the 2021 Hurricane Season
-- Fixed calls to `TCRecordEntry` variables `avg_wind_extent_<STATUS>`
-- `info()` method for `Season` objects removed (use the `stats()` method instead)
-- modification of `<Hurdat2>.basin()`; now a method instead of property.
-- Fixed `rank_seasons_thru()` where a call without keywords (becoming a wrapper for `rank_seasons`) had an ill-advised direct call to a dictionary key instead of the get method
+## Changes in this Version (2.2)
+
+- Docstring'd `TCRecordEntry` properties
+- Changes to the `<Hurdat2>` object:
+  - when reading-in files on `__init__`, multiple local files are now supported.
+  - enabled download of the most-recent hurdat2 dataset through the `basin` kwarg.
+  - added a `urlcheck` kwarg. If `True`, the "file-path"s listed will be treated like URLs and a download attempt will be made.
+  - removed the `_filesappended` attribute
+  - Searching for notoriously-named storms can be done by a dash (`"-"`) prefix to the search string in addition to an underscore (see [Example Calls](#example-calls) section)
+  - Revamped `output_climo_csv`, `output_season_csv`, and `output_storms_csv` methods
+    - simplified code; updated and unified attributes used in the reports and made it significantly easier for future maintenance.
+  - moved `multi_season_info` method to `_reports`
+- New properties for both `Season` and `TropicalCyclone`:
+  - `duration`
+    - `Season` version reports time between the first and last day of the season (see further in the document for explanation)
+	- `TropicalCyclone` version just reports the track-life in days, regardless of status. More useful status-based duration properties were created too. Keep reading (a few lines down).
+  - `tc_entries` returns a list of `TCRecordEntry`s where a storm was a designated tropical cyclone.
+  - `start_date`, `start_ordinal`, and `end_date`, `end_ordinal` report the starting/ending dates and/or days of the year
+- New `TropicalCyclone` variables:
+  - `ACE_no_landfall`
+  - `duration_<TC, TS, HU, MHU>` - These properties report the aggregate time in days that a tropical cyclone was designated that status or stronger, accounting for fluxuations in storm statuses and strengths.
+  - removed `coord_list` method. It was redundant as it was like a shortened combination of the `summary` method.
+- New `TCRecordEntry` variables:
+  - tweaked how location variables are defined. `location` and `location_reversed` are now properties that depend on the express definition of the variables `lat` and `lon` rather than the other way around.
+  - tweak of not-available wind-extent data. As of the moment typing this, wind-extent data is only provided for storms since 2004. All previous wind-extent data is `-999`, meaning its unavailable. But if a storm has max winds of `<` 64, its Hurricane wind extent has to be 0. So when ingesting the data, this determination is made.
+  - tweaked ingest of data to prevent errors due to possible new Hurdat2 categories introduced in future versions. This was the problem with `v2.1` that was responsible for the need for a `v2.11` release. This particular version wouldn't be able to read-in the new variables in such a situation, but it would still be functional with the newer database (unless order of variables are switched around).
+  - the formerly-called variable `wind_radii` from `v2.11` is now called `maxwind_radius`. I don't know why I called it `radii`, as in plural of radius. I guess it sounded science-y or smart. haha. But the change is also more readable.
+  - Surface Area (coverage)-based variables `areal_extent_TS`, `areal_extent_TS50`, and `areal_extent_HU`.
+    - These are calculated from reported wind-extents in the database.
+  - `track_distance`: the track distance of the cyclone up to the point of the respective entry; this does not account for storm status
+  - `previous_entries` and `next_entries`: lists of the previous and next recorded entries, respectively, in the `TropicalCyclone`'s record
+  - `previous_entry` and `next_entry`: the previous and next recorded entry, respectively, in the `TropicalCyclone`'s record
+  - `direction()`: the `TropicalCyclone`'s heading in degrees (or cardinal, if desired...see docstring)
+  - `speed`: the `TropicalCyclone`'s forward speed in knots.
+  - Properties to simplify coding and reduce probability of coding errors.
+    - `is_TC`: `bool` indicating whether or not a storm was designated as a tropical cyclone at the `<TCRecordEntry>.entrytime`.
+    - `is_synoptic`: `bool` indicating whether or not an entry occurred at a synoptic time (0Z, 6Z, 12Z, 18Z).
+- Added `report_type` default keyword argument to the `<Season>.stats` method. User can dictate if report prints to the console or gets back a string version of the report.
+- Fixed an exclusion of `maxwind_radius` (formerly called `wind_radii`) from `<TCRecordEntry>.hurdat2()` calls. (which was only introduced in the previous version).
+- Tweaked landfall-disclaimer in `<Season>.stats()` output to reflect the April 2022 release of the Hurdat2 database.
+- Changed `<Season>.__getitem__` method to account for the possibility of merged basin databases, giving the user a choice between mulitple storms that occurred in the same year, but in different geographical basins with shared cyclone numbers. The East Pacific Hurdat2 is an example, natively including storms from the East and Central Pacific Basins.
+- `<TropicalCyclone>.track_map()` tweaks:
+  - focuses on the part of the track where the storm was designated a tropical cyclone.
+  - now fills more of the screen, offering a better user experience, and lessens the likelihood of the user feeling compelled to resize the initial window.
+  - added legend. By default, it will display. But if you'd rather it not display, there is a keyword to turn it off
+  - I believe it may be slightly faster now, thanks to performance tips in matplotlib docs.
+  - map coordinate lists used now significantly smaller.
+- tweaked a very minor syntax quirk. Somewhere in the code I had used `is not` instead of the more-proper `!=`.
+- `basin` tweaks
+  - introduced a new method `<Hurdat2>.basin_abbr()` which returns a list of basin abbreviations used; will be used in report outputs.
+- Fixed memory-location identification in `__repr__` methods
 
 [&#8679; back to Contents](#contents)
 
 ## Installation
 
 - At the command prompt, run `pip install hurdat2parser`
-  - When installing, packages `pyshp` and `geojson` and `matplotlib` will be downloaded as dependencies (if necessary).
-- You'll then need the actual Hurdat2 Data. You can get it [HERE](https://www.nhc.noaa.gov/data/#hurdat). It's just a text file. Hurdat2 files for the Atlantic Basin and East/Central Pacific Basins are available and compatible with the package.
+  - When installing, packages `pyshp`, `geojson`, and `matplotlib` will be downloaded as dependencies (if necessary). From scratch, it's around 30MB total of dependency downloads.
 
 [&#8679; back to Contents](#contents)
 
 ## Importing the Module
 
-- Import the module and invoke a call to the `Hurdat2` class while passing the file-name of the Hurdat2 dataset
+Follow these commands for genesis!
 
 ```python
 >>> import hurdat2parser
->>> atl = hurdat2parser.Hurdat2("path_to_hurdat2.txt")
+#or if you're lazy like me...
+>>> import hurdat2parser as hd2
 ```
-- * For the `Hurdat2` object, I highly recommend to use something shortened and readable for the parent object name (like `atl` or `al` for the Atlantic database and `ep`, `cp`, or `pac` for the East/Central Pacific)*
 
-After a few seconds you'll be ready to dive into the data! Subsequent examples imply the use of the Atlantic Hurdat2.
+- If you want a local copy of a hurdat2file, got to [https://www.nhc.noaa.gov/data/#hurdat](https://www.nhc.noaa.gov/data/#hurdat) to download. It's a text file. Hurdat2 files for the Atlantic Basin and East/Central Pacific Basins are available and compatible with the package. 
+  - As of `v2.2` this isn't 100% necessary as the datasets can be automatic retrieval can be attempted (keep reading). This method does not keep a local copy though (as of this version).
+
+To read-in a local file:<br/>`>>> atl = hurdat2parser.Hurdat2("path_to_hurdat2.txt")`
+
+And/Or to let the module download and ingest the data for you:
+
+- North Atlantic Basin<br/>`>>> atl = hurdat2parser.Hurdat2(basin="atl")`
+  - Any of the following will be recognized: `"al"`, `"atl"`, or `"atlantic"`
+- NE/CEN Pacific Basin<br/>`>>> pac = hurdat2parser.Hurdat2(basin="pac")`
+  - Any of the following will be recognized: `"pac"`, `"nepac"`, or `"pacific"`
+- Of note, the above commands do not keep a local copy for next time
+
+To include a url to download, set the kwarg `urlcheck` to `True`. This generally will not be needed unless you want to use my (shameless plug) daily-updated current-season hurdat2 during the year (on my website; see [Copyright](#copyright) section)<br/>
+`>>> atl = hurdat2parser.Hurdat2("http://crazygonuts.aboutweatherstuff/myhurdat2file.txt", urlcheck=True)`
+
+These various ways can be mixed/matched too.
+
+* For the `Hurdat2` object, I highly recommend to use something shortened and readable for the parent object name (like `atl` or `al` for the Atlantic database and `ep`, `cp`, or `pac` for the East/Central Pacific)*
+
+After a few seconds (a little longer if downloading) you'll be ready to dive into the data! Subsequent examples imply the use of the Atlantic Hurdat2 (`atl`).
+
+[&#8679; back to Contents](#contents)
+
+## Example calls
+
+There are several ways to invoke a call to a `Season` or `TropicalCyclone` object. These ways are detailed in the [next section](#hurdat2-object-structure), indirectly in the [Methods and Attribute](#methods-and-attributes) tables, and in a large portion of method docstrings. This brief section will demonstrate the ways I navigate the dataset with this module when coding and testing.
+
+- `Season` objects (just the year)
+  - `atl[1995]`
+- `TropicalCyclone` objects
+  - by atcfid number
+    - `atl[2005,12]` -- returns the object for hurricane katrina (`AL200512`)
+  - by name
+    - `atl["danny"]` -- shows a list of storms in the record given the name of Danny, allowing the user to select which one they desire
+    - `atl["_rita"]`, or `atl["-rita"]` -- beginning the name with an underscore or dash shows the most-recent storm named as such (this returns the most-notorious storms as well since storm names can be retired according to the destruction they cause)
+- `TCRecordEntry` calls
+  - `atl[1980,4,29]` -- The entry at index 29 (30th total entry) for Hurricane Allen
+  - or `atl["_allen", 29]`
 
 [&#8679; back to Contents](#contents)
 
 ## Hurdat2 Object Structure
 
 - The structure of a `Hurdat2` object is hierarchal. It has two primary dictionaries:
   - `<Hurdat2>.tc` - A dictionary containing all `TropicalCyclone` objects compiled from the record.
     - Individual storms can be accessed using their ATCF ID, a unique 8-character id for each tropical cyclone <u>OR</u> a name of a storm.
 	  - `atl["AL122005"]` - Call for Hurricane Katrina's Data using its ATCFID (it being the 12th storm from the 2005 Atlantic Season).
 	  - `atl["Name"]` - Use this if you know the name, but the year is unknown. A partial search is okay, but may receive less accurate results. It uses the `difflib` package to calculate close matches and outputs a list (if applicable) that you then can select from.
-	  - `atl["_Name"]` - including an underscore at the beginning of the name will return the **NEWEST** storm by a name that matches. Use this for the most-notoroious storms (as it would return the last-so-named storm, retired names included).
+	  - `atl["_Name"]` or `atl["-Name"]` - including an underscore or dash at the beginning of the name will return the **NEWEST** storm by a name that matches. Use this for the most-notorious storms, as retired names would be the newest.
   - `<Hurdat2>.season` - A dictionary holding `Season` objects (yearly data).
     - A Season's data is accessed via a simple year key of type `int`.
 	  - `atl[1995]` retrieves the object associated with the 1995 hurricane season.
-- `Season` objects also have a dictionary (`<Season>.tc`) that holds `TropicalCyclone` objects, specific to the year.
-  - There are 4 different ways to access individual storm data:
-    1. `atl[1995]["Opal"]` - Storm Name; Useful if you know the name a storm was issued and the season in which it occurred.
-    2. `atl[1992]["A"]` - Storm Name first-letter; I'm not saying you'd forget a named-storm like Hurricane Andrew, but this capability would grab the storm whose first-letter matched the one passed. This primarily works for modern storms (since the beginning of the satellite era), as most in the past were not named. In the Hurdat2 record, storms that were never issued a name are given "UNNAMED" for that field.
-    3. TC Number: `atl[1988][8]` - Use the storm number (type `int`) from the season. This is defined by using the ATCF ID.
-	  - This would be faster (less keystrokes): `atl[2005, 12]` - retrieves Hurricane Katrina
-    4. ATCF ID: `atl[1980]["AL041980"]` - This isn't recommended because of redundancy (it can be done without the initial call to the `1980` object).
-- `TropicalCyclone` objects contain a `list` of `TCRecordEntry` objects in time-ascending order.
-  - Though the user probably wouldn't have general/typical need to access `TCRecordEntry`-level data, it can be done via the desired index from the `<TropicalCyclone>.entry` list:
-    - `atl[2004]["ivan"][0]` - This would grab the first entry associated with the track of Hurricane Ivan.
-    - This would be faster: `atl[2005, 12, 21]` - the 22nd entry of Hurricane Katrina
+- `Season` objects also have a dictionary (`<Season>.tc`) that holds `TropicalCyclone` objects, specific to the year. Some different ways to call these objects:
+  - TC Number: `atl[1988,8]` or `atl[1988][8]` - Use the storm number (type `int`) from the season. This is defined by using the ATCF ID.
+  - Storm starting letter (or name): `atl[1995, "o"]` or `atl[1995, "opal"]` or `atl[1995]["Opal"]` - This method works for most modern tropical storms, as they have been issued names. So in these cases, you wouldn't need to know the atcfid number. Also of note, because tropical depressions aren't issued names, the id numbers do not always correlate with the co-inciding letter of the alphabet. For example, Hurricane Andrew's ATCFID is `AL041992`.
+- `TropicalCyclone` objects contain a `list` of `TCRecordEntry` objects in time-ascending order. To access these:
+  - `atl[2005, 12, 21]` would grab the `TCRecordEntry` for Hurricane Katrina at index 21.
 
 [&#8679; back to Contents](#contents)
 
 ## Methods and Attributes
 
 Now that you know how to call a particular object of interest, you can now access its data, using methods and attributes. The docstrings (accessed via `help()`) are quite detailed and methods that take arguments have example calls listed. But here is a quick reference to what is available, along with some shortcuts and example calls to assist navigating while in this document.
 
@@ -114,17 +189,18 @@
 `rank_climo(...)` | Yet another useful ranking method. This allows one to rank attributes assessed over several to many years (climatological periods) to one another. Optional keyword argument `climatology` (default is 30 years) controls the span of time that data is collected and `increment` (default is 5 years) dictates the temporal distance between periods | `atl.rank_climo(20,"track_distance_TC", climatology=10, increment=1)`
 `rank_storms(...)` | Print a report that compares storms and their attributes to each other. Similar to the above methods, other data is included in the report. See the docstring for info on `coordextent` kw usage | `atl.rank_storms(20,"HDP",1967)`
 `multi_season_info(...)` | Prints a report a gathered statistics based on a range of years. This is similar to the `info()` methods referenced in the next section. This could be thought of as an info method for a climatological period | `atl.multi_season_info(1991, 2000)`<br />`atl[2010, 2019]`
 `storm_name_search(...)` | Search through the entire Hurdat2 record for storms issued a name. If the positional keyword `info` is `True`, the matching storm's info method will print. | `atl.storm_name_search("Hugo")`
 `output_climo(...)` | outputs a .csv file using the `csv` package of 1-year incremented climatological periods. This csv file can then be opened in a spreadsheet program. To compare or rank, the spreadsheet GUI layout is much easier to use especially due to instant sorting and filtering. This accepts a positional keyword argument (`climatology=30`). | `atl.output_climo(15)`
 `output_seasons_csv(...)` | Similar to the above, but for seasons. It takes no arguments. In other words, it would be redundant to run it multiple times, because as the `hurdat2parser` package doesn't natively allow modification of the data, it would just output the same data over and over. The only exception would be when the Hurdat2 database is updated by the NHC. With this in mind, it will automatically write-over the csv if it already exists (file-name is auto-generated within the method). | `atl.output_seasons_csv()`
 `output_storms_csv(...)` | Similar to above, but for individual storms. | `atl.output_storms_csv()`
+`climograph()` | displays a graph of the climatological tendency of a variable over multiple seasons (see docstring for a how-to) | `atl.climograph("ACE", 10, 1, year1=1967)`
 `coord_contains(...)` | Takes 3 tupled lat-lon coordinates. The purpose is to inquire whether the first arg (the test coordinate) is contained within a bounding box formed by the other two coordinates passed (returns a `bool`. This is generally just accessed via the ranking methods | `atl.coord_contains(`<br />&nbsp;&nbsp;&nbsp;&nbsp;`[30.4,-85.0]`,<br />&nbsp;&nbsp;&nbsp;&nbsp;`[31.5, 86.0],`<br />&nbsp;&nbsp;&nbsp;&nbsp;`[29.0, 84.0]`<br />`) -> True`
-`BASIN_DICT` | A dictionary containing abbreviations (keys) and definitions (values) of various basins around the world that hurricane data is kept. This is referenced via the `basin()` method. The data used to form this object came from IBTrACS | `<Hurdat2>.BASIN_DICT`
-`basin(season=None)` | Interprets and returns a readable string identifying the TC basin based on the storms within the record. This allows support of dynamically-created singular OR multiple Hurdat2 datasets OR individual seasons (if a `Season` object is passed to the method). | `atl.basin -> "North Atlantic Basin"
+`BASIN_DICT` | A dictionary containing abbreviations (keys) and definitions (values) of various basins around the world that hurricane data is kept. This is referenced via the `basin()` method. The data used to form this object came from IBTrACS | `atl.BASIN_DICT`
+`basin(season=None)` | Interprets and returns a readable string identifying the TC basin based on the storms within the record. This allows support of dynamically-created singular OR multiple Hurdat2 datasets OR individual seasons (if a `Season` object is passed to the method). The data used to form this property came from IBTrACS | `atl.basin() -> "North Atlantic Basin"
 `record_range` | Returns a tuple of the beginning year and end year of the Hurdat2 record | `atl.record_range -> (1851, 2020)`
 
 [&#8679; back to Methods &amp; Attributes](#methods-and-attributes)
 
 #### Shared Methods and Attributes for `Season` and `TropicalCyclone`
 
 Attributes | Description | Examples
@@ -135,97 +211,132 @@
 `landfalls`<br /> | \*SEE [DISCLAIMER FOR LANDFALL INFO](#landfall-data)\* Sum of all landfalls (remember, a storm can make multiple landfalls). `<Season>.landfalls` is also an unfiltered aggregate of its storms landfalls. At the seasonal level, you'd probably be more interested in the attribute `landfall_TC` (see following section) | `atl[1960]["doNnA"].landfalls`
 `landfall_<STATUS>`<br />*\-can be TC, TD, TS, HU, or MHU* | `Season`: qty of TC's that made landfall as the inquired status; `TropicalCyclone`: `bool` indicating if the storm made landfall while the inquired status<br />*\-CAUTION: These attrs are exclusive of landfalls made while of stronger designation\-* | `atl[1996].landfall_TS -> 2`<br />`atl[2011]["I"].landfall_HU -> True`
 `<STATUS>reach`<br />*\-can be TC, TD, TS, HU, or MHU* | `Season`: qty of TC's that reached <u>at least</u> the inquired status; `TropicalCyclone`: `bool` indicating if the storm ever was designated as the inquired status | `atl[2010].HUreach -> 12`<br />`atl[1991]["danny"].HUreach -> False`
 `ACE`, `HDP`, or `MHDP` | Returns the specified Energy Index reading associated with the season or storm. Note that the MHDP is one you likely won't see elsewhere. It's formula is the same as ACE and HDP but for major-hurricanes only | `atl[1966].HDP`
 `track_distance` | The calculated distance (in nmi) for the entire track of the storm (or aggregate of the season), regardless of status | `atl[1954]["hazel"].track_distance`
 `track_distance_<STATUS>`<br>*\-can be TC, TD, TS, HU, or MHU* | The distance traversed while storm(s) was(were) <u>at least</u> the status designation | `atl[1961].track_distance_MHU`
 `cat45reach`<br>`cat5reach` | For `Season` objects, returns the quantity of storms that reached category 4+ status or category 5 status (respectively)<br>For `TropicalCyclone` objects, returns a `bool`, indicating if the TC ever achieved cat 4+ or 5 status (respectively) | `atl[2020].cat45reach -> 5`<br>`atl[2020].cat5reach -> 0`<br>`atl[2020]["Iota"].cat5reach -> False`
-`maxwind_mslp`<br>`minmslp_wind` | Returns the MSLP (wind) occurring at the time of peak-winds (minimum MSLP) respectively. These attributes were included because peak winds and minimum MSLP do not necessarily occur at the same time. | `atl[2015]["joaquin"].maxwind_mslp -> 934`<br>`atl[2015]["joaquin"].minmslp_wind -> 120`<br>\* This example was given as Joaquin's peak winds (135) were not observed at the time of Joaquin's minimum MSLP (931)
 `hurdat2()` | This method prints a hurdat2-formatted output of the storms's data, emulating the actual hurdat2 record from which it (the Season or Tropical Cyclone) was created | `atl[2005].hurdat2()`
+`duration` | Returns the length of the Season or life of the cyclone (Of note, the `TropicalCyclone` property disregards storm status) | `atl[2022].duration`
+`tc_entries` | Returns a list of `TCRecordEntry`'s from where a storm was designated as a tropical cyclone | `atl["_katrina"].tc_entries`
+`start_date` | The beginning moment of the Season or storm | `atl[1938].start_date`
+`start_ordinal` | The quantified day of the year of the beginning moment of the Season or storm | `atl[1938].start_ordinal`
+`end_date` | The ending date of the Season or storm | `atl[1954, 16].end_date`
+`end_ordinal` | The quantified day of the year of the ending date of the Season or storm | `atl[1954].end_ordinal`
 
 [&#8679; back to Methods &amp; Attributes](#methods-and-attributes)
 
 #### `Season` Only Methods and Attributes
 Attribute | Description | Example
 :---: | :---: | :---:
 `output_shp_segmented()` | Generates a shapefile including each segment from each tropical-cyclone from a given season; each individual segment from each individual storm will be represented | `atl[1932].output_shp_segmented()`
 `output_geojson_segmented()` | Generates a geojson including each segment from each tropical-cyclone from a given season; each individual segment from each individual storm will be representeds | `atl[2003].output_geojson_segmented()`
 `tracks` | Returns the quantity of tropical cyclones from a season | `atl[1995].tracks`
 `<STATUS>only`<br />*\-can be TD, TS, or HU* | Returns the quantity of TC's from a season that made were given the inquired designation, but never strengthened beyond it. `HUonly` implies Category 1 and 2 storms only. To inquire about `MHU`, use the `MHUreach` attr | `atl[1950].TDonly`<br />`atl[2017].HUonly`
-`stats()` | prints a report filled with statistics and ranks for the season, optionally compared with a subset of seasons and/or partial seasons. For `TropicalCyclones`, this is a mirror-method of `.info()` | `atl[2020].stats()`<br>`atl[2005].stats(thru=(9,30))`<br>`atl[1989]["hugo"].stats()
+`stats()` | prints a report filled with statistics and ranks for the season, optionally compared with a subset of seasons and/or partial seasons. Though it technically exists as a  `TropicalCyclone` method, its iteration is a mirror-method of `.info()` | `atl[2020].stats()`<br>`atl[2005].stats(thru=(9,30))`
 
 [&#8679; back to Methods &amp; Attributes](#methods-and-attributes)
 
 #### `TropicalCyclone` Only Methods and Attributes
 | Attribute | Description | Example
 :---: | :---: | :---:
-`coord_list()` | Prints a report with entry dates and the associated Latitude and Longitude | `atl[2005]["rita"].coord_list()`
-`gps` | Returns a `list` of tupled latitude and Longitude coordinates | `atl[1998]["MITCH"].coord_list()`
+`gps` | Returns a `list` of tupled latitude and Longitude coordinates | `atl[1998]["MITCH"].gps`
+`maxwind` | Returns the highest maximum sustained wind-speed observed in the tropical cyclone | `atl["_katrina"].maxwind`
 `minmslp` | Returns the lowest recorded pressure of the TC | `atl[1955][10].minmslp`
+`maxwind_mslp`<br>`minmslp_wind` | Returns the MSLP (wind) occurring at the time of peak-winds (minimum MSLP) respectively. These attributes were included because peak winds and minimum MSLP do not necessarily occur at the same time. | `atl[2015]["joaquin"].maxwind_mslp -> 934`<br>`atl[2015]["joaquin"].minmslp_wind -> 120`<br>\* This example was given as Joaquin's peak winds (135) were not observed at the time of Joaquin's minimum MSLP (931)
 `<EI>_per_nmi`<br />*\-can be ACE, HDP, or MHDP* | Returns the inquired energy index divided by the track distance covered while the energy index was being contributed to (`ACE` &rarr; `track_distance_TS` or `HDP` &rarr; `track_distance_HU` as examples). WARNING! These attributes do not have any kind of threshold controls, so storms which were short-lived can have high values | `atl[1964][10].HDP_per_nmi`<br />`atl[2016]["matthew"].ACE_per_nmi`
 `<EI>_perc_ACE` &rarr; *\-can be HDP or MHDP*<br />`HDP_perc_MHDP` | Simply the storm's HDP or MHDP divided by ACE or the MHDP divided by the HDP. Look at this as the <u>percentage</u> (as a float between 0 and 1) of the storm's ACE or HDP that was contributed to while a Hurricane or Major Hurricane, respectively | `atl[2017]["IRMA"].HDP_perc_ACE`
 `track_<EI1>_perc_<EI2>`<br />*\-&lt;EI1&gt; can be TS, HU, or MHU*<br />*\-&lt;EI2&gt; can be TC, TS, HU, or MHU* | Returns the the storm's &lt;EI2&gt; track_distance divided by the track distance while of status &lt;EI1&gt;. &lt;EI1&gt; must be of higher hierarchal status than &lt;EI2&gt; | `atl[2005][25].track_HU_perc_TC`<br />`atl[2003]["Fabian"].track_MHU_perc_TS`
 `track_map()` | Generates a map of the storm's track using `matplotlib`. Check the docstring for ways to modify the output to your liking. | `atl["_katrina"].track_map()`
 `perc_ACE`<br>`perc_HDP`<br>`perc_MHDP` | Return the percentage (in decimal form) of the contribution of the storm's ACE, HDP, or MHDP value to the season's value | `atl["_matthew"].perc_MHDP
-`info()` | Prints basic stats for the tropical cyclone | `atl[1989]["hugo"].info()`
+`info()` | Prints basic stats for the tropical cyclone | `atl[2005][12].info()`
+`ACE_no_landfall` | Returns the ACE of the storm prior to any landfall made | `atl["_ivan"].ACE_no_landfall
+`duration_<SUFFIX>`<br />*\*&lt;SUFFIX&gt; can be TC, TS, HU, MHU* | Returns the aggregated length in days that the cyclone spent as on of the given statuses. These do account for storm status loss and possible reaquisition | `atl["_irma"].duration_MHU`
 
 [&#8679; back to Methods &amp; Attributes](#methods-and-attributes)
 
 #### `TCRecordEntry` Attributes
 
-- As mentioned earlier, there's generally no need to access`TCRecordEntry` objects directly. Only the most-common attributes will be referenced in this document. A comprehensive list is available via `help`
+- Only the most-common attributes will be referenced in this document. A comprehensive list is available via `help`
 
 | Attribute | Description
 :---: | :---:
 `entrytime` | A `datetime.datetime` object of the entry's timestamp
 `status` | The designated 2-letter abbreviation representing the storm's status
 `location`<br />`location_rev` | A tuple of the latitude/longitude coordinates; `location_rev` is reversed in order, a longitude/latitude tuple; seemingly favored for GIS use.
 `wind` | The maximum-sustained winds at the time of entry-recording
 `mslp` | The Mean Sea-Level Pressure (in hPa or mb) at the time of entry-recording
 `hurdat2()` | Returns a reassembled Hurdat2-formatted string, identical to the one parsed to create the entry
-`wind_radii` | The Radius of Maximum Winds. *As of the May 2022 release of the Hurdat2 database, this is a new variable and the availability of it belongs solely to the 2021 Hurricane season (for now).*
+`maxwind_radius` | The Radius of Maximum Winds. Currently, it is only available for storms since 2021, and is assumed that in subsequent releases, this variable will continue to be updated. It is unknown if this data for previous seasons will (or can) be back-filled.
+`avg_wind_extent_<SUFFIX>`<br/>Suffix can be `TS`, `TS50`, or `HU` | The statistical mean of the reported wind-extents (quadrants). Wind extents are only available for storms since 2004 
+`areal_extent_<SUFFIX>`<br/>Suffix can be `TS`, `TS50`, or `HU` | The calculated area covered by the extent of winds of specified strengths (of note, wind extents are only available for storms since 2004)
+`track_distance`<br/>`track_distance_<SUFFIX>`<br/>Suffix can be `TC`, `TS`, `HU`, or `MHU` | returns the distance tracked by the system from its genesist to the point of the entry. The variables with suffixes do account for status in their calculations
+`previous_entry`<br/>`next_entry` | Returns the entry prior-to or after the `TCRecordEntry` that it is called from
+`direction()` | Returns the heading in degrees that the storm is going. A readable cardinal direction can be returned if `True` is passed to the method
+`speed` | The average speed between the previous entry and this one in nm/h<br/>Of Note, remember that the `Hurdat2` spatial resolution is 0.1 degrees latitude/longitude. So some appreciable error may be present
 
 [&#8679; back to Methods &amp; Attributes](#methods-and-attributes)<br />
 [&#8679; back to Contents](#contents)
 
 ## Landfall Data
 
 An important point to keep in mind when viewing data and ranking, Hurdat2's landfall data is incomplete. It is progressively being updated in conjunction with the yearly release of the dataset. Please see the documentation  [Hurdat2 Format Guide](https://www.nhc.noaa.gov/data/hurdat/hurdat2-format-atl-1851-2021.pdf) for more detail on currently-available landfall data temporal scope.
 
 [&#8679; back to Contents](#contents)
 
+## Access to Future Methods
+
+In `_future.py`, I have some stuff that I've started to develop but not ready/sure to release. The methods are functional though. The quickest way of accessing it is:
+
+```python
+>>> import hurdat2parser._future as future
+```
+
+Valid classes reflect those of the main `hurdat2parser` object, namely `future.Hurdat2`, `future.Season`, `future.TropicalCyclone`, or `future.TCRecordEntry`. They'll be empty if I don't have anything I'm currently developing for that respective class/object. You can see what methods I have available by running `dir()` on the class.
+
+When calling, you will need to manually pass a valid object (a substitute for `self`). For example:
+```python
+>>> future.Season.track_map(atl[1984])
+```
+
+[&#8679; back to Contents](#contents)
+
 ## Roadmap
 
+- [ ] Include more `Season.duration`-related properties based on status
 - [ ] Speed-up `<Season>.stats()` report; because it employs `rank_seasons_thru`, and since that is quite snappy, I think the `stats()` method should be quick too. I'll investigate.
-- [ ] Include a `track_map()` method for `Season`
-- [ ] Include legends for `<TropicalCyclone>.track_map()`
+- [ ] Develop matplotlib-based graphs located in `_future`
 - [ ] Comparison methods to directly compare one season to another or specific storms to another.
-- [ ] Formulate a `stats()` method for `TropicalCyclone`s (to eventually replace their `info` method); including ranking/comparing to storms across the record or a subset of seasons, including a `rank_storms_thru()` companion method for `Hurdat2` objects.
+- [ ] Revamp `hurdat2()` method of `TropicalCyclone` and `Season` objects to optionally return a string instead of merely printing to console
+- [ ] Formulate a `stats()` method for `TropicalCyclone`s (to eventually replace their `info` method); including ranking/comparing to storms across the record or a subset of seasons (right now, this method is just a wrapper for the `info()` method.
 - [ ] Track distance percentage of season total for `TropicalCyclone`s
 - [ ] Maybe simpler rank methods so values sought for ranking will guarantee to show
-- [X] Deprecate `<Season>.info()` method
-- [x] Inclusion of `matplotlib` methods
+- [ ] add maps files for Pacific-centric storms
+- [ ] investigate adding a minmslp_entry or maxwind_entry property for TropicalCyclone objects. It is acknowledged though that multiple entries can have the same minimum mslp or max wind.
+- [ ] a `genesis` property, returning the first entry from a `TropicalCyclone` earning the TC designation. Not sure the feasability of this. I'll think about it.
+- [x] Include legends for `<TropicalCyclone>.track_map()`
+- [x] Account for absent season starts when using stats thru certain time
 
 [&#8679; back to Contents](#contents)
 
 ## Credits
 
-- Hurdat Reference: `Landsea, C. W. and J. L. Franklin, 2013: Atlantic Hurricane Database Uncertainty and Presentation of a New Database Format. Mon. Wea. Rev., 141, 3576-3592.`
+- HURDAT Reference: `Landsea, C. W. and J. L. Franklin, 2013: Atlantic Hurricane Database Uncertainty and Presentation of a New Database Format. Mon. Wea. Rev., 141, 3576-3592.`
 - [Haversine Formula (via Wikipedia)](https://en.wikipedia.org/wiki/Haversine_formula)
 - Bell, et. al. Climate Assessment for 1999. *Bulletin of the American Meteorological Society.* Vol 81, No. 6. June 2000. S19.
 - <span>G. Bell, M. Chelliah.</span> *Journal of Climate.* Vol. 19, Issue 4. pg 593. 15 February 2006.
 - [Hurdat2 Format Guide (PDF)](https://www.nhc.noaa.gov/data/hurdat/hurdat2-format-atl-1851-2021.pdf)
 - [Natural Earth](https://www.naturalearthdata.com/) GIS Data (data extracted there-from to display maps)
 
 [&#8679; back to Contents](#contents)
 
 ## Copyright
 
 **Author**: Kyle S. Gentry<br />
-Copyright &copy; 2019-2022, Kyle Gentry (KyleSGentry@outlook.com)<br />
+Copyright &copy; 2019-2023, Kyle Gentry (KyleSGentry@outlook.com)<br />
 **License**: MIT<br />
 **GitHub**: [https://github.com/ksgwxfan/hurdat2parser](https://github.com/ksgwxfan/hurdat2parser)<br />
 **Author's Webpages**:
  - [https://ksgwxfan.github.io/](https://ksgwxfan.github.io/)<br />
  - [http://echotops.blogspot.com/](http://echotops.blogspot.com/)
 
 [&#8679; back to Contents](#contents)
```

### Comparing `hurdat2parser-2.11/README.md` & `hurdat2parser-2.2/hurdat2parser.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,176 @@
-# hurdat2parser -- v2.11
+Metadata-Version: 2.1
+Name: hurdat2parser
+Version: 2.2
+Summary: Interpret Hurricane Data contained in HURDAT2
+Home-page: http://github.com/ksgwxfan/hurdat2parser
+Author: Kyle S. Gentry
+Author-email: KyleSGentry@outlook.com
+License: MIT
+Keywords: hurricane hurdat2 meteorology weather
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# hurdat2parser -- v2.2
 ---
-### *Interpreting the HURDAT2 Tropical Cyclone Dataset using Python*
+### *Interpreting the Hurdat2 Tropical Cyclone Dataset using Python*
 
 Hurdat2 ([https://www.nhc.noaa.gov/data/#hurdat](https://www.nhc.noaa.gov/data/#hurdat)) is a collection of records from individual Tropical Cyclones. The two primary Hurdat2 records are for the Atlantic (since 1850) and East/Central-Pacific Oceans (since 1949).
 
 The purpose of this module is to provide a quick way to analyze the Hurdat2 datasets. It includes methods for retrieving, inspecting, ranking, or even exporting data for seasons, individual storms, or climatological eras.
 
-This release is primarily a "patch" in response to the newest release of the Hurdat2 database (official inclusion of data from the 2021 season). A new variable has been introduced, and this release accommodates it. But all previous versions of `hurdat2parser` will not be compatible with this and (likely) future Hurdat2 databases. But this (`2.11`) and all future versions of this program will be backward compatible to previous versions of the database.
-
 PyPI Link: [https://pypi.org/project/hurdat2parser/](https://pypi.org/project/hurdat2parser/)
 
 ## Contents
-* [Changes/Fixes in this Version (2.11)](#changes-in-this-version-211)
+* [Changes/Fixes in this Version (2.2)](#changes-in-this-version-22)
 * [Requirements, Installation, and getting the data](#installation)
 * [Importing the module](#importing-the-module)
+* [Example Calls](#example-calls)
 * [Hurdat2 Object Structure](#hurdat2-object-structure)
 * [Methods &amp; Attributes](#methods-and-attributes)
 * [Note on Landfall Data](#landfall-data)
+* [Future/Under-Development/Unreleased Methods](#access-to-future-methods)
 * [Roadmap](#roadmap)
 * [Credits](#credits)
 * [Copyright/License](#copyright)
 
-## Changes in this Version (2.11)
-- Patched to enable compatibility with the May 2022 release of the Hurdat2 database
-- Added a `TCRecordEntry` variable called `wind_radii` (the new variable included in the May 2022 Hurdat2 release. There may be some future potential in expanding the use of this variable, but its availability is currently limited to the 2021 Hurricane Season
-- Fixed calls to `TCRecordEntry` variables `avg_wind_extent_<STATUS>`
-- `info()` method for `Season` objects removed (use the `stats()` method instead)
-- modification of `<Hurdat2>.basin()`; now a method instead of property.
-- Fixed `rank_seasons_thru()` where a call without keywords (becoming a wrapper for `rank_seasons`) had an ill-advised direct call to a dictionary key instead of the get method
+## Changes in this Version (2.2)
+
+- Docstring'd `TCRecordEntry` properties
+- Changes to the `<Hurdat2>` object:
+  - when reading-in files on `__init__`, multiple local files are now supported.
+  - enabled download of the most-recent hurdat2 dataset through the `basin` kwarg.
+  - added a `urlcheck` kwarg. If `True`, the "file-path"s listed will be treated like URLs and a download attempt will be made.
+  - removed the `_filesappended` attribute
+  - Searching for notoriously-named storms can be done by a dash (`"-"`) prefix to the search string in addition to an underscore (see [Example Calls](#example-calls) section)
+  - Revamped `output_climo_csv`, `output_season_csv`, and `output_storms_csv` methods
+    - simplified code; updated and unified attributes used in the reports and made it significantly easier for future maintenance.
+  - moved `multi_season_info` method to `_reports`
+- New properties for both `Season` and `TropicalCyclone`:
+  - `duration`
+    - `Season` version reports time between the first and last day of the season (see further in the document for explanation)
+	- `TropicalCyclone` version just reports the track-life in days, regardless of status. More useful status-based duration properties were created too. Keep reading (a few lines down).
+  - `tc_entries` returns a list of `TCRecordEntry`s where a storm was a designated tropical cyclone.
+  - `start_date`, `start_ordinal`, and `end_date`, `end_ordinal` report the starting/ending dates and/or days of the year
+- New `TropicalCyclone` variables:
+  - `ACE_no_landfall`
+  - `duration_<TC, TS, HU, MHU>` - These properties report the aggregate time in days that a tropical cyclone was designated that status or stronger, accounting for fluxuations in storm statuses and strengths.
+  - removed `coord_list` method. It was redundant as it was like a shortened combination of the `summary` method.
+- New `TCRecordEntry` variables:
+  - tweaked how location variables are defined. `location` and `location_reversed` are now properties that depend on the express definition of the variables `lat` and `lon` rather than the other way around.
+  - tweak of not-available wind-extent data. As of the moment typing this, wind-extent data is only provided for storms since 2004. All previous wind-extent data is `-999`, meaning its unavailable. But if a storm has max winds of `<` 64, its Hurricane wind extent has to be 0. So when ingesting the data, this determination is made.
+  - tweaked ingest of data to prevent errors due to possible new Hurdat2 categories introduced in future versions. This was the problem with `v2.1` that was responsible for the need for a `v2.11` release. This particular version wouldn't be able to read-in the new variables in such a situation, but it would still be functional with the newer database (unless order of variables are switched around).
+  - the formerly-called variable `wind_radii` from `v2.11` is now called `maxwind_radius`. I don't know why I called it `radii`, as in plural of radius. I guess it sounded science-y or smart. haha. But the change is also more readable.
+  - Surface Area (coverage)-based variables `areal_extent_TS`, `areal_extent_TS50`, and `areal_extent_HU`.
+    - These are calculated from reported wind-extents in the database.
+  - `track_distance`: the track distance of the cyclone up to the point of the respective entry; this does not account for storm status
+  - `previous_entries` and `next_entries`: lists of the previous and next recorded entries, respectively, in the `TropicalCyclone`'s record
+  - `previous_entry` and `next_entry`: the previous and next recorded entry, respectively, in the `TropicalCyclone`'s record
+  - `direction()`: the `TropicalCyclone`'s heading in degrees (or cardinal, if desired...see docstring)
+  - `speed`: the `TropicalCyclone`'s forward speed in knots.
+  - Properties to simplify coding and reduce probability of coding errors.
+    - `is_TC`: `bool` indicating whether or not a storm was designated as a tropical cyclone at the `<TCRecordEntry>.entrytime`.
+    - `is_synoptic`: `bool` indicating whether or not an entry occurred at a synoptic time (0Z, 6Z, 12Z, 18Z).
+- Added `report_type` default keyword argument to the `<Season>.stats` method. User can dictate if report prints to the console or gets back a string version of the report.
+- Fixed an exclusion of `maxwind_radius` (formerly called `wind_radii`) from `<TCRecordEntry>.hurdat2()` calls. (which was only introduced in the previous version).
+- Tweaked landfall-disclaimer in `<Season>.stats()` output to reflect the April 2022 release of the Hurdat2 database.
+- Changed `<Season>.__getitem__` method to account for the possibility of merged basin databases, giving the user a choice between mulitple storms that occurred in the same year, but in different geographical basins with shared cyclone numbers. The East Pacific Hurdat2 is an example, natively including storms from the East and Central Pacific Basins.
+- `<TropicalCyclone>.track_map()` tweaks:
+  - focuses on the part of the track where the storm was designated a tropical cyclone.
+  - now fills more of the screen, offering a better user experience, and lessens the likelihood of the user feeling compelled to resize the initial window.
+  - added legend. By default, it will display. But if you'd rather it not display, there is a keyword to turn it off
+  - I believe it may be slightly faster now, thanks to performance tips in matplotlib docs.
+  - map coordinate lists used now significantly smaller.
+- tweaked a very minor syntax quirk. Somewhere in the code I had used `is not` instead of the more-proper `!=`.
+- `basin` tweaks
+  - introduced a new method `<Hurdat2>.basin_abbr()` which returns a list of basin abbreviations used; will be used in report outputs.
+- Fixed memory-location identification in `__repr__` methods
 
 [&#8679; back to Contents](#contents)
 
 ## Installation
 
 - At the command prompt, run `pip install hurdat2parser`
-  - When installing, packages `pyshp` and `geojson` and `matplotlib` will be downloaded as dependencies (if necessary).
-- You'll then need the actual Hurdat2 Data. You can get it [HERE](https://www.nhc.noaa.gov/data/#hurdat). It's just a text file. Hurdat2 files for the Atlantic Basin and East/Central Pacific Basins are available and compatible with the package.
+  - When installing, packages `pyshp`, `geojson`, and `matplotlib` will be downloaded as dependencies (if necessary). From scratch, it's around 30MB total of dependency downloads.
 
 [&#8679; back to Contents](#contents)
 
 ## Importing the Module
 
-- Import the module and invoke a call to the `Hurdat2` class while passing the file-name of the Hurdat2 dataset
+Follow these commands for genesis!
 
 ```python
 >>> import hurdat2parser
->>> atl = hurdat2parser.Hurdat2("path_to_hurdat2.txt")
+#or if you're lazy like me...
+>>> import hurdat2parser as hd2
 ```
-- * For the `Hurdat2` object, I highly recommend to use something shortened and readable for the parent object name (like `atl` or `al` for the Atlantic database and `ep`, `cp`, or `pac` for the East/Central Pacific)*
 
-After a few seconds you'll be ready to dive into the data! Subsequent examples imply the use of the Atlantic Hurdat2.
+- If you want a local copy of a hurdat2file, got to [https://www.nhc.noaa.gov/data/#hurdat](https://www.nhc.noaa.gov/data/#hurdat) to download. It's a text file. Hurdat2 files for the Atlantic Basin and East/Central Pacific Basins are available and compatible with the package. 
+  - As of `v2.2` this isn't 100% necessary as the datasets can be automatic retrieval can be attempted (keep reading). This method does not keep a local copy though (as of this version).
+
+To read-in a local file:<br/>`>>> atl = hurdat2parser.Hurdat2("path_to_hurdat2.txt")`
+
+And/Or to let the module download and ingest the data for you:
+
+- North Atlantic Basin<br/>`>>> atl = hurdat2parser.Hurdat2(basin="atl")`
+  - Any of the following will be recognized: `"al"`, `"atl"`, or `"atlantic"`
+- NE/CEN Pacific Basin<br/>`>>> pac = hurdat2parser.Hurdat2(basin="pac")`
+  - Any of the following will be recognized: `"pac"`, `"nepac"`, or `"pacific"`
+- Of note, the above commands do not keep a local copy for next time
+
+To include a url to download, set the kwarg `urlcheck` to `True`. This generally will not be needed unless you want to use my (shameless plug) daily-updated current-season hurdat2 during the year (on my website; see [Copyright](#copyright) section)<br/>
+`>>> atl = hurdat2parser.Hurdat2("http://crazygonuts.aboutweatherstuff/myhurdat2file.txt", urlcheck=True)`
+
+These various ways can be mixed/matched too.
+
+* For the `Hurdat2` object, I highly recommend to use something shortened and readable for the parent object name (like `atl` or `al` for the Atlantic database and `ep`, `cp`, or `pac` for the East/Central Pacific)*
+
+After a few seconds (a little longer if downloading) you'll be ready to dive into the data! Subsequent examples imply the use of the Atlantic Hurdat2 (`atl`).
+
+[&#8679; back to Contents](#contents)
+
+## Example calls
+
+There are several ways to invoke a call to a `Season` or `TropicalCyclone` object. These ways are detailed in the [next section](#hurdat2-object-structure), indirectly in the [Methods and Attribute](#methods-and-attributes) tables, and in a large portion of method docstrings. This brief section will demonstrate the ways I navigate the dataset with this module when coding and testing.
+
+- `Season` objects (just the year)
+  - `atl[1995]`
+- `TropicalCyclone` objects
+  - by atcfid number
+    - `atl[2005,12]` -- returns the object for hurricane katrina (`AL200512`)
+  - by name
+    - `atl["danny"]` -- shows a list of storms in the record given the name of Danny, allowing the user to select which one they desire
+    - `atl["_rita"]`, or `atl["-rita"]` -- beginning the name with an underscore or dash shows the most-recent storm named as such (this returns the most-notorious storms as well since storm names can be retired according to the destruction they cause)
+- `TCRecordEntry` calls
+  - `atl[1980,4,29]` -- The entry at index 29 (30th total entry) for Hurricane Allen
+  - or `atl["_allen", 29]`
 
 [&#8679; back to Contents](#contents)
 
 ## Hurdat2 Object Structure
 
 - The structure of a `Hurdat2` object is hierarchal. It has two primary dictionaries:
   - `<Hurdat2>.tc` - A dictionary containing all `TropicalCyclone` objects compiled from the record.
     - Individual storms can be accessed using their ATCF ID, a unique 8-character id for each tropical cyclone <u>OR</u> a name of a storm.
 	  - `atl["AL122005"]` - Call for Hurricane Katrina's Data using its ATCFID (it being the 12th storm from the 2005 Atlantic Season).
 	  - `atl["Name"]` - Use this if you know the name, but the year is unknown. A partial search is okay, but may receive less accurate results. It uses the `difflib` package to calculate close matches and outputs a list (if applicable) that you then can select from.
-	  - `atl["_Name"]` - including an underscore at the beginning of the name will return the **NEWEST** storm by a name that matches. Use this for the most-notoroious storms (as it would return the last-so-named storm, retired names included).
+	  - `atl["_Name"]` or `atl["-Name"]` - including an underscore or dash at the beginning of the name will return the **NEWEST** storm by a name that matches. Use this for the most-notorious storms, as retired names would be the newest.
   - `<Hurdat2>.season` - A dictionary holding `Season` objects (yearly data).
     - A Season's data is accessed via a simple year key of type `int`.
 	  - `atl[1995]` retrieves the object associated with the 1995 hurricane season.
-- `Season` objects also have a dictionary (`<Season>.tc`) that holds `TropicalCyclone` objects, specific to the year.
-  - There are 4 different ways to access individual storm data:
-    1. `atl[1995]["Opal"]` - Storm Name; Useful if you know the name a storm was issued and the season in which it occurred.
-    2. `atl[1992]["A"]` - Storm Name first-letter; I'm not saying you'd forget a named-storm like Hurricane Andrew, but this capability would grab the storm whose first-letter matched the one passed. This primarily works for modern storms (since the beginning of the satellite era), as most in the past were not named. In the Hurdat2 record, storms that were never issued a name are given "UNNAMED" for that field.
-    3. TC Number: `atl[1988][8]` - Use the storm number (type `int`) from the season. This is defined by using the ATCF ID.
-	  - This would be faster (less keystrokes): `atl[2005, 12]` - retrieves Hurricane Katrina
-    4. ATCF ID: `atl[1980]["AL041980"]` - This isn't recommended because of redundancy (it can be done without the initial call to the `1980` object).
-- `TropicalCyclone` objects contain a `list` of `TCRecordEntry` objects in time-ascending order.
-  - Though the user probably wouldn't have general/typical need to access `TCRecordEntry`-level data, it can be done via the desired index from the `<TropicalCyclone>.entry` list:
-    - `atl[2004]["ivan"][0]` - This would grab the first entry associated with the track of Hurricane Ivan.
-    - This would be faster: `atl[2005, 12, 21]` - the 22nd entry of Hurricane Katrina
+- `Season` objects also have a dictionary (`<Season>.tc`) that holds `TropicalCyclone` objects, specific to the year. Some different ways to call these objects:
+  - TC Number: `atl[1988,8]` or `atl[1988][8]` - Use the storm number (type `int`) from the season. This is defined by using the ATCF ID.
+  - Storm starting letter (or name): `atl[1995, "o"]` or `atl[1995, "opal"]` or `atl[1995]["Opal"]` - This method works for most modern tropical storms, as they have been issued names. So in these cases, you wouldn't need to know the atcfid number. Also of note, because tropical depressions aren't issued names, the id numbers do not always correlate with the co-inciding letter of the alphabet. For example, Hurricane Andrew's ATCFID is `AL041992`.
+- `TropicalCyclone` objects contain a `list` of `TCRecordEntry` objects in time-ascending order. To access these:
+  - `atl[2005, 12, 21]` would grab the `TCRecordEntry` for Hurricane Katrina at index 21.
 
 [&#8679; back to Contents](#contents)
 
 ## Methods and Attributes
 
 Now that you know how to call a particular object of interest, you can now access its data, using methods and attributes. The docstrings (accessed via `help()`) are quite detailed and methods that take arguments have example calls listed. But here is a quick reference to what is available, along with some shortcuts and example calls to assist navigating while in this document.
 
@@ -97,17 +189,18 @@
 `rank_climo(...)` | Yet another useful ranking method. This allows one to rank attributes assessed over several to many years (climatological periods) to one another. Optional keyword argument `climatology` (default is 30 years) controls the span of time that data is collected and `increment` (default is 5 years) dictates the temporal distance between periods | `atl.rank_climo(20,"track_distance_TC", climatology=10, increment=1)`
 `rank_storms(...)` | Print a report that compares storms and their attributes to each other. Similar to the above methods, other data is included in the report. See the docstring for info on `coordextent` kw usage | `atl.rank_storms(20,"HDP",1967)`
 `multi_season_info(...)` | Prints a report a gathered statistics based on a range of years. This is similar to the `info()` methods referenced in the next section. This could be thought of as an info method for a climatological period | `atl.multi_season_info(1991, 2000)`<br />`atl[2010, 2019]`
 `storm_name_search(...)` | Search through the entire Hurdat2 record for storms issued a name. If the positional keyword `info` is `True`, the matching storm's info method will print. | `atl.storm_name_search("Hugo")`
 `output_climo(...)` | outputs a .csv file using the `csv` package of 1-year incremented climatological periods. This csv file can then be opened in a spreadsheet program. To compare or rank, the spreadsheet GUI layout is much easier to use especially due to instant sorting and filtering. This accepts a positional keyword argument (`climatology=30`). | `atl.output_climo(15)`
 `output_seasons_csv(...)` | Similar to the above, but for seasons. It takes no arguments. In other words, it would be redundant to run it multiple times, because as the `hurdat2parser` package doesn't natively allow modification of the data, it would just output the same data over and over. The only exception would be when the Hurdat2 database is updated by the NHC. With this in mind, it will automatically write-over the csv if it already exists (file-name is auto-generated within the method). | `atl.output_seasons_csv()`
 `output_storms_csv(...)` | Similar to above, but for individual storms. | `atl.output_storms_csv()`
+`climograph()` | displays a graph of the climatological tendency of a variable over multiple seasons (see docstring for a how-to) | `atl.climograph("ACE", 10, 1, year1=1967)`
 `coord_contains(...)` | Takes 3 tupled lat-lon coordinates. The purpose is to inquire whether the first arg (the test coordinate) is contained within a bounding box formed by the other two coordinates passed (returns a `bool`. This is generally just accessed via the ranking methods | `atl.coord_contains(`<br />&nbsp;&nbsp;&nbsp;&nbsp;`[30.4,-85.0]`,<br />&nbsp;&nbsp;&nbsp;&nbsp;`[31.5, 86.0],`<br />&nbsp;&nbsp;&nbsp;&nbsp;`[29.0, 84.0]`<br />`) -> True`
-`BASIN_DICT` | A dictionary containing abbreviations (keys) and definitions (values) of various basins around the world that hurricane data is kept. This is referenced via the `basin()` method. The data used to form this object came from IBTrACS | `<Hurdat2>.BASIN_DICT`
-`basin(season=None)` | Interprets and returns a readable string identifying the TC basin based on the storms within the record. This allows support of dynamically-created singular OR multiple Hurdat2 datasets OR individual seasons (if a `Season` object is passed to the method). | `atl.basin -> "North Atlantic Basin"
+`BASIN_DICT` | A dictionary containing abbreviations (keys) and definitions (values) of various basins around the world that hurricane data is kept. This is referenced via the `basin()` method. The data used to form this object came from IBTrACS | `atl.BASIN_DICT`
+`basin(season=None)` | Interprets and returns a readable string identifying the TC basin based on the storms within the record. This allows support of dynamically-created singular OR multiple Hurdat2 datasets OR individual seasons (if a `Season` object is passed to the method). The data used to form this property came from IBTrACS | `atl.basin() -> "North Atlantic Basin"
 `record_range` | Returns a tuple of the beginning year and end year of the Hurdat2 record | `atl.record_range -> (1851, 2020)`
 
 [&#8679; back to Methods &amp; Attributes](#methods-and-attributes)
 
 #### Shared Methods and Attributes for `Season` and `TropicalCyclone`
 
 Attributes | Description | Examples
@@ -118,97 +211,132 @@
 `landfalls`<br /> | \*SEE [DISCLAIMER FOR LANDFALL INFO](#landfall-data)\* Sum of all landfalls (remember, a storm can make multiple landfalls). `<Season>.landfalls` is also an unfiltered aggregate of its storms landfalls. At the seasonal level, you'd probably be more interested in the attribute `landfall_TC` (see following section) | `atl[1960]["doNnA"].landfalls`
 `landfall_<STATUS>`<br />*\-can be TC, TD, TS, HU, or MHU* | `Season`: qty of TC's that made landfall as the inquired status; `TropicalCyclone`: `bool` indicating if the storm made landfall while the inquired status<br />*\-CAUTION: These attrs are exclusive of landfalls made while of stronger designation\-* | `atl[1996].landfall_TS -> 2`<br />`atl[2011]["I"].landfall_HU -> True`
 `<STATUS>reach`<br />*\-can be TC, TD, TS, HU, or MHU* | `Season`: qty of TC's that reached <u>at least</u> the inquired status; `TropicalCyclone`: `bool` indicating if the storm ever was designated as the inquired status | `atl[2010].HUreach -> 12`<br />`atl[1991]["danny"].HUreach -> False`
 `ACE`, `HDP`, or `MHDP` | Returns the specified Energy Index reading associated with the season or storm. Note that the MHDP is one you likely won't see elsewhere. It's formula is the same as ACE and HDP but for major-hurricanes only | `atl[1966].HDP`
 `track_distance` | The calculated distance (in nmi) for the entire track of the storm (or aggregate of the season), regardless of status | `atl[1954]["hazel"].track_distance`
 `track_distance_<STATUS>`<br>*\-can be TC, TD, TS, HU, or MHU* | The distance traversed while storm(s) was(were) <u>at least</u> the status designation | `atl[1961].track_distance_MHU`
 `cat45reach`<br>`cat5reach` | For `Season` objects, returns the quantity of storms that reached category 4+ status or category 5 status (respectively)<br>For `TropicalCyclone` objects, returns a `bool`, indicating if the TC ever achieved cat 4+ or 5 status (respectively) | `atl[2020].cat45reach -> 5`<br>`atl[2020].cat5reach -> 0`<br>`atl[2020]["Iota"].cat5reach -> False`
-`maxwind_mslp`<br>`minmslp_wind` | Returns the MSLP (wind) occurring at the time of peak-winds (minimum MSLP) respectively. These attributes were included because peak winds and minimum MSLP do not necessarily occur at the same time. | `atl[2015]["joaquin"].maxwind_mslp -> 934`<br>`atl[2015]["joaquin"].minmslp_wind -> 120`<br>\* This example was given as Joaquin's peak winds (135) were not observed at the time of Joaquin's minimum MSLP (931)
 `hurdat2()` | This method prints a hurdat2-formatted output of the storms's data, emulating the actual hurdat2 record from which it (the Season or Tropical Cyclone) was created | `atl[2005].hurdat2()`
+`duration` | Returns the length of the Season or life of the cyclone (Of note, the `TropicalCyclone` property disregards storm status) | `atl[2022].duration`
+`tc_entries` | Returns a list of `TCRecordEntry`'s from where a storm was designated as a tropical cyclone | `atl["_katrina"].tc_entries`
+`start_date` | The beginning moment of the Season or storm | `atl[1938].start_date`
+`start_ordinal` | The quantified day of the year of the beginning moment of the Season or storm | `atl[1938].start_ordinal`
+`end_date` | The ending date of the Season or storm | `atl[1954, 16].end_date`
+`end_ordinal` | The quantified day of the year of the ending date of the Season or storm | `atl[1954].end_ordinal`
 
 [&#8679; back to Methods &amp; Attributes](#methods-and-attributes)
 
 #### `Season` Only Methods and Attributes
 Attribute | Description | Example
 :---: | :---: | :---:
 `output_shp_segmented()` | Generates a shapefile including each segment from each tropical-cyclone from a given season; each individual segment from each individual storm will be represented | `atl[1932].output_shp_segmented()`
 `output_geojson_segmented()` | Generates a geojson including each segment from each tropical-cyclone from a given season; each individual segment from each individual storm will be representeds | `atl[2003].output_geojson_segmented()`
 `tracks` | Returns the quantity of tropical cyclones from a season | `atl[1995].tracks`
 `<STATUS>only`<br />*\-can be TD, TS, or HU* | Returns the quantity of TC's from a season that made were given the inquired designation, but never strengthened beyond it. `HUonly` implies Category 1 and 2 storms only. To inquire about `MHU`, use the `MHUreach` attr | `atl[1950].TDonly`<br />`atl[2017].HUonly`
-`stats()` | prints a report filled with statistics and ranks for the season, optionally compared with a subset of seasons and/or partial seasons. For `TropicalCyclones`, this is a mirror-method of `.info()` | `atl[2020].stats()`<br>`atl[2005].stats(thru=(9,30))`<br>`atl[1989]["hugo"].stats()
+`stats()` | prints a report filled with statistics and ranks for the season, optionally compared with a subset of seasons and/or partial seasons. Though it technically exists as a  `TropicalCyclone` method, its iteration is a mirror-method of `.info()` | `atl[2020].stats()`<br>`atl[2005].stats(thru=(9,30))`
 
 [&#8679; back to Methods &amp; Attributes](#methods-and-attributes)
 
 #### `TropicalCyclone` Only Methods and Attributes
 | Attribute | Description | Example
 :---: | :---: | :---:
-`coord_list()` | Prints a report with entry dates and the associated Latitude and Longitude | `atl[2005]["rita"].coord_list()`
-`gps` | Returns a `list` of tupled latitude and Longitude coordinates | `atl[1998]["MITCH"].coord_list()`
+`gps` | Returns a `list` of tupled latitude and Longitude coordinates | `atl[1998]["MITCH"].gps`
+`maxwind` | Returns the highest maximum sustained wind-speed observed in the tropical cyclone | `atl["_katrina"].maxwind`
 `minmslp` | Returns the lowest recorded pressure of the TC | `atl[1955][10].minmslp`
+`maxwind_mslp`<br>`minmslp_wind` | Returns the MSLP (wind) occurring at the time of peak-winds (minimum MSLP) respectively. These attributes were included because peak winds and minimum MSLP do not necessarily occur at the same time. | `atl[2015]["joaquin"].maxwind_mslp -> 934`<br>`atl[2015]["joaquin"].minmslp_wind -> 120`<br>\* This example was given as Joaquin's peak winds (135) were not observed at the time of Joaquin's minimum MSLP (931)
 `<EI>_per_nmi`<br />*\-can be ACE, HDP, or MHDP* | Returns the inquired energy index divided by the track distance covered while the energy index was being contributed to (`ACE` &rarr; `track_distance_TS` or `HDP` &rarr; `track_distance_HU` as examples). WARNING! These attributes do not have any kind of threshold controls, so storms which were short-lived can have high values | `atl[1964][10].HDP_per_nmi`<br />`atl[2016]["matthew"].ACE_per_nmi`
 `<EI>_perc_ACE` &rarr; *\-can be HDP or MHDP*<br />`HDP_perc_MHDP` | Simply the storm's HDP or MHDP divided by ACE or the MHDP divided by the HDP. Look at this as the <u>percentage</u> (as a float between 0 and 1) of the storm's ACE or HDP that was contributed to while a Hurricane or Major Hurricane, respectively | `atl[2017]["IRMA"].HDP_perc_ACE`
 `track_<EI1>_perc_<EI2>`<br />*\-&lt;EI1&gt; can be TS, HU, or MHU*<br />*\-&lt;EI2&gt; can be TC, TS, HU, or MHU* | Returns the the storm's &lt;EI2&gt; track_distance divided by the track distance while of status &lt;EI1&gt;. &lt;EI1&gt; must be of higher hierarchal status than &lt;EI2&gt; | `atl[2005][25].track_HU_perc_TC`<br />`atl[2003]["Fabian"].track_MHU_perc_TS`
 `track_map()` | Generates a map of the storm's track using `matplotlib`. Check the docstring for ways to modify the output to your liking. | `atl["_katrina"].track_map()`
 `perc_ACE`<br>`perc_HDP`<br>`perc_MHDP` | Return the percentage (in decimal form) of the contribution of the storm's ACE, HDP, or MHDP value to the season's value | `atl["_matthew"].perc_MHDP
-`info()` | Prints basic stats for the tropical cyclone | `atl[1989]["hugo"].info()`
+`info()` | Prints basic stats for the tropical cyclone | `atl[2005][12].info()`
+`ACE_no_landfall` | Returns the ACE of the storm prior to any landfall made | `atl["_ivan"].ACE_no_landfall
+`duration_<SUFFIX>`<br />*\*&lt;SUFFIX&gt; can be TC, TS, HU, MHU* | Returns the aggregated length in days that the cyclone spent as on of the given statuses. These do account for storm status loss and possible reaquisition | `atl["_irma"].duration_MHU`
 
 [&#8679; back to Methods &amp; Attributes](#methods-and-attributes)
 
 #### `TCRecordEntry` Attributes
 
-- As mentioned earlier, there's generally no need to access`TCRecordEntry` objects directly. Only the most-common attributes will be referenced in this document. A comprehensive list is available via `help`
+- Only the most-common attributes will be referenced in this document. A comprehensive list is available via `help`
 
 | Attribute | Description
 :---: | :---:
 `entrytime` | A `datetime.datetime` object of the entry's timestamp
 `status` | The designated 2-letter abbreviation representing the storm's status
 `location`<br />`location_rev` | A tuple of the latitude/longitude coordinates; `location_rev` is reversed in order, a longitude/latitude tuple; seemingly favored for GIS use.
 `wind` | The maximum-sustained winds at the time of entry-recording
 `mslp` | The Mean Sea-Level Pressure (in hPa or mb) at the time of entry-recording
 `hurdat2()` | Returns a reassembled Hurdat2-formatted string, identical to the one parsed to create the entry
-`wind_radii` | The Radius of Maximum Winds. *As of the May 2022 release of the Hurdat2 database, this is a new variable and the availability of it belongs solely to the 2021 Hurricane season (for now).*
+`maxwind_radius` | The Radius of Maximum Winds. Currently, it is only available for storms since 2021, and is assumed that in subsequent releases, this variable will continue to be updated. It is unknown if this data for previous seasons will (or can) be back-filled.
+`avg_wind_extent_<SUFFIX>`<br/>Suffix can be `TS`, `TS50`, or `HU` | The statistical mean of the reported wind-extents (quadrants). Wind extents are only available for storms since 2004 
+`areal_extent_<SUFFIX>`<br/>Suffix can be `TS`, `TS50`, or `HU` | The calculated area covered by the extent of winds of specified strengths (of note, wind extents are only available for storms since 2004)
+`track_distance`<br/>`track_distance_<SUFFIX>`<br/>Suffix can be `TC`, `TS`, `HU`, or `MHU` | returns the distance tracked by the system from its genesist to the point of the entry. The variables with suffixes do account for status in their calculations
+`previous_entry`<br/>`next_entry` | Returns the entry prior-to or after the `TCRecordEntry` that it is called from
+`direction()` | Returns the heading in degrees that the storm is going. A readable cardinal direction can be returned if `True` is passed to the method
+`speed` | The average speed between the previous entry and this one in nm/h<br/>Of Note, remember that the `Hurdat2` spatial resolution is 0.1 degrees latitude/longitude. So some appreciable error may be present
 
 [&#8679; back to Methods &amp; Attributes](#methods-and-attributes)<br />
 [&#8679; back to Contents](#contents)
 
 ## Landfall Data
 
 An important point to keep in mind when viewing data and ranking, Hurdat2's landfall data is incomplete. It is progressively being updated in conjunction with the yearly release of the dataset. Please see the documentation  [Hurdat2 Format Guide](https://www.nhc.noaa.gov/data/hurdat/hurdat2-format-atl-1851-2021.pdf) for more detail on currently-available landfall data temporal scope.
 
 [&#8679; back to Contents](#contents)
 
+## Access to Future Methods
+
+In `_future.py`, I have some stuff that I've started to develop but not ready/sure to release. The methods are functional though. The quickest way of accessing it is:
+
+```python
+>>> import hurdat2parser._future as future
+```
+
+Valid classes reflect those of the main `hurdat2parser` object, namely `future.Hurdat2`, `future.Season`, `future.TropicalCyclone`, or `future.TCRecordEntry`. They'll be empty if I don't have anything I'm currently developing for that respective class/object. You can see what methods I have available by running `dir()` on the class.
+
+When calling, you will need to manually pass a valid object (a substitute for `self`). For example:
+```python
+>>> future.Season.track_map(atl[1984])
+```
+
+[&#8679; back to Contents](#contents)
+
 ## Roadmap
 
+- [ ] Include more `Season.duration`-related properties based on status
 - [ ] Speed-up `<Season>.stats()` report; because it employs `rank_seasons_thru`, and since that is quite snappy, I think the `stats()` method should be quick too. I'll investigate.
-- [ ] Include a `track_map()` method for `Season`
-- [ ] Include legends for `<TropicalCyclone>.track_map()`
+- [ ] Develop matplotlib-based graphs located in `_future`
 - [ ] Comparison methods to directly compare one season to another or specific storms to another.
-- [ ] Formulate a `stats()` method for `TropicalCyclone`s (to eventually replace their `info` method); including ranking/comparing to storms across the record or a subset of seasons, including a `rank_storms_thru()` companion method for `Hurdat2` objects.
+- [ ] Revamp `hurdat2()` method of `TropicalCyclone` and `Season` objects to optionally return a string instead of merely printing to console
+- [ ] Formulate a `stats()` method for `TropicalCyclone`s (to eventually replace their `info` method); including ranking/comparing to storms across the record or a subset of seasons (right now, this method is just a wrapper for the `info()` method.
 - [ ] Track distance percentage of season total for `TropicalCyclone`s
 - [ ] Maybe simpler rank methods so values sought for ranking will guarantee to show
-- [X] Deprecate `<Season>.info()` method
-- [x] Inclusion of `matplotlib` methods
+- [ ] add maps files for Pacific-centric storms
+- [ ] investigate adding a minmslp_entry or maxwind_entry property for TropicalCyclone objects. It is acknowledged though that multiple entries can have the same minimum mslp or max wind.
+- [ ] a `genesis` property, returning the first entry from a `TropicalCyclone` earning the TC designation. Not sure the feasability of this. I'll think about it.
+- [x] Include legends for `<TropicalCyclone>.track_map()`
+- [x] Account for absent season starts when using stats thru certain time
 
 [&#8679; back to Contents](#contents)
 
 ## Credits
 
-- Hurdat Reference: `Landsea, C. W. and J. L. Franklin, 2013: Atlantic Hurricane Database Uncertainty and Presentation of a New Database Format. Mon. Wea. Rev., 141, 3576-3592.`
+- HURDAT Reference: `Landsea, C. W. and J. L. Franklin, 2013: Atlantic Hurricane Database Uncertainty and Presentation of a New Database Format. Mon. Wea. Rev., 141, 3576-3592.`
 - [Haversine Formula (via Wikipedia)](https://en.wikipedia.org/wiki/Haversine_formula)
 - Bell, et. al. Climate Assessment for 1999. *Bulletin of the American Meteorological Society.* Vol 81, No. 6. June 2000. S19.
 - <span>G. Bell, M. Chelliah.</span> *Journal of Climate.* Vol. 19, Issue 4. pg 593. 15 February 2006.
 - [Hurdat2 Format Guide (PDF)](https://www.nhc.noaa.gov/data/hurdat/hurdat2-format-atl-1851-2021.pdf)
 - [Natural Earth](https://www.naturalearthdata.com/) GIS Data (data extracted there-from to display maps)
 
 [&#8679; back to Contents](#contents)
 
 ## Copyright
 
 **Author**: Kyle S. Gentry<br />
-Copyright &copy; 2019-2022, Kyle Gentry (KyleSGentry@outlook.com)<br />
+Copyright &copy; 2019-2023, Kyle Gentry (KyleSGentry@outlook.com)<br />
 **License**: MIT<br />
 **GitHub**: [https://github.com/ksgwxfan/hurdat2parser](https://github.com/ksgwxfan/hurdat2parser)<br />
 **Author's Webpages**:
  - [https://ksgwxfan.github.io/](https://ksgwxfan.github.io/)<br />
  - [http://echotops.blogspot.com/](http://echotops.blogspot.com/)
 
 [&#8679; back to Contents](#contents)
```

### Comparing `hurdat2parser-2.11/hurdat2parser/__init__.py` & `hurdat2parser-2.2/hurdat2parser/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,80 +1,208 @@
-"""hurdat2parser v2.11
+"""hurdat2parser v2.2
 
 https://github.com/ksgwxfan/hurdat2parser
 
-hurdat2parser v2.x is an object-oriented approach to viewing tropical cyclone
-data that is contained in a widely-used and updated dataset, HURDAT2
-(https://www.nhc.noaa.gov/data/#hurdat). The purpose of this module is to
-provide a quick way to investigate HURDAT2 data. Its aim is to make it easier
-to access historical hurricane data.
+hurdat2parser v2.x is provides a convenient access to interpret and work with
+tropical cyclone data that is contained in a widely-used and updated dataset,
+HURDAT2 (https://www.nhc.noaa.gov/data/#hurdat). The purpose of this module is to
+provide a quick way to investigate HURDAT2 data. It includes methods for
+retrieving, inspecting, ranking, or even exporting data for seasons, individual
+storms, or climatological eras.
 
 To get started:
 1) Install: >>> pip install hurdat2parser
-2) Download HURDAT2 Data: https://www.nhc.noaa.gov/data/#hurdat
+2a) Download HURDAT2 Data: https://www.nhc.noaa.gov/data/#hurdat
+    OR See example call below to have the program attempt to download it for you
 3) In python, import and invoke call using the hurdat2 file you downloaded (the
     following is just an example):
 
     >>> import hurdat2parser
     >>> atl = hurdat2parser.Hurdat2("path_to_hurdat2.txt")
 
-hurdat2parser, Copyright (c) 2019-2022, Kyle Gentry (KyleSGentry@outlook.com)
+    OR ATTEMPT TO RETRIEVE FROM ONLINE
+    >>> atl = hurdat2parser.Hurdat2(basin="atl")
+    # Use "pac" to get the NE/CEN Pacific version
+
+hurdat2parser, Copyright (c) 2019-2023, Kyle Gentry (KyleSGentry@outlook.com)
 License: MIT
 ksgwxfan.github.io
 echotops.blogspot.com
 """
 
 import calendar
 import difflib
 import math
 import re
+import urllib.request
 import itertools
 import datetime
+import os
 import collections
 
 from . import _aliases, _calculations, _reports
 
 class Hurdat2(_aliases.Hurdat2Aliases, _calculations.Hurdat2Calculations, _reports.Hurdat2Reports):
 
     BASIN_DICT = dict(
-            AL = "North Atlantic",
-            NA = "North Atlantic",
-            SL = "South Atlantic",
-            SA = "South Atlantic",
-            EP = "East Pacific",
-            CP = "Central Pacific",
-            WP = "West Pacific",
-            SH = "Southern Hemisphere",
-            IO = "North Indian",
-            NI = "North Indian",
-            SI = "South Indian",
-            SP = "South Pacific",
-            AS = "Arabian Sea",
-            BB = "Bay of Bengal",
-        )
+        AL = "North Atlantic",
+        NA = "North Atlantic",
+        SL = "South Atlantic",
+        SA = "South Atlantic",
+        EP = "East Pacific",
+        CP = "Central Pacific",
+        WP = "West Pacific",
+        SH = "Southern Hemisphere",
+        IO = "North Indian",
+        NI = "North Indian",
+        SI = "South Indian",
+        SP = "South Pacific",
+        AS = "Arabian Sea",
+        BB = "Bay of Bengal",
+    )
 
-    def __init__(self, hurdat2file):
+    def __init__(self, *hurdat2file_list, **kw):
         """Initializes a new Hurdat2 object.
         
         Arguments:
-            hurdat2file (str): file-path of the hurdat2 record (a text file)
+            *hurdat2file_list: the local file-paths (or URLs) of the hurdat2
+            record(s)
+
+        Keyword Arguments:
+            basin (None): If you want to try to retrieve the latest hurdat2
+                file from the NHC to ingest, let it know which basin you want
+                to download. Acceptable strings to use would be "atl", "al", or
+                "atlantic" for the North Atlantic hurdat2. For the North-East/
+                Central Pacific, "pac", "nepac", and "pacific" are recognized.
+                Of note, the Atlantic hurdat2 file is around 6MB.
+            urlcheck (False): If True, urls are accepted. This enables the
+                download of a remote version of a Hurdat2 dataset. The url
+                string is passed as if a local file and will eventually be
+                attempted to be downloaded.
+
+        Example call:
+            atl = hurdat2parser.Hurdat2("atlantic_hurdat2.txt")
+                * Attempts to load a local file named "hurdat2_file.txt"
+            atl = hurdat2parser.Hurdat2(basin="pac")
+                * Attempts to download the latest NE/CEN Pacific hurdat2 file
+            atl = hurdat2parser.Hurdat2("https://somewebsite.zxcv/hd2.txt", urlcheck=True)
+                * Attempts to download inspect the passed-string as a url and
+                tries to download
+            
         """
         self._tc = {}        # Dictionary containing all hurdat2 storm data
         self._season = {}    # Dictionary containing all relevant season data
-        self._rank = {"tc":{}, "season":{}}
-        # used to prevent multiple loads of the same file to the same object
-        self._filesappended = []
-        self._build_tc_dictionary(hurdat2file)  # Call to build/analyze the hurdat2 file
+
+        # Validity checking -------------------------------
+        # no local path given and Non-existent or invalid basin
+        if len(hurdat2file_list) == 0 \
+        and (kw.get("basin") is None or type(kw.get("basin")) != str):
+            raise ValueError(
+                "No path to a local hurdat2 file given and no valid basin "
+                "indicated to attempt online retrieval."
+            )
+        # No online, but invalid local paths
+        if kw.get("basin") is None \
+        and len(hurdat2file_list) != 0 \
+        and all(os.path.exists(fi) == False for fi in hurdat2file_list) \
+        and kw.get("urlcheck", False) is False:
+            raise FileNotFoundError(
+                "{} {} not {}valid file path{}.".format(
+                    ", ".join([
+                        "'{}'".format(fi) for fi in hurdat2file_list
+                    ]),
+                    "is" if len(hurdat2file_list) == 1 else "are",
+                    "a " if len(hurdat2file_list) == 1 else "",
+                    "" if len(hurdat2file_list) == 1 else "s",
+                )
+            )
+        # -------------------------------------------------------
+
+        # Download from online
+        if type(kw.get("basin")) == str \
+        and kw.get("basin").lower() in [
+            "al", "atl", "atlantic", "pac", "nepac", "pacific"
+        ]:
+            # determines which dataset will be downloaded
+            basin_prefix = "nepac-" \
+                if kw.get("basin").lower() in ["pac", "nepac", "pacific"] \
+                else ""
+
+            # https://www.nhc.noaa.gov/data/hurdat/hurdat2-1851-2021-100522.txt
+            with urllib.request.urlopen("https://www.nhc.noaa.gov/data/hurdat", timeout=5) as u:
+                _pgdata = u.read().decode()
+
+            _hd2list = re.findall(
+                "hurdat2-{}".format(basin_prefix) + r"\d{4}-\d{4}.*\.txt",
+                _pgdata,
+                flags=re.I
+            )
+            hd2url = "https://www.nhc.noaa.gov/data/hurdat/" \
+                + sorted(_hd2list, reverse=True)[0]
+
+            # read in the url
+            try:
+                with urllib.request.urlopen(hd2url, timeout=5) as u:
+                    hd2fileobj = u.read().decode()
+                # print("* Downloaded '{}'".format(hd2url))
+            except:
+                if len(hurdat2file_list) == 0:
+                    raise
+            self._build_tc_dictionary(hd2fileobj, False)
+            # print("* Download and read-in of `{}` successful!".format(
+                # hd2url
+            # ))
+        # invalid basin listed
+        elif type(kw.get("basin")) == str:
+            if len(hurdat2file_list) == 0:
+                raise ValueError(
+                    "'{}' is an unrecognized basin. ".format(kw.get("basin")) \
+                  + "Please use something like 'atl' or 'pac' to direct the " \
+                  + "module to retrieve the deisred hurdat2 file from online."
+                )
+            else:
+                print(
+                    "* Skipping basin download. " \
+                  + "'{}' is an unrecognized basin. ".format(kw.get("basin")) \
+                  + "Please use something like 'atl' or 'pac' to direct the " \
+                  + "module to retrieve the deisred hurdat2 file from online."
+                )
+
+        for hd2file in hurdat2file_list:
+            if os.path.exists(hd2file):
+                self._build_tc_dictionary(hd2file)  # Call to build/analyze the hurdat2 file
+                # print("* Read-in of `{}` successful!".format(hd2file))
+            # download a given url
+            elif kw.get("urlcheck"):
+                try:
+                    with urllib.request.urlopen(hd2file, timeout=5) as u:
+                        hd2fileobj = u.read().decode()
+                    # print("* Downloaded '{}'".format(hd2file))
+                except Exception as e:
+                    print("* Skipping '{}' due to {}".format(hd2file, e))
+                    hd2fileobj = None
+                if hd2fileobj is not None:
+                    self._build_tc_dictionary(hd2fileobj, False)
+                    # print("* Download and read-in of `{}` successful!".format(
+                        # hd2file
+                    # ))
+            else:
+                print("* Skipping `{}` because that path doesn't exist!".format(
+                    hd2file
+                ))
+
+        if len(self) == 0:
+            raise ValueError("No storm data ingested!")
 
     def __repr__(self):
         return "<{} object - {}: {}-{} - at 0x{}>".format(
             re.search(r"'(.*)'", str(type(self)))[1],
             self.basin(),
             *self.record_range,
-            str(id(self)).upper().zfill(16)
+            hex(id(self))[2:].upper().zfill(16)
         )
 
     def __len__(self):
         """Returns the number of tracked systems in the Hurdat2 record"""
         return len(self.tc)
 
     def __str__(self):
@@ -98,247 +226,88 @@
             tuple or list: returns the Season(1), TropicalCyclone(2), or
                 TCRecordEntry(3) desired, depending on length of tuple passed.
             int: grabs the _season object matching the year passed.
             str: inspects the string and returns either a storm object, a
                 season object, or a call to the name-search function
         """
         # multi-season info
-        if type(s) is slice:
+        if type(s) == slice:
             st = s.start
             en = s.stop-1
             return self.multi_season_info(st, en)
         # use items of an iterable as season, tcnumber, and entry index
         elif type(s) in [tuple, list]:
             if len(s) == 1:
                 return self[s[0]]
             elif len(s) >= 2:
                 return self[s[0]][s[1:]]
         # Season passed as int
-        elif type(s) is int:
+        elif type(s) == int:
             return self.season[s]
         # String based
         elif type(s) == str:
             # ATCFID Request
-            if re.search(r"^[A-Z]{2}[0-9]{6}.*", str(s), flags=re.I):
+            if re.search(r"^[A-Z]{2}[0-9]{6}.*", s, flags=re.I):
                 return self.tc[s.upper()[:8]]
             # Season Request
             elif s.isnumeric():
                 return self.season[int(s[:4])]
             # Name Search implied (will return the last storm so-named)
             else:
-                return self.storm_name_search(s, False, True if "_" in s else False)
+                return self.storm_name_search(s, False, True if "_" in s or "-" in s else False)
         # try handling all other types by converting to str then search by name
         else:
             return self.storm_name_search(str(s), False)
 
-    def _build_tc_dictionary(self, hurdat2file):
+    def _build_tc_dictionary(self, hurdat2file, path=True):
         """Populate the Hurdat2 object with data from a hurdat2 file.
 
         Arguments:
-            hurdat2file: the file-path of the hurdat2 file
-        """
-        if hurdat2file in self.filesappended:
-            return print("OOPS! That file has already been read-in to this Hurdat2 object.")
-        self.filesappended.append(hurdat2file)
-        with open(hurdat2file) as h:
-            # for line in h.readlines():
-                # lineparsed = [each.strip() for each in line.strip("\n").split(",")]
-            for line in h.read().splitlines():
-                lineparsed = re.split(r", *", re.sub(r", *$", "", line))
-                # above definition will leave a trailing comma at the end of e
-                lineparsed[-1] = lineparsed[-1].strip(",")
-                # New Storm
-                if re.search(r"^[A-Z]{2}\d{6}",lineparsed[0]):
-                    atcfid = lineparsed[0]
-                    tcyr = int(atcfid[4:])
-                    # Create Season
-                    if tcyr not in self.season:
-                        self.season[tcyr] = Season(tcyr, self)
-                    # Create TropicalCyclone
-                    self.tc[atcfid] = TropicalCyclone(
-                        atcfid,
-                        lineparsed[1],
-                        self.season[tcyr],
-                        self
-                    )
-                    # Add storm to that particular season
-                    self.season[tcyr].tc[atcfid] = self.tc[atcfid]
-                # TCRecordEntry for storm indicated
-                else:
-                    self.tc[atcfid].entry.append(
-                        TCRecordEntry(
-                            lineparsed.copy(),
-                            self.tc[atcfid],
-                            self.season[tcyr],
-                            self
-                        )
-                    )
+            hurdat2file: the file-path (or string version) of the hurdat2 file
 
-    def multi_season_info(self, year1=None, year2=None):
-        """Grab a chunk of multi-season data and report on that climate era.
-        This method can be viewed as a climatological era info method.
-        
         Default Arguments:
-            year1 (None): The start year
-            year2 (None): The end year
-        """
-
-        year1 = self.record_range[0] if year1 is None \
-            or year1 < self.record_range[0] else year1
-        year2 = self.record_range[1] if year2 is None \
-            or year2 > self.record_range[1] else year2
-        # ---------------------
-
-        # for yr1, yr2 in [(y, y+climatology-1) \
-                # for y in range(1801, year2, increment) \
-                # if year1 <= y <= year2 \
-                # and year1 <= y+climatology-1 <= year2]:
-            # climo[yr1, yr2] = Era(
-                # (yr1, yr2),
-                # sum(self.season[s].tracks for s in range(yr1, yr2+1)),
-                # sum(self.season[s].landfalls for s in range(yr1, yr2+1)),
-                # sum(self.season[s].landfall_TC for s in range(yr1, yr2+1)),
-                # sum(self.season[s].landfall_TD for s in range(yr1, yr2+1)),
-                # sum(self.season[s].landfall_TS for s in range(yr1, yr2+1)),
-                # sum(self.season[s].landfall_HU for s in range(yr1, yr2+1)),
-                # sum(self.season[s].landfall_MHU for s in range(yr1, yr2+1)),
-                # sum(self.season[s].TSreach for s in range(yr1, yr2+1)),
-                # sum(self.season[s].TSonly for s in range(yr1, yr2+1)),
-                # sum(self.season[s].HUreach for s in range(yr1, yr2+1)),
-                # sum(self.season[s].HUonly for s in range(yr1, yr2+1)),
-                # sum(self.season[s].MHUreach for s in range(yr1, yr2+1)),
-                # sum(self.season[s].cat45reach for s in range(yr1, yr2+1)),
-                # sum(self.season[s].cat5reach for s in range(yr1, yr2+1)),
-                # sum(self.season[s].track_distance for s in range(yr1, yr2+1)),
-                # sum(self.season[s].track_distance_TC for s in range(yr1, yr2+1)),
-                # sum(self.season[s].track_distance_TS for s in range(yr1, yr2+1)),
-                # sum(self.season[s].track_distance_HU for s in range(yr1, yr2+1)),
-                # sum(self.season[s].track_distance_MHU for s in range(yr1, yr2+1)),
-                # sum(self.season[s].ACE for s in range(yr1, yr2+1)),
-                # sum(self.season[s].HDP for s in range(yr1, yr2+1)),
-                # sum(self.season[s].MHDP for s in range(yr1, yr2+1))
-            # )
-        # # If this method was called by the output_climo method...
-        # if "op" in climoparam:
-            # return climo
-
-        # # List of tropical-cyclones sorted by stattr
-        # sorted_climo = sorted(
-            # [era for era in climo.values()],
-            # key=lambda era: getattr(era, stattr),
-            # reverse = descending
-        # )
-        # # Values sorted
-        # ranks = sorted(
-            # set([
-                # getattr(era, stattr) for era in sorted_climo \
-                    # if descending is False \
-                    # or getattr(era, stattr) > 0
-            # ]),
-            # reverse = descending
-        # )[:quantity]
-        # --------------------------------
-        class Era(object):
-            def __init__(self, **kw):
-                self.__dict__.update(**kw)
-
-        yrrange = range(year1, year2+1)
-        clmt = Era(
-            era = (year1, year2),
-            tracks = sum(self.season[s].tracks for s in yrrange),
-            landfalls = sum(self.season[s].landfalls for s in yrrange),
-            landfall_TC = sum(self.season[s].landfall_TC for s in yrrange),
-            landfall_TD = sum(self.season[s].landfall_TD for s in yrrange),
-            landfall_TS = sum(self.season[s].landfall_TS for s in yrrange),
-            landfall_HU = sum(self.season[s].landfall_HU for s in yrrange),
-            landfall_MHU = sum(self.season[s].landfall_MHU for s in yrrange),
-            TSreach = sum(self.season[s].TSreach for s in yrrange),
-            TSonly = sum(self.season[s].TSonly for s in yrrange),
-            HUreach = sum(self.season[s].HUreach for s in yrrange),
-            HUonly = sum(self.season[s].HUonly for s in yrrange),
-            MHUreach = sum(self.season[s].MHUreach for s in yrrange),
-            cat45reach = sum(self.season[s].cat45reach for s in yrrange),
-            cat5reach = sum(self.season[s].cat5reach for s in yrrange),
-            track_distance = sum(self.season[s].track_distance for s in yrrange),
-            track_distance_TC = sum(self.season[s].track_distance_TC for s in yrrange),
-            track_distance_TS = sum(self.season[s].track_distance_TS for s in yrrange),
-            track_distance_HU = sum(self.season[s].track_distance_HU for s in yrrange),
-            track_distance_MHU = sum(self.season[s].track_distance_MHU for s in yrrange),
-            ACE = sum(self.season[s].ACE for s in yrrange),
-            HDP = sum(self.season[s].HDP for s in yrrange),
-            MHDP = sum(self.season[s].MHDP for s in yrrange)
-        )
+            path (True): this tells the method what kind object to expect. By
+                default, it will be considered a file-path. If False, it will
+                expect a stringified version of the database.
+        """
+        if path is True:
+            with open(hurdat2file) as h:
+                _hd2data = h.read().splitlines()
+        else:
+            _hd2data = hurdat2file.splitlines()
 
-        # Print Report
-        totalyrs = year2 - year1 + 1
-        print("")
-        print(" --------------------------------------------------------")
-        print(" Tropical Cyclone Season Stats, for {} to {}".format(year1, year2))
-        print(" --------------------------------------------------------")
-        print(" {:^56}".format(
-            "* Distances in nmi; * Energy Indices in 10**(-4) kt^2"
-        ))
-        print(" --------------------------------------------------------")
-        print(" Avg Track Qty (Total): {}/yr ({})".format(
-            round(clmt.tracks / totalyrs,1),
-            clmt.tracks
-        ))
-        print(" Avg TC Track Distance (Total): {}/yr ({})".format(
-            round(clmt.track_distance_TC / totalyrs,1),
-            round(clmt.track_distance_TC,1)
-        ))
-        print(" Avg TS Qty (Total): {}/yr ({})".format(
-            round(clmt.TSreach / totalyrs,1),
-            clmt.TSreach
-        ))
-        print("   -- Avg TS Track Distance (Total): {}/yr ({})".format(
-            round(clmt.track_distance_TS / totalyrs,1),
-            round(clmt.track_distance_TS,1)
-        ))
-        print("   -- Avg ACE (Total): {}/yr ({})".format(
-            round(clmt.ACE * 10**(-4) / totalyrs,1),
-            round(clmt.ACE * 10**(-4),1)
-        ))
-        print(" Avg HU Qty (Total): {}/yr ({})".format(
-            round(clmt.HUreach / totalyrs,1),
-            clmt.HUreach
-        ))
-        print("   -- Avg HU Track Distance (Total): {}/yr ({})".format(
-            round(clmt.track_distance_HU / totalyrs,1),
-            round(clmt.track_distance_HU,1)
-        ))
-        print("   -- Avg HDP (Total): {}/yr ({})".format(
-            round(clmt.HDP * 10**(-4) / totalyrs,1),
-            round(clmt.HDP * 10**(-4),1)
-        ))
-        print(" Avg MHU Qty (Total): {}/yr ({})".format(
-            round(clmt.MHUreach / totalyrs,1),
-            clmt.MHUreach
-        ))
-        print(" Avg Cat-4 and Cat-5 Qty (Total): {}/yr ({})".format(
-            round(clmt.cat45reach / totalyrs,1),
-            clmt.cat45reach
-        ))
-        print(" Avg Cat-5 Qty (Total): {}/yr ({})".format(
-            round(clmt.cat5reach / totalyrs,1),
-            clmt.cat5reach
-        ))
-        print("   -- Avg MHU Track Distance (Total): {}/yr ({})".format(
-            round(clmt.track_distance_MHU / totalyrs,1),
-            round(clmt.track_distance_MHU,1)
-        ))
-        print("   -- Avg MHDP (Total): {}/yr ({})".format(
-            round(clmt.MHDP * 10**(-4) / totalyrs,1),
-            round(clmt.MHDP * 10**(-4),1)
-        ))
-        print(" Avg Landfalling System Qty (Total): {}/yr ({})".format(
-            round(clmt.landfall_TC / totalyrs,1),
-            clmt.landfall_TC
-        ))
-        print("")
+        for line in _hd2data:
+            lineparsed = re.split(r", *", re.sub(r", *$", "", line))
+            # New Storm
+            if re.search(r"^[A-Z]{2}\d{6}",lineparsed[0]):
+                atcfid = lineparsed[0]
+                tcyr = int(atcfid[4:])
+                # Create Season
+                if tcyr not in self.season:
+                    self.season[tcyr] = Season(tcyr, self)
+                # Create TropicalCyclone
+                self.tc[atcfid] = TropicalCyclone(
+                    atcfid,
+                    lineparsed[1],
+                    self.season[tcyr],
+                    self
+                )
+                # Add storm to that particular season
+                self.season[tcyr].tc[atcfid] = self.tc[atcfid]
+            # TCRecordEntry for storm indicated
+            else:
+                self.tc[atcfid].entry.append(
+                    TCRecordEntry(
+                        lineparsed.copy(),
+                        line,
+                        self.tc[atcfid],
+                        self.season[tcyr],
+                        self
+                    )
+                )
 
     def storm_name_search(self, searchname, info=True, feeling_lucky=False):
         """Search the Hurdat2 object's records by storm name. Returns the
         matches info method or returns the matching object itself.
 
         Required Argument:
             searchname: the storm name to search
@@ -357,15 +326,15 @@
                 
         """
         searchname = searchname.upper()     # Capitalize the search term
 
         # Searching for a storm of a particular name; will return the most
         #   recent storm where a match was found in the name
         if feeling_lucky is True:
-            searchname = searchname.replace("_", "")
+            searchname = searchname.replace("_", "").replace("-", "")
             # 1st pass
             matchlist = [(TC, 1.0) for TC in self.tc.values() if searchname == TC.name]
 
             if len(matchlist) > 0:
                 return matchlist[-1][0]
             # 2nd pass
             else:
@@ -404,15 +373,17 @@
                             difflib.SequenceMatcher(
                                 None,
                                 searchname,
                                 TC.name
                             ).quick_ratio()
                         ) for TC in self.tc.values() if TC.name[0] == searchname[0]
                     ]
-                ), key=lambda tup: tup[1], reverse=True
+                ),
+                key=lambda tup: tup[1],
+                reverse=True
             )
         #3rd pass - if necessary; if no match found
         if len(matchlist) == 0:
             matchlist = sorted(
                 filter(
                     lambda tup: tup[1] >= 0.6,
                     [
@@ -474,30 +445,51 @@
         coordinates (lx).
         """
         if lx[0] <= testcoord[0] <= ux[0] and ux[1] <= testcoord[1] <= lx[1]:
             return True
         else:
             return False
 
+    def basin_abbr(self, season_obj=None):
+        """Returns a list of basin abbreviations used in the hurdat2 record.
+        
+        This is primarily of use to the .basin() method.
+        """
+        try:
+            return list(set([
+                tc.atcfid[:2]
+                for tc in (
+                    self.tc.values()
+                    if season_obj is None
+                    else season_obj.tc.values()
+                )
+            ]))
+        except:
+            return ["UNK"]
+
     def basin(self, season_obj=None):
+        """Returns a string containing the various oceanic basins represented in the hurdat2 database(s) being analyzed. As an example, the NHC releases a East/Central Pacific Hurdat2.
+
+        Keyword Argument:
+            season_obj (None): This is used to isolate a basin names from a particular season. It's possible in the aforementioned East/Central Pacific that cyclones occur in the east pacific but not central. So a report or inquired stats from a particular season wouldn't need to show data from the non-existent basin.
+        """
 
-        basin_id = list(set([
-            tc.atcfid[:2] for tc in (self.tc.values() if season_obj is None else season_obj.tc.values())
-        ]))
         basin_names = []
         try:
             basin_names = list(set([
-                self.BASIN_DICT[basin] for basin in basin_id
+                self.BASIN_DICT[basin]
+                for basin in self.basin_abbr(season_obj)
             ]))
         except:
             pass
-        # print(basin_id)
         if len(basin_names) > 0:
             return " / ".join(basin_names) \
-                + " Basin{}".format("s" if len(basin_id) > 1 else "")
+                + " Basin{}".format(
+                    "s" if len(self.basin_abbr(season_obj)) > 1 else ""
+                )
         else:
             return "Unknown Region"
 
     @property
     def record_range(self):
         """Returns a tuple containing the beginning and end seasons covered by
         the Hurdat2 object.
@@ -512,36 +504,57 @@
         self._hd2 = hd2obj
 
     def __repr__(self):
         return "<{} object - {} - {} - at 0x{}>".format(
             re.search(r"'(.*)'", str(type(self)))[1],
             self.year,
             self._hd2.basin(self),
-            str(id(self)).upper().zfill(16)
+            hex(id(self))[2:].upper().zfill(16)
         )
 
     def __len__(self):
         """Returns the number of tropical cyclones from a particular season."""
         return len(self.tc)
 
     def __getitem__(self, s):
         # Storm Number passed
-        if type(s) == int:
-            for atcfid, tc in self.tc.items():
+        if type(s) == int and s >= 0:
+            tcmatches = [
+                tc for atcfid, tc in self.tc.items()
                 if re.search(
                     r"[A-Z][A-Z]{:0>2}\d\d\d\d".format(s),
                     atcfid
-                ):
-                    return tc
-                
-            # return self.tc[
-                # list(self.tc.keys())[
-                    # (s-1) if s > 0 else s
-                # ]
-            # ]
+                )
+            ]
+            if len(tcmatches) == 0:
+                return list(self.tc.values())[s]
+            elif len(tcmatches) == 1:
+                return tcmatches[0]
+            else:
+                print("* Multiple matches found. Choose intended storm:")
+                print("------------------------------------------------")
+                for indx, tc in enumerate(tcmatches):
+                    print("{}. {} - '{}'".format(
+                        indx+1,
+                        tc.atcfid,
+                        tc.name
+                    ))
+                print("------------------------------------------------")
+                choice = input("  -- Enter selection ('c' to cancel): ")
+                while True:
+                    if choice.isnumeric() \
+                    and 0 < int(choice) <= len(tcmatches):
+                        return tcmatches[int(choice)-1]
+                    elif len(choice) > 0 and choice.lower()[0] == "c":
+                        raise KeyboardInterrupt
+                    else:
+                        choice = input("  -- Invalid selection. Try again: ")
+
+        elif type(s) == int and s < 0:
+            return list(self.tc.values())[s]
         # List/Tuple (storm number, tcrecord index)
         elif type(s) in [tuple, list]:
             if len(s) == 1:
                 return self[s[0]]
             else:
                 return self[s[0]][s[1]]
         elif type(s) == str:
@@ -551,15 +564,15 @@
             # Storm name / Starting first-letter
             else:
                 num_name = {tc.atcfid : tc.name for tc in self.tc.values()}
                 for atcfid, name in {tc.atcfid : tc.name for tc in self.tc.values()}.items():
                     if s.upper()[0] == name[0]:
                         return self.tc[atcfid]
 
-    def stats(self, year1=None, year2=None, start=None, thru=None, width=70, **kw):
+    def stats(self, year1=None, year2=None, start=None, thru=None, width=70, report_type=print, **kw):
         """Returns a report of a host of stats from the season and their ranks 
         relative to compared seasons. It also fully supports partial season
         stats (like rank_seasons_thru).
 
         * Of note, this can be quite slow especially when comparing full
         seasons to the full record.
 
@@ -567,14 +580,18 @@
             year1 (None): start year of the comparison.
             year2 (None): end year of the comparison.
             start (None): accepts a 2-member tuple representing month and day;
                 the start month and day for the comparison.
             thru (None): accepts a 2-member tuple representing month and day;
                 the end month and day for the comparison.
             width (70): used to control the width of the report
+            report_type (print): controls the format of the seasonal stats
+                requested. By default, it prints out to the console. if <<str>>
+                (no quotations needed), it returns a stringified version of the
+                stats
 
         Keyword Arguments:
             descending: bool used to determine sorting method of rank results 
                 (defaults to True)
 
         Examples:
             atl[1984].stats() :: Return stat-report for the 1984 season.
@@ -596,16 +613,18 @@
             year2 = self._hd2.record_range[1]
 
         # set bound on calendar dates for comparison
         if start is None:
             start = (1,1)
         if thru is None:
             thru = (12,31)
-        
-        return self._hd2._season_stats(
+        return getattr(
+            self._hd2,
+            "_season_stats" + ("_str" if report_type == str else "")
+        )(
             self.year,
             year1,
             year2,
             start,
             thru,
             width,
             descending=kw.get("descending", True)
@@ -648,33 +667,44 @@
         ))
         print(" {:<10} {:^8} {:<4} {:^4} {:^4}  {:^6}  {:^6}  {:^6}  {:^6}".format(
             "NAME","ATCFID","QTY","MSLP","WIND","(nmi)","ACE","HDP","MHDP"
         ))
         print(" {:-^10} {:-^8} {:-^4} {:-^4} {:-^4}  {:-^6}  {:-^6}  {:-^6}  {:-^6}".format(
             "","","","","","","","",""
         ))
-        for trop in self.tc:
+        for tcid, trop in self.tc.items():
             print(" {:<10} {:8} {:^4} {:>4} {:>4}  {:>6.1f}  {:^6}  {:^6}  {:^6}".format(
-                self.tc[trop].name.title(),
-                self.tc[trop].atcfid,
-                self.tc[trop].landfalls,
-                self.tc[trop].minmslp if self.tc[trop].minmslp != None else "N/A",
-                self.tc[trop].maxwind if self.tc[trop].maxwind > 0 else "N/A",
-                self.tc[trop].track_distance_TC,
-                "{:>6.3f}".format(self.tc[trop].ACE * math.pow(10,-4)) if self.tc[trop].ACE > 0 else "--",
-                "{:>6.3f}".format(self.tc[trop].HDP * math.pow(10,-4)) if self.tc[trop].HDP > 0 else "--",
-                "{:>6.3f}".format(self.tc[trop].MHDP * math.pow(10,-4)) if self.tc[trop].MHDP > 0 else "--"
+                trop.name.title(),
+                trop.atcfid,
+                trop.landfalls,
+                trop.minmslp if trop.minmslp != None else "N/A",
+                trop.maxwind if trop.maxwind > 0 else "N/A",
+                trop.track_distance_TC,
+                "{:>6.3f}".format(trop.ACE * math.pow(10,-4)) if trop.ACE > 0 else "--",
+                "{:>6.3f}".format(trop.HDP * math.pow(10,-4)) if trop.HDP > 0 else "--",
+                "{:>6.3f}".format(trop.MHDP * math.pow(10,-4)) if trop.MHDP > 0 else "--"
             ))
         print("")
 
     def hurdat2(self):
         """Prints a Hurdat2-formatted summary of the entire season."""
         for tc in self.tc.values():
             tc.hurdat2()
 
+    @property
+    def tc_entries(self):
+        """
+        Returns a temporally-ascending list of <<TCRecordEntry>>s of all
+        tropical cyclones occurring during the season.
+        """
+        return sorted([
+            en for tcid, TC in self.tc.items()
+            for en in TC.entry
+            if en.is_TC
+        ], key = lambda moment: moment.entrytime)
 
     @property
     def tracks(self):
         """Returns the total number of tropical cyclones from the season. It's
         the same as calling len(self). It's included for readability in other
         methods.
         """
@@ -812,31 +842,21 @@
         return len(self.entry)
 
     def __repr__(self):
         return "<{} object - {}:{} - at 0x{}>".format(
             re.search(r"'(.*)'", str(type(self)))[1],
             self.atcfid,
             self.name,
-            str(id(self)).upper().zfill(16)
+            hex(id(self))[2:].upper().zfill(16)
         )
 
     def __getitem__(self, indx):
-        return self.entry[indx]
-
-    def coord_list(self):
-        """Prints a report of entry-dates and the corresponding latitude and
-        longitude of the storm's center position.
-        """
-        print("DATE, LAT, LON")
-        for trk in self.entry:
-            print("{:%Y-%m-%d %H:%M},{},{}".format(
-                trk.entrytime,
-                trk.location[0],
-                trk.location[1]
-            ))
+        return self.entry[
+            int(indx) if type(indx) not in [list, tuple] else indx[0]
+        ]
 
     def stats(self):
         self.info()
 
     def info(self):
         """Prints a basic report of information on the tropical cyclone."""
         print("")
@@ -881,18 +901,15 @@
             ))
         if self.MHDP > 0:
             print("* MHDP: {:.3f} * 10^4 kts^2".format(
                 self.MHDP * math.pow(10,-4)
             ))
         print("* Started: {:%Y-%m-%d %H}Z".format(self.entry[0].entrytime))
         print("* Ended: {:%Y-%m-%d %H}Z".format(self.entry[-1].entrytime))
-        print("   -Total Track Time: {} days, {} hours".format(
-            math.floor(int((self.entry[-1].entrytime - self.entry[0].entrytime).total_seconds()) / 60 / 60 / 24),
-            math.floor(int((self.entry[-1].entrytime - self.entry[0].entrytime).total_seconds()) / 60 / 60 % 24)
-        ))
+        print("   - Life as Tropical Cyclone: {} days".format(self.duration))
         print("* Landfall: {}{}".format(
             "Yes" if self.landfalls > 0 else "None",
             ", {} Record{}".format(
                 self.landfalls,
                 "s" if self.landfalls > 1 else ""
             ) if self.landfalls > 0 else ""
         ))
@@ -914,101 +931,135 @@
         print(" {:5} {:^14} {:-^4} {:^13}  {:^18}".format(
             "ENTRY","","LAND", "LOCATION", "INTENSITY"
         ))
         print(" {:5} {:^14} {:^4} {:^5}  {:^6}  {:^4}  {:^4}  {:^6}".format(
             "INDEX","DATE", "FALL", "LAT", "LON", "MSLP", "WIND", "STATUS"
         ))
         print(" {:-^5} {:-^14} {:-^4} {:-^5}  {:-^6}  {:-^4}  {:-^4}  {:-^6}".format("","","","","","","",""))
-        for trk in self.entry:
+        for en in self.entry:
             print(" {:^5} {:%Y-%m-%d %H}Z {:^4} {:5}  {:6}  {:4}  {:4}  {:^6}".format(
-                self.entry.index(trk),
-                trk.entrytime,
-                trk.record_identifier if trk.record_identifier == "L" else "",
-                trk.lat_str,
-                trk.lon_str,
-                trk.mslp if trk.mslp != None else "N/A",
-                trk.wind,
-                trk.status if trk.wind < 96 else "MHU"
+                self.entry.index(en),
+                en.entrytime,
+                en.record_identifier if en.record_identifier == "L" else "",
+                en.lat_str,
+                en.lon_str,
+                en.mslp if en.mslp != None else "N/A",
+                en.wind,
+                en.status if en.wind < 96 else "MHU"
             ))
         print("")
 
     def hurdat2(self):
         """Prints a Hurdat2-formatted summary of the tropical cyclone."""
         print("{:>8},{:>19},{:>7},".format(
             self.atcfid,
             self.name,
             len(self.entry)
         ))
         for entry in self.entry:
             print(entry.hurdat2())
 
     @property
+    def tc_entries(self):
+        """
+        Returns a list of <<TCRecordEntry>>'s where the storm is designated a
+        tropical cyclone.
+        """
+        return [
+            en for en in self.entry
+            if en.is_TC
+        ]
+
+    @property
     def gps(self):
         """Return a list of tuples containing the gps coordinates of the
         tropical cyclone's track
         """
-        return [e.location for e in self.entry]
+        return [en.location for en in self.entry]
 
     @property
     def minmslp(self):
         """Returns the minimum mean sea-level pressure (MSLP) recorded during
         the life of the storm.
 
         If insufficient data exists to determine MSLP, None will be returned.
         """
-        return min([t.mslp for t in self.entry if t.mslp != None],default=None)
+        return min(
+            [en.mslp for en in self.entry if en.mslp != None],
+            default=None
+        )
 
     @property
     def maxwind(self):
         """Returns the max peak-wind recorded during the life of the storm."""
-        return max([t.wind for t in self.entry])
+        return max(en.wind for en in self.entry)
 
     @property
     def landfalls(self):
         """Returns the QUANTITY of landfalls recorded made by the system
         as a tropical cyclone.
         """
-        return len(["L" for t in self.entry if t.record_identifier == "L" and t.status in ["SD","TD","SS","TS","HU"]])
+        return len([
+            "L" for en in self.entry
+            if en.record_identifier == "L"
+            and en.is_TC
+        ])
 
     @property
     def landfall_TC(self):
         """Bool indicating whether at-least one landfall was made while a
         tropical cyclone.
         """
         return self.landfalls > 0
 
     @property
     def landfall_TD(self):
         """Bool indicating whether at-least one landfall was made while a
         tropical depression.
         """
-        return any(t.record_identifier == "L" for t in self.entry if t.status in ["SD","TD"])
+        return any(
+            en.record_identifier == "L"
+            for en in self.entry
+            if en.status in ["SD","TD"]
+        )
 
     @property
     def landfall_TS(self):
         """Bool indicating whether at-least one landfall was recorded by the
         tropical cyclone while designated as a tropical storm (TS) or
         sub-tropical storm (SS).
         """
-        return any(t.record_identifier == "L" for t in self.entry if t.status in ["SS","TS"])
+        return any(
+            en.record_identifier == "L"
+            for en in self.entry
+            if en.status in ["SS","TS"]
+        )
 
     @property
     def landfall_HU(self):
         """Bool indicating whether at-least one landfall was recorded by the
         tropical cyclone while designated as a Hurricane.
         """
-        return any(t.record_identifier == "L" for t in self.entry if t.status == "HU")
+        return any(
+            en.record_identifier == "L"
+            for en in self.entry
+            if en.status == "HU"
+        )
 
     @property
     def landfall_MHU(self):
         """Bool indicating whether at-least one landfall was recorded by the
         tropical cyclone while a hurricane at major-hurricane strength
         (>= 96kts).
         """
-        return any(t.record_identifier == "L" for t in self.entry if t.wind >= 96 and t.status == "HU")
+        return any(
+            en.record_identifier == "L"
+            for en in self.entry
+            if en.wind >= 96 and en.status == "HU"
+        )
 
     @property
     def TSreach(self):
         """Bool indicating whether the storm was ever objectively designated as
         a tropical storm (TS) or sub-tropical storm (SS). Hurricane's (HU) are
         tested for as well with an explanation below.
 
@@ -1017,43 +1068,43 @@
         hurricane since max-wind tendency is a continuous function. But in
         HURDAT2, they are represented as discrete or time-stepped. Because of
         this, though exceptionally rare, it is possible for a storm to have a
         hurricane entry but zero tropical storm entries. For example, in the
         Atlantic HURDAT2, this occurrence happens, but virtually all storms of
         this nature occur before 1900.
         """
-        return any(t.status in ["TS","SS","HU"] for t in self.entry)
+        return any(en.status in ["TS","SS","HU"] for en in self.entry)
 
     @property
     def HUreach(self):
         """Bool indicating whether the storm was ever objectively designated as
         a hurricane (HU).
         """
-        return any(t.status == "HU" for t in self.entry)
+        return any(en.status == "HU" for en in self.entry)
 
     @property
     def MHUreach(self):
         """Bool indicating whether the storm ever reached major hurricane
         status (>= 96kts).
         """
-        return any(t.wind >= 96 for t in self.entry if t.status == "HU")
+        return any(en.wind >= 96 for en in self.entry if en.status == "HU")
 
     @property
     def cat45reach(self):
         """Returns a bool indicating if the tropical cyclone ever reached at-
         least Category 4 strength during its life.
         """
-        return any(t.wind >= 114 for t in self.entry if t.status == "HU")
+        return any(en.wind >= 114 for en in self.entry if en.status == "HU")
 
     @property
     def cat5reach(self):
         """Returns a bool indicating if the tropical cyclone ever reached
         Category 5 strength during its life.
         """
-        return any(t.wind >= 136 for t in self.entry if t.status == "HU")
+        return any(en.wind >= 136 for en in self.entry if en.status == "HU")
 
     @property
     def maxwind_mslp(self):
         """Returns the MSLP recorded at the time of the tropical cyclone's peak
         wind-based intensity. This attribute was included as peak-winds and
         minimum MSLP, though closely related, may not necessarily occur at the
         same time.
@@ -1084,29 +1135,31 @@
         ).wind
 
     @property
     def statuses_reached(self):
         """Returns a list of all designated statuses during the tropical
         cyclone's life.
         """
-        return list(set([s.status for s in self.entry]))
+        return list(set([
+            en.status for en in self.entry
+        ]))
 
     @property
     def status_highest(self):
         """
-        Returns a readable descriptor for the storm based on its highest status
-        reached.
-        
+        Returns a readable descriptor for the storm based on its highest-order
+        status designated.
+
         Examples
         -------
         TS -> 'Tropical Storm'
         HU -> 'Hurricane'
         HU and self.maxwind >= 96 -> 'Major Hurricane'
         """
-        order = ["HU", "TS", "SS", "TD", "SD", "LO", "EX"]
+        order = ["HU", "TS", "SS", "TD", "SD", "EX", "LO", "DB"]
         for status in order:
             if status in self.statuses_reached:
                 return format_status(status, self.maxwind)
 
 class TCRecordEntry(_aliases.TCEntryAliases, _calculations.TCEntryCalculations):
     """Object that holds information from one individual (one line) HURDAT2
     entry.
@@ -1114,121 +1167,279 @@
 
     __slots__ = [
         "_entrytime", "_record_identifier", "_status",
         "_lat_str", "_lon_str", "_location", "_lat", "_lon",
         "_wind", "_status_desc", "_mslp",
         "_tsNE", "_tsSE", "_tsSW", "_tsNW",
         "_ts50NE", "_ts50SE", "_ts50SW", "_ts50NW",
-        "_huNE", "_huSE", "_huSW", "_huNW", "_wind_radii",
-        "_tc", "_season", "_hd2"
+        "_huNE", "_huSE", "_huSW", "_huNW", "_maxwind_radius",
+        "_tc", "_season", "_hd2", "_hurdat2line"
     ]
 
     TCRecordLine = collections.namedtuple(
         "TCRecordLine",
         [
             "day", "time", "record_identifier", "status",
             "latitude", "longitude", "wind", "mslp",
             "tsNE", "tsSE", "tsSW", "tsNW",
             "ts50NE", "ts50SE", "ts50SW", "ts50NW",
-            "huNE", "huSE", "huSW", "huNW", "wind_radii"
+            "huNE", "huSE", "huSW", "huNW", "maxwind_radius"
         ],
-        defaults = (None,)
+        # defaults necessary to maintain backward compatibility
+        # This would be backward compatible
+        defaults = (None, None, None, None, None)
     )
 
-    def __init__(self, tc_entry, tcobj, seasonobj, hd2obj):
+    def __init__(self, tc_entry, hurdat2line, tcobj, seasonobj, hd2obj):
 
-        try:
-            tcentry = self.TCRecordLine(*tc_entry)
-        except:
-            print(tc_entry)
-            raise
+        tcentry = self.TCRecordLine(*tc_entry)
+
+        # The original hurdat2 line that this entry was created from
+        self._hurdat2line = hurdat2line
 
         # Date
         self._entrytime = datetime.datetime(
-            int(tcentry.day[:4]),
-            int(tcentry.day[4:6]),
-            int(tcentry.day[6:]),
-            int(tcentry.time[:2]),
-            int(tcentry.time[2:])
+            int(tcentry[0][:4]),  #year
+            int(tcentry[0][4:6]), #month
+            int(tcentry[0][-2:]), #day
+            int(tcentry[1][:2]),
+            int(tcentry[1][-2:])
         )
 
-        self._record_identifier = tc_entry[2] if tc_entry[2] != '' else None
-        self._status = tc_entry[3]
-        self._lat_str = tc_entry[4]
-        self._lon_str = tc_entry[5]
-        self._location = coord(self.lat_str,self.lon_str)
-        self._lat = self.location[0]
-        self._lon = self.location[1]
-        self._wind = int(tc_entry[6])
-        self._status_desc = format_status(self.status,self.wind)
-        self._mslp = int(tc_entry[7]) if tc_entry[7] != '-999' else None
+        self._record_identifier = tcentry[2] if tcentry[2] != '' else None
+        self._status = tcentry[3]
+        self._lat_str = tcentry[4]
+        self._lon_str = tcentry[5]
+        self._lat = coord_conv(self.lat_str)
+        self._lon = coord_conv(self.lon_str)
+        self._wind = int(tcentry[6])
+        self._status_desc = format_status(self.status, self.wind)
+        self._mslp = int(tcentry[7]) if tcentry[7] != '-999' else None
         # Extent Indices - 0 = NE, 1 = SE, 2 = SW, 3 = NW
-        self._tsNE = int(tcentry.tsNE) if tcentry.tsNE != "-999" else None
-        self._tsSE = int(tcentry.tsSE) if tcentry.tsSE != "-999" else None
-        self._tsSW = int(tcentry.tsSW) if tcentry.tsSW != "-999" else None
-        self._tsNW = int(tcentry.tsNW) if tcentry.tsNW != "-999" else None
-        self._ts50NE = int(tcentry.ts50NE) if tcentry.ts50NE != "-999" else None
-        self._ts50SE = int(tcentry.ts50SE) if tcentry.ts50SE != "-999" else None
-        self._ts50SW = int(tcentry.ts50SW) if tcentry.ts50SW != "-999" else None
-        self._ts50NW = int(tcentry.ts50NW) if tcentry.ts50NW != "-999" else None
-        self._huNE = int(tcentry.huNE) if tcentry.huNE != "-999" else None
-        self._huSE = int(tcentry.huSE) if tcentry.huSE != "-999" else None
-        self._huSW = int(tcentry.huSW) if tcentry.huSW != "-999" else None
-        self._huNW = int(tcentry.huNW) if tcentry.huNW != "-999" else None
-        self._wind_radii = int(tcentry.wind_radii) if tcentry.wind_radii not in ["-999", None] else None
+        # Tropical Storm extents
+        self._tsNE = int(tcentry[8]) \
+            if tcentry[8] != "-999" \
+            else 0 if self._wind < 34 \
+            else None
+        self._tsSE = int(tcentry[9]) \
+            if tcentry[9] != "-999" \
+            else 0 if self._wind < 34 \
+            else None
+        self._tsSW = int(tcentry[10]) \
+            if tcentry[10] != "-999" \
+            else 0 if self._wind < 34 \
+            else None
+        self._tsNW = int(tcentry[11]) \
+            if tcentry[11] != "-999" \
+            else 0 if self._wind < 34 \
+            else None
+        # Gale extents
+        self._ts50NE = int(tcentry[12]) \
+            if tcentry[12] != "-999" \
+            else 0 if self._wind < 50 \
+            else None
+        self._ts50SE = int(tcentry[13]) \
+            if tcentry[13] != "-999" \
+            else 0 if self._wind < 50 \
+            else None
+        self._ts50SW = int(tcentry[14]) \
+            if tcentry[14] != "-999" \
+            else 0 if self._wind < 50 \
+            else None
+        self._ts50NW = int(tcentry[15]) \
+            if tcentry[15] != "-999" \
+            else 0 if self._wind < 50 \
+            else None
+        # Hurricane extents
+        self._huNE = int(tcentry[16]) \
+            if tcentry[16] != "-999" \
+            else 0 if self._wind < 64 \
+            else None
+        self._huSE = int(tcentry[17]) \
+            if tcentry[17] != "-999" \
+            else 0 if self._wind < 64 \
+            else None
+        self._huSW = int(tcentry[18]) \
+            if tcentry[18] != "-999" \
+            else 0 if self._wind < 64 \
+            else None
+        self._huNW = int(tcentry[19]) \
+            if tcentry[19] != "-999" \
+            else 0 if self._wind < 64 \
+            else None
+        self._maxwind_radius = int(tcentry[20]) \
+            if len(tcentry) >= 21 \
+            and tcentry[20] not in ["-999", None] \
+            else None
 
         # Record parent objects
         self._tc = tcobj
         self._season = seasonobj
         self._hd2 = hd2obj
 
     def __repr__(self):
         return "<{} object - {}:{} - Index {}: {:%Y%m%d %H%MZ} - at 0x{}>".format(
             re.search(r"'(.*)'", str(type(self)))[1],
             self._tc.atcfid,
             self._tc.name,
             self._tc.entry.index(self),
             self.date,
-            str(id(self)).upper().zfill(16)
+            hex(id(self))[2:].upper().zfill(16)
         )
 
+    @property
+    def location(self):
+        """
+        Returns a tuple of the latitude and longitude (in decimal degrees and
+        in that respective order) for this entry.
+        """
+        return (self.lat, self.lon)
+
+    @property
+    def location_reversed(self):
+        """
+        Returns a tuple of the longitude and latitude (in decimal degrees and
+        in that respective order) for this entry.
+
+        This was included as GIS programs seem to prefer this order.
+        """
+        return (self.lon, self.lat)
+
+    @property
+    def is_TC(self):
+        """Returns whether or not the storm was designated as a tropical
+        cyclone at the time of this <<TCRecordEntry>>.
+
+        The entry status must be one of the following: "SD", "TD", "SS", "TS", "HU".
+        """
+        return self.status in ["SD", "TD", "SS", "TS", "HU"]
+
+    @property
+    def is_synoptic(self):
+        """Returns whether or not the <<TCRecordEntry>>.entrytime is considered
+        to be synoptic.
+
+        To be True, it must have a recorded hour of 0Z, 6Z, 12Z, or 18Z 'on the
+        dot' (minute, second == 0).
+
+        This is helpful in calculating energy indices.
+        """
+        return self.hour in [0, 6, 12, 18] and self.minute == 0
+
+    @property
+    def previous_entries(self):
+        """
+        Returns a list of preceding <TCRecordEntry>s in the parent
+        <TropicalCyclone>.entry list.
+        """
+        return self._tc[0:self._tc.entry.index(self)]
+
+    @property
+    def previous_entry(self):
+        """
+        Returns the <TCRecordEntry> that occurred PREVIOUS (preceding this
+        entry) in the parent <TropicalCyclone>.entry list. Returns None if it
+        is the first index (index 0).
+        """
+        if self._tc.entry.index(self)-1 >= 0:
+            return self._tc[self._tc.entry.index(self)-1]
+        else:
+            return None
+
+    @property
+    def next_entries(self):
+        """
+        Returns a list of succeeding <TCRecordEntry>s in the parent
+        <TropicalCyclone>.entry list.
+        """
+        return self._tc[self._tc.entry.index(self)+1:]
+
+    @property
+    def next_entry(self):
+        """
+        Returns the <TCRecordEntry> that occurs NEXT (following this entry) in
+        the parent <TropicalCyclone>.entry list. Returns None if it is the last
+        entry.
+        """
+        try:
+            return self._tc[self._tc.entry.index(self)+1]
+        except:
+            return None
+
     def hurdat2(self):
-        """Returns a string of a hurdat2-formatted line of the entry
-        information. It should be identical to the corresponding entry in the
-        actual Hurdat2 record.
+        """
+        Returns a string of a hurdat2-formatted line of the entry information.
+
+        A few minor differences will exist between this output and the actual
+        line found in the hurdat2 database. If using an older hurdat2 database
+        (prior to 2022 release), it won't have maxwind radii available. Though
+        this field is not part of that older database, this method will report
+        it as null ('-999'). Also, wind extent information will likely be
+        different. This is because upon ingest, this module infers non-
+        applicable wind-extents as 0. For example, a tropical storm, having
+        winds < 64kt, will objectively have a hurricane wind-extent as 0, where
+        for storms prior to 2004, the database would say '-999'.
+
+        One other possible difference would occur if this version of the module
+        is used with future hurdat2 databases that include more variables
+        (which this version of the module would be oblivious to).
+
+        To see the line that the data for this entry was formulated from, use
+        the method hurdat2orig()
         """
         return "{:>8},{:>5},{:>2},{:>3},{:>6},{:>7},{:>4},{:>5},".format(
             "{:%Y%m%d}".format(self.entrytime),
             "{:%H%M}".format(self.entrytime),
-            "" if self.record_identifier is not "L" else "L",
+            "" if self.record_identifier != "L" else "L",
             self.status,
             self.lat_str,
             self.lon_str,
             self.wind,
             self.mslp if self.mslp is not None else -999,
         ) + "{:>5},{:>5},{:>5},{:>5},".format(
             *[quad if quad is not None else -999 for quad in self.extent_TS]
         ) + "{:>5},{:>5},{:>5},{:>5},".format(
             *[quad if quad is not None else -999 for quad in self.extent_TS50]
         ) + "{:>5},{:>5},{:>5},{:>5},".format(
             *[quad if quad is not None else -999 for quad in self.extent_HU]
-        )
+        ) + "{:>5},".format(self.maxwind_radius if self.maxwind_radius is not None else -999)
+
+
+    def hurdat2orig(self):
+        """
+        Returns a carbon-copy of the line from the hurdat2 database that this
+        entry was formed from.
+        """
+        return self._hurdat2line
 
-def coord(strlat,strlon):
-    """Method used typically only on read-in of data to convert a Hurdat2-
-    formatted lat/lon coordinate into a float representation of the information
-    and return it.
+    @property
+    def extent_TS(self):
+        return [self.tsNE, self.tsSE, self.tsSW, self.tsNW]
+
+    @property
+    def extent_TS50(self):
+        return [self.ts50NE, self.ts50SE, self.ts50SW, self.ts50NW]
+
+    @property
+    def extent_HU(self):
+        return [self.huNE, self.huSE, self.huSW, self.huNW]
+
+def coord_conv(coordstr):
+    """
+    Takes a hurdat2-formatted lat/lon coordinate and returns a float
+    representation thereof.
 
-    Example: coord("26.1N", "88.9W") -->  (26.1, -88.9)
+    Example:
+        coord_conv("26.1N") -->  26.1
+        coord_conv("98.6W") -->  -98.6
     """
-    if strlat[-1] == "N": decimal_lat = round(float(strlat[:-1]),1)
-    else: decimal_lat = round(-1 * float(strlat[:-1]),1)
-    if strlon[-1] == "E": decimal_lon = round(float(strlon[:-1]),1)
-    else: decimal_lon = round(-1 * float(strlon[:-1]),1)
-    return (decimal_lat, decimal_lon)
+    if coordstr[-1] in ["N", "E"]:
+        return round(float(coordstr[:-1]), 1)
+    else:
+        return round(-1 * float(coordstr[:-1]), 1)
 
 def format_record_identifier(ri):
     """Returns a description about an entry's record_identifier.
 
     Definitions/interpretations found in hurdat2-format pdf found online.
     """
     if ri == "L": return "Landfall"
@@ -1237,15 +1448,15 @@
     elif ri == "I": return "An intensity peak in terms of both pressure and wind"
     elif ri == "C": return "Closest approach to a coast, not followed by a landfall"
     elif ri == "S": return "Change of status of the system"
     elif ri == "G": return "Genesis"
     elif ri == "T": return "Provides additional detail on the track (position) of the cyclone"
     else: return "* No Description Available *"
 
-def format_status(status,wind):
+def format_status(status, wind):
     """Returns a description about a record's 2-letter status.
 
     Definitions/interpretations found in hurdat2-format pdf found online.
     """
     if status == "DB" or status == "LO" or status == "WV": return "Disturbance, Low, or Tropical Wave"
     elif status == "SD": return "Subtropical Depression"
     elif status == "TD": return "Tropical Depression"
```

### Comparing `hurdat2parser-2.11/hurdat2parser/_calculations.py` & `hurdat2parser-2.2/hurdat2parser/_calculations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 import statistics
 import math
 import textwrap
+import datetime
 import calendar
 import collections
 
+blah = dict(
+    tracks = 0, landfalls=0, landfall_TC = 0, landfall_TD = 0,
+    landfall_TS = 0, landfall_HU = 0, landfall_MHU = 0,
+    TSreach = 0, HUreach = 0, MHUreach = 0, track_distance = 0,
+    track_distance_TC = 0, track_distance_TS = 0,
+    track_distance_HU = 0, track_distance_MHU = 0,
+    ACE = 0, HDP = 0, MHDP = 0, cat45reach = 0, cat5reach = 0
+)
+
 class Hurdat2Calculations:
 
     def rank_seasons(self, quantity, stattr, year1=None, year2=None, descending=True, **kw):
         """Rank and compare full tropical cyclone seasons to one another.
 
         Required Arguments:
             quantity: how long of a list of ranks do you want; an integer.
@@ -43,36 +53,44 @@
                 cyclone seasons sorted by the top-10 Accumulated Cyclone
                 Energy values.
         <Hurdat2>.rank_seasons(15,"HDP",1967): Retrieve a report of tropical
                 cyclone seasons sorted by the top-15 Hurricane Destruction
                 Potential values occurring since 1967 (the beginning of the
                 satellite era).
         <Hurdat2>.rank_seasons(5,"track_distance_TS",1951,2000,True):
-                Retrieve a report of the bottom-5 seasons of, distance
+                Retrieve a report of the bottom-5 seasons of distance
                 traversed by, at-least, tropical storms, all between 1951 and
                 2000.
         <Hurdat2>.rank_seasons(10,"HUreach",year2=2000): Retrieves a report 
                 of the top-10 seasons with the most Hurricanes prior-to, and
                 including the year 2000.
         """
 
         # --------------------
-        year1 = year1 if year1 is not None \
-            and type(year1) == int \
-            and year1 >= self.record_range[0] \
+        year1 = abs(year1) \
+            if type(year1) == int \
+            and abs(year1) >= self.record_range[0] \
             else self.record_range[0]
-        year2 = year2 if year2 is not None \
-            and type(year2) == int \
-            and year2 <= self.record_range[1] \
+        year2 = abs(year2) \
+            if type(year2) == int \
+            and abs(year2) <= self.record_range[1] \
             else self.record_range[1]
 
+        year1, year2 = [
+            min([year1, year2]),
+            max([year1, year2])
+        ]
+
+        if len(range(year1, year2)) == 0:
+            raise ValueError("The years given must be different!")
+
         # List seasons sorted by stattr
         sorted_seasons = sorted(
             [s for s in self.season.values() if year1 <= s.year <= year2],
-            key=lambda s: getattr(s, stattr),
+            key=lambda czen: getattr(czen, stattr),
             reverse = descending
         )
         # Values sorted
         ranks = sorted(
             set([
                 getattr(s, stattr) for s in sorted_seasons \
                     if descending is False \
@@ -191,15 +209,17 @@
                 sorted calls; whether results will be printed higher-to-lower
                 or not.
 
         Keyword Arguments:
             start = (1, 1): list/tuple given to indicate the starting month and
                 day wherein a season's calculations will be made.
             thru = (12,31): list/tuple representing the month and day that you
-                want to assess the seasons through.
+                want to assess the seasons through. If start != (1,1) but thru
+                == (12,31), the stats reported will be through the Season's
+                ending.
 
         Examples:
         ---------
         <Hurdat2>.rank_seasons_thru(10, "ACE", thru=[8,31]): Retrieve a report
             of tropical cyclone seasons sorted by the top-10 ACE values through
             August 31.
         <Hurdat2>.rank_seasons_thru(10, "TSreach", 1967, thru=[9,15]): Retrieve
@@ -250,27 +270,40 @@
                 tracks = 0, landfalls=0, landfall_TC = 0, landfall_TD = 0,
                 landfall_TS = 0, landfall_HU = 0, landfall_MHU = 0,
                 TSreach = 0, HUreach = 0, MHUreach = 0, track_distance = 0,
                 track_distance_TC = 0, track_distance_TS = 0,
                 track_distance_HU = 0, track_distance_MHU = 0,
                 ACE = 0, HDP = 0, MHDP = 0, cat45reach = 0, cat5reach = 0
             )
+            # account for a non-existant season being requested by stats method
+            if kw.get("info") is not None and kw.get("info") not in self.season:
+                rseason[kw.get("info")] = dict(
+                tracks = 0, landfalls=0, landfall_TC = 0, landfall_TD = 0,
+                landfall_TS = 0, landfall_HU = 0, landfall_MHU = 0,
+                TSreach = 0, HUreach = 0, MHUreach = 0, track_distance = 0,
+                track_distance_TC = 0, track_distance_TS = 0,
+                track_distance_HU = 0, track_distance_MHU = 0,
+                ACE = 0, HDP = 0, MHDP = 0, cat45reach = 0, cat5reach = 0
+            )
             for tc in season.tc.values():
                 track_added = False
                 lndfls = False; lndfl_TC = False; lndfl_TD = False;
                 lndfl_TS = False; lndfl_HU = False; lndfl_MHU = False;
                 rTS = False; rHU = False; rMHU = False; r45 = False; r5 = False
                 entries = [
                     trk for trk in tc.entry #\
                     # if start <= trk.month_day_tuple <= thru
                 ]
                 for INDX, ENTRY in enumerate(tc.entry):
                     # Handle Track Distance related vars;
                     # only need to check validity of INDX-1
-                    if INDX >= 1 and start <= tc.entry[INDX-1].month_day_tuple <= thru:
+                    # if INDX >= 1 and start <= tc.entry[INDX-1].month_day_tuple <= thru:
+                    if INDX >= 1 \
+                    and ((thru != (12,31) and start <= tc.entry[INDX-1].month_day_tuple <= thru) \
+                    or (thru == (12,31) and datetime.date(tc.year, *start) <= tc.entry[INDX-1].entrytime.date())):
                         rseason[yr]["track_distance"] += haversine(
                             tc.entry[INDX-1].location,
                             tc.entry[INDX].location
                         )
                         rseason[yr]["track_distance_TC"] += haversine(
                             tc.entry[INDX-1].location,
                             tc.entry[INDX].location
@@ -285,40 +318,39 @@
                         ) if tc.entry[INDX-1].status == "HU" else 0
                         rseason[yr]["track_distance_MHU"] += haversine(
                             tc.entry[INDX-1].location,
                             tc.entry[INDX].location
                         ) if tc.entry[INDX-1].status == "HU" \
                           and tc.entry[INDX-1].wind >= 96 else 0
                     # Handle everything else
-                    if start <= ENTRY.month_day_tuple <= thru:
+                    if (thru != (12,31) and start <= ENTRY.month_day_tuple <= thru) \
+                    or (thru == (12,31) and datetime.date(tc.year, *start) <= ENTRY.entrytime.date()):
+                    # if start <= ENTRY.month_day_tuple <= thru:
                         rseason[yr]["ACE"] += math.pow(ENTRY.wind,2) \
                             if ENTRY.wind >= 34 \
                             and ENTRY.status in ("SS","TS","HU") \
-                            and ENTRY.hour in [0,6,12,18] \
-                            and ENTRY.minute == 0 \
+                            and ENTRY.is_synoptic \
                             else 0
                         rseason[yr]["HDP"] += math.pow(ENTRY.wind,2) \
                             if ENTRY.wind >= 64 \
                             and ENTRY.status == "HU" \
-                            and ENTRY.hour in [0,6,12,18] \
-                            and ENTRY.minute == 0 \
+                            and ENTRY.is_synoptic \
                             else 0
                         rseason[yr]["MHDP"] += math.pow(ENTRY.wind,2) \
                             if ENTRY.wind >= 96 and ENTRY.status == "HU" \
-                            and ENTRY.hour in [0,6,12,18] \
-                            and ENTRY.minute == 0 \
+                            and ENTRY.is_synoptic \
                             else 0
                         if track_added is False:
                             rseason[yr]["tracks"] += 1
                             track_added = True
                         if lndfls is False and ENTRY.record_identifier == "L":
                             rseason[yr]["landfalls"] += 1
                             lndfls = True
                         if lndfl_TC is False and ENTRY.record_identifier == "L" \
-                                and ENTRY.status in ["SD","TD","SS","TS","HU"]:
+                                and ENTRY.is_TC:
                             rseason[yr]["landfall_TC"] += 1
                             lndfl_TC = True
                         if lndfl_TD is False and ENTRY.record_identifier == "L" \
                                 and ENTRY.status in ["SD","TD"]:
                             rseason[yr]["landfall_TD"] += 1
                             lndfl_TD = True
                         if lndfl_TS is False and ENTRY.record_identifier == "L" \
@@ -390,15 +422,15 @@
                     "from {} ".format(
                         "{} {}".format(
                             calendar.month_abbr[start[0]], start[1]
                         )
                     ) if "start" in kw else "",
                     "{} {}".format(
                         calendar.month_abbr[thru[0]], thru[1]
-                    )
+                    ) if thru != (12,31) else "End of Season"
                 )
             ).center(79)
         )
 
         print("{}{}".format(
             str(self.basin()),
             ", {}-{}".format(year1, year2)
@@ -778,18 +810,129 @@
                 "{}-{}".format(*clmt.era),
                 getattr(clmt,stattr)
             ))
             if current_rank is not None and current_rank not in printedqty:
                 printedqty.append(current_rank)
         print("")
 
+    def _season_stats_str(self, seasonreq, year1, year2, rstart, rthru, width, **kw):
+        strlist = []
+        yr = seasonreq
+        strlist.append("\n")
+        strlist.append("-" * width)
+        strlist.append("Tropical Cyclone Stats for {}".format(yr).center(width))
+        strlist.append(
+            "{}{}".format(
+                self.basin(),
+                ""
+            ).center(width)
+        )
+        strlist[-1] += "\n"
+        for line in textwrap.wrap(
+            "Stats calculated for Seasons {}".format(
+                "{}-{}".format(
+                    year1,
+                    year2
+                ) if year2 != self.record_range[1] \
+                else "since {} ({} total seasons)".format(
+                    year1,
+                    self.record_range[1] - year1 + 1
+                )
+            ),
+            width,
+        ):
+            strlist.append(line)
+        if rstart != (1,1) or rthru != (12,31):
+            strlist.append(
+                "from {} thru {}".format(
+                    "{} {}".format(
+                        calendar.month_name[rstart[0]],
+                        rstart[1],
+                    ),
+                    "{} {}".format(
+                        calendar.month_name[rthru[0]],
+                        rthru[1],
+                    )
+                ).center(width)
+            )
+        strlist[-1] += "\n"
+        for line in textwrap.wrap(
+            "* TS-related Statistics include Hurricanes in their totals" \
+            " except for landfall data",
+            width,
+            initial_indent=" " * 4,
+            subsequent_indent=" " * 4
+        ):
+            strlist.append(line.center(width))
+        strlist[-1] += "\n"
+        if any(1971 <= y <= 1990 for y in range(year1, year2 + 1)):
+            for line in textwrap.wrap(
+                "* Hurdat2 Landfall data incomplete for seasons 1971-1990",
+                width,
+                initial_indent=" " * 4,
+                subsequent_indent=" " * 4
+            ):
+                strlist.append(line.center(width))
+        strlist.append("-" * width)
+
+        for attr, label in [
+            ("tracks", "Tropical Cyclones"),
+            ("track_distance_TC", "TC Track Distance"),
+            ("track_distance_TS", "TS Distance"),
+            ("track_distance_HU", "HU Distance"),
+            ("track_distance_MHU", "MHU Distance"),
+            ("TSreach", "Tropical Storms"),
+            ("ACE", "ACE"),
+            ("HUreach", "Hurricanes"),
+            ("HDP", "HDP"),
+            ("MHUreach", "Major Hurricanes"),
+            ("MHDP", "MHDP"),
+            ("landfall_TC", "Total Landfalling TC's"),
+            ("landfall_TS", "TS Landfalls"),
+            ("landfall_HU", "HU Landfalls")
+        ]:
+            if "landfall" not in attr or ("landfall" in attr and all(1971 <= y <= 1990 for y in range(year1, year2)) is False):
+                rankinfo = self.rank_seasons_thru(
+                    1337,
+                    attr,
+                    year1,
+                    year2,
+                    start = rstart,
+                    thru = rthru,
+                    descending=kw.get("descending", True),
+                    info=yr
+                )
+                strlist.append('{:<35}Rank {}/{}{}'.format(
+                    "* {}: {}{}   ".format(
+                        label,
+                        "{:.1f}".format(rankinfo["seasonvalu"]) \
+                            if "distance" in attr \
+                            else ("{:.1f}".format(rankinfo["seasonvalu"] * 10 ** (-4)) \
+                                if attr in ["ACE", "HDP", "MHDP"] \
+                                else rankinfo["seasonvalu"]
+                            ),
+                        " nmi" if "track_distance" in attr \
+                            else (" * 10^4 kt^2" \
+                                if attr in ["ACE", "HDP", "MHDP"] else ""
+                            ),
+                    ),
+                    rankinfo["rank"],
+                    rankinfo["outof"],
+                    " (tied w/{} other season{})".format(
+                        rankinfo["tied"],
+                        "s" if rankinfo["tied"] >= 2 else ""
+                    ) if rankinfo["tied"] > 0 else ""
+                ))
+        strlist.append("\n")
+        return "\n".join(strlist)
+
     def _season_stats(self, seasonreq, year1, year2, rstart, rthru, width, **kw):
 
         yr = seasonreq
-            
+
         print("")
         print("-" * width)
         print("Tropical Cyclone Stats for {}".format(yr).center(width))
         print("{}{}".format(
                 self.basin(),
                 ""
             ).center(width)
@@ -830,15 +973,15 @@
                 width,
                 initial_indent=" " * 4,
                 subsequent_indent=" " * 4):
             print(line.center(width))
 
         print("")
         # Only print this disclaimer if years in this range overlap
-        if any(1967 <= y <= 1991 for y in range(year1, year2 + 1)):
+        if any(1971 <= y <= 1990 for y in range(year1, year2 + 1)):
             for line in textwrap.wrap(
                     "* Hurdat2 Landfall data incomplete for seasons 1971-1990",
                     width,
                     initial_indent=" " * 4,
                     subsequent_indent=" " * 4):
                 print(line.center(width))
         print("-" * width)
@@ -855,15 +998,15 @@
             ("HDP", "HDP"),
             ("MHUreach", "Major Hurricanes"),
             ("MHDP", "MHDP"),
             ("landfall_TC", "Total Landfalling TC's"),
             ("landfall_TS", "TS Landfalls"),
             ("landfall_HU", "HU Landfalls")
         ]:
-            if "landfall" not in attr or ("landfall" in attr and all(1967 <= y <= 1991 for y in range(year1, year2)) is False):
+            if "landfall" not in attr or ("landfall" in attr and all(1971 <= y <= 1990 for y in range(year1, year2)) is False):
                 rankinfo = self.rank_seasons_thru(
                     1337,
                     attr,
                     year1,
                     year2,
                     start = rstart,
                     thru = rthru,
@@ -892,94 +1035,223 @@
                     ) if rankinfo["tied"] > 0 else ""
                 ))
         print("")
 
 class SeasonCalculations:
 
     @property
+    def start_date(self):
+        """The <<datetime>> of the start of the season."""
+        return self.tc_entries[0].entrytime
+
+    @property
+    def start_ordinal(self):
+        """The day-number (1-365) of the year that the start of the season took
+        place.
+        """
+        return self.start_date.replace(year=1).toordinal()
+
+    @property
+    def end_date(self):
+        """The <<datetime>> of the end of the season."""
+        last_tc_en = self.tc_entries[-1]
+        return last_tc_en.next_entry.entrytime \
+            if last_tc_en.next_entry is not None \
+            else last_tc_en.entrytime
+
+    @property
+    def end_ordinal(self):
+        """The day-number (1-365) of the year that the end of the season
+        occurred.
+
+        In the event that the day number exceeds 365, it generally means that
+        the season extended into the following year.
+        """
+        end = self.end_date.replace(year=1).toordinal()
+        # protect against seasons that extend into the following year
+        if end <= self.start_ordinal:
+            return self.end_date.replace(year=2).toordinal()
+        else:
+            return end
+
+    @property
+    def duration(self):
+        """Returns the duration of the season in days.
+
+        This is calculated using the .start_date and .end_date for the season
+        """
+        tdelta = self.end_date - self.start_date
+        # return all_times[-1] - all_times[0]
+        return tdelta.days + tdelta.seconds / 86400
+
+    @property
     def track_distance(self):
         """Returns the accumulated track distances (in nmi) of all systems
         during the season, regardless of the systems' status.
         """
-        return sum([self.tc[TC].track_distance for TC in self.tc])
+        return sum(tcyc.track_distance for tcyc in self.tc.values())
 
     @property
     def track_distance_TC(self):
         """Returns the accumulated track distances (in nmi) of all systems
         during the season, while the systems were designated as tropical
         cyclones ("SD","SS","TD","TS","HU").
         """
-        return sum([self.tc[TC].track_distance_TC for TC in self.tc])
+        return sum(tcyc.track_distance_TC for tcyc in self.tc.values())
 
     @property
     def ACE(self):
         """Returns the accumulated cyclone energy (ACE) for the entire season,
         being the sum of all individual tropical cyclone ACE's.
         """
-        return sum([self.tc[trop].ACE for trop in self.tc])
+        return sum(tcyc.ACE for tcyc in self.tc.values())
 
     @property
     def track_distance_TS(self):
         """Returns the sum of track distances (in nmi) of all tropical
         cyclones while they were designated as at-least tropical storms (SS,
         TS, or HU).
         """
-        return sum([self.tc[TC].track_distance_TS for TC in self.tc])
+        return sum(tcyc.track_distance_TS for tcyc in self.tc.values())
 
     @property
     def HDP(self):
         """Returns the hurricane destruction potential (HDP) for the entire
         season, being the sum of all individual tropical cyclone HDP's.
         """
-        return sum([self.tc[trop].HDP for trop in self.tc])
+        return sum(tcyc.HDP for tcyc in self.tc.values())
 
     @property
     def track_distance_HU(self):
         """Returns the sum of track distances (in nmi) of all tropical
         cyclones while they were of hurricane status.
         """
-        return sum([self.tc[TC].track_distance_HU for TC in self.tc])
+        return sum(tcyc.track_distance_HU for tcyc in self.tc.values())
 
     @property
     def MHDP(self):
         """Returns the major hurricane destruction potential (MHDP) for the
         entire season, being the sum of all individual tropical cyclone MHDP's.
         """
-        return sum([self.tc[trop].MHDP for trop in self.tc])
+        return sum(tcyc.MHDP for tcyc in self.tc.values())
 
     @property
     def track_distance_MHU(self):
         """Returns the sum of track distances (in nmi) of all tropical
         cyclones when the storms were designated as major hurricanes.
         """
-        return sum([self.tc[TC].track_distance_MHU for TC in self.tc])
+        return sum(tcyc.track_distance_MHU for tcyc in self.tc.values())
 
 class TropicalCycloneCalculations:
 
     @property
+    def start_date(self):
+        """The <<datetime>> of the birth of the tropical cyclone."""
+        return self.tc_entries[0].entrytime \
+            if len(self.tc_entries) > 0 else None
+
+    @property
+    def start_ordinal(self):
+        """
+        The day-number (1-365) of the year that the birth of the tropical
+        cyclone took place.
+        """
+        return self.tc_entries[0].entrytime.replace(year=1).toordinal() \
+            if len(self.tc_entries) > 0 else None
+
+    @property
+    def end_date(self):
+        """The <<datetime>> where the storm became post-tropical."""
+        if len(self.tc_entries) > 0:
+            return self.tc_entries[-1].next_entry.entrytime \
+                if self.tc_entries[-1].next_entry is not None \
+                else self.tc_entries[-1].entrytime
+        else:
+            return None
+
+    @property
+    def end_ordinal(self):
+        """
+        The day-number (1-365) of the year that the tropical cyclone became
+        post-tropical.
+
+        In the event that the day number exceeds 365, it generally means that
+        the tropical storm didn't become post-tropical until the following
+        year.
+        """
+        if len(self.tc_entries) > 0:
+            end = self.end_date.replace(year=1).toordinal()
+            # protect against seasons that extend into the following year
+            if end <= self.start_ordinal:
+                return self.end_date.replace(year=2).toordinal()
+            else:
+                return end
+        else:
+            return None
+
+    @property
+    def duration(self):
+        """
+        The track duration in days; simply the end time minus the beginning
+        time. In essence, this variable disregards the status of the storm.
+
+        For more substantive properties, try duration_<TC, TS, HU, or MHU> for
+        aggregated measurements as storms can lose and regain statuses
+        """
+
+        return (self.entry[-1].entrytime - self.entry[0].entrytime).days \
+             + (self.entry[-1].entrytime - self.entry[0].entrytime).seconds / 86400
+
+    @property
     def track_distance(self):
         """Returns the distance (in nmi) traversed by the system, regardless of
         status (whether or not the system is designated as a tropical cyclone).
         """
-        d = 0
-        for trk in range(1,len(self.entry)):
-            d += haversine(self.entry[trk-1].location, self.entry[trk].location)
-        return d
+        return sum(
+            haversine(en.previous_entry.location, en.location)
+            for en in self.entry
+            if en.previous_entry is not None
+        )
+
+    @property
+    def duration_TC(self):
+        """
+        This is the total time that a storm was a designated tropical cyclone.
+
+        * Of note * A storm can lose previous tropical cyclone status but
+        regain it. For the Atlantic Hurdat2, this occurs in around 2.6% of
+        storms, but almost 8% of storms since the year 2000. So if one compares
+        track life versus this duration property, it isn't out of the question
+        that they'll be different. See Hurricane Ivan (2004) as a prime
+        example.
+        """
+
+        totes = sum(
+            (en.next_entry.entrytime - en.entrytime).days
+            + (en.next_entry.entrytime - en.entrytime).seconds / 86400
+            if en.next_entry is not None
+            and en.is_TC
+            else 0
+            for en in self.entry
+        )
+
+        return totes
 
     @property
     def track_distance_TC(self):
         """The distance (in nmi) trekked by the system when a designated
         tropical cyclone (status as a tropical or sub-tropical depression, a
         tropical or sub-tropical storm, or a hurricane).
         """
-        d = 0
-        for trk in range(1,len(self.entry)):
-            if self.entry[trk-1].status in ("SD","TD","SS","TS","HU"):
-                d += haversine(self.entry[trk-1].location, self.entry[trk].location)
-        return d
+        return sum(
+            haversine(en.previous_entry.location, en.location)
+            for en in self.entry
+            if en.previous_entry is not None
+            and en.previous_entry.is_TC
+        )
 
     @property
     def ACE(self):
         """Returns the tropical cyclone's Accumulated Cyclone Energy (ACE).
 
         Using values from required observations (0Z, 6Z, 12Z, and 18Z), this
         variable is "calculated by summing the squares of the estimated
@@ -993,41 +1265,59 @@
         case for or against, note that it is a very small contribution. Using
         the Atlantic Hurdat2 Database as an example, when included in the
         calculation (using only storms since 1968, as that is when the SS
         designation first appears in the Atlantic HURDAT2), only around 2.5% of ACE
         contribution has occurred from sub-tropical storms.
         """
         return sum(
-            [math.pow(t.wind,2) for t in self.entry \
-                if t.wind >= 34 \
-                and t.hour in [0,6,12,18] \
-                and t.minute == 0 \
-                and t.status in ("SS","TS","HU")]
+            math.pow(en.wind,2) for en in self.entry
+            if en.wind >= 34
+            and en.is_synoptic
+            and en.status in ("SS","TS","HU")
         )
 
     @property
     def perc_ACE(self):
         """The percent (decimal form) of total season ACE contributed by this
         storm.
         """
         if self._season.ACE > 0:
             return self.ACE / self._season.ACE
         else:
             return 0
 
     @property
+    def duration_TS(self):
+        """
+        This is the total time that a storm was designated at least a tropical
+        storm.
+        """
+
+        totes = sum(
+            (en.next_entry.entrytime - en.entrytime).days
+            + (en.next_entry.entrytime - en.entrytime).seconds / 86400
+            if en.next_entry is not None
+            and en.status in ["SS", "TS", "HU"]
+            else 0
+            for en in self.entry
+        )
+
+        return totes
+
+    @property
     def track_distance_TS(self):
         """The distance (in nmi) trekked by the system while a tropical storm
         or hurricane.
         """
-        d = 0
-        for trk in range(1,len(self.entry)):
-            if self.entry[trk-1].status in ("SS","TS","HU"):
-                d += haversine(self.entry[trk-1].location, self.entry[trk].location)
-        return d
+        return sum(
+            haversine(en.previous_entry.location, en.location)
+            for en in self.entry
+            if en.previous_entry is not None
+            and en.previous_entry.status in ["SS", "TS", "HU"]
+        )
 
     @property
     def track_TS_perc_TC(self):
         """Returns the system's tropical storm track-distance divided by its 
         tropical cyclone track-distance.
 
         This value represents the proportional distance of a storm that
@@ -1045,51 +1335,84 @@
     def ACE_per_nmi(self):
         """Returns the Accumulated Cyclone Energy (ACE) divided by the
         systems's track-distance when it was at-least a tropical storm.
         """
         return self.ACE / self.track_distance_TS if self.track_distance_TS > 0 else 0
 
     @property
+    def ACE_no_landfall(self):
+        """Returns the ACE of the storm prior to any landfall made (if
+        applicable).
+        """
+
+        ace_no_lf = 0
+        for en in self.entry:
+            if en.record_identifier == "L":
+                break
+            if en.wind >= 34 \
+            and en.is_synoptic \
+            and en.status in ("SS","TS","HU"):
+                ace_no_lf += math.pow(en.wind, 2)
+        return ace_no_lf
+
+    @property
     def HDP(self):
         """Returns the tropical cyclone's Hurricane Destruction Potential
         (HDP).
 
         Using values from required observations (0Z, 6Z, 12Z, and 18Z), this
         variable is "calculated by summing the squares of the estimated
         6-hourly maximum sustained wind speed for all periods in which the
         system is a hurricane." (Bell, et. al. Climate Assessment for 1999.
         Bulletin of the American Meteorological Society. Vol 81, No. 6. June
         2000. S19.)
         """
         return sum(
-            [math.pow(t.wind,2) for t in self.entry \
-                if t.wind >= 64 \
-                and t.hour in [0,6,12,18] \
-                and t.minute == 0 \
-                and t.status == "HU"]
+            math.pow(en.wind, 2) for en in self.entry
+            if en.wind >= 64
+            and en.is_synoptic
+            and en.status == "HU"
         )
 
     @property
     def perc_HDP(self):
         """The percent (decimal form) of total season HDP contributed by this
         storm.
         """
         if self._season.HDP > 0:
             return self.HDP / self._season.HDP
         else:
             return 0
 
     @property
+    def duration_HU(self):
+        """
+        This is the total time that a storm was designated at a hurricane.
+        """
+
+        totes = sum(
+            (en.next_entry.entrytime - en.entrytime).days
+            + (en.next_entry.entrytime - en.entrytime).seconds / 86400
+            if en.next_entry is not None
+            and en.status == "HU"
+            else 0
+            for en in self.entry
+        )
+
+        return totes
+
+    @property
     def track_distance_HU(self):
         """The distance (in nmi) trekked by the system while a hurricane."""
-        d = 0
-        for trk in range(1,len(self.entry)):
-            if self.entry[trk-1].status == "HU":
-                d += haversine(self.entry[trk-1].location, self.entry[trk].location)
-        return d
+        return sum(
+            haversine(en.previous_entry.location, en.location)
+            for en in self.entry
+            if en.previous_entry is not None
+            and en.previous_entry.status == "HU"
+        )
 
     @property
     def HDP_per_nmi(self):
         """Returns the system's Hurricane Destruction Potential (HDP) divided
         by the systems's track-distance when it was a hurricane.
         """
 
@@ -1147,41 +1470,59 @@
 
         This inclusion of this variable is merely an extension of the
         definitions of ACE and HDP, which are widely referenced indices. This
         takes the logic of those definitions and applies it only to major-
         hurricanes (max-wind >= 96kts).
         """
         return sum(
-            [math.pow(t.wind,2) for t in self.entry \
-                if t.wind >= 96 \
-                and t.hour in [0,6,12,18] \
-                and t.minute == 0 \
-                and t.status == "HU"]
+            math.pow(en.wind, 2) for en in self.entry
+            if en.wind >= 96
+            and en.is_synoptic
+            and en.status == "HU"
         )
 
     @property
     def perc_MHDP(self):
         """The percent (decimal form) of total season MHDP contributed by this
         storm.
         """
         if self._season.MHDP > 0:
             return self.MHDP / self._season.MHDP
         else:
             return 0
 
     @property
+    def duration_MHU(self):
+        """
+        This is the total time that a storm was designated at a hurricane.
+        """
+
+        totes = sum(
+            (en.next_entry.entrytime - en.entrytime).days
+            + (en.next_entry.entrytime - en.entrytime).seconds / 86400
+            if en.next_entry is not None
+            and en.status == "HU" and en.wind >= 96
+            else 0
+            for en in self.entry
+        )
+
+        return totes
+
+    @property
     def track_distance_MHU(self):
         """The distance (in nmi) trekked by the system while a major
         hurricane.
         """
-        d = 0
-        for trk in range(1,len(self.entry)):
-            if self.entry[trk-1].status == "HU" and self.entry[trk-1].wind >= 96:
-                d += haversine(self.entry[trk-1].location, self.entry[trk].location)
-        return d
+        return sum(
+            haversine(en.previous_entry.location, en.location)
+            for en in self.entry
+            if en.previous_entry is not None
+            and en.previous_entry.wind >= 96
+            and en.previous_entry.status == "HU"
+        )
 
     @property
     def MHDP_per_nmi(self):
         """Returns the system's Major Hurricane Destruction Potential (MHDP)
         divided by the systems's track-distance when it was a major hurricane.
         """
         return self.MHDP / self.track_distance_MHU if self.track_distance_MHU > 0 else 0
@@ -1262,40 +1603,216 @@
 
 
 class TCEntryCalculations:
 
     __slots__ = []
 
     @property
+    def track_distance(self):
+        """
+        The track distance traversed by the system (regardless of status) from
+        the start of the track to the time of this <<TCRecordEntry>>
+        """
+        return sum(
+            haversine(en.previous_entry.location, en.location)
+            for en in self._tc.entry
+            if self._tc.entry.index(en) <= self._tc.entry.index(self)
+            and en.previous_entry is not None
+        )
+
+    @property
+    def track_distance_TC(self):
+        """
+        The track distance traversed by the system while designated a tropical
+        cyclone from the start of the track to the time of this
+        <<TCRecordEntry>>.
+        """
+        return sum(
+            haversine(en.previous_entry.location, en.location)
+            for en in self._tc.entry[:self._tc.entry.index(self)+1]
+            if en.previous_entry is not None
+            and en.previous_entry.is_TC
+        )
+
+    @property
+    def track_distance_TS(self):
+        """
+        The track distance traversed by the system while a tropical storm or
+        stronger, from the start of the track to the time of this
+        <<TCRecordEntry>>
+        """
+        return sum(
+            haversine(en.previous_entry.location, en.location)
+            for en in self._tc.entry[:self._tc.entry.index(self)+1]
+            if en.previous_entry is not None
+            and en.previous_entry.status in ("SS", "TS", "HU")
+        )
+
+    @property
+    def track_distance_HU(self):
+        """
+        The track distance traversed by the system while designated a hurricane
+        from the start of the track to the time of this <<TCRecordEntry>>
+        """
+        return sum(
+            haversine(en.previous_entry.location, en.location)
+            for en in self._tc.entry[:self._tc.entry.index(self)+1]
+            if en.previous_entry is not None
+            and en.previous_entry.status == "HU"
+        )
+
+    @property
+    def track_distance_MHU(self):
+        """
+        The track distance traversed by the system while designated a major-
+        hurricane, from the start of the track to the time of this
+        <<TCRecordEntry>>
+        """
+        return sum(
+            haversine(en.previous_entry.location, en.location)
+            for en in self._tc.entry[:self._tc.entry.index(self)+1]
+            if en.previous_entry is not None
+            and en.previous_entry.status == "HU"
+            and en.previous_entry.wind >= 96
+        )
+
+    def direction(self, cardinal=False):
+        """Returns the heading (in degrees) of the tropical cyclone at the time
+        of the <TCRecordEntry>.
+
+        This is calculated using this and the previous entry locations.
+
+        Default Argument
+        ----------------
+            cardinal (False): if True, it will return an accurate cardinal
+                direction abbreviation (ex: 'NNW' == North-Northwest) instead
+                of degrees.
+
+        Of note, the first entry (index of 0) of any tropical cyclone will not
+        have any associated direction because there is no previous entry to
+        compare it with.
+
+        For reference:
+              Degrees           Direction
+            ----------      -------------------
+              0 //  45      North // North-east
+             90 // 135      East  // South-east
+            180 // 225      South // South-west
+            270 // 315      West  // North-west
+        """
+        if self._tc.entry.index(self) != 0:
+            dlat = self.latitude - self.previous_entry.latitude
+            # account for longitudinal traversals of 180E/-180W
+            if abs(self.longitude - self.previous_entry.longitude) < 180:
+                dlon = self.longitude - self.previous_entry.longitude
+            else:
+                dlon = self.longitude + (
+                    360 * (1 if self.longitude < 0 else -1)
+                ) - self.previous_entry.longitude
+            deg_dir = math.degrees(math.atan2(dlon, dlat))
+            if cardinal is True:
+                return cardinal_direction(
+                    deg_dir + (360 if deg_dir < 0 else 0)
+                )
+            else:
+                return deg_dir + (360 if deg_dir < 0 else 0)
+        else:
+            return None
+
+    @property
+    def speed(self):
+        """
+        Returns the forward lateral speed of the tropical cyclone at the time
+        of the <TCRecordEntry> in knots (nautical miles per hour).
+
+        This is calculated using this and the previous entry locations (gps
+        coordinates) and the time of the entry.
+
+        Of note, the first entry (index of 0) of any tropical cyclone will not
+        have any associated speed because there is no previous entry to compare
+        it to.
+        """
+        if self._tc.entry.index(self) != 0:
+            dist = haversine(self.location, self.previous_entry.location)
+            et = (self.entrytime - self.previous_entry.entrytime).seconds / 60 / 60
+            return dist / et
+        else:
+            return None
+
+    @property
     def saffir_simpson(self):
         return saffir_simpson_scale(self.wind)
 
     @property
     def avg_wind_extent_TS(self):
         """Returns the average extent of at-least tropical storm winds."""
         return statistics.mean(self.extent_TS)
 
     @property
+    def areal_extent_TS(self):
+        """Return the instantaneous maximum tropical-storm-strength wind areal
+        expanse (in nmi^2) covered by the storm.
+        
+        This is calculated by taking each TS-wind quadrant value and summing
+        their areal-extents (those extents being considered 1/4 of a circle). 
+        """
+        return sum(
+            math.pi * math.pow(r, 2) / 4
+            for r in self.extent_TS
+            if r is not None
+        )
+
+    @property
     def avg_wind_extent_TS50(self):
         """Returns the average extent of at-least gale winds."""
         return statistics.mean(self.extent_TS50)
 
     @property
+    def areal_extent_TS50(self):
+        """Return the instantaneous maximum gale-strength wind (TS50; winds >=
+        50kts) areal expanse (in nmi^2) covered by the storm.
+        
+        This is calculated by taking each TS50-wind quadrant value and summing
+        their areal-extents (those extents being considered 1/4 of a circle). 
+        """
+        return sum(
+            math.pi * math.pow(r, 2) / 4 \
+            for r in self.extent_TS50 \
+            if r is not None
+        )
+
+    @property
     def avg_wind_extent_HU(self):
         """Returns the average extent of hurricane-strength winds."""
         return statistics.mean(self.extent_HU)
 
+    @property
+    def areal_extent_HU(self):
+        """Return the instantaneous maximum hurricane-strength wind areal
+        expanse (in nmi^2) covered by the storm.
+        
+        This is calculated by taking each HU-wind quadrant value and summing
+        their areal-extents (those extents being considered 1/4 of a circle).
+        """
+
+        return sum(
+            math.pi * math.pow(r, 2) / 4 \
+            for r in self.extent_HU \
+            if r is not None
+        )
+
 def saffir_simpson_scale(spd):
     """Static method that returns the equivalent saffir-simpson scale rating,
     based on wind-speed in knots.
 
     This is the most-common index used to generalize tropical cyclone
-    intensity.
+    intensity. Tropical storm speeds will return 0; Weaker storms will return
+    -1.
 
-    Example: saffir_simpson(100) --> 3 (implying category 3).
+    Example: saffir_simpson_scale(100) --> 3 (implying category 3).
     """
     if 34 <= spd < 64:     return 0
     elif 64 <= spd < 83:   return 1
     elif 83 <= spd < 96:   return 2
     elif 96 <= spd < 114:  return 3
     elif 114 <= spd < 136: return 4
     elif spd >= 136:   return 5
@@ -1319,20 +1836,97 @@
 
 def haversine(startpos, endpos):
     """Returns the distance (in nmi) between two tupled GPS coordinates.
 
     Args:
         startpos: the starting gps-coordinate point; in tuple form of 
             (latitude, longitude). Both need to be an int or float.
-        endpos: the starting gps-coordinate point; in tuple form of (latitude,
+        endpos: the ending gps-coordinate point; in tuple form of (latitude,
             longitude). Both need to be an int or float.
 
     The formula used was found on Wikipedia
         (https://en.wikipedia.org/wiki/Haversine_formula).
     """
     lat1 = math.radians(startpos[0])
     lon1 = math.radians(startpos[1])
     lat2 = math.radians(endpos[0])
     lon2 = math.radians(endpos[1])
     r = 3440.065    # mean radius of earth in nmi
     d = 2 * r * math.asin(math.sqrt(math.pow(math.sin((lat2 - lat1)/2),2) + math.cos(lat1) * math.cos(lat2) * math.pow(math.sin((lon2-lon1)/2),2)))
-    return d
+    return d
+
+def cardinal_direction(deg):
+    """
+    Returns the cardinal direction (an abbreviation) based on a degree-heading.
+
+    Examples:
+        10.5 --> 'N'
+        257  --> 'WSW'
+        20.2 --> 'NNE'
+        93   --> 'E'
+        165  --> 'SSE'
+    """
+    if   deg <=  11.25: return "N"
+    elif deg <=  33.75: return "NNE"
+    elif deg <=  56.25: return "NE"
+    elif deg <=  78.75: return "ENE"
+    elif deg <= 101.25: return "E"
+    elif deg <= 123.75: return "ESE"
+    elif deg <= 146.25: return "SE"
+    elif deg <= 168.75: return "SSE"
+    elif deg <= 191.25: return "S"
+    elif deg <= 213.75: return "SSW"
+    elif deg <= 236.25: return "SW"
+    elif deg <= 258.75: return "WSW"
+    elif deg <= 281.25: return "W"
+    elif deg <= 303.75: return "WNW"
+    elif deg <= 326.25: return "NW"
+    elif deg <= 348.75: return "NNW"
+    else: return "N"
+
+
+def direction(lat1, lon1, lat2, lon2, cardinal=False):
+    """
+    This is essentially a mirror function of the
+    <TCEntryCalculations>.direction method. Just included so I could test some
+    arbitrary coordinates and revisit later if I choose.
+    """
+    dlat = lat2 - lat1
+    # account for longitudinal traversals of 180E/-180W
+    if abs(lon2 - lon1) < 180:
+        dlon = lon2 - lon1
+    else:
+        dlon = lon2 + (
+            360 * (1 if lon2 < 0 else -1)
+        ) - lon1
+    deg_dir = math.degrees(math.atan2(dlon, dlat))
+    if cardinal is True:
+        return cardinal_direction(
+            deg_dir + (360 if deg_dir < 0 else 0)
+        )
+    else:
+        return deg_dir + (360 if deg_dir < 0 else 0)
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
```

### Comparing `hurdat2parser-2.11/hurdat2parser/_reports.py` & `hurdat2parser-2.2/hurdat2parser/_reports.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,235 +1,311 @@
 import operator
 import json
-import shapefile
-import geojson
 import statistics
 import math
 import os
+import re
 import csv
 import itertools
 import collections
 
+try:
+    import shapefile
+except:
+    print("* Error attempting to import shapefile")
+
+try:
+    import geojson
+except:
+    print("* Error attempting to import geojson")
+
 from . import _calculations
 from . import _maps
 
-import matplotlib
-import matplotlib.pyplot as plt
-import matplotlib.ticker as _ticker
-import matplotlib.dates as _dates
-import matplotlib.figure as _figure
-import matplotlib.patches as _patches
+try:
+    import matplotlib
+    import matplotlib.style as mplstyle
+    import matplotlib.pyplot as plt
+    import matplotlib.ticker as _ticker
+    import matplotlib.dates as _dates
+    import matplotlib.figure as _figure
+    import matplotlib.patches as _patches
+except Exception as e:
+    print("* Error attempting to import matplotlib: {}".format(e))
+
+CSV_VARS = [
+    ('TC Qty', 'tracks'),
+    # ('Trk Dist', 'track_distance'),
+    ('Landfalls (Acc.)', 'landfalls'),
+    ('TC Trk Dist', 'track_distance_TC'),
+    ('TC Landfall', 'landfall_TC'),
+    ('TS', 'TSreach'),
+    ('TS Landfall', 'landfall_TS'),
+    ('ACE', 'ACE'),
+    ('TS Trk Dist', 'track_distance_TS'),
+    ('TS-Excl', 'TSonly'),
+    ('HU', 'HUreach'),
+    ('HU Landfall', 'landfall_HU'),
+    ('HDP', 'HDP'),
+    ('HU Trk Dist', 'track_distance_HU'),
+    ('HU-1and2', 'HUonly'),
+    ('MHU', 'MHUreach'),
+    ('MHU Landfall', 'landfall_MHU'),
+    ('MHDP', 'MHDP'),
+    ('MHU Trk Dist', 'track_distance_MHU'),
+    ('Cat 4 and 5 Qty', 'cat45reach'),
+    ('Cat 5 Qty', 'cat5reach'),
+]
+
+CSV_CLIMO_VARS = [('Climatology', "era")] + CSV_VARS
+
+CSV_SEASON_VARS = [
+    ('Year', 'year'),
+    ('Duration (days)', 'duration'),
+    ('Start Ordinal', 'start_ordinal'),
+    ('End Ordinal', 'end_ordinal'),
+] + CSV_VARS
+
+CSV_TC_VARS = [
+    ('Year', 'year'),
+    ('ATCF Num', 'atcf_num'),
+    ('ATCF Id', 'atcfid'),
+    ('Name', 'name'),
+    ('Duration (days) as TC', 'duration_TC'),
+    ('Start Ordinal', 'start_ordinal'),
+    ('End Ordinal', 'end_ordinal'),
+    ('Min MSLP', 'minmslp'),
+    ('Max Wind', 'maxwind'),
+    ('Highest Status Reached', 'status_highest'),
+] + [
+    VAR for VAR in CSV_VARS[1:]
+    if "only" not in VAR[-1]
+    and "reach" not in VAR[-1]
+]
+
+Era = collections.namedtuple(
+    "Era",
+    [attr for desc, attr in CSV_CLIMO_VARS]
+)
+
+class ClimateEra(object):
+    def __init__(self, **kw):
+        self.__dict__.update(**kw)
 
 class Hurdat2Reports:
 
+    def multi_season_info(self, year1=None, year2=None):
+        """Grab a chunk of multi-season data and report on that climate era.
+        This method can be viewed as a climatological era info method.
+        
+        Default Arguments:
+            year1 (None): The start year
+            year2 (None): The end year
+        """
+
+        year1 = self.record_range[0] if year1 is None \
+            or year1 < self.record_range[0] else year1
+        year2 = self.record_range[1] if year2 is None \
+            or year2 > self.record_range[1] else year2
+        # ---------------------
+
+        yrrange = range(year1, year2+1)
+        clmt = ClimateEra(
+            era = (year1, year2),
+            tracks = sum(self.season[s].tracks for s in yrrange),
+            landfalls = sum(self.season[s].landfalls for s in yrrange),
+            landfall_TC = sum(self.season[s].landfall_TC for s in yrrange),
+            landfall_TD = sum(self.season[s].landfall_TD for s in yrrange),
+            landfall_TS = sum(self.season[s].landfall_TS for s in yrrange),
+            landfall_HU = sum(self.season[s].landfall_HU for s in yrrange),
+            landfall_MHU = sum(self.season[s].landfall_MHU for s in yrrange),
+            TSreach = sum(self.season[s].TSreach for s in yrrange),
+            TSonly = sum(self.season[s].TSonly for s in yrrange),
+            HUreach = sum(self.season[s].HUreach for s in yrrange),
+            HUonly = sum(self.season[s].HUonly for s in yrrange),
+            MHUreach = sum(self.season[s].MHUreach for s in yrrange),
+            cat45reach = sum(self.season[s].cat45reach for s in yrrange),
+            cat5reach = sum(self.season[s].cat5reach for s in yrrange),
+            track_distance = sum(self.season[s].track_distance for s in yrrange),
+            track_distance_TC = sum(self.season[s].track_distance_TC for s in yrrange),
+            track_distance_TS = sum(self.season[s].track_distance_TS for s in yrrange),
+            track_distance_HU = sum(self.season[s].track_distance_HU for s in yrrange),
+            track_distance_MHU = sum(self.season[s].track_distance_MHU for s in yrrange),
+            ACE = sum(self.season[s].ACE for s in yrrange),
+            HDP = sum(self.season[s].HDP for s in yrrange),
+            MHDP = sum(self.season[s].MHDP for s in yrrange)
+        )
+
+        # Print Report
+        totalyrs = year2 - year1 + 1
+        print("")
+        print(" --------------------------------------------------------")
+        print(" Tropical Cyclone Season Stats, for {} to {}".format(year1, year2))
+        print(" --------------------------------------------------------")
+        print(" {:^56}".format(
+            "* Distances in nmi; * Energy Indices in 10**(-4) kt^2"
+        ))
+        print(" --------------------------------------------------------")
+        print(" Avg Track Qty (Total): {}/yr ({})".format(
+            round(clmt.tracks / totalyrs,1),
+            clmt.tracks
+        ))
+        print(" Avg TC Track Distance (Total): {}/yr ({})".format(
+            round(clmt.track_distance_TC / totalyrs,1),
+            round(clmt.track_distance_TC,1)
+        ))
+        print(" Avg TS Qty (Total): {}/yr ({})".format(
+            round(clmt.TSreach / totalyrs,1),
+            clmt.TSreach
+        ))
+        print("   -- Avg TS Track Distance (Total): {}/yr ({})".format(
+            round(clmt.track_distance_TS / totalyrs,1),
+            round(clmt.track_distance_TS,1)
+        ))
+        print("   -- Avg ACE (Total): {}/yr ({})".format(
+            round(clmt.ACE * 10**(-4) / totalyrs,1),
+            round(clmt.ACE * 10**(-4),1)
+        ))
+        print(" Avg HU Qty (Total): {}/yr ({})".format(
+            round(clmt.HUreach / totalyrs,1),
+            clmt.HUreach
+        ))
+        print("   -- Avg HU Track Distance (Total): {}/yr ({})".format(
+            round(clmt.track_distance_HU / totalyrs,1),
+            round(clmt.track_distance_HU,1)
+        ))
+        print("   -- Avg HDP (Total): {}/yr ({})".format(
+            round(clmt.HDP * 10**(-4) / totalyrs,1),
+            round(clmt.HDP * 10**(-4),1)
+        ))
+        print(" Avg MHU Qty (Total): {}/yr ({})".format(
+            round(clmt.MHUreach / totalyrs,1),
+            clmt.MHUreach
+        ))
+        print(" Avg Cat-4 and Cat-5 Qty (Total): {}/yr ({})".format(
+            round(clmt.cat45reach / totalyrs,1),
+            clmt.cat45reach
+        ))
+        print(" Avg Cat-5 Qty (Total): {}/yr ({})".format(
+            round(clmt.cat5reach / totalyrs,1),
+            clmt.cat5reach
+        ))
+        print("   -- Avg MHU Track Distance (Total): {}/yr ({})".format(
+            round(clmt.track_distance_MHU / totalyrs,1),
+            round(clmt.track_distance_MHU,1)
+        ))
+        print("   -- Avg MHDP (Total): {}/yr ({})".format(
+            round(clmt.MHDP * 10**(-4) / totalyrs,1),
+            round(clmt.MHDP * 10**(-4),1)
+        ))
+        print(" Avg Landfalling System Qty (Total): {}/yr ({})".format(
+            round(clmt.landfall_TC / totalyrs,1),
+            clmt.landfall_TC
+        ))
+        print("")
+
     def output_climo(self, climo_len=30):
         """Output a csv of stats from all climatological eras from the record
         of specifiable era-spans. Temporal separations of 1-year increments
         will be used.
 
         Default Arguments:
             climo_len (30): The length of time in years each climate era will
                 be assessed.
         """
-        class LAMBDA_CLASS:
-            def __init__(self, **kw):
-                self.__dict__ = kw
 
         ofn = "{}_HURDAT2_{}-yr_climatology.csv".format(
-            "ATL" if list(self.tc.keys())[0][:2] == "AL" else "PAC",
+            "".join(self.basin_abbr()),
             climo_len
         )
         
         if os.path.exists(ofn):
             choice = input(
                 "* A file named '{}' already exists.".format(ofn) \
                 + "Continue? (y/n): "
             )
             if choice.lower()[0] != "y": return None
         print("** PLEASE WAIT; THIS MAY TAKE A MOMENT **")
-        # climo = self.rank_climo(10,"tracks",climatology=climo_len,increment=1,op=True)
-
-        # ---------------------
-        Era = collections.namedtuple(
-            "Era",
-            [
-                "era", "tracks", "landfalls", "landfall_TC", "landfall_TD",
-                "landfall_TS", "landfall_HU", "landfall_MHU", "TSreach",
-                "TSonly", "HUreach", "HUonly", "MHUreach", "cat45reach",
-                "cat5reach", "track_distance", "track_distance_TC",
-                "track_distance_TS", "track_distance_HU", "track_distance_MHU",
-                "ACE", "HDP", "MHDP"
-            ]
-        )
 
-        year1 = self.record_range[0]
-        year2 = self.record_range[1]
+        year1, year2 = self.record_range
         climo = {}
-        for yr1, yr2 in [(y, y+climo_len-1) \
-                for y in range(year1, year2+1) \
-                if year1 <= y <= year2 \
-                and year1 <= y+climo_len-1 <= year2]:
+        for yr1, yr2 in [
+            (y, y+climo_len-1) \
+            for y in range(year1, year2+1) \
+            if year1 <= y <= year2 \
+            and year1 <= y+climo_len-1 <= year2
+        ]:
             climo[yr1, yr2] = Era(
-                (yr1, yr2),
-                sum(self.season[s].tracks for s in range(yr1, yr2+1)),
-                sum(self.season[s].landfalls for s in range(yr1, yr2+1)),
-                sum(self.season[s].landfall_TC for s in range(yr1, yr2+1)),
-                sum(self.season[s].landfall_TD for s in range(yr1, yr2+1)),
-                sum(self.season[s].landfall_TS for s in range(yr1, yr2+1)),
-                sum(self.season[s].landfall_HU for s in range(yr1, yr2+1)),
-                sum(self.season[s].landfall_MHU for s in range(yr1, yr2+1)),
-                sum(self.season[s].TSreach for s in range(yr1, yr2+1)),
-                sum(self.season[s].TSonly for s in range(yr1, yr2+1)),
-                sum(self.season[s].HUreach for s in range(yr1, yr2+1)),
-                sum(self.season[s].HUonly for s in range(yr1, yr2+1)),
-                sum(self.season[s].MHUreach for s in range(yr1, yr2+1)),
-                sum(self.season[s].cat45reach for s in range(yr1, yr2+1)),
-                sum(self.season[s].cat5reach for s in range(yr1, yr2+1)),
-                sum(self.season[s].track_distance for s in range(yr1, yr2+1)),
-                sum(self.season[s].track_distance_TC for s in range(yr1, yr2+1)),
-                sum(self.season[s].track_distance_TS for s in range(yr1, yr2+1)),
-                sum(self.season[s].track_distance_HU for s in range(yr1, yr2+1)),
-                sum(self.season[s].track_distance_MHU for s in range(yr1, yr2+1)),
-                sum(self.season[s].ACE for s in range(yr1, yr2+1)),
-                sum(self.season[s].HDP for s in range(yr1, yr2+1)),
-                sum(self.season[s].MHDP for s in range(yr1, yr2+1))
+                *(
+                    [(yr1, yr2)] + [
+                        sum(getattr(self.season[s], attr)
+                        for s in range(yr1, yr2+1))
+                        for desc, attr in CSV_CLIMO_VARS[1:]
+                    ]
+                )
             )
 
-        # --------------------------------
-
         with open(ofn, "w", newline="") as w:
             out = csv.writer(w)
-            out.writerow([
-                "Climatology", "TC Qty", "Trk Dist", "Landfalls (Acc.)",
-                "TC Landfall", "TS Landfall", "HU Landfall", "MHU Landfall",
-                "TC Trk Dist", "TS", "ACE", "TS Trk Dist", "TS-Excl", "HU",
-                "HDP", "HU Trk Dist", "HU-1and2", "MHU", "Cat 4 and 5 Qty",
-                "Cat 5 Qty", "MHDP", "MHU Trk Dist"
-            ])
+            out.writerow([desc for desc, attr in CSV_CLIMO_VARS])
             for clmt in climo.values():
-                out.writerow([
-                    "{}-{}".format(
-                        clmt.era[0],
-                        clmt.era[1]
-                    ),
-                    clmt.tracks,
-                    clmt.track_distance,
-                    clmt.landfalls,
-                    clmt.landfall_TC,
-                    clmt.landfall_TS,
-                    clmt.landfall_HU,
-                    clmt.landfall_MHU,
-                    clmt.track_distance_TC,
-                    clmt.TSreach,
-                    clmt.ACE,
-                    clmt.track_distance_TS,
-                    clmt.TSonly,
-                    clmt.HUreach,
-                    clmt.HDP,
-                    clmt.track_distance_HU,
-                    clmt.HUonly,
-                    clmt.MHUreach,
-                    clmt.cat45reach,
-                    clmt.cat5reach,
-                    clmt.MHDP,
-                    clmt.track_distance_MHU
-                ])
+                out.writerow(
+                    ["{}-{}".format(*clmt.era)] \
+                  + [getattr(clmt, attr) for desc, attr in CSV_CLIMO_VARS[1:]]
+                )
 
     def output_seasons_csv(self):
         """Output a csv of season-based stats from the record. In general, this
         method really only has need to be called once. The primary exception to
         this suggestion would only occur upon official annual release of the
         HURDAT2 record.
         """
         ofn = "{}_HURDAT2_seasons_summary.csv".format(
-            "ATL" if list(self.tc.keys())[0][:2] == "AL" else "PAC"
+            "".join(self.basin_abbr())
         )
         with open(ofn, "w", newline="") as w:
             out = csv.writer(w)
-            out.writerow([
-                "Year", "TC Qty", "Trk Dist", "Landfalls (Acc.)",
-                "TC Landfall", "TS Landfall", "HU Landfall", "MHU Landfall",
-                "TC Trk Dist", "TS", "ACE", "TS Trk Dist", "TS-Excl", "HU",
-                "HDP", "HU Trk Dist", "HU-1and2", "MHU", "MHDP", "MHU Trk Dist"
-            ])
-            for y in [YR[1] for YR in self.season.items()]:
-                out.writerow([
-                    y.year,
-                    y.tracks,
-                    y.track_distance,
-                    y.landfalls,
-                    y.landfall_TC,
-                    y.landfall_TS,
-                    y.landfall_HU,
-                    y.landfall_MHU,
-                    y.track_distance_TC,
-                    y.TSreach,
-                    y.ACE,
-                    y.track_distance_TS,
-                    y.TSonly,
-                    y.HUreach,
-                    y.HDP,
-                    y.track_distance_HU,
-                    y.HUonly,
-                    y.MHUreach,
-                    y.MHDP,
-                    y.track_distance_MHU
-                ])
+            out.writerow([desc for desc, attr in CSV_SEASON_VARS])
+            for y in self.season.values():
+                out.writerow(
+                    [getattr(y, attr) for desc, attr in CSV_SEASON_VARS]
+                )
 
     def output_storms_csv(self):
         """Output a csv of individual storm-based stats from the record. In
         general, this method really only has need to be called once. The
         primary exception to this suggestion would only occur upon official
         annual release of the HURDAT2 record.
         """
         ofn = "{}_HURDAT2_storms_summary.csv".format(
-            "ATL" if list(self.tc.keys())[0][:2] == "AL" else "PAC"
+            "".join(self.basin_abbr())
         )
         with open(ofn, "w", newline="") as w:
             out = csv.writer(w)
-            out.writerow([
-                "Year", "ATCF Num", "ATCF ID", "Name", "Start Time",
-                "End Time", "HD2 Entries", "Min MSLP", "Max Wind", "Trk Dist",
-                "(Qty) Landfalls", "TD Landfall", "TS Landfall", "HU Landfall", 
-                "MHU Landfall", "Statuses", "TC Trk Dist", "TS Trk Dist",
-                "ACE", "TS Date", "HU Trk Dist", "HDP", "HU Date",
-                "MHU Trk Dist", "MHDP", "MHU Date"
-            ])
-            for TC in [tc[1] for tc in self.tc.items()]:
-                out.writerow([
-                    TC.year,
-                    int(TC.atcfid[2:4]),
-                    TC.atcfid,
-                    TC.name,
-                    TC.entry[0].entrytime,
-                    TC.entry[-1].entrytime,
-                    len(TC.entry),
-                    TC.minmslp,
-                    TC.maxwind if TC.maxwind > 0 else None,
-                    TC.track_distance,
-                    TC.landfalls,
-                    1 if TC.landfall_TD is True else 0,
-                    1 if TC.landfall_TS is True else 0,
-                    1 if TC.landfall_HU is True else 0,
-                    1 if TC.landfall_MHU is True else 0,
-                    ", ".join(TC.statuses_reached),
-                    TC.track_distance_TC,
-                    TC.track_distance_TS,
-                    TC.ACE,
-                    min([en.entrytime for en in TC.entry if en.status in ("SS","TS","HU")], default=None),
-                    TC.track_distance_HU,
-                    TC.HDP,
-                    min([en.entrytime for en in TC.entry if en.status in ("HU")], default=None),
-                    TC.track_distance_MHU,
-                    TC.MHDP,
-                    min([en.entrytime for en in TC.entry if en.status in ("HU") and en.wind >= 96], default=None)
-                ])
+            out.writerow([desc for desc, attr in CSV_TC_VARS])
+            for tc in self.tc.values():
+                out.writerow(
+                    [getattr(tc, attr) for desc, attr in CSV_TC_VARS]
+                )
 
     def climograph(self, attr, climatology=30, increment=5, **kw):
-        """zxcv
+        """Returns a basic climatological graph.
+
+        Args:
+            attr: the attribute wanted to graph
+
+        Default Keyword Arguments:
+            climatology (30): the length in years that a climatology should be
+                assessed.
+            increment (5): The temporal frequency of assessment of a
+                climatology (in years).
+
+        Keyword Arguments:
+            year1: the start year for assessment
+            year2: the end year for assessment
         """
         _w, _h = _figure.figaspect(kw.get("aspect_ratio", 3/5))
         fig = plt.figure(
             figsize = (_w, _h),
             tight_layout = True,
         )
         plt.get_current_fig_manager().set_window_title(
@@ -249,15 +325,16 @@
                     climatology,
                     increment
                 ),
                 self.basin()
             )
         )
         ax = plt.axes(
-            
+            xlabel = "Climate Era",
+            ylabel = attr
         )
         ax.plot(
             [
                 "{}-{}".format(y, y+climatology-1) \
                 for y in range(
                     kw.get("year1", self.record_range[0]),
                     kw.get("year2", self.record_range[1]) + 1 - climatology,
@@ -273,15 +350,14 @@
                 ) for y in range(
                     kw.get("year1", self.record_range[0]),
                     kw.get("year2", self.record_range[1]) + 1 - climatology,
                 ) if (y+climatology-1) % increment == 0
             ]
         )
 
-        self.rc = matplotlib.rcParams
         ax.xaxis.set_tick_params(
             rotation = 90
         )
         plt.grid(True)
         plt.show(block=False)
 
 class SeasonReports:
@@ -289,15 +365,15 @@
     def output_shp(self):
         """Uses the shapefile module to output a GIS-compatible shapefile of
         the tracks of all storms documented during a particular season. It is
         output to the current directory.
         """
         ofn = "{}_{}_tracks".format(
             self.year,
-            "ATL" if list(self.tc.keys())[0][:2] == "AL" else "PAC"
+            "".join(self._hd2.basin_abbr())
         )
         with shapefile.Writer(ofn,shapeType=3) as gis:
             gis.field("ATCFID","C","8")
             gis.field("NAME","C","10")
             gis.field("START","C","16")
             gis.field("END","C","16")
             gis.field("MAXWIND","N","3")
@@ -334,15 +410,15 @@
         """Uses the shapefile module to output a GIS-compatible shapefile of
         individual segments (as separate geometries) of each system from the
         season. Use this if you'd like the idea of coloring the tracks by
         saffir-simpson strength controlled by the segments.
         """
         ofn = "{}_{}_tracks_segmented".format(
             self.year,
-            "ATL" if list(self.tc.keys())[0][:2] == "AL" else "PAC"
+            "".join(self._hd2.basin_abbr())
         )
         c = itertools.count(0)
         with shapefile.Writer(ofn,shapeType=3) as gis:
             gis.field("ID","N","3")
             gis.field("ATCFID","C","8")
             gis.field("ENTRY_INDEX","N")
             gis.field("NAME","C","10")
@@ -385,15 +461,15 @@
         Default Argument:
             INDENT = 2; used to provide indention to the output. Though it
                 makes the output prettier and easier to read, it increases the
                 file size.
         """
         ofn = "{}_{}_tracks.geojson".format(
             self.year,
-            "ATL" if list(self.tc.keys())[0][:2] == "AL" else "PAC"
+            "".join(self._hd2.basin_abbr())
         )
         # Ensure indention is an int
         INDENT = int(INDENT)
 
         feats = []
         stormnum = itertools.count(1)
         for TC in [tc[1] for tc in self.tc.items()]:
@@ -429,15 +505,15 @@
         Default Argument:
             INDENT = 2; used to provide indention to the output. Though it
                 makes the output prettier and easier to read, it increases the
                 file size.
         """
         ofn = "{}_{}_tracks_segmented.geojson".format(
             self.year,
-            "ATL" if list(self.tc.keys())[0][:2] == "AL" else "PAC"
+            "".join(self._hd2.basin_abbr())
         )
 
         # Ensure indention is an int
         INDENT = int(INDENT)
 
         feats = []
         for TC in [tc[1] for tc in self.tc.items()]:
@@ -563,27 +639,51 @@
             ocean (matplotlib-compatible color): the requested color for the
                 ocean (the background); defaults to 'lightblue'.
             land (matplotlib-compatible color): the requested color for land-
                 masses; defaults to 'lightseagreen'.
             labels (bool): toggle for temporal labels for entries; defaults to
                 True.
             linewidth (float): the line-width of the track; defaults to 1.5.
-            markersize (float): the entry-marker size; defaults to 2.
+            markersize (float): the entry-marker size; defaults to 3.
+            legend (bool): whether or not you want to display a legend (default
+                is True).
         """
-        _w, _h = _figure.figaspect(kw.get("aspect_ratio", 3/4))
+        matplotlib.rcParams['path.simplify_threshold'] = 1
+        # _w, _h = _figure.figaspect(kw.get("aspect_ratio", 3/4))
         fig = plt.figure(
-            figsize = (_w, _h),
+            # figsize = (_w, _h),
             constrained_layout = True,
         )
-        plt.get_current_fig_manager().set_window_title(
+        figman = plt.get_current_fig_manager()
+        figman.set_window_title(
             "{} - {} Tracks".format(
                 self.atcfid,
                 self.name
             )
         )
+        MIN_SCREEN_DIM = "height" \
+            if figman.window.winfo_screenheight() < figman.window.winfo_screenwidth() \
+            else "width"
+
+        # set figure dimensions with a 4:3 aspect ratio
+        if MIN_SCREEN_DIM == "height":
+            fig.set_figheight(
+                figman.window.winfo_screenmmheight() / 25.4 - 2
+            )
+            fig.set_figwidth(
+                fig.get_figheight() * 1 / kw.get("aspect_ratio", 3/4)
+            )
+        else:
+            fig.set_figwidth(
+                figman.window.winfo_screenmmwidth() / 25.4 - 2
+            )
+            fig.set_figheight(
+                fig.get_figwidth() * kw.get("aspect_ratio", 3/4)
+            )
+
         fig.suptitle("Tracks for {} - {}".format(
             "{} {} ({})".format(
                 self.status_highest,
                 self.name.title(),
                 self.atcfid
             ) if self.name != "UNNAMED" else \
             "{} - {}".format(
@@ -599,28 +699,34 @@
                     else "%b %d"
             ) if self.entry[0].time.year == self.entry[-1].time.year else \
             "{:%Y-%m-%d} - {:%Y-%m-%d}".format(
                 self.entry[0].time,
                 self.entry[-1].time
             )
         ))
+
+
         rc = matplotlib.rcParams
         ax = plt.axes(
             facecolor = kw.get("ocean", "lightblue")
         )
         self._hd2.fig = fig
 
         # Set the axis labels
         ax.set_ylabel("Latitude")
         ax.set_xlabel("Longitude")
         ax.yaxis.set_major_locator(_ticker.MultipleLocator(5))
         ax.yaxis.set_minor_locator(_ticker.MultipleLocator(1))
         ax.xaxis.set_major_locator(_ticker.MultipleLocator(5))
         ax.xaxis.set_minor_locator(_ticker.MultipleLocator(1))
         labelrot = 0    # initialization for label rotation
+
+        #Legend Objects list
+        legend_objects = []
+
         for indx, entry in enumerate(self.entry):
             if entry != self.entry[-1]:
                 labelangle = math.degrees(
                     math.atan2(
                         self.entry[indx+1].lat - entry.lat,
                         self.entry[indx+1].lon - entry.lon
                     )
@@ -628,26 +734,41 @@
                 # labelrot = 45 if 150 <= labelangle <= 180 else \
                     # (-45 if -180 <= labelangle <= -150 else 0)
                 labelrot = 45 \
                     if (135 <= labelangle <= 180 or labelangle <= -170) else \
                        (-45 if -170 < labelangle <= -135 else labelangle - 90)
                 halign = "left" if 0 <= labelrot <= 90 else "right"
                 # print(entry.time, labelangle, labelrot, halign)
-                ax.plot(
+                line2dobj_list = ax.plot(
                     [entry.lon, self.entry[indx + 1].lon],
                     [entry.lat, self.entry[indx +1].lat],
-                    "-" if entry.status in ["SD", "TD", "SS", "TS", "HU"] else ":",
+                    "-" if entry.is_TC else ":",
                     color = "hotpink" if entry.saffir_simpson == 5 else \
-                         ("purple" if entry.saffir_simpson == 4 else \
-                         ("red" if entry.saffir_simpson == 3 else \
-                         ("orange" if entry.saffir_simpson == 2 else \
-                         ("yellow" if entry.saffir_simpson == 1 else \
-                         ("green" if entry.saffir_simpson == 0 else "black"))))),
+                         "purple" if entry.saffir_simpson == 4 else \
+                         "red" if entry.saffir_simpson == 3 else \
+                         "orange" if entry.saffir_simpson == 2 else \
+                         "yellow" if entry.saffir_simpson == 1 else \
+                         "green" if entry.saffir_simpson == 0 else \
+                         "black",
+                    marker = ".",
+                    markersize = kw.get("markersize", 3),
+                    markeredgecolor = "black",
+                    markerfacecolor = "black",
                     linewidth = kw.get("linewidth", rc["lines.linewidth"]),
+                    label = "Category {}".format(entry.saffir_simpson) \
+                        if entry.saffir_simpson > 0 and entry.status == "HU" else \
+                        "Tropical Storm" \
+                        if entry.saffir_simpson == 0 and entry.status in ["SS", "TS"] else \
+                        "Tropical Depression" \
+                        if entry.saffir_simpson < 0 and entry.status in ["SD", "TD"] else \
+                        "Non-Tropical Cyclone",
                 )
+                # Add a label to the legend if one doesn't exist already
+                if any(line2dobj_list[0].get_label() == line2dobj.get_label() for line2dobj in legend_objects) is False:
+                    legend_objects.extend(line2dobj_list)
             # from ._calculations import distance_from_coordinates
             # TS Radius
             # w = _patches.Wedge(
                 # entry.location_reversed,
                 
             # )
             # ax.fill(
@@ -660,22 +781,14 @@
                     # entry.latitude,
                     # distance_from_coordinates(*entry.location, entry.tsNE, "N")[0],
                     # distance_from_coordinates(*entry.location, entry.tsNE, "E")[0],
                 # ],
                 # zorder=10
             # )
 
-            # Status points
-            ax.plot(
-                entry.lon,
-                entry.lat,
-                "o",
-                color = "black",
-                markersize = kw.get("markersize", 2),
-            )
             if kw.get("labels", True):
                 if entry.record_identifier == "L":
                     ax.annotate(
                         "L     ",
                         (entry.lon, entry.lat),
                         fontsize = 10,
                         fontweight = "bold",
@@ -706,37 +819,59 @@
                         color = "black" if (entry.hour, entry.minute) == (0,0) \
                             else (0.5,0.5,0.5),
                         rotation = labelrot,
                         horizontalalignment = halign
                     )
         ax.grid(True, color=(0.3, 0.3, 0.3))
         ax.grid(True, which="minor", color=(0.6, 0.6, 0.6), linestyle=":")
-        # print(ax.get_ylim(), ax.get_xlim())
 
-        # Set view-limits to be equal
+        # set focus to the TC entries
+        ax.set_xlim([
+            min(en.lon for en in self.tc_entries) - 2,
+            max(en.lon for en in self.tc_entries) + 2,
+        ])
+        ax.set_ylim([
+            min(en.lat for en in self.tc_entries) - 2,
+            max(en.lat for en in self.tc_entries) + 2,
+        ])
+
+        # Set view-limits to be equal.
+        # *** THIS NEEDS TO BE DONE before maps are added. Once maps are added,
+        #     it places new limits. So to focus the end-result on the track,
+        #     the points are needed to be determined before any map is placed
+        # maxaxis == xaxis if longitudinal span >= latitudinal span, else yaxis
+
         maxaxis = ax.xaxis \
             if abs(operator.sub(*ax.get_xlim())) >= \
             abs(operator.sub(*ax.get_ylim())) else ax.yaxis
+        # multiply the span * the aspect-ratio
         maxaxis_diff = abs(operator.sub(*maxaxis.get_view_interval())) * (
             kw.get("aspect_ratio", 3/4) \
             if ax.xaxis == maxaxis \
             else (1 / kw.get("aspect_ratio", 3/4))
         )
+        # the final maxaxis interval
         maxaxis_interval = maxaxis.get_view_interval()
 
+        # minaxis == xaxis if longitudinal span < latitudinal span, else yaxis
         minaxis = ax.xaxis \
             if abs(operator.sub(*ax.get_xlim())) < \
             abs(operator.sub(*ax.get_ylim())) else ax.yaxis
         # minaxis_diff = abs(operator.sub(*minaxis.get_view_interval()))
+
+        # the final minaxis interval
+        # from the mid-point of the minaxis, add(subtract) half of the maxaxis_diff
+        # this will ensure "equidistant" nice layout of map
         minaxis_interval = [
             (statistics.mean(minaxis.get_view_interval()) + maxaxis_diff / 2),
             (statistics.mean(minaxis.get_view_interval()) - maxaxis_diff / 2)
         ]
 
         # Draw Map
+
         for atlas in [
             _maps.all_land,
             _maps.usa,
             _maps.centam,
             _maps.islands,
         ]:
             for country in atlas:
@@ -744,41 +879,30 @@
                     ax.fill(
                         [lon for lon, lat in polygon],
                         [lat for lon, lat in polygon],
                         color = kw.get("land", "lightseagreen"),
                         edgecolor = "black",
                         linewidth = 0.5,
                     )
-        # for file in [
-            # "countrydb_all_land_minus_americas.json",
-            # "countrydb_centamerica.json",
-            # "countrydb_usafull.json",
-            # "countrydb_islands.json"
-        # ]:
-            # with open(file) as r:
-                # countrydata = json.loads(r.read())
-            # for country in countrydata:
-                # for polygon in country[1:]:
-                    # ax.fill(
-                        # [lon for lon, lat in polygon],
-                        # [lat for lon, lat in polygon],
-                        # color = kw.get("land", "lightseagreen"),
-                        # edgecolor = "black",
-                        # linewidth = 0.5,
-                    # )
 
         # Reset Intervals to the TC Track
         maxaxis.set_view_interval(
             min(maxaxis_interval),
             max(maxaxis_interval),
             ignore=True
         )
         minaxis.set_view_interval(
             min(minaxis_interval),
             max(minaxis_interval),
             ignore=True
         )
 
+        # Legend
+        if kw.get("legend", True):
+            legend = plt.legend(
+                legend_objects,
+                [line2dobj.get_label() for line2dobj in legend_objects],
+                loc = "upper right",
+            )
+            legend.set_draggable(True)
+        mplstyle.use("fast")
         plt.show(block=False)
-
-def ___blah():
-    pass
```

### Comparing `hurdat2parser-2.11/hurdat2parser.egg-info/PKG-INFO` & `hurdat2parser-2.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,101 +1,159 @@
-Metadata-Version: 2.1
-Name: hurdat2parser
-Version: 2.11
-Summary: Interpret Hurricane Data contained in HURDAT2
-Home-page: http://github.com/ksgwxfan/hurdat2parser
-Author: Kyle S. Gentry
-Author-email: KyleSGentry@outlook.com
-License: MIT
-Keywords: hurricane hurdat2 meteorology weather
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# hurdat2parser -- v2.11
+# hurdat2parser -- v2.2
 ---
-### *Interpreting the HURDAT2 Tropical Cyclone Dataset using Python*
+### *Interpreting the Hurdat2 Tropical Cyclone Dataset using Python*
 
 Hurdat2 ([https://www.nhc.noaa.gov/data/#hurdat](https://www.nhc.noaa.gov/data/#hurdat)) is a collection of records from individual Tropical Cyclones. The two primary Hurdat2 records are for the Atlantic (since 1850) and East/Central-Pacific Oceans (since 1949).
 
 The purpose of this module is to provide a quick way to analyze the Hurdat2 datasets. It includes methods for retrieving, inspecting, ranking, or even exporting data for seasons, individual storms, or climatological eras.
 
-This release is primarily a "patch" in response to the newest release of the Hurdat2 database (official inclusion of data from the 2021 season). A new variable has been introduced, and this release accommodates it. But all previous versions of `hurdat2parser` will not be compatible with this and (likely) future Hurdat2 databases. But this (`2.11`) and all future versions of this program will be backward compatible to previous versions of the database.
-
 PyPI Link: [https://pypi.org/project/hurdat2parser/](https://pypi.org/project/hurdat2parser/)
 
 ## Contents
-* [Changes/Fixes in this Version (2.11)](#changes-in-this-version-211)
+* [Changes/Fixes in this Version (2.2)](#changes-in-this-version-22)
 * [Requirements, Installation, and getting the data](#installation)
 * [Importing the module](#importing-the-module)
+* [Example Calls](#example-calls)
 * [Hurdat2 Object Structure](#hurdat2-object-structure)
 * [Methods &amp; Attributes](#methods-and-attributes)
 * [Note on Landfall Data](#landfall-data)
+* [Future/Under-Development/Unreleased Methods](#access-to-future-methods)
 * [Roadmap](#roadmap)
 * [Credits](#credits)
 * [Copyright/License](#copyright)
 
-## Changes in this Version (2.11)
-- Patched to enable compatibility with the May 2022 release of the Hurdat2 database
-- Added a `TCRecordEntry` variable called `wind_radii` (the new variable included in the May 2022 Hurdat2 release. There may be some future potential in expanding the use of this variable, but its availability is currently limited to the 2021 Hurricane Season
-- Fixed calls to `TCRecordEntry` variables `avg_wind_extent_<STATUS>`
-- `info()` method for `Season` objects removed (use the `stats()` method instead)
-- modification of `<Hurdat2>.basin()`; now a method instead of property.
-- Fixed `rank_seasons_thru()` where a call without keywords (becoming a wrapper for `rank_seasons`) had an ill-advised direct call to a dictionary key instead of the get method
+## Changes in this Version (2.2)
+
+- Docstring'd `TCRecordEntry` properties
+- Changes to the `<Hurdat2>` object:
+  - when reading-in files on `__init__`, multiple local files are now supported.
+  - enabled download of the most-recent hurdat2 dataset through the `basin` kwarg.
+  - added a `urlcheck` kwarg. If `True`, the "file-path"s listed will be treated like URLs and a download attempt will be made.
+  - removed the `_filesappended` attribute
+  - Searching for notoriously-named storms can be done by a dash (`"-"`) prefix to the search string in addition to an underscore (see [Example Calls](#example-calls) section)
+  - Revamped `output_climo_csv`, `output_season_csv`, and `output_storms_csv` methods
+    - simplified code; updated and unified attributes used in the reports and made it significantly easier for future maintenance.
+  - moved `multi_season_info` method to `_reports`
+- New properties for both `Season` and `TropicalCyclone`:
+  - `duration`
+    - `Season` version reports time between the first and last day of the season (see further in the document for explanation)
+	- `TropicalCyclone` version just reports the track-life in days, regardless of status. More useful status-based duration properties were created too. Keep reading (a few lines down).
+  - `tc_entries` returns a list of `TCRecordEntry`s where a storm was a designated tropical cyclone.
+  - `start_date`, `start_ordinal`, and `end_date`, `end_ordinal` report the starting/ending dates and/or days of the year
+- New `TropicalCyclone` variables:
+  - `ACE_no_landfall`
+  - `duration_<TC, TS, HU, MHU>` - These properties report the aggregate time in days that a tropical cyclone was designated that status or stronger, accounting for fluxuations in storm statuses and strengths.
+  - removed `coord_list` method. It was redundant as it was like a shortened combination of the `summary` method.
+- New `TCRecordEntry` variables:
+  - tweaked how location variables are defined. `location` and `location_reversed` are now properties that depend on the express definition of the variables `lat` and `lon` rather than the other way around.
+  - tweak of not-available wind-extent data. As of the moment typing this, wind-extent data is only provided for storms since 2004. All previous wind-extent data is `-999`, meaning its unavailable. But if a storm has max winds of `<` 64, its Hurricane wind extent has to be 0. So when ingesting the data, this determination is made.
+  - tweaked ingest of data to prevent errors due to possible new Hurdat2 categories introduced in future versions. This was the problem with `v2.1` that was responsible for the need for a `v2.11` release. This particular version wouldn't be able to read-in the new variables in such a situation, but it would still be functional with the newer database (unless order of variables are switched around).
+  - the formerly-called variable `wind_radii` from `v2.11` is now called `maxwind_radius`. I don't know why I called it `radii`, as in plural of radius. I guess it sounded science-y or smart. haha. But the change is also more readable.
+  - Surface Area (coverage)-based variables `areal_extent_TS`, `areal_extent_TS50`, and `areal_extent_HU`.
+    - These are calculated from reported wind-extents in the database.
+  - `track_distance`: the track distance of the cyclone up to the point of the respective entry; this does not account for storm status
+  - `previous_entries` and `next_entries`: lists of the previous and next recorded entries, respectively, in the `TropicalCyclone`'s record
+  - `previous_entry` and `next_entry`: the previous and next recorded entry, respectively, in the `TropicalCyclone`'s record
+  - `direction()`: the `TropicalCyclone`'s heading in degrees (or cardinal, if desired...see docstring)
+  - `speed`: the `TropicalCyclone`'s forward speed in knots.
+  - Properties to simplify coding and reduce probability of coding errors.
+    - `is_TC`: `bool` indicating whether or not a storm was designated as a tropical cyclone at the `<TCRecordEntry>.entrytime`.
+    - `is_synoptic`: `bool` indicating whether or not an entry occurred at a synoptic time (0Z, 6Z, 12Z, 18Z).
+- Added `report_type` default keyword argument to the `<Season>.stats` method. User can dictate if report prints to the console or gets back a string version of the report.
+- Fixed an exclusion of `maxwind_radius` (formerly called `wind_radii`) from `<TCRecordEntry>.hurdat2()` calls. (which was only introduced in the previous version).
+- Tweaked landfall-disclaimer in `<Season>.stats()` output to reflect the April 2022 release of the Hurdat2 database.
+- Changed `<Season>.__getitem__` method to account for the possibility of merged basin databases, giving the user a choice between mulitple storms that occurred in the same year, but in different geographical basins with shared cyclone numbers. The East Pacific Hurdat2 is an example, natively including storms from the East and Central Pacific Basins.
+- `<TropicalCyclone>.track_map()` tweaks:
+  - focuses on the part of the track where the storm was designated a tropical cyclone.
+  - now fills more of the screen, offering a better user experience, and lessens the likelihood of the user feeling compelled to resize the initial window.
+  - added legend. By default, it will display. But if you'd rather it not display, there is a keyword to turn it off
+  - I believe it may be slightly faster now, thanks to performance tips in matplotlib docs.
+  - map coordinate lists used now significantly smaller.
+- tweaked a very minor syntax quirk. Somewhere in the code I had used `is not` instead of the more-proper `!=`.
+- `basin` tweaks
+  - introduced a new method `<Hurdat2>.basin_abbr()` which returns a list of basin abbreviations used; will be used in report outputs.
+- Fixed memory-location identification in `__repr__` methods
 
 [&#8679; back to Contents](#contents)
 
 ## Installation
 
 - At the command prompt, run `pip install hurdat2parser`
-  - When installing, packages `pyshp` and `geojson` and `matplotlib` will be downloaded as dependencies (if necessary).
-- You'll then need the actual Hurdat2 Data. You can get it [HERE](https://www.nhc.noaa.gov/data/#hurdat). It's just a text file. Hurdat2 files for the Atlantic Basin and East/Central Pacific Basins are available and compatible with the package.
+  - When installing, packages `pyshp`, `geojson`, and `matplotlib` will be downloaded as dependencies (if necessary). From scratch, it's around 30MB total of dependency downloads.
 
 [&#8679; back to Contents](#contents)
 
 ## Importing the Module
 
-- Import the module and invoke a call to the `Hurdat2` class while passing the file-name of the Hurdat2 dataset
+Follow these commands for genesis!
 
 ```python
 >>> import hurdat2parser
->>> atl = hurdat2parser.Hurdat2("path_to_hurdat2.txt")
+#or if you're lazy like me...
+>>> import hurdat2parser as hd2
 ```
-- * For the `Hurdat2` object, I highly recommend to use something shortened and readable for the parent object name (like `atl` or `al` for the Atlantic database and `ep`, `cp`, or `pac` for the East/Central Pacific)*
 
-After a few seconds you'll be ready to dive into the data! Subsequent examples imply the use of the Atlantic Hurdat2.
+- If you want a local copy of a hurdat2file, got to [https://www.nhc.noaa.gov/data/#hurdat](https://www.nhc.noaa.gov/data/#hurdat) to download. It's a text file. Hurdat2 files for the Atlantic Basin and East/Central Pacific Basins are available and compatible with the package. 
+  - As of `v2.2` this isn't 100% necessary as the datasets can be automatic retrieval can be attempted (keep reading). This method does not keep a local copy though (as of this version).
+
+To read-in a local file:<br/>`>>> atl = hurdat2parser.Hurdat2("path_to_hurdat2.txt")`
+
+And/Or to let the module download and ingest the data for you:
+
+- North Atlantic Basin<br/>`>>> atl = hurdat2parser.Hurdat2(basin="atl")`
+  - Any of the following will be recognized: `"al"`, `"atl"`, or `"atlantic"`
+- NE/CEN Pacific Basin<br/>`>>> pac = hurdat2parser.Hurdat2(basin="pac")`
+  - Any of the following will be recognized: `"pac"`, `"nepac"`, or `"pacific"`
+- Of note, the above commands do not keep a local copy for next time
+
+To include a url to download, set the kwarg `urlcheck` to `True`. This generally will not be needed unless you want to use my (shameless plug) daily-updated current-season hurdat2 during the year (on my website; see [Copyright](#copyright) section)<br/>
+`>>> atl = hurdat2parser.Hurdat2("http://crazygonuts.aboutweatherstuff/myhurdat2file.txt", urlcheck=True)`
+
+These various ways can be mixed/matched too.
+
+* For the `Hurdat2` object, I highly recommend to use something shortened and readable for the parent object name (like `atl` or `al` for the Atlantic database and `ep`, `cp`, or `pac` for the East/Central Pacific)*
+
+After a few seconds (a little longer if downloading) you'll be ready to dive into the data! Subsequent examples imply the use of the Atlantic Hurdat2 (`atl`).
+
+[&#8679; back to Contents](#contents)
+
+## Example calls
+
+There are several ways to invoke a call to a `Season` or `TropicalCyclone` object. These ways are detailed in the [next section](#hurdat2-object-structure), indirectly in the [Methods and Attribute](#methods-and-attributes) tables, and in a large portion of method docstrings. This brief section will demonstrate the ways I navigate the dataset with this module when coding and testing.
+
+- `Season` objects (just the year)
+  - `atl[1995]`
+- `TropicalCyclone` objects
+  - by atcfid number
+    - `atl[2005,12]` -- returns the object for hurricane katrina (`AL200512`)
+  - by name
+    - `atl["danny"]` -- shows a list of storms in the record given the name of Danny, allowing the user to select which one they desire
+    - `atl["_rita"]`, or `atl["-rita"]` -- beginning the name with an underscore or dash shows the most-recent storm named as such (this returns the most-notorious storms as well since storm names can be retired according to the destruction they cause)
+- `TCRecordEntry` calls
+  - `atl[1980,4,29]` -- The entry at index 29 (30th total entry) for Hurricane Allen
+  - or `atl["_allen", 29]`
 
 [&#8679; back to Contents](#contents)
 
 ## Hurdat2 Object Structure
 
 - The structure of a `Hurdat2` object is hierarchal. It has two primary dictionaries:
   - `<Hurdat2>.tc` - A dictionary containing all `TropicalCyclone` objects compiled from the record.
     - Individual storms can be accessed using their ATCF ID, a unique 8-character id for each tropical cyclone <u>OR</u> a name of a storm.
 	  - `atl["AL122005"]` - Call for Hurricane Katrina's Data using its ATCFID (it being the 12th storm from the 2005 Atlantic Season).
 	  - `atl["Name"]` - Use this if you know the name, but the year is unknown. A partial search is okay, but may receive less accurate results. It uses the `difflib` package to calculate close matches and outputs a list (if applicable) that you then can select from.
-	  - `atl["_Name"]` - including an underscore at the beginning of the name will return the **NEWEST** storm by a name that matches. Use this for the most-notoroious storms (as it would return the last-so-named storm, retired names included).
+	  - `atl["_Name"]` or `atl["-Name"]` - including an underscore or dash at the beginning of the name will return the **NEWEST** storm by a name that matches. Use this for the most-notorious storms, as retired names would be the newest.
   - `<Hurdat2>.season` - A dictionary holding `Season` objects (yearly data).
     - A Season's data is accessed via a simple year key of type `int`.
 	  - `atl[1995]` retrieves the object associated with the 1995 hurricane season.
-- `Season` objects also have a dictionary (`<Season>.tc`) that holds `TropicalCyclone` objects, specific to the year.
-  - There are 4 different ways to access individual storm data:
-    1. `atl[1995]["Opal"]` - Storm Name; Useful if you know the name a storm was issued and the season in which it occurred.
-    2. `atl[1992]["A"]` - Storm Name first-letter; I'm not saying you'd forget a named-storm like Hurricane Andrew, but this capability would grab the storm whose first-letter matched the one passed. This primarily works for modern storms (since the beginning of the satellite era), as most in the past were not named. In the Hurdat2 record, storms that were never issued a name are given "UNNAMED" for that field.
-    3. TC Number: `atl[1988][8]` - Use the storm number (type `int`) from the season. This is defined by using the ATCF ID.
-	  - This would be faster (less keystrokes): `atl[2005, 12]` - retrieves Hurricane Katrina
-    4. ATCF ID: `atl[1980]["AL041980"]` - This isn't recommended because of redundancy (it can be done without the initial call to the `1980` object).
-- `TropicalCyclone` objects contain a `list` of `TCRecordEntry` objects in time-ascending order.
-  - Though the user probably wouldn't have general/typical need to access `TCRecordEntry`-level data, it can be done via the desired index from the `<TropicalCyclone>.entry` list:
-    - `atl[2004]["ivan"][0]` - This would grab the first entry associated with the track of Hurricane Ivan.
-    - This would be faster: `atl[2005, 12, 21]` - the 22nd entry of Hurricane Katrina
+- `Season` objects also have a dictionary (`<Season>.tc`) that holds `TropicalCyclone` objects, specific to the year. Some different ways to call these objects:
+  - TC Number: `atl[1988,8]` or `atl[1988][8]` - Use the storm number (type `int`) from the season. This is defined by using the ATCF ID.
+  - Storm starting letter (or name): `atl[1995, "o"]` or `atl[1995, "opal"]` or `atl[1995]["Opal"]` - This method works for most modern tropical storms, as they have been issued names. So in these cases, you wouldn't need to know the atcfid number. Also of note, because tropical depressions aren't issued names, the id numbers do not always correlate with the co-inciding letter of the alphabet. For example, Hurricane Andrew's ATCFID is `AL041992`.
+- `TropicalCyclone` objects contain a `list` of `TCRecordEntry` objects in time-ascending order. To access these:
+  - `atl[2005, 12, 21]` would grab the `TCRecordEntry` for Hurricane Katrina at index 21.
 
 [&#8679; back to Contents](#contents)
 
 ## Methods and Attributes
 
 Now that you know how to call a particular object of interest, you can now access its data, using methods and attributes. The docstrings (accessed via `help()`) are quite detailed and methods that take arguments have example calls listed. But here is a quick reference to what is available, along with some shortcuts and example calls to assist navigating while in this document.
 
@@ -114,17 +172,18 @@
 `rank_climo(...)` | Yet another useful ranking method. This allows one to rank attributes assessed over several to many years (climatological periods) to one another. Optional keyword argument `climatology` (default is 30 years) controls the span of time that data is collected and `increment` (default is 5 years) dictates the temporal distance between periods | `atl.rank_climo(20,"track_distance_TC", climatology=10, increment=1)`
 `rank_storms(...)` | Print a report that compares storms and their attributes to each other. Similar to the above methods, other data is included in the report. See the docstring for info on `coordextent` kw usage | `atl.rank_storms(20,"HDP",1967)`
 `multi_season_info(...)` | Prints a report a gathered statistics based on a range of years. This is similar to the `info()` methods referenced in the next section. This could be thought of as an info method for a climatological period | `atl.multi_season_info(1991, 2000)`<br />`atl[2010, 2019]`
 `storm_name_search(...)` | Search through the entire Hurdat2 record for storms issued a name. If the positional keyword `info` is `True`, the matching storm's info method will print. | `atl.storm_name_search("Hugo")`
 `output_climo(...)` | outputs a .csv file using the `csv` package of 1-year incremented climatological periods. This csv file can then be opened in a spreadsheet program. To compare or rank, the spreadsheet GUI layout is much easier to use especially due to instant sorting and filtering. This accepts a positional keyword argument (`climatology=30`). | `atl.output_climo(15)`
 `output_seasons_csv(...)` | Similar to the above, but for seasons. It takes no arguments. In other words, it would be redundant to run it multiple times, because as the `hurdat2parser` package doesn't natively allow modification of the data, it would just output the same data over and over. The only exception would be when the Hurdat2 database is updated by the NHC. With this in mind, it will automatically write-over the csv if it already exists (file-name is auto-generated within the method). | `atl.output_seasons_csv()`
 `output_storms_csv(...)` | Similar to above, but for individual storms. | `atl.output_storms_csv()`
+`climograph()` | displays a graph of the climatological tendency of a variable over multiple seasons (see docstring for a how-to) | `atl.climograph("ACE", 10, 1, year1=1967)`
 `coord_contains(...)` | Takes 3 tupled lat-lon coordinates. The purpose is to inquire whether the first arg (the test coordinate) is contained within a bounding box formed by the other two coordinates passed (returns a `bool`. This is generally just accessed via the ranking methods | `atl.coord_contains(`<br />&nbsp;&nbsp;&nbsp;&nbsp;`[30.4,-85.0]`,<br />&nbsp;&nbsp;&nbsp;&nbsp;`[31.5, 86.0],`<br />&nbsp;&nbsp;&nbsp;&nbsp;`[29.0, 84.0]`<br />`) -> True`
-`BASIN_DICT` | A dictionary containing abbreviations (keys) and definitions (values) of various basins around the world that hurricane data is kept. This is referenced via the `basin()` method. The data used to form this object came from IBTrACS | `<Hurdat2>.BASIN_DICT`
-`basin(season=None)` | Interprets and returns a readable string identifying the TC basin based on the storms within the record. This allows support of dynamically-created singular OR multiple Hurdat2 datasets OR individual seasons (if a `Season` object is passed to the method). | `atl.basin -> "North Atlantic Basin"
+`BASIN_DICT` | A dictionary containing abbreviations (keys) and definitions (values) of various basins around the world that hurricane data is kept. This is referenced via the `basin()` method. The data used to form this object came from IBTrACS | `atl.BASIN_DICT`
+`basin(season=None)` | Interprets and returns a readable string identifying the TC basin based on the storms within the record. This allows support of dynamically-created singular OR multiple Hurdat2 datasets OR individual seasons (if a `Season` object is passed to the method). The data used to form this property came from IBTrACS | `atl.basin() -> "North Atlantic Basin"
 `record_range` | Returns a tuple of the beginning year and end year of the Hurdat2 record | `atl.record_range -> (1851, 2020)`
 
 [&#8679; back to Methods &amp; Attributes](#methods-and-attributes)
 
 #### Shared Methods and Attributes for `Season` and `TropicalCyclone`
 
 Attributes | Description | Examples
@@ -135,97 +194,132 @@
 `landfalls`<br /> | \*SEE [DISCLAIMER FOR LANDFALL INFO](#landfall-data)\* Sum of all landfalls (remember, a storm can make multiple landfalls). `<Season>.landfalls` is also an unfiltered aggregate of its storms landfalls. At the seasonal level, you'd probably be more interested in the attribute `landfall_TC` (see following section) | `atl[1960]["doNnA"].landfalls`
 `landfall_<STATUS>`<br />*\-can be TC, TD, TS, HU, or MHU* | `Season`: qty of TC's that made landfall as the inquired status; `TropicalCyclone`: `bool` indicating if the storm made landfall while the inquired status<br />*\-CAUTION: These attrs are exclusive of landfalls made while of stronger designation\-* | `atl[1996].landfall_TS -> 2`<br />`atl[2011]["I"].landfall_HU -> True`
 `<STATUS>reach`<br />*\-can be TC, TD, TS, HU, or MHU* | `Season`: qty of TC's that reached <u>at least</u> the inquired status; `TropicalCyclone`: `bool` indicating if the storm ever was designated as the inquired status | `atl[2010].HUreach -> 12`<br />`atl[1991]["danny"].HUreach -> False`
 `ACE`, `HDP`, or `MHDP` | Returns the specified Energy Index reading associated with the season or storm. Note that the MHDP is one you likely won't see elsewhere. It's formula is the same as ACE and HDP but for major-hurricanes only | `atl[1966].HDP`
 `track_distance` | The calculated distance (in nmi) for the entire track of the storm (or aggregate of the season), regardless of status | `atl[1954]["hazel"].track_distance`
 `track_distance_<STATUS>`<br>*\-can be TC, TD, TS, HU, or MHU* | The distance traversed while storm(s) was(were) <u>at least</u> the status designation | `atl[1961].track_distance_MHU`
 `cat45reach`<br>`cat5reach` | For `Season` objects, returns the quantity of storms that reached category 4+ status or category 5 status (respectively)<br>For `TropicalCyclone` objects, returns a `bool`, indicating if the TC ever achieved cat 4+ or 5 status (respectively) | `atl[2020].cat45reach -> 5`<br>`atl[2020].cat5reach -> 0`<br>`atl[2020]["Iota"].cat5reach -> False`
-`maxwind_mslp`<br>`minmslp_wind` | Returns the MSLP (wind) occurring at the time of peak-winds (minimum MSLP) respectively. These attributes were included because peak winds and minimum MSLP do not necessarily occur at the same time. | `atl[2015]["joaquin"].maxwind_mslp -> 934`<br>`atl[2015]["joaquin"].minmslp_wind -> 120`<br>\* This example was given as Joaquin's peak winds (135) were not observed at the time of Joaquin's minimum MSLP (931)
 `hurdat2()` | This method prints a hurdat2-formatted output of the storms's data, emulating the actual hurdat2 record from which it (the Season or Tropical Cyclone) was created | `atl[2005].hurdat2()`
+`duration` | Returns the length of the Season or life of the cyclone (Of note, the `TropicalCyclone` property disregards storm status) | `atl[2022].duration`
+`tc_entries` | Returns a list of `TCRecordEntry`'s from where a storm was designated as a tropical cyclone | `atl["_katrina"].tc_entries`
+`start_date` | The beginning moment of the Season or storm | `atl[1938].start_date`
+`start_ordinal` | The quantified day of the year of the beginning moment of the Season or storm | `atl[1938].start_ordinal`
+`end_date` | The ending date of the Season or storm | `atl[1954, 16].end_date`
+`end_ordinal` | The quantified day of the year of the ending date of the Season or storm | `atl[1954].end_ordinal`
 
 [&#8679; back to Methods &amp; Attributes](#methods-and-attributes)
 
 #### `Season` Only Methods and Attributes
 Attribute | Description | Example
 :---: | :---: | :---:
 `output_shp_segmented()` | Generates a shapefile including each segment from each tropical-cyclone from a given season; each individual segment from each individual storm will be represented | `atl[1932].output_shp_segmented()`
 `output_geojson_segmented()` | Generates a geojson including each segment from each tropical-cyclone from a given season; each individual segment from each individual storm will be representeds | `atl[2003].output_geojson_segmented()`
 `tracks` | Returns the quantity of tropical cyclones from a season | `atl[1995].tracks`
 `<STATUS>only`<br />*\-can be TD, TS, or HU* | Returns the quantity of TC's from a season that made were given the inquired designation, but never strengthened beyond it. `HUonly` implies Category 1 and 2 storms only. To inquire about `MHU`, use the `MHUreach` attr | `atl[1950].TDonly`<br />`atl[2017].HUonly`
-`stats()` | prints a report filled with statistics and ranks for the season, optionally compared with a subset of seasons and/or partial seasons. For `TropicalCyclones`, this is a mirror-method of `.info()` | `atl[2020].stats()`<br>`atl[2005].stats(thru=(9,30))`<br>`atl[1989]["hugo"].stats()
+`stats()` | prints a report filled with statistics and ranks for the season, optionally compared with a subset of seasons and/or partial seasons. Though it technically exists as a  `TropicalCyclone` method, its iteration is a mirror-method of `.info()` | `atl[2020].stats()`<br>`atl[2005].stats(thru=(9,30))`
 
 [&#8679; back to Methods &amp; Attributes](#methods-and-attributes)
 
 #### `TropicalCyclone` Only Methods and Attributes
 | Attribute | Description | Example
 :---: | :---: | :---:
-`coord_list()` | Prints a report with entry dates and the associated Latitude and Longitude | `atl[2005]["rita"].coord_list()`
-`gps` | Returns a `list` of tupled latitude and Longitude coordinates | `atl[1998]["MITCH"].coord_list()`
+`gps` | Returns a `list` of tupled latitude and Longitude coordinates | `atl[1998]["MITCH"].gps`
+`maxwind` | Returns the highest maximum sustained wind-speed observed in the tropical cyclone | `atl["_katrina"].maxwind`
 `minmslp` | Returns the lowest recorded pressure of the TC | `atl[1955][10].minmslp`
+`maxwind_mslp`<br>`minmslp_wind` | Returns the MSLP (wind) occurring at the time of peak-winds (minimum MSLP) respectively. These attributes were included because peak winds and minimum MSLP do not necessarily occur at the same time. | `atl[2015]["joaquin"].maxwind_mslp -> 934`<br>`atl[2015]["joaquin"].minmslp_wind -> 120`<br>\* This example was given as Joaquin's peak winds (135) were not observed at the time of Joaquin's minimum MSLP (931)
 `<EI>_per_nmi`<br />*\-can be ACE, HDP, or MHDP* | Returns the inquired energy index divided by the track distance covered while the energy index was being contributed to (`ACE` &rarr; `track_distance_TS` or `HDP` &rarr; `track_distance_HU` as examples). WARNING! These attributes do not have any kind of threshold controls, so storms which were short-lived can have high values | `atl[1964][10].HDP_per_nmi`<br />`atl[2016]["matthew"].ACE_per_nmi`
 `<EI>_perc_ACE` &rarr; *\-can be HDP or MHDP*<br />`HDP_perc_MHDP` | Simply the storm's HDP or MHDP divided by ACE or the MHDP divided by the HDP. Look at this as the <u>percentage</u> (as a float between 0 and 1) of the storm's ACE or HDP that was contributed to while a Hurricane or Major Hurricane, respectively | `atl[2017]["IRMA"].HDP_perc_ACE`
 `track_<EI1>_perc_<EI2>`<br />*\-&lt;EI1&gt; can be TS, HU, or MHU*<br />*\-&lt;EI2&gt; can be TC, TS, HU, or MHU* | Returns the the storm's &lt;EI2&gt; track_distance divided by the track distance while of status &lt;EI1&gt;. &lt;EI1&gt; must be of higher hierarchal status than &lt;EI2&gt; | `atl[2005][25].track_HU_perc_TC`<br />`atl[2003]["Fabian"].track_MHU_perc_TS`
 `track_map()` | Generates a map of the storm's track using `matplotlib`. Check the docstring for ways to modify the output to your liking. | `atl["_katrina"].track_map()`
 `perc_ACE`<br>`perc_HDP`<br>`perc_MHDP` | Return the percentage (in decimal form) of the contribution of the storm's ACE, HDP, or MHDP value to the season's value | `atl["_matthew"].perc_MHDP
-`info()` | Prints basic stats for the tropical cyclone | `atl[1989]["hugo"].info()`
+`info()` | Prints basic stats for the tropical cyclone | `atl[2005][12].info()`
+`ACE_no_landfall` | Returns the ACE of the storm prior to any landfall made | `atl["_ivan"].ACE_no_landfall
+`duration_<SUFFIX>`<br />*\*&lt;SUFFIX&gt; can be TC, TS, HU, MHU* | Returns the aggregated length in days that the cyclone spent as on of the given statuses. These do account for storm status loss and possible reaquisition | `atl["_irma"].duration_MHU`
 
 [&#8679; back to Methods &amp; Attributes](#methods-and-attributes)
 
 #### `TCRecordEntry` Attributes
 
-- As mentioned earlier, there's generally no need to access`TCRecordEntry` objects directly. Only the most-common attributes will be referenced in this document. A comprehensive list is available via `help`
+- Only the most-common attributes will be referenced in this document. A comprehensive list is available via `help`
 
 | Attribute | Description
 :---: | :---:
 `entrytime` | A `datetime.datetime` object of the entry's timestamp
 `status` | The designated 2-letter abbreviation representing the storm's status
 `location`<br />`location_rev` | A tuple of the latitude/longitude coordinates; `location_rev` is reversed in order, a longitude/latitude tuple; seemingly favored for GIS use.
 `wind` | The maximum-sustained winds at the time of entry-recording
 `mslp` | The Mean Sea-Level Pressure (in hPa or mb) at the time of entry-recording
 `hurdat2()` | Returns a reassembled Hurdat2-formatted string, identical to the one parsed to create the entry
-`wind_radii` | The Radius of Maximum Winds. *As of the May 2022 release of the Hurdat2 database, this is a new variable and the availability of it belongs solely to the 2021 Hurricane season (for now).*
+`maxwind_radius` | The Radius of Maximum Winds. Currently, it is only available for storms since 2021, and is assumed that in subsequent releases, this variable will continue to be updated. It is unknown if this data for previous seasons will (or can) be back-filled.
+`avg_wind_extent_<SUFFIX>`<br/>Suffix can be `TS`, `TS50`, or `HU` | The statistical mean of the reported wind-extents (quadrants). Wind extents are only available for storms since 2004 
+`areal_extent_<SUFFIX>`<br/>Suffix can be `TS`, `TS50`, or `HU` | The calculated area covered by the extent of winds of specified strengths (of note, wind extents are only available for storms since 2004)
+`track_distance`<br/>`track_distance_<SUFFIX>`<br/>Suffix can be `TC`, `TS`, `HU`, or `MHU` | returns the distance tracked by the system from its genesist to the point of the entry. The variables with suffixes do account for status in their calculations
+`previous_entry`<br/>`next_entry` | Returns the entry prior-to or after the `TCRecordEntry` that it is called from
+`direction()` | Returns the heading in degrees that the storm is going. A readable cardinal direction can be returned if `True` is passed to the method
+`speed` | The average speed between the previous entry and this one in nm/h<br/>Of Note, remember that the `Hurdat2` spatial resolution is 0.1 degrees latitude/longitude. So some appreciable error may be present
 
 [&#8679; back to Methods &amp; Attributes](#methods-and-attributes)<br />
 [&#8679; back to Contents](#contents)
 
 ## Landfall Data
 
 An important point to keep in mind when viewing data and ranking, Hurdat2's landfall data is incomplete. It is progressively being updated in conjunction with the yearly release of the dataset. Please see the documentation  [Hurdat2 Format Guide](https://www.nhc.noaa.gov/data/hurdat/hurdat2-format-atl-1851-2021.pdf) for more detail on currently-available landfall data temporal scope.
 
 [&#8679; back to Contents](#contents)
 
+## Access to Future Methods
+
+In `_future.py`, I have some stuff that I've started to develop but not ready/sure to release. The methods are functional though. The quickest way of accessing it is:
+
+```python
+>>> import hurdat2parser._future as future
+```
+
+Valid classes reflect those of the main `hurdat2parser` object, namely `future.Hurdat2`, `future.Season`, `future.TropicalCyclone`, or `future.TCRecordEntry`. They'll be empty if I don't have anything I'm currently developing for that respective class/object. You can see what methods I have available by running `dir()` on the class.
+
+When calling, you will need to manually pass a valid object (a substitute for `self`). For example:
+```python
+>>> future.Season.track_map(atl[1984])
+```
+
+[&#8679; back to Contents](#contents)
+
 ## Roadmap
 
+- [ ] Include more `Season.duration`-related properties based on status
 - [ ] Speed-up `<Season>.stats()` report; because it employs `rank_seasons_thru`, and since that is quite snappy, I think the `stats()` method should be quick too. I'll investigate.
-- [ ] Include a `track_map()` method for `Season`
-- [ ] Include legends for `<TropicalCyclone>.track_map()`
+- [ ] Develop matplotlib-based graphs located in `_future`
 - [ ] Comparison methods to directly compare one season to another or specific storms to another.
-- [ ] Formulate a `stats()` method for `TropicalCyclone`s (to eventually replace their `info` method); including ranking/comparing to storms across the record or a subset of seasons, including a `rank_storms_thru()` companion method for `Hurdat2` objects.
+- [ ] Revamp `hurdat2()` method of `TropicalCyclone` and `Season` objects to optionally return a string instead of merely printing to console
+- [ ] Formulate a `stats()` method for `TropicalCyclone`s (to eventually replace their `info` method); including ranking/comparing to storms across the record or a subset of seasons (right now, this method is just a wrapper for the `info()` method.
 - [ ] Track distance percentage of season total for `TropicalCyclone`s
 - [ ] Maybe simpler rank methods so values sought for ranking will guarantee to show
-- [X] Deprecate `<Season>.info()` method
-- [x] Inclusion of `matplotlib` methods
+- [ ] add maps files for Pacific-centric storms
+- [ ] investigate adding a minmslp_entry or maxwind_entry property for TropicalCyclone objects. It is acknowledged though that multiple entries can have the same minimum mslp or max wind.
+- [ ] a `genesis` property, returning the first entry from a `TropicalCyclone` earning the TC designation. Not sure the feasability of this. I'll think about it.
+- [x] Include legends for `<TropicalCyclone>.track_map()`
+- [x] Account for absent season starts when using stats thru certain time
 
 [&#8679; back to Contents](#contents)
 
 ## Credits
 
-- Hurdat Reference: `Landsea, C. W. and J. L. Franklin, 2013: Atlantic Hurricane Database Uncertainty and Presentation of a New Database Format. Mon. Wea. Rev., 141, 3576-3592.`
+- HURDAT Reference: `Landsea, C. W. and J. L. Franklin, 2013: Atlantic Hurricane Database Uncertainty and Presentation of a New Database Format. Mon. Wea. Rev., 141, 3576-3592.`
 - [Haversine Formula (via Wikipedia)](https://en.wikipedia.org/wiki/Haversine_formula)
 - Bell, et. al. Climate Assessment for 1999. *Bulletin of the American Meteorological Society.* Vol 81, No. 6. June 2000. S19.
 - <span>G. Bell, M. Chelliah.</span> *Journal of Climate.* Vol. 19, Issue 4. pg 593. 15 February 2006.
 - [Hurdat2 Format Guide (PDF)](https://www.nhc.noaa.gov/data/hurdat/hurdat2-format-atl-1851-2021.pdf)
 - [Natural Earth](https://www.naturalearthdata.com/) GIS Data (data extracted there-from to display maps)
 
 [&#8679; back to Contents](#contents)
 
 ## Copyright
 
 **Author**: Kyle S. Gentry<br />
-Copyright &copy; 2019-2022, Kyle Gentry (KyleSGentry@outlook.com)<br />
+Copyright &copy; 2019-2023, Kyle Gentry (KyleSGentry@outlook.com)<br />
 **License**: MIT<br />
 **GitHub**: [https://github.com/ksgwxfan/hurdat2parser](https://github.com/ksgwxfan/hurdat2parser)<br />
 **Author's Webpages**:
  - [https://ksgwxfan.github.io/](https://ksgwxfan.github.io/)<br />
  - [http://echotops.blogspot.com/](http://echotops.blogspot.com/)
 
 [&#8679; back to Contents](#contents)
```

### Comparing `hurdat2parser-2.11/setup.py` & `hurdat2parser-2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
  
 with open("README.md", "r") as fh: 
     readme = fh.read() 
 
 setup(
     name = 'hurdat2parser',
-    version = '2.11',
+    version = '2.2',
     author = 'Kyle S. Gentry',
     author_email = 'KyleSGentry@outlook.com',
     url = 'http://github.com/ksgwxfan/hurdat2parser',
     description = 'Interpret Hurricane Data contained in HURDAT2',
     long_description = readme,
     long_description_content_type = "text/markdown",
     license = 'MIT',
```

