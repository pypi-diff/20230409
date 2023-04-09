# Comparing `tmp/synth_mapping_helper-1.0.2.tar.gz` & `tmp/synth_mapping_helper-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synth_mapping_helper-1.0.2.tar", last modified: Sun Apr  2 19:58:42 2023, max compression
+gzip compressed data, was "synth_mapping_helper-1.1.0.tar", last modified: Sun Apr  9 17:16:00 2023, max compression
```

## Comparing `synth_mapping_helper-1.0.2.tar` & `synth_mapping_helper-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 19:58:42.180944 synth_mapping_helper-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-02 19:58:27.000000 synth_mapping_helper-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-02 19:58:27.000000 synth_mapping_helper-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-02 19:58:42.180944 synth_mapping_helper-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-02 19:58:27.000000 synth_mapping_helper-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-02 19:58:27.000000 synth_mapping_helper-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-02 19:58:42.180944 synth_mapping_helper-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-02 19:58:27.000000 synth_mapping_helper-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 19:58:42.176944 synth_mapping_helper-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 19:58:42.180944 synth_mapping_helper-1.0.2/src/synth_mapping_helper/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-02 19:58:27.000000 synth_mapping_helper-1.0.2/src/synth_mapping_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22578 2023-04-02 19:58:27.000000 synth_mapping_helper-1.0.2/src/synth_mapping_helper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    26636 2023-04-02 19:58:27.000000 synth_mapping_helper-1.0.2/src/synth_mapping_helper/companion.py
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-04-02 19:58:27.000000 synth_mapping_helper-1.0.2/src/synth_mapping_helper/finalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-04-02 19:58:27.000000 synth_mapping_helper-1.0.2/src/synth_mapping_helper/movement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-02 19:58:27.000000 synth_mapping_helper-1.0.2/src/synth_mapping_helper/pattern_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9036 2023-04-02 19:58:27.000000 synth_mapping_helper-1.0.2/src/synth_mapping_helper/rails.py
--rw-r--r--   0 runner    (1001) docker     (123)    15741 2023-04-02 19:58:27.000000 synth_mapping_helper-1.0.2/src/synth_mapping_helper/synth_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-02 19:58:27.000000 synth_mapping_helper-1.0.2/src/synth_mapping_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 19:58:42.180944 synth_mapping_helper-1.0.2/src/synth_mapping_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-02 19:58:42.000000 synth_mapping_helper-1.0.2/src/synth_mapping_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-02 19:58:42.000000 synth_mapping_helper-1.0.2/src/synth_mapping_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 19:58:42.000000 synth_mapping_helper-1.0.2/src/synth_mapping_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-02 19:58:42.000000 synth_mapping_helper-1.0.2/src/synth_mapping_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-02 19:58:42.000000 synth_mapping_helper-1.0.2/src/synth_mapping_helper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 19:58:42.180944 synth_mapping_helper-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-02 19:58:27.000000 synth_mapping_helper-1.0.2/tests/test_synth_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:16:00.862068 synth_mapping_helper-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-09 17:16:00.862068 synth_mapping_helper-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 17:16:00.862068 synth_mapping_helper-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:16:00.862068 synth_mapping_helper-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:16:00.862068 synth_mapping_helper-1.1.0/src/synth_mapping_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25631 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26636 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper/companion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper/movement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper/pattern_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper/rails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper/synth_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:16:00.862068 synth_mapping_helper-1.1.0/src/synth_mapping_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-09 17:16:00.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-09 17:16:00.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:16:00.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-09 17:16:00.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-09 17:16:00.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:16:00.862068 synth_mapping_helper-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/tests/test_synth_format.py
```

### Comparing `synth_mapping_helper-1.0.2/LICENSE` & `synth_mapping_helper-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.0.2/PKG-INFO` & `synth_mapping_helper-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth_mapping_helper
-Version: 1.0.2
+Version: 1.1.0
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Home-page: https://github.com/adosikas/synth_mapping_helper
 Author: adosikas
 Author-email: 
 Project-URL: Documentation, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Bug Reports, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Source Code, https://github.com/adosikas/synth_mapping_helper
@@ -65,15 +65,15 @@
     * **Automatic backups** while mapping
     * Plot notes to spot outliers
     * View hand velocity and acceleration to find sections to smooth out
     * Show wall density and estimatation which ones will not render on quest
     * Fix **wall offset** between editor and game ("Finalize")
 
 ### Maybe (contributions welcome)
-* GUI for 
+* GUI for common operations
 * Automatic smoothing
 
 ## How to Install and use
 
 ### Advanced users
 * Install via `pip3 install synth_mapping_helper` (requires Python 3.9 or higher)
 * See `python3 -m synth_mapping_helper.cli -h` for usage of the clipboard manipulation
```

### Comparing `synth_mapping_helper-1.0.2/README.md` & `synth_mapping_helper-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     * **Automatic backups** while mapping
     * Plot notes to spot outliers
     * View hand velocity and acceleration to find sections to smooth out
     * Show wall density and estimatation which ones will not render on quest
     * Fix **wall offset** between editor and game ("Finalize")
 
 ### Maybe (contributions welcome)
-* GUI for 
+* GUI for common operations
 * Automatic smoothing
 
 ## How to Install and use
 
 ### Advanced users
 * Install via `pip3 install synth_mapping_helper` (requires Python 3.9 or higher)
 * See `python3 -m synth_mapping_helper.cli -h` for usage of the clipboard manipulation
```

### Comparing `synth_mapping_helper-1.0.2/setup.py` & `synth_mapping_helper-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.0.2/src/synth_mapping_helper/cli.py` & `synth_mapping_helper-1.1.0/src/synth_mapping_helper/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,32 +9,34 @@
 
 _filter_groups = {
     "notes": synth_format.NOTE_TYPES,
     "walls": list(synth_format.WALL_TYPES),
     "slides": synth_format.SLIDE_TYPES,
 }
 
-def _movement_helper(data: synth_format.DataContainer, base_func, relative_func, pivot_func, relative: bool, pivot: list[int], *args, **kwargs) -> None:
+def _movement_helper(data: synth_format.DataContainer, mirror_left: bool, base_func, relative_func, pivot_func, relative: bool, pivot: list[int], *args, **kwargs) -> None:
     """pick the right function depending on relative or pivot being set"""
     if relative:
-        data.apply_for_all(relative_func, *args, **kwargs)
+        data.apply_for_all(relative_func, *args, mirror_left=mirror_left,  **kwargs)
     elif pivot is not None:
-        data.apply_for_all(pivot_func, *args, pivot_3d=pivot, **kwargs)
+        data.apply_for_all(pivot_func, *args, mirror_left=mirror_left, pivot_3d=pivot, **kwargs)
     else:
-        data.apply_for_all(base_func, *args, **kwargs)
+        data.apply_for_all(base_func, *args, mirror_left=mirror_left, **kwargs)
 
 def do_movement(options, data: synth_format.DataContainer, filter_types: list = synth_format.ALL_TYPES) -> None:
-    if options.scale:
-        _movement_helper(data, movement.scale, movement.scale_relative, movement.scale_from, options.relative, options.pivot, options.scale, types=filter_types)
-    if options.rotate:
-        _movement_helper(data, movement.rotate, movement.rotate_relative, movement.rotate_around, options.relative, options.pivot, options.rotate, types=filter_types)
-    if options.offset:
-        _movement_helper(data, movement.offset, movement.offset_relative, movement.offset, options.relative, options.pivot, options.offset, types=filter_types)
-    if options.outset:
-        _movement_helper(data, movement.outset, movement.outset_relative, movement.outset_from, options.relative, options.pivot, options.outset, types=filter_types)
+    if options.scale is not None:
+        _movement_helper(data, options.mirror_left, movement.scale, movement.scale_relative, movement.scale_from, options.relative, options.pivot, options.scale, types=filter_types)
+    if options.rotate is not None:
+        _movement_helper(data, options.mirror_left, movement.rotate, movement.rotate_relative, movement.rotate_around, options.relative, options.pivot, options.rotate, types=filter_types)
+    if options.wall_rotate is not None:
+        data.apply_for_walls(movement.rotate_relative, options.wall_rotate, mirror_left=options.mirror_left, types=filter_types)
+    if options.offset is not None:
+        _movement_helper(data, options.mirror_left, movement.offset, movement.offset_relative, movement.offset, options.relative, options.pivot, options.offset, types=filter_types)
+    if options.outset is not None:
+        _movement_helper(data, options.mirror_left, movement.outset, movement.outset_relative, movement.outset_from, options.relative, options.pivot, options.outset, types=filter_types)
 
 def get_parser():
     parser = ArgumentParser(
         formatter_class=RawDescriptionHelpFormatter,
         prog=f"python3 -m {__package__}.{Path(__file__).stem}",
         description='\n'.join([
             f"Note types:\n\t{', '.join(synth_format.NOTE_TYPES)}",
@@ -54,14 +56,15 @@
         epilog=f"Version: {__version__}",
     )
 
     parser.add_argument("-E", "--start-empty", type=utils.parse_number, metavar="BPM", help="Start with empty data instead of reading the clipboard. Requires specifing BPM. Use with --spawn.")
     parser.add_argument("--use-original", action="store_true", help="When calling this multiple times, start over with orignal copied json")
     parser.add_argument("-f", "--filter-types", nargs="+", metavar="FILTER_TYPE", choices=synth_format.ALL_TYPES + tuple(_filter_groups), default=synth_format.ALL_TYPES, help=f"Only affect notes and walls of these types. Multiple types can be specified seperated by spaces, defaults to all")
     parser.add_argument("--invert-filter", action="store_true", help="Invert filter so everything *but* the filter is affected")
+    parser.add_argument("--mirror-left", action="store_true", help="Mirror operations for the LEFT hand")
 
     preproc_group = parser.add_argument_group("pre-processing")
     preproc_group.add_argument("-b", "--bpm", type=utils.parse_number, help="Change BPM without changing timing")
     preproc_group.add_argument("--delete-others", action="store_true", help="Delete everything that doesn't match the filter")
     preproc_group.add_argument("--connect-singles", type=utils.parse_time, metavar="MAX_INTERVAL", help="Replace strings of single notes with rails if they are . Use with'--rails-to-singles=1' if you want to keep the singles")
     preproc_group.add_argument("--merge-rails", type=utils.parse_time, nargs="?", action="append", metavar="MAX_INTERVAL", help="Merge sequential rails. By default only joins rails that start close to where another ends (in X, Y AND time), but with MAX_INTERVAL only the time interval counts")
     preproc_group.add_argument("--swap-hands", action="store_true", help="Swap left and right hand notes.")
@@ -84,23 +87,26 @@
 
     movement_group = parser.add_argument_group("movement", description="Operation order is always: scale, rotate, offset, outset")
     pivot_group = movement_group.add_mutually_exclusive_group()
     pivot_group.add_argument("-p", "--pivot", type=utils.parse_position, help="Pivot for outset, scale and rotate as x,y,t")
     pivot_group.add_argument("--note-pivot", choices=synth_format.NOTE_TYPES, help="Use position of first matching note as pivot (determined before any operations)")
     pivot_group.add_argument("--relative", action="store_true", help="Use first node of rails as pivot for outset, scale and rotate, and for walls offset because relative based on rotation")
     movement_group.add_argument("-s", "--scale", type=utils.parse_position, help="Scale positions by x,y,t. Use negative values to mirror across axis. Does NOT change the size of walls. Time-Scale of 2 means twice as long, not twice as fast.")
-    movement_group.add_argument("-r", "--rotate", type=utils.parse_number, metavar="DEGREES", help="Rotate counterclockwise by this many degrees (negative for clockwise)")
+    movement_group.add_argument("-r", "--rotate", type=utils.parse_number, metavar="DEGREES", help="Rotate everything counterclockwise by this many degrees (negative for clockwise)")
+    movement_group.add_argument("--wall-rotate", type=utils.parse_number, metavar="DEGREES", help="Rotate walls counterclockwise around themselves by this many degrees (negative for clockwise)")
     movement_group.add_argument("-o", "--offset", type=utils.parse_position, help="Move/Translate by x,y,t")
     movement_group.add_argument("--outset", type=utils.parse_number, metavar="DISTANCE", help="Move outwards (negative for inwards, can move 'across' pivot)")
     rail_stack_group = movement_group.add_mutually_exclusive_group()
-    rail_stack_group.add_argument("--offset-along", choices=synth_format.NOTE_TYPES, help="Offset objects to follow notes and rails of the specified color")
-    rail_stack_group.add_argument("--rotate-with", choices=synth_format.NOTE_TYPES, help="Rotate and outset the objects to follow notes and rails of the specified color")
+    rail_stack_group.add_argument("--offset-along", choices=synth_format.NOTE_TYPES, help="While stacking: Offset objects to follow notes/rails of the specified type")
+    rail_stack_group.add_argument("--rotate-with", choices=synth_format.NOTE_TYPES, help="While stacking: Rotate and outset the objects to follow notes/rails of the specified type")
     movement_group.add_argument("--offset-random", type=utils.parse_xy_range, metavar="[MIN_X:]MAX_X,[MIN_Y:]MAX_Y", help="Offset by a random amount in the X and Y axis. When no MIN is given, uses negative MAX.")
 
     movement_group.add_argument("-c", "--stack-count", type=int, help="Instead of moving, create copies. Must have time offset set.")
+    movement_group.add_argument("--stack-duration", type=utils.parse_time, help="Like --stack-count, but you can give it during in beats ('4') or seconds ('2s').")
+    movement_group.add_argument("--autostack", nargs="?", choices=("OFFSET", "SPIRAL", "OUTSET", "SCALE"), action="append", metavar="OFFSET/SPIRAL/OUTSET/SCALE", help="Find the first pair of matching objects and continue the pattern. For continuing the positions, the following modes are supported: OFFSET (default, absolute xy), SPIRAL (rotate around implied pivot), OUTSET (distance from pivot) and SCALE (xy ratio).")
 
     postproc_group = parser.add_argument_group("post-processing")
     postproc_group.add_argument("--split-rails", action="store_true", help="Split rails at single notes")
     postproc_group.add_argument("--rails-to-singles", type=int, nargs="?", action="append", metavar="KEEP_RAIL", help="Replace rails with single notes at all nodes. KEEP_RAIL is optional and can be '1' if you want to keep the rail instead of replacing it")
     postproc_group.add_argument("--keep-alignment", action="store_true", help="Do NOT shift the start of selection to first element")
 
     return parser
@@ -122,18 +128,18 @@
 
     # argument post-parsing
     # convert time parsed in seconds to beats
     for pos_val in "spawn-location", "pivot", "offset", "scale":
         v = getattr(options, pos_val, None)
         if v is not None and isinstance(v[2], utils.SecondFloat):
             setattr(options, pos_val[:2] + (v[2].to_beat(data.bpm),))
-    for time_val in "connect_singles", "merge_rails", "interpolate", "interpolate_linear", "shorten_rails", "spike_width":
-        v = getattr(options, pos_val, None)
+    for time_val in "connect_singles", "merge_rails", "interpolate", "interpolate_linear", "shorten_rails", "spike_width", "stack_duration":
+        v = getattr(options, time_val, None)
         if isinstance(v, utils.SecondFloat):
-            setattr(options, pos_val, v.to_beat(data.bpm))
+            setattr(options, time_val, v.to_beat(data.bpm))
     # expand filter groupts
     if any(name in options.filter_types for name in _filter_groups):
         out_filters = []
         for inp in options.filter_types:
             if inp in _filter_groups:
                 out_filters.extend(_filter_groups[inp])
             else:
@@ -151,14 +157,73 @@
     # get note pivot (before filtering)
     if options.note_pivot:
         notes = getattr(data, options.note_pivot)
         if not notes:
             abort(f"Could not find any {options.note_pivot} notes")
         options.pivot = notes[sorted(notes)[0]][:3]
 
+    # stacking
+    if options.autostack is not None:
+        if not options.stack_count and not options.stack_duration:
+            abort("Cannot --autostack without count/duration")
+        first = None
+        second = None
+        for t in synth_format.ALL_TYPES:
+            obj_dict = data.get_object_dict(t)
+            if len(obj_dict) >= 2:
+                it = iter(sorted(obj_dict.items()))
+                _, t_first = next(it)
+                if first is None or t_first[0,2] < first[0,2]:
+                    first = t_first[0]  # rail head only
+                    _, t_second = next(it)
+                    second = t_second[0]
+        if first is None or second is None:
+            abort("Could not find object pair for autostack")
+
+        if options.autostack[0] == "SPIRAL":
+            if first.shape[0] != 5:
+                abort("Can only spiral-autostack based on walls")
+            # rotation from point 'a' to point 'b', around pivot 'p' by angle 'ang':
+            #   x_b = (x_a - x_p) * cos(ang) - (y_a - y_p) * sin(ang) + x_p
+            #   y_b = (x_a - x_p) * sin(ang) + (y_a - y_p) * cos(ang) + y_p
+            # I couldn't find a good way to solve that for x_p and y_p, so lets do it the geometric way:
+            #   p must be an equal distance from both points, so together with p they form an isosceles triangle
+            #   In this triangle we want the the angle at p (alpha) to match wall rotation, allowing us to calculate p using basic trigonometry
+            #   In particular, the first point, the point halfway between both points and the pivot form a right triangle with an angle of alpha/2 at the pivot and an opposite of (b-a)/2
+            #   Therefore, the hypotenuse will be ((b-a)/2) / sin(alpha/2) long and face the direction of (b-a)/2 rotated by 90-alpha/2
+            options.rotate = second[4] - first[4]
+            options.pivot = first[:3] + movement.rotate((second - first)[:3]/2, 90 - options.rotate/2) / np.sin(np.radians(options.rotate/2))
+            options.offset = (0, 0, second[2] - first[2])
+        else:
+            if options.pivot is not None:
+                first[:2] -= options.pivot[:2]
+                second[:2] -= options.pivot[:2]
+
+            if options.autostack[0] is None or options.autostack[0] == "OFFSET":
+                options.offset = (second - first)[:3]
+            elif options.autostack[0] == "OUTSET":
+                # this is equivalent to the "rotate-with" calculations below
+                options.rotate = np.degrees(np.arctan2(first[0], first[1])) - np.degrees(np.arctan2(second[0], second[1]))
+                options.outset = np.sqrt(second[:2].dot(second[:2])) - np.sqrt(first[:2].dot(first[:2]))
+                options.offset = (0, 0, second[2] - first[2])
+            elif options.autostack[0] == "SCALE":
+                options.scale = (second[0] / first[0], second[1] / first[1], 1)
+                options.offset = (0, 0, second[2] - first[2])
+
+            if first.shape[0] == 5:
+                options.wall_rotate = ((second[4] - first[4]) - (options.rotate or 0)) or None  # see if we need to correct wall rotation
+
+    if options.stack_duration:
+        if options.stack_count:
+            abort("Cannot use --stack-count and --stack-duration at the same time")
+        options.stack_count = int(options.stack_duration / options.offset[2])
+
+    if options.stack_count and (options.offset is None or not options.offset[2]):
+        abort("Cannot stack with time offset of 0")
+
     # preprocessing
     if options.bpm:
         bpm_scale = [1, 1, options.bpm / data.bpm]
         data.apply_for_all(movement.scale, bpm_scale, types=filter_types)
 
     if options.delete_others:
         data = data.filtered(types=filter_types)
@@ -231,32 +296,30 @@
     elif options.interpolate_linear:
         data.apply_for_notes(rails.interpolate_nodes, "linear", options.interpolate_linear, types=filter_types)
     if options.shorten_rails:
         data.apply_for_notes(rails.shorten_rail, options.shorten_rails, types=filter_types)
     if options.spiral:
         if (1 / options.spiral) % 1 == 0:
             abort("Chosen spiral factor divides 1 and would result in a straight rail. Refusing action!")
-        def _add_spiral(nodes: "numpy array (n, 3)") -> "numpy array (n, 3)":
-            nodes[:, :2] += pattern_generation.spiral(options.spiral, nodes.shape[0], options.start_angle) * options.radius
+        def _add_spiral(nodes: "numpy array (n, 3)", direction: int = 1) -> "numpy array (n, 3)":
+            nodes[:, :2] += pattern_generation.spiral(options.spiral * direction, nodes.shape[0], options.start_angle if direction == 1 else 180 - options.start_angle) * options.radius
             return nodes
-        data.apply_for_notes(_add_spiral, types=filter_types)
+        data.apply_for_notes(_add_spiral, types=filter_types, mirror_left=options.mirror_left)
     if options.spikes is not None:
-        def _add_spikes(nodes: "numpy array (n, 3)") -> "numpy array (n, 3)":
+        def _add_spikes(nodes: "numpy array (n, 3)", direction: int = 1) -> "numpy array (n, 3)":
             count = nodes.shape[0]
             nodes = np.repeat(nodes, 3, axis=0)
             nodes[::3] -= options.spike_width
             nodes[1::3] -= options.spike_width/2
-            nodes[:, :2] += pattern_generation.spikes(options.spikes, count, options.start_angle) * options.radius
+            nodes[:, :2] += pattern_generation.spikes(options.spikes * direction, count, options.start_angle if direction == 1 else 180 - options.start_angle) * options.radius
             return nodes
-        data.apply_for_notes(_add_spikes, types=filter_types)
+        data.apply_for_notes(_add_spikes, types=filter_types, mirror_left=options.mirror_left)
 
     # movement
     if options.stack_count:
-        if not options.offset or options.offset[2] == 0:
-            abort("Cannot stack with time offset of 0")
         stacking = data.filtered(types=filter_types)
         if options.offset_along or options.rotate_with:
             if options.offset_along and options.rotate_with:
                 abort("Cannot use offset-along and rotate-with at the same time")
             if options.relative:
                 abort("Cannot use offset-along or rotate-with in relative mode")
             start_pos = rails.get_position_at(getattr(data, options.offset_along or options.rotate_with), 0)
@@ -268,70 +331,41 @@
             do_movement(options, stacking)
             tmp = stacking.filtered()  # deep copy
             if options.offset_along:
                 cur_pos = rails.get_position_at(getattr(data, options.offset_along), (i+1) * options.offset[2])
                 if cur_pos is None:
                     abort(f"No intermediate position of {options.offset_along} notes found at {(i+1) * options.offset[2]}")
                 delta = cur_pos - start_pos
-                tmp.apply_for_all(movement.offset, [delta[0], delta[1], 0])
+                tmp.apply_for_all(movement.offset, [delta[0], delta[1], 0], mirror_left=options.mirror_left)
             if options.rotate_with:
                 cur_pos = rails.get_position_at(getattr(data, options.rotate_with), (i+1) * options.offset[2])
                 if cur_pos is None:
                     abort(f"No intermediate position of {options.rotate_with} notes found at {(i+1) * options.offset[2]}")
                 if options.pivot is not None:
                     cur_pos -= options.pivot[:2]
                 angle_diff = np.degrees(np.arctan2(start_pos[0], start_pos[1])) - np.degrees(np.arctan2(cur_pos[0], cur_pos[1]))
                 distance_diff = np.sqrt(cur_pos.dot(cur_pos)) - np.sqrt(start_pos.dot(start_pos))
                 # outset all objects together by precalculating the offset based on rail position
                 group_outset = [cur_pos[0], cur_pos[1], 0] / np.sqrt(cur_pos.dot(cur_pos)) * distance_diff
                 if options.pivot is not None:
-                    tmp.apply_for_all(movement.rotate_around, angle_diff, pivot_3d=options.pivot)
+                    tmp.apply_for_all(movement.rotate_around, angle_diff, pivot_3d=options.pivot, mirror_left=options.mirror_left)
                 else:
-                    tmp.apply_for_all(movement.rotate, angle_diff)
+                    tmp.apply_for_all(movement.rotate, angle_diff, mirror_left=options.mirror_left)
                 tmp.apply_for_all(movement.offset, group_outset)
             if options.offset_random is not None:
                 random_offset = pattern_generation.random_xy(1, options.offset_random[0], options.offset_random[1])[0]
-                tmp.apply_for_all(movement.offset, [random_offset[0], random_offset[1], 0])
+                tmp.apply_for_all(movement.offset, [random_offset[0], random_offset[1], 0], mirror_left=options.mirror_left)
             data.merge(tmp)
     else:
         if options.offset_along or options.rotate_with:
-            if options.offset_along and options.rotate_with:
-                abort("Cannot use offset-along and rotate-with at the same time")
-            start_pos = rails.get_position_at(getattr(data, options.offset_along or options.rotate_with), 0)
-            if start_pos is None:
-                abort(f"No start position of {options.offset_along or options.rotate_with} notes found")
-            if options.pivot is not None:
-                start_pos -= options.pivot[:2]
+            abort("Cannot use offset-along or rotate-with without stacking")
         do_movement(options, data, filter_types=filter_types)
-        if options.offset_along:
-            cur_pos = rails.get_position_at(getattr(data, options.offset_along), options.offset[2])
-            if cur_pos is None:
-                abort(f"No intermediate position of {options.offset_along} notes found at {options.offset[2]}")
-            if options.relative:
-                abort("Cannot use offset-along or rotate-with in relative mode")
-            delta = cur_pos - start_pos
-            data.apply_for_all(movement.offset, [delta[0], delta[1], 0], types=filter_types)
-        if options.rotate_with:
-            cur_pos = rails.get_position_at(getattr(data, options.rotate_with), options.offset[2])
-            if cur_pos is None:
-                abort(f"No intermediate position of {options.rotate_with} notes found at {options.offset[2]}")
-            if options.pivot is not None:
-                cur_pos -= options.pivot[:2]
-            angle_diff = np.degrees(np.arctan2(start_pos[0], start_pos[1])) - np.degrees(np.arctan2(cur_pos[0], cur_pos[1]))
-            distance_diff = np.sqrt(cur_pos.dot(cur_pos)) - np.sqrt(start_pos.dot(start_pos))
-            # outset all objects together by precalculating the offset based on rail position
-            group_outset = [cur_pos[0], cur_pos[1], 0] / np.sqrt(cur_pos.dot(cur_pos)) * distance_diff
-            if options.pivot is not None:
-                data.apply_for_all(movement.rotate_around, angle_diff, pivot_3d=options.pivot, types=filter_types)
-            else:
-                data.apply_for_all(movement.rotate, angle_diff, types=filter_types)
-            data.apply_for_all(movement.offset, group_outset, types=filter_types)
         if options.offset_random is not None:
             random_offset = pattern_generation.random_xy(1, options.offset_random[0], options.offset_random[1])[0]
-            data.apply_for_all(movement.offset, [random_offset[0], random_offset[1], 0], types=filter_types)
+            data.apply_for_all(movement.offset, [random_offset[0], random_offset[1], 0], mirror_left=options.mirror_left)
 
     # postprocessing
     if options.split_rails:
         data.apply_for_note_types(rails.split_rails, types=filter_types)
     if options.rails_to_singles:
         data.apply_for_note_types(rails.rails_to_singles, keep_rail=bool(options.rails_to_singles[0]), types=filter_types)
     synth_format.export_clipboard(data, not options.keep_alignment)
```

### Comparing `synth_mapping_helper-1.0.2/src/synth_mapping_helper/companion.py` & `synth_mapping_helper-1.1.0/src/synth_mapping_helper/companion.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.0.2/src/synth_mapping_helper/finalize.py` & `synth_mapping_helper-1.1.0/src/synth_mapping_helper/finalize.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.0.2/src/synth_mapping_helper/movement.py` & `synth_mapping_helper-1.1.0/src/synth_mapping_helper/movement.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,114 +1,160 @@
 import numpy as np
 
 # Note: None of these functions are allowed to *modify* the input array instance. Returning the same array (if nothing needed to be changed) is allowed.
 
+MIRROR_VEC_2D = np.array([-1, 1])
+MIRROR_VEC_3D = np.array([-1, 1, 1])
+
 # movement
-def offset(data: "numpy array (n, m)", offset_3d: "numpy array (3)", pivot_3d: None = None) -> "numpy array (n, 3+)":
+def offset(
+    data: "numpy array (n, m)",
+    offset_3d: "numpy array (3)",
+    pivot_3d: None = None,
+    direction: int = 1,
+) -> "numpy array (n, 3+)":
     """translate positions"""
     # pivot is ignored, but exists so this can be used as pivot func aswell
     offset_nd = np.zeros((data.shape[-1]))
-    offset_nd[...,:3] = offset_3d
+    offset_nd[..., :3] = offset_3d if direction == 1 else offset_3d * MIRROR_VEC_3D
     return data + offset_nd
 
-def offset_relative(data: "numpy array (n, m)", offset_3d: "numpy array (3)") -> "numpy array (n, 3+)":
+
+def offset_relative(
+    data: "numpy array (n, m)", offset_3d: "numpy array (3)", direction: int = 1
+) -> "numpy array (n, 3+)":
     """translate positions, use relative coordinates for walls"""
     if data.shape[-1] == 3:
-        return offset(data, offset_3d)
+        return offset(data, offset_3d, direction=direction)
     # calculate rot matrix for angle of every wall
     rad_ang = np.radians(np.atleast_1d(data[:, 4]))
-    rot_matrix = np.rollaxis(np.array((
-        (np.cos(rad_ang), np.sin(rad_ang)),
-        (-np.sin(rad_ang), np.cos(rad_ang)),
-    )), -1)
+    rot_matrix = np.rollaxis(
+        np.array(
+            (
+                (np.cos(rad_ang), np.sin(rad_ang)),
+                (-np.sin(rad_ang), np.cos(rad_ang)),
+            )
+        ),
+        -1,
+    )
     offset_nd = np.zeros((data.shape[-1]))
-    offset_nd[...,:2] = np.array(offset_3d[:2]).dot(rot_matrix)  # offset is rotated for each wall
-    offset_nd[...,2] = offset_3d[2]  # t stays as-is
+    offset_nd[..., :2] = (
+        np.array(offset_3d[:2]) if direction == 1 else offset_3d[:2] * MIRROR_VEC_3D
+    ).dot(
+        rot_matrix
+    )  # offset is rotated for each wall
+    offset_nd[..., 2] = offset_3d[2]  # t stays as-is
     return data + offset_nd
-    
-def outset(data: "numpy array (n, m)", outset_scalar: float) -> "numpy array (n, 3+)":
+
+
+def outset(
+    data: "numpy array (n, m)", outset_scalar: float, direction: int = 1
+) -> "numpy array (n, 3+)":
     """move positions outwards"""
-    angles = np.arctan2(data[..., 1], data[..., 0])
+    zero_mask = np.logical_and(np.isclose(data[..., 0], 0, atol=1e-5), np.isclose(data[..., 1], 0, atol=1e-5))  # ignore xy close to 0,0
+    angles = np.arctan2(data[~zero_mask, 1], data[~zero_mask, 0])
     normalized = np.zeros(data.shape)
-    normalized[..., 0] = np.cos(angles)
-    normalized[..., 1] = np.sin(angles)
+    normalized[~zero_mask, 0] = np.cos(angles)
+    normalized[~zero_mask, 1] = np.sin(angles)
     return data + normalized * outset_scalar
 
-def outset_from(data: "numpy array (n, m)", outset_scalar: float, pivot_3d: "numpy array (3)") -> "numpy array (n, 3+)":
+
+def outset_from(
+    data: "numpy array (n, m)",
+    outset_scalar: float,
+    pivot_3d: "numpy array (3)",
+    direction: int = 1,
+) -> "numpy array (n, 3+)":
     """move positions away from pivot"""
     pivot_nd = np.zeros((data.shape[-1]))
-    pivot_nd[...,:3] = pivot_3d
-    return outset(data - pivot_nd, outset_scalar) + pivot_nd
+    pivot_nd[..., :3] = pivot_3d
+    return outset(data - pivot_nd, outset_scalar, direction=direction) + pivot_nd
+
 
-def outset_relative(data: "numpy array (n, m)", outset_scalar: float) -> "numpy array (n, 3+)":
+def outset_relative(
+    data: "numpy array (n, m)", outset_scalar: float, direction: int = 1
+) -> "numpy array (n, 3+)":
     """move positions away from pivot"""
     if data.shape[0] == 1:
         # no effect on single notes / walls
         return data
-    return outset(data - data[0], outset_scalar) + data[0]
+    return outset(data - data[0], outset_scalar, direction=direction) + data[0]
 
 
-def scale(data: "numpy array (n, 3+)", scale_3d: "numpy array (3)") -> "numpy array (n, 3+)":
+def scale(
+    data: "numpy array (n, 3+)", scale_3d: "numpy array (3)", direction: int = 1
+) -> "numpy array (n, 3+)":
     """scale positions relative to center and start of selection"""
     if scale_3d[2] == 0:
         raise ValueError("Cannot have 0 for time scale")
     scale_nd = np.ones((data.shape[-1]))
-    scale_nd[...,:3] = scale_3d
+    scale_nd[..., :3] = scale_3d
     output = data * scale_nd
     if scale_nd[2] < 0:  # reverse order of elements
         output = output[::-1]
     return output
 
 
 def scale_from(
-    data: "numpy array (n, 3+)", scale_3d: "numpy array (3)", pivot_3d: "numpy array (3)"
+    data: "numpy array (n, 3+)",
+    scale_3d: "numpy array (3)",
+    pivot_3d: "numpy array (3)",
+    direction: int = 1,
 ) -> "numpy array (n, 3+)":
     """scale positions relative to pivot"""
     pivot_nd = np.ones((data.shape[-1]))
-    pivot_nd[...,:3] = pivot_3d
-    return scale(data - pivot_nd, scale_3d) + pivot_nd
+    pivot_nd[..., :3] = pivot_3d
+    return scale(data - pivot_nd, scale_3d, direction=direction) + pivot_nd
+
 
 def scale_relative(
     data: "numpy array (n, 3+)", scale_3d: "numpy array (3)"
 ) -> "numpy array (n, 3+)":
     """scale positions relative to first node"""
     if data.shape[0] == 1:
         # no effect on single notes / walls
         return data
     return scale(data - data[0], scale_3d) + data[0]
 
-def rotate(data: "numpy array (n, 3+)", angle: float) -> "numpy array (n, 3+)":
+
+def rotate(
+    data: "numpy array (n, 3+)", angle: float, direction: int = 1
+) -> "numpy array (n, 3+)":
     """rotate positions anticlockwise around center"""
-    rad_ang = np.radians(angle)
+    rad_ang = np.radians(angle * direction)
     rot_matrix = np.identity(data.shape[-1])
-    rot_matrix[:2,:2] = [
+    rot_matrix[:2, :2] = [
         [np.cos(rad_ang), np.sin(rad_ang)],
         [-np.sin(rad_ang), np.cos(rad_ang)],
     ]
     out = data.dot(rot_matrix)
     if data.shape[-1] >= 5:
         # just add to wall rotation
-        out[..., 4] += angle
+        out[..., 4] += angle * direction
     return out
 
 def rotate_around(
-    data: "numpy array (n, 3+)", angle: float, pivot_3d: "numpy array (3)"
+    data: "numpy array (n, 3+)",
+    angle: float,
+    pivot_3d: "numpy array (3)",
+    direction: int = 1,
 ) -> "numpy array (n, 3+)":
     """rotate positions anticlockwise around pivot"""
     pivot_nd = np.zeros((data.shape[-1]))
-    pivot_nd[...,:3] = pivot_3d
-    return rotate(data - pivot_nd, angle) + pivot_nd
+    pivot_nd[..., :3] = pivot_3d
+    return rotate(data - pivot_nd, angle, direction=direction) + pivot_nd
+
 
 def rotate_relative(
-    data: "numpy array (n, 3+)", angle: float
+    data: "numpy array (n, 3+)", angle: float, direction: int = 1
 ) -> "numpy array (n, 3+)":
     """rotate positions anticlockwise around first node/wall center"""
     if data.shape[0] == 1:
         if data.shape[-1] >= 5:
             # just add to wall rotation
             wall_rot = np.zeros((data.shape[-1]))
-            wall_rot[4] = angle
+            wall_rot[4] = angle * direction
             return data + wall_rot
         else:
             # no effect on single notes
             return data
-    return rotate(data - data[0], angle) + data[0]
+    return rotate(data - data[0], angle, direction=direction) + data[0]
```

### Comparing `synth_mapping_helper-1.0.2/src/synth_mapping_helper/pattern_generation.py` & `synth_mapping_helper-1.1.0/src/synth_mapping_helper/pattern_generation.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.0.2/src/synth_mapping_helper/rails.py` & `synth_mapping_helper-1.1.0/src/synth_mapping_helper/rails.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 from .synth_format import DataContainer, SINGLE_COLOR_NOTES
 from .utils import bounded_arange
 
 # How far last node and start note can be spaced for two rails to be merged
 MERGE_ACCURACY_GRID = 1 / 8
 MERGE_ACCURACY_BEAT = 1 / 64
 
-def interpolate_linear(data: "numpy array (n, m)", new_z: "numpy array (x)") -> "numpy array (x, 3)":
+def interpolate_linear(data: "numpy array (n, m)", new_z: "numpy array (x)", *, direction: bool = 1) -> "numpy array (x, 3)":
     return np.stack((
         np.interp(new_z, data[:, 2], data[:, 0]),
         np.interp(new_z, data[:, 2], data[:, 1]),
         new_z,
     ), axis=-1)
 
-def interpolate_spline(data: "numpy array (n, m)", new_z: "numpy array (x)") -> "numpy array (x, 3)":
+def interpolate_spline(data: "numpy array (n, m)", new_z: "numpy array (x)", *, direction: bool = 1) -> "numpy array (x, 3)":
     if data.shape[0] == 1:
         return data
     # add points in straight line from start and end to match shape more closely
     padded_data = np.concatenate(([2*data[0]-data[1]], data, [2*data[-1]-data[-2]]))
     return np.stack((
         pchip_interpolate(padded_data[:, 2], padded_data[:, 0], new_z),
         pchip_interpolate(padded_data[:, 2], padded_data[:, 1], new_z),
@@ -45,15 +45,15 @@
             return interpolate_spline(nodes, beat)[0:2]
 
     # neither
     return None
 
 # Note: None of these functions are allowed to *modify* the input dict instance. Returning the same dict (if nothing needed to be changed) is allowed.
 
-def split_rails(notes: SINGLE_COLOR_NOTES) -> SINGLE_COLOR_NOTES:
+def split_rails(notes: SINGLE_COLOR_NOTES, *, direction: bool = 1) -> SINGLE_COLOR_NOTES:
     """splits rails at single notes"""
     current_rail_start = None
     current_rail_end = None
     out: SINGLE_COLOR_NOTES = {}
 
     for time in sorted(notes):
         if current_rail_start is not None and time >= current_rail_end:
@@ -85,15 +85,15 @@
 
             current_rail_start = remainder[0, 2]
             current_rail_end = remainder[-1, 2]
 
     return out
 
 
-def merge_sequential_rails(notes: SINGLE_COLOR_NOTES) -> SINGLE_COLOR_NOTES:
+def merge_sequential_rails(notes: SINGLE_COLOR_NOTES, *, direction: bool = 1) -> SINGLE_COLOR_NOTES:
     """merges rails where end and start a very close"""
     current_rail_start = None
     current_rail_end = None
     out: SINGLE_COLOR_NOTES = {}
 
     for time in sorted(notes):
         nodes = notes[time]
@@ -120,15 +120,15 @@
     
         current_rail_start = time
         current_rail_end = nodes[-1, 2]
         out[time] = nodes
 
     return out
 
-def merge_rails(notes: SINGLE_COLOR_NOTES, max_interval: float) -> SINGLE_COLOR_NOTES:
+def merge_rails(notes: SINGLE_COLOR_NOTES, max_interval: float, *, direction: bool = 1) -> SINGLE_COLOR_NOTES:
     """merges rails"""
     current_rail_start = None
     current_rail_end = None
     out: SINGLE_COLOR_NOTES = {}
 
     for time in sorted(notes):
         nodes = notes[time]
@@ -157,15 +157,15 @@
             out[current_rail_start] = np.concatenate((previous_nodes, nodes))
             current_rail_end = nodes[-1, 2]
             # add single note where rail started
             out[time] = nodes[:1]
 
     return out
 
-def connect_singles(notes: SINGLE_COLOR_NOTES, max_interval: float) -> SINGLE_COLOR_NOTES:
+def connect_singles(notes: SINGLE_COLOR_NOTES, max_interval: float, *, direction: bool = 1) -> SINGLE_COLOR_NOTES:
     """Turn single notes into rails"""
     current_rail_start = None
     current_rail_end = None
     out: SINGLE_COLOR_NOTES = {}
     for time in sorted(notes):
         nodes = notes[time]
 
@@ -186,30 +186,30 @@
             out[current_rail_start] = np.concatenate((out[current_rail_start], nodes))
             current_rail_end = nodes[-1, 2]
             # note: does not readd the single notes to the output dict
 
     return out
 
 def interpolate_nodes(
-    data: "numpy array (n, 3)", mode: "'spline' or 'linear'", interval: float
+    data: "numpy array (n, 3)", mode: "'spline' or 'linear'", interval: float, *, direction: bool = 1
 ) -> "numpy array (n, 3)":
     """places nodes at defined interval along the rail, interpolating between existing nodes"""
     if data.shape[0] == 1:  # ignore single nodes
         return data
     new_z = bounded_arange(data[0, 2], data[-1, 2], interval)
 
     if mode == "spline":
         return interpolate_spline(data, new_z)
     elif mode == "linear":
         return interpolate_linear(data, new_z)
     else:
         raise RuntimeError("Invalid iterpolation mode")
 
 
-def rails_to_singles(notes: SINGLE_COLOR_NOTES, keep_rail: bool) -> SINGLE_COLOR_NOTES:
+def rails_to_singles(notes: SINGLE_COLOR_NOTES, keep_rail: bool, *, direction: bool = 1) -> SINGLE_COLOR_NOTES:
     """Turn all rails into single notes"""
     out: SINGLE_COLOR_NOTES = {}
     for time in sorted(notes):
         nodes = notes[time]
         if nodes.shape[0] == 1:  # ignore single nodes
             out[time] = nodes
             continue
@@ -217,15 +217,15 @@
             out[nodes[0,2]] = nodes
         for node in nodes[int(keep_rail):]:  # when keeping the rail, don't overwrite the start with a single note
             out[node[2]] = node[np.newaxis]
 
     return out
 
 def shorten_rail(
-    data: "numpy array (n, 3)", distance: float
+    data: "numpy array (n, 3)", distance: float, *, direction: bool = 1
 ) -> "numpy array (n, 3)":
     """Cut a bit of the end or start of the rail"""
     if data.shape[0] == 1:  # ignore single nodes
         return data
     if distance > 0:  # cut at the end
         new_z = data[-1,2] - distance
         last_index = np.argwhere(data[:, 2] < new_z)[-1][0]  # last node before new end
```

### Comparing `synth_mapping_helper-1.0.2/src/synth_mapping_helper/synth_format.py` & `synth_mapping_helper-1.1.0/src/synth_mapping_helper/synth_format.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,46 +81,46 @@
     single: SINGLE_COLOR_NOTES
     both: SINGLE_COLOR_NOTES
     walls: WALLS
 
     # Note: None of these functions are allowed to *modify* the dicts, instead they must create new dicts
     # This avoids requring deep copies for everything
 
-    def apply_for_notes(self, f, *args, types: list = NOTE_TYPES, **kwargs) -> None:
+    def apply_for_notes(self, f, *args, types: list = NOTE_TYPES, mirror_left: bool = False, **kwargs) -> None:
         for t in types:
             if t not in NOTE_TYPES:
                 continue
             notes = getattr(self, t)
             out = {}
             for _, nodes in sorted(notes.items()):
-                out_nodes = f(nodes, *args, **kwargs)
+                out_nodes = f(nodes, *args, direction=(-1 if mirror_left and t == "left" else 1), **kwargs)
                 out[out_nodes[0, 2]] = out_nodes
             setattr(self, str(t), out)
 
-    def apply_for_walls(self, f, *args, types: list = WALL_TYPES, **kwargs) -> None:
+    def apply_for_walls(self, f, *args, types: list = WALL_TYPES, mirror_left: bool = False, **kwargs) -> None:
         wall_types = [WALL_TYPES[t][0] for t in types if t in WALL_TYPES]
         out_walls = {}
         for time_index, wall in sorted(self.walls.items()):
             if wall[0, 3] in wall_types:
-                wall = f(wall, *args, **kwargs)
+                wall = f(wall, *args, **kwargs)  # TODO: support mirror_left
                 out_walls[wall[0, 2]] = wall
             else:
                 out_walls[time_index] = wall
         self.walls = out_walls
 
-    def apply_for_all(self, f, *args, types: list = ALL_TYPES, **kwargs) -> None:
-        self.apply_for_notes(f, *args, types=types, **kwargs)
-        self.apply_for_walls(f, *args, types=types, **kwargs)
+    def apply_for_all(self, f, *args, types: list = ALL_TYPES, mirror_left: bool = False, **kwargs) -> None:
+        self.apply_for_notes(f, *args, types=types, mirror_left=mirror_left, **kwargs)
+        self.apply_for_walls(f, *args, types=types, mirror_left=mirror_left, **kwargs)
 
     # used when the functions needs access to all notes and rails of a color at one
-    def apply_for_note_types(self, f, *args, types: list = NOTE_TYPES, **kwargs) -> None:
+    def apply_for_note_types(self, f, *args, types: list = NOTE_TYPES, mirror_left: bool = False, **kwargs) -> None:
         for t in types:
             if t not in NOTE_TYPES:
                 continue
-            setattr(self, t, f(getattr(self, t), *args, **kwargs))
+            setattr(self, t, f(getattr(self, t), *args, direction=(-1 if mirror_left and t == "left" else 1), **kwargs))
 
     def filtered(self, types: list = ALL_TYPES) -> "DataContainer":
         replacement = {
             t: getattr(self, t) if t in types else {}
             for t in NOTE_TYPES
         }
         wall_types = [WALL_TYPES[t][0] for t in types if t in WALL_TYPES]
@@ -134,14 +134,24 @@
     def merge(self, other: "DataContainer") -> None:
         for t in NOTE_TYPES:
             self_notes = getattr(self, t)
             other_notes = getattr(other, t)
             setattr(self, t, self_notes | other_notes)
         self.walls |= other.walls
 
+    def get_object_dict(self, type_name: str) -> SINGLE_COLOR_NOTES | WALLS:
+        if type_name in NOTE_TYPES:
+            return getattr(self, type_name)
+        wall_type = WALL_TYPES[type_name][0]
+        return {
+            time_index: wall
+            for time_index, wall in sorted(self.walls.items())
+            if wall[0, 3] == wall_type
+        }
+
 @dataclasses.dataclass
 class ClipboardDataContainer(DataContainer):
     original_json: str
 
 @dataclasses.dataclass
 class SynthFile:
     input_file: Path
@@ -365,8 +375,8 @@
     clipboard["lenght"] = (last - first) * ms_per_min / data.bpm
 
     pyperclip.copy(json.dumps(clipboard))
 
 def import_file(file_path: Path) -> SynthFile:
     out = SynthFile(file_path, {}, {}, {})
     out.reload()
-    return out
+    return out
```

### Comparing `synth_mapping_helper-1.0.2/src/synth_mapping_helper/utils.py` & `synth_mapping_helper-1.1.0/src/synth_mapping_helper/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,18 +11,18 @@
         return new_times[:-1]
     # we overshot by less than an interval -> clamp last time to end
     new_times[-1] = end
     return new_times
 
 def parse_number(val: str) -> float:
     if "/" in val:
-        num, denom = val.split("/",1)
+        num, denom = val.split("/", 1)
         if " " in num:
             # mixed fraction, ie "1 1/2" -> 1.5
-            integer, num = num.split(" ",1)
+            integer, num = num.split(" ", 1)
             i = int(integer)
             return i + np.sign(i) * (float(num) / float(denom))
         return float(num) / float(denom)
     elif val.endswith("%"):
         return float(val[:-1]) / 100
     return float(val)
 
@@ -62,23 +62,29 @@
     # dummy class to hold numbers parsed as seconds until bpm was parsed
     def __init__(self, val: float) -> None:
         self.val = val
     def to_beat(self, bpm: float) -> float:
         return self.val / 60 * bpm
     def __str__(self) -> str:
         return f"{self.val}s"
+    def __repr__(self) -> str:
+        return f"{type(self).__name__}({self})"
+
+    def __repr__(self) -> str:
+        return f"{type(self).__name__}({self})"
+
 
 def parse_time(val: str) -> Union[float, SecondFloat]:
-    # note that there is no rounding here, 
+    # note that there is no rounding here,
     if val.endswith("s"):
         return SecondFloat(parse_number(val[:-1]))
     elif ":" in val:
         # parse mm:ss.fff into seconds
         m, s = val.rsplit(":", 1)
-        return SecondFloat(float(m)*60 + float(s))
+        return SecondFloat(float(m) * 60 + float(s))
     return parse_number(val)
 
 def parse_position(val: str) -> tuple[float, float, Union[float, SecondFloat]]:
     split = val.split(",")
     if len(split) != 3:
         raise ValueError("Must be in the form x,y,t")
     try:
@@ -89,8 +95,8 @@
         y = parse_number(split[1])
     except ValueError:
         raise ValueError("Error parsing y")
     try:
         t = parse_time(split[2])
     except ValueError:
         raise ValueError("Error parsing t")
-    return (x,y,t)
+    return (x, y, t)
```

### Comparing `synth_mapping_helper-1.0.2/src/synth_mapping_helper.egg-info/PKG-INFO` & `synth_mapping_helper-1.1.0/src/synth_mapping_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth-mapping-helper
-Version: 1.0.2
+Version: 1.1.0
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Home-page: https://github.com/adosikas/synth_mapping_helper
 Author: adosikas
 Author-email: 
 Project-URL: Documentation, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Bug Reports, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Source Code, https://github.com/adosikas/synth_mapping_helper
@@ -65,15 +65,15 @@
     * **Automatic backups** while mapping
     * Plot notes to spot outliers
     * View hand velocity and acceleration to find sections to smooth out
     * Show wall density and estimatation which ones will not render on quest
     * Fix **wall offset** between editor and game ("Finalize")
 
 ### Maybe (contributions welcome)
-* GUI for 
+* GUI for common operations
 * Automatic smoothing
 
 ## How to Install and use
 
 ### Advanced users
 * Install via `pip3 install synth_mapping_helper` (requires Python 3.9 or higher)
 * See `python3 -m synth_mapping_helper.cli -h` for usage of the clipboard manipulation
```

### Comparing `synth_mapping_helper-1.0.2/src/synth_mapping_helper.egg-info/SOURCES.txt` & `synth_mapping_helper-1.1.0/src/synth_mapping_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

