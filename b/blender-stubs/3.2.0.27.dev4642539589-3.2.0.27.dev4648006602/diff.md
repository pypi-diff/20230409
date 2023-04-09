# Comparing `tmp/blender-stubs-3.2.0.27.dev4642539589.tar.gz` & `tmp/blender-stubs-3.2.0.27.dev4648006602.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blender-stubs-3.2.0.27.dev4642539589.tar", last modified: Sat Apr  8 01:51:19 2023, max compression
+gzip compressed data, was "blender-stubs-3.2.0.27.dev4648006602.tar", last modified: Sun Apr  9 01:46:26 2023, max compression
```

## Comparing `blender-stubs-3.2.0.27.dev4642539589.tar` & `blender-stubs-3.2.0.27.dev4648006602.tar`

### file list

```diff
@@ -1,708 +1,708 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-08 01:51:18.000000 blender-stubs-3.2.0.27.dev4642539589/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.312612 blender-stubs-3.2.0.27.dev4642539589/attribute_curves_domain_items/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/attribute_curves_domain_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/attribute_curves_domain_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.312612 blender-stubs-3.2.0.27.dev4642539589/attribute_domain_items/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/attribute_domain_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/attribute_domain_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.312612 blender-stubs-3.2.0.27.dev4642539589/attribute_domain_only_mesh_items/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/attribute_domain_only_mesh_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/attribute_domain_only_mesh_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.312612 blender-stubs-3.2.0.27.dev4642539589/attribute_domain_with_auto_items/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/attribute_domain_with_auto_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/attribute_domain_with_auto_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.312612 blender-stubs-3.2.0.27.dev4642539589/attribute_domain_without_corner_items/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/attribute_domain_without_corner_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/attribute_domain_without_corner_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.312612 blender-stubs-3.2.0.27.dev4642539589/attribute_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/attribute_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/attribute_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.316612 blender-stubs-3.2.0.27.dev4642539589/attribute_type_with_auto_items/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/attribute_type_with_auto_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/attribute_type_with_auto_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.316612 blender-stubs-3.2.0.27.dev4642539589/axis_flag_xyz_items/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/axis_flag_xyz_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/axis_flag_xyz_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.316612 blender-stubs-3.2.0.27.dev4642539589/axis_xy_items/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/axis_xy_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/axis_xy_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.316612 blender-stubs-3.2.0.27.dev4642539589/axis_xyz_items/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/axis_xyz_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/axis_xyz_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.316612 blender-stubs-3.2.0.27.dev4642539589/bake_margin_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bake_margin_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bake_margin_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.316612 blender-stubs-3.2.0.27.dev4642539589/bake_pass_filter_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bake_pass_filter_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bake_pass_filter_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.316612 blender-stubs-3.2.0.27.dev4642539589/bake_pass_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bake_pass_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bake_pass_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.316612 blender-stubs-3.2.0.27.dev4642539589/bake_save_mode_items/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bake_save_mode_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bake_save_mode_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.316612 blender-stubs-3.2.0.27.dev4642539589/bake_target_items/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bake_target_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bake_target_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.316612 blender-stubs-3.2.0.27.dev4642539589/beztriple_interpolation_easing_items/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/beztriple_interpolation_easing_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/beztriple_interpolation_easing_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.316612 blender-stubs-3.2.0.27.dev4642539589/beztriple_interpolation_mode_items/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/beztriple_interpolation_mode_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/beztriple_interpolation_mode_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.316612 blender-stubs-3.2.0.27.dev4642539589/beztriple_keyframe_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/beztriple_keyframe_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/beztriple_keyframe_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.316612 blender-stubs-3.2.0.27.dev4642539589/bgl/
--rw-r--r--   0 runner    (1001) docker     (123)   144066 2023-04-08 01:50:21.000000 blender-stubs-3.2.0.27.dev4642539589/bgl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:50:21.000000 blender-stubs-3.2.0.27.dev4642539589/bgl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.316612 blender-stubs-3.2.0.27.dev4642539589/bl_math/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-08 01:50:21.000000 blender-stubs-3.2.0.27.dev4642539589/bl_math/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:50:21.000000 blender-stubs-3.2.0.27.dev4642539589/bl_math/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.320613 blender-stubs-3.2.0.27.dev4642539589/blender_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-08 01:51:19.000000 blender-stubs-3.2.0.27.dev4642539589/blender_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-04-08 01:51:19.000000 blender-stubs-3.2.0.27.dev4642539589/blender_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 01:51:19.000000 blender-stubs-3.2.0.27.dev4642539589/blender_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 01:51:19.000000 blender-stubs-3.2.0.27.dev4642539589/blender_stubs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-08 01:51:19.000000 blender-stubs-3.2.0.27.dev4642539589/blender_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.320613 blender-stubs-3.2.0.27.dev4642539589/blf/
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-08 01:50:21.000000 blender-stubs-3.2.0.27.dev4642539589/blf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:50:21.000000 blender-stubs-3.2.0.27.dev4642539589/blf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.320613 blender-stubs-3.2.0.27.dev4642539589/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bmesh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-08 01:50:21.000000 blender-stubs-3.2.0.27.dev4642539589/bmesh/geometry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    29607 2023-04-08 01:50:21.000000 blender-stubs-3.2.0.27.dev4642539589/bmesh/ops.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    32053 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bmesh/types.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bmesh/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.320613 blender-stubs-3.2.0.27.dev4642539589/boidrule_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/boidrule_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/boidrule_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.320613 blender-stubs-3.2.0.27.dev4642539589/bpy/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.320613 blender-stubs-3.2.0.27.dev4642539589/bpy/app/
--rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/app/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/app/handlers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/app/icons.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/app/timers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/app/translations.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/context.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/msgbus.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.328612 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-04-08 01:50:26.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/action.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/anim.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/armature.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/asset.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/boid.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/brush.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/buttons.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/cachefile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/camera.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14795 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/clip.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/cloth.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-08 01:50:22.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/collection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/console.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/constraint.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/curve.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/curves.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/dpaint.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/ed.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/file.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/fluid.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/font.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/geometry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/gizmogroup.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    26622 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/gpencil.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/graph.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/image.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/lattice.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/marker.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/mask.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/material.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-08 01:50:23.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/mball.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    36868 2023-04-08 01:50:24.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/mesh.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-08 01:50:24.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/nla.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14520 2023-04-08 01:50:24.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/node.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    44071 2023-04-08 01:50:24.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/object.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/outliner.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/paint.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/paintcurve.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/palette.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/particle.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/pose.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/poselib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/preferences.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/ptcache.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/render.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/rigidbody.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/scene.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/screen.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/script.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/sculpt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/sculpt_curves.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/sequencer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/sound.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/spreadsheet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/surface.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-08 01:50:25.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/texture.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-04-08 01:50:26.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/transform.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-08 01:50:26.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/ui.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-08 01:50:26.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/uilist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-04-08 01:50:26.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/uv.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-08 01:50:26.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/view2d.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-08 01:50:26.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/view3d.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28866 2023-04-08 01:50:26.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/wm.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-08 01:50:26.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/workspace.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-08 01:50:26.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/ops/world.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-08 01:50:26.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/path.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-04-08 01:50:26.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/props.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)  1757345 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/types.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.328612 blender-stubs-3.2.0.27.dev4642539589/bpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/utils/previews.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bpy/utils/units.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.328612 blender-stubs-3.2.0.27.dev4642539589/bpy_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bpy_extras/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bpy_extras/anim_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bpy_extras/asset_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bpy_extras/id_map_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bpy_extras/image_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bpy_extras/io_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bpy_extras/keyconfig_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bpy_extras/mesh_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bpy_extras/node_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bpy_extras/object_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bpy_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/bpy_extras/view3d_utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/brush_automasking_flag_items/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_automasking_flag_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_automasking_flag_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/brush_curves_sculpt_tool_items/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_curves_sculpt_tool_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_curves_sculpt_tool_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/brush_gpencil_sculpt_types_items/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_gpencil_sculpt_types_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_gpencil_sculpt_types_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/brush_gpencil_types_items/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_gpencil_types_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_gpencil_types_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/brush_gpencil_vertex_types_items/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_gpencil_vertex_types_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_gpencil_vertex_types_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/brush_gpencil_weight_types_items/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_gpencil_weight_types_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_gpencil_weight_types_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/brush_image_tool_items/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_image_tool_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_image_tool_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/brush_sculpt_tool_items/
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_sculpt_tool_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_sculpt_tool_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/brush_uv_sculpt_tool_items/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_uv_sculpt_tool_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_uv_sculpt_tool_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/brush_vertex_tool_items/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_vertex_tool_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_vertex_tool_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/brush_weight_tool_items/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_weight_tool_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/brush_weight_tool_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/clip_editor_mode_items/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/clip_editor_mode_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/clip_editor_mode_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/collection_color_items/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/collection_color_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/collection_color_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/color_attribute_domain_items/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/color_attribute_domain_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/color_attribute_domain_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/color_attribute_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/color_attribute_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/color_attribute_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/color_sets_items/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/color_sets_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/color_sets_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/color_space_convert_default_items/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/color_space_convert_default_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/color_space_convert_default_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/constraint_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/constraint_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/constraint_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/context_mode_items/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/context_mode_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/context_mode_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/curve_fit_method_items/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/curve_fit_method_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/curve_fit_method_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/curve_normal_modes/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/curve_normal_modes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/curve_normal_modes/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/curves_types/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/curves_types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/curves_types/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.332613 blender-stubs-3.2.0.27.dev4642539589/driver_target_rotation_mode_items/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/driver_target_rotation_mode_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/driver_target_rotation_mode_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.336613 blender-stubs-3.2.0.27.dev4642539589/dt_layers_select_dst_items/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/dt_layers_select_dst_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/dt_layers_select_dst_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.336613 blender-stubs-3.2.0.27.dev4642539589/dt_layers_select_src_items/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/dt_layers_select_src_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/dt_layers_select_src_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.336613 blender-stubs-3.2.0.27.dev4642539589/dt_method_edge_items/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/dt_method_edge_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/dt_method_edge_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.336613 blender-stubs-3.2.0.27.dev4642539589/dt_method_loop_items/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/dt_method_loop_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/dt_method_loop_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.336613 blender-stubs-3.2.0.27.dev4642539589/dt_method_poly_items/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/dt_method_poly_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/dt_method_poly_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.336613 blender-stubs-3.2.0.27.dev4642539589/dt_method_vertex_items/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/dt_method_vertex_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/dt_method_vertex_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.336613 blender-stubs-3.2.0.27.dev4642539589/dt_mix_mode_items/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/dt_mix_mode_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/dt_mix_mode_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.336613 blender-stubs-3.2.0.27.dev4642539589/event_direction_items/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/event_direction_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/event_direction_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.336613 blender-stubs-3.2.0.27.dev4642539589/event_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/event_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/event_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.336613 blender-stubs-3.2.0.27.dev4642539589/event_type_mask_items/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/event_type_mask_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/event_type_mask_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.336613 blender-stubs-3.2.0.27.dev4642539589/event_value_items/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/event_value_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/event_value_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.336613 blender-stubs-3.2.0.27.dev4642539589/exr_codec_items/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/exr_codec_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/exr_codec_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.336613 blender-stubs-3.2.0.27.dev4642539589/fcurve_auto_smoothing_items/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/fcurve_auto_smoothing_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/fcurve_auto_smoothing_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.336613 blender-stubs-3.2.0.27.dev4642539589/fileselect_params_sort_items/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/fileselect_params_sort_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/fileselect_params_sort_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.336613 blender-stubs-3.2.0.27.dev4642539589/fmodifier_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/fmodifier_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/fmodifier_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.336613 blender-stubs-3.2.0.27.dev4642539589/freestyle/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/freestyle/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/freestyle/chainingiterators.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    34233 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/freestyle/functions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/freestyle/predicates.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/freestyle/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18843 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/freestyle/shaders.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    75927 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/freestyle/types.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/freestyle/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.336613 blender-stubs-3.2.0.27.dev4642539589/geometry_component_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/geometry_component_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/geometry_component_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.340613 blender-stubs-3.2.0.27.dev4642539589/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)    18995 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/gpu/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/gpu/capabilities.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/gpu/matrix.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/gpu/platform.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/gpu/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/gpu/select.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/gpu/shader.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/gpu/state.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/gpu/texture.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17826 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/gpu/types.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.340613 blender-stubs-3.2.0.27.dev4642539589/gpu_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/gpu_extras/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/gpu_extras/batch.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/gpu_extras/presets.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/gpu_extras/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.340613 blender-stubs-3.2.0.27.dev4642539589/icon_items/
--rw-r--r--   0 runner    (1001) docker     (123)    30503 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/icon_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/icon_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.340613 blender-stubs-3.2.0.27.dev4642539589/id_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/id_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/id_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.340613 blender-stubs-3.2.0.27.dev4642539589/idprop/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/idprop/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/idprop/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/idprop/types.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.340613 blender-stubs-3.2.0.27.dev4642539589/image_color_depth_items/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/image_color_depth_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/image_color_depth_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.340613 blender-stubs-3.2.0.27.dev4642539589/image_color_mode_items/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/image_color_mode_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/image_color_mode_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.340613 blender-stubs-3.2.0.27.dev4642539589/image_generated_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/image_generated_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/image_generated_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.340613 blender-stubs-3.2.0.27.dev4642539589/image_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/image_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/image_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.340613 blender-stubs-3.2.0.27.dev4642539589/imbuf/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/imbuf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/imbuf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/imbuf/types.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.340613 blender-stubs-3.2.0.27.dev4642539589/info_advanced/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/info_advanced/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/info_advanced/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.340613 blender-stubs-3.2.0.27.dev4642539589/info_advanced_blender_as_bpy/
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/info_advanced_blender_as_bpy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/info_advanced_blender_as_bpy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.340613 blender-stubs-3.2.0.27.dev4642539589/keyblock_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/keyblock_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/keyblock_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.340613 blender-stubs-3.2.0.27.dev4642539589/keyframe_handle_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/keyframe_handle_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/keyframe_handle_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.340613 blender-stubs-3.2.0.27.dev4642539589/keyframe_paste_merge_items/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/keyframe_paste_merge_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/keyframe_paste_merge_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.340613 blender-stubs-3.2.0.27.dev4642539589/keyframe_paste_offset_items/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/keyframe_paste_offset_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/keyframe_paste_offset_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.340613 blender-stubs-3.2.0.27.dev4642539589/keyframe_paste_offset_value/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/keyframe_paste_offset_value/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/keyframe_paste_offset_value/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.340613 blender-stubs-3.2.0.27.dev4642539589/keying_flag_items/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/keying_flag_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/keying_flag_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/keying_flag_items_api/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/keying_flag_items_api/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:09.000000 blender-stubs-3.2.0.27.dev4642539589/keying_flag_items_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/keyingset_path_grouping_items/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/keyingset_path_grouping_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/keyingset_path_grouping_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/keymap_propvalue_items/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/keymap_propvalue_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/keymap_propvalue_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/light_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/light_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/light_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/lightprobes_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/lightprobes_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/lightprobes_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/linestyle_alpha_modifier_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/linestyle_alpha_modifier_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/linestyle_alpha_modifier_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/linestyle_color_modifier_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/linestyle_color_modifier_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/linestyle_color_modifier_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/linestyle_geometry_modifier_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/linestyle_geometry_modifier_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/linestyle_geometry_modifier_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/linestyle_thickness_modifier_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/linestyle_thickness_modifier_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/linestyle_thickness_modifier_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/mapping_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/mapping_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/mapping_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/mathutils/
--rw-r--r--   0 runner    (1001) docker     (123)    73710 2023-04-08 01:51:12.000000 blender-stubs-3.2.0.27.dev4642539589/mathutils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/mathutils/bvhtree.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/mathutils/geometry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/mathutils/interpolate.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/mathutils/kdtree.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-08 01:51:11.000000 blender-stubs-3.2.0.27.dev4642539589/mathutils/noise.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:12.000000 blender-stubs-3.2.0.27.dev4642539589/mathutils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/mesh_delimit_mode_items/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/mesh_delimit_mode_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/mesh_delimit_mode_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/mesh_select_mode_items/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/mesh_select_mode_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/mesh_select_mode_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/mesh_select_mode_uv_items/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/mesh_select_mode_uv_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/mesh_select_mode_uv_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/metaelem_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/metaelem_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/metaelem_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/modifier_shrinkwrap_mode_items/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/modifier_shrinkwrap_mode_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/modifier_shrinkwrap_mode_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/modifier_triangulate_ngon_method_items/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/modifier_triangulate_ngon_method_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/modifier_triangulate_ngon_method_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/modifier_triangulate_quad_method_items/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/modifier_triangulate_quad_method_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/modifier_triangulate_quad_method_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/motionpath_bake_location_items/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/motionpath_bake_location_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/motionpath_bake_location_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.344613 blender-stubs-3.2.0.27.dev4642539589/motionpath_display_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/motionpath_display_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/motionpath_display_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/motionpath_range_items/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/motionpath_range_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/motionpath_range_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/navigation_mode_items/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/navigation_mode_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/navigation_mode_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/nla_mode_blend_items/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/nla_mode_blend_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/nla_mode_blend_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/nla_mode_extend_items/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/nla_mode_extend_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/nla_mode_extend_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/node_boolean_math_items/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_boolean_math_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_boolean_math_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/node_clamp_items/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_clamp_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_clamp_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/node_compare_operation_items/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_compare_operation_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_compare_operation_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/node_filter_items/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_filter_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_filter_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/node_float_compare_items/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_float_compare_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_float_compare_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/node_float_to_int_items/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_float_to_int_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_float_to_int_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/node_map_range_items/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_map_range_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_map_range_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/node_math_items/
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_math_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_math_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/node_socket_in_out_items/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_socket_in_out_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_socket_in_out_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/node_vec_math_items/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_vec_math_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/node_vec_math_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/normal_space_items/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/normal_space_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/normal_space_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/normal_swizzle_items/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/normal_swizzle_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/normal_swizzle_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/object_axis_items/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_axis_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_axis_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/object_empty_drawtype_items/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_empty_drawtype_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_empty_drawtype_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/object_gpencil_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_gpencil_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_gpencil_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/object_greasepencil_modifier_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_greasepencil_modifier_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_greasepencil_modifier_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/object_mode_items/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_mode_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_mode_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/object_modifier_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_modifier_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_modifier_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/object_rotation_mode_items/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_rotation_mode_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_rotation_mode_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.348613 blender-stubs-3.2.0.27.dev4642539589/object_shaderfx_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_shaderfx_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_shaderfx_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/object_type_curve_items/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_type_curve_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_type_curve_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/object_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/object_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/operator_context_items/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/operator_context_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/operator_context_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/operator_property_tags/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/operator_property_tags/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/operator_property_tags/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/operator_return_items/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/operator_return_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/operator_return_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/operator_type_flag_items/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/operator_type_flag_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/operator_type_flag_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/particle_edit_disconnected_hair_brush_items/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/particle_edit_disconnected_hair_brush_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/particle_edit_disconnected_hair_brush_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/particle_edit_hair_brush_items/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/particle_edit_hair_brush_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/particle_edit_hair_brush_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/preference_section_items/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/preference_section_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/preference_section_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/prop_dynamicpaint_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/prop_dynamicpaint_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/prop_dynamicpaint_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/property_flag_enum_items/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_flag_enum_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_flag_enum_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/property_flag_items/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_flag_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_flag_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/property_override_flag_collection_items/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_override_flag_collection_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_override_flag_collection_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/property_override_flag_items/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_override_flag_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_override_flag_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/property_string_search_flag_items/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_string_search_flag_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_string_search_flag_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/property_subtype_items/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_subtype_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_subtype_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/property_subtype_number_array_items/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_subtype_number_array_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_subtype_number_array_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/property_subtype_number_items/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_subtype_number_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_subtype_number_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/property_subtype_string_items/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_subtype_string_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_subtype_string_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/property_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/property_unit_items/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_unit_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/property_unit_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.352613 blender-stubs-3.2.0.27.dev4642539589/proportional_falloff_curve_only_items/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/proportional_falloff_curve_only_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/proportional_falloff_curve_only_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/proportional_falloff_items/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/proportional_falloff_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/proportional_falloff_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/ramp_blend_items/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/ramp_blend_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/ramp_blend_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/region_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/region_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/region_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/render_pass_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/render_pass_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/render_pass_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/rigidbody_constraint_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/rigidbody_constraint_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/rigidbody_constraint_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/rigidbody_object_shape_items/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/rigidbody_object_shape_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/rigidbody_object_shape_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/rigidbody_object_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/rigidbody_object_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/rigidbody_object_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/sequence_modifier_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/sequence_modifier_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/sequence_modifier_type_items/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-08 01:51:18.000000 blender-stubs-3.2.0.27.dev4642539589/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/shading_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/shading_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/shading_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/shrinkwrap_face_cull_items/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/shrinkwrap_face_cull_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/shrinkwrap_face_cull_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/shrinkwrap_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/shrinkwrap_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/shrinkwrap_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/snap_element_items/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/snap_element_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/snap_element_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/snap_node_element_items/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/snap_node_element_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/snap_node_element_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/snap_source_items/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/snap_source_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/snap_source_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/space_action_mode_items/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/space_action_mode_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/space_action_mode_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/space_file_browse_mode_items/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/space_file_browse_mode_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/space_file_browse_mode_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/space_graph_mode_items/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/space_graph_mode_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/space_graph_mode_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/space_image_mode_all_items/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/space_image_mode_all_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/space_image_mode_all_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/space_image_mode_items/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/space_image_mode_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/space_image_mode_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/space_sequencer_view_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/space_sequencer_view_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/space_sequencer_view_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/space_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/space_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/space_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/stereo3d_anaglyph_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/stereo3d_anaglyph_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/stereo3d_anaglyph_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.356613 blender-stubs-3.2.0.27.dev4642539589/stereo3d_display_items/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/stereo3d_display_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/stereo3d_display_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/stereo3d_interlace_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/stereo3d_interlace_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/stereo3d_interlace_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/strip_color_items/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/strip_color_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/strip_color_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/subdivision_boundary_smooth_items/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/subdivision_boundary_smooth_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/subdivision_boundary_smooth_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/subdivision_uv_smooth_items/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/subdivision_uv_smooth_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/subdivision_uv_smooth_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/symmetrize_direction_items/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/symmetrize_direction_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/symmetrize_direction_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/texture_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/texture_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/texture_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/transform_mode_types/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/transform_mode_types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/transform_mode_types/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/transform_orientation_items/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/transform_orientation_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/transform_orientation_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/transform_pivot_items_full/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/transform_pivot_items_full/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/transform_pivot_items_full/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/uilist_layout_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/uilist_layout_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/uilist_layout_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/unpack_method_items/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/unpack_method_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/unpack_method_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/velocity_unit_items/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/velocity_unit_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/velocity_unit_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/views_format_items/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/views_format_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/views_format_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/views_format_multilayer_items/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/views_format_multilayer_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/views_format_multilayer_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/views_format_multiview_items/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/views_format_multiview_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/views_format_multiview_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/volume_grid_data_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/volume_grid_data_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/volume_grid_data_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/window_cursor_items/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/window_cursor_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/window_cursor_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/wm_job_type_items/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/wm_job_type_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/wm_job_type_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/wm_report_items/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/wm_report_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/wm_report_items/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:19.360613 blender-stubs-3.2.0.27.dev4642539589/workspace_object_mode_items/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/workspace_object_mode_items/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:51:10.000000 blender-stubs-3.2.0.27.dev4642539589/workspace_object_mode_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.170572 blender-stubs-3.2.0.27.dev4648006602/
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-09 01:46:26.166572 blender-stubs-3.2.0.27.dev4648006602/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-09 01:46:25.000000 blender-stubs-3.2.0.27.dev4648006602/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.090572 blender-stubs-3.2.0.27.dev4648006602/attribute_curves_domain_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/attribute_curves_domain_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/attribute_curves_domain_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.090572 blender-stubs-3.2.0.27.dev4648006602/attribute_domain_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/attribute_domain_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/attribute_domain_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.090572 blender-stubs-3.2.0.27.dev4648006602/attribute_domain_only_mesh_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/attribute_domain_only_mesh_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/attribute_domain_only_mesh_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.090572 blender-stubs-3.2.0.27.dev4648006602/attribute_domain_with_auto_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/attribute_domain_with_auto_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/attribute_domain_with_auto_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.090572 blender-stubs-3.2.0.27.dev4648006602/attribute_domain_without_corner_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/attribute_domain_without_corner_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/attribute_domain_without_corner_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.090572 blender-stubs-3.2.0.27.dev4648006602/attribute_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/attribute_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/attribute_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.090572 blender-stubs-3.2.0.27.dev4648006602/attribute_type_with_auto_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/attribute_type_with_auto_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/attribute_type_with_auto_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.090572 blender-stubs-3.2.0.27.dev4648006602/axis_flag_xyz_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/axis_flag_xyz_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/axis_flag_xyz_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.090572 blender-stubs-3.2.0.27.dev4648006602/axis_xy_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/axis_xy_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/axis_xy_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.090572 blender-stubs-3.2.0.27.dev4648006602/axis_xyz_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/axis_xyz_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/axis_xyz_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.090572 blender-stubs-3.2.0.27.dev4648006602/bake_margin_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bake_margin_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bake_margin_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.090572 blender-stubs-3.2.0.27.dev4648006602/bake_pass_filter_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bake_pass_filter_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bake_pass_filter_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.090572 blender-stubs-3.2.0.27.dev4648006602/bake_pass_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bake_pass_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bake_pass_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.094572 blender-stubs-3.2.0.27.dev4648006602/bake_save_mode_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bake_save_mode_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bake_save_mode_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.094572 blender-stubs-3.2.0.27.dev4648006602/bake_target_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bake_target_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bake_target_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.094572 blender-stubs-3.2.0.27.dev4648006602/beztriple_interpolation_easing_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/beztriple_interpolation_easing_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/beztriple_interpolation_easing_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.094572 blender-stubs-3.2.0.27.dev4648006602/beztriple_interpolation_mode_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/beztriple_interpolation_mode_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/beztriple_interpolation_mode_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.094572 blender-stubs-3.2.0.27.dev4648006602/beztriple_keyframe_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/beztriple_keyframe_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/beztriple_keyframe_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.094572 blender-stubs-3.2.0.27.dev4648006602/bgl/
+-rw-r--r--   0 runner    (1001) docker     (123)   144066 2023-04-09 01:45:15.000000 blender-stubs-3.2.0.27.dev4648006602/bgl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:45:15.000000 blender-stubs-3.2.0.27.dev4648006602/bgl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.094572 blender-stubs-3.2.0.27.dev4648006602/bl_math/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-09 01:45:15.000000 blender-stubs-3.2.0.27.dev4648006602/bl_math/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:45:15.000000 blender-stubs-3.2.0.27.dev4648006602/bl_math/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.094572 blender-stubs-3.2.0.27.dev4648006602/blender_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-09 01:46:25.000000 blender-stubs-3.2.0.27.dev4648006602/blender_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-04-09 01:46:26.000000 blender-stubs-3.2.0.27.dev4648006602/blender_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 01:46:25.000000 blender-stubs-3.2.0.27.dev4648006602/blender_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 01:46:25.000000 blender-stubs-3.2.0.27.dev4648006602/blender_stubs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-09 01:46:25.000000 blender-stubs-3.2.0.27.dev4648006602/blender_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.094572 blender-stubs-3.2.0.27.dev4648006602/blf/
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-09 01:45:15.000000 blender-stubs-3.2.0.27.dev4648006602/blf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:45:15.000000 blender-stubs-3.2.0.27.dev4648006602/blf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.098572 blender-stubs-3.2.0.27.dev4648006602/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bmesh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-09 01:45:15.000000 blender-stubs-3.2.0.27.dev4648006602/bmesh/geometry.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    29607 2023-04-09 01:45:15.000000 blender-stubs-3.2.0.27.dev4648006602/bmesh/ops.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    32053 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bmesh/types.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bmesh/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.098572 blender-stubs-3.2.0.27.dev4648006602/boidrule_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/boidrule_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/boidrule_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.098572 blender-stubs-3.2.0.27.dev4648006602/bpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.102572 blender-stubs-3.2.0.27.dev4648006602/bpy/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/app/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/app/handlers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/app/icons.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/app/timers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/app/translations.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/msgbus.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.110572 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-04-09 01:45:22.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/action.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/anim.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/armature.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/asset.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/boid.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/brush.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/buttons.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/cachefile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/camera.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14795 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/clip.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/cloth.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-09 01:45:16.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/console.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-09 01:45:17.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/constraint.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-04-09 01:45:17.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/curve.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-09 01:45:17.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/curves.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-09 01:45:17.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/dpaint.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-04-09 01:45:17.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/ed.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-09 01:45:17.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/file.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-09 01:45:17.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/fluid.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-09 01:45:17.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/font.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-09 01:45:17.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/geometry.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-09 01:45:17.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/gizmogroup.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26622 2023-04-09 01:45:17.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/gpencil.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-04-09 01:45:17.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/graph.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-04-09 01:45:18.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/image.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-09 01:45:18.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-09 01:45:18.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/lattice.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-09 01:45:18.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/marker.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-09 01:45:18.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/mask.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-09 01:45:18.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/material.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-09 01:45:18.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/mball.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    36868 2023-04-09 01:45:18.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/mesh.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-09 01:45:18.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/nla.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14520 2023-04-09 01:45:19.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/node.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    44071 2023-04-09 01:45:19.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/object.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-04-09 01:45:19.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/outliner.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-09 01:45:19.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/paint.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-09 01:45:19.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/paintcurve.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-09 01:45:19.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/palette.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-09 01:45:19.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/particle.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-04-09 01:45:20.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/pose.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-09 01:45:20.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/poselib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-04-09 01:45:20.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/preferences.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-09 01:45:20.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/ptcache.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-09 01:45:20.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/render.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-09 01:45:20.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/rigidbody.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-09 01:45:20.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/scene.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-04-09 01:45:20.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/screen.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-09 01:45:20.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/script.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-04-09 01:45:20.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/sculpt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-09 01:45:20.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/sculpt_curves.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-04-09 01:45:20.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/sequencer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-09 01:45:20.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/sound.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-09 01:45:20.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/spreadsheet.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-09 01:45:20.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/surface.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-09 01:45:20.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-09 01:45:20.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/texture.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-04-09 01:45:21.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/transform.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-09 01:45:21.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/ui.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-09 01:45:21.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/uilist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-04-09 01:45:21.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/uv.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-09 01:45:21.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/view2d.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-09 01:45:21.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/view3d.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    28866 2023-04-09 01:45:21.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/wm.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-09 01:45:21.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/workspace.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-09 01:45:21.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/ops/world.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-09 01:45:22.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/path.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-04-09 01:45:22.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/props.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)  1757345 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/types.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.114572 blender-stubs-3.2.0.27.dev4648006602/bpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/utils/previews.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bpy/utils/units.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.114572 blender-stubs-3.2.0.27.dev4648006602/bpy_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bpy_extras/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bpy_extras/anim_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bpy_extras/asset_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bpy_extras/id_map_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bpy_extras/image_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bpy_extras/io_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bpy_extras/keyconfig_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bpy_extras/mesh_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bpy_extras/node_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bpy_extras/object_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bpy_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/bpy_extras/view3d_utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.114572 blender-stubs-3.2.0.27.dev4648006602/brush_automasking_flag_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_automasking_flag_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_automasking_flag_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.114572 blender-stubs-3.2.0.27.dev4648006602/brush_curves_sculpt_tool_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_curves_sculpt_tool_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_curves_sculpt_tool_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.114572 blender-stubs-3.2.0.27.dev4648006602/brush_gpencil_sculpt_types_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_gpencil_sculpt_types_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_gpencil_sculpt_types_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.114572 blender-stubs-3.2.0.27.dev4648006602/brush_gpencil_types_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_gpencil_types_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_gpencil_types_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.114572 blender-stubs-3.2.0.27.dev4648006602/brush_gpencil_vertex_types_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_gpencil_vertex_types_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_gpencil_vertex_types_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.114572 blender-stubs-3.2.0.27.dev4648006602/brush_gpencil_weight_types_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_gpencil_weight_types_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_gpencil_weight_types_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.118572 blender-stubs-3.2.0.27.dev4648006602/brush_image_tool_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_image_tool_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_image_tool_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.118572 blender-stubs-3.2.0.27.dev4648006602/brush_sculpt_tool_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_sculpt_tool_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_sculpt_tool_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.118572 blender-stubs-3.2.0.27.dev4648006602/brush_uv_sculpt_tool_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_uv_sculpt_tool_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_uv_sculpt_tool_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.118572 blender-stubs-3.2.0.27.dev4648006602/brush_vertex_tool_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_vertex_tool_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_vertex_tool_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.118572 blender-stubs-3.2.0.27.dev4648006602/brush_weight_tool_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_weight_tool_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/brush_weight_tool_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.118572 blender-stubs-3.2.0.27.dev4648006602/clip_editor_mode_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/clip_editor_mode_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/clip_editor_mode_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.118572 blender-stubs-3.2.0.27.dev4648006602/collection_color_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/collection_color_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/collection_color_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.118572 blender-stubs-3.2.0.27.dev4648006602/color_attribute_domain_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/color_attribute_domain_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/color_attribute_domain_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.118572 blender-stubs-3.2.0.27.dev4648006602/color_attribute_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/color_attribute_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/color_attribute_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.118572 blender-stubs-3.2.0.27.dev4648006602/color_sets_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/color_sets_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/color_sets_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.118572 blender-stubs-3.2.0.27.dev4648006602/color_space_convert_default_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/color_space_convert_default_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/color_space_convert_default_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.118572 blender-stubs-3.2.0.27.dev4648006602/constraint_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/constraint_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/constraint_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.118572 blender-stubs-3.2.0.27.dev4648006602/context_mode_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/context_mode_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/context_mode_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.118572 blender-stubs-3.2.0.27.dev4648006602/curve_fit_method_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/curve_fit_method_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/curve_fit_method_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.122572 blender-stubs-3.2.0.27.dev4648006602/curve_normal_modes/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/curve_normal_modes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/curve_normal_modes/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.122572 blender-stubs-3.2.0.27.dev4648006602/curves_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/curves_types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/curves_types/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.122572 blender-stubs-3.2.0.27.dev4648006602/driver_target_rotation_mode_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/driver_target_rotation_mode_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/driver_target_rotation_mode_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.122572 blender-stubs-3.2.0.27.dev4648006602/dt_layers_select_dst_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/dt_layers_select_dst_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/dt_layers_select_dst_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.122572 blender-stubs-3.2.0.27.dev4648006602/dt_layers_select_src_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/dt_layers_select_src_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/dt_layers_select_src_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.122572 blender-stubs-3.2.0.27.dev4648006602/dt_method_edge_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/dt_method_edge_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/dt_method_edge_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.122572 blender-stubs-3.2.0.27.dev4648006602/dt_method_loop_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/dt_method_loop_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/dt_method_loop_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.122572 blender-stubs-3.2.0.27.dev4648006602/dt_method_poly_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/dt_method_poly_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/dt_method_poly_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.122572 blender-stubs-3.2.0.27.dev4648006602/dt_method_vertex_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/dt_method_vertex_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/dt_method_vertex_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.122572 blender-stubs-3.2.0.27.dev4648006602/dt_mix_mode_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/dt_mix_mode_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/dt_mix_mode_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.122572 blender-stubs-3.2.0.27.dev4648006602/event_direction_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/event_direction_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:14.000000 blender-stubs-3.2.0.27.dev4648006602/event_direction_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.122572 blender-stubs-3.2.0.27.dev4648006602/event_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/event_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/event_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.122572 blender-stubs-3.2.0.27.dev4648006602/event_type_mask_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/event_type_mask_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/event_type_mask_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.122572 blender-stubs-3.2.0.27.dev4648006602/event_value_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/event_value_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/event_value_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.122572 blender-stubs-3.2.0.27.dev4648006602/exr_codec_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/exr_codec_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/exr_codec_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.126572 blender-stubs-3.2.0.27.dev4648006602/fcurve_auto_smoothing_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/fcurve_auto_smoothing_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/fcurve_auto_smoothing_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.126572 blender-stubs-3.2.0.27.dev4648006602/fileselect_params_sort_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/fileselect_params_sort_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/fileselect_params_sort_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.126572 blender-stubs-3.2.0.27.dev4648006602/fmodifier_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/fmodifier_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/fmodifier_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.126572 blender-stubs-3.2.0.27.dev4648006602/freestyle/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/freestyle/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/freestyle/chainingiterators.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    34233 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/freestyle/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/freestyle/predicates.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/freestyle/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18843 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/freestyle/shaders.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    75927 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/freestyle/types.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/freestyle/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.126572 blender-stubs-3.2.0.27.dev4648006602/geometry_component_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/geometry_component_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/geometry_component_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.130572 blender-stubs-3.2.0.27.dev4648006602/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)    18995 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/gpu/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/gpu/capabilities.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/gpu/matrix.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/gpu/platform.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/gpu/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/gpu/select.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/gpu/shader.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/gpu/state.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/gpu/texture.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17826 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/gpu/types.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.130572 blender-stubs-3.2.0.27.dev4648006602/gpu_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/gpu_extras/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/gpu_extras/batch.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/gpu_extras/presets.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/gpu_extras/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.130572 blender-stubs-3.2.0.27.dev4648006602/icon_items/
+-rw-r--r--   0 runner    (1001) docker     (123)    30503 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/icon_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/icon_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.130572 blender-stubs-3.2.0.27.dev4648006602/id_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/id_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/id_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.130572 blender-stubs-3.2.0.27.dev4648006602/idprop/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/idprop/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/idprop/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/idprop/types.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.130572 blender-stubs-3.2.0.27.dev4648006602/image_color_depth_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/image_color_depth_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/image_color_depth_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.130572 blender-stubs-3.2.0.27.dev4648006602/image_color_mode_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/image_color_mode_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/image_color_mode_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.130572 blender-stubs-3.2.0.27.dev4648006602/image_generated_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/image_generated_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/image_generated_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.130572 blender-stubs-3.2.0.27.dev4648006602/image_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/image_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/image_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.130572 blender-stubs-3.2.0.27.dev4648006602/imbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/imbuf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/imbuf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/imbuf/types.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.130572 blender-stubs-3.2.0.27.dev4648006602/info_advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/info_advanced/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/info_advanced/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.134572 blender-stubs-3.2.0.27.dev4648006602/info_advanced_blender_as_bpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/info_advanced_blender_as_bpy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/info_advanced_blender_as_bpy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.134572 blender-stubs-3.2.0.27.dev4648006602/keyblock_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/keyblock_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/keyblock_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.134572 blender-stubs-3.2.0.27.dev4648006602/keyframe_handle_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/keyframe_handle_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/keyframe_handle_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.134572 blender-stubs-3.2.0.27.dev4648006602/keyframe_paste_merge_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/keyframe_paste_merge_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/keyframe_paste_merge_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.134572 blender-stubs-3.2.0.27.dev4648006602/keyframe_paste_offset_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/keyframe_paste_offset_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/keyframe_paste_offset_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.134572 blender-stubs-3.2.0.27.dev4648006602/keyframe_paste_offset_value/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/keyframe_paste_offset_value/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/keyframe_paste_offset_value/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.134572 blender-stubs-3.2.0.27.dev4648006602/keying_flag_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/keying_flag_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/keying_flag_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.134572 blender-stubs-3.2.0.27.dev4648006602/keying_flag_items_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/keying_flag_items_api/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/keying_flag_items_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.134572 blender-stubs-3.2.0.27.dev4648006602/keyingset_path_grouping_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/keyingset_path_grouping_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/keyingset_path_grouping_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.134572 blender-stubs-3.2.0.27.dev4648006602/keymap_propvalue_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/keymap_propvalue_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/keymap_propvalue_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.134572 blender-stubs-3.2.0.27.dev4648006602/light_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/light_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/light_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.134572 blender-stubs-3.2.0.27.dev4648006602/lightprobes_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/lightprobes_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/lightprobes_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.138572 blender-stubs-3.2.0.27.dev4648006602/linestyle_alpha_modifier_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/linestyle_alpha_modifier_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/linestyle_alpha_modifier_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.138572 blender-stubs-3.2.0.27.dev4648006602/linestyle_color_modifier_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/linestyle_color_modifier_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/linestyle_color_modifier_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.138572 blender-stubs-3.2.0.27.dev4648006602/linestyle_geometry_modifier_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/linestyle_geometry_modifier_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/linestyle_geometry_modifier_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.138572 blender-stubs-3.2.0.27.dev4648006602/linestyle_thickness_modifier_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/linestyle_thickness_modifier_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/linestyle_thickness_modifier_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.138572 blender-stubs-3.2.0.27.dev4648006602/mapping_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/mapping_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/mapping_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.138572 blender-stubs-3.2.0.27.dev4648006602/mathutils/
+-rw-r--r--   0 runner    (1001) docker     (123)    73710 2023-04-09 01:46:18.000000 blender-stubs-3.2.0.27.dev4648006602/mathutils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/mathutils/bvhtree.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/mathutils/geometry.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/mathutils/interpolate.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/mathutils/kdtree.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-09 01:46:17.000000 blender-stubs-3.2.0.27.dev4648006602/mathutils/noise.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:18.000000 blender-stubs-3.2.0.27.dev4648006602/mathutils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.138572 blender-stubs-3.2.0.27.dev4648006602/mesh_delimit_mode_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/mesh_delimit_mode_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/mesh_delimit_mode_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.138572 blender-stubs-3.2.0.27.dev4648006602/mesh_select_mode_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/mesh_select_mode_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/mesh_select_mode_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.138572 blender-stubs-3.2.0.27.dev4648006602/mesh_select_mode_uv_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/mesh_select_mode_uv_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/mesh_select_mode_uv_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.138572 blender-stubs-3.2.0.27.dev4648006602/metaelem_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/metaelem_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/metaelem_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.138572 blender-stubs-3.2.0.27.dev4648006602/modifier_shrinkwrap_mode_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/modifier_shrinkwrap_mode_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/modifier_shrinkwrap_mode_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.138572 blender-stubs-3.2.0.27.dev4648006602/modifier_triangulate_ngon_method_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/modifier_triangulate_ngon_method_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/modifier_triangulate_ngon_method_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.142572 blender-stubs-3.2.0.27.dev4648006602/modifier_triangulate_quad_method_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/modifier_triangulate_quad_method_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/modifier_triangulate_quad_method_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.142572 blender-stubs-3.2.0.27.dev4648006602/motionpath_bake_location_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/motionpath_bake_location_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/motionpath_bake_location_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.142572 blender-stubs-3.2.0.27.dev4648006602/motionpath_display_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/motionpath_display_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/motionpath_display_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.142572 blender-stubs-3.2.0.27.dev4648006602/motionpath_range_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/motionpath_range_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/motionpath_range_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.142572 blender-stubs-3.2.0.27.dev4648006602/navigation_mode_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/navigation_mode_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/navigation_mode_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.142572 blender-stubs-3.2.0.27.dev4648006602/nla_mode_blend_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/nla_mode_blend_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/nla_mode_blend_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.142572 blender-stubs-3.2.0.27.dev4648006602/nla_mode_extend_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/nla_mode_extend_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/nla_mode_extend_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.142572 blender-stubs-3.2.0.27.dev4648006602/node_boolean_math_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_boolean_math_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_boolean_math_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.142572 blender-stubs-3.2.0.27.dev4648006602/node_clamp_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_clamp_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_clamp_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.142572 blender-stubs-3.2.0.27.dev4648006602/node_compare_operation_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_compare_operation_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_compare_operation_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.142572 blender-stubs-3.2.0.27.dev4648006602/node_filter_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_filter_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_filter_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.142572 blender-stubs-3.2.0.27.dev4648006602/node_float_compare_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_float_compare_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_float_compare_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.142572 blender-stubs-3.2.0.27.dev4648006602/node_float_to_int_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_float_to_int_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_float_to_int_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.146572 blender-stubs-3.2.0.27.dev4648006602/node_map_range_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_map_range_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_map_range_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.146572 blender-stubs-3.2.0.27.dev4648006602/node_math_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_math_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_math_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.146572 blender-stubs-3.2.0.27.dev4648006602/node_socket_in_out_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_socket_in_out_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_socket_in_out_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.146572 blender-stubs-3.2.0.27.dev4648006602/node_vec_math_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_vec_math_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/node_vec_math_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.146572 blender-stubs-3.2.0.27.dev4648006602/normal_space_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/normal_space_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/normal_space_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.146572 blender-stubs-3.2.0.27.dev4648006602/normal_swizzle_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/normal_swizzle_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/normal_swizzle_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.146572 blender-stubs-3.2.0.27.dev4648006602/object_axis_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_axis_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_axis_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.146572 blender-stubs-3.2.0.27.dev4648006602/object_empty_drawtype_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_empty_drawtype_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_empty_drawtype_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.146572 blender-stubs-3.2.0.27.dev4648006602/object_gpencil_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_gpencil_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_gpencil_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.146572 blender-stubs-3.2.0.27.dev4648006602/object_greasepencil_modifier_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_greasepencil_modifier_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_greasepencil_modifier_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.146572 blender-stubs-3.2.0.27.dev4648006602/object_mode_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_mode_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_mode_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.146572 blender-stubs-3.2.0.27.dev4648006602/object_modifier_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_modifier_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_modifier_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.146572 blender-stubs-3.2.0.27.dev4648006602/object_rotation_mode_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_rotation_mode_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_rotation_mode_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.146572 blender-stubs-3.2.0.27.dev4648006602/object_shaderfx_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_shaderfx_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_shaderfx_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.150572 blender-stubs-3.2.0.27.dev4648006602/object_type_curve_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_type_curve_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_type_curve_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.150572 blender-stubs-3.2.0.27.dev4648006602/object_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/object_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.150572 blender-stubs-3.2.0.27.dev4648006602/operator_context_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/operator_context_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/operator_context_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.150572 blender-stubs-3.2.0.27.dev4648006602/operator_property_tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/operator_property_tags/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/operator_property_tags/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.150572 blender-stubs-3.2.0.27.dev4648006602/operator_return_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/operator_return_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/operator_return_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.150572 blender-stubs-3.2.0.27.dev4648006602/operator_type_flag_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/operator_type_flag_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/operator_type_flag_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.150572 blender-stubs-3.2.0.27.dev4648006602/particle_edit_disconnected_hair_brush_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/particle_edit_disconnected_hair_brush_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/particle_edit_disconnected_hair_brush_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.150572 blender-stubs-3.2.0.27.dev4648006602/particle_edit_hair_brush_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/particle_edit_hair_brush_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/particle_edit_hair_brush_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.150572 blender-stubs-3.2.0.27.dev4648006602/preference_section_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/preference_section_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/preference_section_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.150572 blender-stubs-3.2.0.27.dev4648006602/prop_dynamicpaint_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/prop_dynamicpaint_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/prop_dynamicpaint_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.150572 blender-stubs-3.2.0.27.dev4648006602/property_flag_enum_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_flag_enum_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_flag_enum_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.150572 blender-stubs-3.2.0.27.dev4648006602/property_flag_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_flag_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_flag_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.154572 blender-stubs-3.2.0.27.dev4648006602/property_override_flag_collection_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_override_flag_collection_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_override_flag_collection_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.154572 blender-stubs-3.2.0.27.dev4648006602/property_override_flag_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_override_flag_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_override_flag_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.154572 blender-stubs-3.2.0.27.dev4648006602/property_string_search_flag_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_string_search_flag_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_string_search_flag_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.154572 blender-stubs-3.2.0.27.dev4648006602/property_subtype_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_subtype_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_subtype_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.154572 blender-stubs-3.2.0.27.dev4648006602/property_subtype_number_array_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_subtype_number_array_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_subtype_number_array_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.154572 blender-stubs-3.2.0.27.dev4648006602/property_subtype_number_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_subtype_number_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_subtype_number_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.154572 blender-stubs-3.2.0.27.dev4648006602/property_subtype_string_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_subtype_string_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_subtype_string_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.154572 blender-stubs-3.2.0.27.dev4648006602/property_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.154572 blender-stubs-3.2.0.27.dev4648006602/property_unit_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_unit_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/property_unit_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.154572 blender-stubs-3.2.0.27.dev4648006602/proportional_falloff_curve_only_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/proportional_falloff_curve_only_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/proportional_falloff_curve_only_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.154572 blender-stubs-3.2.0.27.dev4648006602/proportional_falloff_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/proportional_falloff_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/proportional_falloff_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.154572 blender-stubs-3.2.0.27.dev4648006602/ramp_blend_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/ramp_blend_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/ramp_blend_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.154572 blender-stubs-3.2.0.27.dev4648006602/region_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/region_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/region_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.154572 blender-stubs-3.2.0.27.dev4648006602/render_pass_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/render_pass_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/render_pass_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.154572 blender-stubs-3.2.0.27.dev4648006602/rigidbody_constraint_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/rigidbody_constraint_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/rigidbody_constraint_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.158572 blender-stubs-3.2.0.27.dev4648006602/rigidbody_object_shape_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/rigidbody_object_shape_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/rigidbody_object_shape_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.158572 blender-stubs-3.2.0.27.dev4648006602/rigidbody_object_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/rigidbody_object_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/rigidbody_object_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.158572 blender-stubs-3.2.0.27.dev4648006602/sequence_modifier_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/sequence_modifier_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/sequence_modifier_type_items/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 01:46:26.170572 blender-stubs-3.2.0.27.dev4648006602/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-09 01:46:25.000000 blender-stubs-3.2.0.27.dev4648006602/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.158572 blender-stubs-3.2.0.27.dev4648006602/shading_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/shading_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/shading_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.158572 blender-stubs-3.2.0.27.dev4648006602/shrinkwrap_face_cull_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/shrinkwrap_face_cull_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/shrinkwrap_face_cull_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.158572 blender-stubs-3.2.0.27.dev4648006602/shrinkwrap_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/shrinkwrap_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/shrinkwrap_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.158572 blender-stubs-3.2.0.27.dev4648006602/snap_element_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/snap_element_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/snap_element_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.158572 blender-stubs-3.2.0.27.dev4648006602/snap_node_element_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/snap_node_element_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/snap_node_element_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.158572 blender-stubs-3.2.0.27.dev4648006602/snap_source_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/snap_source_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/snap_source_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.158572 blender-stubs-3.2.0.27.dev4648006602/space_action_mode_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/space_action_mode_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/space_action_mode_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.158572 blender-stubs-3.2.0.27.dev4648006602/space_file_browse_mode_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/space_file_browse_mode_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/space_file_browse_mode_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.158572 blender-stubs-3.2.0.27.dev4648006602/space_graph_mode_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/space_graph_mode_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/space_graph_mode_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.158572 blender-stubs-3.2.0.27.dev4648006602/space_image_mode_all_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/space_image_mode_all_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/space_image_mode_all_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.162572 blender-stubs-3.2.0.27.dev4648006602/space_image_mode_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/space_image_mode_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:15.000000 blender-stubs-3.2.0.27.dev4648006602/space_image_mode_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.162572 blender-stubs-3.2.0.27.dev4648006602/space_sequencer_view_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/space_sequencer_view_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/space_sequencer_view_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.162572 blender-stubs-3.2.0.27.dev4648006602/space_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/space_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/space_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.162572 blender-stubs-3.2.0.27.dev4648006602/stereo3d_anaglyph_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/stereo3d_anaglyph_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/stereo3d_anaglyph_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.162572 blender-stubs-3.2.0.27.dev4648006602/stereo3d_display_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/stereo3d_display_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/stereo3d_display_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.162572 blender-stubs-3.2.0.27.dev4648006602/stereo3d_interlace_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/stereo3d_interlace_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/stereo3d_interlace_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.162572 blender-stubs-3.2.0.27.dev4648006602/strip_color_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/strip_color_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/strip_color_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.162572 blender-stubs-3.2.0.27.dev4648006602/subdivision_boundary_smooth_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/subdivision_boundary_smooth_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/subdivision_boundary_smooth_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.162572 blender-stubs-3.2.0.27.dev4648006602/subdivision_uv_smooth_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/subdivision_uv_smooth_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/subdivision_uv_smooth_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.162572 blender-stubs-3.2.0.27.dev4648006602/symmetrize_direction_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/symmetrize_direction_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/symmetrize_direction_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.162572 blender-stubs-3.2.0.27.dev4648006602/texture_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/texture_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/texture_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.162572 blender-stubs-3.2.0.27.dev4648006602/transform_mode_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/transform_mode_types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/transform_mode_types/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.162572 blender-stubs-3.2.0.27.dev4648006602/transform_orientation_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/transform_orientation_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/transform_orientation_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.166572 blender-stubs-3.2.0.27.dev4648006602/transform_pivot_items_full/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/transform_pivot_items_full/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/transform_pivot_items_full/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.166572 blender-stubs-3.2.0.27.dev4648006602/uilist_layout_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/uilist_layout_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/uilist_layout_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.166572 blender-stubs-3.2.0.27.dev4648006602/unpack_method_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/unpack_method_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/unpack_method_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.166572 blender-stubs-3.2.0.27.dev4648006602/velocity_unit_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/velocity_unit_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/velocity_unit_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.166572 blender-stubs-3.2.0.27.dev4648006602/views_format_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/views_format_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/views_format_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.166572 blender-stubs-3.2.0.27.dev4648006602/views_format_multilayer_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/views_format_multilayer_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/views_format_multilayer_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.166572 blender-stubs-3.2.0.27.dev4648006602/views_format_multiview_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/views_format_multiview_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/views_format_multiview_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.166572 blender-stubs-3.2.0.27.dev4648006602/volume_grid_data_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/volume_grid_data_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/volume_grid_data_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.166572 blender-stubs-3.2.0.27.dev4648006602/window_cursor_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/window_cursor_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/window_cursor_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.166572 blender-stubs-3.2.0.27.dev4648006602/wm_job_type_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/wm_job_type_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/wm_job_type_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.166572 blender-stubs-3.2.0.27.dev4648006602/wm_report_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/wm_report_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/wm_report_items/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:26.166572 blender-stubs-3.2.0.27.dev4648006602/workspace_object_mode_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/workspace_object_mode_items/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:46:16.000000 blender-stubs-3.2.0.27.dev4648006602/workspace_object_mode_items/py.typed
```

### Comparing `blender-stubs-3.2.0.27.dev4642539589/PKG-INFO` & `blender-stubs-3.2.0.27.dev4648006602/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blender-stubs
-Version: 3.2.0.27.dev4642539589
+Version: 3.2.0.27.dev4648006602
 Summary: API stubs for Blender and UPBGE generated with bpystubgen.
 Home-page: https://github.com/mysticfall/bpystubgen
 Author: Xavier Cho
 Author-email: mysticfallband@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `blender-stubs-3.2.0.27.dev4642539589/README.md` & `blender-stubs-3.2.0.27.dev4648006602/README.md`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/attribute_domain_with_auto_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/attribute_domain_with_auto_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/attribute_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/attribute_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/attribute_type_with_auto_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/attribute_type_with_auto_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/beztriple_interpolation_easing_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/beztriple_interpolation_easing_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/beztriple_interpolation_mode_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/beztriple_interpolation_mode_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/beztriple_keyframe_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/beztriple_keyframe_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bgl/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bgl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bl_math/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bl_math/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/blender_stubs.egg-info/PKG-INFO` & `blender-stubs-3.2.0.27.dev4648006602/blender_stubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blender-stubs
-Version: 3.2.0.27.dev4642539589
+Version: 3.2.0.27.dev4648006602
 Summary: API stubs for Blender and UPBGE generated with bpystubgen.
 Home-page: https://github.com/mysticfall/bpystubgen
 Author: Xavier Cho
 Author-email: mysticfallband@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `blender-stubs-3.2.0.27.dev4642539589/blender_stubs.egg-info/SOURCES.txt` & `blender-stubs-3.2.0.27.dev4648006602/blender_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/blender_stubs.egg-info/top_level.txt` & `blender-stubs-3.2.0.27.dev4648006602/blender_stubs.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/blf/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/blf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bmesh/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bmesh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bmesh/ops.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bmesh/ops.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bmesh/types.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bmesh/types.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bmesh/utils.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bmesh/utils.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/boidrule_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/boidrule_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/app/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/app/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/app/handlers.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/app/handlers.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/app/icons.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/app/icons.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/app/timers.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/app/timers.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/app/translations.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/app/translations.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/context.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/context.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/msgbus.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/msgbus.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/action.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/action.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/anim.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/anim.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/armature.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/armature.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/asset.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/asset.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/boid.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/boid.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/brush.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/brush.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/buttons.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/buttons.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/cachefile.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/cachefile.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/clip.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/clip.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/collection.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/collection.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/console.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/console.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/constraint.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/constraint.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/curve.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/curve.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/curves.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/curves.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/dpaint.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/dpaint.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/ed.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/ed.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/file.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/file.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/fluid.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/fluid.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/font.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/font.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/geometry.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/geometry.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/gpencil.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/gpencil.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/graph.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/graph.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/image.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/image.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/info.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/info.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/lattice.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/lattice.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/marker.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/marker.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/mask.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/mask.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/mball.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/mball.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/mesh.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/mesh.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/nla.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/nla.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/node.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/node.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/object.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/object.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/outliner.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/outliner.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/paint.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/paint.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/paintcurve.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/paintcurve.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/palette.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/palette.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/particle.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/particle.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/pose.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/pose.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/preferences.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/preferences.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/ptcache.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/ptcache.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/render.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/render.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/rigidbody.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/rigidbody.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/scene.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/scene.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/screen.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/screen.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/sculpt.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/sculpt.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/sculpt_curves.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/sculpt_curves.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/sequencer.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/sequencer.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/sound.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/sound.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/spreadsheet.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/spreadsheet.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/surface.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/surface.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/text.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/text.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/transform.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/transform.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/ui.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/ui.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/uilist.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/uilist.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/uv.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/uv.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/view2d.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/view2d.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/view3d.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/view3d.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/wm.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/wm.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/ops/workspace.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/ops/workspace.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/path.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/path.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/props.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/props.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/types.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/types.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -51188,17 +51188,17 @@
 000c7f30: 6566 2062 6c5f 726e 615f 6765 745f 7375  ef bl_rna_get_su
 000c7f40: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 000c7f50: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 000c7f60: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 000c7f70: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 000c7f80: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 000c7f90: 6173 7320 4669 6c65 4173 7365 7453 656c  ass FileAssetSel
-000c7fa0: 6563 7450 6172 616d 7328 6270 795f 7374  ectParams(bpy_st
-000c7fb0: 7275 6374 2c20 4669 6c65 5365 6c65 6374  ruct, FileSelect
-000c7fc0: 5061 7261 6d73 293a 0a0a 2020 2222 220a  Params):..  """.
+000c7fa0: 6563 7450 6172 616d 7328 4669 6c65 5365  ectParams(FileSe
+000c7fb0: 6c65 6374 5061 7261 6d73 2c20 6270 795f  lectParams, bpy_
+000c7fc0: 7374 7275 6374 293a 0a0a 2020 2222 220a  struct):..  """.
 000c7fd0: 0a20 2053 6574 7469 6e67 7320 666f 7220  .  Settings for 
 000c7fe0: 7468 6520 6669 6c65 2073 656c 6563 7469  the file selecti
 000c7ff0: 6f6e 2069 6e20 4173 7365 7420 4272 6f77  on in Asset Brow
 000c8000: 7365 7220 6d6f 6465 0a0a 2020 2222 220a  ser mode..  """.
 000c8010: 0a20 2061 7373 6574 5f6c 6962 7261 7279  .  asset_library
 000c8020: 5f72 6566 3a20 7374 7220 3d20 2e2e 2e0a  _ref: str = ....
 000c8030: 0a20 2063 6174 616c 6f67 5f69 643a 2073  .  catalog_id: s
@@ -72782,16 +72782,16 @@
 0011c4d0: 7468 6f64 0a0a 2020 6465 6620 626c 5f72  thod..  def bl_r
 0011c4e0: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 0011c4f0: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 0011c500: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 0011c510: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 0011c520: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 0011c530: 2020 2e2e 2e0a 0a63 6c61 7373 2053 7061    .....class Spa
-0011c540: 6365 436c 6970 4564 6974 6f72 2862 7079  ceClipEditor(bpy
-0011c550: 5f73 7472 7563 742c 2053 7061 6365 293a  _struct, Space):
+0011c540: 6365 436c 6970 4564 6974 6f72 2853 7061  ceClipEditor(Spa
+0011c550: 6365 2c20 6270 795f 7374 7275 6374 293a  ce, bpy_struct):
 0011c560: 0a0a 2020 2222 220a 0a20 2043 6c69 7020  ..  """..  Clip 
 0011c570: 6564 6974 6f72 2073 7061 6365 2064 6174  editor space dat
 0011c580: 610a 0a20 2022 2222 0a0a 2020 616e 6e6f  a..  """..  anno
 0011c590: 7461 7469 6f6e 5f73 6f75 7263 653a 2073  tation_source: s
 0011c5a0: 7472 203d 202e 2e2e 0a0a 2020 2222 220a  tr = .....  """.
 0011c5b0: 0a20 2057 6865 7265 2074 6865 2061 6e6e  .  Where the ann
 0011c5c0: 6f74 6174 696f 6e20 636f 6d65 7320 6672  otation comes fr
@@ -73134,16 +73134,16 @@
 0011dad0: 653a 2073 7472 2920 2d3e 204e 6f6e 653a  e: str) -> None:
 0011dae0: 0a0a 2020 2020 2222 220a 0a20 2020 2052  ..    """..    R
 0011daf0: 656d 6f76 6520 6120 6472 6177 2068 616e  emove a draw han
 0011db00: 646c 6572 2074 6861 7420 7761 7320 6164  dler that was ad
 0011db10: 6465 6420 7072 6576 696f 7573 6c79 2e0a  ded previously..
 0011db20: 0a20 2020 2022 2222 0a0a 2020 2020 2e2e  .    """..    ..
 0011db30: 2e0a 0a63 6c61 7373 2053 7061 6365 436f  ...class SpaceCo
-0011db40: 6e73 6f6c 6528 6270 795f 7374 7275 6374  nsole(bpy_struct
-0011db50: 2c20 5370 6163 6529 3a0a 0a20 2022 2222  , Space):..  """
+0011db40: 6e73 6f6c 6528 5370 6163 652c 2062 7079  nsole(Space, bpy
+0011db50: 5f73 7472 7563 7429 3a0a 0a20 2022 2222  _struct):..  """
 0011db60: 0a0a 2020 496e 7465 7261 6374 6976 6520  ..  Interactive 
 0011db70: 7079 7468 6f6e 2063 6f6e 736f 6c65 0a0a  python console..
 0011db80: 2020 2222 220a 0a20 2066 6f6e 745f 7369    """..  font_si
 0011db90: 7a65 3a20 696e 7420 3d20 2e2e 2e0a 0a20  ze: int = ..... 
 0011dba0: 2022 2222 0a0a 2020 466f 6e74 2073 697a   """..  Font siz
 0011dbb0: 6520 746f 2075 7365 2066 6f72 2064 6973  e to use for dis
 0011dbc0: 706c 6179 696e 6720 7468 6520 7465 7874  playing the text
@@ -73220,16 +73220,16 @@
 0011e030: 3e20 4e6f 6e65 3a0a 0a20 2020 2022 2222  > None:..    """
 0011e040: 0a0a 2020 2020 5265 6d6f 7665 2061 2064  ..    Remove a d
 0011e050: 7261 7720 6861 6e64 6c65 7220 7468 6174  raw handler that
 0011e060: 2077 6173 2061 6464 6564 2070 7265 7669   was added previ
 0011e070: 6f75 736c 792e 0a0a 2020 2020 2222 220a  ously...    """.
 0011e080: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 0011e090: 5370 6163 6544 6f70 6553 6865 6574 4564  SpaceDopeSheetEd
-0011e0a0: 6974 6f72 2862 7079 5f73 7472 7563 742c  itor(bpy_struct,
-0011e0b0: 2053 7061 6365 293a 0a0a 2020 2222 220a   Space):..  """.
+0011e0a0: 6974 6f72 2853 7061 6365 2c20 6270 795f  itor(Space, bpy_
+0011e0b0: 7374 7275 6374 293a 0a0a 2020 2222 220a  struct):..  """.
 0011e0c0: 0a20 2044 6f70 6520 5368 6565 7420 7370  .  Dope Sheet sp
 0011e0d0: 6163 6520 6461 7461 0a0a 2020 2222 220a  ace data..  """.
 0011e0e0: 0a20 2061 6374 696f 6e3a 2041 6374 696f  .  action: Actio
 0011e0f0: 6e20 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  n = .....  """..
 0011e100: 2020 4163 7469 6f6e 2064 6973 706c 6179    Action display
 0011e110: 6564 2061 6e64 2065 6469 7465 6420 696e  ed and edited in
 0011e120: 2074 6869 7320 7370 6163 650a 0a20 2022   this space..  "
@@ -73485,16 +73485,16 @@
 0011f0c0: 6e5f 7479 7065 3a20 7374 7229 202d 3e20  n_type: str) -> 
 0011f0d0: 4e6f 6e65 3a0a 0a20 2020 2022 2222 0a0a  None:..    """..
 0011f0e0: 2020 2020 5265 6d6f 7665 2061 2064 7261      Remove a dra
 0011f0f0: 7720 6861 6e64 6c65 7220 7468 6174 2077  w handler that w
 0011f100: 6173 2061 6464 6564 2070 7265 7669 6f75  as added previou
 0011f110: 736c 792e 0a0a 2020 2020 2222 220a 0a20  sly...    """.. 
 0011f120: 2020 202e 2e2e 0a0a 636c 6173 7320 5370     .....class Sp
-0011f130: 6163 6546 696c 6542 726f 7773 6572 2862  aceFileBrowser(b
-0011f140: 7079 5f73 7472 7563 742c 2053 7061 6365  py_struct, Space
+0011f130: 6163 6546 696c 6542 726f 7773 6572 2853  aceFileBrowser(S
+0011f140: 7061 6365 2c20 6270 795f 7374 7275 6374  pace, bpy_struct
 0011f150: 293a 0a0a 2020 2222 220a 0a20 2046 696c  ):..  """..  Fil
 0011f160: 6520 6272 6f77 7365 7220 7370 6163 6520  e browser space 
 0011f170: 6461 7461 0a0a 2020 2222 220a 0a20 2061  data..  """..  a
 0011f180: 6374 6976 655f 6f70 6572 6174 6f72 3a20  ctive_operator: 
 0011f190: 4f70 6572 6174 6f72 203d 202e 2e2e 0a0a  Operator = .....
 0011f1a0: 2020 626f 6f6b 6d61 726b 733a 2074 7970    bookmarks: typ
 0011f1b0: 696e 672e 556e 696f 6e5b 7479 7069 6e67  ing.Union[typing
@@ -73658,16 +73658,16 @@
 0011fb90: 7229 202d 3e20 4e6f 6e65 3a0a 0a20 2020  r) -> None:..   
 0011fba0: 2022 2222 0a0a 2020 2020 5265 6d6f 7665   """..    Remove
 0011fbb0: 2061 2064 7261 7720 6861 6e64 6c65 7220   a draw handler 
 0011fbc0: 7468 6174 2077 6173 2061 6464 6564 2070  that was added p
 0011fbd0: 7265 7669 6f75 736c 792e 0a0a 2020 2020  reviously...    
 0011fbe0: 2222 220a 0a20 2020 202e 2e2e 0a0a 636c  """..    .....cl
 0011fbf0: 6173 7320 5370 6163 6547 7261 7068 4564  ass SpaceGraphEd
-0011fc00: 6974 6f72 2862 7079 5f73 7472 7563 742c  itor(bpy_struct,
-0011fc10: 2053 7061 6365 293a 0a0a 2020 2222 220a   Space):..  """.
+0011fc00: 6974 6f72 2853 7061 6365 2c20 6270 795f  itor(Space, bpy_
+0011fc10: 7374 7275 6374 293a 0a0a 2020 2222 220a  struct):..  """.
 0011fc20: 0a20 2047 7261 7068 2045 6469 746f 7220  .  Graph Editor 
 0011fc30: 7370 6163 6520 6461 7461 0a0a 2020 2222  space data..  ""
 0011fc40: 220a 0a20 2061 7574 6f5f 736e 6170 3a20  "..  auto_snap: 
 0011fc50: 7374 7220 3d20 2e2e 2e0a 0a20 2022 2222  str = .....  """
 0011fc60: 0a0a 2020 4175 746f 6d61 7469 6320 7469  ..  Automatic ti
 0011fc70: 6d65 2073 6e61 7070 696e 6720 7365 7474  me snapping sett
 0011fc80: 696e 6773 2066 6f72 2074 7261 6e73 666f  ings for transfo
@@ -73841,16 +73841,16 @@
 00120700: 3a20 7374 7229 202d 3e20 4e6f 6e65 3a0a  : str) -> None:.
 00120710: 0a20 2020 2022 2222 0a0a 2020 2020 5265  .    """..    Re
 00120720: 6d6f 7665 2061 2064 7261 7720 6861 6e64  move a draw hand
 00120730: 6c65 7220 7468 6174 2077 6173 2061 6464  ler that was add
 00120740: 6564 2070 7265 7669 6f75 736c 792e 0a0a  ed previously...
 00120750: 2020 2020 2222 220a 0a20 2020 202e 2e2e      """..    ...
 00120760: 0a0a 636c 6173 7320 5370 6163 6549 6d61  ..class SpaceIma
-00120770: 6765 4564 6974 6f72 2862 7079 5f73 7472  geEditor(bpy_str
-00120780: 7563 742c 2053 7061 6365 293a 0a0a 2020  uct, Space):..  
+00120770: 6765 4564 6974 6f72 2853 7061 6365 2c20  geEditor(Space, 
+00120780: 6270 795f 7374 7275 6374 293a 0a0a 2020  bpy_struct):..  
 00120790: 2222 220a 0a20 2049 6d61 6765 2061 6e64  """..  Image and
 001207a0: 2055 5620 6564 6974 6f72 2073 7061 6365   UV editor space
 001207b0: 2064 6174 610a 0a20 2022 2222 0a0a 2020   data..  """..  
 001207c0: 626c 656e 645f 6661 6374 6f72 3a20 666c  blend_factor: fl
 001207d0: 6f61 7420 3d20 2e2e 2e0a 0a20 2022 2222  oat = .....  """
 001207e0: 0a0a 2020 4f76 6572 6c61 7920 626c 656e  ..  Overlay blen
 001207f0: 6469 6e67 2066 6163 746f 7220 6f66 2072  ding factor of r
@@ -74132,16 +74132,16 @@
 00121930: 6567 696f 6e5f 7479 7065 3a20 7374 7229  egion_type: str)
 00121940: 202d 3e20 4e6f 6e65 3a0a 0a20 2020 2022   -> None:..    "
 00121950: 2222 0a0a 2020 2020 5265 6d6f 7665 2061  ""..    Remove a
 00121960: 2064 7261 7720 6861 6e64 6c65 7220 7468   draw handler th
 00121970: 6174 2077 6173 2061 6464 6564 2070 7265  at was added pre
 00121980: 7669 6f75 736c 792e 0a0a 2020 2020 2222  viously...    ""
 00121990: 220a 0a20 2020 202e 2e2e 0a0a 636c 6173  "..    .....clas
-001219a0: 7320 5370 6163 6549 6e66 6f28 6270 795f  s SpaceInfo(bpy_
-001219b0: 7374 7275 6374 2c20 5370 6163 6529 3a0a  struct, Space):.
+001219a0: 7320 5370 6163 6549 6e66 6f28 5370 6163  s SpaceInfo(Spac
+001219b0: 652c 2062 7079 5f73 7472 7563 7429 3a0a  e, bpy_struct):.
 001219c0: 0a20 2022 2222 0a0a 2020 496e 666f 2073  .  """..  Info s
 001219d0: 7061 6365 2064 6174 610a 0a20 2022 2222  pace data..  """
 001219e0: 0a0a 2020 7368 6f77 5f72 6570 6f72 745f  ..  show_report_
 001219f0: 6465 6275 673a 2062 6f6f 6c20 3d20 2e2e  debug: bool = ..
 00121a00: 2e0a 0a20 2022 2222 0a0a 2020 4469 7370  ...  """..  Disp
 00121a10: 6c61 7920 6465 6275 6720 7265 706f 7274  lay debug report
 00121a20: 696e 6720 696e 666f 0a0a 2020 2222 220a  ing info..  """.
@@ -74205,16 +74205,16 @@
 00121dc0: 6e5f 7479 7065 3a20 7374 7229 202d 3e20  n_type: str) -> 
 00121dd0: 4e6f 6e65 3a0a 0a20 2020 2022 2222 0a0a  None:..    """..
 00121de0: 2020 2020 5265 6d6f 7665 2061 2064 7261      Remove a dra
 00121df0: 7720 6861 6e64 6c65 7220 7468 6174 2077  w handler that w
 00121e00: 6173 2061 6464 6564 2070 7265 7669 6f75  as added previou
 00121e10: 736c 792e 0a0a 2020 2020 2222 220a 0a20  sly...    """.. 
 00121e20: 2020 202e 2e2e 0a0a 636c 6173 7320 5370     .....class Sp
-00121e30: 6163 654e 4c41 2862 7079 5f73 7472 7563  aceNLA(bpy_struc
-00121e40: 742c 2053 7061 6365 293a 0a0a 2020 2222  t, Space):..  ""
+00121e30: 6163 654e 4c41 2853 7061 6365 2c20 6270  aceNLA(Space, bp
+00121e40: 795f 7374 7275 6374 293a 0a0a 2020 2222  y_struct):..  ""
 00121e50: 220a 0a20 204e 4c41 2065 6469 746f 7220  "..  NLA editor 
 00121e60: 7370 6163 6520 6461 7461 0a0a 2020 2222  space data..  ""
 00121e70: 220a 0a20 2061 7574 6f5f 736e 6170 3a20  "..  auto_snap: 
 00121e80: 7374 7220 3d20 2e2e 2e0a 0a20 2022 2222  str = .....  """
 00121e90: 0a0a 2020 4175 746f 6d61 7469 6320 7469  ..  Automatic ti
 00121ea0: 6d65 2073 6e61 7070 696e 6720 7365 7474  me snapping sett
 00121eb0: 696e 6773 2066 6f72 2074 7261 6e73 666f  ings for transfo
@@ -74327,16 +74327,16 @@
 00122560: 7970 653a 2073 7472 2920 2d3e 204e 6f6e  ype: str) -> Non
 00122570: 653a 0a0a 2020 2020 2222 220a 0a20 2020  e:..    """..   
 00122580: 2052 656d 6f76 6520 6120 6472 6177 2068   Remove a draw h
 00122590: 616e 646c 6572 2074 6861 7420 7761 7320  andler that was 
 001225a0: 6164 6465 6420 7072 6576 696f 7573 6c79  added previously
 001225b0: 2e0a 0a20 2020 2022 2222 0a0a 2020 2020  ...    """..    
 001225c0: 2e2e 2e0a 0a63 6c61 7373 2053 7061 6365  .....class Space
-001225d0: 4e6f 6465 4564 6974 6f72 2862 7079 5f73  NodeEditor(bpy_s
-001225e0: 7472 7563 742c 2053 7061 6365 293a 0a0a  truct, Space):..
+001225d0: 4e6f 6465 4564 6974 6f72 2853 7061 6365  NodeEditor(Space
+001225e0: 2c20 6270 795f 7374 7275 6374 293a 0a0a  , bpy_struct):..
 001225f0: 2020 2222 220a 0a20 204e 6f64 6520 6564    """..  Node ed
 00122600: 6974 6f72 2073 7061 6365 2064 6174 610a  itor space data.
 00122610: 0a20 2022 2222 0a0a 2020 6261 636b 6472  .  """..  backdr
 00122620: 6f70 5f63 6861 6e6e 656c 733a 2073 7472  op_channels: str
 00122630: 203d 202e 2e2e 0a0a 2020 2222 220a 0a20   = .....  """.. 
 00122640: 2043 6861 6e6e 656c 7320 6f66 2074 6865   Channels of the
 00122650: 2069 6d61 6765 2074 6f20 6472 6177 0a0a   image to draw..
@@ -74541,16 +74541,16 @@
 001232c0: 2920 2d3e 204e 6f6e 653a 0a0a 2020 2020  ) -> None:..    
 001232d0: 2222 220a 0a20 2020 2052 656d 6f76 6520  """..    Remove 
 001232e0: 6120 6472 6177 2068 616e 646c 6572 2074  a draw handler t
 001232f0: 6861 7420 7761 7320 6164 6465 6420 7072  hat was added pr
 00123300: 6576 696f 7573 6c79 2e0a 0a20 2020 2022  eviously...    "
 00123310: 2222 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  ""..    .....cla
 00123320: 7373 2053 7061 6365 4f75 746c 696e 6572  ss SpaceOutliner
-00123330: 2862 7079 5f73 7472 7563 742c 2053 7061  (bpy_struct, Spa
-00123340: 6365 293a 0a0a 2020 2222 220a 0a20 204f  ce):..  """..  O
+00123330: 2853 7061 6365 2c20 6270 795f 7374 7275  (Space, bpy_stru
+00123340: 6374 293a 0a0a 2020 2222 220a 0a20 204f  ct):..  """..  O
 00123350: 7574 6c69 6e65 7220 7370 6163 6520 6461  utliner space da
 00123360: 7461 0a0a 2020 2222 220a 0a20 2064 6973  ta..  """..  dis
 00123370: 706c 6179 5f6d 6f64 653a 2073 7472 203d  play_mode: str =
 00123380: 202e 2e2e 0a0a 2020 2222 220a 0a20 2054   .....  """..  T
 00123390: 7970 6520 6f66 2069 6e66 6f72 6d61 7469  ype of informati
 001233a0: 6f6e 2074 6f20 6469 7370 6c61 790a 0a20  on to display.. 
 001233b0: 202a 2060 6053 4345 4e45 5360 600a 5363   * ``SCENES``.Sc
@@ -74836,16 +74836,16 @@
 00124530: 202d 3e20 4e6f 6e65 3a0a 0a20 2020 2022   -> None:..    "
 00124540: 2222 0a0a 2020 2020 5265 6d6f 7665 2061  ""..    Remove a
 00124550: 2064 7261 7720 6861 6e64 6c65 7220 7468   draw handler th
 00124560: 6174 2077 6173 2061 6464 6564 2070 7265  at was added pre
 00124570: 7669 6f75 736c 792e 0a0a 2020 2020 2222  viously...    ""
 00124580: 220a 0a20 2020 202e 2e2e 0a0a 636c 6173  "..    .....clas
 00124590: 7320 5370 6163 6550 7265 6665 7265 6e63  s SpacePreferenc
-001245a0: 6573 2862 7079 5f73 7472 7563 742c 2053  es(bpy_struct, S
-001245b0: 7061 6365 293a 0a0a 2020 2222 220a 0a20  pace):..  """.. 
+001245a0: 6573 2853 7061 6365 2c20 6270 795f 7374  es(Space, bpy_st
+001245b0: 7275 6374 293a 0a0a 2020 2222 220a 0a20  ruct):..  """.. 
 001245c0: 2042 6c65 6e64 6572 2070 7265 6665 7265   Blender prefere
 001245d0: 6e63 6573 2073 7061 6365 2064 6174 610a  nces space data.
 001245e0: 0a20 2022 2222 0a0a 2020 6669 6c74 6572  .  """..  filter
 001245f0: 5f74 6578 743a 2073 7472 203d 202e 2e2e  _text: str = ...
 00124600: 0a0a 2020 2222 220a 0a20 2053 6561 7263  ..  """..  Searc
 00124610: 6820 7465 726d 2066 6f72 2066 696c 7465  h term for filte
 00124620: 7269 6e67 2069 6e20 7468 6520 5549 0a0a  ring in the UI..
@@ -74902,16 +74902,16 @@
 00124950: 7970 653a 2073 7472 2920 2d3e 204e 6f6e  ype: str) -> Non
 00124960: 653a 0a0a 2020 2020 2222 220a 0a20 2020  e:..    """..   
 00124970: 2052 656d 6f76 6520 6120 6472 6177 2068   Remove a draw h
 00124980: 616e 646c 6572 2074 6861 7420 7761 7320  andler that was 
 00124990: 6164 6465 6420 7072 6576 696f 7573 6c79  added previously
 001249a0: 2e0a 0a20 2020 2022 2222 0a0a 2020 2020  ...    """..    
 001249b0: 2e2e 2e0a 0a63 6c61 7373 2053 7061 6365  .....class Space
-001249c0: 5072 6f70 6572 7469 6573 2862 7079 5f73  Properties(bpy_s
-001249d0: 7472 7563 742c 2053 7061 6365 293a 0a0a  truct, Space):..
+001249c0: 5072 6f70 6572 7469 6573 2853 7061 6365  Properties(Space
+001249d0: 2c20 6270 795f 7374 7275 6374 293a 0a0a  , bpy_struct):..
 001249e0: 2020 2222 220a 0a20 2050 726f 7065 7274    """..  Propert
 001249f0: 6965 7320 7370 6163 6520 6461 7461 0a0a  ies space data..
 00124a00: 2020 2222 220a 0a20 2063 6f6e 7465 7874    """..  context
 00124a10: 3a20 7374 7220 3d20 2e2e 2e0a 0a20 2022  : str = .....  "
 00124a20: 2222 0a0a 2020 2a20 6060 544f 4f4c 6060  ""..  * ``TOOL``
 00124a30: 0a54 6f6f 6c20 2d2d 2041 6374 6976 6520  .Tool -- Active 
 00124a40: 546f 6f6c 2061 6e64 2057 6f72 6b73 7061  Tool and Workspa
@@ -75052,16 +75052,16 @@
 001252b0: 2920 2d3e 204e 6f6e 653a 0a0a 2020 2020  ) -> None:..    
 001252c0: 2222 220a 0a20 2020 2052 656d 6f76 6520  """..    Remove 
 001252d0: 6120 6472 6177 2068 616e 646c 6572 2074  a draw handler t
 001252e0: 6861 7420 7761 7320 6164 6465 6420 7072  hat was added pr
 001252f0: 6576 696f 7573 6c79 2e0a 0a20 2020 2022  eviously...    "
 00125300: 2222 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  ""..    .....cla
 00125310: 7373 2053 7061 6365 5365 7175 656e 6365  ss SpaceSequence
-00125320: 4564 6974 6f72 2862 7079 5f73 7472 7563  Editor(bpy_struc
-00125330: 742c 2053 7061 6365 293a 0a0a 2020 2222  t, Space):..  ""
+00125320: 4564 6974 6f72 2853 7061 6365 2c20 6270  Editor(Space, bp
+00125330: 795f 7374 7275 6374 293a 0a0a 2020 2222  y_struct):..  ""
 00125340: 220a 0a20 2053 6571 7565 6e63 6520 6564  "..  Sequence ed
 00125350: 6974 6f72 2073 7061 6365 2064 6174 610a  itor space data.
 00125360: 0a20 2022 2222 0a0a 2020 6375 7273 6f72  .  """..  cursor
 00125370: 5f6c 6f63 6174 696f 6e3a 206d 6174 6875  _location: mathu
 00125380: 7469 6c73 2e56 6563 746f 7220 3d20 2e2e  tils.Vector = ..
 00125390: 2e0a 0a20 2022 2222 0a0a 2020 3244 2063  ...  """..  2D c
 001253a0: 7572 736f 7220 6c6f 6361 7469 6f6e 2066  ursor location f
@@ -75280,16 +75280,16 @@
 001260f0: 202d 3e20 4e6f 6e65 3a0a 0a20 2020 2022   -> None:..    "
 00126100: 2222 0a0a 2020 2020 5265 6d6f 7665 2061  ""..    Remove a
 00126110: 2064 7261 7720 6861 6e64 6c65 7220 7468   draw handler th
 00126120: 6174 2077 6173 2061 6464 6564 2070 7265  at was added pre
 00126130: 7669 6f75 736c 792e 0a0a 2020 2020 2222  viously...    ""
 00126140: 220a 0a20 2020 202e 2e2e 0a0a 636c 6173  "..    .....clas
 00126150: 7320 5370 6163 6553 7072 6561 6473 6865  s SpaceSpreadshe
-00126160: 6574 2862 7079 5f73 7472 7563 742c 2053  et(bpy_struct, S
-00126170: 7061 6365 293a 0a0a 2020 2222 220a 0a20  pace):..  """.. 
+00126160: 6574 2853 7061 6365 2c20 6270 795f 7374  et(Space, bpy_st
+00126170: 7275 6374 293a 0a0a 2020 2222 220a 0a20  ruct):..  """.. 
 00126180: 2053 7072 6561 6473 6865 6574 2073 7061   Spreadsheet spa
 00126190: 6365 2064 6174 610a 0a20 2022 2222 0a0a  ce data..  """..
 001261a0: 2020 6174 7472 6962 7574 655f 646f 6d61    attribute_doma
 001261b0: 696e 3a20 7374 7220 3d20 2e2e 2e0a 0a20  in: str = ..... 
 001261c0: 2022 2222 0a0a 2020 4174 7472 6962 7574   """..  Attribut
 001261d0: 6520 646f 6d61 696e 2074 6f20 6469 7370  e domain to disp
 001261e0: 6c61 790a 0a20 2022 2222 0a0a 2020 636f  lay..  """..  co
@@ -75412,16 +75412,16 @@
 00126930: 7065 3a20 7374 7229 202d 3e20 4e6f 6e65  pe: str) -> None
 00126940: 3a0a 0a20 2020 2022 2222 0a0a 2020 2020  :..    """..    
 00126950: 5265 6d6f 7665 2061 2064 7261 7720 6861  Remove a draw ha
 00126960: 6e64 6c65 7220 7468 6174 2077 6173 2061  ndler that was a
 00126970: 6464 6564 2070 7265 7669 6f75 736c 792e  dded previously.
 00126980: 0a0a 2020 2020 2222 220a 0a20 2020 202e  ..    """..    .
 00126990: 2e2e 0a0a 636c 6173 7320 5370 6163 6554  ....class SpaceT
-001269a0: 6578 7445 6469 746f 7228 6270 795f 7374  extEditor(bpy_st
-001269b0: 7275 6374 2c20 5370 6163 6529 3a0a 0a20  ruct, Space):.. 
+001269a0: 6578 7445 6469 746f 7228 5370 6163 652c  extEditor(Space,
+001269b0: 2062 7079 5f73 7472 7563 7429 3a0a 0a20   bpy_struct):.. 
 001269c0: 2022 2222 0a0a 2020 5465 7874 2065 6469   """..  Text edi
 001269d0: 746f 7220 7370 6163 6520 6461 7461 0a0a  tor space data..
 001269e0: 2020 2222 220a 0a20 2066 696e 645f 7465    """..  find_te
 001269f0: 7874 3a20 7374 7220 3d20 2e2e 2e0a 0a20  xt: str = ..... 
 00126a00: 2022 2222 0a0a 2020 5465 7874 2074 6f20   """..  Text to 
 00126a10: 7365 6172 6368 2066 6f72 2077 6974 6820  search for with 
 00126a20: 7468 6520 6669 6e64 2074 6f6f 6c0a 0a20  the find tool.. 
@@ -75587,16 +75587,16 @@
 00127420: 7065 3a20 7374 7229 202d 3e20 4e6f 6e65  pe: str) -> None
 00127430: 3a0a 0a20 2020 2022 2222 0a0a 2020 2020  :..    """..    
 00127440: 5265 6d6f 7665 2061 2064 7261 7720 6861  Remove a draw ha
 00127450: 6e64 6c65 7220 7468 6174 2077 6173 2061  ndler that was a
 00127460: 6464 6564 2070 7265 7669 6f75 736c 792e  dded previously.
 00127470: 0a0a 2020 2020 2222 220a 0a20 2020 202e  ..    """..    .
 00127480: 2e2e 0a0a 636c 6173 7320 5370 6163 6556  ....class SpaceV
-00127490: 6965 7733 4428 6270 795f 7374 7275 6374  iew3D(bpy_struct
-001274a0: 2c20 5370 6163 6529 3a0a 0a20 2022 2222  , Space):..  """
+00127490: 6965 7733 4428 5370 6163 652c 2062 7079  iew3D(Space, bpy
+001274a0: 5f73 7472 7563 7429 3a0a 0a20 2022 2222  _struct):..  """
 001274b0: 0a0a 2020 3344 2056 6965 7720 7370 6163  ..  3D View spac
 001274c0: 6520 6461 7461 0a0a 2020 2222 220a 0a20  e data..  """.. 
 001274d0: 2063 616d 6572 613a 204f 626a 6563 7420   camera: Object 
 001274e0: 3d20 2e2e 2e0a 0a20 2022 2222 0a0a 2020  = .....  """..  
 001274f0: 4163 7469 7665 2063 616d 6572 6120 7573  Active camera us
 00127500: 6564 2069 6e20 7468 6973 2076 6965 7720  ed in this view 
 00127510: 2877 6865 6e20 756e 6c6f 636b 6564 2066  (when unlocked f
@@ -77552,16 +77552,16 @@
 0012eef0: 686f 640a 0a20 2064 6566 2062 6c5f 726e  hod..  def bl_rn
 0012ef00: 615f 6765 745f 7375 6263 6c61 7373 5f70  a_get_subclass_p
 0012ef10: 7928 636c 732c 2069 643a 2073 7472 2c20  y(cls, id: str, 
 0012ef20: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 0012ef30: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 0012ef40: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 0012ef50: 202e 2e2e 0a0a 636c 6173 7320 5375 7266   .....class Surf
-0012ef60: 6163 6543 7572 7665 2862 7079 5f73 7472  aceCurve(bpy_str
-0012ef70: 7563 742c 2043 7572 7665 2c20 4944 293a  uct, Curve, ID):
+0012ef60: 6163 6543 7572 7665 2843 7572 7665 2c20  aceCurve(Curve, 
+0012ef70: 6270 795f 7374 7275 6374 2c20 4944 293a  bpy_struct, ID):
 0012ef80: 0a0a 2020 2222 220a 0a20 2043 7572 7665  ..  """..  Curve
 0012ef90: 2064 6174 612d 626c 6f63 6b20 7573 6564   data-block used
 0012efa0: 2066 6f72 2073 746f 7269 6e67 2073 7572   for storing sur
 0012efb0: 6661 6365 730a 0a20 2022 2222 0a0a 2020  faces..  """..  
 0012efc0: 4063 6c61 7373 6d65 7468 6f64 0a0a 2020  @classmethod..  
 0012efd0: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 0012efe0: 7562 636c 6173 7328 636c 732c 2069 643a  ubclass(cls, id:
@@ -77572,16 +77572,16 @@
 0012f030: 6574 686f 640a 0a20 2064 6566 2062 6c5f  ethod..  def bl_
 0012f040: 726e 615f 6765 745f 7375 6263 6c61 7373  rna_get_subclass
 0012f050: 5f70 7928 636c 732c 2069 643a 2073 7472  _py(cls, id: str
 0012f060: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 0012f070: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 0012f080: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 0012f090: 2020 202e 2e2e 0a0a 636c 6173 7320 5465     .....class Te
-0012f0a0: 7874 4375 7276 6528 6270 795f 7374 7275  xtCurve(bpy_stru
-0012f0b0: 6374 2c20 4375 7276 652c 2049 4429 3a0a  ct, Curve, ID):.
+0012f0a0: 7874 4375 7276 6528 4375 7276 652c 2062  xtCurve(Curve, b
+0012f0b0: 7079 5f73 7472 7563 742c 2049 4429 3a0a  py_struct, ID):.
 0012f0c0: 0a20 2022 2222 0a0a 2020 4375 7276 6520  .  """..  Curve 
 0012f0d0: 6461 7461 2d62 6c6f 636b 2075 7365 6420  data-block used 
 0012f0e0: 666f 7220 7374 6f72 696e 6720 7465 7874  for storing text
 0012f0f0: 0a0a 2020 2222 220a 0a20 2061 6374 6976  ..  """..  activ
 0012f100: 655f 7465 7874 626f 783a 2069 6e74 203d  e_textbox: int =
 0012f110: 202e 2e2e 0a0a 2020 616c 6967 6e5f 783a   .....  align_x:
 0012f120: 2073 7472 203d 202e 2e2e 0a0a 2020 2222   str = .....  ""
@@ -77758,16 +77758,16 @@
 0012fbd0: 6620 626c 5f72 6e61 5f67 6574 5f73 7562  f bl_rna_get_sub
 0012fbe0: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 0012fbf0: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 0012fc00: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 0012fc10: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 0012fc20: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 0012fc30: 7373 2041 7265 614c 6967 6874 2862 7079  ss AreaLight(bpy
-0012fc40: 5f73 7472 7563 742c 204c 6967 6874 2c20  _struct, Light, 
-0012fc50: 4944 293a 0a0a 2020 2222 220a 0a20 2044  ID):..  """..  D
+0012fc40: 5f73 7472 7563 742c 2049 442c 204c 6967  _struct, ID, Lig
+0012fc50: 6874 293a 0a0a 2020 2222 220a 0a20 2044  ht):..  """..  D
 0012fc60: 6972 6563 7469 6f6e 616c 2061 7265 6120  irectional area 
 0012fc70: 4c69 6768 740a 0a20 2022 2222 0a0a 2020  Light..  """..  
 0012fc80: 636f 6e73 7461 6e74 5f63 6f65 6666 6963  constant_coeffic
 0012fc90: 6965 6e74 3a20 666c 6f61 7420 3d20 2e2e  ient: float = ..
 0012fca0: 2e0a 0a20 2022 2222 0a0a 2020 436f 6e73  ...  """..  Cons
 0012fcb0: 7461 6e74 2064 6973 7461 6e63 6520 6174  tant distance at
 0012fcc0: 7465 6e75 6174 696f 6e20 636f 6566 6669  tenuation coeffi
@@ -77918,16 +77918,16 @@
 001305d0: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 001305e0: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 001305f0: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 00130600: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 00130610: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 00130620: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 00130630: 6c61 7373 2050 6f69 6e74 4c69 6768 7428  lass PointLight(
-00130640: 6270 795f 7374 7275 6374 2c20 4c69 6768  bpy_struct, Ligh
-00130650: 742c 2049 4429 3a0a 0a20 2022 2222 0a0a  t, ID):..  """..
+00130640: 6270 795f 7374 7275 6374 2c20 4944 2c20  bpy_struct, ID, 
+00130650: 4c69 6768 7429 3a0a 0a20 2022 2222 0a0a  Light):..  """..
 00130660: 2020 4f6d 6e69 6469 7265 6374 696f 6e61    Omnidirectiona
 00130670: 6c20 706f 696e 7420 4c69 6768 740a 0a20  l point Light.. 
 00130680: 2022 2222 0a0a 2020 636f 6e73 7461 6e74   """..  constant
 00130690: 5f63 6f65 6666 6963 6965 6e74 3a20 666c  _coefficient: fl
 001306a0: 6f61 7420 3d20 2e2e 2e0a 0a20 2022 2222  oat = .....  """
 001306b0: 0a0a 2020 436f 6e73 7461 6e74 2064 6973  ..  Constant dis
 001306c0: 7461 6e63 6520 6174 7465 6e75 6174 696f  tance attenuatio
@@ -78054,15 +78054,15 @@
 00130e50: 6765 745f 7375 6263 6c61 7373 5f70 7928  get_subclass_py(
 00130e60: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 00130e70: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 00130e80: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 00130e90: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 00130ea0: 2e2e 0a0a 636c 6173 7320 5370 6f74 4c69  ....class SpotLi
 00130eb0: 6768 7428 6270 795f 7374 7275 6374 2c20  ght(bpy_struct, 
-00130ec0: 4c69 6768 742c 2049 4429 3a0a 0a20 2022  Light, ID):..  "
+00130ec0: 4944 2c20 4c69 6768 7429 3a0a 0a20 2022  ID, Light):..  "
 00130ed0: 2222 0a0a 2020 4469 7265 6374 696f 6e61  ""..  Directiona
 00130ee0: 6c20 636f 6e65 204c 6967 6874 0a0a 2020  l cone Light..  
 00130ef0: 2222 220a 0a20 2063 6f6e 7374 616e 745f  """..  constant_
 00130f00: 636f 6566 6669 6369 656e 743a 2066 6c6f  coefficient: flo
 00130f10: 6174 203d 202e 2e2e 0a0a 2020 2222 220a  at = .....  """.
 00130f20: 0a20 2043 6f6e 7374 616e 7420 6469 7374  .  Constant dist
 00130f30: 616e 6365 2061 7474 656e 7561 7469 6f6e  ance attenuation
@@ -78211,16 +78211,16 @@
 00131820: 640a 0a20 2064 6566 2062 6c5f 726e 615f  d..  def bl_rna_
 00131830: 6765 745f 7375 6263 6c61 7373 5f70 7928  get_subclass_py(
 00131840: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 00131850: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 00131860: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 00131870: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 00131880: 2e2e 0a0a 636c 6173 7320 5375 6e4c 6967  ....class SunLig
-00131890: 6874 2862 7079 5f73 7472 7563 742c 204c  ht(bpy_struct, L
-001318a0: 6967 6874 2c20 4944 293a 0a0a 2020 2222  ight, ID):..  ""
+00131890: 6874 2862 7079 5f73 7472 7563 742c 2049  ht(bpy_struct, I
+001318a0: 442c 204c 6967 6874 293a 0a0a 2020 2222  D, Light):..  ""
 001318b0: 220a 0a20 2043 6f6e 7374 616e 7420 6469  "..  Constant di
 001318c0: 7265 6374 696f 6e20 7061 7261 6c6c 656c  rection parallel
 001318d0: 2072 6179 204c 6967 6874 0a0a 2020 2222   ray Light..  ""
 001318e0: 220a 0a20 2061 6e67 6c65 3a20 666c 6f61  "..  angle: floa
 001318f0: 7420 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  t = .....  """..
 00131900: 2020 416e 6775 6c61 7220 6469 616d 6574    Angular diamet
 00131910: 6572 206f 6620 7468 6520 5375 6e20 6173  er of the Sun as
@@ -78342,16 +78342,16 @@
 00132050: 5f67 6574 5f73 7562 636c 6173 735f 7079  _get_subclass_py
 00132060: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 00132070: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 00132080: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 00132090: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 001320a0: 2e2e 2e0a 0a63 6c61 7373 2043 6f6d 706f  .....class Compo
 001320b0: 7369 746f 724e 6f64 6554 7265 6528 6270  sitorNodeTree(bp
-001320c0: 795f 7374 7275 6374 2c20 4e6f 6465 5472  y_struct, NodeTr
-001320d0: 6565 2c20 4944 293a 0a0a 2020 2222 220a  ee, ID):..  """.
+001320c0: 795f 7374 7275 6374 2c20 4944 2c20 4e6f  y_struct, ID, No
+001320d0: 6465 5472 6565 293a 0a0a 2020 2222 220a  deTree):..  """.
 001320e0: 0a20 204e 6f64 6520 7472 6565 2063 6f6e  .  Node tree con
 001320f0: 7369 7374 696e 6720 6f66 206c 696e 6b65  sisting of linke
 00132100: 6420 6e6f 6465 7320 7573 6564 2066 6f72  d nodes used for
 00132110: 2063 6f6d 706f 7369 7469 6e67 0a0a 2020   compositing..  
 00132120: 2222 220a 0a20 2063 6875 6e6b 5f73 697a  """..  chunk_siz
 00132130: 653a 2073 7472 203d 202e 2e2e 0a0a 2020  e: str = .....  
 00132140: 2222 220a 0a20 204d 6178 2073 697a 6520  """..  Max size 
@@ -78454,15 +78454,15 @@
 00132750: 5f73 7562 636c 6173 735f 7079 2863 6c73  _subclass_py(cls
 00132760: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 00132770: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 00132780: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 00132790: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 001327a0: 0a63 6c61 7373 2047 656f 6d65 7472 794e  .class GeometryN
 001327b0: 6f64 6554 7265 6528 6270 795f 7374 7275  odeTree(bpy_stru
-001327c0: 6374 2c20 4e6f 6465 5472 6565 2c20 4944  ct, NodeTree, ID
+001327c0: 6374 2c20 4944 2c20 4e6f 6465 5472 6565  ct, ID, NodeTree
 001327d0: 293a 0a0a 2020 2222 220a 0a20 204e 6f64  ):..  """..  Nod
 001327e0: 6520 7472 6565 2063 6f6e 7369 7374 696e  e tree consistin
 001327f0: 6720 6f66 206c 696e 6b65 6420 6e6f 6465  g of linked node
 00132800: 7320 7573 6564 2066 6f72 2067 656f 6d65  s used for geome
 00132810: 7472 6965 730a 0a20 2022 2222 0a0a 2020  tries..  """..  
 00132820: 4063 6c61 7373 6d65 7468 6f64 0a0a 2020  @classmethod..  
 00132830: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
@@ -78475,16 +78475,16 @@
 001328a0: 726e 615f 6765 745f 7375 6263 6c61 7373  rna_get_subclass
 001328b0: 5f70 7928 636c 732c 2069 643a 2073 7472  _py(cls, id: str
 001328c0: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 001328d0: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 001328e0: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 001328f0: 2020 202e 2e2e 0a0a 636c 6173 7320 5368     .....class Sh
 00132900: 6164 6572 4e6f 6465 5472 6565 2862 7079  aderNodeTree(bpy
-00132910: 5f73 7472 7563 742c 204e 6f64 6554 7265  _struct, NodeTre
-00132920: 652c 2049 4429 3a0a 0a20 2022 2222 0a0a  e, ID):..  """..
+00132910: 5f73 7472 7563 742c 2049 442c 204e 6f64  _struct, ID, Nod
+00132920: 6554 7265 6529 3a0a 0a20 2022 2222 0a0a  eTree):..  """..
 00132930: 2020 4e6f 6465 2074 7265 6520 636f 6e73    Node tree cons
 00132940: 6973 7469 6e67 206f 6620 6c69 6e6b 6564  isting of linked
 00132950: 206e 6f64 6573 2075 7365 6420 666f 7220   nodes used for 
 00132960: 6d61 7465 7269 616c 7320 2861 6e64 206f  materials (and o
 00132970: 7468 6572 2073 6861 6469 6e67 2064 6174  ther shading dat
 00132980: 612d 626c 6f63 6b73 290a 0a20 2022 2222  a-blocks)..  """
 00132990: 0a0a 2020 6465 6620 6765 745f 6f75 7470  ..  def get_outp
@@ -78508,15 +78508,15 @@
 00132ab0: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 00132ac0: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 00132ad0: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 00132ae0: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 00132af0: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 00132b00: 6c61 7373 2054 6578 7475 7265 4e6f 6465  lass TextureNode
 00132b10: 5472 6565 2862 7079 5f73 7472 7563 742c  Tree(bpy_struct,
-00132b20: 204e 6f64 6554 7265 652c 2049 4429 3a0a   NodeTree, ID):.
+00132b20: 2049 442c 204e 6f64 6554 7265 6529 3a0a   ID, NodeTree):.
 00132b30: 0a20 2022 2222 0a0a 2020 4e6f 6465 2074  .  """..  Node t
 00132b40: 7265 6520 636f 6e73 6973 7469 6e67 206f  ree consisting o
 00132b50: 6620 6c69 6e6b 6564 206e 6f64 6573 2075  f linked nodes u
 00132b60: 7365 6420 666f 7220 7465 7874 7572 6573  sed for textures
 00132b70: 0a0a 2020 2222 220a 0a20 2040 636c 6173  ..  """..  @clas
 00132b80: 736d 6574 686f 640a 0a20 2064 6566 2062  smethod..  def b
 00132b90: 6c5f 726e 615f 6765 745f 7375 6263 6c61  l_rna_get_subcla
@@ -78529,15 +78529,15 @@
 00132c00: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 00132c10: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 00132c20: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 00132c30: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 00132c40: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 00132c50: 2e0a 0a63 6c61 7373 2042 6c65 6e64 5465  ...class BlendTe
 00132c60: 7874 7572 6528 6270 795f 7374 7275 6374  xture(bpy_struct
-00132c70: 2c20 5465 7874 7572 652c 2049 4429 3a0a  , Texture, ID):.
+00132c70: 2c20 4944 2c20 5465 7874 7572 6529 3a0a  , ID, Texture):.
 00132c80: 0a20 2022 2222 0a0a 2020 5072 6f63 6564  .  """..  Proced
 00132c90: 7572 616c 2063 6f6c 6f72 2062 6c65 6e64  ural color blend
 00132ca0: 696e 6720 7465 7874 7572 650a 0a20 2022  ing texture..  "
 00132cb0: 2222 0a0a 2020 7072 6f67 7265 7373 696f  ""..  progressio
 00132cc0: 6e3a 2073 7472 203d 202e 2e2e 0a0a 2020  n: str = .....  
 00132cd0: 2222 220a 0a20 2053 7479 6c65 206f 6620  """..  Style of 
 00132ce0: 7468 6520 636f 6c6f 7220 626c 656e 6469  the color blendi
@@ -78608,16 +78608,16 @@
 001330f0: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 00133100: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 00133110: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 00133120: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 00133130: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 00133140: 2020 2e2e 2e0a 0a63 6c61 7373 2043 6c6f    .....class Clo
 00133150: 7564 7354 6578 7475 7265 2862 7079 5f73  udsTexture(bpy_s
-00133160: 7472 7563 742c 2054 6578 7475 7265 2c20  truct, Texture, 
-00133170: 4944 293a 0a0a 2020 2222 220a 0a20 2050  ID):..  """..  P
+00133160: 7472 7563 742c 2049 442c 2054 6578 7475  truct, ID, Textu
+00133170: 7265 293a 0a0a 2020 2222 220a 0a20 2050  re):..  """..  P
 00133180: 726f 6365 6475 7261 6c20 6e6f 6973 6520  rocedural noise 
 00133190: 7465 7874 7572 650a 0a20 2022 2222 0a0a  texture..  """..
 001331a0: 2020 636c 6f75 645f 7479 7065 3a20 7374    cloud_type: st
 001331b0: 7220 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  r = .....  """..
 001331c0: 2020 4465 7465 726d 696e 6520 7768 6574    Determine whet
 001331d0: 6865 7220 4e6f 6973 6520 7265 7475 726e  her Noise return
 001331e0: 7320 6772 6179 7363 616c 6520 6f72 2052  s grayscale or R
@@ -78744,15 +78744,15 @@
 00133970: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 00133980: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 00133990: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 001339a0: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 001339b0: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 001339c0: 2044 6973 746f 7274 6564 4e6f 6973 6554   DistortedNoiseT
 001339d0: 6578 7475 7265 2862 7079 5f73 7472 7563  exture(bpy_struc
-001339e0: 742c 2054 6578 7475 7265 2c20 4944 293a  t, Texture, ID):
+001339e0: 742c 2049 442c 2054 6578 7475 7265 293a  t, ID, Texture):
 001339f0: 0a0a 2020 2222 220a 0a20 2050 726f 6365  ..  """..  Proce
 00133a00: 6475 7261 6c20 6469 7374 6f72 7465 6420  dural distorted 
 00133a10: 6e6f 6973 6520 7465 7874 7572 650a 0a20  noise texture.. 
 00133a20: 2022 2222 0a0a 2020 6469 7374 6f72 7469   """..  distorti
 00133a30: 6f6e 3a20 666c 6f61 7420 3d20 2e2e 2e0a  on: float = ....
 00133a40: 0a20 2022 2222 0a0a 2020 416d 6f75 6e74  .  """..  Amount
 00133a50: 206f 6620 6469 7374 6f72 7469 6f6e 0a0a   of distortion..
@@ -78933,15 +78933,15 @@
 00134540: 5f67 6574 5f73 7562 636c 6173 735f 7079  _get_subclass_py
 00134550: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 00134560: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 00134570: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 00134580: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 00134590: 2e2e 2e0a 0a63 6c61 7373 2049 6d61 6765  .....class Image
 001345a0: 5465 7874 7572 6528 6270 795f 7374 7275  Texture(bpy_stru
-001345b0: 6374 2c20 5465 7874 7572 652c 2049 4429  ct, Texture, ID)
+001345b0: 6374 2c20 4944 2c20 5465 7874 7572 6529  ct, ID, Texture)
 001345c0: 3a0a 0a20 2063 6865 636b 6572 5f64 6973  :..  checker_dis
 001345d0: 7461 6e63 653a 2066 6c6f 6174 203d 202e  tance: float = .
 001345e0: 2e2e 0a0a 2020 2222 220a 0a20 2044 6973  ....  """..  Dis
 001345f0: 7461 6e63 6520 6265 7477 6565 6e20 6368  tance between ch
 00134600: 6563 6b65 7220 7469 6c65 730a 0a20 2022  ecker tiles..  "
 00134610: 2222 0a0a 2020 6372 6f70 5f6d 6178 5f78  ""..  crop_max_x
 00134620: 3a20 666c 6f61 7420 3d20 2e2e 2e0a 0a20  : float = ..... 
@@ -79140,16 +79140,16 @@
 00135230: 626c 5f72 6e61 5f67 6574 5f73 7562 636c  bl_rna_get_subcl
 00135240: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 00135250: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 00135260: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 00135270: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 00135280: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 00135290: 204d 6167 6963 5465 7874 7572 6528 6270   MagicTexture(bp
-001352a0: 795f 7374 7275 6374 2c20 5465 7874 7572  y_struct, Textur
-001352b0: 652c 2049 4429 3a0a 0a20 2022 2222 0a0a  e, ID):..  """..
+001352a0: 795f 7374 7275 6374 2c20 4944 2c20 5465  y_struct, ID, Te
+001352b0: 7874 7572 6529 3a0a 0a20 2022 2222 0a0a  xture):..  """..
 001352c0: 2020 5072 6f63 6564 7572 616c 206e 6f69    Procedural noi
 001352d0: 7365 2074 6578 7475 7265 0a0a 2020 2222  se texture..  ""
 001352e0: 220a 0a20 206e 6f69 7365 5f64 6570 7468  "..  noise_depth
 001352f0: 3a20 696e 7420 3d20 2e2e 2e0a 0a20 2022  : int = .....  "
 00135300: 2222 0a0a 2020 4465 7074 6820 6f66 2074  ""..  Depth of t
 00135310: 6865 206e 6f69 7365 0a0a 2020 2222 220a  he noise..  """.
 00135320: 0a20 2074 7572 6275 6c65 6e63 653a 2066  .  turbulence: f
@@ -79181,15 +79181,15 @@
 001354c0: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 001354d0: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 001354e0: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 001354f0: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 00135500: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 00135510: 2e0a 0a63 6c61 7373 204d 6172 626c 6554  ...class MarbleT
 00135520: 6578 7475 7265 2862 7079 5f73 7472 7563  exture(bpy_struc
-00135530: 742c 2054 6578 7475 7265 2c20 4944 293a  t, Texture, ID):
+00135530: 742c 2049 442c 2054 6578 7475 7265 293a  t, ID, Texture):
 00135540: 0a0a 2020 2222 220a 0a20 2050 726f 6365  ..  """..  Proce
 00135550: 6475 7261 6c20 6e6f 6973 6520 7465 7874  dural noise text
 00135560: 7572 650a 0a20 2022 2222 0a0a 2020 6d61  ure..  """..  ma
 00135570: 7262 6c65 5f74 7970 653a 2073 7472 203d  rble_type: str =
 00135580: 202e 2e2e 0a0a 2020 2222 220a 0a20 202a   .....  """..  *
 00135590: 2060 6053 4f46 5460 600a 536f 6674 202d   ``SOFT``.Soft -
 001355a0: 2d20 5573 6520 736f 6674 206d 6172 626c  - Use soft marbl
@@ -79341,16 +79341,16 @@
 00135ec0: 5f67 6574 5f73 7562 636c 6173 735f 7079  _get_subclass_py
 00135ed0: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 00135ee0: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 00135ef0: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 00135f00: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 00135f10: 2e2e 2e0a 0a63 6c61 7373 204d 7573 6772  .....class Musgr
 00135f20: 6176 6554 6578 7475 7265 2862 7079 5f73  aveTexture(bpy_s
-00135f30: 7472 7563 742c 2054 6578 7475 7265 2c20  truct, Texture, 
-00135f40: 4944 293a 0a0a 2020 2222 220a 0a20 2050  ID):..  """..  P
+00135f30: 7472 7563 742c 2049 442c 2054 6578 7475  truct, ID, Textu
+00135f40: 7265 293a 0a0a 2020 2222 220a 0a20 2050  re):..  """..  P
 00135f50: 726f 6365 6475 7261 6c20 6d75 7367 7261  rocedural musgra
 00135f60: 7665 2074 6578 7475 7265 0a0a 2020 2222  ve texture..  ""
 00135f70: 220a 0a20 2064 696d 656e 7369 6f6e 5f6d  "..  dimension_m
 00135f80: 6178 3a20 666c 6f61 7420 3d20 2e2e 2e0a  ax: float = ....
 00135f90: 0a20 2022 2222 0a0a 2020 4869 6768 6573  .  """..  Highes
 00135fa0: 7420 6672 6163 7461 6c20 6469 6d65 6e73  t fractal dimens
 00135fb0: 696f 6e0a 0a20 2022 2222 0a0a 2020 6761  ion..  """..  ga
@@ -79510,16 +79510,16 @@
 00136950: 6c5f 726e 615f 6765 745f 7375 6263 6c61  l_rna_get_subcla
 00136960: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 00136970: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 00136980: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 00136990: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 001369a0: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 001369b0: 4e6f 6973 6554 6578 7475 7265 2862 7079  NoiseTexture(bpy
-001369c0: 5f73 7472 7563 742c 2054 6578 7475 7265  _struct, Texture
-001369d0: 2c20 4944 293a 0a0a 2020 2222 220a 0a20  , ID):..  """.. 
+001369c0: 5f73 7472 7563 742c 2049 442c 2054 6578  _struct, ID, Tex
+001369d0: 7475 7265 293a 0a0a 2020 2222 220a 0a20  ture):..  """.. 
 001369e0: 2050 726f 6365 6475 7261 6c20 6e6f 6973   Procedural nois
 001369f0: 6520 7465 7874 7572 650a 0a20 2022 2222  e texture..  """
 00136a00: 0a0a 2020 7573 6572 735f 6d61 7465 7269  ..  users_materi
 00136a10: 616c 3a20 7479 7069 6e67 2e41 6e79 203d  al: typing.Any =
 00136a20: 202e 2e2e 0a0a 2020 2222 220a 0a20 204d   .....  """..  M
 00136a30: 6174 6572 6961 6c73 2074 6861 7420 7573  aterials that us
 00136a40: 6520 7468 6973 2074 6578 7475 7265 0a0a  e this texture..
@@ -79543,15 +79543,15 @@
 00136b60: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 00136b70: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 00136b80: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 00136b90: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 00136ba0: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 00136bb0: 636c 6173 7320 5374 7563 6369 5465 7874  class StucciText
 00136bc0: 7572 6528 6270 795f 7374 7275 6374 2c20  ure(bpy_struct, 
-00136bd0: 5465 7874 7572 652c 2049 4429 3a0a 0a20  Texture, ID):.. 
+00136bd0: 4944 2c20 5465 7874 7572 6529 3a0a 0a20  ID, Texture):.. 
 00136be0: 2022 2222 0a0a 2020 5072 6f63 6564 7572   """..  Procedur
 00136bf0: 616c 206e 6f69 7365 2074 6578 7475 7265  al noise texture
 00136c00: 0a0a 2020 2222 220a 0a20 206e 6f69 7365  ..  """..  noise
 00136c10: 5f62 6173 6973 3a20 7374 7220 3d20 2e2e  _basis: str = ..
 00136c20: 2e0a 0a20 2022 2222 0a0a 2020 4e6f 6973  ...  """..  Nois
 00136c30: 6520 6261 7369 7320 7573 6564 2066 6f72  e basis used for
 00136c40: 2074 7572 6275 6c65 6e63 650a 0a20 202a   turbulence..  *
@@ -79677,15 +79677,15 @@
 001373c0: 5f73 7562 636c 6173 735f 7079 2863 6c73  _subclass_py(cls
 001373d0: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 001373e0: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 001373f0: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 00137400: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 00137410: 0a63 6c61 7373 2056 6f72 6f6e 6f69 5465  .class VoronoiTe
 00137420: 7874 7572 6528 6270 795f 7374 7275 6374  xture(bpy_struct
-00137430: 2c20 5465 7874 7572 652c 2049 4429 3a0a  , Texture, ID):.
+00137430: 2c20 4944 2c20 5465 7874 7572 6529 3a0a  , ID, Texture):.
 00137440: 0a20 2022 2222 0a0a 2020 5072 6f63 6564  .  """..  Proced
 00137450: 7572 616c 2076 6f72 6f6e 6f69 2074 6578  ural voronoi tex
 00137460: 7475 7265 0a0a 2020 2222 220a 0a20 2063  ture..  """..  c
 00137470: 6f6c 6f72 5f6d 6f64 653a 2073 7472 203d  olor_mode: str =
 00137480: 202e 2e2e 0a0a 2020 2222 220a 0a20 202a   .....  """..  *
 00137490: 2060 6049 4e54 454e 5349 5459 6060 0a49   ``INTENSITY``.I
 001374a0: 6e74 656e 7369 7479 202d 2d20 4f6e 6c79  ntensity -- Only
@@ -79810,16 +79810,16 @@
 00137c10: 5f72 6e61 5f67 6574 5f73 7562 636c 6173  _rna_get_subclas
 00137c20: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 00137c30: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 00137c40: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 00137c50: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 00137c60: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2057      .....class W
 00137c70: 6f6f 6454 6578 7475 7265 2862 7079 5f73  oodTexture(bpy_s
-00137c80: 7472 7563 742c 2054 6578 7475 7265 2c20  truct, Texture, 
-00137c90: 4944 293a 0a0a 2020 2222 220a 0a20 2050  ID):..  """..  P
+00137c80: 7472 7563 742c 2049 442c 2054 6578 7475  truct, ID, Textu
+00137c90: 7265 293a 0a0a 2020 2222 220a 0a20 2050  re):..  """..  P
 00137ca0: 726f 6365 6475 7261 6c20 6e6f 6973 6520  rocedural noise 
 00137cb0: 7465 7874 7572 650a 0a20 2022 2222 0a0a  texture..  """..
 00137cc0: 2020 6e61 626c 613a 2066 6c6f 6174 203d    nabla: float =
 00137cd0: 202e 2e2e 0a0a 2020 2222 220a 0a20 2053   .....  """..  S
 00137ce0: 697a 6520 6f66 2064 6572 6976 6174 6976  ize of derivativ
 00137cf0: 6520 6f66 6673 6574 2075 7365 6420 666f  e offset used fo
 00137d00: 7220 6361 6c63 756c 6174 696e 6720 6e6f  r calculating no
@@ -79972,16 +79972,16 @@
 00138630: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 00138640: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 00138650: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 00138660: 0a0a 636c 6173 7320 4c69 6e65 5374 796c  ..class LineStyl
 00138670: 6541 6c70 6861 4d6f 6469 6669 6572 5f41  eAlphaModifier_A
 00138680: 6c6f 6e67 5374 726f 6b65 2862 7079 5f73  longStroke(bpy_s
 00138690: 7472 7563 742c 204c 696e 6553 7479 6c65  truct, LineStyle
-001386a0: 4d6f 6469 6669 6572 2c20 4c69 6e65 5374  Modifier, LineSt
-001386b0: 796c 6541 6c70 6861 4d6f 6469 6669 6572  yleAlphaModifier
+001386a0: 416c 7068 614d 6f64 6966 6965 722c 204c  AlphaModifier, L
+001386b0: 696e 6553 7479 6c65 4d6f 6469 6669 6572  ineStyleModifier
 001386c0: 293a 0a0a 2020 2222 220a 0a20 2043 6861  ):..  """..  Cha
 001386d0: 6e67 6520 616c 7068 6120 7472 616e 7370  nge alpha transp
 001386e0: 6172 656e 6379 2061 6c6f 6e67 2073 7472  arency along str
 001386f0: 6f6b 650a 0a20 2022 2222 0a0a 2020 626c  oke..  """..  bl
 00138700: 656e 643a 2073 7472 203d 202e 2e2e 0a0a  end: str = .....
 00138710: 2020 2222 220a 0a20 2053 7065 6369 6679    """..  Specify
 00138720: 2068 6f77 2074 6865 206d 6f64 6966 6965   how the modifie
@@ -80045,17 +80045,17 @@
 00138ac0: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 00138ad0: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 00138ae0: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 00138af0: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 00138b00: 6173 7320 4c69 6e65 5374 796c 6541 6c70  ass LineStyleAlp
 00138b10: 6861 4d6f 6469 6669 6572 5f43 7265 6173  haModifier_Creas
 00138b20: 6541 6e67 6c65 2862 7079 5f73 7472 7563  eAngle(bpy_struc
-00138b30: 742c 204c 696e 6553 7479 6c65 4d6f 6469  t, LineStyleModi
-00138b40: 6669 6572 2c20 4c69 6e65 5374 796c 6541  fier, LineStyleA
-00138b50: 6c70 6861 4d6f 6469 6669 6572 293a 0a0a  lphaModifier):..
+00138b30: 742c 204c 696e 6553 7479 6c65 416c 7068  t, LineStyleAlph
+00138b40: 614d 6f64 6966 6965 722c 204c 696e 6553  aModifier, LineS
+00138b50: 7479 6c65 4d6f 6469 6669 6572 293a 0a0a  tyleModifier):..
 00138b60: 2020 2222 220a 0a20 2041 6c70 6861 2074    """..  Alpha t
 00138b70: 7261 6e73 7061 7265 6e63 7920 6261 7365  ransparency base
 00138b80: 6420 6f6e 2074 6865 2061 6e67 6c65 2062  d on the angle b
 00138b90: 6574 7765 656e 2074 776f 2061 646a 6163  etween two adjac
 00138ba0: 656e 7420 6661 6365 730a 0a20 2022 2222  ent faces..  """
 00138bb0: 0a0a 2020 616e 676c 655f 6d61 783a 2066  ..  angle_max: f
 00138bc0: 6c6f 6174 203d 202e 2e2e 0a0a 2020 2222  loat = .....  ""
@@ -80130,17 +80130,17 @@
 00139010: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 00139020: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 00139030: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 00139040: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 00139050: 6173 7320 4c69 6e65 5374 796c 6541 6c70  ass LineStyleAlp
 00139060: 6861 4d6f 6469 6669 6572 5f43 7572 7661  haModifier_Curva
 00139070: 7475 7265 5f33 4428 6270 795f 7374 7275  ture_3D(bpy_stru
-00139080: 6374 2c20 4c69 6e65 5374 796c 654d 6f64  ct, LineStyleMod
-00139090: 6966 6965 722c 204c 696e 6553 7479 6c65  ifier, LineStyle
-001390a0: 416c 7068 614d 6f64 6966 6965 7229 3a0a  AlphaModifier):.
+00139080: 6374 2c20 4c69 6e65 5374 796c 6541 6c70  ct, LineStyleAlp
+00139090: 6861 4d6f 6469 6669 6572 2c20 4c69 6e65  haModifier, Line
+001390a0: 5374 796c 654d 6f64 6966 6965 7229 3a0a  StyleModifier):.
 001390b0: 0a20 2022 2222 0a0a 2020 416c 7068 6120  .  """..  Alpha 
 001390c0: 7472 616e 7370 6172 656e 6379 2062 6173  transparency bas
 001390d0: 6564 206f 6e20 7468 6520 7261 6469 616c  ed on the radial
 001390e0: 2063 7572 7661 7475 7265 206f 6620 3344   curvature of 3D
 001390f0: 206d 6573 6820 7375 7266 6163 6573 0a0a   mesh surfaces..
 00139100: 2020 2222 220a 0a20 2062 6c65 6e64 3a20    """..  blend: 
 00139110: 7374 7220 3d20 2e2e 2e0a 0a20 2022 2222  str = .....  """
@@ -80215,16 +80215,16 @@
 00139560: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 00139570: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 00139580: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 00139590: 204c 696e 6553 7479 6c65 416c 7068 614d   LineStyleAlphaM
 001395a0: 6f64 6966 6965 725f 4469 7374 616e 6365  odifier_Distance
 001395b0: 4672 6f6d 4361 6d65 7261 2862 7079 5f73  FromCamera(bpy_s
 001395c0: 7472 7563 742c 204c 696e 6553 7479 6c65  truct, LineStyle
-001395d0: 4d6f 6469 6669 6572 2c20 4c69 6e65 5374  Modifier, LineSt
-001395e0: 796c 6541 6c70 6861 4d6f 6469 6669 6572  yleAlphaModifier
+001395d0: 416c 7068 614d 6f64 6966 6965 722c 204c  AlphaModifier, L
+001395e0: 696e 6553 7479 6c65 4d6f 6469 6669 6572  ineStyleModifier
 001395f0: 293a 0a0a 2020 2222 220a 0a20 2043 6861  ):..  """..  Cha
 00139600: 6e67 6520 616c 7068 6120 7472 616e 7370  nge alpha transp
 00139610: 6172 656e 6379 2062 6173 6564 206f 6e20  arency based on 
 00139620: 7468 6520 6469 7374 616e 6365 2066 726f  the distance fro
 00139630: 6d20 7468 6520 6361 6d65 7261 0a0a 2020  m the camera..  
 00139640: 2222 220a 0a20 2062 6c65 6e64 3a20 7374  """..  blend: st
 00139650: 7220 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  r = .....  """..
@@ -80302,17 +80302,17 @@
 00139ad0: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 00139ae0: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 00139af0: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 00139b00: 2020 2020 2e2e 2e0a 0a63 6c61 7373 204c      .....class L
 00139b10: 696e 6553 7479 6c65 416c 7068 614d 6f64  ineStyleAlphaMod
 00139b20: 6966 6965 725f 4469 7374 616e 6365 4672  ifier_DistanceFr
 00139b30: 6f6d 4f62 6a65 6374 2862 7079 5f73 7472  omObject(bpy_str
-00139b40: 7563 742c 204c 696e 6553 7479 6c65 4d6f  uct, LineStyleMo
-00139b50: 6469 6669 6572 2c20 4c69 6e65 5374 796c  difier, LineStyl
-00139b60: 6541 6c70 6861 4d6f 6469 6669 6572 293a  eAlphaModifier):
+00139b40: 7563 742c 204c 696e 6553 7479 6c65 416c  uct, LineStyleAl
+00139b50: 7068 614d 6f64 6966 6965 722c 204c 696e  phaModifier, Lin
+00139b60: 6553 7479 6c65 4d6f 6469 6669 6572 293a  eStyleModifier):
 00139b70: 0a0a 2020 2222 220a 0a20 2043 6861 6e67  ..  """..  Chang
 00139b80: 6520 616c 7068 6120 7472 616e 7370 6172  e alpha transpar
 00139b90: 656e 6379 2062 6173 6564 206f 6e20 7468  ency based on th
 00139ba0: 6520 6469 7374 616e 6365 2066 726f 6d20  e distance from 
 00139bb0: 616e 206f 626a 6563 740a 0a20 2022 2222  an object..  """
 00139bc0: 0a0a 2020 626c 656e 643a 2073 7472 203d  ..  blend: str =
 00139bd0: 202e 2e2e 0a0a 2020 2222 220a 0a20 2053   .....  """..  S
@@ -80395,17 +80395,17 @@
 0013a0a0: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 0013a0b0: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 0013a0c0: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 0013a0d0: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 0013a0e0: 0a63 6c61 7373 204c 696e 6553 7479 6c65  .class LineStyle
 0013a0f0: 416c 7068 614d 6f64 6966 6965 725f 4d61  AlphaModifier_Ma
 0013a100: 7465 7269 616c 2862 7079 5f73 7472 7563  terial(bpy_struc
-0013a110: 742c 204c 696e 6553 7479 6c65 4d6f 6469  t, LineStyleModi
-0013a120: 6669 6572 2c20 4c69 6e65 5374 796c 6541  fier, LineStyleA
-0013a130: 6c70 6861 4d6f 6469 6669 6572 293a 0a0a  lphaModifier):..
+0013a110: 742c 204c 696e 6553 7479 6c65 416c 7068  t, LineStyleAlph
+0013a120: 614d 6f64 6966 6965 722c 204c 696e 6553  aModifier, LineS
+0013a130: 7479 6c65 4d6f 6469 6669 6572 293a 0a0a  tyleModifier):..
 0013a140: 2020 2222 220a 0a20 2043 6861 6e67 6520    """..  Change 
 0013a150: 616c 7068 6120 7472 616e 7370 6172 656e  alpha transparen
 0013a160: 6379 2062 6173 6564 206f 6e20 6120 6d61  cy based on a ma
 0013a170: 7465 7269 616c 2061 7474 7269 6275 7465  terial attribute
 0013a180: 0a0a 2020 2222 220a 0a20 2062 6c65 6e64  ..  """..  blend
 0013a190: 3a20 7374 7220 3d20 2e2e 2e0a 0a20 2022  : str = .....  "
 0013a1a0: 2222 0a0a 2020 5370 6563 6966 7920 686f  ""..  Specify ho
@@ -80475,17 +80475,17 @@
 0013a5a0: 7928 636c 732c 2069 643a 2073 7472 2c20  y(cls, id: str, 
 0013a5b0: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 0013a5c0: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 0013a5d0: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 0013a5e0: 202e 2e2e 0a0a 636c 6173 7320 4c69 6e65   .....class Line
 0013a5f0: 5374 796c 6541 6c70 6861 4d6f 6469 6669  StyleAlphaModifi
 0013a600: 6572 5f4e 6f69 7365 2862 7079 5f73 7472  er_Noise(bpy_str
-0013a610: 7563 742c 204c 696e 6553 7479 6c65 4d6f  uct, LineStyleMo
-0013a620: 6469 6669 6572 2c20 4c69 6e65 5374 796c  difier, LineStyl
-0013a630: 6541 6c70 6861 4d6f 6469 6669 6572 293a  eAlphaModifier):
+0013a610: 7563 742c 204c 696e 6553 7479 6c65 416c  uct, LineStyleAl
+0013a620: 7068 614d 6f64 6966 6965 722c 204c 696e  phaModifier, Lin
+0013a630: 6553 7479 6c65 4d6f 6469 6669 6572 293a  eStyleModifier):
 0013a640: 0a0a 2020 2222 220a 0a20 2041 6c70 6861  ..  """..  Alpha
 0013a650: 2074 7261 6e73 7061 7265 6e63 7920 6261   transparency ba
 0013a660: 7365 6420 6f6e 2072 616e 646f 6d20 6e6f  sed on random no
 0013a670: 6973 650a 0a20 2022 2222 0a0a 2020 616d  ise..  """..  am
 0013a680: 706c 6974 7564 653a 2066 6c6f 6174 203d  plitude: float =
 0013a690: 202e 2e2e 0a0a 2020 2222 220a 0a20 2041   .....  """..  A
 0013a6a0: 6d70 6c69 7475 6465 206f 6620 7468 6520  mplitude of the 
@@ -80561,16 +80561,16 @@
 0013ab00: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 0013ab10: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 0013ab20: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 0013ab30: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 0013ab40: 6173 7320 4c69 6e65 5374 796c 6541 6c70  ass LineStyleAlp
 0013ab50: 6861 4d6f 6469 6669 6572 5f54 616e 6765  haModifier_Tange
 0013ab60: 6e74 2862 7079 5f73 7472 7563 742c 204c  nt(bpy_struct, L
-0013ab70: 696e 6553 7479 6c65 4d6f 6469 6669 6572  ineStyleModifier
-0013ab80: 2c20 4c69 6e65 5374 796c 6541 6c70 6861  , LineStyleAlpha
+0013ab70: 696e 6553 7479 6c65 416c 7068 614d 6f64  ineStyleAlphaMod
+0013ab80: 6966 6965 722c 204c 696e 6553 7479 6c65  ifier, LineStyle
 0013ab90: 4d6f 6469 6669 6572 293a 0a0a 2020 2222  Modifier):..  ""
 0013aba0: 220a 0a20 2041 6c70 6861 2074 7261 6e73  "..  Alpha trans
 0013abb0: 7061 7265 6e63 7920 6261 7365 6420 6f6e  parency based on
 0013abc0: 2074 6865 2064 6972 6563 7469 6f6e 206f   the direction o
 0013abd0: 6620 7468 6520 7374 726f 6b65 0a0a 2020  f the stroke..  
 0013abe0: 2222 220a 0a20 2062 6c65 6e64 3a20 7374  """..  blend: st
 0013abf0: 7220 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  r = .....  """..
@@ -80635,17 +80635,17 @@
 0013afa0: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 0013afb0: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 0013afc0: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 0013afd0: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 0013afe0: 2020 2e2e 2e0a 0a63 6c61 7373 204c 696e    .....class Lin
 0013aff0: 6553 7479 6c65 436f 6c6f 724d 6f64 6966  eStyleColorModif
 0013b000: 6965 725f 416c 6f6e 6753 7472 6f6b 6528  ier_AlongStroke(
-0013b010: 6270 795f 7374 7275 6374 2c20 4c69 6e65  bpy_struct, Line
-0013b020: 5374 796c 6543 6f6c 6f72 4d6f 6469 6669  StyleColorModifi
-0013b030: 6572 2c20 4c69 6e65 5374 796c 654d 6f64  er, LineStyleMod
+0013b010: 4c69 6e65 5374 796c 6543 6f6c 6f72 4d6f  LineStyleColorMo
+0013b020: 6469 6669 6572 2c20 6270 795f 7374 7275  difier, bpy_stru
+0013b030: 6374 2c20 4c69 6e65 5374 796c 654d 6f64  ct, LineStyleMod
 0013b040: 6966 6965 7229 3a0a 0a20 2022 2222 0a0a  ifier):..  """..
 0013b050: 2020 4368 616e 6765 206c 696e 6520 636f    Change line co
 0013b060: 6c6f 7220 616c 6f6e 6720 7374 726f 6b65  lor along stroke
 0013b070: 0a0a 2020 2222 220a 0a20 2062 6c65 6e64  ..  """..  blend
 0013b080: 3a20 7374 7220 3d20 2e2e 2e0a 0a20 2022  : str = .....  "
 0013b090: 2222 0a0a 2020 5370 6563 6966 7920 686f  ""..  Specify ho
 0013b0a0: 7720 7468 6520 6d6f 6469 6669 6572 2076  w the modifier v
@@ -80693,17 +80693,17 @@
 0013b340: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 0013b350: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 0013b360: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 0013b370: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 0013b380: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 0013b390: 6173 7320 4c69 6e65 5374 796c 6543 6f6c  ass LineStyleCol
 0013b3a0: 6f72 4d6f 6469 6669 6572 5f43 7265 6173  orModifier_Creas
-0013b3b0: 6541 6e67 6c65 2862 7079 5f73 7472 7563  eAngle(bpy_struc
-0013b3c0: 742c 204c 696e 6553 7479 6c65 436f 6c6f  t, LineStyleColo
-0013b3d0: 724d 6f64 6966 6965 722c 204c 696e 6553  rModifier, LineS
+0013b3b0: 6541 6e67 6c65 284c 696e 6553 7479 6c65  eAngle(LineStyle
+0013b3c0: 436f 6c6f 724d 6f64 6966 6965 722c 2062  ColorModifier, b
+0013b3d0: 7079 5f73 7472 7563 742c 204c 696e 6553  py_struct, LineS
 0013b3e0: 7479 6c65 4d6f 6469 6669 6572 293a 0a0a  tyleModifier):..
 0013b3f0: 2020 2222 220a 0a20 2043 6861 6e67 6520    """..  Change 
 0013b400: 6c69 6e65 2063 6f6c 6f72 2062 6173 6564  line color based
 0013b410: 206f 6e20 7468 6520 756e 6465 726c 7969   on the underlyi
 0013b420: 6e67 2063 7265 6173 6520 616e 676c 650a  ng crease angle.
 0013b430: 0a20 2022 2222 0a0a 2020 616e 676c 655f  .  """..  angle_
 0013b440: 6d61 783a 2066 6c6f 6174 203d 202e 2e2e  max: float = ...
@@ -80763,17 +80763,17 @@
 0013b7a0: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 0013b7b0: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 0013b7c0: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 0013b7d0: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 0013b7e0: 2020 2e2e 2e0a 0a63 6c61 7373 204c 696e    .....class Lin
 0013b7f0: 6553 7479 6c65 436f 6c6f 724d 6f64 6966  eStyleColorModif
 0013b800: 6965 725f 4375 7276 6174 7572 655f 3344  ier_Curvature_3D
-0013b810: 2862 7079 5f73 7472 7563 742c 204c 696e  (bpy_struct, Lin
-0013b820: 6553 7479 6c65 436f 6c6f 724d 6f64 6966  eStyleColorModif
-0013b830: 6965 722c 204c 696e 6553 7479 6c65 4d6f  ier, LineStyleMo
+0013b810: 284c 696e 6553 7479 6c65 436f 6c6f 724d  (LineStyleColorM
+0013b820: 6f64 6966 6965 722c 2062 7079 5f73 7472  odifier, bpy_str
+0013b830: 7563 742c 204c 696e 6553 7479 6c65 4d6f  uct, LineStyleMo
 0013b840: 6469 6669 6572 293a 0a0a 2020 2222 220a  difier):..  """.
 0013b850: 0a20 2043 6861 6e67 6520 6c69 6e65 2063  .  Change line c
 0013b860: 6f6c 6f72 2062 6173 6564 206f 6e20 7468  olor based on th
 0013b870: 6520 7261 6469 616c 2063 7572 7661 7475  e radial curvatu
 0013b880: 7265 206f 6620 3344 206d 6573 6820 7375  re of 3D mesh su
 0013b890: 7266 6163 6573 0a0a 2020 2222 220a 0a20  rfaces..  """.. 
 0013b8a0: 2062 6c65 6e64 3a20 7374 7220 3d20 2e2e   blend: str = ..
@@ -80832,17 +80832,17 @@
 0013bbf0: 7928 636c 732c 2069 643a 2073 7472 2c20  y(cls, id: str, 
 0013bc00: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 0013bc10: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 0013bc20: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 0013bc30: 202e 2e2e 0a0a 636c 6173 7320 4c69 6e65   .....class Line
 0013bc40: 5374 796c 6543 6f6c 6f72 4d6f 6469 6669  StyleColorModifi
 0013bc50: 6572 5f44 6973 7461 6e63 6546 726f 6d43  er_DistanceFromC
-0013bc60: 616d 6572 6128 6270 795f 7374 7275 6374  amera(bpy_struct
-0013bc70: 2c20 4c69 6e65 5374 796c 6543 6f6c 6f72  , LineStyleColor
-0013bc80: 4d6f 6469 6669 6572 2c20 4c69 6e65 5374  Modifier, LineSt
+0013bc60: 616d 6572 6128 4c69 6e65 5374 796c 6543  amera(LineStyleC
+0013bc70: 6f6c 6f72 4d6f 6469 6669 6572 2c20 6270  olorModifier, bp
+0013bc80: 795f 7374 7275 6374 2c20 4c69 6e65 5374  y_struct, LineSt
 0013bc90: 796c 654d 6f64 6966 6965 7229 3a0a 0a20  yleModifier):.. 
 0013bca0: 2022 2222 0a0a 2020 4368 616e 6765 206c   """..  Change l
 0013bcb0: 696e 6520 636f 6c6f 7220 6261 7365 6420  ine color based 
 0013bcc0: 6f6e 2074 6865 2064 6973 7461 6e63 6520  on the distance 
 0013bcd0: 6672 6f6d 2074 6865 2063 616d 6572 610a  from the camera.
 0013bce0: 0a20 2022 2222 0a0a 2020 626c 656e 643a  .  """..  blend:
 0013bcf0: 2073 7472 203d 202e 2e2e 0a0a 2020 2222   str = .....  ""
@@ -80904,18 +80904,18 @@
 0013c070: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 0013c080: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 0013c090: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 0013c0a0: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 0013c0b0: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 0013c0c0: 6c61 7373 204c 696e 6553 7479 6c65 436f  lass LineStyleCo
 0013c0d0: 6c6f 724d 6f64 6966 6965 725f 4469 7374  lorModifier_Dist
-0013c0e0: 616e 6365 4672 6f6d 4f62 6a65 6374 2862  anceFromObject(b
-0013c0f0: 7079 5f73 7472 7563 742c 204c 696e 6553  py_struct, LineS
-0013c100: 7479 6c65 436f 6c6f 724d 6f64 6966 6965  tyleColorModifie
-0013c110: 722c 204c 696e 6553 7479 6c65 4d6f 6469  r, LineStyleModi
+0013c0e0: 616e 6365 4672 6f6d 4f62 6a65 6374 284c  anceFromObject(L
+0013c0f0: 696e 6553 7479 6c65 436f 6c6f 724d 6f64  ineStyleColorMod
+0013c100: 6966 6965 722c 2062 7079 5f73 7472 7563  ifier, bpy_struc
+0013c110: 742c 204c 696e 6553 7479 6c65 4d6f 6469  t, LineStyleModi
 0013c120: 6669 6572 293a 0a0a 2020 2222 220a 0a20  fier):..  """.. 
 0013c130: 2043 6861 6e67 6520 6c69 6e65 2063 6f6c   Change line col
 0013c140: 6f72 2062 6173 6564 206f 6e20 7468 6520  or based on the 
 0013c150: 6469 7374 616e 6365 2066 726f 6d20 616e  distance from an
 0013c160: 206f 626a 6563 740a 0a20 2022 2222 0a0a   object..  """..
 0013c170: 2020 626c 656e 643a 2073 7472 203d 202e    blend: str = .
 0013c180: 2e2e 0a0a 2020 2222 220a 0a20 2053 7065  ....  """..  Spe
@@ -80982,17 +80982,17 @@
 0013c550: 745f 7375 6263 6c61 7373 5f70 7928 636c  t_subclass_py(cl
 0013c560: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 0013c570: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 0013c580: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 0013c590: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 0013c5a0: 0a0a 636c 6173 7320 4c69 6e65 5374 796c  ..class LineStyl
 0013c5b0: 6543 6f6c 6f72 4d6f 6469 6669 6572 5f4d  eColorModifier_M
-0013c5c0: 6174 6572 6961 6c28 6270 795f 7374 7275  aterial(bpy_stru
-0013c5d0: 6374 2c20 4c69 6e65 5374 796c 6543 6f6c  ct, LineStyleCol
-0013c5e0: 6f72 4d6f 6469 6669 6572 2c20 4c69 6e65  orModifier, Line
+0013c5c0: 6174 6572 6961 6c28 4c69 6e65 5374 796c  aterial(LineStyl
+0013c5d0: 6543 6f6c 6f72 4d6f 6469 6669 6572 2c20  eColorModifier, 
+0013c5e0: 6270 795f 7374 7275 6374 2c20 4c69 6e65  bpy_struct, Line
 0013c5f0: 5374 796c 654d 6f64 6966 6965 7229 3a0a  StyleModifier):.
 0013c600: 0a20 2022 2222 0a0a 2020 4368 616e 6765  .  """..  Change
 0013c610: 206c 696e 6520 636f 6c6f 7220 6261 7365   line color base
 0013c620: 6420 6f6e 2061 206d 6174 6572 6961 6c20  d on a material 
 0013c630: 6174 7472 6962 7574 650a 0a20 2022 2222  attribute..  """
 0013c640: 0a0a 2020 626c 656e 643a 2073 7472 203d  ..  blend: str =
 0013c650: 202e 2e2e 0a0a 2020 2222 220a 0a20 2053   .....  """..  S
@@ -81053,17 +81053,17 @@
 0013c9c0: 745f 7375 6263 6c61 7373 5f70 7928 636c  t_subclass_py(cl
 0013c9d0: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 0013c9e0: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 0013c9f0: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 0013ca00: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 0013ca10: 0a0a 636c 6173 7320 4c69 6e65 5374 796c  ..class LineStyl
 0013ca20: 6543 6f6c 6f72 4d6f 6469 6669 6572 5f4e  eColorModifier_N
-0013ca30: 6f69 7365 2862 7079 5f73 7472 7563 742c  oise(bpy_struct,
-0013ca40: 204c 696e 6553 7479 6c65 436f 6c6f 724d   LineStyleColorM
-0013ca50: 6f64 6966 6965 722c 204c 696e 6553 7479  odifier, LineSty
+0013ca30: 6f69 7365 284c 696e 6553 7479 6c65 436f  oise(LineStyleCo
+0013ca40: 6c6f 724d 6f64 6966 6965 722c 2062 7079  lorModifier, bpy
+0013ca50: 5f73 7472 7563 742c 204c 696e 6553 7479  _struct, LineSty
 0013ca60: 6c65 4d6f 6469 6669 6572 293a 0a0a 2020  leModifier):..  
 0013ca70: 2222 220a 0a20 2043 6861 6e67 6520 6c69  """..  Change li
 0013ca80: 6e65 2063 6f6c 6f72 2062 6173 6564 206f  ne color based o
 0013ca90: 6e20 7261 6e64 6f6d 206e 6f69 7365 0a0a  n random noise..
 0013caa0: 2020 2222 220a 0a20 2061 6d70 6c69 7475    """..  amplitu
 0013cab0: 6465 3a20 666c 6f61 7420 3d20 2e2e 2e0a  de: float = ....
 0013cac0: 0a20 2022 2222 0a0a 2020 416d 706c 6974  .  """..  Amplit
@@ -81124,17 +81124,17 @@
 0013ce30: 6c61 7373 5f70 7928 636c 732c 2069 643a  lass_py(cls, id:
 0013ce40: 2073 7472 2c20 6465 6661 756c 743a 2074   str, default: t
 0013ce50: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 0013ce60: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 0013ce70: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 0013ce80: 7320 4c69 6e65 5374 796c 6543 6f6c 6f72  s LineStyleColor
 0013ce90: 4d6f 6469 6669 6572 5f54 616e 6765 6e74  Modifier_Tangent
-0013cea0: 2862 7079 5f73 7472 7563 742c 204c 696e  (bpy_struct, Lin
-0013ceb0: 6553 7479 6c65 436f 6c6f 724d 6f64 6966  eStyleColorModif
-0013cec0: 6965 722c 204c 696e 6553 7479 6c65 4d6f  ier, LineStyleMo
+0013cea0: 284c 696e 6553 7479 6c65 436f 6c6f 724d  (LineStyleColorM
+0013ceb0: 6f64 6966 6965 722c 2062 7079 5f73 7472  odifier, bpy_str
+0013cec0: 7563 742c 204c 696e 6553 7479 6c65 4d6f  uct, LineStyleMo
 0013ced0: 6469 6669 6572 293a 0a0a 2020 2222 220a  difier):..  """.
 0013cee0: 0a20 2043 6861 6e67 6520 6c69 6e65 2063  .  Change line c
 0013cef0: 6f6c 6f72 2062 6173 6564 206f 6e20 7468  olor based on th
 0013cf00: 6520 6469 7265 6374 696f 6e20 6f66 2061  e direction of a
 0013cf10: 2073 7472 6f6b 650a 0a20 2022 2222 0a0a   stroke..  """..
 0013cf20: 2020 626c 656e 643a 2073 7472 203d 202e    blend: str = .
 0013cf30: 2e2e 0a0a 2020 2222 220a 0a20 2053 7065  ....  """..  Spe
@@ -82029,16 +82029,16 @@
 001406c0: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 001406d0: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 001406e0: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 001406f0: 0a63 6c61 7373 204c 696e 6553 7479 6c65  .class LineStyle
 00140700: 5468 6963 6b6e 6573 734d 6f64 6966 6965  ThicknessModifie
 00140710: 725f 416c 6f6e 6753 7472 6f6b 6528 6270  r_AlongStroke(bp
 00140720: 795f 7374 7275 6374 2c20 4c69 6e65 5374  y_struct, LineSt
-00140730: 796c 6554 6869 636b 6e65 7373 4d6f 6469  yleThicknessModi
-00140740: 6669 6572 2c20 4c69 6e65 5374 796c 654d  fier, LineStyleM
+00140730: 796c 654d 6f64 6966 6965 722c 204c 696e  yleModifier, Lin
+00140740: 6553 7479 6c65 5468 6963 6b6e 6573 734d  eStyleThicknessM
 00140750: 6f64 6966 6965 7229 3a0a 0a20 2022 2222  odifier):..  """
 00140760: 0a0a 2020 4368 616e 6765 206c 696e 6520  ..  Change line 
 00140770: 7468 6963 6b6e 6573 7320 616c 6f6e 6720  thickness along 
 00140780: 7374 726f 6b65 0a0a 2020 2222 220a 0a20  stroke..  """.. 
 00140790: 2062 6c65 6e64 3a20 7374 7220 3d20 2e2e   blend: str = ..
 001407a0: 2e0a 0a20 2022 2222 0a0a 2020 5370 6563  ...  """..  Spec
 001407b0: 6966 7920 686f 7720 7468 6520 6d6f 6469  ify how the modi
@@ -82113,16 +82113,16 @@
 00140c00: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 00140c10: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 00140c20: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 00140c30: 6c61 7373 204c 696e 6553 7479 6c65 5468  lass LineStyleTh
 00140c40: 6963 6b6e 6573 734d 6f64 6966 6965 725f  icknessModifier_
 00140c50: 4361 6c6c 6967 7261 7068 7928 6270 795f  Calligraphy(bpy_
 00140c60: 7374 7275 6374 2c20 4c69 6e65 5374 796c  struct, LineStyl
-00140c70: 6554 6869 636b 6e65 7373 4d6f 6469 6669  eThicknessModifi
-00140c80: 6572 2c20 4c69 6e65 5374 796c 654d 6f64  er, LineStyleMod
+00140c70: 654d 6f64 6966 6965 722c 204c 696e 6553  eModifier, LineS
+00140c80: 7479 6c65 5468 6963 6b6e 6573 734d 6f64  tyleThicknessMod
 00140c90: 6966 6965 7229 3a0a 0a20 2022 2222 0a0a  ifier):..  """..
 00140ca0: 2020 4368 616e 6765 206c 696e 6520 7468    Change line th
 00140cb0: 6963 6b6e 6573 7320 736f 2074 6861 7420  ickness so that 
 00140cc0: 7374 726f 6b65 206c 6f6f 6b73 206c 696b  stroke looks lik
 00140cd0: 6520 6d61 6465 2077 6974 6820 6120 6361  e made with a ca
 00140ce0: 6c6c 6967 7261 7068 6963 2070 656e 0a0a  lligraphic pen..
 00140cf0: 2020 2222 220a 0a20 2062 6c65 6e64 3a20    """..  blend: 
@@ -82186,17 +82186,17 @@
 00141090: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 001410a0: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 001410b0: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 001410c0: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 001410d0: 7373 204c 696e 6553 7479 6c65 5468 6963  ss LineStyleThic
 001410e0: 6b6e 6573 734d 6f64 6966 6965 725f 4372  knessModifier_Cr
 001410f0: 6561 7365 416e 676c 6528 6270 795f 7374  easeAngle(bpy_st
-00141100: 7275 6374 2c20 4c69 6e65 5374 796c 6554  ruct, LineStyleT
-00141110: 6869 636b 6e65 7373 4d6f 6469 6669 6572  hicknessModifier
-00141120: 2c20 4c69 6e65 5374 796c 654d 6f64 6966  , LineStyleModif
+00141100: 7275 6374 2c20 4c69 6e65 5374 796c 654d  ruct, LineStyleM
+00141110: 6f64 6966 6965 722c 204c 696e 6553 7479  odifier, LineSty
+00141120: 6c65 5468 6963 6b6e 6573 734d 6f64 6966  leThicknessModif
 00141130: 6965 7229 3a0a 0a20 2022 2222 0a0a 2020  ier):..  """..  
 00141140: 4c69 6e65 2074 6869 636b 6e65 7373 2062  Line thickness b
 00141150: 6173 6564 206f 6e20 7468 6520 616e 676c  ased on the angl
 00141160: 6520 6265 7477 6565 6e20 7477 6f20 6164  e between two ad
 00141170: 6a61 6365 6e74 2066 6163 6573 0a0a 2020  jacent faces..  
 00141180: 2222 220a 0a20 2061 6e67 6c65 5f6d 6178  """..  angle_max
 00141190: 3a20 666c 6f61 7420 3d20 2e2e 2e0a 0a20  : float = ..... 
@@ -82280,17 +82280,17 @@
 00141670: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 00141680: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 00141690: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 001416a0: 2e0a 0a63 6c61 7373 204c 696e 6553 7479  ...class LineSty
 001416b0: 6c65 5468 6963 6b6e 6573 734d 6f64 6966  leThicknessModif
 001416c0: 6965 725f 4375 7276 6174 7572 655f 3344  ier_Curvature_3D
 001416d0: 2862 7079 5f73 7472 7563 742c 204c 696e  (bpy_struct, Lin
-001416e0: 6553 7479 6c65 5468 6963 6b6e 6573 734d  eStyleThicknessM
-001416f0: 6f64 6966 6965 722c 204c 696e 6553 7479  odifier, LineSty
-00141700: 6c65 4d6f 6469 6669 6572 293a 0a0a 2020  leModifier):..  
+001416e0: 6553 7479 6c65 4d6f 6469 6669 6572 2c20  eStyleModifier, 
+001416f0: 4c69 6e65 5374 796c 6554 6869 636b 6e65  LineStyleThickne
+00141700: 7373 4d6f 6469 6669 6572 293a 0a0a 2020  ssModifier):..  
 00141710: 2222 220a 0a20 204c 696e 6520 7468 6963  """..  Line thic
 00141720: 6b6e 6573 7320 6261 7365 6420 6f6e 2074  kness based on t
 00141730: 6865 2072 6164 6961 6c20 6375 7276 6174  he radial curvat
 00141740: 7572 6520 6f66 2033 4420 6d65 7368 2073  ure of 3D mesh s
 00141750: 7572 6661 6365 730a 0a20 2022 2222 0a0a  urfaces..  """..
 00141760: 2020 626c 656e 643a 2073 7472 203d 202e    blend: str = .
 00141770: 2e2e 0a0a 2020 2222 220a 0a20 2053 7065  ....  """..  Spe
@@ -82372,17 +82372,17 @@
 00141c30: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 00141c40: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 00141c50: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 00141c60: 202e 2e2e 0a0a 636c 6173 7320 4c69 6e65   .....class Line
 00141c70: 5374 796c 6554 6869 636b 6e65 7373 4d6f  StyleThicknessMo
 00141c80: 6469 6669 6572 5f44 6973 7461 6e63 6546  difier_DistanceF
 00141c90: 726f 6d43 616d 6572 6128 6270 795f 7374  romCamera(bpy_st
-00141ca0: 7275 6374 2c20 4c69 6e65 5374 796c 6554  ruct, LineStyleT
-00141cb0: 6869 636b 6e65 7373 4d6f 6469 6669 6572  hicknessModifier
-00141cc0: 2c20 4c69 6e65 5374 796c 654d 6f64 6966  , LineStyleModif
+00141ca0: 7275 6374 2c20 4c69 6e65 5374 796c 654d  ruct, LineStyleM
+00141cb0: 6f64 6966 6965 722c 204c 696e 6553 7479  odifier, LineSty
+00141cc0: 6c65 5468 6963 6b6e 6573 734d 6f64 6966  leThicknessModif
 00141cd0: 6965 7229 3a0a 0a20 2022 2222 0a0a 2020  ier):..  """..  
 00141ce0: 4368 616e 6765 206c 696e 6520 7468 6963  Change line thic
 00141cf0: 6b6e 6573 7320 6261 7365 6420 6f6e 2074  kness based on t
 00141d00: 6865 2064 6973 7461 6e63 6520 6672 6f6d  he distance from
 00141d10: 2074 6865 2063 616d 6572 610a 0a20 2022   the camera..  "
 00141d20: 2222 0a0a 2020 626c 656e 643a 2073 7472  ""..  blend: str
 00141d30: 203d 202e 2e2e 0a0a 2020 2222 220a 0a20   = .....  """.. 
@@ -82470,17 +82470,17 @@
 00142250: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 00142260: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 00142270: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 00142280: 202e 2e2e 0a0a 636c 6173 7320 4c69 6e65   .....class Line
 00142290: 5374 796c 6554 6869 636b 6e65 7373 4d6f  StyleThicknessMo
 001422a0: 6469 6669 6572 5f44 6973 7461 6e63 6546  difier_DistanceF
 001422b0: 726f 6d4f 626a 6563 7428 6270 795f 7374  romObject(bpy_st
-001422c0: 7275 6374 2c20 4c69 6e65 5374 796c 6554  ruct, LineStyleT
-001422d0: 6869 636b 6e65 7373 4d6f 6469 6669 6572  hicknessModifier
-001422e0: 2c20 4c69 6e65 5374 796c 654d 6f64 6966  , LineStyleModif
+001422c0: 7275 6374 2c20 4c69 6e65 5374 796c 654d  ruct, LineStyleM
+001422d0: 6f64 6966 6965 722c 204c 696e 6553 7479  odifier, LineSty
+001422e0: 6c65 5468 6963 6b6e 6573 734d 6f64 6966  leThicknessModif
 001422f0: 6965 7229 3a0a 0a20 2022 2222 0a0a 2020  ier):..  """..  
 00142300: 4368 616e 6765 206c 696e 6520 7468 6963  Change line thic
 00142310: 6b6e 6573 7320 6261 7365 6420 6f6e 2074  kness based on t
 00142320: 6865 2064 6973 7461 6e63 6520 6672 6f6d  he distance from
 00142330: 2061 6e20 6f62 6a65 6374 0a0a 2020 2222   an object..  ""
 00142340: 220a 0a20 2062 6c65 6e64 3a20 7374 7220  "..  blend: str 
 00142350: 3d20 2e2e 2e0a 0a20 2022 2222 0a0a 2020  = .....  """..  
@@ -82573,17 +82573,17 @@
 001428c0: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 001428d0: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 001428e0: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 001428f0: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 00142900: 636c 6173 7320 4c69 6e65 5374 796c 6554  class LineStyleT
 00142910: 6869 636b 6e65 7373 4d6f 6469 6669 6572  hicknessModifier
 00142920: 5f4d 6174 6572 6961 6c28 6270 795f 7374  _Material(bpy_st
-00142930: 7275 6374 2c20 4c69 6e65 5374 796c 6554  ruct, LineStyleT
-00142940: 6869 636b 6e65 7373 4d6f 6469 6669 6572  hicknessModifier
-00142950: 2c20 4c69 6e65 5374 796c 654d 6f64 6966  , LineStyleModif
+00142930: 7275 6374 2c20 4c69 6e65 5374 796c 654d  ruct, LineStyleM
+00142940: 6f64 6966 6965 722c 204c 696e 6553 7479  odifier, LineSty
+00142950: 6c65 5468 6963 6b6e 6573 734d 6f64 6966  leThicknessModif
 00142960: 6965 7229 3a0a 0a20 2022 2222 0a0a 2020  ier):..  """..  
 00142970: 4368 616e 6765 206c 696e 6520 7468 6963  Change line thic
 00142980: 6b6e 6573 7320 6261 7365 6420 6f6e 2061  kness based on a
 00142990: 206d 6174 6572 6961 6c20 6174 7472 6962   material attrib
 001429a0: 7574 650a 0a20 2022 2222 0a0a 2020 626c  ute..  """..  bl
 001429b0: 656e 643a 2073 7472 203d 202e 2e2e 0a0a  end: str = .....
 001429c0: 2020 2222 220a 0a20 2053 7065 6369 6679    """..  Specify
@@ -82664,16 +82664,16 @@
 00142e70: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 00142e80: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 00142e90: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 00142ea0: 2020 2e2e 2e0a 0a63 6c61 7373 204c 696e    .....class Lin
 00142eb0: 6553 7479 6c65 5468 6963 6b6e 6573 734d  eStyleThicknessM
 00142ec0: 6f64 6966 6965 725f 4e6f 6973 6528 6270  odifier_Noise(bp
 00142ed0: 795f 7374 7275 6374 2c20 4c69 6e65 5374  y_struct, LineSt
-00142ee0: 796c 6554 6869 636b 6e65 7373 4d6f 6469  yleThicknessModi
-00142ef0: 6669 6572 2c20 4c69 6e65 5374 796c 654d  fier, LineStyleM
+00142ee0: 796c 654d 6f64 6966 6965 722c 204c 696e  yleModifier, Lin
+00142ef0: 6553 7479 6c65 5468 6963 6b6e 6573 734d  eStyleThicknessM
 00142f00: 6f64 6966 6965 7229 3a0a 0a20 2022 2222  odifier):..  """
 00142f10: 0a0a 2020 4c69 6e65 2074 6869 636b 6e65  ..  Line thickne
 00142f20: 7373 2062 6173 6564 206f 6e20 7261 6e64  ss based on rand
 00142f30: 6f6d 206e 6f69 7365 0a0a 2020 2222 220a  om noise..  """.
 00142f40: 0a20 2061 6d70 6c69 7475 6465 3a20 666c  .  amplitude: fl
 00142f50: 6f61 7420 3d20 2e2e 2e0a 0a20 2022 2222  oat = .....  """
 00142f60: 0a0a 2020 416d 706c 6974 7564 6520 6f66  ..  Amplitude of
@@ -82735,17 +82735,17 @@
 001432e0: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 001432f0: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 00143300: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 00143310: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 00143320: 6173 7320 4c69 6e65 5374 796c 6554 6869  ass LineStyleThi
 00143330: 636b 6e65 7373 4d6f 6469 6669 6572 5f54  cknessModifier_T
 00143340: 616e 6765 6e74 2862 7079 5f73 7472 7563  angent(bpy_struc
-00143350: 742c 204c 696e 6553 7479 6c65 5468 6963  t, LineStyleThic
-00143360: 6b6e 6573 734d 6f64 6966 6965 722c 204c  knessModifier, L
-00143370: 696e 6553 7479 6c65 4d6f 6469 6669 6572  ineStyleModifier
+00143350: 742c 204c 696e 6553 7479 6c65 4d6f 6469  t, LineStyleModi
+00143360: 6669 6572 2c20 4c69 6e65 5374 796c 6554  fier, LineStyleT
+00143370: 6869 636b 6e65 7373 4d6f 6469 6669 6572  hicknessModifier
 00143380: 293a 0a0a 2020 2222 220a 0a20 2054 6869  ):..  """..  Thi
 00143390: 636b 6e65 7373 2062 6173 6564 206f 6e20  ckness based on 
 001433a0: 7468 6520 6469 7265 6374 696f 6e20 6f66  the direction of
 001433b0: 2074 6865 2073 7472 6f6b 650a 0a20 2022   the stroke..  "
 001433c0: 2222 0a0a 2020 626c 656e 643a 2073 7472  ""..  blend: str
 001433d0: 203d 202e 2e2e 0a0a 2020 2222 220a 0a20   = .....  """.. 
 001433e0: 2053 7065 6369 6679 2068 6f77 2074 6865   Specify how the
@@ -82872,16 +82872,16 @@
 00143b70: 6566 2062 6c5f 726e 615f 6765 745f 7375  ef bl_rna_get_su
 00143b80: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 00143b90: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 00143ba0: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 00143bb0: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 00143bc0: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 00143bd0: 6173 7320 4e6f 6465 4672 616d 6528 6270  ass NodeFrame(bp
-00143be0: 795f 7374 7275 6374 2c20 4e6f 6465 2c20  y_struct, Node, 
-00143bf0: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+00143be0: 795f 7374 7275 6374 2c20 4e6f 6465 496e  y_struct, NodeIn
+00143bf0: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 00143c00: 2020 2222 220a 0a20 2043 6f6c 6c65 6374    """..  Collect
 00143c10: 2072 656c 6174 6564 206e 6f64 6573 2074   related nodes t
 00143c20: 6f67 6574 6865 7220 696e 2061 2063 6f6d  ogether in a com
 00143c30: 6d6f 6e20 6172 6561 2e20 5573 6566 756c  mon area. Useful
 00143c40: 2066 6f72 206f 7267 616e 697a 6174 696f   for organizatio
 00143c50: 6e20 7768 656e 2074 6865 2072 652d 7573  n when the re-us
 00143c60: 6162 696c 6974 7920 6f66 2061 206e 6f64  ability of a nod
@@ -82935,16 +82935,16 @@
 00143f60: 726e 615f 6765 745f 7375 6263 6c61 7373  rna_get_subclass
 00143f70: 5f70 7928 636c 732c 2069 643a 2073 7472  _py(cls, id: str
 00143f80: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 00143f90: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 00143fa0: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 00143fb0: 2020 202e 2e2e 0a0a 636c 6173 7320 4e6f     .....class No
 00143fc0: 6465 4772 6f75 7028 6270 795f 7374 7275  deGroup(bpy_stru
-00143fd0: 6374 2c20 4e6f 6465 2c20 4e6f 6465 496e  ct, Node, NodeIn
-00143fe0: 7465 726e 616c 293a 0a0a 2020 6e6f 6465  ternal):..  node
+00143fd0: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+00143fe0: 2c20 4e6f 6465 293a 0a0a 2020 6e6f 6465  , Node):..  node
 00143ff0: 5f74 7265 653a 204e 6f64 6554 7265 6520  _tree: NodeTree 
 00144000: 3d20 2e2e 2e0a 0a20 2040 636c 6173 736d  = .....  @classm
 00144010: 6574 686f 640a 0a20 2064 6566 2069 735f  ethod..  def is_
 00144020: 7265 6769 7374 6572 6564 5f6e 6f64 655f  registered_node_
 00144030: 7479 7065 2863 6c73 2920 2d3e 2062 6f6f  type(cls) -> boo
 00144040: 6c3a 0a0a 2020 2020 2222 220a 0a20 2020  l:..    """..   
 00144050: 2054 7275 6520 6966 2061 2072 6567 6973   True if a regis
@@ -82979,16 +82979,16 @@
 00144220: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 00144230: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 00144240: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 00144250: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 00144260: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 00144270: 2020 2e2e 2e0a 0a63 6c61 7373 204e 6f64    .....class Nod
 00144280: 6547 726f 7570 496e 7075 7428 6270 795f  eGroupInput(bpy_
-00144290: 7374 7275 6374 2c20 4e6f 6465 2c20 4e6f  struct, Node, No
-001442a0: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+00144290: 7374 7275 6374 2c20 4e6f 6465 496e 7465  struct, NodeInte
+001442a0: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 001442b0: 2222 220a 0a20 2045 7870 6f73 6520 636f  """..  Expose co
 001442c0: 6e6e 6563 7465 6420 6461 7461 2066 726f  nnected data fro
 001442d0: 6d20 696e 7369 6465 2061 206e 6f64 6520  m inside a node 
 001442e0: 6772 6f75 7020 6173 2069 6e70 7574 7320  group as inputs 
 001442f0: 746f 2069 7473 2069 6e74 6572 6661 6365  to its interface
 00144300: 0a0a 2020 2222 220a 0a20 2040 636c 6173  ..  """..  @clas
 00144310: 736d 6574 686f 640a 0a20 2064 6566 2069  smethod..  def i
@@ -83027,16 +83027,16 @@
 00144520: 5f72 6e61 5f67 6574 5f73 7562 636c 6173  _rna_get_subclas
 00144530: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 00144540: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 00144550: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 00144560: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 00144570: 2020 2020 2e2e 2e0a 0a63 6c61 7373 204e      .....class N
 00144580: 6f64 6547 726f 7570 4f75 7470 7574 2862  odeGroupOutput(b
-00144590: 7079 5f73 7472 7563 742c 204e 6f64 652c  py_struct, Node,
-001445a0: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+00144590: 7079 5f73 7472 7563 742c 204e 6f64 6549  py_struct, NodeI
+001445a0: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 001445b0: 0a20 2022 2222 0a0a 2020 4f75 7470 7574  .  """..  Output
 001445c0: 2064 6174 6120 6672 6f6d 2069 6e73 6964   data from insid
 001445d0: 6520 6f66 2061 206e 6f64 6520 6772 6f75  e of a node grou
 001445e0: 700a 0a20 2022 2222 0a0a 2020 6973 5f61  p..  """..  is_a
 001445f0: 6374 6976 655f 6f75 7470 7574 3a20 626f  ctive_output: bo
 00144600: 6f6c 203d 202e 2e2e 0a0a 2020 2222 220a  ol = .....  """.
 00144610: 0a20 2054 7275 6520 6966 2074 6869 7320  .  True if this 
@@ -83080,15 +83080,15 @@
 00144870: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 00144880: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 00144890: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 001448a0: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 001448b0: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 001448c0: 636c 6173 7320 4e6f 6465 5265 726f 7574  class NodeRerout
 001448d0: 6528 6270 795f 7374 7275 6374 2c20 4e6f  e(bpy_struct, No
-001448e0: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+001448e0: 6465 496e 7465 726e 616c 2c20 4e6f 6465  deInternal, Node
 001448f0: 293a 0a0a 2020 2222 220a 0a20 2041 2073  ):..  """..  A s
 00144900: 696e 676c 652d 736f 636b 6574 206f 7267  ingle-socket org
 00144910: 616e 697a 6174 696f 6e20 746f 6f6c 2074  anization tool t
 00144920: 6861 7420 7375 7070 6f72 7473 206f 6e65  hat supports one
 00144930: 2069 6e70 7574 2061 6e64 206d 756c 7469   input and multi
 00144940: 706c 6520 6f75 7470 7574 730a 0a20 2022  ple outputs..  "
 00144950: 2222 0a0a 2020 4063 6c61 7373 6d65 7468  ""..  @classmeth
@@ -83161,17 +83161,17 @@
 00144d80: 2020 6465 6620 626c 5f72 6e61 5f67 6574    def bl_rna_get
 00144d90: 5f73 7562 636c 6173 735f 7079 2863 6c73  _subclass_py(cls
 00144da0: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 00144db0: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 00144dc0: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 00144dd0: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 00144de0: 0a63 6c61 7373 204e 6f64 6553 6f63 6b65  .class NodeSocke
-00144df0: 7442 6f6f 6c28 6270 795f 7374 7275 6374  tBool(bpy_struct
-00144e00: 2c20 4e6f 6465 536f 636b 6574 5374 616e  , NodeSocketStan
-00144e10: 6461 7264 2c20 4e6f 6465 536f 636b 6574  dard, NodeSocket
+00144df0: 7442 6f6f 6c28 4e6f 6465 536f 636b 6574  tBool(NodeSocket
+00144e00: 5374 616e 6461 7264 2c20 6270 795f 7374  Standard, bpy_st
+00144e10: 7275 6374 2c20 4e6f 6465 536f 636b 6574  ruct, NodeSocket
 00144e20: 293a 0a0a 2020 2222 220a 0a20 2042 6f6f  ):..  """..  Boo
 00144e30: 6c65 616e 2076 616c 7565 2073 6f63 6b65  lean value socke
 00144e40: 7420 6f66 2061 206e 6f64 650a 0a20 2022  t of a node..  "
 00144e50: 2222 0a0a 2020 6465 6661 756c 745f 7661  ""..  default_va
 00144e60: 6c75 653a 2062 6f6f 6c20 3d20 2e2e 2e0a  lue: bool = ....
 00144e70: 0a20 2022 2222 0a0a 2020 496e 7075 7420  .  """..  Input 
 00144e80: 7661 6c75 6520 7573 6564 2066 6f72 2075  value used for u
@@ -83197,17 +83197,17 @@
 00144fc0: 5f72 6e61 5f67 6574 5f73 7562 636c 6173  _rna_get_subclas
 00144fd0: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 00144fe0: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 00144ff0: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 00145000: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 00145010: 2020 2020 2e2e 2e0a 0a63 6c61 7373 204e      .....class N
 00145020: 6f64 6553 6f63 6b65 7443 6f6c 6c65 6374  odeSocketCollect
-00145030: 696f 6e28 6270 795f 7374 7275 6374 2c20  ion(bpy_struct, 
-00145040: 4e6f 6465 536f 636b 6574 5374 616e 6461  NodeSocketStanda
-00145050: 7264 2c20 4e6f 6465 536f 636b 6574 293a  rd, NodeSocket):
+00145030: 696f 6e28 4e6f 6465 536f 636b 6574 5374  ion(NodeSocketSt
+00145040: 616e 6461 7264 2c20 6270 795f 7374 7275  andard, bpy_stru
+00145050: 6374 2c20 4e6f 6465 536f 636b 6574 293a  ct, NodeSocket):
 00145060: 0a0a 2020 2222 220a 0a20 2043 6f6c 6c65  ..  """..  Colle
 00145070: 6374 696f 6e20 736f 636b 6574 206f 6620  ction socket of 
 00145080: 6120 6e6f 6465 0a0a 2020 2222 220a 0a20  a node..  """.. 
 00145090: 2064 6566 6175 6c74 5f76 616c 7565 3a20   default_value: 
 001450a0: 436f 6c6c 6563 7469 6f6e 203d 202e 2e2e  Collection = ...
 001450b0: 0a0a 2020 2222 220a 0a20 2049 6e70 7574  ..  """..  Input
 001450c0: 2076 616c 7565 2075 7365 6420 666f 7220   value used for 
@@ -83233,16 +83233,16 @@
 00145200: 6c5f 726e 615f 6765 745f 7375 6263 6c61  l_rna_get_subcla
 00145210: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 00145220: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 00145230: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 00145240: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 00145250: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 00145260: 4e6f 6465 536f 636b 6574 436f 6c6f 7228  NodeSocketColor(
-00145270: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
-00145280: 536f 636b 6574 5374 616e 6461 7264 2c20  SocketStandard, 
+00145270: 4e6f 6465 536f 636b 6574 5374 616e 6461  NodeSocketStanda
+00145280: 7264 2c20 6270 795f 7374 7275 6374 2c20  rd, bpy_struct, 
 00145290: 4e6f 6465 536f 636b 6574 293a 0a0a 2020  NodeSocket):..  
 001452a0: 2222 220a 0a20 2052 4742 4120 636f 6c6f  """..  RGBA colo
 001452b0: 7220 736f 636b 6574 206f 6620 6120 6e6f  r socket of a no
 001452c0: 6465 0a0a 2020 2222 220a 0a20 2064 6566  de..  """..  def
 001452d0: 6175 6c74 5f76 616c 7565 3a20 7479 7069  ault_value: typi
 001452e0: 6e67 2e54 7570 6c65 5b66 6c6f 6174 2c20  ng.Tuple[float, 
 001452f0: 666c 6f61 742c 2066 6c6f 6174 2c20 666c  float, float, fl
@@ -83270,17 +83270,17 @@
 00145450: 640a 0a20 2064 6566 2062 6c5f 726e 615f  d..  def bl_rna_
 00145460: 6765 745f 7375 6263 6c61 7373 5f70 7928  get_subclass_py(
 00145470: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 00145480: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 00145490: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 001454a0: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 001454b0: 2e2e 0a0a 636c 6173 7320 4e6f 6465 536f  ....class NodeSo
-001454c0: 636b 6574 466c 6f61 7428 6270 795f 7374  cketFloat(bpy_st
-001454d0: 7275 6374 2c20 4e6f 6465 536f 636b 6574  ruct, NodeSocket
-001454e0: 5374 616e 6461 7264 2c20 4e6f 6465 536f  Standard, NodeSo
+001454c0: 636b 6574 466c 6f61 7428 4e6f 6465 536f  cketFloat(NodeSo
+001454d0: 636b 6574 5374 616e 6461 7264 2c20 6270  cketStandard, bp
+001454e0: 795f 7374 7275 6374 2c20 4e6f 6465 536f  y_struct, NodeSo
 001454f0: 636b 6574 293a 0a0a 2020 2222 220a 0a20  cket):..  """.. 
 00145500: 2046 6c6f 6174 696e 672d 706f 696e 7420   Floating-point 
 00145510: 6e75 6d62 6572 2073 6f63 6b65 7420 6f66  number socket of
 00145520: 2061 206e 6f64 650a 0a20 2022 2222 0a0a   a node..  """..
 00145530: 2020 6465 6661 756c 745f 7661 6c75 653a    default_value:
 00145540: 2066 6c6f 6174 203d 202e 2e2e 0a0a 2020   float = .....  
 00145550: 2222 220a 0a20 2049 6e70 7574 2076 616c  """..  Input val
@@ -83307,16 +83307,16 @@
 001456a0: 615f 6765 745f 7375 6263 6c61 7373 5f70  a_get_subclass_p
 001456b0: 7928 636c 732c 2069 643a 2073 7472 2c20  y(cls, id: str, 
 001456c0: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 001456d0: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 001456e0: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 001456f0: 202e 2e2e 0a0a 636c 6173 7320 4e6f 6465   .....class Node
 00145700: 536f 636b 6574 466c 6f61 7441 6e67 6c65  SocketFloatAngle
-00145710: 2862 7079 5f73 7472 7563 742c 204e 6f64  (bpy_struct, Nod
-00145720: 6553 6f63 6b65 7453 7461 6e64 6172 642c  eSocketStandard,
+00145710: 284e 6f64 6553 6f63 6b65 7453 7461 6e64  (NodeSocketStand
+00145720: 6172 642c 2062 7079 5f73 7472 7563 742c  ard, bpy_struct,
 00145730: 204e 6f64 6553 6f63 6b65 7429 3a0a 0a20   NodeSocket):.. 
 00145740: 2022 2222 0a0a 2020 466c 6f61 7469 6e67   """..  Floating
 00145750: 2d70 6f69 6e74 206e 756d 6265 7220 736f  -point number so
 00145760: 636b 6574 206f 6620 6120 6e6f 6465 0a0a  cket of a node..
 00145770: 2020 2222 220a 0a20 2064 6566 6175 6c74    """..  default
 00145780: 5f76 616c 7565 3a20 666c 6f61 7420 3d20  _value: float = 
 00145790: 2e2e 2e0a 0a20 2022 2222 0a0a 2020 496e  .....  """..  In
@@ -83343,17 +83343,17 @@
 001458e0: 6620 626c 5f72 6e61 5f67 6574 5f73 7562  f bl_rna_get_sub
 001458f0: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 00145900: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 00145910: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 00145920: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 00145930: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 00145940: 7373 204e 6f64 6553 6f63 6b65 7446 6c6f  ss NodeSocketFlo
-00145950: 6174 4469 7374 616e 6365 2862 7079 5f73  atDistance(bpy_s
-00145960: 7472 7563 742c 204e 6f64 6553 6f63 6b65  truct, NodeSocke
-00145970: 7453 7461 6e64 6172 642c 204e 6f64 6553  tStandard, NodeS
+00145950: 6174 4469 7374 616e 6365 284e 6f64 6553  atDistance(NodeS
+00145960: 6f63 6b65 7453 7461 6e64 6172 642c 2062  ocketStandard, b
+00145970: 7079 5f73 7472 7563 742c 204e 6f64 6553  py_struct, NodeS
 00145980: 6f63 6b65 7429 3a0a 0a20 2022 2222 0a0a  ocket):..  """..
 00145990: 2020 466c 6f61 7469 6e67 2d70 6f69 6e74    Floating-point
 001459a0: 206e 756d 6265 7220 736f 636b 6574 206f   number socket o
 001459b0: 6620 6120 6e6f 6465 0a0a 2020 2222 220a  f a node..  """.
 001459c0: 0a20 2064 6566 6175 6c74 5f76 616c 7565  .  default_value
 001459d0: 3a20 666c 6f61 7420 3d20 2e2e 2e0a 0a20  : float = ..... 
 001459e0: 2022 2222 0a0a 2020 496e 7075 7420 7661   """..  Input va
@@ -83380,17 +83380,17 @@
 00145b30: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 00145b40: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 00145b50: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 00145b60: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 00145b70: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 00145b80: 2020 2e2e 2e0a 0a63 6c61 7373 204e 6f64    .....class Nod
 00145b90: 6553 6f63 6b65 7446 6c6f 6174 4661 6374  eSocketFloatFact
-00145ba0: 6f72 2862 7079 5f73 7472 7563 742c 204e  or(bpy_struct, N
-00145bb0: 6f64 6553 6f63 6b65 7453 7461 6e64 6172  odeSocketStandar
-00145bc0: 642c 204e 6f64 6553 6f63 6b65 7429 3a0a  d, NodeSocket):.
+00145ba0: 6f72 284e 6f64 6553 6f63 6b65 7453 7461  or(NodeSocketSta
+00145bb0: 6e64 6172 642c 2062 7079 5f73 7472 7563  ndard, bpy_struc
+00145bc0: 742c 204e 6f64 6553 6f63 6b65 7429 3a0a  t, NodeSocket):.
 00145bd0: 0a20 2022 2222 0a0a 2020 466c 6f61 7469  .  """..  Floati
 00145be0: 6e67 2d70 6f69 6e74 206e 756d 6265 7220  ng-point number 
 00145bf0: 736f 636b 6574 206f 6620 6120 6e6f 6465  socket of a node
 00145c00: 0a0a 2020 2222 220a 0a20 2064 6566 6175  ..  """..  defau
 00145c10: 6c74 5f76 616c 7565 3a20 666c 6f61 7420  lt_value: float 
 00145c20: 3d20 2e2e 2e0a 0a20 2022 2222 0a0a 2020  = .....  """..  
 00145c30: 496e 7075 7420 7661 6c75 6520 7573 6564  Input value used
@@ -83416,17 +83416,17 @@
 00145d70: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 00145d80: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 00145d90: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 00145da0: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 00145db0: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 00145dc0: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 00145dd0: 6c61 7373 204e 6f64 6553 6f63 6b65 7446  lass NodeSocketF
-00145de0: 6c6f 6174 5065 7263 656e 7461 6765 2862  loatPercentage(b
-00145df0: 7079 5f73 7472 7563 742c 204e 6f64 6553  py_struct, NodeS
-00145e00: 6f63 6b65 7453 7461 6e64 6172 642c 204e  ocketStandard, N
+00145de0: 6c6f 6174 5065 7263 656e 7461 6765 284e  loatPercentage(N
+00145df0: 6f64 6553 6f63 6b65 7453 7461 6e64 6172  odeSocketStandar
+00145e00: 642c 2062 7079 5f73 7472 7563 742c 204e  d, bpy_struct, N
 00145e10: 6f64 6553 6f63 6b65 7429 3a0a 0a20 2022  odeSocket):..  "
 00145e20: 2222 0a0a 2020 466c 6f61 7469 6e67 2d70  ""..  Floating-p
 00145e30: 6f69 6e74 206e 756d 6265 7220 736f 636b  oint number sock
 00145e40: 6574 206f 6620 6120 6e6f 6465 0a0a 2020  et of a node..  
 00145e50: 2222 220a 0a20 2064 6566 6175 6c74 5f76  """..  default_v
 00145e60: 616c 7565 3a20 666c 6f61 7420 3d20 2e2e  alue: float = ..
 00145e70: 2e0a 0a20 2022 2222 0a0a 2020 496e 7075  ...  """..  Inpu
@@ -83453,17 +83453,17 @@
 00145fc0: 626c 5f72 6e61 5f67 6574 5f73 7562 636c  bl_rna_get_subcl
 00145fd0: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 00145fe0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 00145ff0: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 00146000: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 00146010: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 00146020: 204e 6f64 6553 6f63 6b65 7446 6c6f 6174   NodeSocketFloat
-00146030: 5469 6d65 2862 7079 5f73 7472 7563 742c  Time(bpy_struct,
-00146040: 204e 6f64 6553 6f63 6b65 7453 7461 6e64   NodeSocketStand
-00146050: 6172 642c 204e 6f64 6553 6f63 6b65 7429  ard, NodeSocket)
+00146030: 5469 6d65 284e 6f64 6553 6f63 6b65 7453  Time(NodeSocketS
+00146040: 7461 6e64 6172 642c 2062 7079 5f73 7472  tandard, bpy_str
+00146050: 7563 742c 204e 6f64 6553 6f63 6b65 7429  uct, NodeSocket)
 00146060: 3a0a 0a20 2022 2222 0a0a 2020 466c 6f61  :..  """..  Floa
 00146070: 7469 6e67 2d70 6f69 6e74 206e 756d 6265  ting-point numbe
 00146080: 7220 736f 636b 6574 206f 6620 6120 6e6f  r socket of a no
 00146090: 6465 0a0a 2020 2222 220a 0a20 2064 6566  de..  """..  def
 001460a0: 6175 6c74 5f76 616c 7565 3a20 666c 6f61  ault_value: floa
 001460b0: 7420 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  t = .....  """..
 001460c0: 2020 496e 7075 7420 7661 6c75 6520 7573    Input value us
@@ -83490,17 +83490,17 @@
 00146210: 5f73 7562 636c 6173 735f 7079 2863 6c73  _subclass_py(cls
 00146220: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 00146230: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 00146240: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 00146250: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 00146260: 0a63 6c61 7373 204e 6f64 6553 6f63 6b65  .class NodeSocke
 00146270: 7446 6c6f 6174 5469 6d65 4162 736f 6c75  tFloatTimeAbsolu
-00146280: 7465 2862 7079 5f73 7472 7563 742c 204e  te(bpy_struct, N
-00146290: 6f64 6553 6f63 6b65 7453 7461 6e64 6172  odeSocketStandar
-001462a0: 642c 204e 6f64 6553 6f63 6b65 7429 3a0a  d, NodeSocket):.
+00146280: 7465 284e 6f64 6553 6f63 6b65 7453 7461  te(NodeSocketSta
+00146290: 6e64 6172 642c 2062 7079 5f73 7472 7563  ndard, bpy_struc
+001462a0: 742c 204e 6f64 6553 6f63 6b65 7429 3a0a  t, NodeSocket):.
 001462b0: 0a20 2022 2222 0a0a 2020 466c 6f61 7469  .  """..  Floati
 001462c0: 6e67 2d70 6f69 6e74 206e 756d 6265 7220  ng-point number 
 001462d0: 736f 636b 6574 206f 6620 6120 6e6f 6465  socket of a node
 001462e0: 0a0a 2020 2222 220a 0a20 2064 6566 6175  ..  """..  defau
 001462f0: 6c74 5f76 616c 7565 3a20 666c 6f61 7420  lt_value: float 
 00146300: 3d20 2e2e 2e0a 0a20 2022 2222 0a0a 2020  = .....  """..  
 00146310: 496e 7075 7420 7661 6c75 6520 7573 6564  Input value used
@@ -83526,17 +83526,17 @@
 00146450: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 00146460: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 00146470: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 00146480: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 00146490: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 001464a0: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 001464b0: 6c61 7373 204e 6f64 6553 6f63 6b65 7446  lass NodeSocketF
-001464c0: 6c6f 6174 556e 7369 676e 6564 2862 7079  loatUnsigned(bpy
-001464d0: 5f73 7472 7563 742c 204e 6f64 6553 6f63  _struct, NodeSoc
-001464e0: 6b65 7453 7461 6e64 6172 642c 204e 6f64  ketStandard, Nod
+001464c0: 6c6f 6174 556e 7369 676e 6564 284e 6f64  loatUnsigned(Nod
+001464d0: 6553 6f63 6b65 7453 7461 6e64 6172 642c  eSocketStandard,
+001464e0: 2062 7079 5f73 7472 7563 742c 204e 6f64   bpy_struct, Nod
 001464f0: 6553 6f63 6b65 7429 3a0a 0a20 2022 2222  eSocket):..  """
 00146500: 0a0a 2020 466c 6f61 7469 6e67 2d70 6f69  ..  Floating-poi
 00146510: 6e74 206e 756d 6265 7220 736f 636b 6574  nt number socket
 00146520: 206f 6620 6120 6e6f 6465 0a0a 2020 2222   of a node..  ""
 00146530: 220a 0a20 2064 6566 6175 6c74 5f76 616c  "..  default_val
 00146540: 7565 3a20 666c 6f61 7420 3d20 2e2e 2e0a  ue: float = ....
 00146550: 0a20 2022 2222 0a0a 2020 496e 7075 7420  .  """..  Input 
@@ -83563,16 +83563,16 @@
 001466a0: 5f72 6e61 5f67 6574 5f73 7562 636c 6173  _rna_get_subclas
 001466b0: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 001466c0: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 001466d0: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 001466e0: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 001466f0: 2020 2020 2e2e 2e0a 0a63 6c61 7373 204e      .....class N
 00146700: 6f64 6553 6f63 6b65 7447 656f 6d65 7472  odeSocketGeometr
-00146710: 7928 6270 795f 7374 7275 6374 2c20 4e6f  y(bpy_struct, No
-00146720: 6465 536f 636b 6574 5374 616e 6461 7264  deSocketStandard
+00146710: 7928 4e6f 6465 536f 636b 6574 5374 616e  y(NodeSocketStan
+00146720: 6461 7264 2c20 6270 795f 7374 7275 6374  dard, bpy_struct
 00146730: 2c20 4e6f 6465 536f 636b 6574 293a 0a0a  , NodeSocket):..
 00146740: 2020 2222 220a 0a20 2047 656f 6d65 7472    """..  Geometr
 00146750: 7920 736f 636b 6574 206f 6620 6120 6e6f  y socket of a no
 00146760: 6465 0a0a 2020 2222 220a 0a20 206c 696e  de..  """..  lin
 00146770: 6b73 3a20 7479 7069 6e67 2e41 6e79 203d  ks: typing.Any =
 00146780: 202e 2e2e 0a0a 2020 2222 220a 0a20 204c   .....  """..  L
 00146790: 6973 7420 6f66 206e 6f64 6520 6c69 6e6b  ist of node link
@@ -83593,16 +83593,16 @@
 00146880: 6c5f 726e 615f 6765 745f 7375 6263 6c61  l_rna_get_subcla
 00146890: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 001468a0: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 001468b0: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 001468c0: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 001468d0: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 001468e0: 4e6f 6465 536f 636b 6574 496d 6167 6528  NodeSocketImage(
-001468f0: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
-00146900: 536f 636b 6574 5374 616e 6461 7264 2c20  SocketStandard, 
+001468f0: 4e6f 6465 536f 636b 6574 5374 616e 6461  NodeSocketStanda
+00146900: 7264 2c20 6270 795f 7374 7275 6374 2c20  rd, bpy_struct, 
 00146910: 4e6f 6465 536f 636b 6574 293a 0a0a 2020  NodeSocket):..  
 00146920: 2222 220a 0a20 2049 6d61 6765 2073 6f63  """..  Image soc
 00146930: 6b65 7420 6f66 2061 206e 6f64 650a 0a20  ket of a node.. 
 00146940: 2022 2222 0a0a 2020 6465 6661 756c 745f   """..  default_
 00146950: 7661 6c75 653a 2049 6d61 6765 203d 202e  value: Image = .
 00146960: 2e2e 0a0a 2020 2222 220a 0a20 2049 6e70  ....  """..  Inp
 00146970: 7574 2076 616c 7565 2075 7365 6420 666f  ut value used fo
@@ -83628,16 +83628,16 @@
 00146ab0: 2062 6c5f 726e 615f 6765 745f 7375 6263   bl_rna_get_subc
 00146ac0: 6c61 7373 5f70 7928 636c 732c 2069 643a  lass_py(cls, id:
 00146ad0: 2073 7472 2c20 6465 6661 756c 743a 2074   str, default: t
 00146ae0: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 00146af0: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 00146b00: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 00146b10: 7320 4e6f 6465 536f 636b 6574 496e 7428  s NodeSocketInt(
-00146b20: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
-00146b30: 536f 636b 6574 5374 616e 6461 7264 2c20  SocketStandard, 
+00146b20: 4e6f 6465 536f 636b 6574 5374 616e 6461  NodeSocketStanda
+00146b30: 7264 2c20 6270 795f 7374 7275 6374 2c20  rd, bpy_struct, 
 00146b40: 4e6f 6465 536f 636b 6574 293a 0a0a 2020  NodeSocket):..  
 00146b50: 2222 220a 0a20 2049 6e74 6567 6572 206e  """..  Integer n
 00146b60: 756d 6265 7220 736f 636b 6574 206f 6620  umber socket of 
 00146b70: 6120 6e6f 6465 0a0a 2020 2222 220a 0a20  a node..  """.. 
 00146b80: 2064 6566 6175 6c74 5f76 616c 7565 3a20   default_value: 
 00146b90: 696e 7420 3d20 2e2e 2e0a 0a20 2022 2222  int = .....  """
 00146ba0: 0a0a 2020 496e 7075 7420 7661 6c75 6520  ..  Input value 
@@ -83663,17 +83663,17 @@
 00146ce0: 0a0a 2020 6465 6620 626c 5f72 6e61 5f67  ..  def bl_rna_g
 00146cf0: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 00146d00: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 00146d10: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 00146d20: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 00146d30: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 00146d40: 2e0a 0a63 6c61 7373 204e 6f64 6553 6f63  ...class NodeSoc
-00146d50: 6b65 7449 6e74 4661 6374 6f72 2862 7079  ketIntFactor(bpy
-00146d60: 5f73 7472 7563 742c 204e 6f64 6553 6f63  _struct, NodeSoc
-00146d70: 6b65 7453 7461 6e64 6172 642c 204e 6f64  ketStandard, Nod
+00146d50: 6b65 7449 6e74 4661 6374 6f72 284e 6f64  ketIntFactor(Nod
+00146d60: 6553 6f63 6b65 7453 7461 6e64 6172 642c  eSocketStandard,
+00146d70: 2062 7079 5f73 7472 7563 742c 204e 6f64   bpy_struct, Nod
 00146d80: 6553 6f63 6b65 7429 3a0a 0a20 2022 2222  eSocket):..  """
 00146d90: 0a0a 2020 496e 7465 6765 7220 6e75 6d62  ..  Integer numb
 00146da0: 6572 2073 6f63 6b65 7420 6f66 2061 206e  er socket of a n
 00146db0: 6f64 650a 0a20 2022 2222 0a0a 2020 6465  ode..  """..  de
 00146dc0: 6661 756c 745f 7661 6c75 653a 2069 6e74  fault_value: int
 00146dd0: 203d 202e 2e2e 0a0a 2020 2222 220a 0a20   = .....  """.. 
 00146de0: 2049 6e70 7574 2076 616c 7565 2075 7365   Input value use
@@ -83699,17 +83699,17 @@
 00146f20: 2064 6566 2062 6c5f 726e 615f 6765 745f   def bl_rna_get_
 00146f30: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 00146f40: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 00146f50: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 00146f60: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 00146f70: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 00146f80: 636c 6173 7320 4e6f 6465 536f 636b 6574  class NodeSocket
-00146f90: 496e 7450 6572 6365 6e74 6167 6528 6270  IntPercentage(bp
-00146fa0: 795f 7374 7275 6374 2c20 4e6f 6465 536f  y_struct, NodeSo
-00146fb0: 636b 6574 5374 616e 6461 7264 2c20 4e6f  cketStandard, No
+00146f90: 496e 7450 6572 6365 6e74 6167 6528 4e6f  IntPercentage(No
+00146fa0: 6465 536f 636b 6574 5374 616e 6461 7264  deSocketStandard
+00146fb0: 2c20 6270 795f 7374 7275 6374 2c20 4e6f  , bpy_struct, No
 00146fc0: 6465 536f 636b 6574 293a 0a0a 2020 2222  deSocket):..  ""
 00146fd0: 220a 0a20 2049 6e74 6567 6572 206e 756d  "..  Integer num
 00146fe0: 6265 7220 736f 636b 6574 206f 6620 6120  ber socket of a 
 00146ff0: 6e6f 6465 0a0a 2020 2222 220a 0a20 2064  node..  """..  d
 00147000: 6566 6175 6c74 5f76 616c 7565 3a20 696e  efault_value: in
 00147010: 7420 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  t = .....  """..
 00147020: 2020 496e 7075 7420 7661 6c75 6520 7573    Input value us
@@ -83735,17 +83735,17 @@
 00147160: 2020 6465 6620 626c 5f72 6e61 5f67 6574    def bl_rna_get
 00147170: 5f73 7562 636c 6173 735f 7079 2863 6c73  _subclass_py(cls
 00147180: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 00147190: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 001471a0: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 001471b0: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 001471c0: 0a63 6c61 7373 204e 6f64 6553 6f63 6b65  .class NodeSocke
-001471d0: 7449 6e74 556e 7369 676e 6564 2862 7079  tIntUnsigned(bpy
-001471e0: 5f73 7472 7563 742c 204e 6f64 6553 6f63  _struct, NodeSoc
-001471f0: 6b65 7453 7461 6e64 6172 642c 204e 6f64  ketStandard, Nod
+001471d0: 7449 6e74 556e 7369 676e 6564 284e 6f64  tIntUnsigned(Nod
+001471e0: 6553 6f63 6b65 7453 7461 6e64 6172 642c  eSocketStandard,
+001471f0: 2062 7079 5f73 7472 7563 742c 204e 6f64   bpy_struct, Nod
 00147200: 6553 6f63 6b65 7429 3a0a 0a20 2022 2222  eSocket):..  """
 00147210: 0a0a 2020 496e 7465 6765 7220 6e75 6d62  ..  Integer numb
 00147220: 6572 2073 6f63 6b65 7420 6f66 2061 206e  er socket of a n
 00147230: 6f64 650a 0a20 2022 2222 0a0a 2020 6465  ode..  """..  de
 00147240: 6661 756c 745f 7661 6c75 653a 2069 6e74  fault_value: int
 00147250: 203d 202e 2e2e 0a0a 2020 2222 220a 0a20   = .....  """.. 
 00147260: 2049 6e70 7574 2076 616c 7565 2075 7365   Input value use
@@ -83771,17 +83771,17 @@
 001473a0: 2064 6566 2062 6c5f 726e 615f 6765 745f   def bl_rna_get_
 001473b0: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 001473c0: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 001473d0: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 001473e0: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 001473f0: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 00147400: 636c 6173 7320 4e6f 6465 536f 636b 6574  class NodeSocket
-00147410: 4d61 7465 7269 616c 2862 7079 5f73 7472  Material(bpy_str
-00147420: 7563 742c 204e 6f64 6553 6f63 6b65 7453  uct, NodeSocketS
-00147430: 7461 6e64 6172 642c 204e 6f64 6553 6f63  tandard, NodeSoc
+00147410: 4d61 7465 7269 616c 284e 6f64 6553 6f63  Material(NodeSoc
+00147420: 6b65 7453 7461 6e64 6172 642c 2062 7079  ketStandard, bpy
+00147430: 5f73 7472 7563 742c 204e 6f64 6553 6f63  _struct, NodeSoc
 00147440: 6b65 7429 3a0a 0a20 2022 2222 0a0a 2020  ket):..  """..  
 00147450: 4d61 7465 7269 616c 2073 6f63 6b65 7420  Material socket 
 00147460: 6f66 2061 206e 6f64 650a 0a20 2022 2222  of a node..  """
 00147470: 0a0a 2020 6465 6661 756c 745f 7661 6c75  ..  default_valu
 00147480: 653a 204d 6174 6572 6961 6c20 3d20 2e2e  e: Material = ..
 00147490: 2e0a 0a20 2022 2222 0a0a 2020 496e 7075  ...  """..  Inpu
 001474a0: 7420 7661 6c75 6520 7573 6564 2066 6f72  t value used for
@@ -83807,16 +83807,16 @@
 001475e0: 626c 5f72 6e61 5f67 6574 5f73 7562 636c  bl_rna_get_subcl
 001475f0: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 00147600: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 00147610: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 00147620: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 00147630: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 00147640: 204e 6f64 6553 6f63 6b65 744f 626a 6563   NodeSocketObjec
-00147650: 7428 6270 795f 7374 7275 6374 2c20 4e6f  t(bpy_struct, No
-00147660: 6465 536f 636b 6574 5374 616e 6461 7264  deSocketStandard
+00147650: 7428 4e6f 6465 536f 636b 6574 5374 616e  t(NodeSocketStan
+00147660: 6461 7264 2c20 6270 795f 7374 7275 6374  dard, bpy_struct
 00147670: 2c20 4e6f 6465 536f 636b 6574 293a 0a0a  , NodeSocket):..
 00147680: 2020 2222 220a 0a20 204f 626a 6563 7420    """..  Object 
 00147690: 736f 636b 6574 206f 6620 6120 6e6f 6465  socket of a node
 001476a0: 0a0a 2020 2222 220a 0a20 2064 6566 6175  ..  """..  defau
 001476b0: 6c74 5f76 616c 7565 3a20 4f62 6a65 6374  lt_value: Object
 001476c0: 203d 202e 2e2e 0a0a 2020 2222 220a 0a20   = .....  """.. 
 001476d0: 2049 6e70 7574 2076 616c 7565 2075 7365   Input value use
@@ -83842,17 +83842,17 @@
 00147810: 2064 6566 2062 6c5f 726e 615f 6765 745f   def bl_rna_get_
 00147820: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 00147830: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 00147840: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 00147850: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 00147860: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 00147870: 636c 6173 7320 4e6f 6465 536f 636b 6574  class NodeSocket
-00147880: 5368 6164 6572 2862 7079 5f73 7472 7563  Shader(bpy_struc
-00147890: 742c 204e 6f64 6553 6f63 6b65 7453 7461  t, NodeSocketSta
-001478a0: 6e64 6172 642c 204e 6f64 6553 6f63 6b65  ndard, NodeSocke
+00147880: 5368 6164 6572 284e 6f64 6553 6f63 6b65  Shader(NodeSocke
+00147890: 7453 7461 6e64 6172 642c 2062 7079 5f73  tStandard, bpy_s
+001478a0: 7472 7563 742c 204e 6f64 6553 6f63 6b65  truct, NodeSocke
 001478b0: 7429 3a0a 0a20 2022 2222 0a0a 2020 5368  t):..  """..  Sh
 001478c0: 6164 6572 2073 6f63 6b65 7420 6f66 2061  ader socket of a
 001478d0: 206e 6f64 650a 0a20 2022 2222 0a0a 2020   node..  """..  
 001478e0: 6c69 6e6b 733a 2074 7970 696e 672e 416e  links: typing.An
 001478f0: 7920 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  y = .....  """..
 00147900: 2020 4c69 7374 206f 6620 6e6f 6465 206c    List of node l
 00147910: 696e 6b73 2066 726f 6d20 6f72 2074 6f20  inks from or to 
@@ -83872,17 +83872,17 @@
 001479f0: 6620 626c 5f72 6e61 5f67 6574 5f73 7562  f bl_rna_get_sub
 00147a00: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 00147a10: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 00147a20: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 00147a30: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 00147a40: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 00147a50: 7373 204e 6f64 6553 6f63 6b65 7453 7472  ss NodeSocketStr
-00147a60: 696e 6728 6270 795f 7374 7275 6374 2c20  ing(bpy_struct, 
-00147a70: 4e6f 6465 536f 636b 6574 5374 616e 6461  NodeSocketStanda
-00147a80: 7264 2c20 4e6f 6465 536f 636b 6574 293a  rd, NodeSocket):
+00147a60: 696e 6728 4e6f 6465 536f 636b 6574 5374  ing(NodeSocketSt
+00147a70: 616e 6461 7264 2c20 6270 795f 7374 7275  andard, bpy_stru
+00147a80: 6374 2c20 4e6f 6465 536f 636b 6574 293a  ct, NodeSocket):
 00147a90: 0a0a 2020 2222 220a 0a20 2053 7472 696e  ..  """..  Strin
 00147aa0: 6720 736f 636b 6574 206f 6620 6120 6e6f  g socket of a no
 00147ab0: 6465 0a0a 2020 2222 220a 0a20 2064 6566  de..  """..  def
 00147ac0: 6175 6c74 5f76 616c 7565 3a20 7374 7220  ault_value: str 
 00147ad0: 3d20 2e2e 2e0a 0a20 2022 2222 0a0a 2020  = .....  """..  
 00147ae0: 496e 7075 7420 7661 6c75 6520 7573 6564  Input value used
 00147af0: 2066 6f72 2075 6e63 6f6e 6e65 6374 6564   for unconnected
@@ -83907,17 +83907,17 @@
 00147c20: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 00147c30: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 00147c40: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 00147c50: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 00147c60: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 00147c70: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 00147c80: 6c61 7373 204e 6f64 6553 6f63 6b65 7454  lass NodeSocketT
-00147c90: 6578 7475 7265 2862 7079 5f73 7472 7563  exture(bpy_struc
-00147ca0: 742c 204e 6f64 6553 6f63 6b65 7453 7461  t, NodeSocketSta
-00147cb0: 6e64 6172 642c 204e 6f64 6553 6f63 6b65  ndard, NodeSocke
+00147c90: 6578 7475 7265 284e 6f64 6553 6f63 6b65  exture(NodeSocke
+00147ca0: 7453 7461 6e64 6172 642c 2062 7079 5f73  tStandard, bpy_s
+00147cb0: 7472 7563 742c 204e 6f64 6553 6f63 6b65  truct, NodeSocke
 00147cc0: 7429 3a0a 0a20 2022 2222 0a0a 2020 5465  t):..  """..  Te
 00147cd0: 7874 7572 6520 736f 636b 6574 206f 6620  xture socket of 
 00147ce0: 6120 6e6f 6465 0a0a 2020 2222 220a 0a20  a node..  """.. 
 00147cf0: 2064 6566 6175 6c74 5f76 616c 7565 3a20   default_value: 
 00147d00: 5465 7874 7572 6520 3d20 2e2e 2e0a 0a20  Texture = ..... 
 00147d10: 2022 2222 0a0a 2020 496e 7075 7420 7661   """..  Input va
 00147d20: 6c75 6520 7573 6564 2066 6f72 2075 6e63  lue used for unc
@@ -83942,17 +83942,17 @@
 00147e50: 7468 6f64 0a0a 2020 6465 6620 626c 5f72  thod..  def bl_r
 00147e60: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 00147e70: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 00147e80: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 00147e90: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 00147ea0: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 00147eb0: 2020 2e2e 2e0a 0a63 6c61 7373 204e 6f64    .....class Nod
-00147ec0: 6553 6f63 6b65 7456 6563 746f 7228 6270  eSocketVector(bp
-00147ed0: 795f 7374 7275 6374 2c20 4e6f 6465 536f  y_struct, NodeSo
-00147ee0: 636b 6574 5374 616e 6461 7264 2c20 4e6f  cketStandard, No
+00147ec0: 6553 6f63 6b65 7456 6563 746f 7228 4e6f  eSocketVector(No
+00147ed0: 6465 536f 636b 6574 5374 616e 6461 7264  deSocketStandard
+00147ee0: 2c20 6270 795f 7374 7275 6374 2c20 4e6f  , bpy_struct, No
 00147ef0: 6465 536f 636b 6574 293a 0a0a 2020 2222  deSocket):..  ""
 00147f00: 220a 0a20 2033 4420 7665 6374 6f72 2073  "..  3D vector s
 00147f10: 6f63 6b65 7420 6f66 2061 206e 6f64 650a  ocket of a node.
 00147f20: 0a20 2022 2222 0a0a 2020 6465 6661 756c  .  """..  defaul
 00147f30: 745f 7661 6c75 653a 2074 7970 696e 672e  t_value: typing.
 00147f40: 5475 706c 655b 666c 6f61 742c 2066 6c6f  Tuple[float, flo
 00147f50: 6174 2c20 666c 6f61 745d 203d 202e 2e2e  at, float] = ...
@@ -83980,17 +83980,17 @@
 001480b0: 6c5f 726e 615f 6765 745f 7375 6263 6c61  l_rna_get_subcla
 001480c0: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 001480d0: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 001480e0: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 001480f0: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 00148100: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 00148110: 4e6f 6465 536f 636b 6574 5665 6374 6f72  NodeSocketVector
-00148120: 4163 6365 6c65 7261 7469 6f6e 2862 7079  Acceleration(bpy
-00148130: 5f73 7472 7563 742c 204e 6f64 6553 6f63  _struct, NodeSoc
-00148140: 6b65 7453 7461 6e64 6172 642c 204e 6f64  ketStandard, Nod
+00148120: 4163 6365 6c65 7261 7469 6f6e 284e 6f64  Acceleration(Nod
+00148130: 6553 6f63 6b65 7453 7461 6e64 6172 642c  eSocketStandard,
+00148140: 2062 7079 5f73 7472 7563 742c 204e 6f64   bpy_struct, Nod
 00148150: 6553 6f63 6b65 7429 3a0a 0a20 2022 2222  eSocket):..  """
 00148160: 0a0a 2020 3344 2076 6563 746f 7220 736f  ..  3D vector so
 00148170: 636b 6574 206f 6620 6120 6e6f 6465 0a0a  cket of a node..
 00148180: 2020 2222 220a 0a20 2064 6566 6175 6c74    """..  default
 00148190: 5f76 616c 7565 3a20 6d61 7468 7574 696c  _value: mathutil
 001481a0: 732e 5665 6374 6f72 203d 202e 2e2e 0a0a  s.Vector = .....
 001481b0: 2020 2222 220a 0a20 2049 6e70 7574 2076    """..  Input v
@@ -84017,17 +84017,17 @@
 00148300: 726e 615f 6765 745f 7375 6263 6c61 7373  rna_get_subclass
 00148310: 5f70 7928 636c 732c 2069 643a 2073 7472  _py(cls, id: str
 00148320: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 00148330: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 00148340: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 00148350: 2020 202e 2e2e 0a0a 636c 6173 7320 4e6f     .....class No
 00148360: 6465 536f 636b 6574 5665 6374 6f72 4469  deSocketVectorDi
-00148370: 7265 6374 696f 6e28 6270 795f 7374 7275  rection(bpy_stru
-00148380: 6374 2c20 4e6f 6465 536f 636b 6574 5374  ct, NodeSocketSt
-00148390: 616e 6461 7264 2c20 4e6f 6465 536f 636b  andard, NodeSock
+00148370: 7265 6374 696f 6e28 4e6f 6465 536f 636b  rection(NodeSock
+00148380: 6574 5374 616e 6461 7264 2c20 6270 795f  etStandard, bpy_
+00148390: 7374 7275 6374 2c20 4e6f 6465 536f 636b  struct, NodeSock
 001483a0: 6574 293a 0a0a 2020 2222 220a 0a20 2033  et):..  """..  3
 001483b0: 4420 7665 6374 6f72 2073 6f63 6b65 7420  D vector socket 
 001483c0: 6f66 2061 206e 6f64 650a 0a20 2022 2222  of a node..  """
 001483d0: 0a0a 2020 6465 6661 756c 745f 7661 6c75  ..  default_valu
 001483e0: 653a 206d 6174 6875 7469 6c73 2e56 6563  e: mathutils.Vec
 001483f0: 746f 7220 3d20 2e2e 2e0a 0a20 2022 2222  tor = .....  """
 00148400: 0a0a 2020 496e 7075 7420 7661 6c75 6520  ..  Input value 
@@ -84053,17 +84053,17 @@
 00148540: 0a0a 2020 6465 6620 626c 5f72 6e61 5f67  ..  def bl_rna_g
 00148550: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 00148560: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 00148570: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 00148580: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 00148590: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 001485a0: 2e0a 0a63 6c61 7373 204e 6f64 6553 6f63  ...class NodeSoc
-001485b0: 6b65 7456 6563 746f 7245 756c 6572 2862  ketVectorEuler(b
-001485c0: 7079 5f73 7472 7563 742c 204e 6f64 6553  py_struct, NodeS
-001485d0: 6f63 6b65 7453 7461 6e64 6172 642c 204e  ocketStandard, N
+001485b0: 6b65 7456 6563 746f 7245 756c 6572 284e  ketVectorEuler(N
+001485c0: 6f64 6553 6f63 6b65 7453 7461 6e64 6172  odeSocketStandar
+001485d0: 642c 2062 7079 5f73 7472 7563 742c 204e  d, bpy_struct, N
 001485e0: 6f64 6553 6f63 6b65 7429 3a0a 0a20 2022  odeSocket):..  "
 001485f0: 2222 0a0a 2020 3344 2076 6563 746f 7220  ""..  3D vector 
 00148600: 736f 636b 6574 206f 6620 6120 6e6f 6465  socket of a node
 00148610: 0a0a 2020 2222 220a 0a20 2064 6566 6175  ..  """..  defau
 00148620: 6c74 5f76 616c 7565 3a20 6d61 7468 7574  lt_value: mathut
 00148630: 696c 732e 4575 6c65 7220 3d20 2e2e 2e0a  ils.Euler = ....
 00148640: 0a20 2022 2222 0a0a 2020 496e 7075 7420  .  """..  Input 
@@ -84090,17 +84090,17 @@
 00148790: 5f72 6e61 5f67 6574 5f73 7562 636c 6173  _rna_get_subclas
 001487a0: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 001487b0: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 001487c0: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 001487d0: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 001487e0: 2020 2020 2e2e 2e0a 0a63 6c61 7373 204e      .....class N
 001487f0: 6f64 6553 6f63 6b65 7456 6563 746f 7254  odeSocketVectorT
-00148800: 7261 6e73 6c61 7469 6f6e 2862 7079 5f73  ranslation(bpy_s
-00148810: 7472 7563 742c 204e 6f64 6553 6f63 6b65  truct, NodeSocke
-00148820: 7453 7461 6e64 6172 642c 204e 6f64 6553  tStandard, NodeS
+00148800: 7261 6e73 6c61 7469 6f6e 284e 6f64 6553  ranslation(NodeS
+00148810: 6f63 6b65 7453 7461 6e64 6172 642c 2062  ocketStandard, b
+00148820: 7079 5f73 7472 7563 742c 204e 6f64 6553  py_struct, NodeS
 00148830: 6f63 6b65 7429 3a0a 0a20 2022 2222 0a0a  ocket):..  """..
 00148840: 2020 3344 2076 6563 746f 7220 736f 636b    3D vector sock
 00148850: 6574 206f 6620 6120 6e6f 6465 0a0a 2020  et of a node..  
 00148860: 2222 220a 0a20 2064 6566 6175 6c74 5f76  """..  default_v
 00148870: 616c 7565 3a20 6d61 7468 7574 696c 732e  alue: mathutils.
 00148880: 5665 6374 6f72 203d 202e 2e2e 0a0a 2020  Vector = .....  
 00148890: 2222 220a 0a20 2049 6e70 7574 2076 616c  """..  Input val
@@ -84127,17 +84127,17 @@
 001489e0: 615f 6765 745f 7375 6263 6c61 7373 5f70  a_get_subclass_p
 001489f0: 7928 636c 732c 2069 643a 2073 7472 2c20  y(cls, id: str, 
 00148a00: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 00148a10: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 00148a20: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 00148a30: 202e 2e2e 0a0a 636c 6173 7320 4e6f 6465   .....class Node
 00148a40: 536f 636b 6574 5665 6374 6f72 5665 6c6f  SocketVectorVelo
-00148a50: 6369 7479 2862 7079 5f73 7472 7563 742c  city(bpy_struct,
-00148a60: 204e 6f64 6553 6f63 6b65 7453 7461 6e64   NodeSocketStand
-00148a70: 6172 642c 204e 6f64 6553 6f63 6b65 7429  ard, NodeSocket)
+00148a50: 6369 7479 284e 6f64 6553 6f63 6b65 7453  city(NodeSocketS
+00148a60: 7461 6e64 6172 642c 2062 7079 5f73 7472  tandard, bpy_str
+00148a70: 7563 742c 204e 6f64 6553 6f63 6b65 7429  uct, NodeSocket)
 00148a80: 3a0a 0a20 2022 2222 0a0a 2020 3344 2076  :..  """..  3D v
 00148a90: 6563 746f 7220 736f 636b 6574 206f 6620  ector socket of 
 00148aa0: 6120 6e6f 6465 0a0a 2020 2222 220a 0a20  a node..  """.. 
 00148ab0: 2064 6566 6175 6c74 5f76 616c 7565 3a20   default_value: 
 00148ac0: 6d61 7468 7574 696c 732e 5665 6374 6f72  mathutils.Vector
 00148ad0: 203d 202e 2e2e 0a0a 2020 2222 220a 0a20   = .....  """.. 
 00148ae0: 2049 6e70 7574 2076 616c 7565 2075 7365   Input value use
@@ -84163,17 +84163,17 @@
 00148c20: 2064 6566 2062 6c5f 726e 615f 6765 745f   def bl_rna_get_
 00148c30: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 00148c40: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 00148c50: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 00148c60: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 00148c70: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 00148c80: 636c 6173 7320 4e6f 6465 536f 636b 6574  class NodeSocket
-00148c90: 5665 6374 6f72 5859 5a28 6270 795f 7374  VectorXYZ(bpy_st
-00148ca0: 7275 6374 2c20 4e6f 6465 536f 636b 6574  ruct, NodeSocket
-00148cb0: 5374 616e 6461 7264 2c20 4e6f 6465 536f  Standard, NodeSo
+00148c90: 5665 6374 6f72 5859 5a28 4e6f 6465 536f  VectorXYZ(NodeSo
+00148ca0: 636b 6574 5374 616e 6461 7264 2c20 6270  cketStandard, bp
+00148cb0: 795f 7374 7275 6374 2c20 4e6f 6465 536f  y_struct, NodeSo
 00148cc0: 636b 6574 293a 0a0a 2020 2222 220a 0a20  cket):..  """.. 
 00148cd0: 2033 4420 7665 6374 6f72 2073 6f63 6b65   3D vector socke
 00148ce0: 7420 6f66 2061 206e 6f64 650a 0a20 2022  t of a node..  "
 00148cf0: 2222 0a0a 2020 6465 6661 756c 745f 7661  ""..  default_va
 00148d00: 6c75 653a 206d 6174 6875 7469 6c73 2e56  lue: mathutils.V
 00148d10: 6563 746f 7220 3d20 2e2e 2e0a 0a20 2022  ector = .....  "
 00148d20: 2222 0a0a 2020 496e 7075 7420 7661 6c75  ""..  Input valu
@@ -84199,17 +84199,17 @@
 00148e60: 6f64 0a0a 2020 6465 6620 626c 5f72 6e61  od..  def bl_rna
 00148e70: 5f67 6574 5f73 7562 636c 6173 735f 7079  _get_subclass_py
 00148e80: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 00148e90: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 00148ea0: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 00148eb0: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 00148ec0: 2e2e 2e0a 0a63 6c61 7373 204e 6f64 6553  .....class NodeS
-00148ed0: 6f63 6b65 7456 6972 7475 616c 2862 7079  ocketVirtual(bpy
-00148ee0: 5f73 7472 7563 742c 204e 6f64 6553 6f63  _struct, NodeSoc
-00148ef0: 6b65 7453 7461 6e64 6172 642c 204e 6f64  ketStandard, Nod
+00148ed0: 6f63 6b65 7456 6972 7475 616c 284e 6f64  ocketVirtual(Nod
+00148ee0: 6553 6f63 6b65 7453 7461 6e64 6172 642c  eSocketStandard,
+00148ef0: 2062 7079 5f73 7472 7563 742c 204e 6f64   bpy_struct, Nod
 00148f00: 6553 6f63 6b65 7429 3a0a 0a20 2022 2222  eSocket):..  """
 00148f10: 0a0a 2020 5669 7274 7561 6c20 736f 636b  ..  Virtual sock
 00148f20: 6574 206f 6620 6120 6e6f 6465 0a0a 2020  et of a node..  
 00148f30: 2222 220a 0a20 206c 696e 6b73 3a20 7479  """..  links: ty
 00148f40: 7069 6e67 2e41 6e79 203d 202e 2e2e 0a0a  ping.Any = .....
 00148f50: 2020 2222 220a 0a20 204c 6973 7420 6f66    """..  List of
 00148f60: 206e 6f64 6520 6c69 6e6b 7320 6672 6f6d   node links from
@@ -85181,16 +85181,16 @@
 0014cbc0: 2062 6c5f 726e 615f 6765 745f 7375 6263   bl_rna_get_subc
 0014cbd0: 6c61 7373 5f70 7928 636c 732c 2069 643a  lass_py(cls, id:
 0014cbe0: 2073 7472 2c20 6465 6661 756c 743a 2074   str, default: t
 0014cbf0: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 0014cc00: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 0014cc10: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 0014cc20: 7320 4164 6453 6571 7565 6e63 6528 6270  s AddSequence(bp
-0014cc30: 795f 7374 7275 6374 2c20 5365 7175 656e  y_struct, Sequen
-0014cc40: 6365 2c20 4566 6665 6374 5365 7175 656e  ce, EffectSequen
+0014cc30: 795f 7374 7275 6374 2c20 4566 6665 6374  y_struct, Effect
+0014cc40: 5365 7175 656e 6365 2c20 5365 7175 656e  Sequence, Sequen
 0014cc50: 6365 293a 0a0a 2020 2222 220a 0a20 2041  ce):..  """..  A
 0014cc60: 6464 2053 6571 7565 6e63 650a 0a20 2022  dd Sequence..  "
 0014cc70: 2222 0a0a 2020 696e 7075 745f 313a 2053  ""..  input_1: S
 0014cc80: 6571 7565 6e63 6520 3d20 2e2e 2e0a 0a20  equence = ..... 
 0014cc90: 2022 2222 0a0a 2020 4669 7273 7420 696e   """..  First in
 0014cca0: 7075 7420 666f 7220 7468 6520 6566 6665  put for the effe
 0014ccb0: 6374 2073 7472 6970 0a0a 2020 2222 220a  ct strip..  """.
@@ -85212,16 +85212,16 @@
 0014cdb0: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 0014cdc0: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 0014cdd0: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 0014cde0: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 0014cdf0: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 0014ce00: 2e0a 0a63 6c61 7373 2041 646a 7573 746d  ...class Adjustm
 0014ce10: 656e 7453 6571 7565 6e63 6528 6270 795f  entSequence(bpy_
-0014ce20: 7374 7275 6374 2c20 5365 7175 656e 6365  struct, Sequence
-0014ce30: 2c20 4566 6665 6374 5365 7175 656e 6365  , EffectSequence
+0014ce20: 7374 7275 6374 2c20 4566 6665 6374 5365  struct, EffectSe
+0014ce30: 7175 656e 6365 2c20 5365 7175 656e 6365  quence, Sequence
 0014ce40: 293a 0a0a 2020 2222 220a 0a20 2053 6571  ):..  """..  Seq
 0014ce50: 7565 6e63 6520 7374 7269 7020 746f 2070  uence strip to p
 0014ce60: 6572 666f 726d 2066 696c 7465 7220 6164  erform filter ad
 0014ce70: 6a75 7374 6d65 6e74 7320 746f 206c 6179  justments to lay
 0014ce80: 6572 7320 6265 6c6f 770a 0a20 2022 2222  ers below..  """
 0014ce90: 0a0a 2020 616e 696d 6174 696f 6e5f 6f66  ..  animation_of
 0014cea0: 6673 6574 5f65 6e64 3a20 696e 7420 3d20  fset_end: int = 
@@ -85247,16 +85247,16 @@
 0014cfe0: 6765 745f 7375 6263 6c61 7373 5f70 7928  get_subclass_py(
 0014cff0: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 0014d000: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 0014d010: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 0014d020: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 0014d030: 2e2e 0a0a 636c 6173 7320 416c 7068 614f  ....class AlphaO
 0014d040: 7665 7253 6571 7565 6e63 6528 6270 795f  verSequence(bpy_
-0014d050: 7374 7275 6374 2c20 5365 7175 656e 6365  struct, Sequence
-0014d060: 2c20 4566 6665 6374 5365 7175 656e 6365  , EffectSequence
+0014d050: 7374 7275 6374 2c20 4566 6665 6374 5365  struct, EffectSe
+0014d060: 7175 656e 6365 2c20 5365 7175 656e 6365  quence, Sequence
 0014d070: 293a 0a0a 2020 2222 220a 0a20 2041 6c70  ):..  """..  Alp
 0014d080: 6861 204f 7665 7220 5365 7175 656e 6365  ha Over Sequence
 0014d090: 0a0a 2020 2222 220a 0a20 2069 6e70 7574  ..  """..  input
 0014d0a0: 5f31 3a20 5365 7175 656e 6365 203d 202e  _1: Sequence = .
 0014d0b0: 2e2e 0a0a 2020 2222 220a 0a20 2046 6972  ....  """..  Fir
 0014d0c0: 7374 2069 6e70 7574 2066 6f72 2074 6865  st input for the
 0014d0d0: 2065 6666 6563 7420 7374 7269 700a 0a20   effect strip.. 
@@ -85278,16 +85278,16 @@
 0014d1d0: 726e 615f 6765 745f 7375 6263 6c61 7373  rna_get_subclass
 0014d1e0: 5f70 7928 636c 732c 2069 643a 2073 7472  _py(cls, id: str
 0014d1f0: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 0014d200: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 0014d210: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 0014d220: 2020 202e 2e2e 0a0a 636c 6173 7320 416c     .....class Al
 0014d230: 7068 6155 6e64 6572 5365 7175 656e 6365  phaUnderSequence
-0014d240: 2862 7079 5f73 7472 7563 742c 2053 6571  (bpy_struct, Seq
-0014d250: 7565 6e63 652c 2045 6666 6563 7453 6571  uence, EffectSeq
+0014d240: 2862 7079 5f73 7472 7563 742c 2045 6666  (bpy_struct, Eff
+0014d250: 6563 7453 6571 7565 6e63 652c 2053 6571  ectSequence, Seq
 0014d260: 7565 6e63 6529 3a0a 0a20 2022 2222 0a0a  uence):..  """..
 0014d270: 2020 416c 7068 6120 556e 6465 7220 5365    Alpha Under Se
 0014d280: 7175 656e 6365 0a0a 2020 2222 220a 0a20  quence..  """.. 
 0014d290: 2069 6e70 7574 5f31 3a20 5365 7175 656e   input_1: Sequen
 0014d2a0: 6365 203d 202e 2e2e 0a0a 2020 2222 220a  ce = .....  """.
 0014d2b0: 0a20 2046 6972 7374 2069 6e70 7574 2066  .  First input f
 0014d2c0: 6f72 2074 6865 2065 6666 6563 7420 7374  or the effect st
@@ -85310,16 +85310,16 @@
 0014d3d0: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 0014d3e0: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 0014d3f0: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 0014d400: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 0014d410: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 0014d420: 6173 7320 436f 6c6f 724d 6978 5365 7175  ass ColorMixSequ
 0014d430: 656e 6365 2862 7079 5f73 7472 7563 742c  ence(bpy_struct,
-0014d440: 2053 6571 7565 6e63 652c 2045 6666 6563   Sequence, Effec
-0014d450: 7453 6571 7565 6e63 6529 3a0a 0a20 2022  tSequence):..  "
+0014d440: 2045 6666 6563 7453 6571 7565 6e63 652c   EffectSequence,
+0014d450: 2053 6571 7565 6e63 6529 3a0a 0a20 2022   Sequence):..  "
 0014d460: 2222 0a0a 2020 436f 6c6f 7220 4d69 7820  ""..  Color Mix 
 0014d470: 5365 7175 656e 6365 0a0a 2020 2222 220a  Sequence..  """.
 0014d480: 0a20 2062 6c65 6e64 5f65 6666 6563 743a  .  blend_effect:
 0014d490: 2073 7472 203d 202e 2e2e 0a0a 2020 2222   str = .....  ""
 0014d4a0: 220a 0a20 204d 6574 686f 6420 666f 7220  "..  Method for 
 0014d4b0: 636f 6e74 726f 6c6c 696e 6720 686f 7720  controlling how 
 0014d4c0: 7468 6520 7374 7269 7020 636f 6d62 696e  the strip combin
@@ -85354,16 +85354,16 @@
 0014d690: 745f 7375 6263 6c61 7373 5f70 7928 636c  t_subclass_py(cl
 0014d6a0: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 0014d6b0: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 0014d6c0: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 0014d6d0: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 0014d6e0: 0a0a 636c 6173 7320 436f 6c6f 7253 6571  ..class ColorSeq
 0014d6f0: 7565 6e63 6528 6270 795f 7374 7275 6374  uence(bpy_struct
-0014d700: 2c20 5365 7175 656e 6365 2c20 4566 6665  , Sequence, Effe
-0014d710: 6374 5365 7175 656e 6365 293a 0a0a 2020  ctSequence):..  
+0014d700: 2c20 4566 6665 6374 5365 7175 656e 6365  , EffectSequence
+0014d710: 2c20 5365 7175 656e 6365 293a 0a0a 2020  , Sequence):..  
 0014d720: 2222 220a 0a20 2053 6571 7565 6e63 6520  """..  Sequence 
 0014d730: 7374 7269 7020 6372 6561 7469 6e67 2061  strip creating a
 0014d740: 6e20 696d 6167 6520 6669 6c6c 6564 2077  n image filled w
 0014d750: 6974 6820 6120 7369 6e67 6c65 2063 6f6c  ith a single col
 0014d760: 6f72 0a0a 2020 2222 220a 0a20 2063 6f6c  or..  """..  col
 0014d770: 6f72 3a20 6d61 7468 7574 696c 732e 436f  or: mathutils.Co
 0014d780: 6c6f 7220 3d20 2e2e 2e0a 0a20 2022 2222  lor = .....  """
@@ -85382,16 +85382,16 @@
 0014d850: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 0014d860: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 0014d870: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 0014d880: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 0014d890: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 0014d8a0: 2e0a 0a63 6c61 7373 2043 726f 7373 5365  ...class CrossSe
 0014d8b0: 7175 656e 6365 2862 7079 5f73 7472 7563  quence(bpy_struc
-0014d8c0: 742c 2053 6571 7565 6e63 652c 2045 6666  t, Sequence, Eff
-0014d8d0: 6563 7453 6571 7565 6e63 6529 3a0a 0a20  ectSequence):.. 
+0014d8c0: 742c 2045 6666 6563 7453 6571 7565 6e63  t, EffectSequenc
+0014d8d0: 652c 2053 6571 7565 6e63 6529 3a0a 0a20  e, Sequence):.. 
 0014d8e0: 2022 2222 0a0a 2020 4372 6f73 7320 5365   """..  Cross Se
 0014d8f0: 7175 656e 6365 0a0a 2020 2222 220a 0a20  quence..  """.. 
 0014d900: 2069 6e70 7574 5f31 3a20 5365 7175 656e   input_1: Sequen
 0014d910: 6365 203d 202e 2e2e 0a0a 2020 2222 220a  ce = .....  """.
 0014d920: 0a20 2046 6972 7374 2069 6e70 7574 2066  .  First input f
 0014d930: 6f72 2074 6865 2065 6666 6563 7420 7374  or the effect st
 0014d940: 7269 700a 0a20 2022 2222 0a0a 2020 696e  rip..  """..  in
@@ -85413,16 +85413,16 @@
 0014da40: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 0014da50: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 0014da60: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 0014da70: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 0014da80: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 0014da90: 6173 7320 4761 6d6d 6143 726f 7373 5365  ass GammaCrossSe
 0014daa0: 7175 656e 6365 2862 7079 5f73 7472 7563  quence(bpy_struc
-0014dab0: 742c 2053 6571 7565 6e63 652c 2045 6666  t, Sequence, Eff
-0014dac0: 6563 7453 6571 7565 6e63 6529 3a0a 0a20  ectSequence):.. 
+0014dab0: 742c 2045 6666 6563 7453 6571 7565 6e63  t, EffectSequenc
+0014dac0: 652c 2053 6571 7565 6e63 6529 3a0a 0a20  e, Sequence):.. 
 0014dad0: 2022 2222 0a0a 2020 4761 6d6d 6120 4372   """..  Gamma Cr
 0014dae0: 6f73 7320 5365 7175 656e 6365 0a0a 2020  oss Sequence..  
 0014daf0: 2222 220a 0a20 2069 6e70 7574 5f31 3a20  """..  input_1: 
 0014db00: 5365 7175 656e 6365 203d 202e 2e2e 0a0a  Sequence = .....
 0014db10: 2020 2222 220a 0a20 2046 6972 7374 2069    """..  First i
 0014db20: 6e70 7574 2066 6f72 2074 6865 2065 6666  nput for the eff
 0014db30: 6563 7420 7374 7269 700a 0a20 2022 2222  ect strip..  """
@@ -85444,16 +85444,16 @@
 0014dc30: 6765 745f 7375 6263 6c61 7373 5f70 7928  get_subclass_py(
 0014dc40: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 0014dc50: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 0014dc60: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 0014dc70: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 0014dc80: 2e2e 0a0a 636c 6173 7320 4761 7573 7369  ....class Gaussi
 0014dc90: 616e 426c 7572 5365 7175 656e 6365 2862  anBlurSequence(b
-0014dca0: 7079 5f73 7472 7563 742c 2053 6571 7565  py_struct, Seque
-0014dcb0: 6e63 652c 2045 6666 6563 7453 6571 7565  nce, EffectSeque
+0014dca0: 7079 5f73 7472 7563 742c 2045 6666 6563  py_struct, Effec
+0014dcb0: 7453 6571 7565 6e63 652c 2053 6571 7565  tSequence, Seque
 0014dcc0: 6e63 6529 3a0a 0a20 2022 2222 0a0a 2020  nce):..  """..  
 0014dcd0: 5365 7175 656e 6365 2073 7472 6970 2063  Sequence strip c
 0014dce0: 7265 6174 696e 6720 6120 6761 7573 7369  reating a gaussi
 0014dcf0: 616e 2062 6c75 720a 0a20 2022 2222 0a0a  an blur..  """..
 0014dd00: 2020 696e 7075 745f 313a 2053 6571 7565    input_1: Seque
 0014dd10: 6e63 6520 3d20 2e2e 2e0a 0a20 2022 2222  nce = .....  """
 0014dd20: 0a0a 2020 4669 7273 7420 696e 7075 7420  ..  First input 
@@ -85480,16 +85480,16 @@
 0014de70: 6620 626c 5f72 6e61 5f67 6574 5f73 7562  f bl_rna_get_sub
 0014de80: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 0014de90: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 0014dea0: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 0014deb0: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 0014dec0: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 0014ded0: 7373 2047 6c6f 7753 6571 7565 6e63 6528  ss GlowSequence(
-0014dee0: 6270 795f 7374 7275 6374 2c20 5365 7175  bpy_struct, Sequ
-0014def0: 656e 6365 2c20 4566 6665 6374 5365 7175  ence, EffectSequ
+0014dee0: 6270 795f 7374 7275 6374 2c20 4566 6665  bpy_struct, Effe
+0014def0: 6374 5365 7175 656e 6365 2c20 5365 7175  ctSequence, Sequ
 0014df00: 656e 6365 293a 0a0a 2020 2222 220a 0a20  ence):..  """.. 
 0014df10: 2053 6571 7565 6e63 6520 7374 7269 7020   Sequence strip 
 0014df20: 6372 6561 7469 6e67 2061 2067 6c6f 7720  creating a glow 
 0014df30: 6566 6665 6374 0a0a 2020 2222 220a 0a20  effect..  """.. 
 0014df40: 2062 6c75 725f 7261 6469 7573 3a20 666c   blur_radius: fl
 0014df50: 6f61 7420 3d20 2e2e 2e0a 0a20 2022 2222  oat = .....  """
 0014df60: 0a0a 2020 5261 6469 7573 206f 6620 676c  ..  Radius of gl
@@ -85534,16 +85534,16 @@
 0014e1d0: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 0014e1e0: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 0014e1f0: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 0014e200: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 0014e210: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 0014e220: 2020 2e2e 2e0a 0a63 6c61 7373 204d 756c    .....class Mul
 0014e230: 7469 6361 6d53 6571 7565 6e63 6528 6270  ticamSequence(bp
-0014e240: 795f 7374 7275 6374 2c20 5365 7175 656e  y_struct, Sequen
-0014e250: 6365 2c20 4566 6665 6374 5365 7175 656e  ce, EffectSequen
+0014e240: 795f 7374 7275 6374 2c20 4566 6665 6374  y_struct, Effect
+0014e250: 5365 7175 656e 6365 2c20 5365 7175 656e  Sequence, Sequen
 0014e260: 6365 293a 0a0a 2020 2222 220a 0a20 2053  ce):..  """..  S
 0014e270: 6571 7565 6e63 6520 7374 7269 7020 746f  equence strip to
 0014e280: 2070 6572 666f 726d 206d 756c 7469 6361   perform multica
 0014e290: 6d20 6564 6974 696e 670a 0a20 2022 2222  m editing..  """
 0014e2a0: 0a0a 2020 616e 696d 6174 696f 6e5f 6f66  ..  animation_of
 0014e2b0: 6673 6574 5f65 6e64 3a20 696e 7420 3d20  fset_end: int = 
 0014e2c0: 2e2e 2e0a 0a20 2022 2222 0a0a 2020 416e  .....  """..  An
@@ -85570,16 +85570,16 @@
 0014e410: 745f 7375 6263 6c61 7373 5f70 7928 636c  t_subclass_py(cl
 0014e420: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 0014e430: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 0014e440: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 0014e450: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 0014e460: 0a0a 636c 6173 7320 4d75 6c74 6970 6c79  ..class Multiply
 0014e470: 5365 7175 656e 6365 2862 7079 5f73 7472  Sequence(bpy_str
-0014e480: 7563 742c 2053 6571 7565 6e63 652c 2045  uct, Sequence, E
-0014e490: 6666 6563 7453 6571 7565 6e63 6529 3a0a  ffectSequence):.
+0014e480: 7563 742c 2045 6666 6563 7453 6571 7565  uct, EffectSeque
+0014e490: 6e63 652c 2053 6571 7565 6e63 6529 3a0a  nce, Sequence):.
 0014e4a0: 0a20 2022 2222 0a0a 2020 4d75 6c74 6970  .  """..  Multip
 0014e4b0: 6c79 2053 6571 7565 6e63 650a 0a20 2022  ly Sequence..  "
 0014e4c0: 2222 0a0a 2020 696e 7075 745f 313a 2053  ""..  input_1: S
 0014e4d0: 6571 7565 6e63 6520 3d20 2e2e 2e0a 0a20  equence = ..... 
 0014e4e0: 2022 2222 0a0a 2020 4669 7273 7420 696e   """..  First in
 0014e4f0: 7075 7420 666f 7220 7468 6520 6566 6665  put for the effe
 0014e500: 6374 2073 7472 6970 0a0a 2020 2222 220a  ct strip..  """.
@@ -85601,16 +85601,16 @@
 0014e600: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 0014e610: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 0014e620: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 0014e630: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 0014e640: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 0014e650: 2e0a 0a63 6c61 7373 204f 7665 7244 726f  ...class OverDro
 0014e660: 7053 6571 7565 6e63 6528 6270 795f 7374  pSequence(bpy_st
-0014e670: 7275 6374 2c20 5365 7175 656e 6365 2c20  ruct, Sequence, 
-0014e680: 4566 6665 6374 5365 7175 656e 6365 293a  EffectSequence):
+0014e670: 7275 6374 2c20 4566 6665 6374 5365 7175  ruct, EffectSequ
+0014e680: 656e 6365 2c20 5365 7175 656e 6365 293a  ence, Sequence):
 0014e690: 0a0a 2020 2222 220a 0a20 204f 7665 7220  ..  """..  Over 
 0014e6a0: 4472 6f70 2053 6571 7565 6e63 650a 0a20  Drop Sequence.. 
 0014e6b0: 2022 2222 0a0a 2020 696e 7075 745f 313a   """..  input_1:
 0014e6c0: 2053 6571 7565 6e63 6520 3d20 2e2e 2e0a   Sequence = ....
 0014e6d0: 0a20 2022 2222 0a0a 2020 4669 7273 7420  .  """..  First 
 0014e6e0: 696e 7075 7420 666f 7220 7468 6520 6566  input for the ef
 0014e6f0: 6665 6374 2073 7472 6970 0a0a 2020 2222  fect strip..  ""
@@ -85632,16 +85632,16 @@
 0014e7f0: 5f67 6574 5f73 7562 636c 6173 735f 7079  _get_subclass_py
 0014e800: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 0014e810: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 0014e820: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 0014e830: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 0014e840: 2e2e 2e0a 0a63 6c61 7373 2053 7065 6564  .....class Speed
 0014e850: 436f 6e74 726f 6c53 6571 7565 6e63 6528  ControlSequence(
-0014e860: 6270 795f 7374 7275 6374 2c20 5365 7175  bpy_struct, Sequ
-0014e870: 656e 6365 2c20 4566 6665 6374 5365 7175  ence, EffectSequ
+0014e860: 6270 795f 7374 7275 6374 2c20 4566 6665  bpy_struct, Effe
+0014e870: 6374 5365 7175 656e 6365 2c20 5365 7175  ctSequence, Sequ
 0014e880: 656e 6365 293a 0a0a 2020 2222 220a 0a20  ence):..  """.. 
 0014e890: 2053 6571 7565 6e63 6520 7374 7269 7020   Sequence strip 
 0014e8a0: 746f 2063 6f6e 7472 6f6c 2074 6865 2073  to control the s
 0014e8b0: 7065 6564 206f 6620 6f74 6865 7220 7374  peed of other st
 0014e8c0: 7269 7073 0a0a 2020 2222 220a 0a20 2069  rips..  """..  i
 0014e8d0: 6e70 7574 5f31 3a20 5365 7175 656e 6365  nput_1: Sequence
 0014e8e0: 203d 202e 2e2e 0a0a 2020 2222 220a 0a20   = .....  """.. 
@@ -85708,16 +85708,16 @@
 0014ecb0: 6c5f 726e 615f 6765 745f 7375 6263 6c61  l_rna_get_subcla
 0014ecc0: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 0014ecd0: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 0014ece0: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 0014ecf0: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 0014ed00: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 0014ed10: 5375 6274 7261 6374 5365 7175 656e 6365  SubtractSequence
-0014ed20: 2862 7079 5f73 7472 7563 742c 2053 6571  (bpy_struct, Seq
-0014ed30: 7565 6e63 652c 2045 6666 6563 7453 6571  uence, EffectSeq
+0014ed20: 2862 7079 5f73 7472 7563 742c 2045 6666  (bpy_struct, Eff
+0014ed30: 6563 7453 6571 7565 6e63 652c 2053 6571  ectSequence, Seq
 0014ed40: 7565 6e63 6529 3a0a 0a20 2022 2222 0a0a  uence):..  """..
 0014ed50: 2020 5375 6274 7261 6374 2053 6571 7565    Subtract Seque
 0014ed60: 6e63 650a 0a20 2022 2222 0a0a 2020 696e  nce..  """..  in
 0014ed70: 7075 745f 313a 2053 6571 7565 6e63 6520  put_1: Sequence 
 0014ed80: 3d20 2e2e 2e0a 0a20 2022 2222 0a0a 2020  = .....  """..  
 0014ed90: 4669 7273 7420 696e 7075 7420 666f 7220  First input for 
 0014eda0: 7468 6520 6566 6665 6374 2073 7472 6970  the effect strip
@@ -85739,16 +85739,16 @@
 0014eea0: 626c 5f72 6e61 5f67 6574 5f73 7562 636c  bl_rna_get_subcl
 0014eeb0: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 0014eec0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 0014eed0: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 0014eee0: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 0014eef0: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 0014ef00: 2054 6578 7453 6571 7565 6e63 6528 6270   TextSequence(bp
-0014ef10: 795f 7374 7275 6374 2c20 5365 7175 656e  y_struct, Sequen
-0014ef20: 6365 2c20 4566 6665 6374 5365 7175 656e  ce, EffectSequen
+0014ef10: 795f 7374 7275 6374 2c20 4566 6665 6374  y_struct, Effect
+0014ef20: 5365 7175 656e 6365 2c20 5365 7175 656e  Sequence, Sequen
 0014ef30: 6365 293a 0a0a 2020 2222 220a 0a20 2053  ce):..  """..  S
 0014ef40: 6571 7565 6e63 6520 7374 7269 7020 6372  equence strip cr
 0014ef50: 6561 7469 6e67 2074 6578 740a 0a20 2022  eating text..  "
 0014ef60: 2222 0a0a 2020 616c 6967 6e5f 783a 2073  ""..  align_x: s
 0014ef70: 7472 203d 202e 2e2e 0a0a 2020 2222 220a  tr = .....  """.
 0014ef80: 0a20 2041 6c69 676e 2074 6865 2074 6578  .  Align the tex
 0014ef90: 7420 616c 6f6e 6720 7468 6520 5820 6178  t along the X ax
@@ -85833,16 +85833,16 @@
 0014f480: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 0014f490: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 0014f4a0: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 0014f4b0: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 0014f4c0: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 0014f4d0: 7373 2054 7261 6e73 666f 726d 5365 7175  ss TransformSequ
 0014f4e0: 656e 6365 2862 7079 5f73 7472 7563 742c  ence(bpy_struct,
-0014f4f0: 2053 6571 7565 6e63 652c 2045 6666 6563   Sequence, Effec
-0014f500: 7453 6571 7565 6e63 6529 3a0a 0a20 2022  tSequence):..  "
+0014f4f0: 2045 6666 6563 7453 6571 7565 6e63 652c   EffectSequence,
+0014f500: 2053 6571 7565 6e63 6529 3a0a 0a20 2022   Sequence):..  "
 0014f510: 2222 0a0a 2020 5365 7175 656e 6365 2073  ""..  Sequence s
 0014f520: 7472 6970 2061 7070 6c79 696e 6720 6166  trip applying af
 0014f530: 6669 6e65 2074 7261 6e73 666f 726d 6174  fine transformat
 0014f540: 696f 6e73 2074 6f20 6f74 6865 7220 7374  ions to other st
 0014f550: 7269 7073 0a0a 2020 2222 220a 0a20 2069  rips..  """..  i
 0014f560: 6e70 7574 5f31 3a20 5365 7175 656e 6365  nput_1: Sequence
 0014f570: 203d 202e 2e2e 0a0a 2020 2222 220a 0a20   = .....  """.. 
@@ -85914,16 +85914,16 @@
 0014f990: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 0014f9a0: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 0014f9b0: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 0014f9c0: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 0014f9d0: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 0014f9e0: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 0014f9f0: 6c61 7373 2057 6970 6553 6571 7565 6e63  lass WipeSequenc
-0014fa00: 6528 6270 795f 7374 7275 6374 2c20 5365  e(bpy_struct, Se
-0014fa10: 7175 656e 6365 2c20 4566 6665 6374 5365  quence, EffectSe
+0014fa00: 6528 6270 795f 7374 7275 6374 2c20 4566  e(bpy_struct, Ef
+0014fa10: 6665 6374 5365 7175 656e 6365 2c20 5365  fectSequence, Se
 0014fa20: 7175 656e 6365 293a 0a0a 2020 2222 220a  quence):..  """.
 0014fa30: 0a20 2053 6571 7565 6e63 6520 7374 7269  .  Sequence stri
 0014fa40: 7020 6372 6561 7469 6e67 2061 2077 6970  p creating a wip
 0014fa50: 6520 7472 616e 7369 7469 6f6e 0a0a 2020  e transition..  
 0014fa60: 2222 220a 0a20 2061 6e67 6c65 3a20 666c  """..  angle: fl
 0014fa70: 6f61 7420 3d20 2e2e 2e0a 0a20 2022 2222  oat = .....  """
 0014fa80: 0a0a 2020 4564 6765 2061 6e67 6c65 0a0a  ..  Edge angle..
@@ -85963,17 +85963,17 @@
 0014fca0: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 0014fcb0: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 0014fcc0: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 0014fcd0: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 0014fce0: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2043      .....class C
 0014fcf0: 6f6d 706f 7369 746f 724e 6f64 6541 6c70  ompositorNodeAlp
 0014fd00: 6861 4f76 6572 2862 7079 5f73 7472 7563  haOver(bpy_struc
-0014fd10: 742c 2043 6f6d 706f 7369 746f 724e 6f64  t, CompositorNod
-0014fd20: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-0014fd30: 6572 6e61 6c29 3a0a 0a20 2070 7265 6d75  ernal):..  premu
+0014fd10: 742c 204e 6f64 6549 6e74 6572 6e61 6c2c  t, NodeInternal,
+0014fd20: 2043 6f6d 706f 7369 746f 724e 6f64 652c   CompositorNode,
+0014fd30: 204e 6f64 6529 3a0a 0a20 2070 7265 6d75   Node):..  premu
 0014fd40: 6c3a 2066 6c6f 6174 203d 202e 2e2e 0a0a  l: float = .....
 0014fd50: 2020 2222 220a 0a20 204d 6978 2046 6163    """..  Mix Fac
 0014fd60: 746f 720a 0a20 2022 2222 0a0a 2020 7573  tor..  """..  us
 0014fd70: 655f 7072 656d 756c 7469 706c 793a 2062  e_premultiply: b
 0014fd80: 6f6f 6c20 3d20 2e2e 2e0a 0a20 2040 636c  ool = .....  @cl
 0014fd90: 6173 736d 6574 686f 640a 0a20 2064 6566  assmethod..  def
 0014fda0: 2069 735f 7265 6769 7374 6572 6564 5f6e   is_registered_n
@@ -86014,17 +86014,17 @@
 0014ffd0: 5f73 7562 636c 6173 735f 7079 2863 6c73  _subclass_py(cls
 0014ffe0: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 0014fff0: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 00150000: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 00150010: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 00150020: 0a63 6c61 7373 2043 6f6d 706f 7369 746f  .class Composito
 00150030: 724e 6f64 6541 6e74 6941 6c69 6173 696e  rNodeAntiAliasin
-00150040: 6728 6270 795f 7374 7275 6374 2c20 436f  g(bpy_struct, Co
-00150050: 6d70 6f73 6974 6f72 4e6f 6465 2c20 4e6f  mpositorNode, No
-00150060: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+00150040: 6728 6270 795f 7374 7275 6374 2c20 4e6f  g(bpy_struct, No
+00150050: 6465 496e 7465 726e 616c 2c20 436f 6d70  deInternal, Comp
+00150060: 6f73 6974 6f72 4e6f 6465 2c20 4e6f 6465  ositorNode, Node
 00150070: 293a 0a0a 2020 636f 6e74 7261 7374 5f6c  ):..  contrast_l
 00150080: 696d 6974 3a20 666c 6f61 7420 3d20 2e2e  imit: float = ..
 00150090: 2e0a 0a20 2022 2222 0a0a 2020 486f 7720  ...  """..  How 
 001500a0: 6d75 6368 2074 6f20 656c 696d 696e 6174  much to eliminat
 001500b0: 6520 7370 7572 696f 7573 2065 6467 6573  e spurious edges
 001500c0: 2074 6f20 6176 6f69 6420 6172 7469 6661   to avoid artifa
 001500d0: 6374 7320 2874 6865 206c 6172 6765 7220  cts (the larger 
@@ -86092,17 +86092,17 @@
 001504b0: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 001504c0: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 001504d0: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 001504e0: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 001504f0: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2043      .....class C
 00150500: 6f6d 706f 7369 746f 724e 6f64 6542 696c  ompositorNodeBil
 00150510: 6174 6572 616c 626c 7572 2862 7079 5f73  ateralblur(bpy_s
-00150520: 7472 7563 742c 2043 6f6d 706f 7369 746f  truct, Composito
-00150530: 724e 6f64 652c 204e 6f64 652c 204e 6f64  rNode, Node, Nod
-00150540: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2069  eInternal):..  i
+00150520: 7472 7563 742c 204e 6f64 6549 6e74 6572  truct, NodeInter
+00150530: 6e61 6c2c 2043 6f6d 706f 7369 746f 724e  nal, CompositorN
+00150540: 6f64 652c 204e 6f64 6529 3a0a 0a20 2069  ode, Node):..  i
 00150550: 7465 7261 7469 6f6e 733a 2069 6e74 203d  terations: int =
 00150560: 202e 2e2e 0a0a 2020 7369 676d 615f 636f   .....  sigma_co
 00150570: 6c6f 723a 2066 6c6f 6174 203d 202e 2e2e  lor: float = ...
 00150580: 0a0a 2020 7369 676d 615f 7370 6163 653a  ..  sigma_space:
 00150590: 2066 6c6f 6174 203d 202e 2e2e 0a0a 2020   float = .....  
 001505a0: 4063 6c61 7373 6d65 7468 6f64 0a0a 2020  @classmethod..  
 001505b0: 6465 6620 6973 5f72 6567 6973 7465 7265  def is_registere
@@ -86143,17 +86143,17 @@
 001507e0: 6765 745f 7375 6263 6c61 7373 5f70 7928  get_subclass_py(
 001507f0: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 00150800: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 00150810: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 00150820: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 00150830: 2e2e 0a0a 636c 6173 7320 436f 6d70 6f73  ....class Compos
 00150840: 6974 6f72 4e6f 6465 426c 7572 2862 7079  itorNodeBlur(bpy
-00150850: 5f73 7472 7563 742c 2043 6f6d 706f 7369  _struct, Composi
-00150860: 746f 724e 6f64 652c 204e 6f64 652c 204e  torNode, Node, N
-00150870: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+00150850: 5f73 7472 7563 742c 204e 6f64 6549 6e74  _struct, NodeInt
+00150860: 6572 6e61 6c2c 2043 6f6d 706f 7369 746f  ernal, Composito
+00150870: 724e 6f64 652c 204e 6f64 6529 3a0a 0a20  rNode, Node):.. 
 00150880: 2061 7370 6563 745f 636f 7272 6563 7469   aspect_correcti
 00150890: 6f6e 3a20 7374 7220 3d20 2e2e 2e0a 0a20  on: str = ..... 
 001508a0: 2022 2222 0a0a 2020 5479 7065 206f 6620   """..  Type of 
 001508b0: 6173 7065 6374 2063 6f72 7265 6374 696f  aspect correctio
 001508c0: 6e20 746f 2075 7365 0a0a 2020 2222 220a  n to use..  """.
 001508d0: 0a20 2066 6163 746f 723a 2066 6c6f 6174  .  factor: float
 001508e0: 203d 202e 2e2e 0a0a 2020 6661 6374 6f72   = .....  factor
@@ -86234,17 +86234,17 @@
 00150d90: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 00150da0: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 00150db0: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 00150dc0: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 00150dd0: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 00150de0: 7373 2043 6f6d 706f 7369 746f 724e 6f64  ss CompositorNod
 00150df0: 6542 6f6b 6568 426c 7572 2862 7079 5f73  eBokehBlur(bpy_s
-00150e00: 7472 7563 742c 2043 6f6d 706f 7369 746f  truct, Composito
-00150e10: 724e 6f64 652c 204e 6f64 652c 204e 6f64  rNode, Node, Nod
-00150e20: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2062  eInternal):..  b
+00150e00: 7472 7563 742c 204e 6f64 6549 6e74 6572  truct, NodeInter
+00150e10: 6e61 6c2c 2043 6f6d 706f 7369 746f 724e  nal, CompositorN
+00150e20: 6f64 652c 204e 6f64 6529 3a0a 0a20 2062  ode, Node):..  b
 00150e30: 6c75 725f 6d61 783a 2066 6c6f 6174 203d  lur_max: float =
 00150e40: 202e 2e2e 0a0a 2020 2222 220a 0a20 2042   .....  """..  B
 00150e50: 6c75 7220 6c69 6d69 742c 206d 6178 696d  lur limit, maxim
 00150e60: 756d 2043 6f43 2072 6164 6975 730a 0a20  um CoC radius.. 
 00150e70: 2022 2222 0a0a 2020 7573 655f 6578 7465   """..  use_exte
 00150e80: 6e64 6564 5f62 6f75 6e64 733a 2062 6f6f  nded_bounds: boo
 00150e90: 6c20 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  l = .....  """..
@@ -86299,17 +86299,17 @@
 001511a0: 5f73 7562 636c 6173 735f 7079 2863 6c73  _subclass_py(cls
 001511b0: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 001511c0: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 001511d0: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 001511e0: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 001511f0: 0a63 6c61 7373 2043 6f6d 706f 7369 746f  .class Composito
 00151200: 724e 6f64 6542 6f6b 6568 496d 6167 6528  rNodeBokehImage(
-00151210: 6270 795f 7374 7275 6374 2c20 436f 6d70  bpy_struct, Comp
-00151220: 6f73 6974 6f72 4e6f 6465 2c20 4e6f 6465  ositorNode, Node
-00151230: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+00151210: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+00151220: 496e 7465 726e 616c 2c20 436f 6d70 6f73  Internal, Compos
+00151230: 6974 6f72 4e6f 6465 2c20 4e6f 6465 293a  itorNode, Node):
 00151240: 0a0a 2020 616e 676c 653a 2066 6c6f 6174  ..  angle: float
 00151250: 203d 202e 2e2e 0a0a 2020 2222 220a 0a20   = .....  """.. 
 00151260: 2041 6e67 6c65 206f 6620 7468 6520 626f   Angle of the bo
 00151270: 6b65 680a 0a20 2022 2222 0a0a 2020 6361  keh..  """..  ca
 00151280: 7461 6469 6f70 7472 6963 3a20 666c 6f61  tadioptric: floa
 00151290: 7420 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  t = .....  """..
 001512a0: 2020 4c65 7665 6c20 6f66 2063 6174 6164    Level of catad
@@ -86366,17 +86366,17 @@
 001515d0: 5f67 6574 5f73 7562 636c 6173 735f 7079  _get_subclass_py
 001515e0: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 001515f0: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 00151600: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 00151610: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 00151620: 2e2e 2e0a 0a63 6c61 7373 2043 6f6d 706f  .....class Compo
 00151630: 7369 746f 724e 6f64 6542 6f78 4d61 736b  sitorNodeBoxMask
-00151640: 2862 7079 5f73 7472 7563 742c 2043 6f6d  (bpy_struct, Com
-00151650: 706f 7369 746f 724e 6f64 652c 204e 6f64  positorNode, Nod
-00151660: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+00151640: 2862 7079 5f73 7472 7563 742c 204e 6f64  (bpy_struct, Nod
+00151650: 6549 6e74 6572 6e61 6c2c 2043 6f6d 706f  eInternal, Compo
+00151660: 7369 746f 724e 6f64 652c 204e 6f64 6529  sitorNode, Node)
 00151670: 3a0a 0a20 2068 6569 6768 743a 2066 6c6f  :..  height: flo
 00151680: 6174 203d 202e 2e2e 0a0a 2020 2222 220a  at = .....  """.
 00151690: 0a20 2048 6569 6768 7420 6f66 2074 6865  .  Height of the
 001516a0: 2062 6f78 0a0a 2020 2222 220a 0a20 206d   box..  """..  m
 001516b0: 6173 6b5f 7479 7065 3a20 7374 7220 3d20  ask_type: str = 
 001516c0: 2e2e 2e0a 0a20 2072 6f74 6174 696f 6e3a  .....  rotation:
 001516d0: 2066 6c6f 6174 203d 202e 2e2e 0a0a 2020   float = .....  
@@ -86435,17 +86435,17 @@
 00151a20: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 00151a30: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 00151a40: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 00151a50: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 00151a60: 2e2e 2e0a 0a63 6c61 7373 2043 6f6d 706f  .....class Compo
 00151a70: 7369 746f 724e 6f64 6542 7269 6768 7443  sitorNodeBrightC
 00151a80: 6f6e 7472 6173 7428 6270 795f 7374 7275  ontrast(bpy_stru
-00151a90: 6374 2c20 436f 6d70 6f73 6974 6f72 4e6f  ct, CompositorNo
-00151aa0: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-00151ab0: 7465 726e 616c 293a 0a0a 2020 7573 655f  ternal):..  use_
+00151a90: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+00151aa0: 2c20 436f 6d70 6f73 6974 6f72 4e6f 6465  , CompositorNode
+00151ab0: 2c20 4e6f 6465 293a 0a0a 2020 7573 655f  , Node):..  use_
 00151ac0: 7072 656d 756c 7469 706c 793a 2062 6f6f  premultiply: boo
 00151ad0: 6c20 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  l = .....  """..
 00151ae0: 2020 4b65 6570 206f 7574 7075 7420 696d    Keep output im
 00151af0: 6167 6520 7072 656d 756c 7469 706c 6965  age premultiplie
 00151b00: 6420 616c 7068 610a 0a20 2022 2222 0a0a  d alpha..  """..
 00151b10: 2020 4063 6c61 7373 6d65 7468 6f64 0a0a    @classmethod..
 00151b20: 2020 6465 6620 6973 5f72 6567 6973 7465    def is_registe
@@ -86487,17 +86487,17 @@
 00151d60: 7928 636c 732c 2069 643a 2073 7472 2c20  y(cls, id: str, 
 00151d70: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 00151d80: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 00151d90: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 00151da0: 202e 2e2e 0a0a 636c 6173 7320 436f 6d70   .....class Comp
 00151db0: 6f73 6974 6f72 4e6f 6465 4368 616e 6e65  ositorNodeChanne
 00151dc0: 6c4d 6174 7465 2862 7079 5f73 7472 7563  lMatte(bpy_struc
-00151dd0: 742c 2043 6f6d 706f 7369 746f 724e 6f64  t, CompositorNod
-00151de0: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-00151df0: 6572 6e61 6c29 3a0a 0a20 2063 6f6c 6f72  ernal):..  color
+00151dd0: 742c 204e 6f64 6549 6e74 6572 6e61 6c2c  t, NodeInternal,
+00151de0: 2043 6f6d 706f 7369 746f 724e 6f64 652c   CompositorNode,
+00151df0: 204e 6f64 6529 3a0a 0a20 2063 6f6c 6f72   Node):..  color
 00151e00: 5f73 7061 6365 3a20 7374 7220 3d20 2e2e  _space: str = ..
 00151e10: 2e0a 0a20 2022 2222 0a0a 2020 2a20 6060  ...  """..  * ``
 00151e20: 5247 4260 600a 5247 4220 2d2d 2052 4742  RGB``.RGB -- RGB
 00151e30: 2063 6f6c 6f72 2073 7061 6365 2e0a 0a20   color space... 
 00151e40: 202a 2060 6048 5356 6060 0a48 5356 202d   * ``HSV``.HSV -
 00151e50: 2d20 4853 5620 636f 6c6f 7220 7370 6163  - HSV color spac
 00151e60: 652e 0a0a 2020 2a20 6060 5955 5660 600a  e...  * ``YUV``.
@@ -86586,17 +86586,17 @@
 00152390: 5f70 7928 636c 732c 2069 643a 2073 7472  _py(cls, id: str
 001523a0: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 001523b0: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 001523c0: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 001523d0: 2020 202e 2e2e 0a0a 636c 6173 7320 436f     .....class Co
 001523e0: 6d70 6f73 6974 6f72 4e6f 6465 4368 726f  mpositorNodeChro
 001523f0: 6d61 4d61 7474 6528 6270 795f 7374 7275  maMatte(bpy_stru
-00152400: 6374 2c20 436f 6d70 6f73 6974 6f72 4e6f  ct, CompositorNo
-00152410: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-00152420: 7465 726e 616c 293a 0a0a 2020 6761 696e  ternal):..  gain
+00152400: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+00152410: 2c20 436f 6d70 6f73 6974 6f72 4e6f 6465  , CompositorNode
+00152420: 2c20 4e6f 6465 293a 0a0a 2020 6761 696e  , Node):..  gain
 00152430: 3a20 666c 6f61 7420 3d20 2e2e 2e0a 0a20  : float = ..... 
 00152440: 2022 2222 0a0a 2020 416c 7068 6120 6661   """..  Alpha fa
 00152450: 6c6c 6f66 660a 0a20 2022 2222 0a0a 2020  lloff..  """..  
 00152460: 6c69 6674 3a20 666c 6f61 7420 3d20 2e2e  lift: float = ..
 00152470: 2e0a 0a20 2022 2222 0a0a 2020 416c 7068  ...  """..  Alph
 00152480: 6120 6c69 6674 0a0a 2020 2222 220a 0a20  a lift..  """.. 
 00152490: 2073 6861 646f 775f 6164 6a75 7374 3a20   shadow_adjust: 
@@ -86657,17 +86657,17 @@
 00152800: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 00152810: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 00152820: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 00152830: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 00152840: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 00152850: 636c 6173 7320 436f 6d70 6f73 6974 6f72  class Compositor
 00152860: 4e6f 6465 436f 6c6f 7242 616c 616e 6365  NodeColorBalance
-00152870: 2862 7079 5f73 7472 7563 742c 2043 6f6d  (bpy_struct, Com
-00152880: 706f 7369 746f 724e 6f64 652c 204e 6f64  positorNode, Nod
-00152890: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+00152870: 2862 7079 5f73 7472 7563 742c 204e 6f64  (bpy_struct, Nod
+00152880: 6549 6e74 6572 6e61 6c2c 2043 6f6d 706f  eInternal, Compo
+00152890: 7369 746f 724e 6f64 652c 204e 6f64 6529  sitorNode, Node)
 001528a0: 3a0a 0a20 2063 6f72 7265 6374 696f 6e5f  :..  correction_
 001528b0: 6d65 7468 6f64 3a20 7374 7220 3d20 2e2e  method: str = ..
 001528c0: 2e0a 0a20 2022 2222 0a0a 2020 2a20 6060  ...  """..  * ``
 001528d0: 4c49 4654 5f47 414d 4d41 5f47 4149 4e60  LIFT_GAMMA_GAIN`
 001528e0: 600a 4c69 6674 2f47 616d 6d61 2f47 6169  `.Lift/Gamma/Gai
 001528f0: 6e2e 0a0a 2020 2a20 6060 4f46 4653 4554  n...  * ``OFFSET
 00152900: 5f50 4f57 4552 5f53 4c4f 5045 6060 0a4f  _POWER_SLOPE``.O
@@ -86750,17 +86750,17 @@
 00152dd0: 7928 636c 732c 2069 643a 2073 7472 2c20  y(cls, id: str, 
 00152de0: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 00152df0: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 00152e00: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 00152e10: 202e 2e2e 0a0a 636c 6173 7320 436f 6d70   .....class Comp
 00152e20: 6f73 6974 6f72 4e6f 6465 436f 6c6f 7243  ositorNodeColorC
 00152e30: 6f72 7265 6374 696f 6e28 6270 795f 7374  orrection(bpy_st
-00152e40: 7275 6374 2c20 436f 6d70 6f73 6974 6f72  ruct, Compositor
-00152e50: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-00152e60: 496e 7465 726e 616c 293a 0a0a 2020 626c  Internal):..  bl
+00152e40: 7275 6374 2c20 4e6f 6465 496e 7465 726e  ruct, NodeIntern
+00152e50: 616c 2c20 436f 6d70 6f73 6974 6f72 4e6f  al, CompositorNo
+00152e60: 6465 2c20 4e6f 6465 293a 0a0a 2020 626c  de, Node):..  bl
 00152e70: 7565 3a20 626f 6f6c 203d 202e 2e2e 0a0a  ue: bool = .....
 00152e80: 2020 2222 220a 0a20 2042 6c75 6520 6368    """..  Blue ch
 00152e90: 616e 6e65 6c20 6163 7469 7665 0a0a 2020  annel active..  
 00152ea0: 2222 220a 0a20 2067 7265 656e 3a20 626f  """..  green: bo
 00152eb0: 6f6c 203d 202e 2e2e 0a0a 2020 2222 220a  ol = .....  """.
 00152ec0: 0a20 2047 7265 656e 2063 6861 6e6e 656c  .  Green channel
 00152ed0: 2061 6374 6976 650a 0a20 2022 2222 0a0a   active..  """..
@@ -86896,17 +86896,17 @@
 001536f0: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 00153700: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 00153710: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 00153720: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 00153730: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 00153740: 6c61 7373 2043 6f6d 706f 7369 746f 724e  lass CompositorN
 00153750: 6f64 6543 6f6c 6f72 4d61 7474 6528 6270  odeColorMatte(bp
-00153760: 795f 7374 7275 6374 2c20 436f 6d70 6f73  y_struct, Compos
-00153770: 6974 6f72 4e6f 6465 2c20 4e6f 6465 2c20  itorNode, Node, 
-00153780: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+00153760: 795f 7374 7275 6374 2c20 4e6f 6465 496e  y_struct, NodeIn
+00153770: 7465 726e 616c 2c20 436f 6d70 6f73 6974  ternal, Composit
+00153780: 6f72 4e6f 6465 2c20 4e6f 6465 293a 0a0a  orNode, Node):..
 00153790: 2020 636f 6c6f 725f 6875 653a 2066 6c6f    color_hue: flo
 001537a0: 6174 203d 202e 2e2e 0a0a 2020 2222 220a  at = .....  """.
 001537b0: 0a20 2048 7565 2074 6f6c 6572 616e 6365  .  Hue tolerance
 001537c0: 2066 6f72 2063 6f6c 6f72 7320 746f 2062   for colors to b
 001537d0: 6520 636f 6e73 6964 6572 6564 2061 206b  e considered a k
 001537e0: 6579 696e 6720 636f 6c6f 720a 0a20 2022  eying color..  "
 001537f0: 2222 0a0a 2020 636f 6c6f 725f 7361 7475  ""..  color_satu
@@ -86959,17 +86959,17 @@
 00153ae0: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 00153af0: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 00153b00: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 00153b10: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 00153b20: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 00153b30: 436f 6d70 6f73 6974 6f72 4e6f 6465 436f  CompositorNodeCo
 00153b40: 6c6f 7253 7069 6c6c 2862 7079 5f73 7472  lorSpill(bpy_str
-00153b50: 7563 742c 2043 6f6d 706f 7369 746f 724e  uct, CompositorN
-00153b60: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-00153b70: 6e74 6572 6e61 6c29 3a0a 0a20 2063 6861  nternal):..  cha
+00153b50: 7563 742c 204e 6f64 6549 6e74 6572 6e61  uct, NodeInterna
+00153b60: 6c2c 2043 6f6d 706f 7369 746f 724e 6f64  l, CompositorNod
+00153b70: 652c 204e 6f64 6529 3a0a 0a20 2063 6861  e, Node):..  cha
 00153b80: 6e6e 656c 3a20 7374 7220 3d20 2e2e 2e0a  nnel: str = ....
 00153b90: 0a20 2022 2222 0a0a 2020 2a20 6060 5260  .  """..  * ``R`
 00153ba0: 600a 5220 2d2d 2052 6564 2073 7069 6c6c  `.R -- Red spill
 00153bb0: 2073 7570 7072 6573 7369 6f6e 2e0a 0a20   suppression... 
 00153bc0: 202a 2060 6047 6060 0a47 202d 2d20 4772   * ``G``.G -- Gr
 00153bd0: 6565 6e20 7370 696c 6c20 7375 7070 7265  een spill suppre
 00153be0: 7373 696f 6e2e 0a0a 2020 2a20 6060 4260  ssion...  * ``B`
@@ -87054,17 +87054,17 @@
 001540d0: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 001540e0: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 001540f0: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 00154100: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 00154110: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 00154120: 636c 6173 7320 436f 6d70 6f73 6974 6f72  class Compositor
 00154130: 4e6f 6465 436f 6d62 4853 5641 2862 7079  NodeCombHSVA(bpy
-00154140: 5f73 7472 7563 742c 2043 6f6d 706f 7369  _struct, Composi
-00154150: 746f 724e 6f64 652c 204e 6f64 652c 204e  torNode, Node, N
-00154160: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+00154140: 5f73 7472 7563 742c 204e 6f64 6549 6e74  _struct, NodeInt
+00154150: 6572 6e61 6c2c 2043 6f6d 706f 7369 746f  ernal, Composito
+00154160: 724e 6f64 652c 204e 6f64 6529 3a0a 0a20  rNode, Node):.. 
 00154170: 2040 636c 6173 736d 6574 686f 640a 0a20   @classmethod.. 
 00154180: 2064 6566 2069 735f 7265 6769 7374 6572   def is_register
 00154190: 6564 5f6e 6f64 655f 7479 7065 2863 6c73  ed_node_type(cls
 001541a0: 2920 2d3e 2062 6f6f 6c3a 0a0a 2020 2020  ) -> bool:..    
 001541b0: 2222 220a 0a20 2020 2054 7275 6520 6966  """..    True if
 001541c0: 2061 2072 6567 6973 7465 7265 6420 6e6f   a registered no
 001541d0: 6465 2074 7970 650a 0a20 2020 2022 2222  de type..    """
@@ -87100,17 +87100,17 @@
 001543b0: 5f67 6574 5f73 7562 636c 6173 735f 7079  _get_subclass_py
 001543c0: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 001543d0: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 001543e0: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 001543f0: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 00154400: 2e2e 2e0a 0a63 6c61 7373 2043 6f6d 706f  .....class Compo
 00154410: 7369 746f 724e 6f64 6543 6f6d 6252 4742  sitorNodeCombRGB
-00154420: 4128 6270 795f 7374 7275 6374 2c20 436f  A(bpy_struct, Co
-00154430: 6d70 6f73 6974 6f72 4e6f 6465 2c20 4e6f  mpositorNode, No
-00154440: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+00154420: 4128 6270 795f 7374 7275 6374 2c20 4e6f  A(bpy_struct, No
+00154430: 6465 496e 7465 726e 616c 2c20 436f 6d70  deInternal, Comp
+00154440: 6f73 6974 6f72 4e6f 6465 2c20 4e6f 6465  ositorNode, Node
 00154450: 293a 0a0a 2020 4063 6c61 7373 6d65 7468  ):..  @classmeth
 00154460: 6f64 0a0a 2020 6465 6620 6973 5f72 6567  od..  def is_reg
 00154470: 6973 7465 7265 645f 6e6f 6465 5f74 7970  istered_node_typ
 00154480: 6528 636c 7329 202d 3e20 626f 6f6c 3a0a  e(cls) -> bool:.
 00154490: 0a20 2020 2022 2222 0a0a 2020 2020 5472  .    """..    Tr
 001544a0: 7565 2069 6620 6120 7265 6769 7374 6572  ue if a register
 001544b0: 6564 206e 6f64 6520 7479 7065 0a0a 2020  ed node type..  
@@ -87147,17 +87147,17 @@
 001546a0: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 001546b0: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 001546c0: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 001546d0: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 001546e0: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 001546f0: 436f 6d70 6f73 6974 6f72 4e6f 6465 436f  CompositorNodeCo
 00154700: 6d62 5943 4341 2862 7079 5f73 7472 7563  mbYCCA(bpy_struc
-00154710: 742c 2043 6f6d 706f 7369 746f 724e 6f64  t, CompositorNod
-00154720: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-00154730: 6572 6e61 6c29 3a0a 0a20 206d 6f64 653a  ernal):..  mode:
+00154710: 742c 204e 6f64 6549 6e74 6572 6e61 6c2c  t, NodeInternal,
+00154720: 2043 6f6d 706f 7369 746f 724e 6f64 652c   CompositorNode,
+00154730: 204e 6f64 6529 3a0a 0a20 206d 6f64 653a   Node):..  mode:
 00154740: 2073 7472 203d 202e 2e2e 0a0a 2020 4063   str = .....  @c
 00154750: 6c61 7373 6d65 7468 6f64 0a0a 2020 6465  lassmethod..  de
 00154760: 6620 6973 5f72 6567 6973 7465 7265 645f  f is_registered_
 00154770: 6e6f 6465 5f74 7970 6528 636c 7329 202d  node_type(cls) -
 00154780: 3e20 626f 6f6c 3a0a 0a20 2020 2022 2222  > bool:..    """
 00154790: 0a0a 2020 2020 5472 7565 2069 6620 6120  ..    True if a 
 001547a0: 7265 6769 7374 6572 6564 206e 6f64 6520  registered node 
@@ -87194,17 +87194,17 @@
 00154990: 745f 7375 6263 6c61 7373 5f70 7928 636c  t_subclass_py(cl
 001549a0: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 001549b0: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 001549c0: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 001549d0: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 001549e0: 0a0a 636c 6173 7320 436f 6d70 6f73 6974  ..class Composit
 001549f0: 6f72 4e6f 6465 436f 6d62 5955 5641 2862  orNodeCombYUVA(b
-00154a00: 7079 5f73 7472 7563 742c 2043 6f6d 706f  py_struct, Compo
-00154a10: 7369 746f 724e 6f64 652c 204e 6f64 652c  sitorNode, Node,
-00154a20: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+00154a00: 7079 5f73 7472 7563 742c 204e 6f64 6549  py_struct, NodeI
+00154a10: 6e74 6572 6e61 6c2c 2043 6f6d 706f 7369  nternal, Composi
+00154a20: 746f 724e 6f64 652c 204e 6f64 6529 3a0a  torNode, Node):.
 00154a30: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
 00154a40: 0a20 2064 6566 2069 735f 7265 6769 7374  .  def is_regist
 00154a50: 6572 6564 5f6e 6f64 655f 7479 7065 2863  ered_node_type(c
 00154a60: 6c73 2920 2d3e 2062 6f6f 6c3a 0a0a 2020  ls) -> bool:..  
 00154a70: 2020 2222 220a 0a20 2020 2054 7275 6520    """..    True 
 00154a80: 6966 2061 2072 6567 6973 7465 7265 6420  if a registered 
 00154a90: 6e6f 6465 2074 7970 650a 0a20 2020 2022  node type..    "
@@ -87241,17 +87241,17 @@
 00154c80: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 00154c90: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 00154ca0: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 00154cb0: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 00154cc0: 2020 2e2e 2e0a 0a63 6c61 7373 2043 6f6d    .....class Com
 00154cd0: 706f 7369 746f 724e 6f64 6543 6f6d 6269  positorNodeCombi
 00154ce0: 6e65 436f 6c6f 7228 6270 795f 7374 7275  neColor(bpy_stru
-00154cf0: 6374 2c20 436f 6d70 6f73 6974 6f72 4e6f  ct, CompositorNo
-00154d00: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-00154d10: 7465 726e 616c 293a 0a0a 2020 6d6f 6465  ternal):..  mode
+00154cf0: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+00154d00: 2c20 436f 6d70 6f73 6974 6f72 4e6f 6465  , CompositorNode
+00154d10: 2c20 4e6f 6465 293a 0a0a 2020 6d6f 6465  , Node):..  mode
 00154d20: 3a20 7374 7220 3d20 2e2e 2e0a 0a20 2022  : str = .....  "
 00154d30: 2222 0a0a 2020 4d6f 6465 206f 6620 636f  ""..  Mode of co
 00154d40: 6c6f 7220 7072 6f63 6573 7369 6e67 0a0a  lor processing..
 00154d50: 2020 2a20 6060 5247 4260 600a 5247 4220    * ``RGB``.RGB 
 00154d60: 2d2d 2055 7365 2052 4742 2063 6f6c 6f72  -- Use RGB color
 00154d70: 2070 726f 6365 7373 696e 672e 0a0a 2020   processing...  
 00154d80: 2a20 6060 4853 5660 600a 4853 5620 2d2d  * ``HSV``.HSV --
@@ -87311,17 +87311,17 @@
 001550e0: 7928 636c 732c 2069 643a 2073 7472 2c20  y(cls, id: str, 
 001550f0: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 00155100: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 00155110: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 00155120: 202e 2e2e 0a0a 636c 6173 7320 436f 6d70   .....class Comp
 00155130: 6f73 6974 6f72 4e6f 6465 436f 6d62 696e  ositorNodeCombin
 00155140: 6558 595a 2862 7079 5f73 7472 7563 742c  eXYZ(bpy_struct,
-00155150: 2043 6f6d 706f 7369 746f 724e 6f64 652c   CompositorNode,
-00155160: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-00155170: 6e61 6c29 3a0a 0a20 2040 636c 6173 736d  nal):..  @classm
+00155150: 204e 6f64 6549 6e74 6572 6e61 6c2c 2043   NodeInternal, C
+00155160: 6f6d 706f 7369 746f 724e 6f64 652c 204e  ompositorNode, N
+00155170: 6f64 6529 3a0a 0a20 2040 636c 6173 736d  ode):..  @classm
 00155180: 6574 686f 640a 0a20 2064 6566 2069 735f  ethod..  def is_
 00155190: 7265 6769 7374 6572 6564 5f6e 6f64 655f  registered_node_
 001551a0: 7479 7065 2863 6c73 2920 2d3e 2062 6f6f  type(cls) -> boo
 001551b0: 6c3a 0a0a 2020 2020 2222 220a 0a20 2020  l:..    """..   
 001551c0: 2054 7275 6520 6966 2061 2072 6567 6973   True if a regis
 001551d0: 7465 7265 6420 6e6f 6465 2074 7970 650a  tered node type.
 001551e0: 0a20 2020 2022 2222 0a0a 2020 2020 2e2e  .    """..    ..
@@ -87357,17 +87357,17 @@
 001553c0: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 001553d0: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 001553e0: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 001553f0: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 00155400: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 00155410: 7373 2043 6f6d 706f 7369 746f 724e 6f64  ss CompositorNod
 00155420: 6543 6f6d 706f 7369 7465 2862 7079 5f73  eComposite(bpy_s
-00155430: 7472 7563 742c 2043 6f6d 706f 7369 746f  truct, Composito
-00155440: 724e 6f64 652c 204e 6f64 652c 204e 6f64  rNode, Node, Nod
-00155450: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2075  eInternal):..  u
+00155430: 7472 7563 742c 204e 6f64 6549 6e74 6572  truct, NodeInter
+00155440: 6e61 6c2c 2043 6f6d 706f 7369 746f 724e  nal, CompositorN
+00155450: 6f64 652c 204e 6f64 6529 3a0a 0a20 2075  ode, Node):..  u
 00155460: 7365 5f61 6c70 6861 3a20 626f 6f6c 203d  se_alpha: bool =
 00155470: 202e 2e2e 0a0a 2020 2222 220a 0a20 2043   .....  """..  C
 00155480: 6f6c 6f72 7320 6172 6520 7472 6561 7465  olors are treate
 00155490: 6420 616c 7068 6120 7072 656d 756c 7469  d alpha premulti
 001554a0: 706c 6965 642c 206f 7220 636f 6c6f 7273  plied, or colors
 001554b0: 206f 7574 7075 7420 7374 7261 6967 6874   output straight
 001554c0: 2028 616c 7068 6120 6765 7473 2073 6574   (alpha gets set
@@ -87412,17 +87412,17 @@
 00155730: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 00155740: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 00155750: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 00155760: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 00155770: 2e2e 2e0a 0a63 6c61 7373 2043 6f6d 706f  .....class Compo
 00155780: 7369 746f 724e 6f64 6543 6f6e 7665 7274  sitorNodeConvert
 00155790: 436f 6c6f 7253 7061 6365 2862 7079 5f73  ColorSpace(bpy_s
-001557a0: 7472 7563 742c 2043 6f6d 706f 7369 746f  truct, Composito
-001557b0: 724e 6f64 652c 204e 6f64 652c 204e 6f64  rNode, Node, Nod
-001557c0: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2066  eInternal):..  f
+001557a0: 7472 7563 742c 204e 6f64 6549 6e74 6572  truct, NodeInter
+001557b0: 6e61 6c2c 2043 6f6d 706f 7369 746f 724e  nal, CompositorN
+001557c0: 6f64 652c 204e 6f64 6529 3a0a 0a20 2066  ode, Node):..  f
 001557d0: 726f 6d5f 636f 6c6f 725f 7370 6163 653a  rom_color_space:
 001557e0: 2073 7472 203d 202e 2e2e 0a0a 2020 2222   str = .....  ""
 001557f0: 220a 0a20 2043 6f6c 6f72 2073 7061 6365  "..  Color space
 00155800: 206f 6620 7468 6520 696e 7075 7420 696d   of the input im
 00155810: 6167 650a 0a20 2022 2222 0a0a 2020 746f  age..  """..  to
 00155820: 5f63 6f6c 6f72 5f73 7061 6365 3a20 7374  _color_space: st
 00155830: 7220 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  r = .....  """..
@@ -87468,17 +87468,17 @@
 00155ab0: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 00155ac0: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 00155ad0: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 00155ae0: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 00155af0: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 00155b00: 636c 6173 7320 436f 6d70 6f73 6974 6f72  class Compositor
 00155b10: 4e6f 6465 436f 726e 6572 5069 6e28 6270  NodeCornerPin(bp
-00155b20: 795f 7374 7275 6374 2c20 436f 6d70 6f73  y_struct, Compos
-00155b30: 6974 6f72 4e6f 6465 2c20 4e6f 6465 2c20  itorNode, Node, 
-00155b40: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+00155b20: 795f 7374 7275 6374 2c20 4e6f 6465 496e  y_struct, NodeIn
+00155b30: 7465 726e 616c 2c20 436f 6d70 6f73 6974  ternal, Composit
+00155b40: 6f72 4e6f 6465 2c20 4e6f 6465 293a 0a0a  orNode, Node):..
 00155b50: 2020 4063 6c61 7373 6d65 7468 6f64 0a0a    @classmethod..
 00155b60: 2020 6465 6620 6973 5f72 6567 6973 7465    def is_registe
 00155b70: 7265 645f 6e6f 6465 5f74 7970 6528 636c  red_node_type(cl
 00155b80: 7329 202d 3e20 626f 6f6c 3a0a 0a20 2020  s) -> bool:..   
 00155b90: 2022 2222 0a0a 2020 2020 5472 7565 2069   """..    True i
 00155ba0: 6620 6120 7265 6769 7374 6572 6564 206e  f a registered n
 00155bb0: 6f64 6520 7479 7065 0a0a 2020 2020 2222  ode type..    ""
@@ -87514,17 +87514,17 @@
 00155d90: 615f 6765 745f 7375 6263 6c61 7373 5f70  a_get_subclass_p
 00155da0: 7928 636c 732c 2069 643a 2073 7472 2c20  y(cls, id: str, 
 00155db0: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 00155dc0: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 00155dd0: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 00155de0: 202e 2e2e 0a0a 636c 6173 7320 436f 6d70   .....class Comp
 00155df0: 6f73 6974 6f72 4e6f 6465 4372 6f70 2862  ositorNodeCrop(b
-00155e00: 7079 5f73 7472 7563 742c 2043 6f6d 706f  py_struct, Compo
-00155e10: 7369 746f 724e 6f64 652c 204e 6f64 652c  sitorNode, Node,
-00155e20: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+00155e00: 7079 5f73 7472 7563 742c 204e 6f64 6549  py_struct, NodeI
+00155e10: 6e74 6572 6e61 6c2c 2043 6f6d 706f 7369  nternal, Composi
+00155e20: 746f 724e 6f64 652c 204e 6f64 6529 3a0a  torNode, Node):.
 00155e30: 0a20 206d 6178 5f78 3a20 696e 7420 3d20  .  max_x: int = 
 00155e40: 2e2e 2e0a 0a20 206d 6178 5f79 3a20 696e  .....  max_y: in
 00155e50: 7420 3d20 2e2e 2e0a 0a20 206d 696e 5f78  t = .....  min_x
 00155e60: 3a20 696e 7420 3d20 2e2e 2e0a 0a20 206d  : int = .....  m
 00155e70: 696e 5f79 3a20 696e 7420 3d20 2e2e 2e0a  in_y: int = ....
 00155e80: 0a20 2072 656c 5f6d 6178 5f78 3a20 666c  .  rel_max_x: fl
 00155e90: 6f61 7420 3d20 2e2e 2e0a 0a20 2072 656c  oat = .....  rel
@@ -87583,17 +87583,17 @@
 001561e0: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 001561f0: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 00156200: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 00156210: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 00156220: 2e2e 0a0a 636c 6173 7320 436f 6d70 6f73  ....class Compos
 00156230: 6974 6f72 4e6f 6465 4372 7970 746f 6d61  itorNodeCryptoma
 00156240: 7474 6528 6270 795f 7374 7275 6374 2c20  tte(bpy_struct, 
-00156250: 436f 6d70 6f73 6974 6f72 4e6f 6465 2c20  CompositorNode, 
-00156260: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-00156270: 616c 293a 0a0a 2020 6164 643a 206d 6174  al):..  add: mat
+00156250: 4e6f 6465 496e 7465 726e 616c 2c20 436f  NodeInternal, Co
+00156260: 6d70 6f73 6974 6f72 4e6f 6465 2c20 4e6f  mpositorNode, No
+00156270: 6465 293a 0a0a 2020 6164 643a 206d 6174  de):..  add: mat
 00156280: 6875 7469 6c73 2e43 6f6c 6f72 203d 202e  hutils.Color = .
 00156290: 2e2e 0a0a 2020 2222 220a 0a20 2041 6464  ....  """..  Add
 001562a0: 206f 626a 6563 7420 6f72 206d 6174 6572   object or mater
 001562b0: 6961 6c20 746f 206d 6174 7465 2c20 6279  ial to matte, by
 001562c0: 2070 6963 6b69 6e67 2061 2063 6f6c 6f72   picking a color
 001562d0: 2066 726f 6d20 7468 6520 5069 636b 206f   from the Pick o
 001562e0: 7574 7075 740a 0a20 2022 2222 0a0a 2020  utput..  """..  
@@ -87651,17 +87651,17 @@
 00156620: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 00156630: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 00156640: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 00156650: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 00156660: 2020 2e2e 2e0a 0a63 6c61 7373 2043 6f6d    .....class Com
 00156670: 706f 7369 746f 724e 6f64 6543 7279 7074  positorNodeCrypt
 00156680: 6f6d 6174 7465 5632 2862 7079 5f73 7472  omatteV2(bpy_str
-00156690: 7563 742c 2043 6f6d 706f 7369 746f 724e  uct, CompositorN
-001566a0: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-001566b0: 6e74 6572 6e61 6c29 3a0a 0a20 2061 6464  nternal):..  add
+00156690: 7563 742c 204e 6f64 6549 6e74 6572 6e61  uct, NodeInterna
+001566a0: 6c2c 2043 6f6d 706f 7369 746f 724e 6f64  l, CompositorNod
+001566b0: 652c 204e 6f64 6529 3a0a 0a20 2061 6464  e, Node):..  add
 001566c0: 3a20 6d61 7468 7574 696c 732e 436f 6c6f  : mathutils.Colo
 001566d0: 7220 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  r = .....  """..
 001566e0: 2020 4164 6420 6f62 6a65 6374 206f 7220    Add object or 
 001566f0: 6d61 7465 7269 616c 2074 6f20 6d61 7474  material to matt
 00156700: 652c 2062 7920 7069 636b 696e 6720 6120  e, by picking a 
 00156710: 636f 6c6f 7220 6672 6f6d 2074 6865 2050  color from the P
 00156720: 6963 6b20 6f75 7470 7574 0a0a 2020 2222  ick output..  ""
@@ -87798,17 +87798,17 @@
 00156f50: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 00156f60: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 00156f70: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 00156f80: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 00156f90: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 00156fa0: 6173 7320 436f 6d70 6f73 6974 6f72 4e6f  ass CompositorNo
 00156fb0: 6465 4375 7276 6552 4742 2862 7079 5f73  deCurveRGB(bpy_s
-00156fc0: 7472 7563 742c 2043 6f6d 706f 7369 746f  truct, Composito
-00156fd0: 724e 6f64 652c 204e 6f64 652c 204e 6f64  rNode, Node, Nod
-00156fe0: 6549 6e74 6572 6e61 6c29 3a0a 0a20 206d  eInternal):..  m
+00156fc0: 7472 7563 742c 204e 6f64 6549 6e74 6572  truct, NodeInter
+00156fd0: 6e61 6c2c 2043 6f6d 706f 7369 746f 724e  nal, CompositorN
+00156fe0: 6f64 652c 204e 6f64 6529 3a0a 0a20 206d  ode, Node):..  m
 00156ff0: 6170 7069 6e67 3a20 4375 7276 654d 6170  apping: CurveMap
 00157000: 7069 6e67 203d 202e 2e2e 0a0a 2020 4063  ping = .....  @c
 00157010: 6c61 7373 6d65 7468 6f64 0a0a 2020 6465  lassmethod..  de
 00157020: 6620 6973 5f72 6567 6973 7465 7265 645f  f is_registered_
 00157030: 6e6f 6465 5f74 7970 6528 636c 7329 202d  node_type(cls) -
 00157040: 3e20 626f 6f6c 3a0a 0a20 2020 2022 2222  > bool:..    """
 00157050: 0a0a 2020 2020 5472 7565 2069 6620 6120  ..    True if a 
@@ -87846,17 +87846,17 @@
 00157250: 745f 7375 6263 6c61 7373 5f70 7928 636c  t_subclass_py(cl
 00157260: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 00157270: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 00157280: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 00157290: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 001572a0: 0a0a 636c 6173 7320 436f 6d70 6f73 6974  ..class Composit
 001572b0: 6f72 4e6f 6465 4375 7276 6556 6563 2862  orNodeCurveVec(b
-001572c0: 7079 5f73 7472 7563 742c 2043 6f6d 706f  py_struct, Compo
-001572d0: 7369 746f 724e 6f64 652c 204e 6f64 652c  sitorNode, Node,
-001572e0: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+001572c0: 7079 5f73 7472 7563 742c 204e 6f64 6549  py_struct, NodeI
+001572d0: 6e74 6572 6e61 6c2c 2043 6f6d 706f 7369  nternal, Composi
+001572e0: 746f 724e 6f64 652c 204e 6f64 6529 3a0a  torNode, Node):.
 001572f0: 0a20 206d 6170 7069 6e67 3a20 4375 7276  .  mapping: Curv
 00157300: 654d 6170 7069 6e67 203d 202e 2e2e 0a0a  eMapping = .....
 00157310: 2020 4063 6c61 7373 6d65 7468 6f64 0a0a    @classmethod..
 00157320: 2020 6465 6620 6973 5f72 6567 6973 7465    def is_registe
 00157330: 7265 645f 6e6f 6465 5f74 7970 6528 636c  red_node_type(cl
 00157340: 7329 202d 3e20 626f 6f6c 3a0a 0a20 2020  s) -> bool:..   
 00157350: 2022 2222 0a0a 2020 2020 5472 7565 2069   """..    True i
@@ -87895,17 +87895,17 @@
 00157560: 7928 636c 732c 2069 643a 2073 7472 2c20  y(cls, id: str, 
 00157570: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 00157580: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 00157590: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 001575a0: 202e 2e2e 0a0a 636c 6173 7320 436f 6d70   .....class Comp
 001575b0: 6f73 6974 6f72 4e6f 6465 4375 7374 6f6d  ositorNodeCustom
 001575c0: 4772 6f75 7028 6270 795f 7374 7275 6374  Group(bpy_struct
-001575d0: 2c20 436f 6d70 6f73 6974 6f72 4e6f 6465  , CompositorNode
-001575e0: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-001575f0: 726e 616c 293a 0a0a 2020 2222 220a 0a20  rnal):..  """.. 
+001575d0: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+001575e0: 436f 6d70 6f73 6974 6f72 4e6f 6465 2c20  CompositorNode, 
+001575f0: 4e6f 6465 293a 0a0a 2020 2222 220a 0a20  Node):..  """.. 
 00157600: 2043 7573 746f 6d20 436f 6d70 6f73 6974   Custom Composit
 00157610: 6f72 2047 726f 7570 204e 6f64 6520 666f  or Group Node fo
 00157620: 7220 5079 7468 6f6e 206e 6f64 6573 0a0a  r Python nodes..
 00157630: 2020 2222 220a 0a20 206e 6f64 655f 7472    """..  node_tr
 00157640: 6565 3a20 4e6f 6465 5472 6565 203d 202e  ee: NodeTree = .
 00157650: 2e2e 0a0a 2020 6465 6620 7570 6461 7465  ....  def update
 00157660: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
@@ -87921,17 +87921,17 @@
 00157700: 6765 745f 7375 6263 6c61 7373 5f70 7928  get_subclass_py(
 00157710: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 00157720: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 00157730: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 00157740: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 00157750: 2e2e 0a0a 636c 6173 7320 436f 6d70 6f73  ....class Compos
 00157760: 6974 6f72 4e6f 6465 4442 6c75 7228 6270  itorNodeDBlur(bp
-00157770: 795f 7374 7275 6374 2c20 436f 6d70 6f73  y_struct, Compos
-00157780: 6974 6f72 4e6f 6465 2c20 4e6f 6465 2c20  itorNode, Node, 
-00157790: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+00157770: 795f 7374 7275 6374 2c20 4e6f 6465 496e  y_struct, NodeIn
+00157780: 7465 726e 616c 2c20 436f 6d70 6f73 6974  ternal, Composit
+00157790: 6f72 4e6f 6465 2c20 4e6f 6465 293a 0a0a  orNode, Node):..
 001577a0: 2020 616e 676c 653a 2066 6c6f 6174 203d    angle: float =
 001577b0: 202e 2e2e 0a0a 2020 6365 6e74 6572 5f78   .....  center_x
 001577c0: 3a20 666c 6f61 7420 3d20 2e2e 2e0a 0a20  : float = ..... 
 001577d0: 2063 656e 7465 725f 793a 2066 6c6f 6174   center_y: float
 001577e0: 203d 202e 2e2e 0a0a 2020 6469 7374 616e   = .....  distan
 001577f0: 6365 3a20 666c 6f61 7420 3d20 2e2e 2e0a  ce: float = ....
 00157800: 0a20 2069 7465 7261 7469 6f6e 733a 2069  .  iterations: i
@@ -87978,17 +87978,17 @@
 00157a90: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 00157aa0: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 00157ab0: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 00157ac0: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 00157ad0: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 00157ae0: 436f 6d70 6f73 6974 6f72 4e6f 6465 4465  CompositorNodeDe
 00157af0: 666f 6375 7328 6270 795f 7374 7275 6374  focus(bpy_struct
-00157b00: 2c20 436f 6d70 6f73 6974 6f72 4e6f 6465  , CompositorNode
-00157b10: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-00157b20: 726e 616c 293a 0a0a 2020 616e 676c 653a  rnal):..  angle:
+00157b00: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+00157b10: 436f 6d70 6f73 6974 6f72 4e6f 6465 2c20  CompositorNode, 
+00157b20: 4e6f 6465 293a 0a0a 2020 616e 676c 653a  Node):..  angle:
 00157b30: 2066 6c6f 6174 203d 202e 2e2e 0a0a 2020   float = .....  
 00157b40: 2222 220a 0a20 2042 6f6b 6568 2073 6861  """..  Bokeh sha
 00157b50: 7065 2072 6f74 6174 696f 6e20 6f66 6673  pe rotation offs
 00157b60: 6574 0a0a 2020 2222 220a 0a20 2062 6c75  et..  """..  blu
 00157b70: 725f 6d61 783a 2066 6c6f 6174 203d 202e  r_max: float = .
 00157b80: 2e2e 0a0a 2020 2222 220a 0a20 2042 6c75  ....  """..  Blu
 00157b90: 7220 6c69 6d69 742c 206d 6178 696d 756d  r limit, maximum
@@ -88107,17 +88107,17 @@
 001582a0: 5f70 7928 636c 732c 2069 643a 2073 7472  _py(cls, id: str
 001582b0: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 001582c0: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 001582d0: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 001582e0: 2020 202e 2e2e 0a0a 636c 6173 7320 436f     .....class Co
 001582f0: 6d70 6f73 6974 6f72 4e6f 6465 4465 6e6f  mpositorNodeDeno
 00158300: 6973 6528 6270 795f 7374 7275 6374 2c20  ise(bpy_struct, 
-00158310: 436f 6d70 6f73 6974 6f72 4e6f 6465 2c20  CompositorNode, 
-00158320: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-00158330: 616c 293a 0a0a 2020 7072 6566 696c 7465  al):..  prefilte
+00158310: 4e6f 6465 496e 7465 726e 616c 2c20 436f  NodeInternal, Co
+00158320: 6d70 6f73 6974 6f72 4e6f 6465 2c20 4e6f  mpositorNode, No
+00158330: 6465 293a 0a0a 2020 7072 6566 696c 7465  de):..  prefilte
 00158340: 723a 2073 7472 203d 202e 2e2e 0a0a 2020  r: str = .....  
 00158350: 2222 220a 0a20 2044 656e 6f69 7369 6e67  """..  Denoising
 00158360: 2070 7265 6669 6c74 6572 0a0a 2020 2a20   prefilter..  * 
 00158370: 6060 4e4f 4e45 6060 0a4e 6f6e 6520 2d2d  ``NONE``.None --
 00158380: 204e 6f20 7072 6566 696c 7465 7269 6e67   No prefiltering
 00158390: 2c20 7573 6520 7768 656e 2067 7569 6469  , use when guidi
 001583a0: 6e67 2070 6173 7365 7320 6172 6520 6e6f  ng passes are no
@@ -88185,17 +88185,17 @@
 00158780: 5f73 7562 636c 6173 735f 7079 2863 6c73  _subclass_py(cls
 00158790: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 001587a0: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 001587b0: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 001587c0: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 001587d0: 0a63 6c61 7373 2043 6f6d 706f 7369 746f  .class Composito
 001587e0: 724e 6f64 6544 6573 7065 636b 6c65 2862  rNodeDespeckle(b
-001587f0: 7079 5f73 7472 7563 742c 2043 6f6d 706f  py_struct, Compo
-00158800: 7369 746f 724e 6f64 652c 204e 6f64 652c  sitorNode, Node,
-00158810: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+001587f0: 7079 5f73 7472 7563 742c 204e 6f64 6549  py_struct, NodeI
+00158800: 6e74 6572 6e61 6c2c 2043 6f6d 706f 7369  nternal, Composi
+00158810: 746f 724e 6f64 652c 204e 6f64 6529 3a0a  torNode, Node):.
 00158820: 0a20 2074 6872 6573 686f 6c64 3a20 666c  .  threshold: fl
 00158830: 6f61 7420 3d20 2e2e 2e0a 0a20 2022 2222  oat = .....  """
 00158840: 0a0a 2020 5468 7265 7368 6f6c 6420 666f  ..  Threshold fo
 00158850: 7220 6465 7465 6374 696e 6720 7069 7865  r detecting pixe
 00158860: 6c73 2074 6f20 6465 7370 6563 6b6c 650a  ls to despeckle.
 00158870: 0a20 2022 2222 0a0a 2020 7468 7265 7368  .  """..  thresh
 00158880: 6f6c 645f 6e65 6967 6862 6f72 3a20 666c  old_neighbor: fl
@@ -88244,17 +88244,17 @@
 00158b30: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 00158b40: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 00158b50: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 00158b60: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 00158b70: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 00158b80: 6173 7320 436f 6d70 6f73 6974 6f72 4e6f  ass CompositorNo
 00158b90: 6465 4469 6666 4d61 7474 6528 6270 795f  deDiffMatte(bpy_
-00158ba0: 7374 7275 6374 2c20 436f 6d70 6f73 6974  struct, Composit
-00158bb0: 6f72 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  orNode, Node, No
-00158bc0: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+00158ba0: 7374 7275 6374 2c20 4e6f 6465 496e 7465  struct, NodeInte
+00158bb0: 726e 616c 2c20 436f 6d70 6f73 6974 6f72  rnal, Compositor
+00158bc0: 4e6f 6465 2c20 4e6f 6465 293a 0a0a 2020  Node, Node):..  
 00158bd0: 6661 6c6c 6f66 663a 2066 6c6f 6174 203d  falloff: float =
 00158be0: 202e 2e2e 0a0a 2020 2222 220a 0a20 2043   .....  """..  C
 00158bf0: 6f6c 6f72 2064 6973 7461 6e63 6573 2062  olor distances b
 00158c00: 656c 6f77 2074 6869 7320 6164 6469 7469  elow this additi
 00158c10: 6f6e 616c 2074 6872 6573 686f 6c64 2061  onal threshold a
 00158c20: 7265 2070 6172 7469 616c 6c79 206b 6579  re partially key
 00158c30: 6564 0a0a 2020 2222 220a 0a20 2074 6f6c  ed..  """..  tol
@@ -88303,17 +88303,17 @@
 00158ee0: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 00158ef0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 00158f00: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 00158f10: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 00158f20: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 00158f30: 2043 6f6d 706f 7369 746f 724e 6f64 6544   CompositorNodeD
 00158f40: 696c 6174 6545 726f 6465 2862 7079 5f73  ilateErode(bpy_s
-00158f50: 7472 7563 742c 2043 6f6d 706f 7369 746f  truct, Composito
-00158f60: 724e 6f64 652c 204e 6f64 652c 204e 6f64  rNode, Node, Nod
-00158f70: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2064  eInternal):..  d
+00158f50: 7472 7563 742c 204e 6f64 6549 6e74 6572  truct, NodeInter
+00158f60: 6e61 6c2c 2043 6f6d 706f 7369 746f 724e  nal, CompositorN
+00158f70: 6f64 652c 204e 6f64 6529 3a0a 0a20 2064  ode, Node):..  d
 00158f80: 6973 7461 6e63 653a 2069 6e74 203d 202e  istance: int = .
 00158f90: 2e2e 0a0a 2020 2222 220a 0a20 2044 6973  ....  """..  Dis
 00158fa0: 7461 6e63 6520 746f 2067 726f 772f 7368  tance to grow/sh
 00158fb0: 7269 6e6b 2028 6e75 6d62 6572 206f 6620  rink (number of 
 00158fc0: 6974 6572 6174 696f 6e73 290a 0a20 2022  iterations)..  "
 00158fd0: 2222 0a0a 2020 6564 6765 3a20 666c 6f61  ""..  edge: floa
 00158fe0: 7420 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  t = .....  """..
@@ -88366,17 +88366,17 @@
 001592d0: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 001592e0: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 001592f0: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 00159300: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 00159310: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2043      .....class C
 00159320: 6f6d 706f 7369 746f 724e 6f64 6544 6973  ompositorNodeDis
 00159330: 706c 6163 6528 6270 795f 7374 7275 6374  place(bpy_struct
-00159340: 2c20 436f 6d70 6f73 6974 6f72 4e6f 6465  , CompositorNode
-00159350: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-00159360: 726e 616c 293a 0a0a 2020 4063 6c61 7373  rnal):..  @class
+00159340: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+00159350: 436f 6d70 6f73 6974 6f72 4e6f 6465 2c20  CompositorNode, 
+00159360: 4e6f 6465 293a 0a0a 2020 4063 6c61 7373  Node):..  @class
 00159370: 6d65 7468 6f64 0a0a 2020 6465 6620 6973  method..  def is
 00159380: 5f72 6567 6973 7465 7265 645f 6e6f 6465  _registered_node
 00159390: 5f74 7970 6528 636c 7329 202d 3e20 626f  _type(cls) -> bo
 001593a0: 6f6c 3a0a 0a20 2020 2022 2222 0a0a 2020  ol:..    """..  
 001593b0: 2020 5472 7565 2069 6620 6120 7265 6769    True if a regi
 001593c0: 7374 6572 6564 206e 6f64 6520 7479 7065  stered node type
 001593d0: 0a0a 2020 2020 2222 220a 0a20 2020 202e  ..    """..    .
@@ -88412,17 +88412,17 @@
 001595b0: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 001595c0: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 001595d0: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 001595e0: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 001595f0: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 00159600: 6173 7320 436f 6d70 6f73 6974 6f72 4e6f  ass CompositorNo
 00159610: 6465 4469 7374 616e 6365 4d61 7474 6528  deDistanceMatte(
-00159620: 6270 795f 7374 7275 6374 2c20 436f 6d70  bpy_struct, Comp
-00159630: 6f73 6974 6f72 4e6f 6465 2c20 4e6f 6465  ositorNode, Node
-00159640: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+00159620: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+00159630: 496e 7465 726e 616c 2c20 436f 6d70 6f73  Internal, Compos
+00159640: 6974 6f72 4e6f 6465 2c20 4e6f 6465 293a  itorNode, Node):
 00159650: 0a0a 2020 6368 616e 6e65 6c3a 2073 7472  ..  channel: str
 00159660: 203d 202e 2e2e 0a0a 2020 2222 220a 0a20   = .....  """.. 
 00159670: 202a 2060 6052 4742 6060 0a52 4742 202d   * ``RGB``.RGB -
 00159680: 2d20 5247 4220 636f 6c6f 7220 7370 6163  - RGB color spac
 00159690: 652e 0a0a 2020 2a20 6060 5943 4360 600a  e...  * ``YCC``.
 001596a0: 5943 4320 2d2d 2059 4362 4372 2073 7570  YCC -- YCbCr sup
 001596b0: 7072 6573 7369 6f6e 2e0a 0a20 2022 2222  pression...  """
@@ -88478,17 +88478,17 @@
 001599d0: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 001599e0: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 001599f0: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 00159a00: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 00159a10: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 00159a20: 6c61 7373 2043 6f6d 706f 7369 746f 724e  lass CompositorN
 00159a30: 6f64 6544 6f75 626c 6545 6467 654d 6173  odeDoubleEdgeMas
-00159a40: 6b28 6270 795f 7374 7275 6374 2c20 436f  k(bpy_struct, Co
-00159a50: 6d70 6f73 6974 6f72 4e6f 6465 2c20 4e6f  mpositorNode, No
-00159a60: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+00159a40: 6b28 6270 795f 7374 7275 6374 2c20 4e6f  k(bpy_struct, No
+00159a50: 6465 496e 7465 726e 616c 2c20 436f 6d70  deInternal, Comp
+00159a60: 6f73 6974 6f72 4e6f 6465 2c20 4e6f 6465  ositorNode, Node
 00159a70: 293a 0a0a 2020 6564 6765 5f6d 6f64 653a  ):..  edge_mode:
 00159a80: 2073 7472 203d 202e 2e2e 0a0a 2020 2222   str = .....  ""
 00159a90: 220a 0a20 202a 2060 6042 4c45 4544 5f4f  "..  * ``BLEED_O
 00159aa0: 5554 6060 0a42 6c65 6564 204f 7574 202d  UT``.Bleed Out -
 00159ab0: 2d20 416c 6c6f 7720 6d61 736b 2070 6978  - Allow mask pix
 00159ac0: 656c 7320 746f 2062 6c65 6564 2061 6c6f  els to bleed alo
 00159ad0: 6e67 2065 6467 6573 2e0a 0a20 202a 2060  ng edges...  * `
@@ -88553,17 +88553,17 @@
 00159e80: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 00159e90: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 00159ea0: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 00159eb0: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 00159ec0: 2e2e 0a0a 636c 6173 7320 436f 6d70 6f73  ....class Compos
 00159ed0: 6974 6f72 4e6f 6465 456c 6c69 7073 654d  itorNodeEllipseM
 00159ee0: 6173 6b28 6270 795f 7374 7275 6374 2c20  ask(bpy_struct, 
-00159ef0: 436f 6d70 6f73 6974 6f72 4e6f 6465 2c20  CompositorNode, 
-00159f00: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-00159f10: 616c 293a 0a0a 2020 6865 6967 6874 3a20  al):..  height: 
+00159ef0: 4e6f 6465 496e 7465 726e 616c 2c20 436f  NodeInternal, Co
+00159f00: 6d70 6f73 6974 6f72 4e6f 6465 2c20 4e6f  mpositorNode, No
+00159f10: 6465 293a 0a0a 2020 6865 6967 6874 3a20  de):..  height: 
 00159f20: 666c 6f61 7420 3d20 2e2e 2e0a 0a20 2022  float = .....  "
 00159f30: 2222 0a0a 2020 4865 6967 6874 206f 6620  ""..  Height of 
 00159f40: 7468 6520 656c 6c69 7073 650a 0a20 2022  the ellipse..  "
 00159f50: 2222 0a0a 2020 6d61 736b 5f74 7970 653a  ""..  mask_type:
 00159f60: 2073 7472 203d 202e 2e2e 0a0a 2020 726f   str = .....  ro
 00159f70: 7461 7469 6f6e 3a20 666c 6f61 7420 3d20  tation: float = 
 00159f80: 2e2e 2e0a 0a20 2022 2222 0a0a 2020 526f  .....  """..  Ro
@@ -88622,17 +88622,17 @@
 0015a2d0: 6c61 7373 5f70 7928 636c 732c 2069 643a  lass_py(cls, id:
 0015a2e0: 2073 7472 2c20 6465 6661 756c 743a 2074   str, default: t
 0015a2f0: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 0015a300: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 0015a310: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 0015a320: 7320 436f 6d70 6f73 6974 6f72 4e6f 6465  s CompositorNode
 0015a330: 4578 706f 7375 7265 2862 7079 5f73 7472  Exposure(bpy_str
-0015a340: 7563 742c 2043 6f6d 706f 7369 746f 724e  uct, CompositorN
-0015a350: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-0015a360: 6e74 6572 6e61 6c29 3a0a 0a20 2040 636c  nternal):..  @cl
+0015a340: 7563 742c 204e 6f64 6549 6e74 6572 6e61  uct, NodeInterna
+0015a350: 6c2c 2043 6f6d 706f 7369 746f 724e 6f64  l, CompositorNod
+0015a360: 652c 204e 6f64 6529 3a0a 0a20 2040 636c  e, Node):..  @cl
 0015a370: 6173 736d 6574 686f 640a 0a20 2064 6566  assmethod..  def
 0015a380: 2069 735f 7265 6769 7374 6572 6564 5f6e   is_registered_n
 0015a390: 6f64 655f 7479 7065 2863 6c73 2920 2d3e  ode_type(cls) ->
 0015a3a0: 2062 6f6f 6c3a 0a0a 2020 2020 2222 220a   bool:..    """.
 0015a3b0: 0a20 2020 2054 7275 6520 6966 2061 2072  .    True if a r
 0015a3c0: 6567 6973 7465 7265 6420 6e6f 6465 2074  egistered node t
 0015a3d0: 7970 650a 0a20 2020 2022 2222 0a0a 2020  ype..    """..  
@@ -88668,17 +88668,17 @@
 0015a5b0: 5f73 7562 636c 6173 735f 7079 2863 6c73  _subclass_py(cls
 0015a5c0: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 0015a5d0: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 0015a5e0: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 0015a5f0: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 0015a600: 0a63 6c61 7373 2043 6f6d 706f 7369 746f  .class Composito
 0015a610: 724e 6f64 6546 696c 7465 7228 6270 795f  rNodeFilter(bpy_
-0015a620: 7374 7275 6374 2c20 436f 6d70 6f73 6974  struct, Composit
-0015a630: 6f72 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  orNode, Node, No
-0015a640: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+0015a620: 7374 7275 6374 2c20 4e6f 6465 496e 7465  struct, NodeInte
+0015a630: 726e 616c 2c20 436f 6d70 6f73 6974 6f72  rnal, Compositor
+0015a640: 4e6f 6465 2c20 4e6f 6465 293a 0a0a 2020  Node, Node):..  
 0015a650: 6669 6c74 6572 5f74 7970 653a 2073 7472  filter_type: str
 0015a660: 203d 202e 2e2e 0a0a 2020 4063 6c61 7373   = .....  @class
 0015a670: 6d65 7468 6f64 0a0a 2020 6465 6620 6973  method..  def is
 0015a680: 5f72 6567 6973 7465 7265 645f 6e6f 6465  _registered_node
 0015a690: 5f74 7970 6528 636c 7329 202d 3e20 626f  _type(cls) -> bo
 0015a6a0: 6f6c 3a0a 0a20 2020 2022 2222 0a0a 2020  ol:..    """..  
 0015a6b0: 2020 5472 7565 2069 6620 6120 7265 6769    True if a regi
@@ -88716,17 +88716,17 @@
 0015a8b0: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 0015a8c0: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 0015a8d0: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 0015a8e0: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 0015a8f0: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 0015a900: 6173 7320 436f 6d70 6f73 6974 6f72 4e6f  ass CompositorNo
 0015a910: 6465 466c 6970 2862 7079 5f73 7472 7563  deFlip(bpy_struc
-0015a920: 742c 2043 6f6d 706f 7369 746f 724e 6f64  t, CompositorNod
-0015a930: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-0015a940: 6572 6e61 6c29 3a0a 0a20 2061 7869 733a  ernal):..  axis:
+0015a920: 742c 204e 6f64 6549 6e74 6572 6e61 6c2c  t, NodeInternal,
+0015a930: 2043 6f6d 706f 7369 746f 724e 6f64 652c   CompositorNode,
+0015a940: 204e 6f64 6529 3a0a 0a20 2061 7869 733a   Node):..  axis:
 0015a950: 2073 7472 203d 202e 2e2e 0a0a 2020 4063   str = .....  @c
 0015a960: 6c61 7373 6d65 7468 6f64 0a0a 2020 6465  lassmethod..  de
 0015a970: 6620 6973 5f72 6567 6973 7465 7265 645f  f is_registered_
 0015a980: 6e6f 6465 5f74 7970 6528 636c 7329 202d  node_type(cls) -
 0015a990: 3e20 626f 6f6c 3a0a 0a20 2020 2022 2222  > bool:..    """
 0015a9a0: 0a0a 2020 2020 5472 7565 2069 6620 6120  ..    True if a 
 0015a9b0: 7265 6769 7374 6572 6564 206e 6f64 6520  registered node 
@@ -88763,17 +88763,17 @@
 0015aba0: 745f 7375 6263 6c61 7373 5f70 7928 636c  t_subclass_py(cl
 0015abb0: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 0015abc0: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 0015abd0: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 0015abe0: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 0015abf0: 0a0a 636c 6173 7320 436f 6d70 6f73 6974  ..class Composit
 0015ac00: 6f72 4e6f 6465 4761 6d6d 6128 6270 795f  orNodeGamma(bpy_
-0015ac10: 7374 7275 6374 2c20 436f 6d70 6f73 6974  struct, Composit
-0015ac20: 6f72 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  orNode, Node, No
-0015ac30: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+0015ac10: 7374 7275 6374 2c20 4e6f 6465 496e 7465  struct, NodeInte
+0015ac20: 726e 616c 2c20 436f 6d70 6f73 6974 6f72  rnal, Compositor
+0015ac30: 4e6f 6465 2c20 4e6f 6465 293a 0a0a 2020  Node, Node):..  
 0015ac40: 4063 6c61 7373 6d65 7468 6f64 0a0a 2020  @classmethod..  
 0015ac50: 6465 6620 6973 5f72 6567 6973 7465 7265  def is_registere
 0015ac60: 645f 6e6f 6465 5f74 7970 6528 636c 7329  d_node_type(cls)
 0015ac70: 202d 3e20 626f 6f6c 3a0a 0a20 2020 2022   -> bool:..    "
 0015ac80: 2222 0a0a 2020 2020 5472 7565 2069 6620  ""..    True if 
 0015ac90: 6120 7265 6769 7374 6572 6564 206e 6f64  a registered nod
 0015aca0: 6520 7479 7065 0a0a 2020 2020 2222 220a  e type..    """.
@@ -88809,17 +88809,17 @@
 0015ae80: 6765 745f 7375 6263 6c61 7373 5f70 7928  get_subclass_py(
 0015ae90: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 0015aea0: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 0015aeb0: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 0015aec0: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 0015aed0: 2e2e 0a0a 636c 6173 7320 436f 6d70 6f73  ....class Compos
 0015aee0: 6974 6f72 4e6f 6465 476c 6172 6528 6270  itorNodeGlare(bp
-0015aef0: 795f 7374 7275 6374 2c20 436f 6d70 6f73  y_struct, Compos
-0015af00: 6974 6f72 4e6f 6465 2c20 4e6f 6465 2c20  itorNode, Node, 
-0015af10: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+0015aef0: 795f 7374 7275 6374 2c20 4e6f 6465 496e  y_struct, NodeIn
+0015af00: 7465 726e 616c 2c20 436f 6d70 6f73 6974  ternal, Composit
+0015af10: 6f72 4e6f 6465 2c20 4e6f 6465 293a 0a0a  orNode, Node):..
 0015af20: 2020 616e 676c 655f 6f66 6673 6574 3a20    angle_offset: 
 0015af30: 666c 6f61 7420 3d20 2e2e 2e0a 0a20 2022  float = .....  "
 0015af40: 2222 0a0a 2020 5374 7265 616b 2061 6e67  ""..  Streak ang
 0015af50: 6c65 206f 6666 7365 740a 0a20 2022 2222  le offset..  """
 0015af60: 0a0a 2020 636f 6c6f 725f 6d6f 6475 6c61  ..  color_modula
 0015af70: 7469 6f6e 3a20 666c 6f61 7420 3d20 2e2e  tion: float = ..
 0015af80: 2e0a 0a20 2022 2222 0a0a 2020 416d 6f75  ...  """..  Amou
@@ -88916,17 +88916,17 @@
 0015b530: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 0015b540: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 0015b550: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 0015b560: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 0015b570: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 0015b580: 7373 2043 6f6d 706f 7369 746f 724e 6f64  ss CompositorNod
 0015b590: 6547 726f 7570 2862 7079 5f73 7472 7563  eGroup(bpy_struc
-0015b5a0: 742c 2043 6f6d 706f 7369 746f 724e 6f64  t, CompositorNod
-0015b5b0: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-0015b5c0: 6572 6e61 6c29 3a0a 0a20 206e 6f64 655f  ernal):..  node_
+0015b5a0: 742c 204e 6f64 6549 6e74 6572 6e61 6c2c  t, NodeInternal,
+0015b5b0: 2043 6f6d 706f 7369 746f 724e 6f64 652c   CompositorNode,
+0015b5c0: 204e 6f64 6529 3a0a 0a20 206e 6f64 655f   Node):..  node_
 0015b5d0: 7472 6565 3a20 4e6f 6465 5472 6565 203d  tree: NodeTree =
 0015b5e0: 202e 2e2e 0a0a 2020 4063 6c61 7373 6d65   .....  @classme
 0015b5f0: 7468 6f64 0a0a 2020 6465 6620 6973 5f72  thod..  def is_r
 0015b600: 6567 6973 7465 7265 645f 6e6f 6465 5f74  egistered_node_t
 0015b610: 7970 6528 636c 7329 202d 3e20 626f 6f6c  ype(cls) -> bool
 0015b620: 3a0a 0a20 2020 2022 2222 0a0a 2020 2020  :..    """..    
 0015b630: 5472 7565 2069 6620 6120 7265 6769 7374  True if a regist
@@ -88964,17 +88964,17 @@
 0015b830: 6c61 7373 5f70 7928 636c 732c 2069 643a  lass_py(cls, id:
 0015b840: 2073 7472 2c20 6465 6661 756c 743a 2074   str, default: t
 0015b850: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 0015b860: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 0015b870: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 0015b880: 7320 436f 6d70 6f73 6974 6f72 4e6f 6465  s CompositorNode
 0015b890: 4875 6543 6f72 7265 6374 2862 7079 5f73  HueCorrect(bpy_s
-0015b8a0: 7472 7563 742c 2043 6f6d 706f 7369 746f  truct, Composito
-0015b8b0: 724e 6f64 652c 204e 6f64 652c 204e 6f64  rNode, Node, Nod
-0015b8c0: 6549 6e74 6572 6e61 6c29 3a0a 0a20 206d  eInternal):..  m
+0015b8a0: 7472 7563 742c 204e 6f64 6549 6e74 6572  truct, NodeInter
+0015b8b0: 6e61 6c2c 2043 6f6d 706f 7369 746f 724e  nal, CompositorN
+0015b8c0: 6f64 652c 204e 6f64 6529 3a0a 0a20 206d  ode, Node):..  m
 0015b8d0: 6170 7069 6e67 3a20 4375 7276 654d 6170  apping: CurveMap
 0015b8e0: 7069 6e67 203d 202e 2e2e 0a0a 2020 4063  ping = .....  @c
 0015b8f0: 6c61 7373 6d65 7468 6f64 0a0a 2020 6465  lassmethod..  de
 0015b900: 6620 6973 5f72 6567 6973 7465 7265 645f  f is_registered_
 0015b910: 6e6f 6465 5f74 7970 6528 636c 7329 202d  node_type(cls) -
 0015b920: 3e20 626f 6f6c 3a0a 0a20 2020 2022 2222  > bool:..    """
 0015b930: 0a0a 2020 2020 5472 7565 2069 6620 6120  ..    True if a 
@@ -89012,17 +89012,17 @@
 0015bb30: 745f 7375 6263 6c61 7373 5f70 7928 636c  t_subclass_py(cl
 0015bb40: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 0015bb50: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 0015bb60: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 0015bb70: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 0015bb80: 0a0a 636c 6173 7320 436f 6d70 6f73 6974  ..class Composit
 0015bb90: 6f72 4e6f 6465 4875 6553 6174 2862 7079  orNodeHueSat(bpy
-0015bba0: 5f73 7472 7563 742c 2043 6f6d 706f 7369  _struct, Composi
-0015bbb0: 746f 724e 6f64 652c 204e 6f64 652c 204e  torNode, Node, N
-0015bbc0: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+0015bba0: 5f73 7472 7563 742c 204e 6f64 6549 6e74  _struct, NodeInt
+0015bbb0: 6572 6e61 6c2c 2043 6f6d 706f 7369 746f  ernal, Composito
+0015bbc0: 724e 6f64 652c 204e 6f64 6529 3a0a 0a20  rNode, Node):.. 
 0015bbd0: 2040 636c 6173 736d 6574 686f 640a 0a20   @classmethod.. 
 0015bbe0: 2064 6566 2069 735f 7265 6769 7374 6572   def is_register
 0015bbf0: 6564 5f6e 6f64 655f 7479 7065 2863 6c73  ed_node_type(cls
 0015bc00: 2920 2d3e 2062 6f6f 6c3a 0a0a 2020 2020  ) -> bool:..    
 0015bc10: 2222 220a 0a20 2020 2054 7275 6520 6966  """..    True if
 0015bc20: 2061 2072 6567 6973 7465 7265 6420 6e6f   a registered no
 0015bc30: 6465 2074 7970 650a 0a20 2020 2022 2222  de type..    """
@@ -89058,17 +89058,17 @@
 0015be10: 5f67 6574 5f73 7562 636c 6173 735f 7079  _get_subclass_py
 0015be20: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 0015be30: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 0015be40: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 0015be50: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 0015be60: 2e2e 2e0a 0a63 6c61 7373 2043 6f6d 706f  .....class Compo
 0015be70: 7369 746f 724e 6f64 6549 444d 6173 6b28  sitorNodeIDMask(
-0015be80: 6270 795f 7374 7275 6374 2c20 436f 6d70  bpy_struct, Comp
-0015be90: 6f73 6974 6f72 4e6f 6465 2c20 4e6f 6465  ositorNode, Node
-0015bea0: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+0015be80: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+0015be90: 496e 7465 726e 616c 2c20 436f 6d70 6f73  Internal, Compos
+0015bea0: 6974 6f72 4e6f 6465 2c20 4e6f 6465 293a  itorNode, Node):
 0015beb0: 0a0a 2020 696e 6465 783a 2069 6e74 203d  ..  index: int =
 0015bec0: 202e 2e2e 0a0a 2020 2222 220a 0a20 2050   .....  """..  P
 0015bed0: 6173 7320 696e 6465 7820 6e75 6d62 6572  ass index number
 0015bee0: 2074 6f20 636f 6e76 6572 7420 746f 2061   to convert to a
 0015bef0: 6c70 6861 0a0a 2020 2222 220a 0a20 2075  lpha..  """..  u
 0015bf00: 7365 5f61 6e74 6961 6c69 6173 696e 673a  se_antialiasing:
 0015bf10: 2062 6f6f 6c20 3d20 2e2e 2e0a 0a20 2022   bool = .....  "
@@ -89115,17 +89115,17 @@
 0015c1a0: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 0015c1b0: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 0015c1c0: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 0015c1d0: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 0015c1e0: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 0015c1f0: 6173 7320 436f 6d70 6f73 6974 6f72 4e6f  ass CompositorNo
 0015c200: 6465 496d 6167 6528 6270 795f 7374 7275  deImage(bpy_stru
-0015c210: 6374 2c20 436f 6d70 6f73 6974 6f72 4e6f  ct, CompositorNo
-0015c220: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-0015c230: 7465 726e 616c 293a 0a0a 2020 6672 616d  ternal):..  fram
+0015c210: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+0015c220: 2c20 436f 6d70 6f73 6974 6f72 4e6f 6465  , CompositorNode
+0015c230: 2c20 4e6f 6465 293a 0a0a 2020 6672 616d  , Node):..  fram
 0015c240: 655f 6475 7261 7469 6f6e 3a20 696e 7420  e_duration: int 
 0015c250: 3d20 2e2e 2e0a 0a20 2022 2222 0a0a 2020  = .....  """..  
 0015c260: 4e75 6d62 6572 206f 6620 696d 6167 6573  Number of images
 0015c270: 206f 6620 6120 6d6f 7669 6520 746f 2075   of a movie to u
 0015c280: 7365 0a0a 2020 2222 220a 0a20 2066 7261  se..  """..  fra
 0015c290: 6d65 5f6f 6666 7365 743a 2069 6e74 203d  me_offset: int =
 0015c2a0: 202e 2e2e 0a0a 2020 2222 220a 0a20 204f   .....  """..  O
@@ -89211,18 +89211,18 @@
 0015c7a0: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 0015c7b0: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 0015c7c0: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 0015c7d0: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 0015c7e0: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 0015c7f0: 2020 2e2e 2e0a 0a63 6c61 7373 2043 6f6d    .....class Com
 0015c800: 706f 7369 746f 724e 6f64 6549 6e70 6169  positorNodeInpai
-0015c810: 6e74 2862 7079 5f73 7472 7563 742c 2043  nt(bpy_struct, C
-0015c820: 6f6d 706f 7369 746f 724e 6f64 652c 204e  ompositorNode, N
-0015c830: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-0015c840: 6c29 3a0a 0a20 2064 6973 7461 6e63 653a  l):..  distance:
+0015c810: 6e74 2862 7079 5f73 7472 7563 742c 204e  nt(bpy_struct, N
+0015c820: 6f64 6549 6e74 6572 6e61 6c2c 2043 6f6d  odeInternal, Com
+0015c830: 706f 7369 746f 724e 6f64 652c 204e 6f64  positorNode, Nod
+0015c840: 6529 3a0a 0a20 2064 6973 7461 6e63 653a  e):..  distance:
 0015c850: 2069 6e74 203d 202e 2e2e 0a0a 2020 2222   int = .....  ""
 0015c860: 220a 0a20 2044 6973 7461 6e63 6520 746f  "..  Distance to
 0015c870: 2069 6e70 6169 6e74 2028 6e75 6d62 6572   inpaint (number
 0015c880: 206f 6620 6974 6572 6174 696f 6e73 290a   of iterations).
 0015c890: 0a20 2022 2222 0a0a 2020 4063 6c61 7373  .  """..  @class
 0015c8a0: 6d65 7468 6f64 0a0a 2020 6465 6620 6973  method..  def is
 0015c8b0: 5f72 6567 6973 7465 7265 645f 6e6f 6465  _registered_node
@@ -89263,17 +89263,17 @@
 0015cae0: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 0015caf0: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 0015cb00: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 0015cb10: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 0015cb20: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 0015cb30: 6173 7320 436f 6d70 6f73 6974 6f72 4e6f  ass CompositorNo
 0015cb40: 6465 496e 7665 7274 2862 7079 5f73 7472  deInvert(bpy_str
-0015cb50: 7563 742c 2043 6f6d 706f 7369 746f 724e  uct, CompositorN
-0015cb60: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-0015cb70: 6e74 6572 6e61 6c29 3a0a 0a20 2069 6e76  nternal):..  inv
+0015cb50: 7563 742c 204e 6f64 6549 6e74 6572 6e61  uct, NodeInterna
+0015cb60: 6c2c 2043 6f6d 706f 7369 746f 724e 6f64  l, CompositorNod
+0015cb70: 652c 204e 6f64 6529 3a0a 0a20 2069 6e76  e, Node):..  inv
 0015cb80: 6572 745f 616c 7068 613a 2062 6f6f 6c20  ert_alpha: bool 
 0015cb90: 3d20 2e2e 2e0a 0a20 2069 6e76 6572 745f  = .....  invert_
 0015cba0: 7267 623a 2062 6f6f 6c20 3d20 2e2e 2e0a  rgb: bool = ....
 0015cbb0: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
 0015cbc0: 0a20 2064 6566 2069 735f 7265 6769 7374  .  def is_regist
 0015cbd0: 6572 6564 5f6e 6f64 655f 7479 7065 2863  ered_node_type(c
 0015cbe0: 6c73 2920 2d3e 2062 6f6f 6c3a 0a0a 2020  ls) -> bool:..  
@@ -89312,17 +89312,17 @@
 0015cdf0: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 0015ce00: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 0015ce10: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 0015ce20: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 0015ce30: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 0015ce40: 2020 2e2e 2e0a 0a63 6c61 7373 2043 6f6d    .....class Com
 0015ce50: 706f 7369 746f 724e 6f64 654b 6579 696e  positorNodeKeyin
-0015ce60: 6728 6270 795f 7374 7275 6374 2c20 436f  g(bpy_struct, Co
-0015ce70: 6d70 6f73 6974 6f72 4e6f 6465 2c20 4e6f  mpositorNode, No
-0015ce80: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+0015ce60: 6728 6270 795f 7374 7275 6374 2c20 4e6f  g(bpy_struct, No
+0015ce70: 6465 496e 7465 726e 616c 2c20 436f 6d70  deInternal, Comp
+0015ce80: 6f73 6974 6f72 4e6f 6465 2c20 4e6f 6465  ositorNode, Node
 0015ce90: 293a 0a0a 2020 626c 7572 5f70 6f73 743a  ):..  blur_post:
 0015cea0: 2069 6e74 203d 202e 2e2e 0a0a 2020 2222   int = .....  ""
 0015ceb0: 220a 0a20 204d 6174 7465 2062 6c75 7220  "..  Matte blur 
 0015cec0: 7369 7a65 2077 6869 6368 2061 7070 6c69  size which appli
 0015ced0: 6573 2061 6674 6572 2063 6c69 7070 696e  es after clippin
 0015cee0: 6720 616e 6420 6469 6c61 7465 2f65 726f  g and dilate/ero
 0015cef0: 6469 6e67 0a0a 2020 2222 220a 0a20 2062  ding..  """..  b
@@ -89438,17 +89438,17 @@
 0015d5d0: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 0015d5e0: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 0015d5f0: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 0015d600: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 0015d610: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2043      .....class C
 0015d620: 6f6d 706f 7369 746f 724e 6f64 654b 6579  ompositorNodeKey
 0015d630: 696e 6753 6372 6565 6e28 6270 795f 7374  ingScreen(bpy_st
-0015d640: 7275 6374 2c20 436f 6d70 6f73 6974 6f72  ruct, Compositor
-0015d650: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-0015d660: 496e 7465 726e 616c 293a 0a0a 2020 636c  Internal):..  cl
+0015d640: 7275 6374 2c20 4e6f 6465 496e 7465 726e  ruct, NodeIntern
+0015d650: 616c 2c20 436f 6d70 6f73 6974 6f72 4e6f  al, CompositorNo
+0015d660: 6465 2c20 4e6f 6465 293a 0a0a 2020 636c  de, Node):..  cl
 0015d670: 6970 3a20 4d6f 7669 6543 6c69 7020 3d20  ip: MovieClip = 
 0015d680: 2e2e 2e0a 0a20 2074 7261 636b 696e 675f  .....  tracking_
 0015d690: 6f62 6a65 6374 3a20 7374 7220 3d20 2e2e  object: str = ..
 0015d6a0: 2e0a 0a20 2040 636c 6173 736d 6574 686f  ...  @classmetho
 0015d6b0: 640a 0a20 2064 6566 2069 735f 7265 6769  d..  def is_regi
 0015d6c0: 7374 6572 6564 5f6e 6f64 655f 7479 7065  stered_node_type
 0015d6d0: 2863 6c73 2920 2d3e 2062 6f6f 6c3a 0a0a  (cls) -> bool:..
@@ -89488,17 +89488,17 @@
 0015d8f0: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 0015d900: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 0015d910: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 0015d920: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 0015d930: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2043      .....class C
 0015d940: 6f6d 706f 7369 746f 724e 6f64 654c 656e  ompositorNodeLen
 0015d950: 7364 6973 7428 6270 795f 7374 7275 6374  sdist(bpy_struct
-0015d960: 2c20 436f 6d70 6f73 6974 6f72 4e6f 6465  , CompositorNode
-0015d970: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-0015d980: 726e 616c 293a 0a0a 2020 7573 655f 6669  rnal):..  use_fi
+0015d960: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+0015d970: 436f 6d70 6f73 6974 6f72 4e6f 6465 2c20  CompositorNode, 
+0015d980: 4e6f 6465 293a 0a0a 2020 7573 655f 6669  Node):..  use_fi
 0015d990: 743a 2062 6f6f 6c20 3d20 2e2e 2e0a 0a20  t: bool = ..... 
 0015d9a0: 2022 2222 0a0a 2020 466f 7220 706f 7369   """..  For posi
 0015d9b0: 7469 7665 2064 6973 746f 7274 696f 6e20  tive distortion 
 0015d9c0: 6661 6374 6f72 206f 6e6c 793a 2073 6361  factor only: sca
 0015d9d0: 6c65 2069 6d61 6765 2073 7563 6820 7468  le image such th
 0015d9e0: 6174 2062 6c61 636b 2061 7265 6173 2061  at black areas a
 0015d9f0: 7265 206e 6f74 2076 6973 6962 6c65 0a0a  re not visible..
@@ -89556,17 +89556,17 @@
 0015dd30: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 0015dd40: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 0015dd50: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 0015dd60: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 0015dd70: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 0015dd80: 7373 2043 6f6d 706f 7369 746f 724e 6f64  ss CompositorNod
 0015dd90: 654c 6576 656c 7328 6270 795f 7374 7275  eLevels(bpy_stru
-0015dda0: 6374 2c20 436f 6d70 6f73 6974 6f72 4e6f  ct, CompositorNo
-0015ddb0: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-0015ddc0: 7465 726e 616c 293a 0a0a 2020 6368 616e  ternal):..  chan
+0015dda0: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+0015ddb0: 2c20 436f 6d70 6f73 6974 6f72 4e6f 6465  , CompositorNode
+0015ddc0: 2c20 4e6f 6465 293a 0a0a 2020 6368 616e  , Node):..  chan
 0015ddd0: 6e65 6c3a 2073 7472 203d 202e 2e2e 0a0a  nel: str = .....
 0015dde0: 2020 2222 220a 0a20 202a 2060 6043 4f4d    """..  * ``COM
 0015ddf0: 4249 4e45 445f 5247 4260 600a 436f 6d62  BINED_RGB``.Comb
 0015de00: 696e 6564 202d 2d20 436f 6d62 696e 6564  ined -- Combined
 0015de10: 2052 4742 2e0a 0a20 202a 2060 6052 4544   RGB...  * ``RED
 0015de20: 6060 0a52 6564 202d 2d20 5265 6420 4368  ``.Red -- Red Ch
 0015de30: 616e 6e65 6c2e 0a0a 2020 2a20 6060 4752  annel...  * ``GR
@@ -89617,17 +89617,17 @@
 0015e100: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 0015e110: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 0015e120: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 0015e130: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 0015e140: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 0015e150: 2e0a 0a63 6c61 7373 2043 6f6d 706f 7369  ...class Composi
 0015e160: 746f 724e 6f64 654c 756d 614d 6174 7465  torNodeLumaMatte
-0015e170: 2862 7079 5f73 7472 7563 742c 2043 6f6d  (bpy_struct, Com
-0015e180: 706f 7369 746f 724e 6f64 652c 204e 6f64  positorNode, Nod
-0015e190: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+0015e170: 2862 7079 5f73 7472 7563 742c 204e 6f64  (bpy_struct, Nod
+0015e180: 6549 6e74 6572 6e61 6c2c 2043 6f6d 706f  eInternal, Compo
+0015e190: 7369 746f 724e 6f64 652c 204e 6f64 6529  sitorNode, Node)
 0015e1a0: 3a0a 0a20 206c 696d 6974 5f6d 6178 3a20  :..  limit_max: 
 0015e1b0: 666c 6f61 7420 3d20 2e2e 2e0a 0a20 2022  float = .....  "
 0015e1c0: 2222 0a0a 2020 5661 6c75 6573 2068 6967  ""..  Values hig
 0015e1d0: 6865 7220 7468 616e 2074 6869 7320 7365  her than this se
 0015e1e0: 7474 696e 6720 6172 6520 3130 3025 206f  tting are 100% o
 0015e1f0: 7061 7175 650a 0a20 2022 2222 0a0a 2020  paque..  """..  
 0015e200: 6c69 6d69 745f 6d69 6e3a 2066 6c6f 6174  limit_min: float
@@ -89675,17 +89675,17 @@
 0015e4a0: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 0015e4b0: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 0015e4c0: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 0015e4d0: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 0015e4e0: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 0015e4f0: 7373 2043 6f6d 706f 7369 746f 724e 6f64  ss CompositorNod
 0015e500: 654d 6170 5261 6e67 6528 6270 795f 7374  eMapRange(bpy_st
-0015e510: 7275 6374 2c20 436f 6d70 6f73 6974 6f72  ruct, Compositor
-0015e520: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-0015e530: 496e 7465 726e 616c 293a 0a0a 2020 7573  Internal):..  us
+0015e510: 7275 6374 2c20 4e6f 6465 496e 7465 726e  ruct, NodeIntern
+0015e520: 616c 2c20 436f 6d70 6f73 6974 6f72 4e6f  al, CompositorNo
+0015e530: 6465 2c20 4e6f 6465 293a 0a0a 2020 7573  de, Node):..  us
 0015e540: 655f 636c 616d 703a 2062 6f6f 6c20 3d20  e_clamp: bool = 
 0015e550: 2e2e 2e0a 0a20 2022 2222 0a0a 2020 436c  .....  """..  Cl
 0015e560: 616d 7020 7468 6520 7265 7375 6c74 206f  amp the result o
 0015e570: 6620 7468 6520 6e6f 6465 2074 6f20 7468  f the node to th
 0015e580: 6520 7461 7267 6574 2072 616e 6765 0a0a  e target range..
 0015e590: 2020 2222 220a 0a20 2040 636c 6173 736d    """..  @classm
 0015e5a0: 6574 686f 640a 0a20 2064 6566 2069 735f  ethod..  def is_
@@ -89727,17 +89727,17 @@
 0015e7e0: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 0015e7f0: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 0015e800: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 0015e810: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 0015e820: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 0015e830: 7373 2043 6f6d 706f 7369 746f 724e 6f64  ss CompositorNod
 0015e840: 654d 6170 5556 2862 7079 5f73 7472 7563  eMapUV(bpy_struc
-0015e850: 742c 2043 6f6d 706f 7369 746f 724e 6f64  t, CompositorNod
-0015e860: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-0015e870: 6572 6e61 6c29 3a0a 0a20 2061 6c70 6861  ernal):..  alpha
+0015e850: 742c 204e 6f64 6549 6e74 6572 6e61 6c2c  t, NodeInternal,
+0015e860: 2043 6f6d 706f 7369 746f 724e 6f64 652c   CompositorNode,
+0015e870: 204e 6f64 6529 3a0a 0a20 2061 6c70 6861   Node):..  alpha
 0015e880: 3a20 696e 7420 3d20 2e2e 2e0a 0a20 2040  : int = .....  @
 0015e890: 636c 6173 736d 6574 686f 640a 0a20 2064  classmethod..  d
 0015e8a0: 6566 2069 735f 7265 6769 7374 6572 6564  ef is_registered
 0015e8b0: 5f6e 6f64 655f 7479 7065 2863 6c73 2920  _node_type(cls) 
 0015e8c0: 2d3e 2062 6f6f 6c3a 0a0a 2020 2020 2222  -> bool:..    ""
 0015e8d0: 220a 0a20 2020 2054 7275 6520 6966 2061  "..    True if a
 0015e8e0: 2072 6567 6973 7465 7265 6420 6e6f 6465   registered node
@@ -89774,17 +89774,17 @@
 0015ead0: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 0015eae0: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 0015eaf0: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 0015eb00: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 0015eb10: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 0015eb20: 2e0a 0a63 6c61 7373 2043 6f6d 706f 7369  ...class Composi
 0015eb30: 746f 724e 6f64 654d 6170 5661 6c75 6528  torNodeMapValue(
-0015eb40: 6270 795f 7374 7275 6374 2c20 436f 6d70  bpy_struct, Comp
-0015eb50: 6f73 6974 6f72 4e6f 6465 2c20 4e6f 6465  ositorNode, Node
-0015eb60: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+0015eb40: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+0015eb50: 496e 7465 726e 616c 2c20 436f 6d70 6f73  Internal, Compos
+0015eb60: 6974 6f72 4e6f 6465 2c20 4e6f 6465 293a  itorNode, Node):
 0015eb70: 0a0a 2020 6d61 783a 2074 7970 696e 672e  ..  max: typing.
 0015eb80: 5475 706c 655b 666c 6f61 745d 203d 202e  Tuple[float] = .
 0015eb90: 2e2e 0a0a 2020 6d69 6e3a 2074 7970 696e  ....  min: typin
 0015eba0: 672e 5475 706c 655b 666c 6f61 745d 203d  g.Tuple[float] =
 0015ebb0: 202e 2e2e 0a0a 2020 6f66 6673 6574 3a20   .....  offset: 
 0015ebc0: 7479 7069 6e67 2e54 7570 6c65 5b66 6c6f  typing.Tuple[flo
 0015ebd0: 6174 5d20 3d20 2e2e 2e0a 0a20 2073 697a  at] = .....  siz
@@ -89832,17 +89832,17 @@
 0015ee70: 745f 7375 6263 6c61 7373 5f70 7928 636c  t_subclass_py(cl
 0015ee80: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 0015ee90: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 0015eea0: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 0015eeb0: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 0015eec0: 0a0a 636c 6173 7320 436f 6d70 6f73 6974  ..class Composit
 0015eed0: 6f72 4e6f 6465 4d61 736b 2862 7079 5f73  orNodeMask(bpy_s
-0015eee0: 7472 7563 742c 2043 6f6d 706f 7369 746f  truct, Composito
-0015eef0: 724e 6f64 652c 204e 6f64 652c 204e 6f64  rNode, Node, Nod
-0015ef00: 6549 6e74 6572 6e61 6c29 3a0a 0a20 206d  eInternal):..  m
+0015eee0: 7472 7563 742c 204e 6f64 6549 6e74 6572  truct, NodeInter
+0015eef0: 6e61 6c2c 2043 6f6d 706f 7369 746f 724e  nal, CompositorN
+0015ef00: 6f64 652c 204e 6f64 6529 3a0a 0a20 206d  ode, Node):..  m
 0015ef10: 6173 6b3a 204d 6173 6b20 3d20 2e2e 2e0a  ask: Mask = ....
 0015ef20: 0a20 206d 6f74 696f 6e5f 626c 7572 5f73  .  motion_blur_s
 0015ef30: 616d 706c 6573 3a20 696e 7420 3d20 2e2e  amples: int = ..
 0015ef40: 2e0a 0a20 2022 2222 0a0a 2020 4e75 6d62  ...  """..  Numb
 0015ef50: 6572 206f 6620 6d6f 7469 6f6e 2062 6c75  er of motion blu
 0015ef60: 7220 7361 6d70 6c65 730a 0a20 2022 2222  r samples..  """
 0015ef70: 0a0a 2020 6d6f 7469 6f6e 5f62 6c75 725f  ..  motion_blur_
@@ -89920,17 +89920,17 @@
 0015f3f0: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 0015f400: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 0015f410: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 0015f420: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 0015f430: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 0015f440: 2e0a 0a63 6c61 7373 2043 6f6d 706f 7369  ...class Composi
 0015f450: 746f 724e 6f64 654d 6174 6828 6270 795f  torNodeMath(bpy_
-0015f460: 7374 7275 6374 2c20 436f 6d70 6f73 6974  struct, Composit
-0015f470: 6f72 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  orNode, Node, No
-0015f480: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+0015f460: 7374 7275 6374 2c20 4e6f 6465 496e 7465  struct, NodeInte
+0015f470: 726e 616c 2c20 436f 6d70 6f73 6974 6f72  rnal, Compositor
+0015f480: 4e6f 6465 2c20 4e6f 6465 293a 0a0a 2020  Node, Node):..  
 0015f490: 6f70 6572 6174 696f 6e3a 2073 7472 203d  operation: str =
 0015f4a0: 202e 2e2e 0a0a 2020 7573 655f 636c 616d   .....  use_clam
 0015f4b0: 703a 2062 6f6f 6c20 3d20 2e2e 2e0a 0a20  p: bool = ..... 
 0015f4c0: 2022 2222 0a0a 2020 436c 616d 7020 7265   """..  Clamp re
 0015f4d0: 7375 6c74 206f 6620 7468 6520 6e6f 6465  sult of the node
 0015f4e0: 2074 6f20 302e 3020 746f 2031 2e30 2072   to 0.0 to 1.0 r
 0015f4f0: 616e 6765 0a0a 2020 2222 220a 0a20 2040  ange..  """..  @
@@ -89973,17 +89973,17 @@
 0015f740: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 0015f750: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 0015f760: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 0015f770: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 0015f780: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 0015f790: 2e0a 0a63 6c61 7373 2043 6f6d 706f 7369  ...class Composi
 0015f7a0: 746f 724e 6f64 654d 6978 5247 4228 6270  torNodeMixRGB(bp
-0015f7b0: 795f 7374 7275 6374 2c20 436f 6d70 6f73  y_struct, Compos
-0015f7c0: 6974 6f72 4e6f 6465 2c20 4e6f 6465 2c20  itorNode, Node, 
-0015f7d0: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+0015f7b0: 795f 7374 7275 6374 2c20 4e6f 6465 496e  y_struct, NodeIn
+0015f7c0: 7465 726e 616c 2c20 436f 6d70 6f73 6974  ternal, Composit
+0015f7d0: 6f72 4e6f 6465 2c20 4e6f 6465 293a 0a0a  orNode, Node):..
 0015f7e0: 2020 626c 656e 645f 7479 7065 3a20 7374    blend_type: st
 0015f7f0: 7220 3d20 2e2e 2e0a 0a20 2075 7365 5f61  r = .....  use_a
 0015f800: 6c70 6861 3a20 626f 6f6c 203d 202e 2e2e  lpha: bool = ...
 0015f810: 0a0a 2020 2222 220a 0a20 2049 6e63 6c75  ..  """..  Inclu
 0015f820: 6465 2061 6c70 6861 206f 6620 7365 636f  de alpha of seco
 0015f830: 6e64 2069 6e70 7574 2069 6e20 7468 6973  nd input in this
 0015f840: 206f 7065 7261 7469 6f6e 0a0a 2020 2222   operation..  ""
@@ -90032,17 +90032,17 @@
 0015faf0: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 0015fb00: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 0015fb10: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 0015fb20: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 0015fb30: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 0015fb40: 636c 6173 7320 436f 6d70 6f73 6974 6f72  class Compositor
 0015fb50: 4e6f 6465 4d6f 7669 6543 6c69 7028 6270  NodeMovieClip(bp
-0015fb60: 795f 7374 7275 6374 2c20 436f 6d70 6f73  y_struct, Compos
-0015fb70: 6974 6f72 4e6f 6465 2c20 4e6f 6465 2c20  itorNode, Node, 
-0015fb80: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+0015fb60: 795f 7374 7275 6374 2c20 4e6f 6465 496e  y_struct, NodeIn
+0015fb70: 7465 726e 616c 2c20 436f 6d70 6f73 6974  ternal, Composit
+0015fb80: 6f72 4e6f 6465 2c20 4e6f 6465 293a 0a0a  orNode, Node):..
 0015fb90: 2020 636c 6970 3a20 4d6f 7669 6543 6c69    clip: MovieCli
 0015fba0: 7020 3d20 2e2e 2e0a 0a20 2040 636c 6173  p = .....  @clas
 0015fbb0: 736d 6574 686f 640a 0a20 2064 6566 2069  smethod..  def i
 0015fbc0: 735f 7265 6769 7374 6572 6564 5f6e 6f64  s_registered_nod
 0015fbd0: 655f 7479 7065 2863 6c73 2920 2d3e 2062  e_type(cls) -> b
 0015fbe0: 6f6f 6c3a 0a0a 2020 2020 2222 220a 0a20  ool:..    """.. 
 0015fbf0: 2020 2054 7275 6520 6966 2061 2072 6567     True if a reg
@@ -90080,18 +90080,18 @@
 0015fdf0: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 0015fe00: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 0015fe10: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 0015fe20: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 0015fe30: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 0015fe40: 6c61 7373 2043 6f6d 706f 7369 746f 724e  lass CompositorN
 0015fe50: 6f64 654d 6f76 6965 4469 7374 6f72 7469  odeMovieDistorti
-0015fe60: 6f6e 2862 7079 5f73 7472 7563 742c 2043  on(bpy_struct, C
-0015fe70: 6f6d 706f 7369 746f 724e 6f64 652c 204e  ompositorNode, N
-0015fe80: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-0015fe90: 6c29 3a0a 0a20 2063 6c69 703a 204d 6f76  l):..  clip: Mov
+0015fe60: 6f6e 2862 7079 5f73 7472 7563 742c 204e  on(bpy_struct, N
+0015fe70: 6f64 6549 6e74 6572 6e61 6c2c 2043 6f6d  odeInternal, Com
+0015fe80: 706f 7369 746f 724e 6f64 652c 204e 6f64  positorNode, Nod
+0015fe90: 6529 3a0a 0a20 2063 6c69 703a 204d 6f76  e):..  clip: Mov
 0015fea0: 6965 436c 6970 203d 202e 2e2e 0a0a 2020  ieClip = .....  
 0015feb0: 6469 7374 6f72 7469 6f6e 5f74 7970 653a  distortion_type:
 0015fec0: 2073 7472 203d 202e 2e2e 0a0a 2020 2222   str = .....  ""
 0015fed0: 220a 0a20 2044 6973 746f 7274 696f 6e20  "..  Distortion 
 0015fee0: 746f 2075 7365 2074 6f20 6669 6c74 6572  to use to filter
 0015fef0: 2069 6d61 6765 0a0a 2020 2222 220a 0a20   image..  """.. 
 0015ff00: 2040 636c 6173 736d 6574 686f 640a 0a20   @classmethod.. 
@@ -90133,17 +90133,17 @@
 00160140: 5f67 6574 5f73 7562 636c 6173 735f 7079  _get_subclass_py
 00160150: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 00160160: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 00160170: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 00160180: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 00160190: 2e2e 2e0a 0a63 6c61 7373 2043 6f6d 706f  .....class Compo
 001601a0: 7369 746f 724e 6f64 654e 6f72 6d61 6c28  sitorNodeNormal(
-001601b0: 6270 795f 7374 7275 6374 2c20 436f 6d70  bpy_struct, Comp
-001601c0: 6f73 6974 6f72 4e6f 6465 2c20 4e6f 6465  ositorNode, Node
-001601d0: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+001601b0: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+001601c0: 496e 7465 726e 616c 2c20 436f 6d70 6f73  Internal, Compos
+001601d0: 6974 6f72 4e6f 6465 2c20 4e6f 6465 293a  itorNode, Node):
 001601e0: 0a0a 2020 4063 6c61 7373 6d65 7468 6f64  ..  @classmethod
 001601f0: 0a0a 2020 6465 6620 6973 5f72 6567 6973  ..  def is_regis
 00160200: 7465 7265 645f 6e6f 6465 5f74 7970 6528  tered_node_type(
 00160210: 636c 7329 202d 3e20 626f 6f6c 3a0a 0a20  cls) -> bool:.. 
 00160220: 2020 2022 2222 0a0a 2020 2020 5472 7565     """..    True
 00160230: 2069 6620 6120 7265 6769 7374 6572 6564   if a registered
 00160240: 206e 6f64 6520 7479 7065 0a0a 2020 2020   node type..    
@@ -90180,17 +90180,17 @@
 00160430: 5f70 7928 636c 732c 2069 643a 2073 7472  _py(cls, id: str
 00160440: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 00160450: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 00160460: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 00160470: 2020 202e 2e2e 0a0a 636c 6173 7320 436f     .....class Co
 00160480: 6d70 6f73 6974 6f72 4e6f 6465 4e6f 726d  mpositorNodeNorm
 00160490: 616c 697a 6528 6270 795f 7374 7275 6374  alize(bpy_struct
-001604a0: 2c20 436f 6d70 6f73 6974 6f72 4e6f 6465  , CompositorNode
-001604b0: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-001604c0: 726e 616c 293a 0a0a 2020 4063 6c61 7373  rnal):..  @class
+001604a0: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+001604b0: 436f 6d70 6f73 6974 6f72 4e6f 6465 2c20  CompositorNode, 
+001604c0: 4e6f 6465 293a 0a0a 2020 4063 6c61 7373  Node):..  @class
 001604d0: 6d65 7468 6f64 0a0a 2020 6465 6620 6973  method..  def is
 001604e0: 5f72 6567 6973 7465 7265 645f 6e6f 6465  _registered_node
 001604f0: 5f74 7970 6528 636c 7329 202d 3e20 626f  _type(cls) -> bo
 00160500: 6f6c 3a0a 0a20 2020 2022 2222 0a0a 2020  ol:..    """..  
 00160510: 2020 5472 7565 2069 6620 6120 7265 6769    True if a regi
 00160520: 7374 6572 6564 206e 6f64 6520 7479 7065  stered node type
 00160530: 0a0a 2020 2020 2222 220a 0a20 2020 202e  ..    """..    .
@@ -90226,17 +90226,17 @@
 00160710: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 00160720: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 00160730: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 00160740: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 00160750: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 00160760: 6173 7320 436f 6d70 6f73 6974 6f72 4e6f  ass CompositorNo
 00160770: 6465 4f75 7470 7574 4669 6c65 2862 7079  deOutputFile(bpy
-00160780: 5f73 7472 7563 742c 2043 6f6d 706f 7369  _struct, Composi
-00160790: 746f 724e 6f64 652c 204e 6f64 652c 204e  torNode, Node, N
-001607a0: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+00160780: 5f73 7472 7563 742c 204e 6f64 6549 6e74  _struct, NodeInt
+00160790: 6572 6e61 6c2c 2043 6f6d 706f 7369 746f  ernal, Composito
+001607a0: 724e 6f64 652c 204e 6f64 6529 3a0a 0a20  rNode, Node):.. 
 001607b0: 2061 6374 6976 655f 696e 7075 745f 696e   active_input_in
 001607c0: 6465 783a 2069 6e74 203d 202e 2e2e 0a0a  dex: int = .....
 001607d0: 2020 2222 220a 0a20 2041 6374 6976 6520    """..  Active 
 001607e0: 696e 7075 7420 696e 6465 7820 696e 2064  input index in d
 001607f0: 6574 6169 6c73 2076 6965 7720 6c69 7374  etails view list
 00160800: 0a0a 2020 2222 220a 0a20 2062 6173 655f  ..  """..  base_
 00160810: 7061 7468 3a20 7374 7220 3d20 2e2e 2e0a  path: str = ....
@@ -90307,17 +90307,17 @@
 00160c20: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 00160c30: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 00160c40: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 00160c50: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 00160c60: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 00160c70: 636c 6173 7320 436f 6d70 6f73 6974 6f72  class Compositor
 00160c80: 4e6f 6465 5069 7865 6c61 7465 2862 7079  NodePixelate(bpy
-00160c90: 5f73 7472 7563 742c 2043 6f6d 706f 7369  _struct, Composi
-00160ca0: 746f 724e 6f64 652c 204e 6f64 652c 204e  torNode, Node, N
-00160cb0: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+00160c90: 5f73 7472 7563 742c 204e 6f64 6549 6e74  _struct, NodeInt
+00160ca0: 6572 6e61 6c2c 2043 6f6d 706f 7369 746f  ernal, Composito
+00160cb0: 724e 6f64 652c 204e 6f64 6529 3a0a 0a20  rNode, Node):.. 
 00160cc0: 2040 636c 6173 736d 6574 686f 640a 0a20   @classmethod.. 
 00160cd0: 2064 6566 2069 735f 7265 6769 7374 6572   def is_register
 00160ce0: 6564 5f6e 6f64 655f 7479 7065 2863 6c73  ed_node_type(cls
 00160cf0: 2920 2d3e 2062 6f6f 6c3a 0a0a 2020 2020  ) -> bool:..    
 00160d00: 2222 220a 0a20 2020 2054 7275 6520 6966  """..    True if
 00160d10: 2061 2072 6567 6973 7465 7265 6420 6e6f   a registered no
 00160d20: 6465 2074 7970 650a 0a20 2020 2022 2222  de type..    """
@@ -90354,17 +90354,17 @@
 00160f10: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 00160f20: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 00160f30: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 00160f40: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 00160f50: 2e2e 2e0a 0a63 6c61 7373 2043 6f6d 706f  .....class Compo
 00160f60: 7369 746f 724e 6f64 6550 6c61 6e65 5472  sitorNodePlaneTr
 00160f70: 6163 6b44 6566 6f72 6d28 6270 795f 7374  ackDeform(bpy_st
-00160f80: 7275 6374 2c20 436f 6d70 6f73 6974 6f72  ruct, Compositor
-00160f90: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-00160fa0: 496e 7465 726e 616c 293a 0a0a 2020 636c  Internal):..  cl
+00160f80: 7275 6374 2c20 4e6f 6465 496e 7465 726e  ruct, NodeIntern
+00160f90: 616c 2c20 436f 6d70 6f73 6974 6f72 4e6f  al, CompositorNo
+00160fa0: 6465 2c20 4e6f 6465 293a 0a0a 2020 636c  de, Node):..  cl
 00160fb0: 6970 3a20 4d6f 7669 6543 6c69 7020 3d20  ip: MovieClip = 
 00160fc0: 2e2e 2e0a 0a20 206d 6f74 696f 6e5f 626c  .....  motion_bl
 00160fd0: 7572 5f73 616d 706c 6573 3a20 696e 7420  ur_samples: int 
 00160fe0: 3d20 2e2e 2e0a 0a20 2022 2222 0a0a 2020  = .....  """..  
 00160ff0: 4e75 6d62 6572 206f 6620 6d6f 7469 6f6e  Number of motion
 00161000: 2062 6c75 7220 7361 6d70 6c65 730a 0a20   blur samples.. 
 00161010: 2022 2222 0a0a 2020 6d6f 7469 6f6e 5f62   """..  motion_b
@@ -90422,17 +90422,17 @@
 00161350: 6765 745f 7375 6263 6c61 7373 5f70 7928  get_subclass_py(
 00161360: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 00161370: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 00161380: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 00161390: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 001613a0: 2e2e 0a0a 636c 6173 7320 436f 6d70 6f73  ....class Compos
 001613b0: 6974 6f72 4e6f 6465 506f 7374 6572 697a  itorNodePosteriz
-001613c0: 6528 6270 795f 7374 7275 6374 2c20 436f  e(bpy_struct, Co
-001613d0: 6d70 6f73 6974 6f72 4e6f 6465 2c20 4e6f  mpositorNode, No
-001613e0: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+001613c0: 6528 6270 795f 7374 7275 6374 2c20 4e6f  e(bpy_struct, No
+001613d0: 6465 496e 7465 726e 616c 2c20 436f 6d70  deInternal, Comp
+001613e0: 6f73 6974 6f72 4e6f 6465 2c20 4e6f 6465  ositorNode, Node
 001613f0: 293a 0a0a 2020 4063 6c61 7373 6d65 7468  ):..  @classmeth
 00161400: 6f64 0a0a 2020 6465 6620 6973 5f72 6567  od..  def is_reg
 00161410: 6973 7465 7265 645f 6e6f 6465 5f74 7970  istered_node_typ
 00161420: 6528 636c 7329 202d 3e20 626f 6f6c 3a0a  e(cls) -> bool:.
 00161430: 0a20 2020 2022 2222 0a0a 2020 2020 5472  .    """..    Tr
 00161440: 7565 2069 6620 6120 7265 6769 7374 6572  ue if a register
 00161450: 6564 206e 6f64 6520 7479 7065 0a0a 2020  ed node type..  
@@ -90469,17 +90469,17 @@
 00161640: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 00161650: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 00161660: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 00161670: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 00161680: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 00161690: 436f 6d70 6f73 6974 6f72 4e6f 6465 5072  CompositorNodePr
 001616a0: 656d 756c 4b65 7928 6270 795f 7374 7275  emulKey(bpy_stru
-001616b0: 6374 2c20 436f 6d70 6f73 6974 6f72 4e6f  ct, CompositorNo
-001616c0: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-001616d0: 7465 726e 616c 293a 0a0a 2020 6d61 7070  ternal):..  mapp
+001616b0: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+001616c0: 2c20 436f 6d70 6f73 6974 6f72 4e6f 6465  , CompositorNode
+001616d0: 2c20 4e6f 6465 293a 0a0a 2020 6d61 7070  , Node):..  mapp
 001616e0: 696e 673a 2073 7472 203d 202e 2e2e 0a0a  ing: str = .....
 001616f0: 2020 2222 220a 0a20 2043 6f6e 7665 7273    """..  Convers
 00161700: 696f 6e20 6265 7477 6565 6e20 7072 656d  ion between prem
 00161710: 756c 7469 706c 6965 6420 616c 7068 6120  ultiplied alpha 
 00161720: 616e 6420 6b65 7920 616c 7068 610a 0a20  and key alpha.. 
 00161730: 202a 2060 6053 5452 4149 4748 545f 544f   * ``STRAIGHT_TO
 00161740: 5f50 5245 4d55 4c60 600a 546f 2050 7265  _PREMUL``.To Pre
@@ -90531,17 +90531,17 @@
 00161a20: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 00161a30: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 00161a40: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 00161a50: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 00161a60: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 00161a70: 7373 2043 6f6d 706f 7369 746f 724e 6f64  ss CompositorNod
 00161a80: 6552 4742 2862 7079 5f73 7472 7563 742c  eRGB(bpy_struct,
-00161a90: 2043 6f6d 706f 7369 746f 724e 6f64 652c   CompositorNode,
-00161aa0: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-00161ab0: 6e61 6c29 3a0a 0a20 2040 636c 6173 736d  nal):..  @classm
+00161a90: 204e 6f64 6549 6e74 6572 6e61 6c2c 2043   NodeInternal, C
+00161aa0: 6f6d 706f 7369 746f 724e 6f64 652c 204e  ompositorNode, N
+00161ab0: 6f64 6529 3a0a 0a20 2040 636c 6173 736d  ode):..  @classm
 00161ac0: 6574 686f 640a 0a20 2064 6566 2069 735f  ethod..  def is_
 00161ad0: 7265 6769 7374 6572 6564 5f6e 6f64 655f  registered_node_
 00161ae0: 7479 7065 2863 6c73 2920 2d3e 2062 6f6f  type(cls) -> boo
 00161af0: 6c3a 0a0a 2020 2020 2222 220a 0a20 2020  l:..    """..   
 00161b00: 2054 7275 6520 6966 2061 2072 6567 6973   True if a regis
 00161b10: 7465 7265 6420 6e6f 6465 2074 7970 650a  tered node type.
 00161b20: 0a20 2020 2022 2222 0a0a 2020 2020 2e2e  .    """..    ..
@@ -90577,17 +90577,17 @@
 00161d00: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 00161d10: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 00161d20: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 00161d30: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 00161d40: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 00161d50: 7373 2043 6f6d 706f 7369 746f 724e 6f64  ss CompositorNod
 00161d60: 6552 4742 546f 4257 2862 7079 5f73 7472  eRGBToBW(bpy_str
-00161d70: 7563 742c 2043 6f6d 706f 7369 746f 724e  uct, CompositorN
-00161d80: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-00161d90: 6e74 6572 6e61 6c29 3a0a 0a20 2040 636c  nternal):..  @cl
+00161d70: 7563 742c 204e 6f64 6549 6e74 6572 6e61  uct, NodeInterna
+00161d80: 6c2c 2043 6f6d 706f 7369 746f 724e 6f64  l, CompositorNod
+00161d90: 652c 204e 6f64 6529 3a0a 0a20 2040 636c  e, Node):..  @cl
 00161da0: 6173 736d 6574 686f 640a 0a20 2064 6566  assmethod..  def
 00161db0: 2069 735f 7265 6769 7374 6572 6564 5f6e   is_registered_n
 00161dc0: 6f64 655f 7479 7065 2863 6c73 2920 2d3e  ode_type(cls) ->
 00161dd0: 2062 6f6f 6c3a 0a0a 2020 2020 2222 220a   bool:..    """.
 00161de0: 0a20 2020 2054 7275 6520 6966 2061 2072  .    True if a r
 00161df0: 6567 6973 7465 7265 6420 6e6f 6465 2074  egistered node t
 00161e00: 7970 650a 0a20 2020 2022 2222 0a0a 2020  ype..    """..  
@@ -90623,17 +90623,17 @@
 00161fe0: 5f73 7562 636c 6173 735f 7079 2863 6c73  _subclass_py(cls
 00161ff0: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 00162000: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 00162010: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 00162020: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 00162030: 0a63 6c61 7373 2043 6f6d 706f 7369 746f  .class Composito
 00162040: 724e 6f64 6552 4c61 7965 7273 2862 7079  rNodeRLayers(bpy
-00162050: 5f73 7472 7563 742c 2043 6f6d 706f 7369  _struct, Composi
-00162060: 746f 724e 6f64 652c 204e 6f64 652c 204e  torNode, Node, N
-00162070: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+00162050: 5f73 7472 7563 742c 204e 6f64 6549 6e74  _struct, NodeInt
+00162060: 6572 6e61 6c2c 2043 6f6d 706f 7369 746f  ernal, Composito
+00162070: 724e 6f64 652c 204e 6f64 6529 3a0a 0a20  rNode, Node):.. 
 00162080: 206c 6179 6572 3a20 7374 7220 3d20 2e2e   layer: str = ..
 00162090: 2e0a 0a20 2073 6365 6e65 3a20 5363 656e  ...  scene: Scen
 001620a0: 6520 3d20 2e2e 2e0a 0a20 2040 636c 6173  e = .....  @clas
 001620b0: 736d 6574 686f 640a 0a20 2064 6566 2069  smethod..  def i
 001620c0: 735f 7265 6769 7374 6572 6564 5f6e 6f64  s_registered_nod
 001620d0: 655f 7479 7065 2863 6c73 2920 2d3e 2062  e_type(cls) -> b
 001620e0: 6f6f 6c3a 0a0a 2020 2020 2222 220a 0a20  ool:..    """.. 
@@ -90672,17 +90672,17 @@
 001622f0: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 00162300: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 00162310: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 00162320: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 00162330: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 00162340: 6c61 7373 2043 6f6d 706f 7369 746f 724e  lass CompositorN
 00162350: 6f64 6552 6f74 6174 6528 6270 795f 7374  odeRotate(bpy_st
-00162360: 7275 6374 2c20 436f 6d70 6f73 6974 6f72  ruct, Compositor
-00162370: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-00162380: 496e 7465 726e 616c 293a 0a0a 2020 6669  Internal):..  fi
+00162360: 7275 6374 2c20 4e6f 6465 496e 7465 726e  ruct, NodeIntern
+00162370: 616c 2c20 436f 6d70 6f73 6974 6f72 4e6f  al, CompositorNo
+00162380: 6465 2c20 4e6f 6465 293a 0a0a 2020 6669  de, Node):..  fi
 00162390: 6c74 6572 5f74 7970 653a 2073 7472 203d  lter_type: str =
 001623a0: 202e 2e2e 0a0a 2020 2222 220a 0a20 204d   .....  """..  M
 001623b0: 6574 686f 6420 746f 2075 7365 2074 6f20  ethod to use to 
 001623c0: 6669 6c74 6572 2072 6f74 6174 696f 6e0a  filter rotation.
 001623d0: 0a20 2022 2222 0a0a 2020 4063 6c61 7373  .  """..  @class
 001623e0: 6d65 7468 6f64 0a0a 2020 6465 6620 6973  method..  def is
 001623f0: 5f72 6567 6973 7465 7265 645f 6e6f 6465  _registered_node
@@ -90723,17 +90723,17 @@
 00162620: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 00162630: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 00162640: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 00162650: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 00162660: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 00162670: 6173 7320 436f 6d70 6f73 6974 6f72 4e6f  ass CompositorNo
 00162680: 6465 5363 616c 6528 6270 795f 7374 7275  deScale(bpy_stru
-00162690: 6374 2c20 436f 6d70 6f73 6974 6f72 4e6f  ct, CompositorNo
-001626a0: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-001626b0: 7465 726e 616c 293a 0a0a 2020 6672 616d  ternal):..  fram
+00162690: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+001626a0: 2c20 436f 6d70 6f73 6974 6f72 4e6f 6465  , CompositorNode
+001626b0: 2c20 4e6f 6465 293a 0a0a 2020 6672 616d  , Node):..  fram
 001626c0: 655f 6d65 7468 6f64 3a20 7374 7220 3d20  e_method: str = 
 001626d0: 2e2e 2e0a 0a20 2022 2222 0a0a 2020 486f  .....  """..  Ho
 001626e0: 7720 7468 6520 696d 6167 6520 6669 7473  w the image fits
 001626f0: 2069 6e20 7468 6520 6361 6d65 7261 2066   in the camera f
 00162700: 7261 6d65 0a0a 2020 2222 220a 0a20 206f  rame..  """..  o
 00162710: 6666 7365 745f 783a 2066 6c6f 6174 203d  ffset_x: float =
 00162720: 202e 2e2e 0a0a 2020 2222 220a 0a20 204f   .....  """..  O
@@ -90790,17 +90790,17 @@
 00162a50: 745f 7375 6263 6c61 7373 5f70 7928 636c  t_subclass_py(cl
 00162a60: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 00162a70: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 00162a80: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 00162a90: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 00162aa0: 0a0a 636c 6173 7320 436f 6d70 6f73 6974  ..class Composit
 00162ab0: 6f72 4e6f 6465 5363 656e 6554 696d 6528  orNodeSceneTime(
-00162ac0: 6270 795f 7374 7275 6374 2c20 436f 6d70  bpy_struct, Comp
-00162ad0: 6f73 6974 6f72 4e6f 6465 2c20 4e6f 6465  ositorNode, Node
-00162ae0: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+00162ac0: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+00162ad0: 496e 7465 726e 616c 2c20 436f 6d70 6f73  Internal, Compos
+00162ae0: 6974 6f72 4e6f 6465 2c20 4e6f 6465 293a  itorNode, Node):
 00162af0: 0a0a 2020 4063 6c61 7373 6d65 7468 6f64  ..  @classmethod
 00162b00: 0a0a 2020 6465 6620 6973 5f72 6567 6973  ..  def is_regis
 00162b10: 7465 7265 645f 6e6f 6465 5f74 7970 6528  tered_node_type(
 00162b20: 636c 7329 202d 3e20 626f 6f6c 3a0a 0a20  cls) -> bool:.. 
 00162b30: 2020 2022 2222 0a0a 2020 2020 5472 7565     """..    True
 00162b40: 2069 6620 6120 7265 6769 7374 6572 6564   if a registered
 00162b50: 206e 6f64 6520 7479 7065 0a0a 2020 2020   node type..    
@@ -90837,17 +90837,17 @@
 00162d40: 5f70 7928 636c 732c 2069 643a 2073 7472  _py(cls, id: str
 00162d50: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 00162d60: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 00162d70: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 00162d80: 2020 202e 2e2e 0a0a 636c 6173 7320 436f     .....class Co
 00162d90: 6d70 6f73 6974 6f72 4e6f 6465 5365 7048  mpositorNodeSepH
 00162da0: 5356 4128 6270 795f 7374 7275 6374 2c20  SVA(bpy_struct, 
-00162db0: 436f 6d70 6f73 6974 6f72 4e6f 6465 2c20  CompositorNode, 
-00162dc0: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-00162dd0: 616c 293a 0a0a 2020 4063 6c61 7373 6d65  al):..  @classme
+00162db0: 4e6f 6465 496e 7465 726e 616c 2c20 436f  NodeInternal, Co
+00162dc0: 6d70 6f73 6974 6f72 4e6f 6465 2c20 4e6f  mpositorNode, No
+00162dd0: 6465 293a 0a0a 2020 4063 6c61 7373 6d65  de):..  @classme
 00162de0: 7468 6f64 0a0a 2020 6465 6620 6973 5f72  thod..  def is_r
 00162df0: 6567 6973 7465 7265 645f 6e6f 6465 5f74  egistered_node_t
 00162e00: 7970 6528 636c 7329 202d 3e20 626f 6f6c  ype(cls) -> bool
 00162e10: 3a0a 0a20 2020 2022 2222 0a0a 2020 2020  :..    """..    
 00162e20: 5472 7565 2069 6620 6120 7265 6769 7374  True if a regist
 00162e30: 6572 6564 206e 6f64 6520 7479 7065 0a0a  ered node type..
 00162e40: 2020 2020 2222 220a 0a20 2020 202e 2e2e      """..    ...
@@ -90883,17 +90883,17 @@
 00163020: 6c61 7373 5f70 7928 636c 732c 2069 643a  lass_py(cls, id:
 00163030: 2073 7472 2c20 6465 6661 756c 743a 2074   str, default: t
 00163040: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 00163050: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 00163060: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 00163070: 7320 436f 6d70 6f73 6974 6f72 4e6f 6465  s CompositorNode
 00163080: 5365 7052 4742 4128 6270 795f 7374 7275  SepRGBA(bpy_stru
-00163090: 6374 2c20 436f 6d70 6f73 6974 6f72 4e6f  ct, CompositorNo
-001630a0: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-001630b0: 7465 726e 616c 293a 0a0a 2020 4063 6c61  ternal):..  @cla
+00163090: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+001630a0: 2c20 436f 6d70 6f73 6974 6f72 4e6f 6465  , CompositorNode
+001630b0: 2c20 4e6f 6465 293a 0a0a 2020 4063 6c61  , Node):..  @cla
 001630c0: 7373 6d65 7468 6f64 0a0a 2020 6465 6620  ssmethod..  def 
 001630d0: 6973 5f72 6567 6973 7465 7265 645f 6e6f  is_registered_no
 001630e0: 6465 5f74 7970 6528 636c 7329 202d 3e20  de_type(cls) -> 
 001630f0: 626f 6f6c 3a0a 0a20 2020 2022 2222 0a0a  bool:..    """..
 00163100: 2020 2020 5472 7565 2069 6620 6120 7265      True if a re
 00163110: 6769 7374 6572 6564 206e 6f64 6520 7479  gistered node ty
 00163120: 7065 0a0a 2020 2020 2222 220a 0a20 2020  pe..    """..   
@@ -90929,17 +90929,17 @@
 00163300: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 00163310: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 00163320: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 00163330: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 00163340: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 00163350: 636c 6173 7320 436f 6d70 6f73 6974 6f72  class Compositor
 00163360: 4e6f 6465 5365 7059 4343 4128 6270 795f  NodeSepYCCA(bpy_
-00163370: 7374 7275 6374 2c20 436f 6d70 6f73 6974  struct, Composit
-00163380: 6f72 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  orNode, Node, No
-00163390: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+00163370: 7374 7275 6374 2c20 4e6f 6465 496e 7465  struct, NodeInte
+00163380: 726e 616c 2c20 436f 6d70 6f73 6974 6f72  rnal, Compositor
+00163390: 4e6f 6465 2c20 4e6f 6465 293a 0a0a 2020  Node, Node):..  
 001633a0: 6d6f 6465 3a20 7374 7220 3d20 2e2e 2e0a  mode: str = ....
 001633b0: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
 001633c0: 0a20 2064 6566 2069 735f 7265 6769 7374  .  def is_regist
 001633d0: 6572 6564 5f6e 6f64 655f 7479 7065 2863  ered_node_type(c
 001633e0: 6c73 2920 2d3e 2062 6f6f 6c3a 0a0a 2020  ls) -> bool:..  
 001633f0: 2020 2222 220a 0a20 2020 2054 7275 6520    """..    True 
 00163400: 6966 2061 2072 6567 6973 7465 7265 6420  if a registered 
@@ -90976,18 +90976,18 @@
 001635f0: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 00163600: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 00163610: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 00163620: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 00163630: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 00163640: 2020 2e2e 2e0a 0a63 6c61 7373 2043 6f6d    .....class Com
 00163650: 706f 7369 746f 724e 6f64 6553 6570 5955  positorNodeSepYU
-00163660: 5641 2862 7079 5f73 7472 7563 742c 2043  VA(bpy_struct, C
-00163670: 6f6d 706f 7369 746f 724e 6f64 652c 204e  ompositorNode, N
-00163680: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-00163690: 6c29 3a0a 0a20 2040 636c 6173 736d 6574  l):..  @classmet
+00163660: 5641 2862 7079 5f73 7472 7563 742c 204e  VA(bpy_struct, N
+00163670: 6f64 6549 6e74 6572 6e61 6c2c 2043 6f6d  odeInternal, Com
+00163680: 706f 7369 746f 724e 6f64 652c 204e 6f64  positorNode, Nod
+00163690: 6529 3a0a 0a20 2040 636c 6173 736d 6574  e):..  @classmet
 001636a0: 686f 640a 0a20 2064 6566 2069 735f 7265  hod..  def is_re
 001636b0: 6769 7374 6572 6564 5f6e 6f64 655f 7479  gistered_node_ty
 001636c0: 7065 2863 6c73 2920 2d3e 2062 6f6f 6c3a  pe(cls) -> bool:
 001636d0: 0a0a 2020 2020 2222 220a 0a20 2020 2054  ..    """..    T
 001636e0: 7275 6520 6966 2061 2072 6567 6973 7465  rue if a registe
 001636f0: 7265 6420 6e6f 6465 2074 7970 650a 0a20  red node type.. 
 00163700: 2020 2022 2222 0a0a 2020 2020 2e2e 2e0a     """..    ....
@@ -91023,17 +91023,17 @@
 001638e0: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 001638f0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 00163900: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 00163910: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 00163920: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 00163930: 2043 6f6d 706f 7369 746f 724e 6f64 6553   CompositorNodeS
 00163940: 6570 6172 6174 6543 6f6c 6f72 2862 7079  eparateColor(bpy
-00163950: 5f73 7472 7563 742c 2043 6f6d 706f 7369  _struct, Composi
-00163960: 746f 724e 6f64 652c 204e 6f64 652c 204e  torNode, Node, N
-00163970: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+00163950: 5f73 7472 7563 742c 204e 6f64 6549 6e74  _struct, NodeInt
+00163960: 6572 6e61 6c2c 2043 6f6d 706f 7369 746f  ernal, Composito
+00163970: 724e 6f64 652c 204e 6f64 6529 3a0a 0a20  rNode, Node):.. 
 00163980: 206d 6f64 653a 2073 7472 203d 202e 2e2e   mode: str = ...
 00163990: 0a0a 2020 2222 220a 0a20 204d 6f64 6520  ..  """..  Mode 
 001639a0: 6f66 2063 6f6c 6f72 2070 726f 6365 7373  of color process
 001639b0: 696e 670a 0a20 202a 2060 6052 4742 6060  ing..  * ``RGB``
 001639c0: 0a52 4742 202d 2d20 5573 6520 5247 4220  .RGB -- Use RGB 
 001639d0: 636f 6c6f 7220 7072 6f63 6573 7369 6e67  color processing
 001639e0: 2e0a 0a20 202a 2060 6048 5356 6060 0a48  ...  * ``HSV``.H
@@ -91093,17 +91093,17 @@
 00163d40: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 00163d50: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 00163d60: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 00163d70: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 00163d80: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 00163d90: 2043 6f6d 706f 7369 746f 724e 6f64 6553   CompositorNodeS
 00163da0: 6570 6172 6174 6558 595a 2862 7079 5f73  eparateXYZ(bpy_s
-00163db0: 7472 7563 742c 2043 6f6d 706f 7369 746f  truct, Composito
-00163dc0: 724e 6f64 652c 204e 6f64 652c 204e 6f64  rNode, Node, Nod
-00163dd0: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2040  eInternal):..  @
+00163db0: 7472 7563 742c 204e 6f64 6549 6e74 6572  truct, NodeInter
+00163dc0: 6e61 6c2c 2043 6f6d 706f 7369 746f 724e  nal, CompositorN
+00163dd0: 6f64 652c 204e 6f64 6529 3a0a 0a20 2040  ode, Node):..  @
 00163de0: 636c 6173 736d 6574 686f 640a 0a20 2064  classmethod..  d
 00163df0: 6566 2069 735f 7265 6769 7374 6572 6564  ef is_registered
 00163e00: 5f6e 6f64 655f 7479 7065 2863 6c73 2920  _node_type(cls) 
 00163e10: 2d3e 2062 6f6f 6c3a 0a0a 2020 2020 2222  -> bool:..    ""
 00163e20: 220a 0a20 2020 2054 7275 6520 6966 2061  "..    True if a
 00163e30: 2072 6567 6973 7465 7265 6420 6e6f 6465   registered node
 00163e40: 2074 7970 650a 0a20 2020 2022 2222 0a0a   type..    """..
@@ -91139,17 +91139,17 @@
 00164020: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 00164030: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 00164040: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 00164050: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 00164060: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 00164070: 2e0a 0a63 6c61 7373 2043 6f6d 706f 7369  ...class Composi
 00164080: 746f 724e 6f64 6553 6574 416c 7068 6128  torNodeSetAlpha(
-00164090: 6270 795f 7374 7275 6374 2c20 436f 6d70  bpy_struct, Comp
-001640a0: 6f73 6974 6f72 4e6f 6465 2c20 4e6f 6465  ositorNode, Node
-001640b0: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+00164090: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+001640a0: 496e 7465 726e 616c 2c20 436f 6d70 6f73  Internal, Compos
+001640b0: 6974 6f72 4e6f 6465 2c20 4e6f 6465 293a  itorNode, Node):
 001640c0: 0a0a 2020 6d6f 6465 3a20 7374 7220 3d20  ..  mode: str = 
 001640d0: 2e2e 2e0a 0a20 2022 2222 0a0a 2020 2a20  .....  """..  * 
 001640e0: 6060 4150 504c 5960 600a 4170 706c 7920  ``APPLY``.Apply 
 001640f0: 4d61 736b 202d 2d20 4d75 6c74 6970 6c79  Mask -- Multiply
 00164100: 2074 6865 2069 6e70 7574 2069 6d61 6765   the input image
 00164110: 2773 2052 4742 4120 6368 616e 6e65 6c73  's RGBA channels
 00164120: 2062 7920 7468 6520 616c 7068 6120 696e   by the alpha in
@@ -91200,18 +91200,18 @@
 001643f0: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 00164400: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 00164410: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 00164420: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 00164430: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 00164440: 2e0a 0a63 6c61 7373 2043 6f6d 706f 7369  ...class Composi
 00164450: 746f 724e 6f64 6553 706c 6974 5669 6577  torNodeSplitView
-00164460: 6572 2862 7079 5f73 7472 7563 742c 2043  er(bpy_struct, C
-00164470: 6f6d 706f 7369 746f 724e 6f64 652c 204e  ompositorNode, N
-00164480: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-00164490: 6c29 3a0a 0a20 2061 7869 733a 2073 7472  l):..  axis: str
+00164460: 6572 2862 7079 5f73 7472 7563 742c 204e  er(bpy_struct, N
+00164470: 6f64 6549 6e74 6572 6e61 6c2c 2043 6f6d  odeInternal, Com
+00164480: 706f 7369 746f 724e 6f64 652c 204e 6f64  positorNode, Nod
+00164490: 6529 3a0a 0a20 2061 7869 733a 2073 7472  e):..  axis: str
 001644a0: 203d 202e 2e2e 0a0a 2020 6661 6374 6f72   = .....  factor
 001644b0: 3a20 696e 7420 3d20 2e2e 2e0a 0a20 2040  : int = .....  @
 001644c0: 636c 6173 736d 6574 686f 640a 0a20 2064  classmethod..  d
 001644d0: 6566 2069 735f 7265 6769 7374 6572 6564  ef is_registered
 001644e0: 5f6e 6f64 655f 7479 7065 2863 6c73 2920  _node_type(cls) 
 001644f0: 2d3e 2062 6f6f 6c3a 0a0a 2020 2020 2222  -> bool:..    ""
 00164500: 220a 0a20 2020 2054 7275 6520 6966 2061  "..    True if a
@@ -91249,17 +91249,17 @@
 00164700: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 00164710: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 00164720: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 00164730: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 00164740: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 00164750: 2e0a 0a63 6c61 7373 2043 6f6d 706f 7369  ...class Composi
 00164760: 746f 724e 6f64 6553 7461 6269 6c69 7a65  torNodeStabilize
-00164770: 2862 7079 5f73 7472 7563 742c 2043 6f6d  (bpy_struct, Com
-00164780: 706f 7369 746f 724e 6f64 652c 204e 6f64  positorNode, Nod
-00164790: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+00164770: 2862 7079 5f73 7472 7563 742c 204e 6f64  (bpy_struct, Nod
+00164780: 6549 6e74 6572 6e61 6c2c 2043 6f6d 706f  eInternal, Compo
+00164790: 7369 746f 724e 6f64 652c 204e 6f64 6529  sitorNode, Node)
 001647a0: 3a0a 0a20 2063 6c69 703a 204d 6f76 6965  :..  clip: Movie
 001647b0: 436c 6970 203d 202e 2e2e 0a0a 2020 6669  Clip = .....  fi
 001647c0: 6c74 6572 5f74 7970 653a 2073 7472 203d  lter_type: str =
 001647d0: 202e 2e2e 0a0a 2020 2222 220a 0a20 204d   .....  """..  M
 001647e0: 6574 686f 6420 746f 2075 7365 2074 6f20  ethod to use to 
 001647f0: 6669 6c74 6572 2073 7461 6269 6c69 7a61  filter stabiliza
 00164800: 7469 6f6e 0a0a 2020 2222 220a 0a20 2069  tion..  """..  i
@@ -91308,17 +91308,17 @@
 00164ab0: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 00164ac0: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 00164ad0: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 00164ae0: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 00164af0: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 00164b00: 2e0a 0a63 6c61 7373 2043 6f6d 706f 7369  ...class Composi
 00164b10: 746f 724e 6f64 6553 756e 4265 616d 7328  torNodeSunBeams(
-00164b20: 6270 795f 7374 7275 6374 2c20 436f 6d70  bpy_struct, Comp
-00164b30: 6f73 6974 6f72 4e6f 6465 2c20 4e6f 6465  ositorNode, Node
-00164b40: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+00164b20: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+00164b30: 496e 7465 726e 616c 2c20 436f 6d70 6f73  Internal, Compos
+00164b40: 6974 6f72 4e6f 6465 2c20 4e6f 6465 293a  itorNode, Node):
 00164b50: 0a0a 2020 7261 795f 6c65 6e67 7468 3a20  ..  ray_length: 
 00164b60: 666c 6f61 7420 3d20 2e2e 2e0a 0a20 2022  float = .....  "
 00164b70: 2222 0a0a 2020 4c65 6e67 7468 206f 6620  ""..  Length of 
 00164b80: 7261 7973 2061 7320 6120 6661 6374 6f72  rays as a factor
 00164b90: 206f 6620 7468 6520 696d 6167 6520 7369   of the image si
 00164ba0: 7a65 0a0a 2020 2222 220a 0a20 2073 6f75  ze..  """..  sou
 00164bb0: 7263 653a 2074 7970 696e 672e 5475 706c  rce: typing.Tupl
@@ -91368,17 +91368,17 @@
 00164e70: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 00164e80: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 00164e90: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 00164ea0: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 00164eb0: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 00164ec0: 7373 2043 6f6d 706f 7369 746f 724e 6f64  ss CompositorNod
 00164ed0: 6553 7769 7463 6828 6270 795f 7374 7275  eSwitch(bpy_stru
-00164ee0: 6374 2c20 436f 6d70 6f73 6974 6f72 4e6f  ct, CompositorNo
-00164ef0: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-00164f00: 7465 726e 616c 293a 0a0a 2020 6368 6563  ternal):..  chec
+00164ee0: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+00164ef0: 2c20 436f 6d70 6f73 6974 6f72 4e6f 6465  , CompositorNode
+00164f00: 2c20 4e6f 6465 293a 0a0a 2020 6368 6563  , Node):..  chec
 00164f10: 6b3a 2062 6f6f 6c20 3d20 2e2e 2e0a 0a20  k: bool = ..... 
 00164f20: 2022 2222 0a0a 2020 4f66 663a 2066 6972   """..  Off: fir
 00164f30: 7374 2073 6f63 6b65 742c 204f 6e3a 2073  st socket, On: s
 00164f40: 6563 6f6e 6420 736f 636b 6574 0a0a 2020  econd socket..  
 00164f50: 2222 220a 0a20 2040 636c 6173 736d 6574  """..  @classmet
 00164f60: 686f 640a 0a20 2064 6566 2069 735f 7265  hod..  def is_re
 00164f70: 6769 7374 6572 6564 5f6e 6f64 655f 7479  gistered_node_ty
@@ -91419,17 +91419,17 @@
 001651a0: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 001651b0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 001651c0: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 001651d0: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 001651e0: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 001651f0: 2043 6f6d 706f 7369 746f 724e 6f64 6553   CompositorNodeS
 00165200: 7769 7463 6856 6965 7728 6270 795f 7374  witchView(bpy_st
-00165210: 7275 6374 2c20 436f 6d70 6f73 6974 6f72  ruct, Compositor
-00165220: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-00165230: 496e 7465 726e 616c 293a 0a0a 2020 4063  Internal):..  @c
+00165210: 7275 6374 2c20 4e6f 6465 496e 7465 726e  ruct, NodeIntern
+00165220: 616c 2c20 436f 6d70 6f73 6974 6f72 4e6f  al, CompositorNo
+00165230: 6465 2c20 4e6f 6465 293a 0a0a 2020 4063  de, Node):..  @c
 00165240: 6c61 7373 6d65 7468 6f64 0a0a 2020 6465  lassmethod..  de
 00165250: 6620 6973 5f72 6567 6973 7465 7265 645f  f is_registered_
 00165260: 6e6f 6465 5f74 7970 6528 636c 7329 202d  node_type(cls) -
 00165270: 3e20 626f 6f6c 3a0a 0a20 2020 2022 2222  > bool:..    """
 00165280: 0a0a 2020 2020 5472 7565 2069 6620 6120  ..    True if a 
 00165290: 7265 6769 7374 6572 6564 206e 6f64 6520  registered node 
 001652a0: 7479 7065 0a0a 2020 2020 2222 220a 0a20  type..    """.. 
@@ -91465,17 +91465,17 @@
 00165480: 745f 7375 6263 6c61 7373 5f70 7928 636c  t_subclass_py(cl
 00165490: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 001654a0: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 001654b0: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 001654c0: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 001654d0: 0a0a 636c 6173 7320 436f 6d70 6f73 6974  ..class Composit
 001654e0: 6f72 4e6f 6465 5465 7874 7572 6528 6270  orNodeTexture(bp
-001654f0: 795f 7374 7275 6374 2c20 436f 6d70 6f73  y_struct, Compos
-00165500: 6974 6f72 4e6f 6465 2c20 4e6f 6465 2c20  itorNode, Node, 
-00165510: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+001654f0: 795f 7374 7275 6374 2c20 4e6f 6465 496e  y_struct, NodeIn
+00165500: 7465 726e 616c 2c20 436f 6d70 6f73 6974  ternal, Composit
+00165510: 6f72 4e6f 6465 2c20 4e6f 6465 293a 0a0a  orNode, Node):..
 00165520: 2020 6e6f 6465 5f6f 7574 7075 743a 2069    node_output: i
 00165530: 6e74 203d 202e 2e2e 0a0a 2020 2222 220a  nt = .....  """.
 00165540: 0a20 2046 6f72 206e 6f64 652d 6261 7365  .  For node-base
 00165550: 6420 7465 7874 7572 6573 2c20 7768 6963  d textures, whic
 00165560: 6820 6f75 7470 7574 206e 6f64 6520 746f  h output node to
 00165570: 2075 7365 0a0a 2020 2222 220a 0a20 2074   use..  """..  t
 00165580: 6578 7475 7265 3a20 5465 7874 7572 6520  exture: Texture 
@@ -91519,17 +91519,17 @@
 001657e0: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 001657f0: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 00165800: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 00165810: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 00165820: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 00165830: 7373 2043 6f6d 706f 7369 746f 724e 6f64  ss CompositorNod
 00165840: 6554 696d 6528 6270 795f 7374 7275 6374  eTime(bpy_struct
-00165850: 2c20 436f 6d70 6f73 6974 6f72 4e6f 6465  , CompositorNode
-00165860: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-00165870: 726e 616c 293a 0a0a 2020 6375 7276 653a  rnal):..  curve:
+00165850: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+00165860: 436f 6d70 6f73 6974 6f72 4e6f 6465 2c20  CompositorNode, 
+00165870: 4e6f 6465 293a 0a0a 2020 6375 7276 653a  Node):..  curve:
 00165880: 2043 7572 7665 4d61 7070 696e 6720 3d20   CurveMapping = 
 00165890: 2e2e 2e0a 0a20 2066 7261 6d65 5f65 6e64  .....  frame_end
 001658a0: 3a20 696e 7420 3d20 2e2e 2e0a 0a20 2066  : int = .....  f
 001658b0: 7261 6d65 5f73 7461 7274 3a20 696e 7420  rame_start: int 
 001658c0: 3d20 2e2e 2e0a 0a20 2040 636c 6173 736d  = .....  @classm
 001658d0: 6574 686f 640a 0a20 2064 6566 2069 735f  ethod..  def is_
 001658e0: 7265 6769 7374 6572 6564 5f6e 6f64 655f  registered_node_
@@ -91570,17 +91570,17 @@
 00165b10: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 00165b20: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 00165b30: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 00165b40: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 00165b50: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 00165b60: 7373 2043 6f6d 706f 7369 746f 724e 6f64  ss CompositorNod
 00165b70: 6554 6f6e 656d 6170 2862 7079 5f73 7472  eTonemap(bpy_str
-00165b80: 7563 742c 2043 6f6d 706f 7369 746f 724e  uct, CompositorN
-00165b90: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-00165ba0: 6e74 6572 6e61 6c29 3a0a 0a20 2061 6461  nternal):..  ada
+00165b80: 7563 742c 204e 6f64 6549 6e74 6572 6e61  uct, NodeInterna
+00165b90: 6c2c 2043 6f6d 706f 7369 746f 724e 6f64  l, CompositorNod
+00165ba0: 652c 204e 6f64 6529 3a0a 0a20 2061 6461  e, Node):..  ada
 00165bb0: 7074 6174 696f 6e3a 2066 6c6f 6174 203d  ptation: float =
 00165bc0: 202e 2e2e 0a0a 2020 2222 220a 0a20 2049   .....  """..  I
 00165bd0: 6620 302c 2067 6c6f 6261 6c3b 2069 6620  f 0, global; if 
 00165be0: 312c 2062 6173 6564 206f 6e20 7069 7865  1, based on pixe
 00165bf0: 6c20 696e 7465 6e73 6974 790a 0a20 2022  l intensity..  "
 00165c00: 2222 0a0a 2020 636f 6e74 7261 7374 3a20  ""..  contrast: 
 00165c10: 666c 6f61 7420 3d20 2e2e 2e0a 0a20 2022  float = .....  "
@@ -91658,17 +91658,17 @@
 00166090: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 001660a0: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 001660b0: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 001660c0: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 001660d0: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 001660e0: 6c61 7373 2043 6f6d 706f 7369 746f 724e  lass CompositorN
 001660f0: 6f64 6554 7261 636b 506f 7328 6270 795f  odeTrackPos(bpy_
-00166100: 7374 7275 6374 2c20 436f 6d70 6f73 6974  struct, Composit
-00166110: 6f72 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  orNode, Node, No
-00166120: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+00166100: 7374 7275 6374 2c20 4e6f 6465 496e 7465  struct, NodeInte
+00166110: 726e 616c 2c20 436f 6d70 6f73 6974 6f72  rnal, Compositor
+00166120: 4e6f 6465 2c20 4e6f 6465 293a 0a0a 2020  Node, Node):..  
 00166130: 636c 6970 3a20 4d6f 7669 6543 6c69 7020  clip: MovieClip 
 00166140: 3d20 2e2e 2e0a 0a20 2066 7261 6d65 5f72  = .....  frame_r
 00166150: 656c 6174 6976 653a 2069 6e74 203d 202e  elative: int = .
 00166160: 2e2e 0a0a 2020 2222 220a 0a20 2046 7261  ....  """..  Fra
 00166170: 6d65 2074 6f20 6265 2075 7365 6420 666f  me to be used fo
 00166180: 7220 7265 6c61 7469 7665 2070 6f73 6974  r relative posit
 00166190: 696f 6e0a 0a20 2022 2222 0a0a 2020 706f  ion..  """..  po
@@ -91744,17 +91744,17 @@
 001665f0: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 00166600: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 00166610: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 00166620: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 00166630: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 00166640: 6173 7320 436f 6d70 6f73 6974 6f72 4e6f  ass CompositorNo
 00166650: 6465 5472 616e 7366 6f72 6d28 6270 795f  deTransform(bpy_
-00166660: 7374 7275 6374 2c20 436f 6d70 6f73 6974  struct, Composit
-00166670: 6f72 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  orNode, Node, No
-00166680: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+00166660: 7374 7275 6374 2c20 4e6f 6465 496e 7465  struct, NodeInte
+00166670: 726e 616c 2c20 436f 6d70 6f73 6974 6f72  rnal, Compositor
+00166680: 4e6f 6465 2c20 4e6f 6465 293a 0a0a 2020  Node, Node):..  
 00166690: 6669 6c74 6572 5f74 7970 653a 2073 7472  filter_type: str
 001666a0: 203d 202e 2e2e 0a0a 2020 2222 220a 0a20   = .....  """.. 
 001666b0: 204d 6574 686f 6420 746f 2075 7365 2074   Method to use t
 001666c0: 6f20 6669 6c74 6572 2074 7261 6e73 666f  o filter transfo
 001666d0: 726d 0a0a 2020 2222 220a 0a20 2040 636c  rm..  """..  @cl
 001666e0: 6173 736d 6574 686f 640a 0a20 2064 6566  assmethod..  def
 001666f0: 2069 735f 7265 6769 7374 6572 6564 5f6e   is_registered_n
@@ -91795,17 +91795,17 @@
 00166920: 5f73 7562 636c 6173 735f 7079 2863 6c73  _subclass_py(cls
 00166930: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 00166940: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 00166950: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 00166960: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 00166970: 0a63 6c61 7373 2043 6f6d 706f 7369 746f  .class Composito
 00166980: 724e 6f64 6554 7261 6e73 6c61 7465 2862  rNodeTranslate(b
-00166990: 7079 5f73 7472 7563 742c 2043 6f6d 706f  py_struct, Compo
-001669a0: 7369 746f 724e 6f64 652c 204e 6f64 652c  sitorNode, Node,
-001669b0: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+00166990: 7079 5f73 7472 7563 742c 204e 6f64 6549  py_struct, NodeI
+001669a0: 6e74 6572 6e61 6c2c 2043 6f6d 706f 7369  nternal, Composi
+001669b0: 746f 724e 6f64 652c 204e 6f64 6529 3a0a  torNode, Node):.
 001669c0: 0a20 2075 7365 5f72 656c 6174 6976 653a  .  use_relative:
 001669d0: 2062 6f6f 6c20 3d20 2e2e 2e0a 0a20 2022   bool = .....  "
 001669e0: 2222 0a0a 2020 5573 6520 7265 6c61 7469  ""..  Use relati
 001669f0: 7665 2028 6672 6163 7469 6f6e 206f 6620  ve (fraction of 
 00166a00: 696e 7075 7420 696d 6167 6520 7369 7a65  input image size
 00166a10: 2920 7661 6c75 6573 2074 6f20 6465 6669  ) values to defi
 00166a20: 6e65 2074 7261 6e73 6c61 7469 6f6e 0a0a  ne translation..
@@ -91867,17 +91867,17 @@
 00166da0: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 00166db0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 00166dc0: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 00166dd0: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 00166de0: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 00166df0: 2043 6f6d 706f 7369 746f 724e 6f64 6556   CompositorNodeV
 00166e00: 616c 546f 5247 4228 6270 795f 7374 7275  alToRGB(bpy_stru
-00166e10: 6374 2c20 436f 6d70 6f73 6974 6f72 4e6f  ct, CompositorNo
-00166e20: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-00166e30: 7465 726e 616c 293a 0a0a 2020 636f 6c6f  ternal):..  colo
+00166e10: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+00166e20: 2c20 436f 6d70 6f73 6974 6f72 4e6f 6465  , CompositorNode
+00166e30: 2c20 4e6f 6465 293a 0a0a 2020 636f 6c6f  , Node):..  colo
 00166e40: 725f 7261 6d70 3a20 436f 6c6f 7252 616d  r_ramp: ColorRam
 00166e50: 7020 3d20 2e2e 2e0a 0a20 2040 636c 6173  p = .....  @clas
 00166e60: 736d 6574 686f 640a 0a20 2064 6566 2069  smethod..  def i
 00166e70: 735f 7265 6769 7374 6572 6564 5f6e 6f64  s_registered_nod
 00166e80: 655f 7479 7065 2863 6c73 2920 2d3e 2062  e_type(cls) -> b
 00166e90: 6f6f 6c3a 0a0a 2020 2020 2222 220a 0a20  ool:..    """.. 
 00166ea0: 2020 2054 7275 6520 6966 2061 2072 6567     True if a reg
@@ -91915,17 +91915,17 @@
 001670a0: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 001670b0: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 001670c0: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 001670d0: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 001670e0: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 001670f0: 6c61 7373 2043 6f6d 706f 7369 746f 724e  lass CompositorN
 00167100: 6f64 6556 616c 7565 2862 7079 5f73 7472  odeValue(bpy_str
-00167110: 7563 742c 2043 6f6d 706f 7369 746f 724e  uct, CompositorN
-00167120: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-00167130: 6e74 6572 6e61 6c29 3a0a 0a20 2040 636c  nternal):..  @cl
+00167110: 7563 742c 204e 6f64 6549 6e74 6572 6e61  uct, NodeInterna
+00167120: 6c2c 2043 6f6d 706f 7369 746f 724e 6f64  l, CompositorNod
+00167130: 652c 204e 6f64 6529 3a0a 0a20 2040 636c  e, Node):..  @cl
 00167140: 6173 736d 6574 686f 640a 0a20 2064 6566  assmethod..  def
 00167150: 2069 735f 7265 6769 7374 6572 6564 5f6e   is_registered_n
 00167160: 6f64 655f 7479 7065 2863 6c73 2920 2d3e  ode_type(cls) ->
 00167170: 2062 6f6f 6c3a 0a0a 2020 2020 2222 220a   bool:..    """.
 00167180: 0a20 2020 2054 7275 6520 6966 2061 2072  .    True if a r
 00167190: 6567 6973 7465 7265 6420 6e6f 6465 2074  egistered node t
 001671a0: 7970 650a 0a20 2020 2022 2222 0a0a 2020  ype..    """..  
@@ -91961,17 +91961,17 @@
 00167380: 5f73 7562 636c 6173 735f 7079 2863 6c73  _subclass_py(cls
 00167390: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 001673a0: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 001673b0: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 001673c0: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 001673d0: 0a63 6c61 7373 2043 6f6d 706f 7369 746f  .class Composito
 001673e0: 724e 6f64 6556 6563 426c 7572 2862 7079  rNodeVecBlur(bpy
-001673f0: 5f73 7472 7563 742c 2043 6f6d 706f 7369  _struct, Composi
-00167400: 746f 724e 6f64 652c 204e 6f64 652c 204e  torNode, Node, N
-00167410: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+001673f0: 5f73 7472 7563 742c 204e 6f64 6549 6e74  _struct, NodeInt
+00167400: 6572 6e61 6c2c 2043 6f6d 706f 7369 746f  ernal, Composito
+00167410: 724e 6f64 652c 204e 6f64 6529 3a0a 0a20  rNode, Node):.. 
 00167420: 2066 6163 746f 723a 2066 6c6f 6174 203d   factor: float =
 00167430: 202e 2e2e 0a0a 2020 2222 220a 0a20 2053   .....  """..  S
 00167440: 6361 6c69 6e67 2066 6163 746f 7220 666f  caling factor fo
 00167450: 7220 6d6f 7469 6f6e 2076 6563 746f 7273  r motion vectors
 00167460: 2028 6163 7475 616c 6c79 2c20 2773 6875   (actually, 'shu
 00167470: 7474 6572 2073 7065 6564 272c 2069 6e20  tter speed', in 
 00167480: 6672 616d 6573 290a 0a20 2022 2222 0a0a  frames)..  """..
@@ -92035,17 +92035,17 @@
 00167820: 745f 7375 6263 6c61 7373 5f70 7928 636c  t_subclass_py(cl
 00167830: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 00167840: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 00167850: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 00167860: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 00167870: 0a0a 636c 6173 7320 436f 6d70 6f73 6974  ..class Composit
 00167880: 6f72 4e6f 6465 5669 6577 6572 2862 7079  orNodeViewer(bpy
-00167890: 5f73 7472 7563 742c 2043 6f6d 706f 7369  _struct, Composi
-001678a0: 746f 724e 6f64 652c 204e 6f64 652c 204e  torNode, Node, N
-001678b0: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+00167890: 5f73 7472 7563 742c 204e 6f64 6549 6e74  _struct, NodeInt
+001678a0: 6572 6e61 6c2c 2043 6f6d 706f 7369 746f  ernal, Composito
+001678b0: 724e 6f64 652c 204e 6f64 6529 3a0a 0a20  rNode, Node):.. 
 001678c0: 2063 656e 7465 725f 783a 2066 6c6f 6174   center_x: float
 001678d0: 203d 202e 2e2e 0a0a 2020 6365 6e74 6572   = .....  center
 001678e0: 5f79 3a20 666c 6f61 7420 3d20 2e2e 2e0a  _y: float = ....
 001678f0: 0a20 2074 696c 655f 6f72 6465 723a 2073  .  tile_order: s
 00167900: 7472 203d 202e 2e2e 0a0a 2020 2222 220a  tr = .....  """.
 00167910: 0a20 2054 696c 6520 6f72 6465 720a 0a20  .  Tile order.. 
 00167920: 202a 2060 6043 454e 5445 524f 5554 6060   * ``CENTEROUT``
@@ -92109,17 +92109,17 @@
 00167cc0: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 00167cd0: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 00167ce0: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 00167cf0: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 00167d00: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 00167d10: 436f 6d70 6f73 6974 6f72 4e6f 6465 5a63  CompositorNodeZc
 00167d20: 6f6d 6269 6e65 2862 7079 5f73 7472 7563  ombine(bpy_struc
-00167d30: 742c 2043 6f6d 706f 7369 746f 724e 6f64  t, CompositorNod
-00167d40: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-00167d50: 6572 6e61 6c29 3a0a 0a20 2075 7365 5f61  ernal):..  use_a
+00167d30: 742c 204e 6f64 6549 6e74 6572 6e61 6c2c  t, NodeInternal,
+00167d40: 2043 6f6d 706f 7369 746f 724e 6f64 652c   CompositorNode,
+00167d50: 204e 6f64 6529 3a0a 0a20 2075 7365 5f61   Node):..  use_a
 00167d60: 6c70 6861 3a20 626f 6f6c 203d 202e 2e2e  lpha: bool = ...
 00167d70: 0a0a 2020 2222 220a 0a20 2054 616b 6520  ..  """..  Take 
 00167d80: 616c 7068 6120 6368 616e 6e65 6c20 696e  alpha channel in
 00167d90: 746f 2061 6363 6f75 6e74 2077 6865 6e20  to account when 
 00167da0: 646f 696e 6720 7468 6520 5a20 6f70 6572  doing the Z oper
 00167db0: 6174 696f 6e0a 0a20 2022 2222 0a0a 2020  ation..  """..  
 00167dc0: 7573 655f 616e 7469 616c 6961 735f 7a3a  use_antialias_z:
@@ -92170,17 +92170,17 @@
 00168090: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 001680a0: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 001680b0: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 001680c0: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 001680d0: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2046      .....class F
 001680e0: 756e 6374 696f 6e4e 6f64 6541 6c69 676e  unctionNodeAlign
 001680f0: 4575 6c65 7254 6f56 6563 746f 7228 6270  EulerToVector(bp
-00168100: 795f 7374 7275 6374 2c20 4e6f 6465 2c20  y_struct, Node, 
-00168110: 4675 6e63 7469 6f6e 4e6f 6465 2c20 4e6f  FunctionNode, No
-00168120: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+00168100: 795f 7374 7275 6374 2c20 4675 6e63 7469  y_struct, Functi
+00168110: 6f6e 4e6f 6465 2c20 4e6f 6465 496e 7465  onNode, NodeInte
+00168120: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 00168130: 6178 6973 3a20 7374 7220 3d20 2e2e 2e0a  axis: str = ....
 00168140: 0a20 2022 2222 0a0a 2020 4178 6973 2074  .  """..  Axis t
 00168150: 6f20 616c 6967 6e20 746f 2074 6865 2076  o align to the v
 00168160: 6563 746f 720a 0a20 202a 2060 6058 6060  ector..  * ``X``
 00168170: 0a58 202d 2d20 416c 6967 6e20 7468 6520  .X -- Align the 
 00168180: 5820 6178 6973 2077 6974 6820 7468 6520  X axis with the 
 00168190: 7665 6374 6f72 2e0a 0a20 202a 2060 6059  vector...  * ``Y
@@ -92246,17 +92246,17 @@
 00168550: 6765 745f 7375 6263 6c61 7373 5f70 7928  get_subclass_py(
 00168560: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 00168570: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 00168580: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 00168590: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 001685a0: 2e2e 0a0a 636c 6173 7320 4675 6e63 7469  ....class Functi
 001685b0: 6f6e 4e6f 6465 426f 6f6c 6561 6e4d 6174  onNodeBooleanMat
-001685c0: 6828 6270 795f 7374 7275 6374 2c20 4e6f  h(bpy_struct, No
-001685d0: 6465 2c20 4675 6e63 7469 6f6e 4e6f 6465  de, FunctionNode
-001685e0: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+001685c0: 6828 6270 795f 7374 7275 6374 2c20 4675  h(bpy_struct, Fu
+001685d0: 6e63 7469 6f6e 4e6f 6465 2c20 4e6f 6465  nctionNode, Node
+001685e0: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 001685f0: 0a0a 2020 6f70 6572 6174 696f 6e3a 2073  ..  operation: s
 00168600: 7472 203d 202e 2e2e 0a0a 2020 4063 6c61  tr = .....  @cla
 00168610: 7373 6d65 7468 6f64 0a0a 2020 6465 6620  ssmethod..  def 
 00168620: 6973 5f72 6567 6973 7465 7265 645f 6e6f  is_registered_no
 00168630: 6465 5f74 7970 6528 636c 7329 202d 3e20  de_type(cls) -> 
 00168640: 626f 6f6c 3a0a 0a20 2020 2022 2222 0a0a  bool:..    """..
 00168650: 2020 2020 5472 7565 2069 6620 6120 7265      True if a re
@@ -92292,17 +92292,17 @@
 00168830: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 00168840: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 00168850: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 00168860: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 00168870: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 00168880: 4675 6e63 7469 6f6e 4e6f 6465 436f 6d62  FunctionNodeComb
 00168890: 696e 6543 6f6c 6f72 2862 7079 5f73 7472  ineColor(bpy_str
-001688a0: 7563 742c 204e 6f64 652c 2046 756e 6374  uct, Node, Funct
-001688b0: 696f 6e4e 6f64 652c 204e 6f64 6549 6e74  ionNode, NodeInt
-001688c0: 6572 6e61 6c29 3a0a 0a20 206d 6f64 653a  ernal):..  mode:
+001688a0: 7563 742c 2046 756e 6374 696f 6e4e 6f64  uct, FunctionNod
+001688b0: 652c 204e 6f64 6549 6e74 6572 6e61 6c2c  e, NodeInternal,
+001688c0: 204e 6f64 6529 3a0a 0a20 206d 6f64 653a   Node):..  mode:
 001688d0: 2073 7472 203d 202e 2e2e 0a0a 2020 2222   str = .....  ""
 001688e0: 220a 0a20 204d 6f64 6520 6f66 2063 6f6c  "..  Mode of col
 001688f0: 6f72 2070 726f 6365 7373 696e 670a 0a20  or processing.. 
 00168900: 202a 2060 6052 4742 6060 0a52 4742 202d   * ``RGB``.RGB -
 00168910: 2d20 5573 6520 5247 4220 636f 6c6f 7220  - Use RGB color 
 00168920: 7072 6f63 6573 7369 6e67 2e0a 0a20 202a  processing...  *
 00168930: 2060 6048 5356 6060 0a48 5356 202d 2d20   ``HSV``.HSV -- 
@@ -92348,17 +92348,17 @@
 00168bb0: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 00168bc0: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 00168bd0: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 00168be0: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 00168bf0: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 00168c00: 636c 6173 7320 4675 6e63 7469 6f6e 4e6f  class FunctionNo
 00168c10: 6465 436f 6d70 6172 6528 6270 795f 7374  deCompare(bpy_st
-00168c20: 7275 6374 2c20 4e6f 6465 2c20 4675 6e63  ruct, Node, Func
-00168c30: 7469 6f6e 4e6f 6465 2c20 4e6f 6465 496e  tionNode, NodeIn
-00168c40: 7465 726e 616c 293a 0a0a 2020 6461 7461  ternal):..  data
+00168c20: 7275 6374 2c20 4675 6e63 7469 6f6e 4e6f  ruct, FunctionNo
+00168c30: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+00168c40: 2c20 4e6f 6465 293a 0a0a 2020 6461 7461  , Node):..  data
 00168c50: 5f74 7970 653a 2073 7472 203d 202e 2e2e  _type: str = ...
 00168c60: 0a0a 2020 6d6f 6465 3a20 7374 7220 3d20  ..  mode: str = 
 00168c70: 2e2e 2e0a 0a20 2022 2222 0a0a 2020 2a20  .....  """..  * 
 00168c80: 6060 454c 454d 454e 5460 600a 456c 656d  ``ELEMENT``.Elem
 00168c90: 656e 742d 5769 7365 202d 2d20 436f 6d70  ent-Wise -- Comp
 00168ca0: 6172 6520 6561 6368 2065 6c65 6d65 6e74  are each element
 00168cb0: 206f 6620 7468 6520 696e 7075 7420 7665   of the input ve
@@ -92421,17 +92421,17 @@
 00169040: 5f70 7928 636c 732c 2069 643a 2073 7472  _py(cls, id: str
 00169050: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 00169060: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 00169070: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 00169080: 2020 202e 2e2e 0a0a 636c 6173 7320 4675     .....class Fu
 00169090: 6e63 7469 6f6e 4e6f 6465 466c 6f61 7454  nctionNodeFloatT
 001690a0: 6f49 6e74 2862 7079 5f73 7472 7563 742c  oInt(bpy_struct,
-001690b0: 204e 6f64 652c 2046 756e 6374 696f 6e4e   Node, FunctionN
-001690c0: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-001690d0: 6c29 3a0a 0a20 2072 6f75 6e64 696e 675f  l):..  rounding_
+001690b0: 2046 756e 6374 696f 6e4e 6f64 652c 204e   FunctionNode, N
+001690c0: 6f64 6549 6e74 6572 6e61 6c2c 204e 6f64  odeInternal, Nod
+001690d0: 6529 3a0a 0a20 2072 6f75 6e64 696e 675f  e):..  rounding_
 001690e0: 6d6f 6465 3a20 7374 7220 3d20 2e2e 2e0a  mode: str = ....
 001690f0: 0a20 2022 2222 0a0a 2020 4d65 7468 6f64  .  """..  Method
 00169100: 2075 7365 6420 746f 2063 6f6e 7665 7274   used to convert
 00169110: 2074 6865 2066 6c6f 6174 2074 6f20 616e   the float to an
 00169120: 2069 6e74 6567 6572 0a0a 2020 2222 220a   integer..  """.
 00169130: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
 00169140: 0a20 2064 6566 2069 735f 7265 6769 7374  .  def is_regist
@@ -92470,17 +92470,17 @@
 00169350: 5f73 7562 636c 6173 735f 7079 2863 6c73  _subclass_py(cls
 00169360: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 00169370: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 00169380: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 00169390: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 001693a0: 0a63 6c61 7373 2046 756e 6374 696f 6e4e  .class FunctionN
 001693b0: 6f64 6549 6e70 7574 426f 6f6c 2862 7079  odeInputBool(bpy
-001693c0: 5f73 7472 7563 742c 204e 6f64 652c 2046  _struct, Node, F
-001693d0: 756e 6374 696f 6e4e 6f64 652c 204e 6f64  unctionNode, Nod
-001693e0: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2062  eInternal):..  b
+001693c0: 5f73 7472 7563 742c 2046 756e 6374 696f  _struct, Functio
+001693d0: 6e4e 6f64 652c 204e 6f64 6549 6e74 6572  nNode, NodeInter
+001693e0: 6e61 6c2c 204e 6f64 6529 3a0a 0a20 2062  nal, Node):..  b
 001693f0: 6f6f 6c65 616e 3a20 626f 6f6c 203d 202e  oolean: bool = .
 00169400: 2e2e 0a0a 2020 2222 220a 0a20 2049 6e70  ....  """..  Inp
 00169410: 7574 2076 616c 7565 2075 7365 6420 666f  ut value used fo
 00169420: 7220 756e 636f 6e6e 6563 7465 6420 736f  r unconnected so
 00169430: 636b 6574 0a0a 2020 2222 220a 0a20 2040  cket..  """..  @
 00169440: 636c 6173 736d 6574 686f 640a 0a20 2064  classmethod..  d
 00169450: 6566 2069 735f 7265 6769 7374 6572 6564  ef is_registered
@@ -92519,17 +92519,17 @@
 00169660: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 00169670: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 00169680: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 00169690: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 001696a0: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 001696b0: 7373 2046 756e 6374 696f 6e4e 6f64 6549  ss FunctionNodeI
 001696c0: 6e70 7574 436f 6c6f 7228 6270 795f 7374  nputColor(bpy_st
-001696d0: 7275 6374 2c20 4e6f 6465 2c20 4675 6e63  ruct, Node, Func
-001696e0: 7469 6f6e 4e6f 6465 2c20 4e6f 6465 496e  tionNode, NodeIn
-001696f0: 7465 726e 616c 293a 0a0a 2020 636f 6c6f  ternal):..  colo
+001696d0: 7275 6374 2c20 4675 6e63 7469 6f6e 4e6f  ruct, FunctionNo
+001696e0: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+001696f0: 2c20 4e6f 6465 293a 0a0a 2020 636f 6c6f  , Node):..  colo
 00169700: 723a 2074 7970 696e 672e 5475 706c 655b  r: typing.Tuple[
 00169710: 666c 6f61 742c 2066 6c6f 6174 2c20 666c  float, float, fl
 00169720: 6f61 742c 2066 6c6f 6174 5d20 3d20 2e2e  oat, float] = ..
 00169730: 2e0a 0a20 2040 636c 6173 736d 6574 686f  ...  @classmetho
 00169740: 640a 0a20 2064 6566 2069 735f 7265 6769  d..  def is_regi
 00169750: 7374 6572 6564 5f6e 6f64 655f 7479 7065  stered_node_type
 00169760: 2863 6c73 2920 2d3e 2062 6f6f 6c3a 0a0a  (cls) -> bool:..
@@ -92566,17 +92566,17 @@
 00169950: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 00169960: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 00169970: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 00169980: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 00169990: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 001699a0: 2e0a 0a63 6c61 7373 2046 756e 6374 696f  ...class Functio
 001699b0: 6e4e 6f64 6549 6e70 7574 496e 7428 6270  nNodeInputInt(bp
-001699c0: 795f 7374 7275 6374 2c20 4e6f 6465 2c20  y_struct, Node, 
-001699d0: 4675 6e63 7469 6f6e 4e6f 6465 2c20 4e6f  FunctionNode, No
-001699e0: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+001699c0: 795f 7374 7275 6374 2c20 4675 6e63 7469  y_struct, Functi
+001699d0: 6f6e 4e6f 6465 2c20 4e6f 6465 496e 7465  onNode, NodeInte
+001699e0: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 001699f0: 696e 7465 6765 723a 2069 6e74 203d 202e  integer: int = .
 00169a00: 2e2e 0a0a 2020 2222 220a 0a20 2049 6e70  ....  """..  Inp
 00169a10: 7574 2076 616c 7565 2075 7365 6420 666f  ut value used fo
 00169a20: 7220 756e 636f 6e6e 6563 7465 6420 736f  r unconnected so
 00169a30: 636b 6574 0a0a 2020 2222 220a 0a20 2040  cket..  """..  @
 00169a40: 636c 6173 736d 6574 686f 640a 0a20 2064  classmethod..  d
 00169a50: 6566 2069 735f 7265 6769 7374 6572 6564  ef is_registered
@@ -92616,17 +92616,17 @@
 00169c70: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 00169c80: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 00169c90: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 00169ca0: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 00169cb0: 7373 2046 756e 6374 696f 6e4e 6f64 6549  ss FunctionNodeI
 00169cc0: 6e70 7574 5370 6563 6961 6c43 6861 7261  nputSpecialChara
 00169cd0: 6374 6572 7328 6270 795f 7374 7275 6374  cters(bpy_struct
-00169ce0: 2c20 4e6f 6465 2c20 4675 6e63 7469 6f6e  , Node, Function
-00169cf0: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-00169d00: 616c 293a 0a0a 2020 4063 6c61 7373 6d65  al):..  @classme
+00169ce0: 2c20 4675 6e63 7469 6f6e 4e6f 6465 2c20  , FunctionNode, 
+00169cf0: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+00169d00: 6465 293a 0a0a 2020 4063 6c61 7373 6d65  de):..  @classme
 00169d10: 7468 6f64 0a0a 2020 6465 6620 6973 5f72  thod..  def is_r
 00169d20: 6567 6973 7465 7265 645f 6e6f 6465 5f74  egistered_node_t
 00169d30: 7970 6528 636c 7329 202d 3e20 626f 6f6c  ype(cls) -> bool
 00169d40: 3a0a 0a20 2020 2022 2222 0a0a 2020 2020  :..    """..    
 00169d50: 5472 7565 2069 6620 6120 7265 6769 7374  True if a regist
 00169d60: 6572 6564 206e 6f64 6520 7479 7065 0a0a  ered node type..
 00169d70: 2020 2020 2222 220a 0a20 2020 202e 2e2e      """..    ...
@@ -92660,16 +92660,16 @@
 00169f30: 7928 636c 732c 2069 643a 2073 7472 2c20  y(cls, id: str, 
 00169f40: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 00169f50: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 00169f60: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 00169f70: 202e 2e2e 0a0a 636c 6173 7320 4675 6e63   .....class Func
 00169f80: 7469 6f6e 4e6f 6465 496e 7075 7453 7472  tionNodeInputStr
 00169f90: 696e 6728 6270 795f 7374 7275 6374 2c20  ing(bpy_struct, 
-00169fa0: 4e6f 6465 2c20 4675 6e63 7469 6f6e 4e6f  Node, FunctionNo
-00169fb0: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+00169fa0: 4675 6e63 7469 6f6e 4e6f 6465 2c20 4e6f  FunctionNode, No
+00169fb0: 6465 496e 7465 726e 616c 2c20 4e6f 6465  deInternal, Node
 00169fc0: 293a 0a0a 2020 7374 7269 6e67 3a20 7374  ):..  string: st
 00169fd0: 7220 3d20 2e2e 2e0a 0a20 2040 636c 6173  r = .....  @clas
 00169fe0: 736d 6574 686f 640a 0a20 2064 6566 2069  smethod..  def i
 00169ff0: 735f 7265 6769 7374 6572 6564 5f6e 6f64  s_registered_nod
 0016a000: 655f 7479 7065 2863 6c73 2920 2d3e 2062  e_type(cls) -> b
 0016a010: 6f6f 6c3a 0a0a 2020 2020 2222 220a 0a20  ool:..    """.. 
 0016a020: 2020 2054 7275 6520 6966 2061 2072 6567     True if a reg
@@ -92705,17 +92705,17 @@
 0016a200: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 0016a210: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 0016a220: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 0016a230: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 0016a240: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2046      .....class F
 0016a250: 756e 6374 696f 6e4e 6f64 6549 6e70 7574  unctionNodeInput
 0016a260: 5665 6374 6f72 2862 7079 5f73 7472 7563  Vector(bpy_struc
-0016a270: 742c 204e 6f64 652c 2046 756e 6374 696f  t, Node, Functio
-0016a280: 6e4e 6f64 652c 204e 6f64 6549 6e74 6572  nNode, NodeInter
-0016a290: 6e61 6c29 3a0a 0a20 2076 6563 746f 723a  nal):..  vector:
+0016a270: 742c 2046 756e 6374 696f 6e4e 6f64 652c  t, FunctionNode,
+0016a280: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+0016a290: 6f64 6529 3a0a 0a20 2076 6563 746f 723a  ode):..  vector:
 0016a2a0: 206d 6174 6875 7469 6c73 2e56 6563 746f   mathutils.Vecto
 0016a2b0: 7220 3d20 2e2e 2e0a 0a20 2040 636c 6173  r = .....  @clas
 0016a2c0: 736d 6574 686f 640a 0a20 2064 6566 2069  smethod..  def i
 0016a2d0: 735f 7265 6769 7374 6572 6564 5f6e 6f64  s_registered_nod
 0016a2e0: 655f 7479 7065 2863 6c73 2920 2d3e 2062  e_type(cls) -> b
 0016a2f0: 6f6f 6c3a 0a0a 2020 2020 2222 220a 0a20  ool:..    """.. 
 0016a300: 2020 2054 7275 6520 6966 2061 2072 6567     True if a reg
@@ -92751,17 +92751,17 @@
 0016a4e0: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 0016a4f0: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 0016a500: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 0016a510: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 0016a520: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2046      .....class F
 0016a530: 756e 6374 696f 6e4e 6f64 6552 616e 646f  unctionNodeRando
 0016a540: 6d56 616c 7565 2862 7079 5f73 7472 7563  mValue(bpy_struc
-0016a550: 742c 204e 6f64 652c 2046 756e 6374 696f  t, Node, Functio
-0016a560: 6e4e 6f64 652c 204e 6f64 6549 6e74 6572  nNode, NodeInter
-0016a570: 6e61 6c29 3a0a 0a20 2064 6174 615f 7479  nal):..  data_ty
+0016a550: 742c 2046 756e 6374 696f 6e4e 6f64 652c  t, FunctionNode,
+0016a560: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+0016a570: 6f64 6529 3a0a 0a20 2064 6174 615f 7479  ode):..  data_ty
 0016a580: 7065 3a20 7374 7220 3d20 2e2e 2e0a 0a20  pe: str = ..... 
 0016a590: 2022 2222 0a0a 2020 5479 7065 206f 6620   """..  Type of 
 0016a5a0: 6461 7461 2073 746f 7265 6420 696e 2061  data stored in a
 0016a5b0: 7474 7269 6275 7465 0a0a 2020 2222 220a  ttribute..  """.
 0016a5c0: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
 0016a5d0: 0a20 2064 6566 2069 735f 7265 6769 7374  .  def is_regist
 0016a5e0: 6572 6564 5f6e 6f64 655f 7479 7065 2863  ered_node_type(c
@@ -92799,17 +92799,17 @@
 0016a7e0: 5f73 7562 636c 6173 735f 7079 2863 6c73  _subclass_py(cls
 0016a7f0: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 0016a800: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 0016a810: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 0016a820: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 0016a830: 0a63 6c61 7373 2046 756e 6374 696f 6e4e  .class FunctionN
 0016a840: 6f64 6552 6570 6c61 6365 5374 7269 6e67  odeReplaceString
-0016a850: 2862 7079 5f73 7472 7563 742c 204e 6f64  (bpy_struct, Nod
-0016a860: 652c 2046 756e 6374 696f 6e4e 6f64 652c  e, FunctionNode,
-0016a870: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+0016a850: 2862 7079 5f73 7472 7563 742c 2046 756e  (bpy_struct, Fun
+0016a860: 6374 696f 6e4e 6f64 652c 204e 6f64 6549  ctionNode, NodeI
+0016a870: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 0016a880: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
 0016a890: 0a20 2064 6566 2069 735f 7265 6769 7374  .  def is_regist
 0016a8a0: 6572 6564 5f6e 6f64 655f 7479 7065 2863  ered_node_type(c
 0016a8b0: 6c73 2920 2d3e 2062 6f6f 6c3a 0a0a 2020  ls) -> bool:..  
 0016a8c0: 2020 2222 220a 0a20 2020 2054 7275 6520    """..    True 
 0016a8d0: 6966 2061 2072 6567 6973 7465 7265 6420  if a registered 
 0016a8e0: 6e6f 6465 2074 7970 650a 0a20 2020 2022  node type..    "
@@ -92843,17 +92843,17 @@
 0016aaa0: 5f73 7562 636c 6173 735f 7079 2863 6c73  _subclass_py(cls
 0016aab0: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 0016aac0: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 0016aad0: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 0016aae0: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 0016aaf0: 0a63 6c61 7373 2046 756e 6374 696f 6e4e  .class FunctionN
 0016ab00: 6f64 6552 6f74 6174 6545 756c 6572 2862  odeRotateEuler(b
-0016ab10: 7079 5f73 7472 7563 742c 204e 6f64 652c  py_struct, Node,
-0016ab20: 2046 756e 6374 696f 6e4e 6f64 652c 204e   FunctionNode, N
-0016ab30: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+0016ab10: 7079 5f73 7472 7563 742c 2046 756e 6374  py_struct, Funct
+0016ab20: 696f 6e4e 6f64 652c 204e 6f64 6549 6e74  ionNode, NodeInt
+0016ab30: 6572 6e61 6c2c 204e 6f64 6529 3a0a 0a20  ernal, Node):.. 
 0016ab40: 2073 7061 6365 3a20 7374 7220 3d20 2e2e   space: str = ..
 0016ab50: 2e0a 0a20 2022 2222 0a0a 2020 4261 7365  ...  """..  Base
 0016ab60: 206f 7269 656e 7461 7469 6f6e 2066 6f72   orientation for
 0016ab70: 2072 6f74 6174 696f 6e0a 0a20 202a 2060   rotation..  * `
 0016ab80: 604f 424a 4543 5460 600a 4f62 6a65 6374  `OBJECT``.Object
 0016ab90: 202d 2d20 526f 7461 7465 2074 6865 2069   -- Rotate the i
 0016aba0: 6e70 7574 2072 6f74 6174 696f 6e20 696e  nput rotation in
@@ -92914,17 +92914,17 @@
 0016af10: 5f70 7928 636c 732c 2069 643a 2073 7472  _py(cls, id: str
 0016af20: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 0016af30: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 0016af40: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 0016af50: 2020 202e 2e2e 0a0a 636c 6173 7320 4675     .....class Fu
 0016af60: 6e63 7469 6f6e 4e6f 6465 5365 7061 7261  nctionNodeSepara
 0016af70: 7465 436f 6c6f 7228 6270 795f 7374 7275  teColor(bpy_stru
-0016af80: 6374 2c20 4e6f 6465 2c20 4675 6e63 7469  ct, Node, Functi
-0016af90: 6f6e 4e6f 6465 2c20 4e6f 6465 496e 7465  onNode, NodeInte
-0016afa0: 726e 616c 293a 0a0a 2020 6d6f 6465 3a20  rnal):..  mode: 
+0016af80: 6374 2c20 4675 6e63 7469 6f6e 4e6f 6465  ct, FunctionNode
+0016af90: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+0016afa0: 4e6f 6465 293a 0a0a 2020 6d6f 6465 3a20  Node):..  mode: 
 0016afb0: 7374 7220 3d20 2e2e 2e0a 0a20 2022 2222  str = .....  """
 0016afc0: 0a0a 2020 4d6f 6465 206f 6620 636f 6c6f  ..  Mode of colo
 0016afd0: 7220 7072 6f63 6573 7369 6e67 0a0a 2020  r processing..  
 0016afe0: 2a20 6060 5247 4260 600a 5247 4220 2d2d  * ``RGB``.RGB --
 0016aff0: 2055 7365 2052 4742 2063 6f6c 6f72 2070   Use RGB color p
 0016b000: 726f 6365 7373 696e 672e 0a0a 2020 2a20  rocessing...  * 
 0016b010: 6060 4853 5660 600a 4853 5620 2d2d 2055  ``HSV``.HSV -- U
@@ -92970,17 +92970,17 @@
 0016b290: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 0016b2a0: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 0016b2b0: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 0016b2c0: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 0016b2d0: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 0016b2e0: 6c61 7373 2046 756e 6374 696f 6e4e 6f64  lass FunctionNod
 0016b2f0: 6553 6c69 6365 5374 7269 6e67 2862 7079  eSliceString(bpy
-0016b300: 5f73 7472 7563 742c 204e 6f64 652c 2046  _struct, Node, F
-0016b310: 756e 6374 696f 6e4e 6f64 652c 204e 6f64  unctionNode, Nod
-0016b320: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2040  eInternal):..  @
+0016b300: 5f73 7472 7563 742c 2046 756e 6374 696f  _struct, Functio
+0016b310: 6e4e 6f64 652c 204e 6f64 6549 6e74 6572  nNode, NodeInter
+0016b320: 6e61 6c2c 204e 6f64 6529 3a0a 0a20 2040  nal, Node):..  @
 0016b330: 636c 6173 736d 6574 686f 640a 0a20 2064  classmethod..  d
 0016b340: 6566 2069 735f 7265 6769 7374 6572 6564  ef is_registered
 0016b350: 5f6e 6f64 655f 7479 7065 2863 6c73 2920  _node_type(cls) 
 0016b360: 2d3e 2062 6f6f 6c3a 0a0a 2020 2020 2222  -> bool:..    ""
 0016b370: 220a 0a20 2020 2054 7275 6520 6966 2061  "..    True if a
 0016b380: 2072 6567 6973 7465 7265 6420 6e6f 6465   registered node
 0016b390: 2074 7970 650a 0a20 2020 2022 2222 0a0a   type..    """..
@@ -93014,17 +93014,17 @@
 0016b550: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 0016b560: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 0016b570: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 0016b580: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 0016b590: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 0016b5a0: 7373 2046 756e 6374 696f 6e4e 6f64 6553  ss FunctionNodeS
 0016b5b0: 7472 696e 674c 656e 6774 6828 6270 795f  tringLength(bpy_
-0016b5c0: 7374 7275 6374 2c20 4e6f 6465 2c20 4675  struct, Node, Fu
-0016b5d0: 6e63 7469 6f6e 4e6f 6465 2c20 4e6f 6465  nctionNode, Node
-0016b5e0: 496e 7465 726e 616c 293a 0a0a 2020 4063  Internal):..  @c
+0016b5c0: 7374 7275 6374 2c20 4675 6e63 7469 6f6e  struct, Function
+0016b5d0: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
+0016b5e0: 616c 2c20 4e6f 6465 293a 0a0a 2020 4063  al, Node):..  @c
 0016b5f0: 6c61 7373 6d65 7468 6f64 0a0a 2020 6465  lassmethod..  de
 0016b600: 6620 6973 5f72 6567 6973 7465 7265 645f  f is_registered_
 0016b610: 6e6f 6465 5f74 7970 6528 636c 7329 202d  node_type(cls) -
 0016b620: 3e20 626f 6f6c 3a0a 0a20 2020 2022 2222  > bool:..    """
 0016b630: 0a0a 2020 2020 5472 7565 2069 6620 6120  ..    True if a 
 0016b640: 7265 6769 7374 6572 6564 206e 6f64 6520  registered node 
 0016b650: 7479 7065 0a0a 2020 2020 2222 220a 0a20  type..    """.. 
@@ -93058,17 +93058,17 @@
 0016b810: 6c61 7373 5f70 7928 636c 732c 2069 643a  lass_py(cls, id:
 0016b820: 2073 7472 2c20 6465 6661 756c 743a 2074   str, default: t
 0016b830: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 0016b840: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 0016b850: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 0016b860: 7320 4675 6e63 7469 6f6e 4e6f 6465 5661  s FunctionNodeVa
 0016b870: 6c75 6554 6f53 7472 696e 6728 6270 795f  lueToString(bpy_
-0016b880: 7374 7275 6374 2c20 4e6f 6465 2c20 4675  struct, Node, Fu
-0016b890: 6e63 7469 6f6e 4e6f 6465 2c20 4e6f 6465  nctionNode, Node
-0016b8a0: 496e 7465 726e 616c 293a 0a0a 2020 4063  Internal):..  @c
+0016b880: 7374 7275 6374 2c20 4675 6e63 7469 6f6e  struct, Function
+0016b890: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
+0016b8a0: 616c 2c20 4e6f 6465 293a 0a0a 2020 4063  al, Node):..  @c
 0016b8b0: 6c61 7373 6d65 7468 6f64 0a0a 2020 6465  lassmethod..  de
 0016b8c0: 6620 6973 5f72 6567 6973 7465 7265 645f  f is_registered_
 0016b8d0: 6e6f 6465 5f74 7970 6528 636c 7329 202d  node_type(cls) -
 0016b8e0: 3e20 626f 6f6c 3a0a 0a20 2020 2022 2222  > bool:..    """
 0016b8f0: 0a0a 2020 2020 5472 7565 2069 6620 6120  ..    True if a 
 0016b900: 7265 6769 7374 6572 6564 206e 6f64 6520  registered node 
 0016b910: 7479 7065 0a0a 2020 2020 2222 220a 0a20  type..    """.. 
@@ -93103,16 +93103,16 @@
 0016bae0: 2073 7472 2c20 6465 6661 756c 743a 2074   str, default: t
 0016baf0: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 0016bb00: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 0016bb10: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 0016bb20: 7320 4765 6f6d 6574 7279 4e6f 6465 4163  s GeometryNodeAc
 0016bb30: 6375 6d75 6c61 7465 4669 656c 6428 6270  cumulateField(bp
 0016bb40: 795f 7374 7275 6374 2c20 4765 6f6d 6574  y_struct, Geomet
-0016bb50: 7279 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  ryNode, Node, No
-0016bb60: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+0016bb50: 7279 4e6f 6465 2c20 4e6f 6465 496e 7465  ryNode, NodeInte
+0016bb60: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 0016bb70: 2222 220a 0a20 2041 6464 2074 6865 2076  """..  Add the v
 0016bb80: 616c 7565 7320 6f66 2061 6e20 6576 616c  alues of an eval
 0016bb90: 7561 7465 6420 6669 656c 6420 746f 6765  uated field toge
 0016bba0: 7468 6572 2061 6e64 206f 7574 7075 7420  ther and output 
 0016bbb0: 7468 6520 7275 6e6e 696e 6720 746f 7461  the running tota
 0016bbc0: 6c20 666f 7220 6561 6368 2065 6c65 6d65  l for each eleme
 0016bbd0: 6e74 0a0a 2020 2222 220a 0a20 2064 6174  nt..  """..  dat
@@ -93160,16 +93160,16 @@
 0016be70: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 0016be80: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 0016be90: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 0016bea0: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 0016beb0: 4765 6f6d 6574 7279 4e6f 6465 4174 7472  GeometryNodeAttr
 0016bec0: 6962 7574 6544 6f6d 6169 6e53 697a 6528  ibuteDomainSize(
 0016bed0: 6270 795f 7374 7275 6374 2c20 4765 6f6d  bpy_struct, Geom
-0016bee0: 6574 7279 4e6f 6465 2c20 4e6f 6465 2c20  etryNode, Node, 
-0016bef0: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+0016bee0: 6574 7279 4e6f 6465 2c20 4e6f 6465 496e  etryNode, NodeIn
+0016bef0: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 0016bf00: 2020 2222 220a 0a20 2052 6574 7269 6576    """..  Retriev
 0016bf10: 6520 7468 6520 6e75 6d62 6572 206f 6620  e the number of 
 0016bf20: 656c 656d 656e 7473 2069 6e20 6120 6765  elements in a ge
 0016bf30: 6f6d 6574 7279 2066 6f72 2065 6163 6820  ometry for each 
 0016bf40: 6174 7472 6962 7574 6520 646f 6d61 696e  attribute domain
 0016bf50: 0a0a 2020 2222 220a 0a20 2063 6f6d 706f  ..  """..  compo
 0016bf60: 6e65 6e74 3a20 7374 7220 3d20 2e2e 2e0a  nent: str = ....
@@ -93212,16 +93212,16 @@
 0016c1b0: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 0016c1c0: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 0016c1d0: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 0016c1e0: 0a63 6c61 7373 2047 656f 6d65 7472 794e  .class GeometryN
 0016c1f0: 6f64 6541 7474 7269 6275 7465 5374 6174  odeAttributeStat
 0016c200: 6973 7469 6328 6270 795f 7374 7275 6374  istic(bpy_struct
 0016c210: 2c20 4765 6f6d 6574 7279 4e6f 6465 2c20  , GeometryNode, 
-0016c220: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-0016c230: 616c 293a 0a0a 2020 2222 220a 0a20 2043  al):..  """..  C
+0016c220: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+0016c230: 6465 293a 0a0a 2020 2222 220a 0a20 2043  de):..  """..  C
 0016c240: 616c 6375 6c61 7465 2073 7461 7469 7374  alculate statist
 0016c250: 6963 7320 6162 6f75 7420 6120 6461 7461  ics about a data
 0016c260: 2073 6574 2066 726f 6d20 6120 6669 656c   set from a fiel
 0016c270: 6420 6576 616c 7561 7465 6420 6f6e 2061  d evaluated on a
 0016c280: 2067 656f 6d65 7472 790a 0a20 2022 2222   geometry..  """
 0016c290: 0a0a 2020 6461 7461 5f74 7970 653a 2073  ..  data_type: s
 0016c2a0: 7472 203d 202e 2e2e 0a0a 2020 2222 220a  tr = .....  """.
@@ -93273,16 +93273,16 @@
 0016c580: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 0016c590: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 0016c5a0: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 0016c5b0: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 0016c5c0: 6c61 7373 2047 656f 6d65 7472 794e 6f64  lass GeometryNod
 0016c5d0: 6542 6c75 7241 7474 7269 6275 7465 2862  eBlurAttribute(b
 0016c5e0: 7079 5f73 7472 7563 742c 2047 656f 6d65  py_struct, Geome
-0016c5f0: 7472 794e 6f64 652c 204e 6f64 652c 204e  tryNode, Node, N
-0016c600: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+0016c5f0: 7472 794e 6f64 652c 204e 6f64 6549 6e74  tryNode, NodeInt
+0016c600: 6572 6e61 6c2c 204e 6f64 6529 3a0a 0a20  ernal, Node):.. 
 0016c610: 2022 2222 0a0a 2020 4d69 7820 6174 7472   """..  Mix attr
 0016c620: 6962 7574 6520 7661 6c75 6573 206f 6620  ibute values of 
 0016c630: 6e65 6967 6862 6f72 696e 6720 656c 656d  neighboring elem
 0016c640: 656e 7473 0a0a 2020 2222 220a 0a20 2064  ents..  """..  d
 0016c650: 6174 615f 7479 7065 3a20 7374 7220 3d20  ata_type: str = 
 0016c660: 2e2e 2e0a 0a20 2040 636c 6173 736d 6574  .....  @classmet
 0016c670: 686f 640a 0a20 2064 6566 2069 735f 7265  hod..  def is_re
@@ -93322,16 +93322,16 @@
 0016c890: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 0016c8a0: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 0016c8b0: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 0016c8c0: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 0016c8d0: 2e2e 2e0a 0a63 6c61 7373 2047 656f 6d65  .....class Geome
 0016c8e0: 7472 794e 6f64 6542 6f75 6e64 426f 7828  tryNodeBoundBox(
 0016c8f0: 6270 795f 7374 7275 6374 2c20 4765 6f6d  bpy_struct, Geom
-0016c900: 6574 7279 4e6f 6465 2c20 4e6f 6465 2c20  etryNode, Node, 
-0016c910: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+0016c900: 6574 7279 4e6f 6465 2c20 4e6f 6465 496e  etryNode, NodeIn
+0016c910: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 0016c920: 2020 2222 220a 0a20 2043 616c 6375 6c61    """..  Calcula
 0016c930: 7465 2074 6865 206c 696d 6974 7320 6f66  te the limits of
 0016c940: 2061 2067 656f 6d65 7472 7927 7320 706f   a geometry's po
 0016c950: 7369 7469 6f6e 7320 616e 6420 6765 6e65  sitions and gene
 0016c960: 7261 7465 2061 2062 6f78 206d 6573 6820  rate a box mesh 
 0016c970: 7769 7468 2074 686f 7365 2064 696d 656e  with those dimen
 0016c980: 7369 6f6e 730a 0a20 2022 2222 0a0a 2020  sions..  """..  
@@ -93373,16 +93373,16 @@
 0016cbc0: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 0016cbd0: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 0016cbe0: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 0016cbf0: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 0016cc00: 6173 7320 4765 6f6d 6574 7279 4e6f 6465  ass GeometryNode
 0016cc10: 4361 7074 7572 6541 7474 7269 6275 7465  CaptureAttribute
 0016cc20: 2862 7079 5f73 7472 7563 742c 2047 656f  (bpy_struct, Geo
-0016cc30: 6d65 7472 794e 6f64 652c 204e 6f64 652c  metryNode, Node,
-0016cc40: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+0016cc30: 6d65 7472 794e 6f64 652c 204e 6f64 6549  metryNode, NodeI
+0016cc40: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 0016cc50: 0a20 2022 2222 0a0a 2020 5374 6f72 6520  .  """..  Store 
 0016cc60: 7468 6520 7265 7375 6c74 206f 6620 6120  the result of a 
 0016cc70: 6669 656c 6420 6f6e 2061 2067 656f 6d65  field on a geome
 0016cc80: 7472 7920 616e 6420 6f75 7470 7574 2074  try and output t
 0016cc90: 6865 2064 6174 6120 6173 2061 206e 6f64  he data as a nod
 0016cca0: 6520 736f 636b 6574 2e20 416c 6c6f 7773  e socket. Allows
 0016ccb0: 2072 656d 656d 6265 7269 6e67 206f 7220   remembering or 
@@ -93439,16 +93439,16 @@
 0016cfe0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 0016cff0: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 0016d000: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 0016d010: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 0016d020: 2047 656f 6d65 7472 794e 6f64 6543 6f6c   GeometryNodeCol
 0016d030: 6c65 6374 696f 6e49 6e66 6f28 6270 795f  lectionInfo(bpy_
 0016d040: 7374 7275 6374 2c20 4765 6f6d 6574 7279  struct, Geometry
-0016d050: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-0016d060: 496e 7465 726e 616c 293a 0a0a 2020 2222  Internal):..  ""
+0016d050: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
+0016d060: 616c 2c20 4e6f 6465 293a 0a0a 2020 2222  al, Node):..  ""
 0016d070: 220a 0a20 2052 6574 7269 6576 6520 6765  "..  Retrieve ge
 0016d080: 6f6d 6574 7279 2069 6e73 7461 6e63 6573  ometry instances
 0016d090: 2066 726f 6d20 6120 636f 6c6c 6563 7469   from a collecti
 0016d0a0: 6f6e 0a0a 2020 2222 220a 0a20 2074 7261  on..  """..  tra
 0016d0b0: 6e73 666f 726d 5f73 7061 6365 3a20 7374  nsform_space: st
 0016d0c0: 7220 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  r = .....  """..
 0016d0d0: 2020 5468 6520 7472 616e 7366 6f72 6d61    The transforma
@@ -93510,16 +93510,16 @@
 0016d450: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 0016d460: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 0016d470: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 0016d480: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 0016d490: 0a63 6c61 7373 2047 656f 6d65 7472 794e  .class GeometryN
 0016d4a0: 6f64 6543 6f6e 7665 7848 756c 6c28 6270  odeConvexHull(bp
 0016d4b0: 795f 7374 7275 6374 2c20 4765 6f6d 6574  y_struct, Geomet
-0016d4c0: 7279 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  ryNode, Node, No
-0016d4d0: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+0016d4c0: 7279 4e6f 6465 2c20 4e6f 6465 496e 7465  ryNode, NodeInte
+0016d4d0: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 0016d4e0: 2222 220a 0a20 2043 7265 6174 6520 6120  """..  Create a 
 0016d4f0: 6d65 7368 2074 6861 7420 656e 636c 6f73  mesh that enclos
 0016d500: 6573 2061 6c6c 2070 6f69 6e74 7320 696e  es all points in
 0016d510: 2074 6865 2069 6e70 7574 2067 656f 6d65   the input geome
 0016d520: 7472 7920 7769 7468 2074 6865 2073 6d61  try with the sma
 0016d530: 6c6c 6573 7420 6e75 6d62 6572 206f 6620  llest number of 
 0016d540: 706f 696e 7473 0a0a 2020 2222 220a 0a20  points..  """.. 
@@ -93561,16 +93561,16 @@
 0016d780: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 0016d790: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 0016d7a0: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 0016d7b0: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 0016d7c0: 6c61 7373 2047 656f 6d65 7472 794e 6f64  lass GeometryNod
 0016d7d0: 6543 6f72 6e65 7273 4f66 4661 6365 2862  eCornersOfFace(b
 0016d7e0: 7079 5f73 7472 7563 742c 2047 656f 6d65  py_struct, Geome
-0016d7f0: 7472 794e 6f64 652c 204e 6f64 652c 204e  tryNode, Node, N
-0016d800: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+0016d7f0: 7472 794e 6f64 652c 204e 6f64 6549 6e74  tryNode, NodeInt
+0016d800: 6572 6e61 6c2c 204e 6f64 6529 3a0a 0a20  ernal, Node):.. 
 0016d810: 2022 2222 0a0a 2020 5265 7472 6965 7665   """..  Retrieve
 0016d820: 2063 6f72 6e65 7273 2074 6861 7420 6d61   corners that ma
 0016d830: 6b65 2075 7020 6120 6661 6365 0a0a 2020  ke up a face..  
 0016d840: 2222 220a 0a20 2040 636c 6173 736d 6574  """..  @classmet
 0016d850: 686f 640a 0a20 2064 6566 2069 735f 7265  hod..  def is_re
 0016d860: 6769 7374 6572 6564 5f6e 6f64 655f 7479  gistered_node_ty
 0016d870: 7065 2863 6c73 2920 2d3e 2062 6f6f 6c3a  pe(cls) -> bool:
@@ -93609,16 +93609,16 @@
 0016da80: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 0016da90: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 0016daa0: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 0016dab0: 2e2e 2e0a 0a63 6c61 7373 2047 656f 6d65  .....class Geome
 0016dac0: 7472 794e 6f64 6543 6f72 6e65 7273 4f66  tryNodeCornersOf
 0016dad0: 5665 7274 6578 2862 7079 5f73 7472 7563  Vertex(bpy_struc
 0016dae0: 742c 2047 656f 6d65 7472 794e 6f64 652c  t, GeometryNode,
-0016daf0: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-0016db00: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+0016daf0: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+0016db00: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 0016db10: 5265 7472 6965 7665 2066 6163 6520 636f  Retrieve face co
 0016db20: 726e 6572 7320 636f 6e6e 6563 7465 6420  rners connected 
 0016db30: 746f 2076 6572 7469 6365 730a 0a20 2022  to vertices..  "
 0016db40: 2222 0a0a 2020 4063 6c61 7373 6d65 7468  ""..  @classmeth
 0016db50: 6f64 0a0a 2020 6465 6620 6973 5f72 6567  od..  def is_reg
 0016db60: 6973 7465 7265 645f 6e6f 6465 5f74 7970  istered_node_typ
 0016db70: 6528 636c 7329 202d 3e20 626f 6f6c 3a0a  e(cls) -> bool:.
@@ -93656,16 +93656,16 @@
 0016dd70: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 0016dd80: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 0016dd90: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 0016dda0: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 0016ddb0: 2e2e 0a0a 636c 6173 7320 4765 6f6d 6574  ....class Geomet
 0016ddc0: 7279 4e6f 6465 4375 7276 6541 7263 2862  ryNodeCurveArc(b
 0016ddd0: 7079 5f73 7472 7563 742c 2047 656f 6d65  py_struct, Geome
-0016dde0: 7472 794e 6f64 652c 204e 6f64 652c 204e  tryNode, Node, N
-0016ddf0: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+0016dde0: 7472 794e 6f64 652c 204e 6f64 6549 6e74  tryNode, NodeInt
+0016ddf0: 6572 6e61 6c2c 204e 6f64 6529 3a0a 0a20  ernal, Node):.. 
 0016de00: 2022 2222 0a0a 2020 4765 6e65 7261 7465   """..  Generate
 0016de10: 2061 2070 6f6c 7920 7370 6c69 6e65 2061   a poly spline a
 0016de20: 7263 0a0a 2020 2222 220a 0a20 206d 6f64  rc..  """..  mod
 0016de30: 653a 2073 7472 203d 202e 2e2e 0a0a 2020  e: str = .....  
 0016de40: 2222 220a 0a20 204d 6574 686f 6420 7573  """..  Method us
 0016de50: 6564 2074 6f20 6465 7465 726d 696e 6520  ed to determine 
 0016de60: 7261 6469 7573 2061 6e64 2070 6c61 6365  radius and place
@@ -93719,16 +93719,16 @@
 0016e160: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 0016e170: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 0016e180: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 0016e190: 6c61 7373 2047 656f 6d65 7472 794e 6f64  lass GeometryNod
 0016e1a0: 6543 7572 7665 456e 6470 6f69 6e74 5365  eCurveEndpointSe
 0016e1b0: 6c65 6374 696f 6e28 6270 795f 7374 7275  lection(bpy_stru
 0016e1c0: 6374 2c20 4765 6f6d 6574 7279 4e6f 6465  ct, GeometryNode
-0016e1d0: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-0016e1e0: 726e 616c 293a 0a0a 2020 2222 220a 0a20  rnal):..  """.. 
+0016e1d0: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+0016e1e0: 4e6f 6465 293a 0a0a 2020 2222 220a 0a20  Node):..  """.. 
 0016e1f0: 2050 726f 7669 6465 2061 2073 656c 6563   Provide a selec
 0016e200: 7469 6f6e 2066 6f72 2061 6e20 6172 6269  tion for an arbi
 0016e210: 7472 6172 7920 6e75 6d62 6572 206f 6620  trary number of 
 0016e220: 656e 6470 6f69 6e74 7320 696e 2065 6163  endpoints in eac
 0016e230: 6820 7370 6c69 6e65 0a0a 2020 2222 220a  h spline..  """.
 0016e240: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
 0016e250: 0a20 2064 6566 2069 735f 7265 6769 7374  .  def is_regist
@@ -93769,16 +93769,16 @@
 0016e480: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 0016e490: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 0016e4a0: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 0016e4b0: 0a63 6c61 7373 2047 656f 6d65 7472 794e  .class GeometryN
 0016e4c0: 6f64 6543 7572 7665 4861 6e64 6c65 5479  odeCurveHandleTy
 0016e4d0: 7065 5365 6c65 6374 696f 6e28 6270 795f  peSelection(bpy_
 0016e4e0: 7374 7275 6374 2c20 4765 6f6d 6574 7279  struct, Geometry
-0016e4f0: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-0016e500: 496e 7465 726e 616c 293a 0a0a 2020 2222  Internal):..  ""
+0016e4f0: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
+0016e500: 616c 2c20 4e6f 6465 293a 0a0a 2020 2222  al, Node):..  ""
 0016e510: 220a 0a20 2050 726f 7669 6465 2061 2073  "..  Provide a s
 0016e520: 656c 6563 7469 6f6e 2062 6173 6564 206f  election based o
 0016e530: 6e20 7468 6520 6861 6e64 6c65 2074 7970  n the handle typ
 0016e540: 6573 206f 6620 42c3 a97a 6965 7220 636f  es of B..zier co
 0016e550: 6e74 726f 6c20 706f 696e 7473 0a0a 2020  ntrol points..  
 0016e560: 2222 220a 0a20 2068 616e 646c 655f 7479  """..  handle_ty
 0016e570: 7065 3a20 7374 7220 3d20 2e2e 2e0a 0a20  pe: str = ..... 
@@ -93857,16 +93857,16 @@
 0016ea00: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 0016ea10: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 0016ea20: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 0016ea30: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 0016ea40: 6c61 7373 2047 656f 6d65 7472 794e 6f64  lass GeometryNod
 0016ea50: 6543 7572 7665 4c65 6e67 7468 2862 7079  eCurveLength(bpy
 0016ea60: 5f73 7472 7563 742c 2047 656f 6d65 7472  _struct, Geometr
-0016ea70: 794e 6f64 652c 204e 6f64 652c 204e 6f64  yNode, Node, Nod
-0016ea80: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2022  eInternal):..  "
+0016ea70: 794e 6f64 652c 204e 6f64 6549 6e74 6572  yNode, NodeInter
+0016ea80: 6e61 6c2c 204e 6f64 6529 3a0a 0a20 2022  nal, Node):..  "
 0016ea90: 2222 0a0a 2020 5265 7472 6965 7665 2074  ""..  Retrieve t
 0016eaa0: 6865 206c 656e 6774 6820 6f66 2061 6c6c  he length of all
 0016eab0: 2073 706c 696e 6573 2061 6464 6564 2074   splines added t
 0016eac0: 6f67 6574 6865 720a 0a20 2022 2222 0a0a  ogether..  """..
 0016ead0: 2020 4063 6c61 7373 6d65 7468 6f64 0a0a    @classmethod..
 0016eae0: 2020 6465 6620 6973 5f72 6567 6973 7465    def is_registe
 0016eaf0: 7265 645f 6e6f 6465 5f74 7970 6528 636c  red_node_type(cl
@@ -93905,16 +93905,16 @@
 0016ed00: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 0016ed10: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 0016ed20: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 0016ed30: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 0016ed40: 636c 6173 7320 4765 6f6d 6574 7279 4e6f  class GeometryNo
 0016ed50: 6465 4375 7276 654f 6650 6f69 6e74 2862  deCurveOfPoint(b
 0016ed60: 7079 5f73 7472 7563 742c 2047 656f 6d65  py_struct, Geome
-0016ed70: 7472 794e 6f64 652c 204e 6f64 652c 204e  tryNode, Node, N
-0016ed80: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+0016ed70: 7472 794e 6f64 652c 204e 6f64 6549 6e74  tryNode, NodeInt
+0016ed80: 6572 6e61 6c2c 204e 6f64 6529 3a0a 0a20  ernal, Node):.. 
 0016ed90: 2022 2222 0a0a 2020 5265 7472 6965 7665   """..  Retrieve
 0016eda0: 2074 6865 2063 7572 7665 2061 2063 6f6e   the curve a con
 0016edb0: 7472 6f6c 2070 6f69 6e74 2069 7320 7061  trol point is pa
 0016edc0: 7274 206f 660a 0a20 2022 2222 0a0a 2020  rt of..  """..  
 0016edd0: 4063 6c61 7373 6d65 7468 6f64 0a0a 2020  @classmethod..  
 0016ede0: 6465 6620 6973 5f72 6567 6973 7465 7265  def is_registere
 0016edf0: 645f 6e6f 6465 5f74 7970 6528 636c 7329  d_node_type(cls)
@@ -93954,16 +93954,16 @@
 0016f010: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 0016f020: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 0016f030: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 0016f040: 6173 7320 4765 6f6d 6574 7279 4e6f 6465  ass GeometryNode
 0016f050: 4375 7276 6550 7269 6d69 7469 7665 4265  CurvePrimitiveBe
 0016f060: 7a69 6572 5365 676d 656e 7428 6270 795f  zierSegment(bpy_
 0016f070: 7374 7275 6374 2c20 4765 6f6d 6574 7279  struct, Geometry
-0016f080: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-0016f090: 496e 7465 726e 616c 293a 0a0a 2020 2222  Internal):..  ""
+0016f080: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
+0016f090: 616c 2c20 4e6f 6465 293a 0a0a 2020 2222  al, Node):..  ""
 0016f0a0: 220a 0a20 2047 656e 6572 6174 6520 6120  "..  Generate a 
 0016f0b0: 3244 2042 c3a9 7a69 6572 2073 706c 696e  2D B..zier splin
 0016f0c0: 6520 6672 6f6d 2074 6865 2067 6976 656e  e from the given
 0016f0d0: 2063 6f6e 7472 6f6c 2070 6f69 6e74 7320   control points 
 0016f0e0: 616e 6420 6861 6e64 6c65 730a 0a20 2022  and handles..  "
 0016f0f0: 2222 0a0a 2020 6d6f 6465 3a20 7374 7220  ""..  mode: str 
 0016f100: 3d20 2e2e 2e0a 0a20 2022 2222 0a0a 2020  = .....  """..  
@@ -94020,16 +94020,16 @@
 0016f430: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 0016f440: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 0016f450: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 0016f460: 636c 6173 7320 4765 6f6d 6574 7279 4e6f  class GeometryNo
 0016f470: 6465 4375 7276 6550 7269 6d69 7469 7665  deCurvePrimitive
 0016f480: 4369 7263 6c65 2862 7079 5f73 7472 7563  Circle(bpy_struc
 0016f490: 742c 2047 656f 6d65 7472 794e 6f64 652c  t, GeometryNode,
-0016f4a0: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-0016f4b0: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+0016f4a0: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+0016f4b0: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 0016f4c0: 4765 6e65 7261 7465 2061 2070 6f6c 7920  Generate a poly 
 0016f4d0: 7370 6c69 6e65 2063 6972 636c 650a 0a20  spline circle.. 
 0016f4e0: 2022 2222 0a0a 2020 6d6f 6465 3a20 7374   """..  mode: st
 0016f4f0: 7220 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  r = .....  """..
 0016f500: 2020 4d65 7468 6f64 2075 7365 6420 746f    Method used to
 0016f510: 2064 6574 6572 6d69 6e65 2072 6164 6975   determine radiu
 0016f520: 7320 616e 6420 706c 6163 656d 656e 740a  s and placement.
@@ -94081,15 +94081,15 @@
 0016f800: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 0016f810: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 0016f820: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 0016f830: 6173 7320 4765 6f6d 6574 7279 4e6f 6465  ass GeometryNode
 0016f840: 4375 7276 6550 7269 6d69 7469 7665 4c69  CurvePrimitiveLi
 0016f850: 6e65 2862 7079 5f73 7472 7563 742c 2047  ne(bpy_struct, G
 0016f860: 656f 6d65 7472 794e 6f64 652c 204e 6f64  eometryNode, Nod
-0016f870: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+0016f870: 6549 6e74 6572 6e61 6c2c 204e 6f64 6529  eInternal, Node)
 0016f880: 3a0a 0a20 2022 2222 0a0a 2020 4765 6e65  :..  """..  Gene
 0016f890: 7261 7465 2061 2070 6f6c 7920 7370 6c69  rate a poly spli
 0016f8a0: 6e65 206c 696e 6520 7769 7468 2074 776f  ne line with two
 0016f8b0: 2070 6f69 6e74 730a 0a20 2022 2222 0a0a   points..  """..
 0016f8c0: 2020 6d6f 6465 3a20 7374 7220 3d20 2e2e    mode: str = ..
 0016f8d0: 2e0a 0a20 2022 2222 0a0a 2020 4d65 7468  ...  """..  Meth
 0016f8e0: 6f64 2075 7365 6420 746f 2064 6574 6572  od used to deter
@@ -94144,16 +94144,16 @@
 0016fbf0: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 0016fc00: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 0016fc10: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 0016fc20: 0a63 6c61 7373 2047 656f 6d65 7472 794e  .class GeometryN
 0016fc30: 6f64 6543 7572 7665 5072 696d 6974 6976  odeCurvePrimitiv
 0016fc40: 6551 7561 6472 696c 6174 6572 616c 2862  eQuadrilateral(b
 0016fc50: 7079 5f73 7472 7563 742c 2047 656f 6d65  py_struct, Geome
-0016fc60: 7472 794e 6f64 652c 204e 6f64 652c 204e  tryNode, Node, N
-0016fc70: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+0016fc60: 7472 794e 6f64 652c 204e 6f64 6549 6e74  tryNode, NodeInt
+0016fc70: 6572 6e61 6c2c 204e 6f64 6529 3a0a 0a20  ernal, Node):.. 
 0016fc80: 2022 2222 0a0a 2020 4765 6e65 7261 7465   """..  Generate
 0016fc90: 2061 2070 6f6c 7967 6f6e 2077 6974 6820   a polygon with 
 0016fca0: 666f 7572 2070 6f69 6e74 730a 0a20 2022  four points..  "
 0016fcb0: 2222 0a0a 2020 6d6f 6465 3a20 7374 7220  ""..  mode: str 
 0016fcc0: 3d20 2e2e 2e0a 0a20 2022 2222 0a0a 2020  = .....  """..  
 0016fcd0: 2a20 6060 5245 4354 414e 474c 4560 600a  * ``RECTANGLE``.
 0016fce0: 5265 6374 616e 676c 6520 2d2d 2043 7265  Rectangle -- Cre
@@ -94212,15 +94212,15 @@
 00170030: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 00170040: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 00170050: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 00170060: 7320 4765 6f6d 6574 7279 4e6f 6465 4375  s GeometryNodeCu
 00170070: 7276 6551 7561 6472 6174 6963 4265 7a69  rveQuadraticBezi
 00170080: 6572 2862 7079 5f73 7472 7563 742c 2047  er(bpy_struct, G
 00170090: 656f 6d65 7472 794e 6f64 652c 204e 6f64  eometryNode, Nod
-001700a0: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+001700a0: 6549 6e74 6572 6e61 6c2c 204e 6f64 6529  eInternal, Node)
 001700b0: 3a0a 0a20 2022 2222 0a0a 2020 4765 6e65  :..  """..  Gene
 001700c0: 7261 7465 2061 2070 6f6c 7920 7370 6c69  rate a poly spli
 001700d0: 6e65 2069 6e20 6120 7061 7261 626f 6c61  ne in a parabola
 001700e0: 2073 6861 7065 2077 6974 6820 636f 6e74   shape with cont
 001700f0: 726f 6c20 706f 696e 7473 2070 6f73 6974  rol points posit
 00170100: 696f 6e73 0a0a 2020 2222 220a 0a20 2040  ions..  """..  @
 00170110: 636c 6173 736d 6574 686f 640a 0a20 2064  classmethod..  d
@@ -94261,16 +94261,16 @@
 00170340: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 00170350: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 00170360: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 00170370: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 00170380: 7373 2047 656f 6d65 7472 794e 6f64 6543  ss GeometryNodeC
 00170390: 7572 7665 5365 7448 616e 646c 6573 2862  urveSetHandles(b
 001703a0: 7079 5f73 7472 7563 742c 2047 656f 6d65  py_struct, Geome
-001703b0: 7472 794e 6f64 652c 204e 6f64 652c 204e  tryNode, Node, N
-001703c0: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+001703b0: 7472 794e 6f64 652c 204e 6f64 6549 6e74  tryNode, NodeInt
+001703c0: 6572 6e61 6c2c 204e 6f64 6529 3a0a 0a20  ernal, Node):.. 
 001703d0: 2022 2222 0a0a 2020 5365 7420 7468 6520   """..  Set the 
 001703e0: 6861 6e64 6c65 2074 7970 6520 666f 7220  handle type for 
 001703f0: 7468 6520 636f 6e74 726f 6c20 706f 696e  the control poin
 00170400: 7473 206f 6620 6120 42c3 a97a 6965 7220  ts of a B..zier 
 00170410: 6375 7276 650a 0a20 2022 2222 0a0a 2020  curve..  """..  
 00170420: 6861 6e64 6c65 5f74 7970 653a 2073 7472  handle_type: str
 00170430: 203d 202e 2e2e 0a0a 2020 2222 220a 0a20   = .....  """.. 
@@ -94348,16 +94348,16 @@
 001708b0: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 001708c0: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 001708d0: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 001708e0: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 001708f0: 7373 2047 656f 6d65 7472 794e 6f64 6543  ss GeometryNodeC
 00170900: 7572 7665 5370 6972 616c 2862 7079 5f73  urveSpiral(bpy_s
 00170910: 7472 7563 742c 2047 656f 6d65 7472 794e  truct, GeometryN
-00170920: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-00170930: 6e74 6572 6e61 6c29 3a0a 0a20 2022 2222  nternal):..  """
+00170920: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
+00170930: 6c2c 204e 6f64 6529 3a0a 0a20 2022 2222  l, Node):..  """
 00170940: 0a0a 2020 4765 6e65 7261 7465 2061 2070  ..  Generate a p
 00170950: 6f6c 7920 7370 6c69 6e65 2069 6e20 6120  oly spline in a 
 00170960: 7370 6972 616c 2073 6861 7065 0a0a 2020  spiral shape..  
 00170970: 2222 220a 0a20 2040 636c 6173 736d 6574  """..  @classmet
 00170980: 686f 640a 0a20 2064 6566 2069 735f 7265  hod..  def is_re
 00170990: 6769 7374 6572 6564 5f6e 6f64 655f 7479  gistered_node_ty
 001709a0: 7065 2863 6c73 2920 2d3e 2062 6f6f 6c3a  pe(cls) -> bool:
@@ -94396,16 +94396,16 @@
 00170bb0: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 00170bc0: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 00170bd0: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 00170be0: 2e2e 2e0a 0a63 6c61 7373 2047 656f 6d65  .....class Geome
 00170bf0: 7472 794e 6f64 6543 7572 7665 5370 6c69  tryNodeCurveSpli
 00170c00: 6e65 5479 7065 2862 7079 5f73 7472 7563  neType(bpy_struc
 00170c10: 742c 2047 656f 6d65 7472 794e 6f64 652c  t, GeometryNode,
-00170c20: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-00170c30: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+00170c20: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+00170c30: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 00170c40: 4368 616e 6765 2074 6865 2074 7970 6520  Change the type 
 00170c50: 6f66 2063 7572 7665 730a 0a20 2022 2222  of curves..  """
 00170c60: 0a0a 2020 7370 6c69 6e65 5f74 7970 653a  ..  spline_type:
 00170c70: 2073 7472 203d 202e 2e2e 0a0a 2020 2222   str = .....  ""
 00170c80: 220a 0a20 2054 6865 2063 7572 7665 2074  "..  The curve t
 00170c90: 7970 6520 746f 2063 6861 6e67 6520 7468  ype to change th
 00170ca0: 6520 7365 6c65 6374 6564 2063 7572 7665  e selected curve
@@ -94448,16 +94448,16 @@
 00170ef0: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 00170f00: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 00170f10: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 00170f20: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 00170f30: 7373 2047 656f 6d65 7472 794e 6f64 6543  ss GeometryNodeC
 00170f40: 7572 7665 5374 6172 2862 7079 5f73 7472  urveStar(bpy_str
 00170f50: 7563 742c 2047 656f 6d65 7472 794e 6f64  uct, GeometryNod
-00170f60: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-00170f70: 6572 6e61 6c29 3a0a 0a20 2022 2222 0a0a  ernal):..  """..
+00170f60: 652c 204e 6f64 6549 6e74 6572 6e61 6c2c  e, NodeInternal,
+00170f70: 204e 6f64 6529 3a0a 0a20 2022 2222 0a0a   Node):..  """..
 00170f80: 2020 4765 6e65 7261 7465 2061 2070 6f6c    Generate a pol
 00170f90: 7920 7370 6c69 6e65 2069 6e20 6120 7374  y spline in a st
 00170fa0: 6172 2070 6174 7465 726e 2062 7920 636f  ar pattern by co
 00170fb0: 6e6e 6563 7469 6e67 2061 6c74 6572 6e61  nnecting alterna
 00170fc0: 7469 6e67 2070 6f69 6e74 7320 6f66 2074  ting points of t
 00170fd0: 776f 2063 6972 636c 6573 0a0a 2020 2222  wo circles..  ""
 00170fe0: 220a 0a20 2040 636c 6173 736d 6574 686f  "..  @classmetho
@@ -94498,16 +94498,16 @@
 00171210: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 00171220: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 00171230: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 00171240: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 00171250: 2e0a 0a63 6c61 7373 2047 656f 6d65 7472  ...class Geometr
 00171260: 794e 6f64 6543 7572 7665 546f 4d65 7368  yNodeCurveToMesh
 00171270: 2862 7079 5f73 7472 7563 742c 2047 656f  (bpy_struct, Geo
-00171280: 6d65 7472 794e 6f64 652c 204e 6f64 652c  metryNode, Node,
-00171290: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+00171280: 6d65 7472 794e 6f64 652c 204e 6f64 6549  metryNode, NodeI
+00171290: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 001712a0: 0a20 2022 2222 0a0a 2020 436f 6e76 6572  .  """..  Conver
 001712b0: 7420 6375 7276 6573 2069 6e74 6f20 6120  t curves into a 
 001712c0: 6d65 7368 2c20 6f70 7469 6f6e 616c 6c79  mesh, optionally
 001712d0: 2077 6974 6820 6120 6375 7374 6f6d 2070   with a custom p
 001712e0: 726f 6669 6c65 2073 6861 7065 2064 6566  rofile shape def
 001712f0: 696e 6564 2062 7920 6375 7276 6573 0a0a  ined by curves..
 00171300: 2020 2222 220a 0a20 2040 636c 6173 736d    """..  @classm
@@ -94549,16 +94549,16 @@
 00171540: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 00171550: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 00171560: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 00171570: 2020 2e2e 2e0a 0a63 6c61 7373 2047 656f    .....class Geo
 00171580: 6d65 7472 794e 6f64 6543 7572 7665 546f  metryNodeCurveTo
 00171590: 506f 696e 7473 2862 7079 5f73 7472 7563  Points(bpy_struc
 001715a0: 742c 2047 656f 6d65 7472 794e 6f64 652c  t, GeometryNode,
-001715b0: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-001715c0: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+001715b0: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+001715c0: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 001715d0: 4765 6e65 7261 7465 2061 2070 6f69 6e74  Generate a point
 001715e0: 2063 6c6f 7564 2062 7920 7361 6d70 6c69   cloud by sampli
 001715f0: 6e67 2070 6f73 6974 696f 6e73 2061 6c6f  ng positions alo
 00171600: 6e67 2063 7572 7665 730a 0a20 2022 2222  ng curves..  """
 00171610: 0a0a 2020 6d6f 6465 3a20 7374 7220 3d20  ..  mode: str = 
 00171620: 2e2e 2e0a 0a20 2022 2222 0a0a 2020 486f  .....  """..  Ho
 00171630: 7720 746f 2067 656e 6572 6174 6520 706f  w to generate po
@@ -94624,16 +94624,16 @@
 001719f0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 00171a00: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 00171a10: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 00171a20: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 00171a30: 2047 656f 6d65 7472 794e 6f64 6543 7573   GeometryNodeCus
 00171a40: 746f 6d47 726f 7570 2862 7079 5f73 7472  tomGroup(bpy_str
 00171a50: 7563 742c 2047 656f 6d65 7472 794e 6f64  uct, GeometryNod
-00171a60: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-00171a70: 6572 6e61 6c29 3a0a 0a20 2022 2222 0a0a  ernal):..  """..
+00171a60: 652c 204e 6f64 6549 6e74 6572 6e61 6c2c  e, NodeInternal,
+00171a70: 204e 6f64 6529 3a0a 0a20 2022 2222 0a0a   Node):..  """..
 00171a80: 2020 4375 7374 6f6d 2047 656f 6d65 7472    Custom Geometr
 00171a90: 7920 4772 6f75 7020 4e6f 6465 2066 6f72  y Group Node for
 00171aa0: 2050 7974 686f 6e20 6e6f 6465 730a 0a20   Python nodes.. 
 00171ab0: 2022 2222 0a0a 2020 6e6f 6465 5f74 7265   """..  node_tre
 00171ac0: 653a 204e 6f64 6554 7265 6520 3d20 2e2e  e: NodeTree = ..
 00171ad0: 2e0a 0a20 2040 636c 6173 736d 6574 686f  ...  @classmetho
 00171ae0: 640a 0a20 2064 6566 2062 6c5f 726e 615f  d..  def bl_rna_
@@ -94649,16 +94649,16 @@
 00171b80: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 00171b90: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 00171ba0: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 00171bb0: 7373 2047 656f 6d65 7472 794e 6f64 6544  ss GeometryNodeD
 00171bc0: 6566 6f72 6d43 7572 7665 734f 6e53 7572  eformCurvesOnSur
 00171bd0: 6661 6365 2862 7079 5f73 7472 7563 742c  face(bpy_struct,
 00171be0: 2047 656f 6d65 7472 794e 6f64 652c 204e   GeometryNode, N
-00171bf0: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-00171c00: 6c29 3a0a 0a20 2022 2222 0a0a 2020 5472  l):..  """..  Tr
+00171bf0: 6f64 6549 6e74 6572 6e61 6c2c 204e 6f64  odeInternal, Nod
+00171c00: 6529 3a0a 0a20 2022 2222 0a0a 2020 5472  e):..  """..  Tr
 00171c10: 616e 736c 6174 6520 616e 6420 726f 7461  anslate and rota
 00171c20: 7465 2063 7572 7665 7320 6261 7365 6420  te curves based 
 00171c30: 6f6e 2063 6861 6e67 6573 2062 6574 7765  on changes betwe
 00171c40: 656e 2074 6865 206f 626a 6563 7427 7320  en the object's 
 00171c50: 6f72 6967 696e 616c 2061 6e64 2065 7661  original and eva
 00171c60: 6c75 6174 6564 2073 7572 6661 6365 206d  luated surface m
 00171c70: 6573 680a 0a20 2022 2222 0a0a 2020 4063  esh..  """..  @c
@@ -94700,16 +94700,16 @@
 00171eb0: 2073 7472 2c20 6465 6661 756c 743a 2074   str, default: t
 00171ec0: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 00171ed0: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 00171ee0: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 00171ef0: 7320 4765 6f6d 6574 7279 4e6f 6465 4465  s GeometryNodeDe
 00171f00: 6c65 7465 4765 6f6d 6574 7279 2862 7079  leteGeometry(bpy
 00171f10: 5f73 7472 7563 742c 2047 656f 6d65 7472  _struct, Geometr
-00171f20: 794e 6f64 652c 204e 6f64 652c 204e 6f64  yNode, Node, Nod
-00171f30: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2022  eInternal):..  "
+00171f20: 794e 6f64 652c 204e 6f64 6549 6e74 6572  yNode, NodeInter
+00171f30: 6e61 6c2c 204e 6f64 6529 3a0a 0a20 2022  nal, Node):..  "
 00171f40: 2222 0a0a 2020 5265 6d6f 7665 2073 656c  ""..  Remove sel
 00171f50: 6563 7465 6420 656c 656d 656e 7473 206f  ected elements o
 00171f60: 6620 6120 6765 6f6d 6574 7279 0a0a 2020  f a geometry..  
 00171f70: 2222 220a 0a20 2064 6f6d 6169 6e3a 2073  """..  domain: s
 00171f80: 7472 203d 202e 2e2e 0a0a 2020 2222 220a  tr = .....  """.
 00171f90: 0a20 2057 6869 6368 2064 6f6d 6169 6e20  .  Which domain 
 00171fa0: 746f 2064 656c 6574 6520 696e 0a0a 2020  to delete in..  
@@ -94757,16 +94757,16 @@
 00172240: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 00172250: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 00172260: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 00172270: 2e2e 2e0a 0a63 6c61 7373 2047 656f 6d65  .....class Geome
 00172280: 7472 794e 6f64 6544 6973 7472 6962 7574  tryNodeDistribut
 00172290: 6550 6f69 6e74 7349 6e56 6f6c 756d 6528  ePointsInVolume(
 001722a0: 6270 795f 7374 7275 6374 2c20 4765 6f6d  bpy_struct, Geom
-001722b0: 6574 7279 4e6f 6465 2c20 4e6f 6465 2c20  etryNode, Node, 
-001722c0: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+001722b0: 6574 7279 4e6f 6465 2c20 4e6f 6465 496e  etryNode, NodeIn
+001722c0: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 001722d0: 2020 2222 220a 0a20 2047 656e 6572 6174    """..  Generat
 001722e0: 6520 706f 696e 7473 2069 6e73 6964 6520  e points inside 
 001722f0: 6120 766f 6c75 6d65 0a0a 2020 2222 220a  a volume..  """.
 00172300: 0a20 206d 6f64 653a 2073 7472 203d 202e  .  mode: str = .
 00172310: 2e2e 0a0a 2020 2222 220a 0a20 204d 6574  ....  """..  Met
 00172320: 686f 6420 746f 2075 7365 2066 6f72 2073  hod to use for s
 00172330: 6361 7474 6572 696e 6720 706f 696e 7473  cattering points
@@ -94821,15 +94821,15 @@
 00172640: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 00172650: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 00172660: 2020 202e 2e2e 0a0a 636c 6173 7320 4765     .....class Ge
 00172670: 6f6d 6574 7279 4e6f 6465 4469 7374 7269  ometryNodeDistri
 00172680: 6275 7465 506f 696e 7473 4f6e 4661 6365  butePointsOnFace
 00172690: 7328 6270 795f 7374 7275 6374 2c20 4765  s(bpy_struct, Ge
 001726a0: 6f6d 6574 7279 4e6f 6465 2c20 4e6f 6465  ometryNode, Node
-001726b0: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+001726b0: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 001726c0: 0a0a 2020 2222 220a 0a20 2047 656e 6572  ..  """..  Gener
 001726d0: 6174 6520 706f 696e 7473 2073 7072 6561  ate points sprea
 001726e0: 6420 6f75 7420 6f6e 2074 6865 2073 7572  d out on the sur
 001726f0: 6661 6365 206f 6620 6120 6d65 7368 0a0a  face of a mesh..
 00172700: 2020 2222 220a 0a20 2064 6973 7472 6962    """..  distrib
 00172710: 7574 655f 6d65 7468 6f64 3a20 7374 7220  ute_method: str 
 00172720: 3d20 2e2e 2e0a 0a20 2022 2222 0a0a 2020  = .....  """..  
@@ -94897,16 +94897,16 @@
 00172b00: 7928 636c 732c 2069 643a 2073 7472 2c20  y(cls, id: str, 
 00172b10: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 00172b20: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 00172b30: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 00172b40: 202e 2e2e 0a0a 636c 6173 7320 4765 6f6d   .....class Geom
 00172b50: 6574 7279 4e6f 6465 4475 616c 4d65 7368  etryNodeDualMesh
 00172b60: 2862 7079 5f73 7472 7563 742c 2047 656f  (bpy_struct, Geo
-00172b70: 6d65 7472 794e 6f64 652c 204e 6f64 652c  metryNode, Node,
-00172b80: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+00172b70: 6d65 7472 794e 6f64 652c 204e 6f64 6549  metryNode, NodeI
+00172b80: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 00172b90: 0a20 2022 2222 0a0a 2020 436f 6e76 6572  .  """..  Conver
 00172ba0: 7420 4661 6365 7320 696e 746f 2076 6572  t Faces into ver
 00172bb0: 7469 6365 7320 616e 6420 7665 7274 6963  tices and vertic
 00172bc0: 6573 2069 6e74 6f20 6661 6365 730a 0a20  es into faces.. 
 00172bd0: 2022 2222 0a0a 2020 4063 6c61 7373 6d65   """..  @classme
 00172be0: 7468 6f64 0a0a 2020 6465 6620 6973 5f72  thod..  def is_r
 00172bf0: 6567 6973 7465 7265 645f 6e6f 6465 5f74  egistered_node_t
@@ -94946,16 +94946,16 @@
 00172e10: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 00172e20: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 00172e30: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 00172e40: 202e 2e2e 0a0a 636c 6173 7320 4765 6f6d   .....class Geom
 00172e50: 6574 7279 4e6f 6465 4475 706c 6963 6174  etryNodeDuplicat
 00172e60: 6545 6c65 6d65 6e74 7328 6270 795f 7374  eElements(bpy_st
 00172e70: 7275 6374 2c20 4765 6f6d 6574 7279 4e6f  ruct, GeometryNo
-00172e80: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-00172e90: 7465 726e 616c 293a 0a0a 2020 2222 220a  ternal):..  """.
+00172e80: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+00172e90: 2c20 4e6f 6465 293a 0a0a 2020 2222 220a  , Node):..  """.
 00172ea0: 0a20 2047 656e 6572 6174 6520 616e 2061  .  Generate an a
 00172eb0: 7262 6974 7261 7279 206e 756d 6265 7220  rbitrary number 
 00172ec0: 636f 7069 6573 206f 6620 6561 6368 2073  copies of each s
 00172ed0: 656c 6563 7465 6420 696e 7075 7420 656c  elected input el
 00172ee0: 656d 656e 740a 0a20 2022 2222 0a0a 2020  ement..  """..  
 00172ef0: 646f 6d61 696e 3a20 7374 7220 3d20 2e2e  domain: str = ..
 00172f00: 2e0a 0a20 2022 2222 0a0a 2020 5768 6963  ...  """..  Whic
@@ -95000,15 +95000,15 @@
 00173170: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 00173180: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 00173190: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 001731a0: 6173 7320 4765 6f6d 6574 7279 4e6f 6465  ass GeometryNode
 001731b0: 4564 6765 5061 7468 7354 6f43 7572 7665  EdgePathsToCurve
 001731c0: 7328 6270 795f 7374 7275 6374 2c20 4765  s(bpy_struct, Ge
 001731d0: 6f6d 6574 7279 4e6f 6465 2c20 4e6f 6465  ometryNode, Node
-001731e0: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+001731e0: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 001731f0: 0a0a 2020 4063 6c61 7373 6d65 7468 6f64  ..  @classmethod
 00173200: 0a0a 2020 6465 6620 6973 5f72 6567 6973  ..  def is_regis
 00173210: 7465 7265 645f 6e6f 6465 5f74 7970 6528  tered_node_type(
 00173220: 636c 7329 202d 3e20 626f 6f6c 3a0a 0a20  cls) -> bool:.. 
 00173230: 2020 2022 2222 0a0a 2020 2020 5472 7565     """..    True
 00173240: 2069 6620 6120 7265 6769 7374 6572 6564   if a registered
 00173250: 206e 6f64 6520 7479 7065 0a0a 2020 2020   node type..    
@@ -95044,16 +95044,16 @@
 00173430: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 00173440: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 00173450: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 00173460: 0a0a 636c 6173 7320 4765 6f6d 6574 7279  ..class Geometry
 00173470: 4e6f 6465 4564 6765 5061 7468 7354 6f53  NodeEdgePathsToS
 00173480: 656c 6563 7469 6f6e 2862 7079 5f73 7472  election(bpy_str
 00173490: 7563 742c 2047 656f 6d65 7472 794e 6f64  uct, GeometryNod
-001734a0: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-001734b0: 6572 6e61 6c29 3a0a 0a20 2040 636c 6173  ernal):..  @clas
+001734a0: 652c 204e 6f64 6549 6e74 6572 6e61 6c2c  e, NodeInternal,
+001734b0: 204e 6f64 6529 3a0a 0a20 2040 636c 6173   Node):..  @clas
 001734c0: 736d 6574 686f 640a 0a20 2064 6566 2069  smethod..  def i
 001734d0: 735f 7265 6769 7374 6572 6564 5f6e 6f64  s_registered_nod
 001734e0: 655f 7479 7065 2863 6c73 2920 2d3e 2062  e_type(cls) -> b
 001734f0: 6f6f 6c3a 0a0a 2020 2020 2222 220a 0a20  ool:..    """.. 
 00173500: 2020 2054 7275 6520 6966 2061 2072 6567     True if a reg
 00173510: 6973 7465 7265 6420 6e6f 6465 2074 7970  istered node typ
 00173520: 650a 0a20 2020 2022 2222 0a0a 2020 2020  e..    """..    
@@ -95088,16 +95088,16 @@
 001736f0: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 00173700: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 00173710: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 00173720: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2047      .....class G
 00173730: 656f 6d65 7472 794e 6f64 6545 6467 6573  eometryNodeEdges
 00173740: 4f66 436f 726e 6572 2862 7079 5f73 7472  OfCorner(bpy_str
 00173750: 7563 742c 2047 656f 6d65 7472 794e 6f64  uct, GeometryNod
-00173760: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-00173770: 6572 6e61 6c29 3a0a 0a20 2022 2222 0a0a  ernal):..  """..
+00173760: 652c 204e 6f64 6549 6e74 6572 6e61 6c2c  e, NodeInternal,
+00173770: 204e 6f64 6529 3a0a 0a20 2022 2222 0a0a   Node):..  """..
 00173780: 2020 5265 7472 6965 7665 2074 6865 2065    Retrieve the e
 00173790: 6467 6573 206f 6e20 626f 7468 2073 6964  dges on both sid
 001737a0: 6573 206f 6620 6120 6661 6365 2063 6f72  es of a face cor
 001737b0: 6e65 720a 0a20 2022 2222 0a0a 2020 4063  ner..  """..  @c
 001737c0: 6c61 7373 6d65 7468 6f64 0a0a 2020 6465  lassmethod..  de
 001737d0: 6620 6973 5f72 6567 6973 7465 7265 645f  f is_registered_
 001737e0: 6e6f 6465 5f74 7970 6528 636c 7329 202d  node_type(cls) -
@@ -95136,16 +95136,16 @@
 001739f0: 2073 7472 2c20 6465 6661 756c 743a 2074   str, default: t
 00173a00: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 00173a10: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 00173a20: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 00173a30: 7320 4765 6f6d 6574 7279 4e6f 6465 4564  s GeometryNodeEd
 00173a40: 6765 734f 6656 6572 7465 7828 6270 795f  gesOfVertex(bpy_
 00173a50: 7374 7275 6374 2c20 4765 6f6d 6574 7279  struct, Geometry
-00173a60: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-00173a70: 496e 7465 726e 616c 293a 0a0a 2020 2222  Internal):..  ""
+00173a60: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
+00173a70: 616c 2c20 4e6f 6465 293a 0a0a 2020 2222  al, Node):..  ""
 00173a80: 220a 0a20 2052 6574 7269 6576 6520 7468  "..  Retrieve th
 00173a90: 6520 6564 6765 7320 636f 6e6e 6563 7465  e edges connecte
 00173aa0: 6420 746f 2065 6163 6820 7665 7274 6578  d to each vertex
 00173ab0: 0a0a 2020 2222 220a 0a20 2040 636c 6173  ..  """..  @clas
 00173ac0: 736d 6574 686f 640a 0a20 2064 6566 2069  smethod..  def i
 00173ad0: 735f 7265 6769 7374 6572 6564 5f6e 6f64  s_registered_nod
 00173ae0: 655f 7479 7065 2863 6c73 2920 2d3e 2062  e_type(cls) -> b
@@ -95184,16 +95184,16 @@
 00173cf0: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 00173d00: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 00173d10: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 00173d20: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2047      .....class G
 00173d30: 656f 6d65 7472 794e 6f64 6545 6467 6573  eometryNodeEdges
 00173d40: 546f 4661 6365 4772 6f75 7073 2862 7079  ToFaceGroups(bpy
 00173d50: 5f73 7472 7563 742c 2047 656f 6d65 7472  _struct, Geometr
-00173d60: 794e 6f64 652c 204e 6f64 652c 204e 6f64  yNode, Node, Nod
-00173d70: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2022  eInternal):..  "
+00173d60: 794e 6f64 652c 204e 6f64 6549 6e74 6572  yNode, NodeInter
+00173d70: 6e61 6c2c 204e 6f64 6529 3a0a 0a20 2022  nal, Node):..  "
 00173d80: 2222 0a0a 2020 4772 6f75 7020 6661 6365  ""..  Group face
 00173d90: 7320 696e 746f 2072 6567 696f 6e73 2073  s into regions s
 00173da0: 7572 726f 756e 6465 6420 6279 2074 6865  urrounded by the
 00173db0: 2073 656c 6563 7465 6420 626f 756e 6461   selected bounda
 00173dc0: 7279 2065 6467 6573 0a0a 2020 2222 220a  ry edges..  """.
 00173dd0: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
 00173de0: 0a20 2064 6566 2069 735f 7265 6769 7374  .  def is_regist
@@ -95233,16 +95233,16 @@
 00174000: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 00174010: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 00174020: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 00174030: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 00174040: 0a63 6c61 7373 2047 656f 6d65 7472 794e  .class GeometryN
 00174050: 6f64 6545 7874 7275 6465 4d65 7368 2862  odeExtrudeMesh(b
 00174060: 7079 5f73 7472 7563 742c 2047 656f 6d65  py_struct, Geome
-00174070: 7472 794e 6f64 652c 204e 6f64 652c 204e  tryNode, Node, N
-00174080: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+00174070: 7472 794e 6f64 652c 204e 6f64 6549 6e74  tryNode, NodeInt
+00174080: 6572 6e61 6c2c 204e 6f64 6529 3a0a 0a20  ernal, Node):.. 
 00174090: 2022 2222 0a0a 2020 4765 6e65 7261 7465   """..  Generate
 001740a0: 206e 6577 2076 6572 7469 6365 732c 2065   new vertices, e
 001740b0: 6467 6573 2c20 6f72 2066 6163 6573 2066  dges, or faces f
 001740c0: 726f 6d20 7365 6c65 6374 6564 2065 6c65  rom selected ele
 001740d0: 6d65 6e74 7320 616e 6420 6d6f 7665 2074  ments and move t
 001740e0: 6865 6d20 6261 7365 6420 6f6e 2061 6e20  hem based on an 
 001740f0: 6f66 6673 6574 2077 6869 6c65 206b 6565  offset while kee
@@ -95288,16 +95288,16 @@
 00174370: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 00174380: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 00174390: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 001743a0: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 001743b0: 0a63 6c61 7373 2047 656f 6d65 7472 794e  .class GeometryN
 001743c0: 6f64 6546 6163 654f 6643 6f72 6e65 7228  odeFaceOfCorner(
 001743d0: 6270 795f 7374 7275 6374 2c20 4765 6f6d  bpy_struct, Geom
-001743e0: 6574 7279 4e6f 6465 2c20 4e6f 6465 2c20  etryNode, Node, 
-001743f0: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+001743e0: 6574 7279 4e6f 6465 2c20 4e6f 6465 496e  etryNode, NodeIn
+001743f0: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 00174400: 2020 2222 220a 0a20 2052 6574 7269 6576    """..  Retriev
 00174410: 6520 7468 6520 6661 6365 2065 6163 6820  e the face each 
 00174420: 6661 6365 2063 6f72 6e65 7220 6973 2070  face corner is p
 00174430: 6172 7420 6f66 0a0a 2020 2222 220a 0a20  art of..  """.. 
 00174440: 2040 636c 6173 736d 6574 686f 640a 0a20   @classmethod.. 
 00174450: 2064 6566 2069 735f 7265 6769 7374 6572   def is_register
 00174460: 6564 5f6e 6f64 655f 7479 7065 2863 6c73  ed_node_type(cls
@@ -95336,16 +95336,16 @@
 00174670: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 00174680: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 00174690: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 001746a0: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 001746b0: 6c61 7373 2047 656f 6d65 7472 794e 6f64  lass GeometryNod
 001746c0: 6546 6965 6c64 4174 496e 6465 7828 6270  eFieldAtIndex(bp
 001746d0: 795f 7374 7275 6374 2c20 4765 6f6d 6574  y_struct, Geomet
-001746e0: 7279 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  ryNode, Node, No
-001746f0: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+001746e0: 7279 4e6f 6465 2c20 4e6f 6465 496e 7465  ryNode, NodeInte
+001746f0: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 00174700: 2222 220a 0a20 2052 6574 7269 6576 6520  """..  Retrieve 
 00174710: 6461 7461 206f 6620 6f74 6865 7220 656c  data of other el
 00174720: 656d 656e 7473 2069 6e20 7468 6520 636f  ements in the co
 00174730: 6e74 6578 7427 7320 6765 6f6d 6574 7279  ntext's geometry
 00174740: 0a0a 2020 2222 220a 0a20 2064 6174 615f  ..  """..  data_
 00174750: 7479 7065 3a20 7374 7220 3d20 2e2e 2e0a  type: str = ....
 00174760: 0a20 2064 6f6d 6169 6e3a 2073 7472 203d  .  domain: str =
@@ -95391,16 +95391,16 @@
 001749e0: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 001749f0: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 00174a00: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 00174a10: 2020 202e 2e2e 0a0a 636c 6173 7320 4765     .....class Ge
 00174a20: 6f6d 6574 7279 4e6f 6465 4669 656c 644f  ometryNodeFieldO
 00174a30: 6e44 6f6d 6169 6e28 6270 795f 7374 7275  nDomain(bpy_stru
 00174a40: 6374 2c20 4765 6f6d 6574 7279 4e6f 6465  ct, GeometryNode
-00174a50: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-00174a60: 726e 616c 293a 0a0a 2020 2222 220a 0a20  rnal):..  """.. 
+00174a50: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+00174a60: 4e6f 6465 293a 0a0a 2020 2222 220a 0a20  Node):..  """.. 
 00174a70: 2052 6574 7269 6576 6520 7661 6c75 6573   Retrieve values
 00174a80: 2066 726f 6d20 6120 6669 656c 6420 6f6e   from a field on
 00174a90: 2061 2064 6966 6665 7265 6e74 2064 6f6d   a different dom
 00174aa0: 6169 6e20 6265 7369 6465 7320 7468 6520  ain besides the 
 00174ab0: 646f 6d61 696e 2066 726f 6d20 7468 6520  domain from the 
 00174ac0: 636f 6e74 6578 740a 0a20 2022 2222 0a0a  context..  """..
 00174ad0: 2020 6461 7461 5f74 7970 653a 2073 7472    data_type: str
@@ -95447,16 +95447,16 @@
 00174d60: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 00174d70: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 00174d80: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 00174d90: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 00174da0: 6c61 7373 2047 656f 6d65 7472 794e 6f64  lass GeometryNod
 00174db0: 6546 696c 6c43 7572 7665 2862 7079 5f73  eFillCurve(bpy_s
 00174dc0: 7472 7563 742c 2047 656f 6d65 7472 794e  truct, GeometryN
-00174dd0: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-00174de0: 6e74 6572 6e61 6c29 3a0a 0a20 2022 2222  nternal):..  """
+00174dd0: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
+00174de0: 6c2c 204e 6f64 6529 3a0a 0a20 2022 2222  l, Node):..  """
 00174df0: 0a0a 2020 4765 6e65 7261 7465 2061 206d  ..  Generate a m
 00174e00: 6573 6820 6f6e 2074 6865 2058 5920 706c  esh on the XY pl
 00174e10: 616e 6520 7769 7468 2066 6163 6573 206f  ane with faces o
 00174e20: 6e20 7468 6520 696e 7369 6465 206f 6620  n the inside of 
 00174e30: 696e 7075 7420 6375 7276 6573 0a0a 2020  input curves..  
 00174e40: 2222 220a 0a20 206d 6f64 653a 2073 7472  """..  mode: str
 00174e50: 203d 202e 2e2e 0a0a 2020 4063 6c61 7373   = .....  @class
@@ -95498,16 +95498,16 @@
 00175090: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 001750a0: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 001750b0: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 001750c0: 2020 202e 2e2e 0a0a 636c 6173 7320 4765     .....class Ge
 001750d0: 6f6d 6574 7279 4e6f 6465 4669 6c6c 6574  ometryNodeFillet
 001750e0: 4375 7276 6528 6270 795f 7374 7275 6374  Curve(bpy_struct
 001750f0: 2c20 4765 6f6d 6574 7279 4e6f 6465 2c20  , GeometryNode, 
-00175100: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-00175110: 616c 293a 0a0a 2020 2222 220a 0a20 2052  al):..  """..  R
+00175100: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+00175110: 6465 293a 0a0a 2020 2222 220a 0a20 2052  de):..  """..  R
 00175120: 6f75 6e64 2063 6f72 6e65 7273 2062 7920  ound corners by 
 00175130: 6765 6e65 7261 7469 6e67 2063 6972 6375  generating circu
 00175140: 6c61 7220 6172 6373 206f 6e20 6561 6368  lar arcs on each
 00175150: 2063 6f6e 7472 6f6c 2070 6f69 6e74 0a0a   control point..
 00175160: 2020 2222 220a 0a20 206d 6f64 653a 2073    """..  mode: s
 00175170: 7472 203d 202e 2e2e 0a0a 2020 2222 220a  tr = .....  """.
 00175180: 0a20 2048 6f77 2074 6f20 6368 6f6f 7365  .  How to choose
@@ -95564,16 +95564,16 @@
 001754b0: 2073 7472 2c20 6465 6661 756c 743a 2074   str, default: t
 001754c0: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 001754d0: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 001754e0: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 001754f0: 7320 4765 6f6d 6574 7279 4e6f 6465 466c  s GeometryNodeFl
 00175500: 6970 4661 6365 7328 6270 795f 7374 7275  ipFaces(bpy_stru
 00175510: 6374 2c20 4765 6f6d 6574 7279 4e6f 6465  ct, GeometryNode
-00175520: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-00175530: 726e 616c 293a 0a0a 2020 2222 220a 0a20  rnal):..  """.. 
+00175520: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+00175530: 4e6f 6465 293a 0a0a 2020 2222 220a 0a20  Node):..  """.. 
 00175540: 2052 6576 6572 7365 2074 6865 206f 7264   Reverse the ord
 00175550: 6572 206f 6620 7468 6520 7665 7274 6963  er of the vertic
 00175560: 6573 2061 6e64 2065 6467 6573 206f 6620  es and edges of 
 00175570: 7365 6c65 6374 6564 2066 6163 6573 2c20  selected faces, 
 00175580: 666c 6970 7069 6e67 2074 6865 6972 206e  flipping their n
 00175590: 6f72 6d61 6c20 6469 7265 6374 696f 6e0a  ormal direction.
 001755a0: 0a20 2022 2222 0a0a 2020 4063 6c61 7373  .  """..  @class
@@ -95615,16 +95615,16 @@
 001757e0: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 001757f0: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 00175800: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 00175810: 2020 202e 2e2e 0a0a 636c 6173 7320 4765     .....class Ge
 00175820: 6f6d 6574 7279 4e6f 6465 4765 6f6d 6574  ometryNodeGeomet
 00175830: 7279 546f 496e 7374 616e 6365 2862 7079  ryToInstance(bpy
 00175840: 5f73 7472 7563 742c 2047 656f 6d65 7472  _struct, Geometr
-00175850: 794e 6f64 652c 204e 6f64 652c 204e 6f64  yNode, Node, Nod
-00175860: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2022  eInternal):..  "
+00175850: 794e 6f64 652c 204e 6f64 6549 6e74 6572  yNode, NodeInter
+00175860: 6e61 6c2c 204e 6f64 6529 3a0a 0a20 2022  nal, Node):..  "
 00175870: 2222 0a0a 2020 436f 6e76 6572 7420 6561  ""..  Convert ea
 00175880: 6368 2069 6e70 7574 2067 656f 6d65 7472  ch input geometr
 00175890: 7920 696e 746f 2061 6e20 696e 7374 616e  y into an instan
 001758a0: 6365 2c20 7768 6963 6820 6361 6e20 6265  ce, which can be
 001758b0: 206d 7563 6820 6661 7374 6572 2074 6861   much faster tha
 001758c0: 6e20 7468 6520 4a6f 696e 2047 656f 6d65  n the Join Geome
 001758d0: 7472 7920 6e6f 6465 2077 6865 6e20 7468  try node when th
@@ -95668,15 +95668,15 @@
 00175b30: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 00175b40: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 00175b50: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 00175b60: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 00175b70: 2047 656f 6d65 7472 794e 6f64 6547 726f   GeometryNodeGro
 00175b80: 7570 2862 7079 5f73 7472 7563 742c 2047  up(bpy_struct, G
 00175b90: 656f 6d65 7472 794e 6f64 652c 204e 6f64  eometryNode, Nod
-00175ba0: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+00175ba0: 6549 6e74 6572 6e61 6c2c 204e 6f64 6529  eInternal, Node)
 00175bb0: 3a0a 0a20 206e 6f64 655f 7472 6565 3a20  :..  node_tree: 
 00175bc0: 4e6f 6465 5472 6565 203d 202e 2e2e 0a0a  NodeTree = .....
 00175bd0: 2020 4063 6c61 7373 6d65 7468 6f64 0a0a    @classmethod..
 00175be0: 2020 6465 6620 6973 5f72 6567 6973 7465    def is_registe
 00175bf0: 7265 645f 6e6f 6465 5f74 7970 6528 636c  red_node_type(cl
 00175c00: 7329 202d 3e20 626f 6f6c 3a0a 0a20 2020  s) -> bool:..   
 00175c10: 2022 2222 0a0a 2020 2020 5472 7565 2069   """..    True i
@@ -95713,16 +95713,16 @@
 00175e00: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 00175e10: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 00175e20: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 00175e30: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 00175e40: 636c 6173 7320 4765 6f6d 6574 7279 4e6f  class GeometryNo
 00175e50: 6465 496d 6167 6549 6e66 6f28 6270 795f  deImageInfo(bpy_
 00175e60: 7374 7275 6374 2c20 4765 6f6d 6574 7279  struct, Geometry
-00175e70: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-00175e80: 496e 7465 726e 616c 293a 0a0a 2020 2222  Internal):..  ""
+00175e70: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
+00175e80: 616c 2c20 4e6f 6465 293a 0a0a 2020 2222  al, Node):..  ""
 00175e90: 220a 0a20 2052 6574 7269 6576 6520 696e  "..  Retrieve in
 00175ea0: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
 00175eb0: 616e 2069 6d61 6765 0a0a 2020 2222 220a  an image..  """.
 00175ec0: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
 00175ed0: 0a20 2064 6566 2069 735f 7265 6769 7374  .  def is_regist
 00175ee0: 6572 6564 5f6e 6f64 655f 7479 7065 2863  ered_node_type(c
 00175ef0: 6c73 2920 2d3e 2062 6f6f 6c3a 0a0a 2020  ls) -> bool:..  
@@ -95760,16 +95760,16 @@
 001760f0: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 00176100: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 00176110: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 00176120: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 00176130: 0a63 6c61 7373 2047 656f 6d65 7472 794e  .class GeometryN
 00176140: 6f64 6549 6d61 6765 5465 7874 7572 6528  odeImageTexture(
 00176150: 6270 795f 7374 7275 6374 2c20 4765 6f6d  bpy_struct, Geom
-00176160: 6574 7279 4e6f 6465 2c20 4e6f 6465 2c20  etryNode, Node, 
-00176170: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+00176160: 6574 7279 4e6f 6465 2c20 4e6f 6465 496e  etryNode, NodeIn
+00176170: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 00176180: 2020 2222 220a 0a20 2053 616d 706c 6520    """..  Sample 
 00176190: 7661 6c75 6573 2066 726f 6d20 616e 2069  values from an i
 001761a0: 6d61 6765 2074 6578 7475 7265 0a0a 2020  mage texture..  
 001761b0: 2222 220a 0a20 2065 7874 656e 7369 6f6e  """..  extension
 001761c0: 3a20 7374 7220 3d20 2e2e 2e0a 0a20 2022  : str = .....  "
 001761d0: 2222 0a0a 2020 486f 7720 7468 6520 696d  ""..  How the im
 001761e0: 6167 6520 6973 2065 7874 7261 706f 6c61  age is extrapola
@@ -95850,16 +95850,16 @@
 00176690: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 001766a0: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 001766b0: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 001766c0: 4765 6f6d 6574 7279 4e6f 6465 496e 7075  GeometryNodeInpu
 001766d0: 7443 7572 7665 4861 6e64 6c65 506f 7369  tCurveHandlePosi
 001766e0: 7469 6f6e 7328 6270 795f 7374 7275 6374  tions(bpy_struct
 001766f0: 2c20 4765 6f6d 6574 7279 4e6f 6465 2c20  , GeometryNode, 
-00176700: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-00176710: 616c 293a 0a0a 2020 2222 220a 0a20 2052  al):..  """..  R
+00176700: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+00176710: 6465 293a 0a0a 2020 2222 220a 0a20 2052  de):..  """..  R
 00176720: 6574 7269 6576 6520 7468 6520 706f 7369  etrieve the posi
 00176730: 7469 6f6e 206f 6620 6561 6368 2042 c3a9  tion of each B..
 00176740: 7a69 6572 2063 6f6e 7472 6f6c 2070 6f69  zier control poi
 00176750: 6e74 2773 2068 616e 646c 6573 0a0a 2020  nt's handles..  
 00176760: 2222 220a 0a20 2040 636c 6173 736d 6574  """..  @classmet
 00176770: 686f 640a 0a20 2064 6566 2069 735f 7265  hod..  def is_re
 00176780: 6769 7374 6572 6564 5f6e 6f64 655f 7479  gistered_node_ty
@@ -95899,16 +95899,16 @@
 001769a0: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 001769b0: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 001769c0: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 001769d0: 2e2e 2e0a 0a63 6c61 7373 2047 656f 6d65  .....class Geome
 001769e0: 7472 794e 6f64 6549 6e70 7574 4375 7276  tryNodeInputCurv
 001769f0: 6554 696c 7428 6270 795f 7374 7275 6374  eTilt(bpy_struct
 00176a00: 2c20 4765 6f6d 6574 7279 4e6f 6465 2c20  , GeometryNode, 
-00176a10: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-00176a20: 616c 293a 0a0a 2020 2222 220a 0a20 2052  al):..  """..  R
+00176a10: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+00176a20: 6465 293a 0a0a 2020 2222 220a 0a20 2052  de):..  """..  R
 00176a30: 6574 7269 6576 6520 7468 6520 616e 676c  etrieve the angl
 00176a40: 6520 6174 2065 6163 6820 636f 6e74 726f  e at each contro
 00176a50: 6c20 706f 696e 7420 7573 6564 2074 6f20  l point used to 
 00176a60: 7477 6973 7420 7468 6520 6375 7276 6527  twist the curve'
 00176a70: 7320 6e6f 726d 616c 2061 726f 756e 6420  s normal around 
 00176a80: 6974 7320 7461 6e67 656e 740a 0a20 2022  its tangent..  "
 00176a90: 2222 0a0a 2020 4063 6c61 7373 6d65 7468  ""..  @classmeth
@@ -95949,16 +95949,16 @@
 00176cc0: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 00176cd0: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 00176ce0: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 00176cf0: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 00176d00: 2e2e 0a0a 636c 6173 7320 4765 6f6d 6574  ....class Geomet
 00176d10: 7279 4e6f 6465 496e 7075 7449 4428 6270  ryNodeInputID(bp
 00176d20: 795f 7374 7275 6374 2c20 4765 6f6d 6574  y_struct, Geomet
-00176d30: 7279 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  ryNode, Node, No
-00176d40: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+00176d30: 7279 4e6f 6465 2c20 4e6f 6465 496e 7465  ryNode, NodeInte
+00176d40: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 00176d50: 2222 220a 0a20 2052 6574 7269 6576 6520  """..  Retrieve 
 00176d60: 6120 7374 6162 6c65 2072 616e 646f 6d20  a stable random 
 00176d70: 6964 656e 7469 6669 6572 2076 616c 7565  identifier value
 00176d80: 2066 726f 6d20 7468 6520 2269 6422 2061   from the "id" a
 00176d90: 7474 7269 6275 7465 206f 6e20 7468 6520  ttribute on the 
 00176da0: 706f 696e 7420 646f 6d61 696e 2c20 6f72  point domain, or
 00176db0: 2074 6865 2069 6e64 6578 2069 6620 7468   the index if th
@@ -96002,16 +96002,16 @@
 00177010: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 00177020: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 00177030: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 00177040: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 00177050: 2e0a 0a63 6c61 7373 2047 656f 6d65 7472  ...class Geometr
 00177060: 794e 6f64 6549 6e70 7574 496d 6167 6528  yNodeInputImage(
 00177070: 6270 795f 7374 7275 6374 2c20 4765 6f6d  bpy_struct, Geom
-00177080: 6574 7279 4e6f 6465 2c20 4e6f 6465 2c20  etryNode, Node, 
-00177090: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+00177080: 6574 7279 4e6f 6465 2c20 4e6f 6465 496e  etryNode, NodeIn
+00177090: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 001770a0: 2020 2222 220a 0a20 2049 6e70 7574 2069    """..  Input i
 001770b0: 6d61 6765 0a0a 2020 2222 220a 0a20 2069  mage..  """..  i
 001770c0: 6d61 6765 3a20 496d 6167 6520 3d20 2e2e  mage: Image = ..
 001770d0: 2e0a 0a20 2040 636c 6173 736d 6574 686f  ...  @classmetho
 001770e0: 640a 0a20 2064 6566 2069 735f 7265 6769  d..  def is_regi
 001770f0: 7374 6572 6564 5f6e 6f64 655f 7479 7065  stered_node_type
 00177100: 2863 6c73 2920 2d3e 2062 6f6f 6c3a 0a0a  (cls) -> bool:..
@@ -96049,16 +96049,16 @@
 00177300: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 00177310: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 00177320: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 00177330: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 00177340: 2e0a 0a63 6c61 7373 2047 656f 6d65 7472  ...class Geometr
 00177350: 794e 6f64 6549 6e70 7574 496e 6465 7828  yNodeInputIndex(
 00177360: 6270 795f 7374 7275 6374 2c20 4765 6f6d  bpy_struct, Geom
-00177370: 6574 7279 4e6f 6465 2c20 4e6f 6465 2c20  etryNode, Node, 
-00177380: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+00177370: 6574 7279 4e6f 6465 2c20 4e6f 6465 496e  etryNode, NodeIn
+00177380: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 00177390: 2020 2222 220a 0a20 2052 6574 7269 6576    """..  Retriev
 001773a0: 6520 616e 2069 6e74 6567 6572 2076 616c  e an integer val
 001773b0: 7565 2069 6e64 6963 6174 696e 6720 7468  ue indicating th
 001773c0: 6520 706f 7369 7469 6f6e 206f 6620 6561  e position of ea
 001773d0: 6368 2065 6c65 6d65 6e74 2069 6e20 7468  ch element in th
 001773e0: 6520 6c69 7374 2c20 7374 6172 7469 6e67  e list, starting
 001773f0: 2061 7420 7a65 726f 0a0a 2020 2222 220a   at zero..  """.
@@ -96101,16 +96101,16 @@
 00177640: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 00177650: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 00177660: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 00177670: 0a63 6c61 7373 2047 656f 6d65 7472 794e  .class GeometryN
 00177680: 6f64 6549 6e70 7574 496e 7374 616e 6365  odeInputInstance
 00177690: 526f 7461 7469 6f6e 2862 7079 5f73 7472  Rotation(bpy_str
 001776a0: 7563 742c 2047 656f 6d65 7472 794e 6f64  uct, GeometryNod
-001776b0: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-001776c0: 6572 6e61 6c29 3a0a 0a20 2022 2222 0a0a  ernal):..  """..
+001776b0: 652c 204e 6f64 6549 6e74 6572 6e61 6c2c  e, NodeInternal,
+001776c0: 204e 6f64 6529 3a0a 0a20 2022 2222 0a0a   Node):..  """..
 001776d0: 2020 5265 7472 6965 7665 2074 6865 2072    Retrieve the r
 001776e0: 6f74 6174 696f 6e20 6f66 2065 6163 6820  otation of each 
 001776f0: 696e 7374 616e 6365 2069 6e20 7468 6520  instance in the 
 00177700: 6765 6f6d 6574 7279 0a0a 2020 2222 220a  geometry..  """.
 00177710: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
 00177720: 0a20 2064 6566 2069 735f 7265 6769 7374  .  def is_regist
 00177730: 6572 6564 5f6e 6f64 655f 7479 7065 2863  ered_node_type(c
@@ -96150,16 +96150,16 @@
 00177950: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 00177960: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 00177970: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 00177980: 0a63 6c61 7373 2047 656f 6d65 7472 794e  .class GeometryN
 00177990: 6f64 6549 6e70 7574 496e 7374 616e 6365  odeInputInstance
 001779a0: 5363 616c 6528 6270 795f 7374 7275 6374  Scale(bpy_struct
 001779b0: 2c20 4765 6f6d 6574 7279 4e6f 6465 2c20  , GeometryNode, 
-001779c0: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-001779d0: 616c 293a 0a0a 2020 2222 220a 0a20 2052  al):..  """..  R
+001779c0: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+001779d0: 6465 293a 0a0a 2020 2222 220a 0a20 2052  de):..  """..  R
 001779e0: 6574 7269 6576 6520 7468 6520 7363 616c  etrieve the scal
 001779f0: 6520 6f66 2065 6163 6820 696e 7374 616e  e of each instan
 00177a00: 6365 2069 6e20 7468 6520 6765 6f6d 6574  ce in the geomet
 00177a10: 7279 0a0a 2020 2222 220a 0a20 2040 636c  ry..  """..  @cl
 00177a20: 6173 736d 6574 686f 640a 0a20 2064 6566  assmethod..  def
 00177a30: 2069 735f 7265 6769 7374 6572 6564 5f6e   is_registered_n
 00177a40: 6f64 655f 7479 7065 2863 6c73 2920 2d3e  ode_type(cls) ->
@@ -96198,16 +96198,16 @@
 00177c50: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 00177c60: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 00177c70: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 00177c80: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 00177c90: 2047 656f 6d65 7472 794e 6f64 6549 6e70   GeometryNodeInp
 00177ca0: 7574 4d61 7465 7269 616c 2862 7079 5f73  utMaterial(bpy_s
 00177cb0: 7472 7563 742c 2047 656f 6d65 7472 794e  truct, GeometryN
-00177cc0: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-00177cd0: 6e74 6572 6e61 6c29 3a0a 0a20 2022 2222  nternal):..  """
+00177cc0: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
+00177cd0: 6c2c 204e 6f64 6529 3a0a 0a20 2022 2222  l, Node):..  """
 00177ce0: 0a0a 2020 4f75 7470 7574 2061 2073 696e  ..  Output a sin
 00177cf0: 676c 6520 6d61 7465 7269 616c 0a0a 2020  gle material..  
 00177d00: 2222 220a 0a20 206d 6174 6572 6961 6c3a  """..  material:
 00177d10: 204d 6174 6572 6961 6c20 3d20 2e2e 2e0a   Material = ....
 00177d20: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
 00177d30: 0a20 2064 6566 2069 735f 7265 6769 7374  .  def is_regist
 00177d40: 6572 6564 5f6e 6f64 655f 7479 7065 2863  ered_node_type(c
@@ -96247,16 +96247,16 @@
 00177f60: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 00177f70: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 00177f80: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 00177f90: 0a63 6c61 7373 2047 656f 6d65 7472 794e  .class GeometryN
 00177fa0: 6f64 6549 6e70 7574 4d61 7465 7269 616c  odeInputMaterial
 00177fb0: 496e 6465 7828 6270 795f 7374 7275 6374  Index(bpy_struct
 00177fc0: 2c20 4765 6f6d 6574 7279 4e6f 6465 2c20  , GeometryNode, 
-00177fd0: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-00177fe0: 616c 293a 0a0a 2020 2222 220a 0a20 2052  al):..  """..  R
+00177fd0: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+00177fe0: 6465 293a 0a0a 2020 2222 220a 0a20 2052  de):..  """..  R
 00177ff0: 6574 7269 6576 6520 7468 6520 696e 6465  etrieve the inde
 00178000: 7820 6f66 2074 6865 206d 6174 6572 6961  x of the materia
 00178010: 6c20 7573 6564 2066 6f72 2065 6163 6820  l used for each 
 00178020: 656c 656d 656e 7420 696e 2074 6865 2067  element in the g
 00178030: 656f 6d65 7472 7927 7320 6c69 7374 206f  eometry's list o
 00178040: 6620 6d61 7465 7269 616c 730a 0a20 2022  f materials..  "
 00178050: 2222 0a0a 2020 4063 6c61 7373 6d65 7468  ""..  @classmeth
@@ -96298,16 +96298,16 @@
 00178290: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 001782a0: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 001782b0: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 001782c0: 2e2e 0a0a 636c 6173 7320 4765 6f6d 6574  ....class Geomet
 001782d0: 7279 4e6f 6465 496e 7075 744d 6573 6845  ryNodeInputMeshE
 001782e0: 6467 6541 6e67 6c65 2862 7079 5f73 7472  dgeAngle(bpy_str
 001782f0: 7563 742c 2047 656f 6d65 7472 794e 6f64  uct, GeometryNod
-00178300: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-00178310: 6572 6e61 6c29 3a0a 0a20 2022 2222 0a0a  ernal):..  """..
+00178300: 652c 204e 6f64 6549 6e74 6572 6e61 6c2c  e, NodeInternal,
+00178310: 204e 6f64 6529 3a0a 0a20 2022 2222 0a0a   Node):..  """..
 00178320: 2020 4361 6c63 756c 6174 6520 7468 6520    Calculate the 
 00178330: 7375 7266 6163 6520 6172 6561 206f 6620  surface area of 
 00178340: 6561 6368 2066 6163 6520 696e 2061 206d  each face in a m
 00178350: 6573 680a 0a20 2022 2222 0a0a 2020 4063  esh..  """..  @c
 00178360: 6c61 7373 6d65 7468 6f64 0a0a 2020 6465  lassmethod..  de
 00178370: 6620 6973 5f72 6567 6973 7465 7265 645f  f is_registered_
 00178380: 6e6f 6465 5f74 7970 6528 636c 7329 202d  node_type(cls) -
@@ -96347,16 +96347,16 @@
 001785a0: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 001785b0: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 001785c0: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 001785d0: 7320 4765 6f6d 6574 7279 4e6f 6465 496e  s GeometryNodeIn
 001785e0: 7075 744d 6573 6845 6467 654e 6569 6768  putMeshEdgeNeigh
 001785f0: 626f 7273 2862 7079 5f73 7472 7563 742c  bors(bpy_struct,
 00178600: 2047 656f 6d65 7472 794e 6f64 652c 204e   GeometryNode, N
-00178610: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-00178620: 6c29 3a0a 0a20 2022 2222 0a0a 2020 5265  l):..  """..  Re
+00178610: 6f64 6549 6e74 6572 6e61 6c2c 204e 6f64  odeInternal, Nod
+00178620: 6529 3a0a 0a20 2022 2222 0a0a 2020 5265  e):..  """..  Re
 00178630: 7472 6965 7665 2074 6865 206e 756d 6265  trieve the numbe
 00178640: 7220 6f66 2066 6163 6573 2074 6861 7420  r of faces that 
 00178650: 7573 6520 6561 6368 2065 6467 6520 6173  use each edge as
 00178660: 206f 6e65 206f 6620 7468 6569 7220 7369   one of their si
 00178670: 6465 730a 0a20 2022 2222 0a0a 2020 4063  des..  """..  @c
 00178680: 6c61 7373 6d65 7468 6f64 0a0a 2020 6465  lassmethod..  de
 00178690: 6620 6973 5f72 6567 6973 7465 7265 645f  f is_registered_
@@ -96397,15 +96397,15 @@
 001788c0: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 001788d0: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 001788e0: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 001788f0: 7320 4765 6f6d 6574 7279 4e6f 6465 496e  s GeometryNodeIn
 00178900: 7075 744d 6573 6845 6467 6556 6572 7469  putMeshEdgeVerti
 00178910: 6365 7328 6270 795f 7374 7275 6374 2c20  ces(bpy_struct, 
 00178920: 4765 6f6d 6574 7279 4e6f 6465 2c20 4e6f  GeometryNode, No
-00178930: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+00178930: 6465 496e 7465 726e 616c 2c20 4e6f 6465  deInternal, Node
 00178940: 293a 0a0a 2020 2222 220a 0a20 2052 6574  ):..  """..  Ret
 00178950: 7269 6576 6520 746f 706f 6c6f 6779 2069  rieve topology i
 00178960: 6e66 6f72 6d61 7469 6f6e 2072 656c 6174  nformation relat
 00178970: 696e 6720 746f 2065 6163 6820 6564 6765  ing to each edge
 00178980: 206f 6620 6120 6d65 7368 0a0a 2020 2222   of a mesh..  ""
 00178990: 220a 0a20 2040 636c 6173 736d 6574 686f  "..  @classmetho
 001789a0: 640a 0a20 2064 6566 2069 735f 7265 6769  d..  def is_regi
@@ -96446,16 +96446,16 @@
 00178bd0: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 00178be0: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 00178bf0: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 00178c00: 2e0a 0a63 6c61 7373 2047 656f 6d65 7472  ...class Geometr
 00178c10: 794e 6f64 6549 6e70 7574 4d65 7368 4661  yNodeInputMeshFa
 00178c20: 6365 4172 6561 2862 7079 5f73 7472 7563  ceArea(bpy_struc
 00178c30: 742c 2047 656f 6d65 7472 794e 6f64 652c  t, GeometryNode,
-00178c40: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-00178c50: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+00178c40: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+00178c50: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 00178c60: 4361 6c63 756c 6174 6520 7468 6520 7375  Calculate the su
 00178c70: 7266 6163 6520 6172 6561 206f 6620 6120  rface area of a 
 00178c80: 6d65 7368 2773 2066 6163 6573 0a0a 2020  mesh's faces..  
 00178c90: 2222 220a 0a20 2040 636c 6173 736d 6574  """..  @classmet
 00178ca0: 686f 640a 0a20 2064 6566 2069 735f 7265  hod..  def is_re
 00178cb0: 6769 7374 6572 6564 5f6e 6f64 655f 7479  gistered_node_ty
 00178cc0: 7065 2863 6c73 2920 2d3e 2062 6f6f 6c3a  pe(cls) -> bool:
@@ -96494,16 +96494,16 @@
 00178ed0: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 00178ee0: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 00178ef0: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 00178f00: 2e2e 2e0a 0a63 6c61 7373 2047 656f 6d65  .....class Geome
 00178f10: 7472 794e 6f64 6549 6e70 7574 4d65 7368  tryNodeInputMesh
 00178f20: 4661 6365 4973 506c 616e 6172 2862 7079  FaceIsPlanar(bpy
 00178f30: 5f73 7472 7563 742c 2047 656f 6d65 7472  _struct, Geometr
-00178f40: 794e 6f64 652c 204e 6f64 652c 204e 6f64  yNode, Node, Nod
-00178f50: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2022  eInternal):..  "
+00178f40: 794e 6f64 652c 204e 6f64 6549 6e74 6572  yNode, NodeInter
+00178f50: 6e61 6c2c 204e 6f64 6529 3a0a 0a20 2022  nal, Node):..  "
 00178f60: 2222 0a0a 2020 5265 7472 6965 7665 2077  ""..  Retrieve w
 00178f70: 6865 7468 6572 2061 6c6c 2074 7269 616e  hether all trian
 00178f80: 676c 6573 2069 6e20 6120 6661 6365 2061  gles in a face a
 00178f90: 7265 206f 6e20 7468 6520 7361 6d65 2070  re on the same p
 00178fa0: 6c61 6e65 2c20 692e 652e 2077 6865 7468  lane, i.e. wheth
 00178fb0: 6572 2074 6865 7920 6861 7665 2074 6865  er they have the
 00178fc0: 2073 616d 6520 6e6f 726d 616c 0a0a 2020   same normal..  
@@ -96546,16 +96546,16 @@
 00179210: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 00179220: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 00179230: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 00179240: 2e2e 2e0a 0a63 6c61 7373 2047 656f 6d65  .....class Geome
 00179250: 7472 794e 6f64 6549 6e70 7574 4d65 7368  tryNodeInputMesh
 00179260: 4661 6365 4e65 6967 6862 6f72 7328 6270  FaceNeighbors(bp
 00179270: 795f 7374 7275 6374 2c20 4765 6f6d 6574  y_struct, Geomet
-00179280: 7279 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  ryNode, Node, No
-00179290: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+00179280: 7279 4e6f 6465 2c20 4e6f 6465 496e 7465  ryNode, NodeInte
+00179290: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 001792a0: 2222 220a 0a20 2052 6574 7269 6576 6520  """..  Retrieve 
 001792b0: 746f 706f 6c6f 6779 2069 6e66 6f72 6d61  topology informa
 001792c0: 7469 6f6e 2072 656c 6174 696e 6720 746f  tion relating to
 001792d0: 2065 6163 6820 6661 6365 206f 6620 6120   each face of a 
 001792e0: 6d65 7368 0a0a 2020 2222 220a 0a20 2040  mesh..  """..  @
 001792f0: 636c 6173 736d 6574 686f 640a 0a20 2064  classmethod..  d
 00179300: 6566 2069 735f 7265 6769 7374 6572 6564  ef is_registered
@@ -96595,16 +96595,16 @@
 00179520: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 00179530: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 00179540: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 00179550: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 00179560: 7373 2047 656f 6d65 7472 794e 6f64 6549  ss GeometryNodeI
 00179570: 6e70 7574 4d65 7368 4973 6c61 6e64 2862  nputMeshIsland(b
 00179580: 7079 5f73 7472 7563 742c 2047 656f 6d65  py_struct, Geome
-00179590: 7472 794e 6f64 652c 204e 6f64 652c 204e  tryNode, Node, N
-001795a0: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+00179590: 7472 794e 6f64 652c 204e 6f64 6549 6e74  tryNode, NodeInt
+001795a0: 6572 6e61 6c2c 204e 6f64 6529 3a0a 0a20  ernal, Node):.. 
 001795b0: 2022 2222 0a0a 2020 5265 7472 6965 7665   """..  Retrieve
 001795c0: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
 001795d0: 7574 2073 6570 6172 6174 6520 636f 6e6e  ut separate conn
 001795e0: 6563 7465 6420 7265 6769 6f6e 7320 696e  ected regions in
 001795f0: 2061 206d 6573 680a 0a20 2022 2222 0a0a   a mesh..  """..
 00179600: 2020 4063 6c61 7373 6d65 7468 6f64 0a0a    @classmethod..
 00179610: 2020 6465 6620 6973 5f72 6567 6973 7465    def is_registe
@@ -96645,16 +96645,16 @@
 00179840: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 00179850: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 00179860: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 00179870: 636c 6173 7320 4765 6f6d 6574 7279 4e6f  class GeometryNo
 00179880: 6465 496e 7075 744d 6573 6856 6572 7465  deInputMeshVerte
 00179890: 784e 6569 6768 626f 7273 2862 7079 5f73  xNeighbors(bpy_s
 001798a0: 7472 7563 742c 2047 656f 6d65 7472 794e  truct, GeometryN
-001798b0: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-001798c0: 6e74 6572 6e61 6c29 3a0a 0a20 2022 2222  nternal):..  """
+001798b0: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
+001798c0: 6c2c 204e 6f64 6529 3a0a 0a20 2022 2222  l, Node):..  """
 001798d0: 0a0a 2020 5265 7472 6965 7665 2074 6f70  ..  Retrieve top
 001798e0: 6f6c 6f67 7920 696e 666f 726d 6174 696f  ology informatio
 001798f0: 6e20 7265 6c61 7469 6e67 2074 6f20 6561  n relating to ea
 00179900: 6368 2076 6572 7465 7820 6f66 2061 206d  ch vertex of a m
 00179910: 6573 680a 0a20 2022 2222 0a0a 2020 4063  esh..  """..  @c
 00179920: 6c61 7373 6d65 7468 6f64 0a0a 2020 6465  lassmethod..  de
 00179930: 6620 6973 5f72 6567 6973 7465 7265 645f  f is_registered_
@@ -96695,15 +96695,15 @@
 00179b60: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 00179b70: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 00179b80: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 00179b90: 7320 4765 6f6d 6574 7279 4e6f 6465 496e  s GeometryNodeIn
 00179ba0: 7075 744e 616d 6564 4174 7472 6962 7574  putNamedAttribut
 00179bb0: 6528 6270 795f 7374 7275 6374 2c20 4765  e(bpy_struct, Ge
 00179bc0: 6f6d 6574 7279 4e6f 6465 2c20 4e6f 6465  ometryNode, Node
-00179bd0: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+00179bd0: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 00179be0: 0a0a 2020 2222 220a 0a20 2052 6574 7269  ..  """..  Retri
 00179bf0: 6576 6520 7468 6520 6461 7461 206f 6620  eve the data of 
 00179c00: 6120 7370 6563 6966 6965 6420 6174 7472  a specified attr
 00179c10: 6962 7574 650a 0a20 2022 2222 0a0a 2020  ibute..  """..  
 00179c20: 6461 7461 5f74 7970 653a 2073 7472 203d  data_type: str =
 00179c30: 202e 2e2e 0a0a 2020 2222 220a 0a20 2054   .....  """..  T
 00179c40: 6865 2064 6174 6120 7479 7065 2075 7365  he data type use
@@ -96748,16 +96748,16 @@
 00179eb0: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 00179ec0: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 00179ed0: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 00179ee0: 2020 2e2e 2e0a 0a63 6c61 7373 2047 656f    .....class Geo
 00179ef0: 6d65 7472 794e 6f64 6549 6e70 7574 4e6f  metryNodeInputNo
 00179f00: 726d 616c 2862 7079 5f73 7472 7563 742c  rmal(bpy_struct,
 00179f10: 2047 656f 6d65 7472 794e 6f64 652c 204e   GeometryNode, N
-00179f20: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-00179f30: 6c29 3a0a 0a20 2022 2222 0a0a 2020 5265  l):..  """..  Re
+00179f20: 6f64 6549 6e74 6572 6e61 6c2c 204e 6f64  odeInternal, Nod
+00179f30: 6529 3a0a 0a20 2022 2222 0a0a 2020 5265  e):..  """..  Re
 00179f40: 7472 6965 7665 2061 2075 6e69 7420 6c65  trieve a unit le
 00179f50: 6e67 7468 2076 6563 746f 7220 696e 6469  ngth vector indi
 00179f60: 6361 7469 6e67 2074 6865 2064 6972 6563  cating the direc
 00179f70: 7469 6f6e 2070 6f69 6e74 696e 6720 6177  tion pointing aw
 00179f80: 6179 2066 726f 6d20 7468 6520 6765 6f6d  ay from the geom
 00179f90: 6574 7279 2061 7420 6561 6368 2065 6c65  etry at each ele
 00179fa0: 6d65 6e74 0a0a 2020 2222 220a 0a20 2040  ment..  """..  @
@@ -96799,16 +96799,16 @@
 0017a1e0: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 0017a1f0: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 0017a200: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 0017a210: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 0017a220: 7373 2047 656f 6d65 7472 794e 6f64 6549  ss GeometryNodeI
 0017a230: 6e70 7574 506f 7369 7469 6f6e 2862 7079  nputPosition(bpy
 0017a240: 5f73 7472 7563 742c 2047 656f 6d65 7472  _struct, Geometr
-0017a250: 794e 6f64 652c 204e 6f64 652c 204e 6f64  yNode, Node, Nod
-0017a260: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2022  eInternal):..  "
+0017a250: 794e 6f64 652c 204e 6f64 6549 6e74 6572  yNode, NodeInter
+0017a260: 6e61 6c2c 204e 6f64 6529 3a0a 0a20 2022  nal, Node):..  "
 0017a270: 2222 0a0a 2020 5265 7472 6965 7665 2061  ""..  Retrieve a
 0017a280: 2076 6563 746f 7220 696e 6469 6361 7469   vector indicati
 0017a290: 6e67 2074 6865 206c 6f63 6174 696f 6e20  ng the location 
 0017a2a0: 6f66 2065 6163 6820 656c 656d 656e 740a  of each element.
 0017a2b0: 0a20 2022 2222 0a0a 2020 4063 6c61 7373  .  """..  @class
 0017a2c0: 6d65 7468 6f64 0a0a 2020 6465 6620 6973  method..  def is
 0017a2d0: 5f72 6567 6973 7465 7265 645f 6e6f 6465  _registered_node
@@ -96848,16 +96848,16 @@
 0017a4f0: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 0017a500: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 0017a510: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 0017a520: 2020 202e 2e2e 0a0a 636c 6173 7320 4765     .....class Ge
 0017a530: 6f6d 6574 7279 4e6f 6465 496e 7075 7452  ometryNodeInputR
 0017a540: 6164 6975 7328 6270 795f 7374 7275 6374  adius(bpy_struct
 0017a550: 2c20 4765 6f6d 6574 7279 4e6f 6465 2c20  , GeometryNode, 
-0017a560: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-0017a570: 616c 293a 0a0a 2020 2222 220a 0a20 2052  al):..  """..  R
+0017a560: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+0017a570: 6465 293a 0a0a 2020 2222 220a 0a20 2052  de):..  """..  R
 0017a580: 6574 7269 6576 6520 7468 6520 7261 6469  etrieve the radi
 0017a590: 7573 2061 7420 6561 6368 2070 6f69 6e74  us at each point
 0017a5a0: 206f 6e20 6375 7276 6520 6f72 2070 6f69   on curve or poi
 0017a5b0: 6e74 2063 6c6f 7564 2067 656f 6d65 7472  nt cloud geometr
 0017a5c0: 790a 0a20 2022 2222 0a0a 2020 4063 6c61  y..  """..  @cla
 0017a5d0: 7373 6d65 7468 6f64 0a0a 2020 6465 6620  ssmethod..  def 
 0017a5e0: 6973 5f72 6567 6973 7465 7265 645f 6e6f  is_registered_no
@@ -96897,16 +96897,16 @@
 0017a800: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 0017a810: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 0017a820: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 0017a830: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 0017a840: 4765 6f6d 6574 7279 4e6f 6465 496e 7075  GeometryNodeInpu
 0017a850: 7453 6365 6e65 5469 6d65 2862 7079 5f73  tSceneTime(bpy_s
 0017a860: 7472 7563 742c 2047 656f 6d65 7472 794e  truct, GeometryN
-0017a870: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-0017a880: 6e74 6572 6e61 6c29 3a0a 0a20 2022 2222  nternal):..  """
+0017a870: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
+0017a880: 6c2c 204e 6f64 6529 3a0a 0a20 2022 2222  l, Node):..  """
 0017a890: 0a0a 2020 5265 7472 6965 7665 2074 6865  ..  Retrieve the
 0017a8a0: 2063 7572 7265 6e74 2074 696d 6520 696e   current time in
 0017a8b0: 2074 6865 2073 6365 6e65 2773 2061 6e69   the scene's ani
 0017a8c0: 6d61 7469 6f6e 2069 6e20 756e 6974 7320  mation in units 
 0017a8d0: 6f66 2073 6563 6f6e 6473 206f 7220 6672  of seconds or fr
 0017a8e0: 616d 6573 0a0a 2020 2222 220a 0a20 2040  ames..  """..  @
 0017a8f0: 636c 6173 736d 6574 686f 640a 0a20 2064  classmethod..  d
@@ -96947,16 +96947,16 @@
 0017ab20: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 0017ab30: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 0017ab40: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 0017ab50: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 0017ab60: 7373 2047 656f 6d65 7472 794e 6f64 6549  ss GeometryNodeI
 0017ab70: 6e70 7574 5368 6164 6553 6d6f 6f74 6828  nputShadeSmooth(
 0017ab80: 6270 795f 7374 7275 6374 2c20 4765 6f6d  bpy_struct, Geom
-0017ab90: 6574 7279 4e6f 6465 2c20 4e6f 6465 2c20  etryNode, Node, 
-0017aba0: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+0017ab90: 6574 7279 4e6f 6465 2c20 4e6f 6465 496e  etryNode, NodeIn
+0017aba0: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 0017abb0: 2020 2222 220a 0a20 2052 6574 7269 6576    """..  Retriev
 0017abc0: 6520 7768 6574 6865 7220 6561 6368 2066  e whether each f
 0017abd0: 6163 6520 6973 206d 6172 6b65 6420 666f  ace is marked fo
 0017abe0: 7220 736d 6f6f 7468 2073 6861 6469 6e67  r smooth shading
 0017abf0: 0a0a 2020 2222 220a 0a20 2040 636c 6173  ..  """..  @clas
 0017ac00: 736d 6574 686f 640a 0a20 2064 6566 2069  smethod..  def i
 0017ac10: 735f 7265 6769 7374 6572 6564 5f6e 6f64  s_registered_nod
@@ -96997,15 +96997,15 @@
 0017ae40: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 0017ae50: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 0017ae60: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2047      .....class G
 0017ae70: 656f 6d65 7472 794e 6f64 6549 6e70 7574  eometryNodeInput
 0017ae80: 5368 6f72 7465 7374 4564 6765 5061 7468  ShortestEdgePath
 0017ae90: 7328 6270 795f 7374 7275 6374 2c20 4765  s(bpy_struct, Ge
 0017aea0: 6f6d 6574 7279 4e6f 6465 2c20 4e6f 6465  ometryNode, Node
-0017aeb0: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+0017aeb0: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 0017aec0: 0a0a 2020 4063 6c61 7373 6d65 7468 6f64  ..  @classmethod
 0017aed0: 0a0a 2020 6465 6620 6973 5f72 6567 6973  ..  def is_regis
 0017aee0: 7465 7265 645f 6e6f 6465 5f74 7970 6528  tered_node_type(
 0017aef0: 636c 7329 202d 3e20 626f 6f6c 3a0a 0a20  cls) -> bool:.. 
 0017af00: 2020 2022 2222 0a0a 2020 2020 5472 7565     """..    True
 0017af10: 2069 6620 6120 7265 6769 7374 6572 6564   if a registered
 0017af20: 206e 6f64 6520 7479 7065 0a0a 2020 2020   node type..    
@@ -97041,16 +97041,16 @@
 0017b100: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 0017b110: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 0017b120: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 0017b130: 0a0a 636c 6173 7320 4765 6f6d 6574 7279  ..class Geometry
 0017b140: 4e6f 6465 496e 7075 7453 706c 696e 6543  NodeInputSplineC
 0017b150: 7963 6c69 6328 6270 795f 7374 7275 6374  yclic(bpy_struct
 0017b160: 2c20 4765 6f6d 6574 7279 4e6f 6465 2c20  , GeometryNode, 
-0017b170: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-0017b180: 616c 293a 0a0a 2020 2222 220a 0a20 2052  al):..  """..  R
+0017b170: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+0017b180: 6465 293a 0a0a 2020 2222 220a 0a20 2052  de):..  """..  R
 0017b190: 6574 7269 6576 6520 7768 6574 6865 7220  etrieve whether 
 0017b1a0: 6561 6368 2073 706c 696e 6520 656e 6470  each spline endp
 0017b1b0: 6f69 6e74 2063 6f6e 6e65 6374 7320 746f  oint connects to
 0017b1c0: 2074 6865 2062 6567 696e 6e69 6e67 0a0a   the beginning..
 0017b1d0: 2020 2222 220a 0a20 2040 636c 6173 736d    """..  @classm
 0017b1e0: 6574 686f 640a 0a20 2064 6566 2069 735f  ethod..  def is_
 0017b1f0: 7265 6769 7374 6572 6564 5f6e 6f64 655f  registered_node_
@@ -97090,16 +97090,16 @@
 0017b410: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 0017b420: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 0017b430: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 0017b440: 2020 2e2e 2e0a 0a63 6c61 7373 2047 656f    .....class Geo
 0017b450: 6d65 7472 794e 6f64 6549 6e70 7574 5370  metryNodeInputSp
 0017b460: 6c69 6e65 5265 736f 6c75 7469 6f6e 2862  lineResolution(b
 0017b470: 7079 5f73 7472 7563 742c 2047 656f 6d65  py_struct, Geome
-0017b480: 7472 794e 6f64 652c 204e 6f64 652c 204e  tryNode, Node, N
-0017b490: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+0017b480: 7472 794e 6f64 652c 204e 6f64 6549 6e74  tryNode, NodeInt
+0017b490: 6572 6e61 6c2c 204e 6f64 6529 3a0a 0a20  ernal, Node):.. 
 0017b4a0: 2022 2222 0a0a 2020 5265 7472 6965 7665   """..  Retrieve
 0017b4b0: 2074 6865 206e 756d 6265 7220 6f66 2065   the number of e
 0017b4c0: 7661 6c75 6174 6564 2070 6f69 6e74 7320  valuated points 
 0017b4d0: 7468 6174 2077 696c 6c20 6265 2067 656e  that will be gen
 0017b4e0: 6572 6174 6564 2066 6f72 2065 7665 7279  erated for every
 0017b4f0: 2063 6f6e 7472 6f6c 2070 6f69 6e74 206f   control point o
 0017b500: 6e20 6375 7276 6573 0a0a 2020 2222 220a  n curves..  """.
@@ -97141,16 +97141,16 @@
 0017b740: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 0017b750: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 0017b760: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 0017b770: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 0017b780: 0a63 6c61 7373 2047 656f 6d65 7472 794e  .class GeometryN
 0017b790: 6f64 6549 6e70 7574 5461 6e67 656e 7428  odeInputTangent(
 0017b7a0: 6270 795f 7374 7275 6374 2c20 4765 6f6d  bpy_struct, Geom
-0017b7b0: 6574 7279 4e6f 6465 2c20 4e6f 6465 2c20  etryNode, Node, 
-0017b7c0: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+0017b7b0: 6574 7279 4e6f 6465 2c20 4e6f 6465 496e  etryNode, NodeIn
+0017b7c0: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 0017b7d0: 2020 2222 220a 0a20 2052 6574 7269 6576    """..  Retriev
 0017b7e0: 6520 7468 6520 6469 7265 6374 696f 6e20  e the direction 
 0017b7f0: 6f66 2063 7572 7665 7320 6174 2065 6163  of curves at eac
 0017b800: 6820 636f 6e74 726f 6c20 706f 696e 740a  h control point.
 0017b810: 0a20 2022 2222 0a0a 2020 4063 6c61 7373  .  """..  @class
 0017b820: 6d65 7468 6f64 0a0a 2020 6465 6620 6973  method..  def is
 0017b830: 5f72 6567 6973 7465 7265 645f 6e6f 6465  _registered_node
@@ -97190,16 +97190,16 @@
 0017ba50: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 0017ba60: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 0017ba70: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 0017ba80: 2020 202e 2e2e 0a0a 636c 6173 7320 4765     .....class Ge
 0017ba90: 6f6d 6574 7279 4e6f 6465 496e 7374 616e  ometryNodeInstan
 0017baa0: 6365 4f6e 506f 696e 7473 2862 7079 5f73  ceOnPoints(bpy_s
 0017bab0: 7472 7563 742c 2047 656f 6d65 7472 794e  truct, GeometryN
-0017bac0: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-0017bad0: 6e74 6572 6e61 6c29 3a0a 0a20 2022 2222  nternal):..  """
+0017bac0: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
+0017bad0: 6c2c 204e 6f64 6529 3a0a 0a20 2022 2222  l, Node):..  """
 0017bae0: 0a0a 2020 4765 6e65 7261 7465 2061 2072  ..  Generate a r
 0017baf0: 6566 6572 656e 6365 2074 6f20 6765 6f6d  eference to geom
 0017bb00: 6574 7279 2061 7420 6561 6368 206f 6620  etry at each of 
 0017bb10: 7468 6520 696e 7075 7420 706f 696e 7473  the input points
 0017bb20: 2c20 7769 7468 6f75 7420 6475 706c 6963  , without duplic
 0017bb30: 6174 696e 6720 6974 7320 756e 6465 726c  ating its underl
 0017bb40: 7969 6e67 2064 6174 610a 0a20 2022 2222  ying data..  """
@@ -97242,16 +97242,16 @@
 0017bd90: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 0017bda0: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 0017bdb0: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 0017bdc0: 0a0a 636c 6173 7320 4765 6f6d 6574 7279  ..class Geometry
 0017bdd0: 4e6f 6465 496e 7374 616e 6365 7354 6f50  NodeInstancesToP
 0017bde0: 6f69 6e74 7328 6270 795f 7374 7275 6374  oints(bpy_struct
 0017bdf0: 2c20 4765 6f6d 6574 7279 4e6f 6465 2c20  , GeometryNode, 
-0017be00: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-0017be10: 616c 293a 0a0a 2020 2222 220a 0a20 2047  al):..  """..  G
+0017be00: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+0017be10: 6465 293a 0a0a 2020 2222 220a 0a20 2047  de):..  """..  G
 0017be20: 656e 6572 6174 6520 706f 696e 7473 2061  enerate points a
 0017be30: 7420 7468 6520 6f72 6967 696e 7320 6f66  t the origins of
 0017be40: 2069 6e73 7461 6e63 6573 2e0a 4e6f 7465   instances..Note
 0017be50: 3a20 4e65 7374 6564 2069 6e73 7461 6e63  : Nested instanc
 0017be60: 6573 2061 7265 206e 6f74 2061 6666 6563  es are not affec
 0017be70: 7465 6420 6279 2074 6869 7320 6e6f 6465  ted by this node
 0017be80: 0a0a 2020 2222 220a 0a20 2040 636c 6173  ..  """..  @clas
@@ -97293,16 +97293,16 @@
 0017c0c0: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 0017c0d0: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 0017c0e0: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 0017c0f0: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2047      .....class G
 0017c100: 656f 6d65 7472 794e 6f64 6549 6e74 6572  eometryNodeInter
 0017c110: 706f 6c61 7465 4375 7276 6573 2862 7079  polateCurves(bpy
 0017c120: 5f73 7472 7563 742c 2047 656f 6d65 7472  _struct, Geometr
-0017c130: 794e 6f64 652c 204e 6f64 652c 204e 6f64  yNode, Node, Nod
-0017c140: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2022  eInternal):..  "
+0017c130: 794e 6f64 652c 204e 6f64 6549 6e74 6572  yNode, NodeInter
+0017c140: 6e61 6c2c 204e 6f64 6529 3a0a 0a20 2022  nal, Node):..  "
 0017c150: 2222 0a0a 2020 4765 6e65 7261 7465 206e  ""..  Generate n
 0017c160: 6577 2063 7572 7665 7320 6f6e 2070 6f69  ew curves on poi
 0017c170: 6e74 7320 6279 2069 6e74 6572 706f 6c61  nts by interpola
 0017c180: 7469 6e67 2062 6574 7765 656e 2065 7869  ting between exi
 0017c190: 7374 696e 6720 6375 7276 6573 0a0a 2020  sting curves..  
 0017c1a0: 2222 220a 0a20 2040 636c 6173 736d 6574  """..  @classmet
 0017c1b0: 686f 640a 0a20 2064 6566 2069 735f 7265  hod..  def is_re
@@ -97343,15 +97343,15 @@
 0017c3e0: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 0017c3f0: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 0017c400: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 0017c410: 2e2e 2e0a 0a63 6c61 7373 2047 656f 6d65  .....class Geome
 0017c420: 7472 794e 6f64 6549 7356 6965 7770 6f72  tryNodeIsViewpor
 0017c430: 7428 6270 795f 7374 7275 6374 2c20 4765  t(bpy_struct, Ge
 0017c440: 6f6d 6574 7279 4e6f 6465 2c20 4e6f 6465  ometryNode, Node
-0017c450: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+0017c450: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 0017c460: 0a0a 2020 2222 220a 0a20 2052 6574 7269  ..  """..  Retri
 0017c470: 6576 6520 7768 6574 6865 7220 7468 6520  eve whether the 
 0017c480: 6e6f 6465 7320 6172 6520 6265 696e 6720  nodes are being 
 0017c490: 6576 616c 7561 7465 6420 666f 7220 7468  evaluated for th
 0017c4a0: 6520 7669 6577 706f 7274 2072 6174 6865  e viewport rathe
 0017c4b0: 7220 7468 616e 2074 6865 2066 696e 616c  r than the final
 0017c4c0: 2072 656e 6465 720a 0a20 2022 2222 0a0a   render..  """..
@@ -97393,16 +97393,16 @@
 0017c700: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 0017c710: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 0017c720: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 0017c730: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 0017c740: 636c 6173 7320 4765 6f6d 6574 7279 4e6f  class GeometryNo
 0017c750: 6465 4a6f 696e 4765 6f6d 6574 7279 2862  deJoinGeometry(b
 0017c760: 7079 5f73 7472 7563 742c 2047 656f 6d65  py_struct, Geome
-0017c770: 7472 794e 6f64 652c 204e 6f64 652c 204e  tryNode, Node, N
-0017c780: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+0017c770: 7472 794e 6f64 652c 204e 6f64 6549 6e74  tryNode, NodeInt
+0017c780: 6572 6e61 6c2c 204e 6f64 6529 3a0a 0a20  ernal, Node):.. 
 0017c790: 2022 2222 0a0a 2020 4d65 7267 6520 7365   """..  Merge se
 0017c7a0: 7061 7261 7465 6c79 2067 656e 6572 6174  parately generat
 0017c7b0: 6564 2067 656f 6d65 7472 6965 7320 696e  ed geometries in
 0017c7c0: 746f 2061 2073 696e 676c 6520 6f6e 650a  to a single one.
 0017c7d0: 0a20 2022 2222 0a0a 2020 4063 6c61 7373  .  """..  @class
 0017c7e0: 6d65 7468 6f64 0a0a 2020 6465 6620 6973  method..  def is
 0017c7f0: 5f72 6567 6973 7465 7265 645f 6e6f 6465  _registered_node
@@ -97442,16 +97442,16 @@
 0017ca10: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 0017ca20: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 0017ca30: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 0017ca40: 2020 202e 2e2e 0a0a 636c 6173 7320 4765     .....class Ge
 0017ca50: 6f6d 6574 7279 4e6f 6465 4d61 7465 7269  ometryNodeMateri
 0017ca60: 616c 5365 6c65 6374 696f 6e28 6270 795f  alSelection(bpy_
 0017ca70: 7374 7275 6374 2c20 4765 6f6d 6574 7279  struct, Geometry
-0017ca80: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-0017ca90: 496e 7465 726e 616c 293a 0a0a 2020 2222  Internal):..  ""
+0017ca80: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
+0017ca90: 616c 2c20 4e6f 6465 293a 0a0a 2020 2222  al, Node):..  ""
 0017caa0: 220a 0a20 2050 726f 7669 6465 2061 2073  "..  Provide a s
 0017cab0: 656c 6563 7469 6f6e 206f 6620 6661 6365  election of face
 0017cac0: 7320 7468 6174 2075 7365 2074 6865 2073  s that use the s
 0017cad0: 7065 6369 6669 6564 206d 6174 6572 6961  pecified materia
 0017cae0: 6c0a 0a20 2022 2222 0a0a 2020 4063 6c61  l..  """..  @cla
 0017caf0: 7373 6d65 7468 6f64 0a0a 2020 6465 6620  ssmethod..  def 
 0017cb00: 6973 5f72 6567 6973 7465 7265 645f 6e6f  is_registered_no
@@ -97491,16 +97491,16 @@
 0017cd20: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 0017cd30: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 0017cd40: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 0017cd50: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 0017cd60: 4765 6f6d 6574 7279 4e6f 6465 4d65 616e  GeometryNodeMean
 0017cd70: 4669 6c74 6572 5344 4656 6f6c 756d 6528  FilterSDFVolume(
 0017cd80: 6270 795f 7374 7275 6374 2c20 4765 6f6d  bpy_struct, Geom
-0017cd90: 6574 7279 4e6f 6465 2c20 4e6f 6465 2c20  etryNode, Node, 
-0017cda0: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+0017cd90: 6574 7279 4e6f 6465 2c20 4e6f 6465 496e  etryNode, NodeIn
+0017cda0: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 0017cdb0: 2020 2222 220a 0a20 2053 6d6f 6f74 6820    """..  Smooth 
 0017cdc0: 7468 6520 7375 7266 6163 6520 6f66 2061  the surface of a
 0017cdd0: 6e20 5344 4620 766f 6c75 6d65 2062 7920  n SDF volume by 
 0017cde0: 6170 706c 7969 6e67 2061 206d 6561 6e20  applying a mean 
 0017cdf0: 6669 6c74 6572 0a0a 2020 2222 220a 0a20  filter..  """.. 
 0017ce00: 2040 636c 6173 736d 6574 686f 640a 0a20   @classmethod.. 
 0017ce10: 2064 6566 2069 735f 7265 6769 7374 6572   def is_register
@@ -97540,16 +97540,16 @@
 0017d030: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 0017d040: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 0017d050: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 0017d060: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 0017d070: 6c61 7373 2047 656f 6d65 7472 794e 6f64  lass GeometryNod
 0017d080: 654d 6572 6765 4279 4469 7374 616e 6365  eMergeByDistance
 0017d090: 2862 7079 5f73 7472 7563 742c 2047 656f  (bpy_struct, Geo
-0017d0a0: 6d65 7472 794e 6f64 652c 204e 6f64 652c  metryNode, Node,
-0017d0b0: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+0017d0a0: 6d65 7472 794e 6f64 652c 204e 6f64 6549  metryNode, NodeI
+0017d0b0: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 0017d0c0: 0a20 2022 2222 0a0a 2020 4d65 7267 6520  .  """..  Merge 
 0017d0d0: 7665 7274 6963 6573 206f 7220 706f 696e  vertices or poin
 0017d0e0: 7473 2077 6974 6869 6e20 6120 6769 7665  ts within a give
 0017d0f0: 6e20 6469 7374 616e 6365 0a0a 2020 2222  n distance..  ""
 0017d100: 220a 0a20 206d 6f64 653a 2073 7472 203d  "..  mode: str =
 0017d110: 202e 2e2e 0a0a 2020 2222 220a 0a20 202a   .....  """..  *
 0017d120: 2060 6041 4c4c 6060 0a41 6c6c 202d 2d20   ``ALL``.All -- 
@@ -97603,16 +97603,16 @@
 0017d420: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 0017d430: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 0017d440: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 0017d450: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 0017d460: 2047 656f 6d65 7472 794e 6f64 654d 6573   GeometryNodeMes
 0017d470: 6842 6f6f 6c65 616e 2862 7079 5f73 7472  hBoolean(bpy_str
 0017d480: 7563 742c 2047 656f 6d65 7472 794e 6f64  uct, GeometryNod
-0017d490: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-0017d4a0: 6572 6e61 6c29 3a0a 0a20 2022 2222 0a0a  ernal):..  """..
+0017d490: 652c 204e 6f64 6549 6e74 6572 6e61 6c2c  e, NodeInternal,
+0017d4a0: 204e 6f64 6529 3a0a 0a20 2022 2222 0a0a   Node):..  """..
 0017d4b0: 2020 4375 742c 2073 7562 7472 6163 742c    Cut, subtract,
 0017d4c0: 206f 7220 6a6f 696e 206d 756c 7469 706c   or join multipl
 0017d4d0: 6520 6d65 7368 2069 6e70 7574 730a 0a20  e mesh inputs.. 
 0017d4e0: 2022 2222 0a0a 2020 6f70 6572 6174 696f   """..  operatio
 0017d4f0: 6e3a 2073 7472 203d 202e 2e2e 0a0a 2020  n: str = .....  
 0017d500: 2222 220a 0a20 202a 2060 6049 4e54 4552  """..  * ``INTER
 0017d510: 5345 4354 6060 0a49 6e74 6572 7365 6374  SECT``.Intersect
@@ -97667,16 +97667,16 @@
 0017d820: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 0017d830: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 0017d840: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 0017d850: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 0017d860: 7373 2047 656f 6d65 7472 794e 6f64 654d  ss GeometryNodeM
 0017d870: 6573 6843 6972 636c 6528 6270 795f 7374  eshCircle(bpy_st
 0017d880: 7275 6374 2c20 4765 6f6d 6574 7279 4e6f  ruct, GeometryNo
-0017d890: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-0017d8a0: 7465 726e 616c 293a 0a0a 2020 2222 220a  ternal):..  """.
+0017d890: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+0017d8a0: 2c20 4e6f 6465 293a 0a0a 2020 2222 220a  , Node):..  """.
 0017d8b0: 0a20 2047 656e 6572 6174 6520 6120 6369  .  Generate a ci
 0017d8c0: 7263 756c 6172 2072 696e 6720 6f66 2065  rcular ring of e
 0017d8d0: 6467 6573 0a0a 2020 2222 220a 0a20 2066  dges..  """..  f
 0017d8e0: 696c 6c5f 7479 7065 3a20 7374 7220 3d20  ill_type: str = 
 0017d8f0: 2e2e 2e0a 0a20 2040 636c 6173 736d 6574  .....  @classmet
 0017d900: 686f 640a 0a20 2064 6566 2069 735f 7265  hod..  def is_re
 0017d910: 6769 7374 6572 6564 5f6e 6f64 655f 7479  gistered_node_ty
@@ -97715,16 +97715,16 @@
 0017db20: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 0017db30: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 0017db40: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 0017db50: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 0017db60: 2e2e 2e0a 0a63 6c61 7373 2047 656f 6d65  .....class Geome
 0017db70: 7472 794e 6f64 654d 6573 6843 6f6e 6528  tryNodeMeshCone(
 0017db80: 6270 795f 7374 7275 6374 2c20 4765 6f6d  bpy_struct, Geom
-0017db90: 6574 7279 4e6f 6465 2c20 4e6f 6465 2c20  etryNode, Node, 
-0017dba0: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+0017db90: 6574 7279 4e6f 6465 2c20 4e6f 6465 496e  etryNode, NodeIn
+0017dba0: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 0017dbb0: 2020 2222 220a 0a20 2047 656e 6572 6174    """..  Generat
 0017dbc0: 6520 6120 636f 6e65 206d 6573 680a 0a20  e a cone mesh.. 
 0017dbd0: 2022 2222 0a0a 2020 6669 6c6c 5f74 7970   """..  fill_typ
 0017dbe0: 653a 2073 7472 203d 202e 2e2e 0a0a 2020  e: str = .....  
 0017dbf0: 4063 6c61 7373 6d65 7468 6f64 0a0a 2020  @classmethod..  
 0017dc00: 6465 6620 6973 5f72 6567 6973 7465 7265  def is_registere
 0017dc10: 645f 6e6f 6465 5f74 7970 6528 636c 7329  d_node_type(cls)
@@ -97763,16 +97763,16 @@
 0017de20: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 0017de30: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 0017de40: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 0017de50: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 0017de60: 6173 7320 4765 6f6d 6574 7279 4e6f 6465  ass GeometryNode
 0017de70: 4d65 7368 4375 6265 2862 7079 5f73 7472  MeshCube(bpy_str
 0017de80: 7563 742c 2047 656f 6d65 7472 794e 6f64  uct, GeometryNod
-0017de90: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-0017dea0: 6572 6e61 6c29 3a0a 0a20 2022 2222 0a0a  ernal):..  """..
+0017de90: 652c 204e 6f64 6549 6e74 6572 6e61 6c2c  e, NodeInternal,
+0017dea0: 204e 6f64 6529 3a0a 0a20 2022 2222 0a0a   Node):..  """..
 0017deb0: 2020 4765 6e65 7261 7465 2061 2063 7562    Generate a cub
 0017dec0: 6f69 6420 6d65 7368 2077 6974 6820 7661  oid mesh with va
 0017ded0: 7269 6162 6c65 2073 6964 6520 6c65 6e67  riable side leng
 0017dee0: 7468 7320 616e 6420 7375 6264 6976 6973  ths and subdivis
 0017def0: 696f 6e73 0a0a 2020 2222 220a 0a20 2040  ions..  """..  @
 0017df00: 636c 6173 736d 6574 686f 640a 0a20 2064  classmethod..  d
 0017df10: 6566 2069 735f 7265 6769 7374 6572 6564  ef is_registered
@@ -97812,16 +97812,16 @@
 0017e130: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 0017e140: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 0017e150: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 0017e160: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 0017e170: 7373 2047 656f 6d65 7472 794e 6f64 654d  ss GeometryNodeM
 0017e180: 6573 6843 796c 696e 6465 7228 6270 795f  eshCylinder(bpy_
 0017e190: 7374 7275 6374 2c20 4765 6f6d 6574 7279  struct, Geometry
-0017e1a0: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-0017e1b0: 496e 7465 726e 616c 293a 0a0a 2020 2222  Internal):..  ""
+0017e1a0: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
+0017e1b0: 616c 2c20 4e6f 6465 293a 0a0a 2020 2222  al, Node):..  ""
 0017e1c0: 220a 0a20 2047 656e 6572 6174 6520 6120  "..  Generate a 
 0017e1d0: 6379 6c69 6e64 6572 206d 6573 680a 0a20  cylinder mesh.. 
 0017e1e0: 2022 2222 0a0a 2020 6669 6c6c 5f74 7970   """..  fill_typ
 0017e1f0: 653a 2073 7472 203d 202e 2e2e 0a0a 2020  e: str = .....  
 0017e200: 4063 6c61 7373 6d65 7468 6f64 0a0a 2020  @classmethod..  
 0017e210: 6465 6620 6973 5f72 6567 6973 7465 7265  def is_registere
 0017e220: 645f 6e6f 6465 5f74 7970 6528 636c 7329  d_node_type(cls)
@@ -97861,16 +97861,16 @@
 0017e440: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 0017e450: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 0017e460: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 0017e470: 6173 7320 4765 6f6d 6574 7279 4e6f 6465  ass GeometryNode
 0017e480: 4d65 7368 4661 6365 5365 7442 6f75 6e64  MeshFaceSetBound
 0017e490: 6172 6965 7328 6270 795f 7374 7275 6374  aries(bpy_struct
 0017e4a0: 2c20 4765 6f6d 6574 7279 4e6f 6465 2c20  , GeometryNode, 
-0017e4b0: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-0017e4c0: 616c 293a 0a0a 2020 2222 220a 0a20 2046  al):..  """..  F
+0017e4b0: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+0017e4c0: 6465 293a 0a0a 2020 2222 220a 0a20 2046  de):..  """..  F
 0017e4d0: 696e 6420 6564 6765 7320 6f6e 2074 6865  ind edges on the
 0017e4e0: 2062 6f75 6e64 6172 6965 7320 6265 7477   boundaries betw
 0017e4f0: 6565 6e20 6772 6f75 7073 206f 6620 6661  een groups of fa
 0017e500: 6365 7320 7769 7468 2074 6865 2073 616d  ces with the sam
 0017e510: 6520 4944 2076 616c 7565 0a0a 2020 2222  e ID value..  ""
 0017e520: 220a 0a20 2040 636c 6173 736d 6574 686f  "..  @classmetho
 0017e530: 640a 0a20 2064 6566 2069 735f 7265 6769  d..  def is_regi
@@ -97910,16 +97910,16 @@
 0017e750: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 0017e760: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 0017e770: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 0017e780: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 0017e790: 2e0a 0a63 6c61 7373 2047 656f 6d65 7472  ...class Geometr
 0017e7a0: 794e 6f64 654d 6573 6847 7269 6428 6270  yNodeMeshGrid(bp
 0017e7b0: 795f 7374 7275 6374 2c20 4765 6f6d 6574  y_struct, Geomet
-0017e7c0: 7279 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  ryNode, Node, No
-0017e7d0: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+0017e7c0: 7279 4e6f 6465 2c20 4e6f 6465 496e 7465  ryNode, NodeInte
+0017e7d0: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 0017e7e0: 2222 220a 0a20 2047 656e 6572 6174 6520  """..  Generate 
 0017e7f0: 6120 706c 616e 6172 206d 6573 6820 6f6e  a planar mesh on
 0017e800: 2074 6865 2058 5920 706c 616e 650a 0a20   the XY plane.. 
 0017e810: 2022 2222 0a0a 2020 4063 6c61 7373 6d65   """..  @classme
 0017e820: 7468 6f64 0a0a 2020 6465 6620 6973 5f72  thod..  def is_r
 0017e830: 6567 6973 7465 7265 645f 6e6f 6465 5f74  egistered_node_t
 0017e840: 7970 6528 636c 7329 202d 3e20 626f 6f6c  ype(cls) -> bool
@@ -97958,16 +97958,16 @@
 0017ea50: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 0017ea60: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 0017ea70: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 0017ea80: 202e 2e2e 0a0a 636c 6173 7320 4765 6f6d   .....class Geom
 0017ea90: 6574 7279 4e6f 6465 4d65 7368 4963 6f53  etryNodeMeshIcoS
 0017eaa0: 7068 6572 6528 6270 795f 7374 7275 6374  phere(bpy_struct
 0017eab0: 2c20 4765 6f6d 6574 7279 4e6f 6465 2c20  , GeometryNode, 
-0017eac0: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-0017ead0: 616c 293a 0a0a 2020 2222 220a 0a20 2047  al):..  """..  G
+0017eac0: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+0017ead0: 6465 293a 0a0a 2020 2222 220a 0a20 2047  de):..  """..  G
 0017eae0: 656e 6572 6174 6520 6120 7370 6865 7269  enerate a spheri
 0017eaf0: 6361 6c20 6d65 7368 2074 6861 7420 636f  cal mesh that co
 0017eb00: 6e73 6973 7473 206f 6620 6571 7561 6c6c  nsists of equall
 0017eb10: 7920 7369 7a65 6420 7472 6961 6e67 6c65  y sized triangle
 0017eb20: 730a 0a20 2022 2222 0a0a 2020 4063 6c61  s..  """..  @cla
 0017eb30: 7373 6d65 7468 6f64 0a0a 2020 6465 6620  ssmethod..  def 
 0017eb40: 6973 5f72 6567 6973 7465 7265 645f 6e6f  is_registered_no
@@ -98007,16 +98007,16 @@
 0017ed60: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 0017ed70: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 0017ed80: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 0017ed90: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 0017eda0: 4765 6f6d 6574 7279 4e6f 6465 4d65 7368  GeometryNodeMesh
 0017edb0: 4c69 6e65 2862 7079 5f73 7472 7563 742c  Line(bpy_struct,
 0017edc0: 2047 656f 6d65 7472 794e 6f64 652c 204e   GeometryNode, N
-0017edd0: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-0017ede0: 6c29 3a0a 0a20 2022 2222 0a0a 2020 4765  l):..  """..  Ge
+0017edd0: 6f64 6549 6e74 6572 6e61 6c2c 204e 6f64  odeInternal, Nod
+0017ede0: 6529 3a0a 0a20 2022 2222 0a0a 2020 4765  e):..  """..  Ge
 0017edf0: 6e65 7261 7465 2076 6572 7469 6365 7320  nerate vertices 
 0017ee00: 696e 2061 206c 696e 6520 616e 6420 636f  in a line and co
 0017ee10: 6e6e 6563 7420 7468 656d 2077 6974 6820  nnect them with 
 0017ee20: 6564 6765 730a 0a20 2022 2222 0a0a 2020  edges..  """..  
 0017ee30: 636f 756e 745f 6d6f 6465 3a20 7374 7220  count_mode: str 
 0017ee40: 3d20 2e2e 2e0a 0a20 2022 2222 0a0a 2020  = .....  """..  
 0017ee50: 2a20 6060 544f 5441 4c60 600a 436f 756e  * ``TOTAL``.Coun
@@ -98077,16 +98077,16 @@
 0017f1c0: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 0017f1d0: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 0017f1e0: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 0017f1f0: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 0017f200: 0a0a 636c 6173 7320 4765 6f6d 6574 7279  ..class Geometry
 0017f210: 4e6f 6465 4d65 7368 546f 4375 7276 6528  NodeMeshToCurve(
 0017f220: 6270 795f 7374 7275 6374 2c20 4765 6f6d  bpy_struct, Geom
-0017f230: 6574 7279 4e6f 6465 2c20 4e6f 6465 2c20  etryNode, Node, 
-0017f240: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+0017f230: 6574 7279 4e6f 6465 2c20 4e6f 6465 496e  etryNode, NodeIn
+0017f240: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 0017f250: 2020 2222 220a 0a20 2047 656e 6572 6174    """..  Generat
 0017f260: 6520 6120 6375 7276 6520 6672 6f6d 2061  e a curve from a
 0017f270: 206d 6573 680a 0a20 2022 2222 0a0a 2020   mesh..  """..  
 0017f280: 4063 6c61 7373 6d65 7468 6f64 0a0a 2020  @classmethod..  
 0017f290: 6465 6620 6973 5f72 6567 6973 7465 7265  def is_registere
 0017f2a0: 645f 6e6f 6465 5f74 7970 6528 636c 7329  d_node_type(cls)
 0017f2b0: 202d 3e20 626f 6f6c 3a0a 0a20 2020 2022   -> bool:..    "
@@ -98124,16 +98124,16 @@
 0017f4b0: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 0017f4c0: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 0017f4d0: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 0017f4e0: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 0017f4f0: 6173 7320 4765 6f6d 6574 7279 4e6f 6465  ass GeometryNode
 0017f500: 4d65 7368 546f 506f 696e 7473 2862 7079  MeshToPoints(bpy
 0017f510: 5f73 7472 7563 742c 2047 656f 6d65 7472  _struct, Geometr
-0017f520: 794e 6f64 652c 204e 6f64 652c 204e 6f64  yNode, Node, Nod
-0017f530: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2022  eInternal):..  "
+0017f520: 794e 6f64 652c 204e 6f64 6549 6e74 6572  yNode, NodeInter
+0017f530: 6e61 6c2c 204e 6f64 6529 3a0a 0a20 2022  nal, Node):..  "
 0017f540: 2222 0a0a 2020 4765 6e65 7261 7465 2061  ""..  Generate a
 0017f550: 2070 6f69 6e74 2063 6c6f 7564 2066 726f   point cloud fro
 0017f560: 6d20 6120 6d65 7368 2773 2076 6572 7469  m a mesh's verti
 0017f570: 6365 730a 0a20 2022 2222 0a0a 2020 6d6f  ces..  """..  mo
 0017f580: 6465 3a20 7374 7220 3d20 2e2e 2e0a 0a20  de: str = ..... 
 0017f590: 2022 2222 0a0a 2020 2a20 6060 5645 5254   """..  * ``VERT
 0017f5a0: 4943 4553 6060 0a56 6572 7469 6365 7320  ICES``.Vertices 
@@ -98196,16 +98196,16 @@
 0017f930: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 0017f940: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 0017f950: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 0017f960: 2020 202e 2e2e 0a0a 636c 6173 7320 4765     .....class Ge
 0017f970: 6f6d 6574 7279 4e6f 6465 4d65 7368 546f  ometryNodeMeshTo
 0017f980: 5344 4656 6f6c 756d 6528 6270 795f 7374  SDFVolume(bpy_st
 0017f990: 7275 6374 2c20 4765 6f6d 6574 7279 4e6f  ruct, GeometryNo
-0017f9a0: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-0017f9b0: 7465 726e 616c 293a 0a0a 2020 2222 220a  ternal):..  """.
+0017f9a0: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+0017f9b0: 2c20 4e6f 6465 293a 0a0a 2020 2222 220a  , Node):..  """.
 0017f9c0: 0a20 2043 7265 6174 6520 616e 2053 4446  .  Create an SDF
 0017f9d0: 2076 6f6c 756d 6520 7769 7468 2074 6865   volume with the
 0017f9e0: 2073 6861 7065 206f 6620 7468 6520 696e   shape of the in
 0017f9f0: 7075 7420 6d65 7368 2773 2073 7572 6661  put mesh's surfa
 0017fa00: 6365 0a0a 2020 2222 220a 0a20 2072 6573  ce..  """..  res
 0017fa10: 6f6c 7574 696f 6e5f 6d6f 6465 3a20 7374  olution_mode: st
 0017fa20: 7220 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  r = .....  """..
@@ -98258,16 +98258,16 @@
 0017fd10: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 0017fd20: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 0017fd30: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 0017fd40: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 0017fd50: 4765 6f6d 6574 7279 4e6f 6465 4d65 7368  GeometryNodeMesh
 0017fd60: 546f 566f 6c75 6d65 2862 7079 5f73 7472  ToVolume(bpy_str
 0017fd70: 7563 742c 2047 656f 6d65 7472 794e 6f64  uct, GeometryNod
-0017fd80: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-0017fd90: 6572 6e61 6c29 3a0a 0a20 2022 2222 0a0a  ernal):..  """..
+0017fd80: 652c 204e 6f64 6549 6e74 6572 6e61 6c2c  e, NodeInternal,
+0017fd90: 204e 6f64 6529 3a0a 0a20 2022 2222 0a0a   Node):..  """..
 0017fda0: 2020 4372 6561 7465 2061 2066 6f67 2076    Create a fog v
 0017fdb0: 6f6c 756d 6520 7769 7468 2074 6865 2073  olume with the s
 0017fdc0: 6861 7065 206f 6620 7468 6520 696e 7075  hape of the inpu
 0017fdd0: 7420 6d65 7368 2773 2073 7572 6661 6365  t mesh's surface
 0017fde0: 0a0a 2020 2222 220a 0a20 2072 6573 6f6c  ..  """..  resol
 0017fdf0: 7574 696f 6e5f 6d6f 6465 3a20 7374 7220  ution_mode: str 
 0017fe00: 3d20 2e2e 2e0a 0a20 2022 2222 0a0a 2020  = .....  """..  
@@ -98320,16 +98320,16 @@
 001800f0: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 00180100: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 00180110: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 00180120: 2020 202e 2e2e 0a0a 636c 6173 7320 4765     .....class Ge
 00180130: 6f6d 6574 7279 4e6f 6465 4d65 7368 5556  ometryNodeMeshUV
 00180140: 5370 6865 7265 2862 7079 5f73 7472 7563  Sphere(bpy_struc
 00180150: 742c 2047 656f 6d65 7472 794e 6f64 652c  t, GeometryNode,
-00180160: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-00180170: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+00180160: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+00180170: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 00180180: 4765 6e65 7261 7465 2061 2073 7068 6572  Generate a spher
 00180190: 6963 616c 206d 6573 6820 7769 7468 2071  ical mesh with q
 001801a0: 7561 6473 2c20 6578 6365 7074 2066 6f72  uads, except for
 001801b0: 2074 7269 616e 676c 6573 2061 7420 7468   triangles at th
 001801c0: 6520 746f 7020 616e 6420 626f 7474 6f6d  e top and bottom
 001801d0: 0a0a 2020 2222 220a 0a20 2040 636c 6173  ..  """..  @clas
 001801e0: 736d 6574 686f 640a 0a20 2064 6566 2069  smethod..  def i
@@ -98370,16 +98370,16 @@
 00180410: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 00180420: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 00180430: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 00180440: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2047      .....class G
 00180450: 656f 6d65 7472 794e 6f64 654f 626a 6563  eometryNodeObjec
 00180460: 7449 6e66 6f28 6270 795f 7374 7275 6374  tInfo(bpy_struct
 00180470: 2c20 4765 6f6d 6574 7279 4e6f 6465 2c20  , GeometryNode, 
-00180480: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-00180490: 616c 293a 0a0a 2020 2222 220a 0a20 2052  al):..  """..  R
+00180480: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+00180490: 6465 293a 0a0a 2020 2222 220a 0a20 2052  de):..  """..  R
 001804a0: 6574 7269 6576 6520 696e 666f 726d 6174  etrieve informat
 001804b0: 696f 6e20 6672 6f6d 2061 6e20 6f62 6a65  ion from an obje
 001804c0: 6374 0a0a 2020 2222 220a 0a20 2074 7261  ct..  """..  tra
 001804d0: 6e73 666f 726d 5f73 7061 6365 3a20 7374  nsform_space: st
 001804e0: 7220 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  r = .....  """..
 001804f0: 2020 5468 6520 7472 616e 7366 6f72 6d61    The transforma
 00180500: 7469 6f6e 206f 6620 7468 6520 7665 6374  tion of the vect
@@ -98445,16 +98445,16 @@
 001808c0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 001808d0: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 001808e0: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 001808f0: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 00180900: 2047 656f 6d65 7472 794e 6f64 654f 6666   GeometryNodeOff
 00180910: 7365 7443 6f72 6e65 7249 6e46 6163 6528  setCornerInFace(
 00180920: 6270 795f 7374 7275 6374 2c20 4765 6f6d  bpy_struct, Geom
-00180930: 6574 7279 4e6f 6465 2c20 4e6f 6465 2c20  etryNode, Node, 
-00180940: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+00180930: 6574 7279 4e6f 6465 2c20 4e6f 6465 496e  etryNode, NodeIn
+00180940: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 00180950: 2020 2222 220a 0a20 2052 6574 7269 6576    """..  Retriev
 00180960: 6520 636f 726e 6572 7320 696e 2074 6865  e corners in the
 00180970: 2073 616d 6520 6661 6365 2061 7320 616e   same face as an
 00180980: 6f74 6865 720a 0a20 2022 2222 0a0a 2020  other..  """..  
 00180990: 4063 6c61 7373 6d65 7468 6f64 0a0a 2020  @classmethod..  
 001809a0: 6465 6620 6973 5f72 6567 6973 7465 7265  def is_registere
 001809b0: 645f 6e6f 6465 5f74 7970 6528 636c 7329  d_node_type(cls)
@@ -98494,15 +98494,15 @@
 00180bd0: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 00180be0: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 00180bf0: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 00180c00: 6173 7320 4765 6f6d 6574 7279 4e6f 6465  ass GeometryNode
 00180c10: 4f66 6673 6574 506f 696e 7449 6e43 7572  OffsetPointInCur
 00180c20: 7665 2862 7079 5f73 7472 7563 742c 2047  ve(bpy_struct, G
 00180c30: 656f 6d65 7472 794e 6f64 652c 204e 6f64  eometryNode, Nod
-00180c40: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+00180c40: 6549 6e74 6572 6e61 6c2c 204e 6f64 6529  eInternal, Node)
 00180c50: 3a0a 0a20 2022 2222 0a0a 2020 4f66 6673  :..  """..  Offs
 00180c60: 6574 2061 2063 6f6e 7472 6f6c 2070 6f69  et a control poi
 00180c70: 6e74 2069 6e64 6578 2077 6974 6869 6e20  nt index within 
 00180c80: 6974 7320 6375 7276 650a 0a20 2022 2222  its curve..  """
 00180c90: 0a0a 2020 4063 6c61 7373 6d65 7468 6f64  ..  @classmethod
 00180ca0: 0a0a 2020 6465 6620 6973 5f72 6567 6973  ..  def is_regis
 00180cb0: 7465 7265 645f 6e6f 6465 5f74 7970 6528  tered_node_type(
@@ -98542,15 +98542,15 @@
 00180ed0: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 00180ee0: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 00180ef0: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 00180f00: 0a0a 636c 6173 7320 4765 6f6d 6574 7279  ..class Geometry
 00180f10: 4e6f 6465 4f66 6673 6574 5344 4656 6f6c  NodeOffsetSDFVol
 00180f20: 756d 6528 6270 795f 7374 7275 6374 2c20  ume(bpy_struct, 
 00180f30: 4765 6f6d 6574 7279 4e6f 6465 2c20 4e6f  GeometryNode, No
-00180f40: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+00180f40: 6465 496e 7465 726e 616c 2c20 4e6f 6465  deInternal, Node
 00180f50: 293a 0a0a 2020 2222 220a 0a20 204d 6f76  ):..  """..  Mov
 00180f60: 6520 7468 6520 7375 7266 6163 6520 6f66  e the surface of
 00180f70: 2061 6e20 5344 4620 766f 6c75 6d65 2069   an SDF volume i
 00180f80: 6e77 6172 6473 206f 7220 6f75 7477 6172  nwards or outwar
 00180f90: 6473 0a0a 2020 2222 220a 0a20 2040 636c  ds..  """..  @cl
 00180fa0: 6173 736d 6574 686f 640a 0a20 2064 6566  assmethod..  def
 00180fb0: 2069 735f 7265 6769 7374 6572 6564 5f6e   is_registered_n
@@ -98590,15 +98590,15 @@
 001811d0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 001811e0: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 001811f0: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 00181200: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 00181210: 2047 656f 6d65 7472 794e 6f64 6550 6f69   GeometryNodePoi
 00181220: 6e74 7328 6270 795f 7374 7275 6374 2c20  nts(bpy_struct, 
 00181230: 4765 6f6d 6574 7279 4e6f 6465 2c20 4e6f  GeometryNode, No
-00181240: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+00181240: 6465 496e 7465 726e 616c 2c20 4e6f 6465  deInternal, Node
 00181250: 293a 0a0a 2020 2222 220a 0a20 2047 656e  ):..  """..  Gen
 00181260: 6572 6174 6520 6120 706f 696e 7420 636c  erate a point cl
 00181270: 6f75 6420 7769 7468 2070 6f73 6974 696f  oud with positio
 00181280: 6e73 2061 6e64 2072 6164 6969 2064 6566  ns and radii def
 00181290: 696e 6564 2062 7920 6669 656c 6473 0a0a  ined by fields..
 001812a0: 2020 2222 220a 0a20 2040 636c 6173 736d    """..  @classm
 001812b0: 6574 686f 640a 0a20 2064 6566 2069 735f  ethod..  def is_
@@ -98639,16 +98639,16 @@
 001814e0: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 001814f0: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 00181500: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 00181510: 2020 2e2e 2e0a 0a63 6c61 7373 2047 656f    .....class Geo
 00181520: 6d65 7472 794e 6f64 6550 6f69 6e74 734f  metryNodePointsO
 00181530: 6643 7572 7665 2862 7079 5f73 7472 7563  fCurve(bpy_struc
 00181540: 742c 2047 656f 6d65 7472 794e 6f64 652c  t, GeometryNode,
-00181550: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-00181560: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+00181550: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+00181560: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 00181570: 5265 7472 6965 7665 2061 2070 6f69 6e74  Retrieve a point
 00181580: 2069 6e64 6578 2077 6974 6869 6e20 6120   index within a 
 00181590: 6375 7276 650a 0a20 2022 2222 0a0a 2020  curve..  """..  
 001815a0: 4063 6c61 7373 6d65 7468 6f64 0a0a 2020  @classmethod..  
 001815b0: 6465 6620 6973 5f72 6567 6973 7465 7265  def is_registere
 001815c0: 645f 6e6f 6465 5f74 7970 6528 636c 7329  d_node_type(cls)
 001815d0: 202d 3e20 626f 6f6c 3a0a 0a20 2020 2022   -> bool:..    "
@@ -98687,15 +98687,15 @@
 001817e0: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 001817f0: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 00181800: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 00181810: 6173 7320 4765 6f6d 6574 7279 4e6f 6465  ass GeometryNode
 00181820: 506f 696e 7473 546f 5344 4656 6f6c 756d  PointsToSDFVolum
 00181830: 6528 6270 795f 7374 7275 6374 2c20 4765  e(bpy_struct, Ge
 00181840: 6f6d 6574 7279 4e6f 6465 2c20 4e6f 6465  ometryNode, Node
-00181850: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+00181850: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 00181860: 0a0a 2020 2222 220a 0a20 2047 656e 6572  ..  """..  Gener
 00181870: 6174 6520 616e 2053 4446 2076 6f6c 756d  ate an SDF volum
 00181880: 6520 7370 6865 7265 2061 726f 756e 6420  e sphere around 
 00181890: 6576 6572 7920 706f 696e 740a 0a20 2022  every point..  "
 001818a0: 2222 0a0a 2020 7265 736f 6c75 7469 6f6e  ""..  resolution
 001818b0: 5f6d 6f64 653a 2073 7472 203d 202e 2e2e  _mode: str = ...
 001818c0: 0a0a 2020 2222 220a 0a20 2048 6f77 2074  ..  """..  How t
@@ -98749,16 +98749,16 @@
 00181bc0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 00181bd0: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 00181be0: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 00181bf0: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 00181c00: 2047 656f 6d65 7472 794e 6f64 6550 6f69   GeometryNodePoi
 00181c10: 6e74 7354 6f56 6572 7469 6365 7328 6270  ntsToVertices(bp
 00181c20: 795f 7374 7275 6374 2c20 4765 6f6d 6574  y_struct, Geomet
-00181c30: 7279 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  ryNode, Node, No
-00181c40: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+00181c30: 7279 4e6f 6465 2c20 4e6f 6465 496e 7465  ryNode, NodeInte
+00181c40: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 00181c50: 2222 220a 0a20 2047 656e 6572 6174 6520  """..  Generate 
 00181c60: 6120 6d65 7368 2076 6572 7465 7820 666f  a mesh vertex fo
 00181c70: 7220 6561 6368 2070 6f69 6e74 2063 6c6f  r each point clo
 00181c80: 7564 2070 6f69 6e74 0a0a 2020 2222 220a  ud point..  """.
 00181c90: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
 00181ca0: 0a20 2064 6566 2069 735f 7265 6769 7374  .  def is_regist
 00181cb0: 6572 6564 5f6e 6f64 655f 7479 7065 2863  ered_node_type(c
@@ -98798,15 +98798,15 @@
 00181ed0: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 00181ee0: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 00181ef0: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 00181f00: 0a63 6c61 7373 2047 656f 6d65 7472 794e  .class GeometryN
 00181f10: 6f64 6550 6f69 6e74 7354 6f56 6f6c 756d  odePointsToVolum
 00181f20: 6528 6270 795f 7374 7275 6374 2c20 4765  e(bpy_struct, Ge
 00181f30: 6f6d 6574 7279 4e6f 6465 2c20 4e6f 6465  ometryNode, Node
-00181f40: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+00181f40: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 00181f50: 0a0a 2020 2222 220a 0a20 2047 656e 6572  ..  """..  Gener
 00181f60: 6174 6520 6120 666f 6720 766f 6c75 6d65  ate a fog volume
 00181f70: 2073 7068 6572 6520 6172 6f75 6e64 2065   sphere around e
 00181f80: 7665 7279 2070 6f69 6e74 0a0a 2020 2222  very point..  ""
 00181f90: 220a 0a20 2072 6573 6f6c 7574 696f 6e5f  "..  resolution_
 00181fa0: 6d6f 6465 3a20 7374 7220 3d20 2e2e 2e0a  mode: str = ....
 00181fb0: 0a20 2022 2222 0a0a 2020 486f 7720 7468  .  """..  How th
@@ -98860,16 +98860,16 @@
 001822b0: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 001822c0: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 001822d0: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 001822e0: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 001822f0: 4765 6f6d 6574 7279 4e6f 6465 5072 6f78  GeometryNodeProx
 00182300: 696d 6974 7928 6270 795f 7374 7275 6374  imity(bpy_struct
 00182310: 2c20 4765 6f6d 6574 7279 4e6f 6465 2c20  , GeometryNode, 
-00182320: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-00182330: 616c 293a 0a0a 2020 2222 220a 0a20 2043  al):..  """..  C
+00182320: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+00182330: 6465 293a 0a0a 2020 2222 220a 0a20 2043  de):..  """..  C
 00182340: 6f6d 7075 7465 2074 6865 2063 6c6f 7365  ompute the close
 00182350: 7374 206c 6f63 6174 696f 6e20 6f6e 2074  st location on t
 00182360: 6865 2074 6172 6765 7420 6765 6f6d 6574  he target geomet
 00182370: 7279 0a0a 2020 2222 220a 0a20 2074 6172  ry..  """..  tar
 00182380: 6765 745f 656c 656d 656e 743a 2073 7472  get_element: str
 00182390: 203d 202e 2e2e 0a0a 2020 2222 220a 0a20   = .....  """.. 
 001823a0: 2045 6c65 6d65 6e74 206f 6620 7468 6520   Element of the 
@@ -98930,16 +98930,16 @@
 00182710: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 00182720: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 00182730: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 00182740: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 00182750: 7373 2047 656f 6d65 7472 794e 6f64 6552  ss GeometryNodeR
 00182760: 6179 6361 7374 2862 7079 5f73 7472 7563  aycast(bpy_struc
 00182770: 742c 2047 656f 6d65 7472 794e 6f64 652c  t, GeometryNode,
-00182780: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-00182790: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+00182780: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+00182790: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 001827a0: 4361 7374 2072 6179 7320 6672 6f6d 2074  Cast rays from t
 001827b0: 6865 2063 6f6e 7465 7874 2067 656f 6d65  he context geome
 001827c0: 7472 7920 6f6e 746f 2061 2074 6172 6765  try onto a targe
 001827d0: 7420 6765 6f6d 6574 7279 2c20 616e 6420  t geometry, and 
 001827e0: 7265 7472 6965 7665 2069 6e66 6f72 6d61  retrieve informa
 001827f0: 7469 6f6e 2066 726f 6d20 6561 6368 2068  tion from each h
 00182800: 6974 2070 6f69 6e74 0a0a 2020 2222 220a  it point..  """.
@@ -99003,16 +99003,16 @@
 00182ba0: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 00182bb0: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 00182bc0: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 00182bd0: 2e2e 0a0a 636c 6173 7320 4765 6f6d 6574  ....class Geomet
 00182be0: 7279 4e6f 6465 5265 616c 697a 6549 6e73  ryNodeRealizeIns
 00182bf0: 7461 6e63 6573 2862 7079 5f73 7472 7563  tances(bpy_struc
 00182c00: 742c 2047 656f 6d65 7472 794e 6f64 652c  t, GeometryNode,
-00182c10: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-00182c20: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+00182c10: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+00182c20: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 00182c30: 436f 6e76 6572 7420 696e 7374 616e 6365  Convert instance
 00182c40: 7320 696e 746f 2072 6561 6c20 6765 6f6d  s into real geom
 00182c50: 6574 7279 2064 6174 610a 0a20 2022 2222  etry data..  """
 00182c60: 0a0a 2020 6c65 6761 6379 5f62 6568 6176  ..  legacy_behav
 00182c70: 696f 723a 2062 6f6f 6c20 3d20 2e2e 2e0a  ior: bool = ....
 00182c80: 0a20 2022 2222 0a0a 2020 4265 6861 7665  .  """..  Behave
 00182c90: 206c 696b 6520 6265 666f 7265 2069 6e73   like before ins
@@ -99057,15 +99057,15 @@
 00182f00: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 00182f10: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 00182f20: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 00182f30: 0a63 6c61 7373 2047 656f 6d65 7472 794e  .class GeometryN
 00182f40: 6f64 6552 656d 6f76 6541 7474 7269 6275  odeRemoveAttribu
 00182f50: 7465 2862 7079 5f73 7472 7563 742c 2047  te(bpy_struct, G
 00182f60: 656f 6d65 7472 794e 6f64 652c 204e 6f64  eometryNode, Nod
-00182f70: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+00182f70: 6549 6e74 6572 6e61 6c2c 204e 6f64 6529  eInternal, Node)
 00182f80: 3a0a 0a20 2022 2222 0a0a 2020 4465 6c65  :..  """..  Dele
 00182f90: 7465 2061 6e20 6174 7472 6962 7574 6520  te an attribute 
 00182fa0: 7769 7468 2061 2073 7065 6369 6669 6564  with a specified
 00182fb0: 206e 616d 6520 6672 6f6d 2061 2067 656f   name from a geo
 00182fc0: 6d65 7472 792e 2054 7970 6963 616c 6c79  metry. Typically
 00182fd0: 2075 7365 6420 746f 206f 7074 696d 697a   used to optimiz
 00182fe0: 6520 7065 7266 6f72 6d61 6e63 650a 0a20  e performance.. 
@@ -99108,16 +99108,16 @@
 00183230: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 00183240: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 00183250: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 00183260: 202e 2e2e 0a0a 636c 6173 7320 4765 6f6d   .....class Geom
 00183270: 6574 7279 4e6f 6465 5265 706c 6163 654d  etryNodeReplaceM
 00183280: 6174 6572 6961 6c28 6270 795f 7374 7275  aterial(bpy_stru
 00183290: 6374 2c20 4765 6f6d 6574 7279 4e6f 6465  ct, GeometryNode
-001832a0: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-001832b0: 726e 616c 293a 0a0a 2020 2222 220a 0a20  rnal):..  """.. 
+001832a0: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+001832b0: 4e6f 6465 293a 0a0a 2020 2222 220a 0a20  Node):..  """.. 
 001832c0: 2053 7761 7020 6f6e 6520 6d61 7465 7269   Swap one materi
 001832d0: 616c 2077 6974 6820 616e 6f74 6865 720a  al with another.
 001832e0: 0a20 2022 2222 0a0a 2020 4063 6c61 7373  .  """..  @class
 001832f0: 6d65 7468 6f64 0a0a 2020 6465 6620 6973  method..  def is
 00183300: 5f72 6567 6973 7465 7265 645f 6e6f 6465  _registered_node
 00183310: 5f74 7970 6528 636c 7329 202d 3e20 626f  _type(cls) -> bo
 00183320: 6f6c 3a0a 0a20 2020 2022 2222 0a0a 2020  ol:..    """..  
@@ -99155,16 +99155,16 @@
 00183520: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 00183530: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 00183540: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 00183550: 2020 202e 2e2e 0a0a 636c 6173 7320 4765     .....class Ge
 00183560: 6f6d 6574 7279 4e6f 6465 5265 7361 6d70  ometryNodeResamp
 00183570: 6c65 4375 7276 6528 6270 795f 7374 7275  leCurve(bpy_stru
 00183580: 6374 2c20 4765 6f6d 6574 7279 4e6f 6465  ct, GeometryNode
-00183590: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-001835a0: 726e 616c 293a 0a0a 2020 2222 220a 0a20  rnal):..  """.. 
+00183590: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+001835a0: 4e6f 6465 293a 0a0a 2020 2222 220a 0a20  Node):..  """.. 
 001835b0: 2047 656e 6572 6174 6520 6120 706f 6c79   Generate a poly
 001835c0: 2073 706c 696e 6520 666f 7220 6561 6368   spline for each
 001835d0: 2069 6e70 7574 2073 706c 696e 650a 0a20   input spline.. 
 001835e0: 2022 2222 0a0a 2020 6d6f 6465 3a20 7374   """..  mode: st
 001835f0: 7220 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  r = .....  """..
 00183600: 2020 486f 7720 746f 2073 7065 6369 6679    How to specify
 00183610: 2074 6865 2061 6d6f 756e 7420 6f66 2073   the amount of s
@@ -99231,15 +99231,15 @@
 001839e0: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 001839f0: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 00183a00: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 00183a10: 2e2e 0a0a 636c 6173 7320 4765 6f6d 6574  ....class Geomet
 00183a20: 7279 4e6f 6465 5265 7665 7273 6543 7572  ryNodeReverseCur
 00183a30: 7665 2862 7079 5f73 7472 7563 742c 2047  ve(bpy_struct, G
 00183a40: 656f 6d65 7472 794e 6f64 652c 204e 6f64  eometryNode, Nod
-00183a50: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+00183a50: 6549 6e74 6572 6e61 6c2c 204e 6f64 6529  eInternal, Node)
 00183a60: 3a0a 0a20 2022 2222 0a0a 2020 4368 616e  :..  """..  Chan
 00183a70: 6765 2074 6865 2064 6972 6563 7469 6f6e  ge the direction
 00183a80: 206f 6620 6375 7276 6573 2062 7920 7377   of curves by sw
 00183a90: 6170 7069 6e67 2074 6865 6972 2073 7461  apping their sta
 00183aa0: 7274 2061 6e64 2065 6e64 2064 6174 610a  rt and end data.
 00183ab0: 0a20 2022 2222 0a0a 2020 4063 6c61 7373  .  """..  @class
 00183ac0: 6d65 7468 6f64 0a0a 2020 6465 6620 6973  method..  def is
@@ -99280,16 +99280,16 @@
 00183cf0: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 00183d00: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 00183d10: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 00183d20: 2020 202e 2e2e 0a0a 636c 6173 7320 4765     .....class Ge
 00183d30: 6f6d 6574 7279 4e6f 6465 526f 7461 7465  ometryNodeRotate
 00183d40: 496e 7374 616e 6365 7328 6270 795f 7374  Instances(bpy_st
 00183d50: 7275 6374 2c20 4765 6f6d 6574 7279 4e6f  ruct, GeometryNo
-00183d60: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-00183d70: 7465 726e 616c 293a 0a0a 2020 2222 220a  ternal):..  """.
+00183d60: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+00183d70: 2c20 4e6f 6465 293a 0a0a 2020 2222 220a  , Node):..  """.
 00183d80: 0a20 2052 6f74 6174 6520 6765 6f6d 6574  .  Rotate geomet
 00183d90: 7279 2069 6e73 7461 6e63 6573 2069 6e20  ry instances in 
 00183da0: 6c6f 6361 6c20 6f72 2067 6c6f 6261 6c20  local or global 
 00183db0: 7370 6163 650a 0a20 2022 2222 0a0a 2020  space..  """..  
 00183dc0: 4063 6c61 7373 6d65 7468 6f64 0a0a 2020  @classmethod..  
 00183dd0: 6465 6620 6973 5f72 6567 6973 7465 7265  def is_registere
 00183de0: 645f 6e6f 6465 5f74 7970 6528 636c 7329  d_node_type(cls)
@@ -99328,16 +99328,16 @@
 00183ff0: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 00184000: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 00184010: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 00184020: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 00184030: 6173 7320 4765 6f6d 6574 7279 4e6f 6465  ass GeometryNode
 00184040: 5344 4656 6f6c 756d 6553 7068 6572 6528  SDFVolumeSphere(
 00184050: 6270 795f 7374 7275 6374 2c20 4765 6f6d  bpy_struct, Geom
-00184060: 6574 7279 4e6f 6465 2c20 4e6f 6465 2c20  etryNode, Node, 
-00184070: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+00184060: 6574 7279 4e6f 6465 2c20 4e6f 6465 496e  etryNode, NodeIn
+00184070: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 00184080: 2020 2222 220a 0a20 2047 656e 6572 6174    """..  Generat
 00184090: 6520 616e 2053 4446 2056 6f6c 756d 6520  e an SDF Volume 
 001840a0: 5370 6865 7265 0a0a 2020 2222 220a 0a20  Sphere..  """.. 
 001840b0: 2040 636c 6173 736d 6574 686f 640a 0a20   @classmethod.. 
 001840c0: 2064 6566 2069 735f 7265 6769 7374 6572   def is_register
 001840d0: 6564 5f6e 6f64 655f 7479 7065 2863 6c73  ed_node_type(cls
 001840e0: 2920 2d3e 2062 6f6f 6c3a 0a0a 2020 2020  ) -> bool:..    
@@ -99375,16 +99375,16 @@
 001842e0: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 001842f0: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 00184300: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 00184310: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 00184320: 6c61 7373 2047 656f 6d65 7472 794e 6f64  lass GeometryNod
 00184330: 6553 616d 706c 6543 7572 7665 2862 7079  eSampleCurve(bpy
 00184340: 5f73 7472 7563 742c 2047 656f 6d65 7472  _struct, Geometr
-00184350: 794e 6f64 652c 204e 6f64 652c 204e 6f64  yNode, Node, Nod
-00184360: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2022  eInternal):..  "
+00184350: 794e 6f64 652c 204e 6f64 6549 6e74 6572  yNode, NodeInter
+00184360: 6e61 6c2c 204e 6f64 6529 3a0a 0a20 2022  nal, Node):..  "
 00184370: 2222 0a0a 2020 5265 7472 6965 7665 2064  ""..  Retrieve d
 00184380: 6174 6120 6672 6f6d 2061 2070 6f69 6e74  ata from a point
 00184390: 206f 6e20 6120 6375 7276 6520 6174 2061   on a curve at a
 001843a0: 2063 6572 7461 696e 2064 6973 7461 6e63   certain distanc
 001843b0: 6520 6672 6f6d 2069 7473 2073 7461 7274  e from its start
 001843c0: 0a0a 2020 2222 220a 0a20 2064 6174 615f  ..  """..  data_
 001843d0: 7479 7065 3a20 7374 7220 3d20 2e2e 2e0a  type: str = ....
@@ -99452,16 +99452,16 @@
 001847b0: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 001847c0: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 001847d0: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 001847e0: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 001847f0: 6c61 7373 2047 656f 6d65 7472 794e 6f64  lass GeometryNod
 00184800: 6553 616d 706c 6549 6e64 6578 2862 7079  eSampleIndex(bpy
 00184810: 5f73 7472 7563 742c 2047 656f 6d65 7472  _struct, Geometr
-00184820: 794e 6f64 652c 204e 6f64 652c 204e 6f64  yNode, Node, Nod
-00184830: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2022  eInternal):..  "
+00184820: 794e 6f64 652c 204e 6f64 6549 6e74 6572  yNode, NodeInter
+00184830: 6e61 6c2c 204e 6f64 6529 3a0a 0a20 2022  nal, Node):..  "
 00184840: 2222 0a0a 2020 5265 7472 6965 7665 2076  ""..  Retrieve v
 00184850: 616c 7565 7320 6672 6f6d 2073 7065 6369  alues from speci
 00184860: 6669 6320 6765 6f6d 6574 7279 2065 6c65  fic geometry ele
 00184870: 6d65 6e74 730a 0a20 2022 2222 0a0a 2020  ments..  """..  
 00184880: 636c 616d 703a 2062 6f6f 6c20 3d20 2e2e  clamp: bool = ..
 00184890: 2e0a 0a20 2022 2222 0a0a 2020 436c 616d  ...  """..  Clam
 001848a0: 7020 7468 6520 696e 6469 6365 7320 746f  p the indices to
@@ -99512,16 +99512,16 @@
 00184b70: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 00184b80: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 00184b90: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 00184ba0: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 00184bb0: 0a63 6c61 7373 2047 656f 6d65 7472 794e  .class GeometryN
 00184bc0: 6f64 6553 616d 706c 654e 6561 7265 7374  odeSampleNearest
 00184bd0: 2862 7079 5f73 7472 7563 742c 2047 656f  (bpy_struct, Geo
-00184be0: 6d65 7472 794e 6f64 652c 204e 6f64 652c  metryNode, Node,
-00184bf0: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+00184be0: 6d65 7472 794e 6f64 652c 204e 6f64 6549  metryNode, NodeI
+00184bf0: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 00184c00: 0a20 2022 2222 0a0a 2020 4669 6e64 2074  .  """..  Find t
 00184c10: 6865 2065 6c65 6d65 6e74 206f 6620 6120  he element of a 
 00184c20: 6765 6f6d 6574 7279 2063 6c6f 7365 7374  geometry closest
 00184c30: 2074 6f20 6120 706f 7369 7469 6f6e 0a0a   to a position..
 00184c40: 2020 2222 220a 0a20 2064 6f6d 6169 6e3a    """..  domain:
 00184c50: 2073 7472 203d 202e 2e2e 0a0a 2020 4063   str = .....  @c
 00184c60: 6c61 7373 6d65 7468 6f64 0a0a 2020 6465  lassmethod..  de
@@ -99563,15 +99563,15 @@
 00184ea0: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 00184eb0: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 00184ec0: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 00184ed0: 7320 4765 6f6d 6574 7279 4e6f 6465 5361  s GeometryNodeSa
 00184ee0: 6d70 6c65 4e65 6172 6573 7453 7572 6661  mpleNearestSurfa
 00184ef0: 6365 2862 7079 5f73 7472 7563 742c 2047  ce(bpy_struct, G
 00184f00: 656f 6d65 7472 794e 6f64 652c 204e 6f64  eometryNode, Nod
-00184f10: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+00184f10: 6549 6e74 6572 6e61 6c2c 204e 6f64 6529  eInternal, Node)
 00184f20: 3a0a 0a20 2022 2222 0a0a 2020 4361 6c63  :..  """..  Calc
 00184f30: 756c 6174 6520 7468 6520 696e 7465 7270  ulate the interp
 00184f40: 6f6c 6174 6564 2076 616c 7565 206f 6620  olated value of 
 00184f50: 6120 6d65 7368 2061 7474 7269 6275 7465  a mesh attribute
 00184f60: 206f 6e20 7468 6520 636c 6f73 6573 7420   on the closest 
 00184f70: 706f 696e 7420 6f66 2069 7473 2073 7572  point of its sur
 00184f80: 6661 6365 0a0a 2020 2222 220a 0a20 2064  face..  """..  d
@@ -99615,16 +99615,16 @@
 001851e0: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 001851f0: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 00185200: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 00185210: 2e2e 2e0a 0a63 6c61 7373 2047 656f 6d65  .....class Geome
 00185220: 7472 794e 6f64 6553 616d 706c 6555 5653  tryNodeSampleUVS
 00185230: 7572 6661 6365 2862 7079 5f73 7472 7563  urface(bpy_struc
 00185240: 742c 2047 656f 6d65 7472 794e 6f64 652c  t, GeometryNode,
-00185250: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-00185260: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+00185250: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+00185260: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 00185270: 4361 6c63 756c 6174 6520 7468 6520 696e  Calculate the in
 00185280: 7465 7270 6f6c 6174 6564 2076 616c 7565  terpolated value
 00185290: 7320 6f66 2061 206d 6573 6820 6174 7472  s of a mesh attr
 001852a0: 6962 7574 6520 6174 2061 2055 5620 636f  ibute at a UV co
 001852b0: 6f72 6469 6e61 7465 0a0a 2020 2222 220a  ordinate..  """.
 001852c0: 0a20 2064 6174 615f 7479 7065 3a20 7374  .  data_type: st
 001852d0: 7220 3d20 2e2e 2e0a 0a20 2040 636c 6173  r = .....  @clas
@@ -99666,16 +99666,16 @@
 00185510: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 00185520: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 00185530: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 00185540: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2047      .....class G
 00185550: 656f 6d65 7472 794e 6f64 6553 6361 6c65  eometryNodeScale
 00185560: 456c 656d 656e 7473 2862 7079 5f73 7472  Elements(bpy_str
 00185570: 7563 742c 2047 656f 6d65 7472 794e 6f64  uct, GeometryNod
-00185580: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-00185590: 6572 6e61 6c29 3a0a 0a20 2022 2222 0a0a  ernal):..  """..
+00185580: 652c 204e 6f64 6549 6e74 6572 6e61 6c2c  e, NodeInternal,
+00185590: 204e 6f64 6529 3a0a 0a20 2022 2222 0a0a   Node):..  """..
 001855a0: 2020 5363 616c 6520 6772 6f75 7073 206f    Scale groups o
 001855b0: 6620 636f 6e6e 6563 7465 6420 6564 6765  f connected edge
 001855c0: 7320 616e 6420 6661 6365 730a 0a20 2022  s and faces..  "
 001855d0: 2222 0a0a 2020 646f 6d61 696e 3a20 7374  ""..  domain: st
 001855e0: 7220 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  r = .....  """..
 001855f0: 2020 456c 656d 656e 7420 7479 7065 2074    Element type t
 00185600: 6f20 7472 616e 7366 6f72 6d0a 0a20 202a  o transform..  *
@@ -99739,16 +99739,16 @@
 001859a0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 001859b0: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 001859c0: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 001859d0: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 001859e0: 2047 656f 6d65 7472 794e 6f64 6553 6361   GeometryNodeSca
 001859f0: 6c65 496e 7374 616e 6365 7328 6270 795f  leInstances(bpy_
 00185a00: 7374 7275 6374 2c20 4765 6f6d 6574 7279  struct, Geometry
-00185a10: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-00185a20: 496e 7465 726e 616c 293a 0a0a 2020 2222  Internal):..  ""
+00185a10: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
+00185a20: 616c 2c20 4e6f 6465 293a 0a0a 2020 2222  al, Node):..  ""
 00185a30: 220a 0a20 2053 6361 6c65 2067 656f 6d65  "..  Scale geome
 00185a40: 7472 7920 696e 7374 616e 6365 7320 696e  try instances in
 00185a50: 206c 6f63 616c 206f 7220 676c 6f62 616c   local or global
 00185a60: 2073 7061 6365 0a0a 2020 2222 220a 0a20   space..  """.. 
 00185a70: 2040 636c 6173 736d 6574 686f 640a 0a20   @classmethod.. 
 00185a80: 2064 6566 2069 735f 7265 6769 7374 6572   def is_register
 00185a90: 6564 5f6e 6f64 655f 7479 7065 2863 6c73  ed_node_type(cls
@@ -99787,16 +99787,16 @@
 00185ca0: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 00185cb0: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 00185cc0: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 00185cd0: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 00185ce0: 6c61 7373 2047 656f 6d65 7472 794e 6f64  lass GeometryNod
 00185cf0: 6553 656c 664f 626a 6563 7428 6270 795f  eSelfObject(bpy_
 00185d00: 7374 7275 6374 2c20 4765 6f6d 6574 7279  struct, Geometry
-00185d10: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-00185d20: 496e 7465 726e 616c 293a 0a0a 2020 2222  Internal):..  ""
+00185d10: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
+00185d20: 616c 2c20 4e6f 6465 293a 0a0a 2020 2222  al, Node):..  ""
 00185d30: 220a 0a20 2052 6574 7269 6576 6520 7468  "..  Retrieve th
 00185d40: 6520 6f62 6a65 6374 2074 6861 7420 636f  e object that co
 00185d50: 6e74 6169 6e73 2074 6865 2067 656f 6d65  ntains the geome
 00185d60: 7472 7920 6e6f 6465 7320 6d6f 6469 6669  try nodes modifi
 00185d70: 6572 2063 7572 7265 6e74 6c79 2062 6569  er currently bei
 00185d80: 6e67 2065 7865 6375 7465 640a 0a20 2022  ng executed..  "
 00185d90: 2222 0a0a 2020 4063 6c61 7373 6d65 7468  ""..  @classmeth
@@ -99838,16 +99838,16 @@
 00185fd0: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 00185fe0: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 00185ff0: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 00186000: 2e2e 0a0a 636c 6173 7320 4765 6f6d 6574  ....class Geomet
 00186010: 7279 4e6f 6465 5365 7061 7261 7465 436f  ryNodeSeparateCo
 00186020: 6d70 6f6e 656e 7473 2862 7079 5f73 7472  mponents(bpy_str
 00186030: 7563 742c 2047 656f 6d65 7472 794e 6f64  uct, GeometryNod
-00186040: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-00186050: 6572 6e61 6c29 3a0a 0a20 2022 2222 0a0a  ernal):..  """..
+00186040: 652c 204e 6f64 6549 6e74 6572 6e61 6c2c  e, NodeInternal,
+00186050: 204e 6f64 6529 3a0a 0a20 2022 2222 0a0a   Node):..  """..
 00186060: 2020 5370 6c69 7420 6120 6765 6f6d 6574    Split a geomet
 00186070: 7279 2069 6e74 6f20 6120 7365 7061 7261  ry into a separa
 00186080: 7465 206f 7574 7075 7420 666f 7220 6561  te output for ea
 00186090: 6368 2074 7970 6520 6f66 2064 6174 6120  ch type of data 
 001860a0: 696e 2074 6865 2067 656f 6d65 7472 790a  in the geometry.
 001860b0: 0a20 2022 2222 0a0a 2020 4063 6c61 7373  .  """..  @class
 001860c0: 6d65 7468 6f64 0a0a 2020 6465 6620 6973  method..  def is
@@ -99888,16 +99888,16 @@
 001862f0: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 00186300: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 00186310: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 00186320: 2020 202e 2e2e 0a0a 636c 6173 7320 4765     .....class Ge
 00186330: 6f6d 6574 7279 4e6f 6465 5365 7061 7261  ometryNodeSepara
 00186340: 7465 4765 6f6d 6574 7279 2862 7079 5f73  teGeometry(bpy_s
 00186350: 7472 7563 742c 2047 656f 6d65 7472 794e  truct, GeometryN
-00186360: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-00186370: 6e74 6572 6e61 6c29 3a0a 0a20 2022 2222  nternal):..  """
+00186360: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
+00186370: 6c2c 204e 6f64 6529 3a0a 0a20 2022 2222  l, Node):..  """
 00186380: 0a0a 2020 5370 6c69 7420 6120 6765 6f6d  ..  Split a geom
 00186390: 6574 7279 2069 6e74 6f20 7477 6f20 6765  etry into two ge
 001863a0: 6f6d 6574 7279 206f 7574 7075 7473 2062  ometry outputs b
 001863b0: 6173 6564 206f 6e20 6120 7365 6c65 6374  ased on a select
 001863c0: 696f 6e0a 0a20 2022 2222 0a0a 2020 646f  ion..  """..  do
 001863d0: 6d61 696e 3a20 7374 7220 3d20 2e2e 2e0a  main: str = ....
 001863e0: 0a20 2022 2222 0a0a 2020 5768 6963 6820  .  """..  Which 
@@ -99942,16 +99942,16 @@
 00186650: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 00186660: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 00186670: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 00186680: 6173 7320 4765 6f6d 6574 7279 4e6f 6465  ass GeometryNode
 00186690: 5365 7443 7572 7665 4861 6e64 6c65 506f  SetCurveHandlePo
 001866a0: 7369 7469 6f6e 7328 6270 795f 7374 7275  sitions(bpy_stru
 001866b0: 6374 2c20 4765 6f6d 6574 7279 4e6f 6465  ct, GeometryNode
-001866c0: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-001866d0: 726e 616c 293a 0a0a 2020 2222 220a 0a20  rnal):..  """.. 
+001866c0: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+001866d0: 4e6f 6465 293a 0a0a 2020 2222 220a 0a20  Node):..  """.. 
 001866e0: 2053 6574 2074 6865 2070 6f73 6974 696f   Set the positio
 001866f0: 6e73 2066 6f72 2074 6865 2068 616e 646c  ns for the handl
 00186700: 6573 206f 6620 42c3 a97a 6965 7220 6375  es of B..zier cu
 00186710: 7276 6573 0a0a 2020 2222 220a 0a20 206d  rves..  """..  m
 00186720: 6f64 653a 2073 7472 203d 202e 2e2e 0a0a  ode: str = .....
 00186730: 2020 2222 220a 0a20 2057 6865 7468 6572    """..  Whether
 00186740: 2074 6f20 7570 6461 7465 206c 6566 7420   to update left 
@@ -100001,16 +100001,16 @@
 00186a00: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 00186a10: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 00186a20: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 00186a30: 2e2e 2e0a 0a63 6c61 7373 2047 656f 6d65  .....class Geome
 00186a40: 7472 794e 6f64 6553 6574 4375 7276 654e  tryNodeSetCurveN
 00186a50: 6f72 6d61 6c28 6270 795f 7374 7275 6374  ormal(bpy_struct
 00186a60: 2c20 4765 6f6d 6574 7279 4e6f 6465 2c20  , GeometryNode, 
-00186a70: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-00186a80: 616c 293a 0a0a 2020 2222 220a 0a20 2053  al):..  """..  S
+00186a70: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+00186a80: 6465 293a 0a0a 2020 2222 220a 0a20 2053  de):..  """..  S
 00186a90: 6574 2074 6865 2065 7661 6c75 6174 696f  et the evaluatio
 00186aa0: 6e20 6d6f 6465 2066 6f72 2063 7572 7665  n mode for curve
 00186ab0: 206e 6f72 6d61 6c73 0a0a 2020 2222 220a   normals..  """.
 00186ac0: 0a20 206d 6f64 653a 2073 7472 203d 202e  .  mode: str = .
 00186ad0: 2e2e 0a0a 2020 2222 220a 0a20 204d 6f64  ....  """..  Mod
 00186ae0: 6520 666f 7220 6375 7276 6520 6e6f 726d  e for curve norm
 00186af0: 616c 2065 7661 6c75 6174 696f 6e0a 0a20  al evaluation.. 
@@ -100053,16 +100053,16 @@
 00186d40: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 00186d50: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 00186d60: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 00186d70: 202e 2e2e 0a0a 636c 6173 7320 4765 6f6d   .....class Geom
 00186d80: 6574 7279 4e6f 6465 5365 7443 7572 7665  etryNodeSetCurve
 00186d90: 5261 6469 7573 2862 7079 5f73 7472 7563  Radius(bpy_struc
 00186da0: 742c 2047 656f 6d65 7472 794e 6f64 652c  t, GeometryNode,
-00186db0: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-00186dc0: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+00186db0: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+00186dc0: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 00186dd0: 5365 7420 7468 6520 7261 6469 7573 206f  Set the radius o
 00186de0: 6620 7468 6520 6375 7276 6520 6174 2065  f the curve at e
 00186df0: 6163 6820 636f 6e74 726f 6c20 706f 696e  ach control poin
 00186e00: 740a 0a20 2022 2222 0a0a 2020 4063 6c61  t..  """..  @cla
 00186e10: 7373 6d65 7468 6f64 0a0a 2020 6465 6620  ssmethod..  def 
 00186e20: 6973 5f72 6567 6973 7465 7265 645f 6e6f  is_registered_no
 00186e30: 6465 5f74 7970 6528 636c 7329 202d 3e20  de_type(cls) -> 
@@ -100101,16 +100101,16 @@
 00187040: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 00187050: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 00187060: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 00187070: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 00187080: 4765 6f6d 6574 7279 4e6f 6465 5365 7443  GeometryNodeSetC
 00187090: 7572 7665 5469 6c74 2862 7079 5f73 7472  urveTilt(bpy_str
 001870a0: 7563 742c 2047 656f 6d65 7472 794e 6f64  uct, GeometryNod
-001870b0: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-001870c0: 6572 6e61 6c29 3a0a 0a20 2022 2222 0a0a  ernal):..  """..
+001870b0: 652c 204e 6f64 6549 6e74 6572 6e61 6c2c  e, NodeInternal,
+001870c0: 204e 6f64 6529 3a0a 0a20 2022 2222 0a0a   Node):..  """..
 001870d0: 2020 5365 7420 7468 6520 7469 6c74 2061    Set the tilt a
 001870e0: 6e67 6c65 2061 7420 6561 6368 2063 7572  ngle at each cur
 001870f0: 7665 2063 6f6e 7472 6f6c 2070 6f69 6e74  ve control point
 00187100: 0a0a 2020 2222 220a 0a20 2040 636c 6173  ..  """..  @clas
 00187110: 736d 6574 686f 640a 0a20 2064 6566 2069  smethod..  def i
 00187120: 735f 7265 6769 7374 6572 6564 5f6e 6f64  s_registered_nod
 00187130: 655f 7479 7065 2863 6c73 2920 2d3e 2062  e_type(cls) -> b
@@ -100148,16 +100148,16 @@
 00187330: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 00187340: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 00187350: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 00187360: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 00187370: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2047      .....class G
 00187380: 656f 6d65 7472 794e 6f64 6553 6574 4944  eometryNodeSetID
 00187390: 2862 7079 5f73 7472 7563 742c 2047 656f  (bpy_struct, Geo
-001873a0: 6d65 7472 794e 6f64 652c 204e 6f64 652c  metryNode, Node,
-001873b0: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+001873a0: 6d65 7472 794e 6f64 652c 204e 6f64 6549  metryNode, NodeI
+001873b0: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 001873c0: 0a20 2022 2222 0a0a 2020 5365 7420 7468  .  """..  Set th
 001873d0: 6520 6964 2061 7474 7269 6275 7465 206f  e id attribute o
 001873e0: 6e20 7468 6520 696e 7075 7420 6765 6f6d  n the input geom
 001873f0: 6574 7279 2c20 6d61 696e 6c79 2075 7365  etry, mainly use
 00187400: 6420 696e 7465 726e 616c 6c79 2066 6f72  d internally for
 00187410: 2072 616e 646f 6d69 7a69 6e67 0a0a 2020   randomizing..  
 00187420: 2222 220a 0a20 2040 636c 6173 736d 6574  """..  @classmet
@@ -100199,15 +100199,15 @@
 00187660: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 00187670: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 00187680: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 00187690: 2e2e 2e0a 0a63 6c61 7373 2047 656f 6d65  .....class Geome
 001876a0: 7472 794e 6f64 6553 6574 4d61 7465 7269  tryNodeSetMateri
 001876b0: 616c 2862 7079 5f73 7472 7563 742c 2047  al(bpy_struct, G
 001876c0: 656f 6d65 7472 794e 6f64 652c 204e 6f64  eometryNode, Nod
-001876d0: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+001876d0: 6549 6e74 6572 6e61 6c2c 204e 6f64 6529  eInternal, Node)
 001876e0: 3a0a 0a20 2022 2222 0a0a 2020 4173 7369  :..  """..  Assi
 001876f0: 676e 2061 206d 6174 6572 6961 6c20 746f  gn a material to
 00187700: 2067 656f 6d65 7472 7920 656c 656d 656e   geometry elemen
 00187710: 7473 0a0a 2020 2222 220a 0a20 2040 636c  ts..  """..  @cl
 00187720: 6173 736d 6574 686f 640a 0a20 2064 6566  assmethod..  def
 00187730: 2069 735f 7265 6769 7374 6572 6564 5f6e   is_registered_n
 00187740: 6f64 655f 7479 7065 2863 6c73 2920 2d3e  ode_type(cls) ->
@@ -100246,16 +100246,16 @@
 00187950: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 00187960: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 00187970: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 00187980: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 00187990: 2047 656f 6d65 7472 794e 6f64 6553 6574   GeometryNodeSet
 001879a0: 4d61 7465 7269 616c 496e 6465 7828 6270  MaterialIndex(bp
 001879b0: 795f 7374 7275 6374 2c20 4765 6f6d 6574  y_struct, Geomet
-001879c0: 7279 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  ryNode, Node, No
-001879d0: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+001879c0: 7279 4e6f 6465 2c20 4e6f 6465 496e 7465  ryNode, NodeInte
+001879d0: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 001879e0: 2222 220a 0a20 2053 6574 2074 6865 206d  """..  Set the m
 001879f0: 6174 6572 6961 6c20 696e 6465 7820 666f  aterial index fo
 00187a00: 7220 6561 6368 2073 656c 6563 7465 6420  r each selected 
 00187a10: 6765 6f6d 6574 7279 2065 6c65 6d65 6e74  geometry element
 00187a20: 0a0a 2020 2222 220a 0a20 2040 636c 6173  ..  """..  @clas
 00187a30: 736d 6574 686f 640a 0a20 2064 6566 2069  smethod..  def i
 00187a40: 735f 7265 6769 7374 6572 6564 5f6e 6f64  s_registered_nod
@@ -100295,16 +100295,16 @@
 00187c60: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 00187c70: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 00187c80: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 00187c90: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2047      .....class G
 00187ca0: 656f 6d65 7472 794e 6f64 6553 6574 506f  eometryNodeSetPo
 00187cb0: 696e 7452 6164 6975 7328 6270 795f 7374  intRadius(bpy_st
 00187cc0: 7275 6374 2c20 4765 6f6d 6574 7279 4e6f  ruct, GeometryNo
-00187cd0: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-00187ce0: 7465 726e 616c 293a 0a0a 2020 2222 220a  ternal):..  """.
+00187cd0: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+00187ce0: 2c20 4e6f 6465 293a 0a0a 2020 2222 220a  , Node):..  """.
 00187cf0: 0a20 2053 6574 2074 6865 2064 6973 706c  .  Set the displ
 00187d00: 6179 2073 697a 6520 6f66 2070 6f69 6e74  ay size of point
 00187d10: 2063 6c6f 7564 2070 6f69 6e74 730a 0a20   cloud points.. 
 00187d20: 2022 2222 0a0a 2020 4063 6c61 7373 6d65   """..  @classme
 00187d30: 7468 6f64 0a0a 2020 6465 6620 6973 5f72  thod..  def is_r
 00187d40: 6567 6973 7465 7265 645f 6e6f 6465 5f74  egistered_node_t
 00187d50: 7970 6528 636c 7329 202d 3e20 626f 6f6c  ype(cls) -> bool
@@ -100343,15 +100343,15 @@
 00187f60: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 00187f70: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 00187f80: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 00187f90: 202e 2e2e 0a0a 636c 6173 7320 4765 6f6d   .....class Geom
 00187fa0: 6574 7279 4e6f 6465 5365 7450 6f73 6974  etryNodeSetPosit
 00187fb0: 696f 6e28 6270 795f 7374 7275 6374 2c20  ion(bpy_struct, 
 00187fc0: 4765 6f6d 6574 7279 4e6f 6465 2c20 4e6f  GeometryNode, No
-00187fd0: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+00187fd0: 6465 496e 7465 726e 616c 2c20 4e6f 6465  deInternal, Node
 00187fe0: 293a 0a0a 2020 2222 220a 0a20 2053 6574  ):..  """..  Set
 00187ff0: 2074 6865 206c 6f63 6174 696f 6e20 6f66   the location of
 00188000: 2065 6163 6820 706f 696e 740a 0a20 2022   each point..  "
 00188010: 2222 0a0a 2020 4063 6c61 7373 6d65 7468  ""..  @classmeth
 00188020: 6f64 0a0a 2020 6465 6620 6973 5f72 6567  od..  def is_reg
 00188030: 6973 7465 7265 645f 6e6f 6465 5f74 7970  istered_node_typ
 00188040: 6528 636c 7329 202d 3e20 626f 6f6c 3a0a  e(cls) -> bool:.
@@ -100390,16 +100390,16 @@
 00188250: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 00188260: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 00188270: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 00188280: 2e2e 0a0a 636c 6173 7320 4765 6f6d 6574  ....class Geomet
 00188290: 7279 4e6f 6465 5365 7453 6861 6465 536d  ryNodeSetShadeSm
 001882a0: 6f6f 7468 2862 7079 5f73 7472 7563 742c  ooth(bpy_struct,
 001882b0: 2047 656f 6d65 7472 794e 6f64 652c 204e   GeometryNode, N
-001882c0: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-001882d0: 6c29 3a0a 0a20 2022 2222 0a0a 2020 436f  l):..  """..  Co
+001882c0: 6f64 6549 6e74 6572 6e61 6c2c 204e 6f64  odeInternal, Nod
+001882d0: 6529 3a0a 0a20 2022 2222 0a0a 2020 436f  e):..  """..  Co
 001882e0: 6e74 726f 6c20 7468 6520 736d 6f6f 7468  ntrol the smooth
 001882f0: 6e65 7373 206f 6620 6d65 7368 206e 6f72  ness of mesh nor
 00188300: 6d61 6c73 2061 726f 756e 6420 6561 6368  mals around each
 00188310: 2066 6163 6520 6279 2063 6861 6e67 696e   face by changin
 00188320: 6720 7468 6520 2273 6861 6465 2073 6d6f  g the "shade smo
 00188330: 6f74 6822 2061 7474 7269 6275 7465 0a0a  oth" attribute..
 00188340: 2020 2222 220a 0a20 2040 636c 6173 736d    """..  @classm
@@ -100441,16 +100441,16 @@
 00188580: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 00188590: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 001885a0: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 001885b0: 2020 2e2e 2e0a 0a63 6c61 7373 2047 656f    .....class Geo
 001885c0: 6d65 7472 794e 6f64 6553 6574 5370 6c69  metryNodeSetSpli
 001885d0: 6e65 4379 636c 6963 2862 7079 5f73 7472  neCyclic(bpy_str
 001885e0: 7563 742c 2047 656f 6d65 7472 794e 6f64  uct, GeometryNod
-001885f0: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-00188600: 6572 6e61 6c29 3a0a 0a20 2022 2222 0a0a  ernal):..  """..
+001885f0: 652c 204e 6f64 6549 6e74 6572 6e61 6c2c  e, NodeInternal,
+00188600: 204e 6f64 6529 3a0a 0a20 2022 2222 0a0a   Node):..  """..
 00188610: 2020 436f 6e74 726f 6c20 7768 6574 6865    Control whethe
 00188620: 7220 6561 6368 2073 706c 696e 6520 6c6f  r each spline lo
 00188630: 6f70 7320 6261 636b 206f 6e20 6974 7365  ops back on itse
 00188640: 6c66 2062 7920 6368 616e 6769 6e67 2074  lf by changing t
 00188650: 6865 2022 6379 636c 6963 2220 6174 7472  he "cyclic" attr
 00188660: 6962 7574 650a 0a20 2022 2222 0a0a 2020  ibute..  """..  
 00188670: 4063 6c61 7373 6d65 7468 6f64 0a0a 2020  @classmethod..  
@@ -100492,15 +100492,15 @@
 001888b0: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 001888c0: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 001888d0: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 001888e0: 6173 7320 4765 6f6d 6574 7279 4e6f 6465  ass GeometryNode
 001888f0: 5365 7453 706c 696e 6552 6573 6f6c 7574  SetSplineResolut
 00188900: 696f 6e28 6270 795f 7374 7275 6374 2c20  ion(bpy_struct, 
 00188910: 4765 6f6d 6574 7279 4e6f 6465 2c20 4e6f  GeometryNode, No
-00188920: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+00188920: 6465 496e 7465 726e 616c 2c20 4e6f 6465  deInternal, Node
 00188930: 293a 0a0a 2020 2222 220a 0a20 2043 6f6e  ):..  """..  Con
 00188940: 7472 6f6c 2068 6f77 206d 616e 7920 6576  trol how many ev
 00188950: 616c 7561 7465 6420 706f 696e 7473 2073  aluated points s
 00188960: 686f 756c 6420 6265 2067 656e 6572 6174  hould be generat
 00188970: 6564 206f 6e20 6576 6572 7920 6375 7276  ed on every curv
 00188980: 6520 7365 676d 656e 740a 0a20 2022 2222  e segment..  """
 00188990: 0a0a 2020 4063 6c61 7373 6d65 7468 6f64  ..  @classmethod
@@ -100541,16 +100541,16 @@
 00188bc0: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 00188bd0: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 00188be0: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 00188bf0: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 00188c00: 0a0a 636c 6173 7320 4765 6f6d 6574 7279  ..class Geometry
 00188c10: 4e6f 6465 5370 6c69 6e65 4c65 6e67 7468  NodeSplineLength
 00188c20: 2862 7079 5f73 7472 7563 742c 2047 656f  (bpy_struct, Geo
-00188c30: 6d65 7472 794e 6f64 652c 204e 6f64 652c  metryNode, Node,
-00188c40: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+00188c30: 6d65 7472 794e 6f64 652c 204e 6f64 6549  metryNode, NodeI
+00188c40: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 00188c50: 0a20 2022 2222 0a0a 2020 5265 7472 6965  .  """..  Retrie
 00188c60: 7665 2074 6865 2074 6f74 616c 206c 656e  ve the total len
 00188c70: 6774 6820 6f66 2065 6163 6820 7370 6c69  gth of each spli
 00188c80: 6e65 2c20 6173 2061 2064 6973 7461 6e63  ne, as a distanc
 00188c90: 6520 6f72 2061 7320 6120 6e75 6d62 6572  e or as a number
 00188ca0: 206f 6620 706f 696e 7473 0a0a 2020 2222   of points..  ""
 00188cb0: 220a 0a20 2040 636c 6173 736d 6574 686f  "..  @classmetho
@@ -100592,16 +100592,16 @@
 00188ef0: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 00188f00: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 00188f10: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 00188f20: 2e0a 0a63 6c61 7373 2047 656f 6d65 7472  ...class Geometr
 00188f30: 794e 6f64 6553 706c 696e 6550 6172 616d  yNodeSplineParam
 00188f40: 6574 6572 2862 7079 5f73 7472 7563 742c  eter(bpy_struct,
 00188f50: 2047 656f 6d65 7472 794e 6f64 652c 204e   GeometryNode, N
-00188f60: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-00188f70: 6c29 3a0a 0a20 2022 2222 0a0a 2020 5265  l):..  """..  Re
+00188f60: 6f64 6549 6e74 6572 6e61 6c2c 204e 6f64  odeInternal, Nod
+00188f70: 6529 3a0a 0a20 2022 2222 0a0a 2020 5265  e):..  """..  Re
 00188f80: 7472 6965 7665 2068 6f77 2066 6172 2061  trieve how far a
 00188f90: 6c6f 6e67 2065 6163 6820 7370 6c69 6e65  long each spline
 00188fa0: 2061 2063 6f6e 7472 6f6c 2070 6f69 6e74   a control point
 00188fb0: 2069 730a 0a20 2022 2222 0a0a 2020 4063   is..  """..  @c
 00188fc0: 6c61 7373 6d65 7468 6f64 0a0a 2020 6465  lassmethod..  de
 00188fd0: 6620 6973 5f72 6567 6973 7465 7265 645f  f is_registered_
 00188fe0: 6e6f 6465 5f74 7970 6528 636c 7329 202d  node_type(cls) -
@@ -100640,16 +100640,16 @@
 001891f0: 2073 7472 2c20 6465 6661 756c 743a 2074   str, default: t
 00189200: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 00189210: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 00189220: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 00189230: 7320 4765 6f6d 6574 7279 4e6f 6465 5370  s GeometryNodeSp
 00189240: 6c69 7445 6467 6573 2862 7079 5f73 7472  litEdges(bpy_str
 00189250: 7563 742c 2047 656f 6d65 7472 794e 6f64  uct, GeometryNod
-00189260: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-00189270: 6572 6e61 6c29 3a0a 0a20 2022 2222 0a0a  ernal):..  """..
+00189260: 652c 204e 6f64 6549 6e74 6572 6e61 6c2c  e, NodeInternal,
+00189270: 204e 6f64 6529 3a0a 0a20 2022 2222 0a0a   Node):..  """..
 00189280: 2020 4475 706c 6963 6174 6520 6d65 7368    Duplicate mesh
 00189290: 2065 6467 6573 2061 6e64 2062 7265 616b   edges and break
 001892a0: 2063 6f6e 6e65 6374 696f 6e73 2077 6974   connections wit
 001892b0: 6820 7468 6520 7375 7272 6f75 6e64 696e  h the surroundin
 001892c0: 6720 6661 6365 730a 0a20 2022 2222 0a0a  g faces..  """..
 001892d0: 2020 4063 6c61 7373 6d65 7468 6f64 0a0a    @classmethod..
 001892e0: 2020 6465 6620 6973 5f72 6567 6973 7465    def is_registe
@@ -100690,16 +100690,16 @@
 00189510: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 00189520: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 00189530: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 00189540: 636c 6173 7320 4765 6f6d 6574 7279 4e6f  class GeometryNo
 00189550: 6465 5374 6f72 654e 616d 6564 4174 7472  deStoreNamedAttr
 00189560: 6962 7574 6528 6270 795f 7374 7275 6374  ibute(bpy_struct
 00189570: 2c20 4765 6f6d 6574 7279 4e6f 6465 2c20  , GeometryNode, 
-00189580: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-00189590: 616c 293a 0a0a 2020 2222 220a 0a20 2053  al):..  """..  S
+00189580: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+00189590: 6465 293a 0a0a 2020 2222 220a 0a20 2053  de):..  """..  S
 001895a0: 746f 7265 2074 6865 2072 6573 756c 7420  tore the result 
 001895b0: 6f66 2061 2066 6965 6c64 206f 6e20 6120  of a field on a 
 001895c0: 6765 6f6d 6574 7279 2061 7320 616e 2061  geometry as an a
 001895d0: 7474 7269 6275 7465 2077 6974 6820 7468  ttribute with th
 001895e0: 6520 7370 6563 6966 6965 6420 6e61 6d65  e specified name
 001895f0: 0a0a 2020 2222 220a 0a20 2064 6174 615f  ..  """..  data_
 00189600: 7479 7065 3a20 7374 7220 3d20 2e2e 2e0a  type: str = ....
@@ -100749,16 +100749,16 @@
 001898c0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 001898d0: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 001898e0: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 001898f0: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 00189900: 2047 656f 6d65 7472 794e 6f64 6553 7472   GeometryNodeStr
 00189910: 696e 674a 6f69 6e28 6270 795f 7374 7275  ingJoin(bpy_stru
 00189920: 6374 2c20 4765 6f6d 6574 7279 4e6f 6465  ct, GeometryNode
-00189930: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-00189940: 726e 616c 293a 0a0a 2020 2222 220a 0a20  rnal):..  """.. 
+00189930: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+00189940: 4e6f 6465 293a 0a0a 2020 2222 220a 0a20  Node):..  """.. 
 00189950: 2043 6f6d 6269 6e65 2061 6e79 206e 756d   Combine any num
 00189960: 6265 7220 6f66 2069 6e70 7574 2073 7472  ber of input str
 00189970: 696e 6773 0a0a 2020 2222 220a 0a20 2040  ings..  """..  @
 00189980: 636c 6173 736d 6574 686f 640a 0a20 2064  classmethod..  d
 00189990: 6566 2069 735f 7265 6769 7374 6572 6564  ef is_registered
 001899a0: 5f6e 6f64 655f 7479 7065 2863 6c73 2920  _node_type(cls) 
 001899b0: 2d3e 2062 6f6f 6c3a 0a0a 2020 2020 2222  -> bool:..    ""
@@ -100796,16 +100796,16 @@
 00189bb0: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 00189bc0: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 00189bd0: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 00189be0: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 00189bf0: 7373 2047 656f 6d65 7472 794e 6f64 6553  ss GeometryNodeS
 00189c00: 7472 696e 6754 6f43 7572 7665 7328 6270  tringToCurves(bp
 00189c10: 795f 7374 7275 6374 2c20 4765 6f6d 6574  y_struct, Geomet
-00189c20: 7279 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  ryNode, Node, No
-00189c30: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+00189c20: 7279 4e6f 6465 2c20 4e6f 6465 496e 7465  ryNode, NodeInte
+00189c30: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 00189c40: 2222 220a 0a20 2047 656e 6572 6174 6520  """..  Generate 
 00189c50: 6120 7061 7261 6772 6170 6820 6f66 2074  a paragraph of t
 00189c60: 6578 7420 7769 7468 2061 2073 7065 6369  ext with a speci
 00189c70: 6669 6320 666f 6e74 2c20 7573 696e 6720  fic font, using 
 00189c80: 6120 6375 7276 6520 696e 7374 616e 6365  a curve instance
 00189c90: 2074 6f20 7374 6f72 6520 6561 6368 2063   to store each c
 00189ca0: 6861 7261 6374 6572 0a0a 2020 2222 220a  haracter..  """.
@@ -100955,15 +100955,15 @@
 0018a5a0: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 0018a5b0: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 0018a5c0: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 0018a5d0: 2e0a 0a63 6c61 7373 2047 656f 6d65 7472  ...class Geometr
 0018a5e0: 794e 6f64 6553 7562 6469 7669 6465 4375  yNodeSubdivideCu
 0018a5f0: 7276 6528 6270 795f 7374 7275 6374 2c20  rve(bpy_struct, 
 0018a600: 4765 6f6d 6574 7279 4e6f 6465 2c20 4e6f  GeometryNode, No
-0018a610: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+0018a610: 6465 496e 7465 726e 616c 2c20 4e6f 6465  deInternal, Node
 0018a620: 293a 0a0a 2020 2222 220a 0a20 2044 6976  ):..  """..  Div
 0018a630: 6964 696e 6720 6561 6368 2063 7572 7665  iding each curve
 0018a640: 2073 6567 6d65 6e74 2069 6e74 6f20 6120   segment into a 
 0018a650: 7370 6563 6966 6965 6420 6e75 6d62 6572  specified number
 0018a660: 206f 6620 7069 6563 6573 0a0a 2020 2222   of pieces..  ""
 0018a670: 220a 0a20 2040 636c 6173 736d 6574 686f  "..  @classmetho
 0018a680: 640a 0a20 2064 6566 2069 735f 7265 6769  d..  def is_regi
@@ -101004,15 +101004,15 @@
 0018a8b0: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 0018a8c0: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 0018a8d0: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 0018a8e0: 2e0a 0a63 6c61 7373 2047 656f 6d65 7472  ...class Geometr
 0018a8f0: 794e 6f64 6553 7562 6469 7669 6465 4d65  yNodeSubdivideMe
 0018a900: 7368 2862 7079 5f73 7472 7563 742c 2047  sh(bpy_struct, G
 0018a910: 656f 6d65 7472 794e 6f64 652c 204e 6f64  eometryNode, Nod
-0018a920: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+0018a920: 6549 6e74 6572 6e61 6c2c 204e 6f64 6529  eInternal, Node)
 0018a930: 3a0a 0a20 2022 2222 0a0a 2020 4469 7669  :..  """..  Divi
 0018a940: 6465 206d 6573 6820 6661 6365 7320 696e  de mesh faces in
 0018a950: 746f 2073 6d61 6c6c 6572 206f 6e65 7320  to smaller ones 
 0018a960: 7769 7468 6f75 7420 6368 616e 6769 6e67  without changing
 0018a970: 2074 6865 2073 6861 7065 206f 7220 766f   the shape or vo
 0018a980: 6c75 6d65 2c20 7573 696e 6720 6c69 6e65  lume, using line
 0018a990: 6172 2069 6e74 6572 706f 6c61 7469 6f6e  ar interpolation
@@ -101057,16 +101057,16 @@
 0018ac00: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 0018ac10: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 0018ac20: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 0018ac30: 2e0a 0a63 6c61 7373 2047 656f 6d65 7472  ...class Geometr
 0018ac40: 794e 6f64 6553 7562 6469 7669 7369 6f6e  yNodeSubdivision
 0018ac50: 5375 7266 6163 6528 6270 795f 7374 7275  Surface(bpy_stru
 0018ac60: 6374 2c20 4765 6f6d 6574 7279 4e6f 6465  ct, GeometryNode
-0018ac70: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-0018ac80: 726e 616c 293a 0a0a 2020 2222 220a 0a20  rnal):..  """.. 
+0018ac70: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+0018ac80: 4e6f 6465 293a 0a0a 2020 2222 220a 0a20  Node):..  """.. 
 0018ac90: 2044 6976 6964 6520 6d65 7368 2066 6163   Divide mesh fac
 0018aca0: 6573 2074 6f20 666f 726d 2061 2073 6d6f  es to form a smo
 0018acb0: 6f74 6820 7375 7266 6163 652c 2075 7369  oth surface, usi
 0018acc0: 6e67 2074 6865 2043 6174 6d75 6c6c 2d43  ng the Catmull-C
 0018acd0: 6c61 726b 2073 7562 6469 7669 7369 6f6e  lark subdivision
 0018ace0: 206d 6574 686f 640a 0a20 2022 2222 0a0a   method..  """..
 0018acf0: 2020 626f 756e 6461 7279 5f73 6d6f 6f74    boundary_smoot
@@ -101118,15 +101118,15 @@
 0018afd0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 0018afe0: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 0018aff0: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 0018b000: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 0018b010: 2047 656f 6d65 7472 794e 6f64 6553 7769   GeometryNodeSwi
 0018b020: 7463 6828 6270 795f 7374 7275 6374 2c20  tch(bpy_struct, 
 0018b030: 4765 6f6d 6574 7279 4e6f 6465 2c20 4e6f  GeometryNode, No
-0018b040: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+0018b040: 6465 496e 7465 726e 616c 2c20 4e6f 6465  deInternal, Node
 0018b050: 293a 0a0a 2020 2222 220a 0a20 2053 7769  ):..  """..  Swi
 0018b060: 7463 6820 6265 7477 6565 6e20 7477 6f20  tch between two 
 0018b070: 696e 7075 7473 0a0a 2020 2222 220a 0a20  inputs..  """.. 
 0018b080: 2069 6e70 7574 5f74 7970 653a 2073 7472   input_type: str
 0018b090: 203d 202e 2e2e 0a0a 2020 4063 6c61 7373   = .....  @class
 0018b0a0: 6d65 7468 6f64 0a0a 2020 6465 6620 6973  method..  def is
 0018b0b0: 5f72 6567 6973 7465 7265 645f 6e6f 6465  _registered_node
@@ -101166,15 +101166,15 @@
 0018b2d0: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 0018b2e0: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 0018b2f0: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 0018b300: 2020 202e 2e2e 0a0a 636c 6173 7320 4765     .....class Ge
 0018b310: 6f6d 6574 7279 4e6f 6465 5472 616e 7366  ometryNodeTransf
 0018b320: 6f72 6d28 6270 795f 7374 7275 6374 2c20  orm(bpy_struct, 
 0018b330: 4765 6f6d 6574 7279 4e6f 6465 2c20 4e6f  GeometryNode, No
-0018b340: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+0018b340: 6465 496e 7465 726e 616c 2c20 4e6f 6465  deInternal, Node
 0018b350: 293a 0a0a 2020 2222 220a 0a20 2054 7261  ):..  """..  Tra
 0018b360: 6e73 6c61 7465 2c20 726f 7461 7465 206f  nslate, rotate o
 0018b370: 7220 7363 616c 6520 7468 6520 6765 6f6d  r scale the geom
 0018b380: 6574 7279 0a0a 2020 2222 220a 0a20 2040  etry..  """..  @
 0018b390: 636c 6173 736d 6574 686f 640a 0a20 2064  classmethod..  d
 0018b3a0: 6566 2069 735f 7265 6769 7374 6572 6564  ef is_registered
 0018b3b0: 5f6e 6f64 655f 7479 7065 2863 6c73 2920  _node_type(cls) 
@@ -101214,15 +101214,15 @@
 0018b5d0: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 0018b5e0: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 0018b5f0: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 0018b600: 7373 2047 656f 6d65 7472 794e 6f64 6554  ss GeometryNodeT
 0018b610: 7261 6e73 6c61 7465 496e 7374 616e 6365  ranslateInstance
 0018b620: 7328 6270 795f 7374 7275 6374 2c20 4765  s(bpy_struct, Ge
 0018b630: 6f6d 6574 7279 4e6f 6465 2c20 4e6f 6465  ometryNode, Node
-0018b640: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+0018b640: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 0018b650: 0a0a 2020 2222 220a 0a20 204d 6f76 6520  ..  """..  Move 
 0018b660: 746f 702d 6c65 7665 6c20 6765 6f6d 6574  top-level geomet
 0018b670: 7279 2069 6e73 7461 6e63 6573 2069 6e20  ry instances in 
 0018b680: 6c6f 6361 6c20 6f72 2067 6c6f 6261 6c20  local or global 
 0018b690: 7370 6163 650a 0a20 2022 2222 0a0a 2020  space..  """..  
 0018b6a0: 4063 6c61 7373 6d65 7468 6f64 0a0a 2020  @classmethod..  
 0018b6b0: 6465 6620 6973 5f72 6567 6973 7465 7265  def is_registere
@@ -101262,16 +101262,16 @@
 0018b8d0: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 0018b8e0: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 0018b8f0: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 0018b900: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 0018b910: 6173 7320 4765 6f6d 6574 7279 4e6f 6465  ass GeometryNode
 0018b920: 5472 6961 6e67 756c 6174 6528 6270 795f  Triangulate(bpy_
 0018b930: 7374 7275 6374 2c20 4765 6f6d 6574 7279  struct, Geometry
-0018b940: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-0018b950: 496e 7465 726e 616c 293a 0a0a 2020 2222  Internal):..  ""
+0018b940: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
+0018b950: 616c 2c20 4e6f 6465 293a 0a0a 2020 2222  al, Node):..  ""
 0018b960: 220a 0a20 2043 6f6e 7665 7274 2061 6c6c  "..  Convert all
 0018b970: 2066 6163 6573 2069 6e20 6120 6d65 7368   faces in a mesh
 0018b980: 2074 6f20 7472 6961 6e67 756c 6172 2066   to triangular f
 0018b990: 6163 6573 0a0a 2020 2222 220a 0a20 206e  aces..  """..  n
 0018b9a0: 676f 6e5f 6d65 7468 6f64 3a20 7374 7220  gon_method: str 
 0018b9b0: 3d20 2e2e 2e0a 0a20 2022 2222 0a0a 2020  = .....  """..  
 0018b9c0: 4d65 7468 6f64 2066 6f72 2073 706c 6974  Method for split
@@ -101356,16 +101356,16 @@
 0018beb0: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 0018bec0: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 0018bed0: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 0018bee0: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 0018bef0: 2e2e 2e0a 0a63 6c61 7373 2047 656f 6d65  .....class Geome
 0018bf00: 7472 794e 6f64 6554 7269 6d43 7572 7665  tryNodeTrimCurve
 0018bf10: 2862 7079 5f73 7472 7563 742c 2047 656f  (bpy_struct, Geo
-0018bf20: 6d65 7472 794e 6f64 652c 204e 6f64 652c  metryNode, Node,
-0018bf30: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+0018bf20: 6d65 7472 794e 6f64 652c 204e 6f64 6549  metryNode, NodeI
+0018bf30: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 0018bf40: 0a20 2022 2222 0a0a 2020 5368 6f72 7465  .  """..  Shorte
 0018bf50: 6e20 6375 7276 6573 2062 7920 7265 6d6f  n curves by remo
 0018bf60: 7669 6e67 2070 6f72 7469 6f6e 7320 6174  ving portions at
 0018bf70: 2074 6865 2073 7461 7274 206f 7220 656e   the start or en
 0018bf80: 640a 0a20 2022 2222 0a0a 2020 6d6f 6465  d..  """..  mode
 0018bf90: 3a20 7374 7220 3d20 2e2e 2e0a 0a20 2022  : str = .....  "
 0018bfa0: 2222 0a0a 2020 486f 7720 746f 2066 696e  ""..  How to fin
@@ -101423,16 +101423,16 @@
 0018c2e0: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 0018c2f0: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 0018c300: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 0018c310: 202e 2e2e 0a0a 636c 6173 7320 4765 6f6d   .....class Geom
 0018c320: 6574 7279 4e6f 6465 5556 5061 636b 4973  etryNodeUVPackIs
 0018c330: 6c61 6e64 7328 6270 795f 7374 7275 6374  lands(bpy_struct
 0018c340: 2c20 4765 6f6d 6574 7279 4e6f 6465 2c20  , GeometryNode, 
-0018c350: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-0018c360: 616c 293a 0a0a 2020 2222 220a 0a20 2053  al):..  """..  S
+0018c350: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+0018c360: 6465 293a 0a0a 2020 2222 220a 0a20 2053  de):..  """..  S
 0018c370: 6361 6c65 2069 736c 616e 6473 206f 6620  cale islands of 
 0018c380: 6120 5556 206d 6170 2061 6e64 206d 6f76  a UV map and mov
 0018c390: 6520 7468 656d 2073 6f20 7468 6579 2066  e them so they f
 0018c3a0: 696c 6c20 7468 6520 5556 2073 7061 6365  ill the UV space
 0018c3b0: 2061 7320 6d75 6368 2061 7320 706f 7373   as much as poss
 0018c3c0: 6962 6c65 0a0a 2020 2222 220a 0a20 2040  ible..  """..  @
 0018c3d0: 636c 6173 736d 6574 686f 640a 0a20 2064  classmethod..  d
@@ -101473,16 +101473,16 @@
 0018c600: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 0018c610: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 0018c620: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 0018c630: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 0018c640: 7373 2047 656f 6d65 7472 794e 6f64 6555  ss GeometryNodeU
 0018c650: 5655 6e77 7261 7028 6270 795f 7374 7275  VUnwrap(bpy_stru
 0018c660: 6374 2c20 4765 6f6d 6574 7279 4e6f 6465  ct, GeometryNode
-0018c670: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-0018c680: 726e 616c 293a 0a0a 2020 2222 220a 0a20  rnal):..  """.. 
+0018c670: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+0018c680: 4e6f 6465 293a 0a0a 2020 2222 220a 0a20  Node):..  """.. 
 0018c690: 2047 656e 6572 6174 6520 6120 5556 206d   Generate a UV m
 0018c6a0: 6170 2062 6173 6564 206f 6e20 7365 616d  ap based on seam
 0018c6b0: 2065 6467 6573 0a0a 2020 2222 220a 0a20   edges..  """.. 
 0018c6c0: 206d 6574 686f 643a 2073 7472 203d 202e   method: str = .
 0018c6d0: 2e2e 0a0a 2020 2222 220a 0a20 202a 2060  ....  """..  * `
 0018c6e0: 6041 4e47 4c45 5f42 4153 4544 6060 0a41  `ANGLE_BASED``.A
 0018c6f0: 6e67 6c65 2042 6173 6564 202d 2d20 5468  ngle Based -- Th
@@ -101539,16 +101539,16 @@
 0018ca20: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 0018ca30: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 0018ca40: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 0018ca50: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 0018ca60: 6c61 7373 2047 656f 6d65 7472 794e 6f64  lass GeometryNod
 0018ca70: 6556 6572 7465 784f 6643 6f72 6e65 7228  eVertexOfCorner(
 0018ca80: 6270 795f 7374 7275 6374 2c20 4765 6f6d  bpy_struct, Geom
-0018ca90: 6574 7279 4e6f 6465 2c20 4e6f 6465 2c20  etryNode, Node, 
-0018caa0: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+0018ca90: 6574 7279 4e6f 6465 2c20 4e6f 6465 496e  etryNode, NodeIn
+0018caa0: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 0018cab0: 2020 2222 220a 0a20 2052 6574 7269 6576    """..  Retriev
 0018cac0: 6520 7468 6520 7665 7274 6578 2065 6163  e the vertex eac
 0018cad0: 6820 6661 6365 2063 6f72 6e65 7220 6973  h face corner is
 0018cae0: 2061 7474 6163 6865 6420 746f 0a0a 2020   attached to..  
 0018caf0: 2222 220a 0a20 2040 636c 6173 736d 6574  """..  @classmet
 0018cb00: 686f 640a 0a20 2064 6566 2069 735f 7265  hod..  def is_re
 0018cb10: 6769 7374 6572 6564 5f6e 6f64 655f 7479  gistered_node_ty
@@ -101587,16 +101587,16 @@
 0018cd20: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 0018cd30: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 0018cd40: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 0018cd50: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 0018cd60: 2e2e 2e0a 0a63 6c61 7373 2047 656f 6d65  .....class Geome
 0018cd70: 7472 794e 6f64 6556 6965 7765 7228 6270  tryNodeViewer(bp
 0018cd80: 795f 7374 7275 6374 2c20 4765 6f6d 6574  y_struct, Geomet
-0018cd90: 7279 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  ryNode, Node, No
-0018cda0: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+0018cd90: 7279 4e6f 6465 2c20 4e6f 6465 496e 7465  ryNode, NodeInte
+0018cda0: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 0018cdb0: 2222 220a 0a20 2044 6973 706c 6179 2074  """..  Display t
 0018cdc0: 6865 2069 6e70 7574 2064 6174 6120 696e  he input data in
 0018cdd0: 2074 6865 2053 7072 6561 6473 6865 6574   the Spreadsheet
 0018cde0: 2045 6469 746f 720a 0a20 2022 2222 0a0a   Editor..  """..
 0018cdf0: 2020 6461 7461 5f74 7970 653a 2073 7472    data_type: str
 0018ce00: 203d 202e 2e2e 0a0a 2020 646f 6d61 696e   = .....  domain
 0018ce10: 3a20 7374 7220 3d20 2e2e 2e0a 0a20 2022  : str = .....  "
@@ -101641,16 +101641,16 @@
 0018d080: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 0018d090: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 0018d0a0: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 0018d0b0: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 0018d0c0: 6173 7320 4765 6f6d 6574 7279 4e6f 6465  ass GeometryNode
 0018d0d0: 566f 6c75 6d65 4375 6265 2862 7079 5f73  VolumeCube(bpy_s
 0018d0e0: 7472 7563 742c 2047 656f 6d65 7472 794e  truct, GeometryN
-0018d0f0: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-0018d100: 6e74 6572 6e61 6c29 3a0a 0a20 2022 2222  nternal):..  """
+0018d0f0: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
+0018d100: 6c2c 204e 6f64 6529 3a0a 0a20 2022 2222  l, Node):..  """
 0018d110: 0a0a 2020 4765 6e65 7261 7465 2061 2064  ..  Generate a d
 0018d120: 656e 7365 2076 6f6c 756d 6520 7769 7468  ense volume with
 0018d130: 2061 2066 6965 6c64 2074 6861 7420 636f   a field that co
 0018d140: 6e74 726f 6c73 2074 6865 2064 656e 7369  ntrols the densi
 0018d150: 7479 2061 7420 6561 6368 2067 7269 6420  ty at each grid 
 0018d160: 766f 7865 6c20 6261 7365 6420 6f6e 2069  voxel based on i
 0018d170: 7473 2070 6f73 6974 696f 6e0a 0a20 2022  ts position..  "
@@ -101693,15 +101693,15 @@
 0018d3c0: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 0018d3d0: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 0018d3e0: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 0018d3f0: 2e2e 0a0a 636c 6173 7320 4765 6f6d 6574  ....class Geomet
 0018d400: 7279 4e6f 6465 566f 6c75 6d65 546f 4d65  ryNodeVolumeToMe
 0018d410: 7368 2862 7079 5f73 7472 7563 742c 2047  sh(bpy_struct, G
 0018d420: 656f 6d65 7472 794e 6f64 652c 204e 6f64  eometryNode, Nod
-0018d430: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+0018d430: 6549 6e74 6572 6e61 6c2c 204e 6f64 6529  eInternal, Node)
 0018d440: 3a0a 0a20 2022 2222 0a0a 2020 4765 6e65  :..  """..  Gene
 0018d450: 7261 7465 2061 206d 6573 6820 6f6e 2074  rate a mesh on t
 0018d460: 6865 2022 7375 7266 6163 6522 206f 6620  he "surface" of 
 0018d470: 6120 766f 6c75 6d65 0a0a 2020 2222 220a  a volume..  """.
 0018d480: 0a20 2072 6573 6f6c 7574 696f 6e5f 6d6f  .  resolution_mo
 0018d490: 6465 3a20 7374 7220 3d20 2e2e 2e0a 0a20  de: str = ..... 
 0018d4a0: 2022 2222 0a0a 2020 486f 7720 7468 6520   """..  How the 
@@ -101755,17 +101755,17 @@
 0018d7a0: 5f72 6e61 5f67 6574 5f73 7562 636c 6173  _rna_get_subclas
 0018d7b0: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 0018d7c0: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 0018d7d0: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 0018d7e0: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 0018d7f0: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2053      .....class S
 0018d800: 6861 6465 724e 6f64 6541 6464 5368 6164  haderNodeAddShad
-0018d810: 6572 2862 7079 5f73 7472 7563 742c 2053  er(bpy_struct, S
-0018d820: 6861 6465 724e 6f64 652c 204e 6f64 652c  haderNode, Node,
-0018d830: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+0018d810: 6572 2853 6861 6465 724e 6f64 652c 2062  er(ShaderNode, b
+0018d820: 7079 5f73 7472 7563 742c 204e 6f64 6549  py_struct, NodeI
+0018d830: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 0018d840: 0a20 2022 2222 0a0a 2020 4164 6420 7477  .  """..  Add tw
 0018d850: 6f20 5368 6164 6572 7320 746f 6765 7468  o Shaders togeth
 0018d860: 6572 0a0a 2020 2222 220a 0a20 2040 636c  er..  """..  @cl
 0018d870: 6173 736d 6574 686f 640a 0a20 2064 6566  assmethod..  def
 0018d880: 2069 735f 7265 6769 7374 6572 6564 5f6e   is_registered_n
 0018d890: 6f64 655f 7479 7065 2863 6c73 2920 2d3e  ode_type(cls) ->
 0018d8a0: 2062 6f6f 6c3a 0a0a 2020 2020 2222 220a   bool:..    """.
@@ -101801,18 +101801,18 @@
 0018da80: 626c 5f72 6e61 5f67 6574 5f73 7562 636c  bl_rna_get_subcl
 0018da90: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 0018daa0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 0018dab0: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 0018dac0: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 0018dad0: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 0018dae0: 2053 6861 6465 724e 6f64 6541 6d62 6965   ShaderNodeAmbie
-0018daf0: 6e74 4f63 636c 7573 696f 6e28 6270 795f  ntOcclusion(bpy_
-0018db00: 7374 7275 6374 2c20 5368 6164 6572 4e6f  struct, ShaderNo
-0018db10: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-0018db20: 7465 726e 616c 293a 0a0a 2020 2222 220a  ternal):..  """.
+0018daf0: 6e74 4f63 636c 7573 696f 6e28 5368 6164  ntOcclusion(Shad
+0018db00: 6572 4e6f 6465 2c20 6270 795f 7374 7275  erNode, bpy_stru
+0018db10: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+0018db20: 2c20 4e6f 6465 293a 0a0a 2020 2222 220a  , Node):..  """.
 0018db30: 0a20 2043 6f6d 7075 7465 2068 6f77 206d  .  Compute how m
 0018db40: 7563 6820 7468 6520 6865 6d69 7370 6865  uch the hemisphe
 0018db50: 7265 2061 626f 7665 2074 6865 2073 6861  re above the sha
 0018db60: 6469 6e67 2070 6f69 6e74 2069 7320 6f63  ding point is oc
 0018db70: 636c 7564 6564 2c20 666f 7220 6578 616d  cluded, for exam
 0018db80: 706c 6520 746f 2061 6464 2077 6561 7468  ple to add weath
 0018db90: 6572 696e 6720 6566 6665 6374 7320 746f  ering effects to
@@ -101873,18 +101873,18 @@
 0018df00: 0a20 2064 6566 2062 6c5f 726e 615f 6765  .  def bl_rna_ge
 0018df10: 745f 7375 6263 6c61 7373 5f70 7928 636c  t_subclass_py(cl
 0018df20: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 0018df30: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 0018df40: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 0018df50: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 0018df60: 0a0a 636c 6173 7320 5368 6164 6572 4e6f  ..class ShaderNo
-0018df70: 6465 4174 7472 6962 7574 6528 6270 795f  deAttribute(bpy_
-0018df80: 7374 7275 6374 2c20 5368 6164 6572 4e6f  struct, ShaderNo
-0018df90: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-0018dfa0: 7465 726e 616c 293a 0a0a 2020 2222 220a  ternal):..  """.
+0018df70: 6465 4174 7472 6962 7574 6528 5368 6164  deAttribute(Shad
+0018df80: 6572 4e6f 6465 2c20 6270 795f 7374 7275  erNode, bpy_stru
+0018df90: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+0018dfa0: 2c20 4e6f 6465 293a 0a0a 2020 2222 220a  , Node):..  """.
 0018dfb0: 0a20 2052 6574 7269 6576 6520 6174 7472  .  Retrieve attr
 0018dfc0: 6962 7574 6573 2061 7474 6163 6865 6420  ibutes attached 
 0018dfd0: 746f 206f 626a 6563 7473 206f 7220 6765  to objects or ge
 0018dfe0: 6f6d 6574 7279 0a0a 2020 2222 220a 0a20  ometry..  """.. 
 0018dff0: 2061 7474 7269 6275 7465 5f6e 616d 653a   attribute_name:
 0018e000: 2073 7472 203d 202e 2e2e 0a0a 2020 6174   str = .....  at
 0018e010: 7472 6962 7574 655f 7479 7065 3a20 7374  tribute_type: st
@@ -101965,18 +101965,18 @@
 0018e4c0: 0a20 2064 6566 2062 6c5f 726e 615f 6765  .  def bl_rna_ge
 0018e4d0: 745f 7375 6263 6c61 7373 5f70 7928 636c  t_subclass_py(cl
 0018e4e0: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 0018e4f0: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 0018e500: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 0018e510: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 0018e520: 0a0a 636c 6173 7320 5368 6164 6572 4e6f  ..class ShaderNo
-0018e530: 6465 4261 636b 6772 6f75 6e64 2862 7079  deBackground(bpy
-0018e540: 5f73 7472 7563 742c 2053 6861 6465 724e  _struct, ShaderN
-0018e550: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-0018e560: 6e74 6572 6e61 6c29 3a0a 0a20 2022 2222  nternal):..  """
+0018e530: 6465 4261 636b 6772 6f75 6e64 2853 6861  deBackground(Sha
+0018e540: 6465 724e 6f64 652c 2062 7079 5f73 7472  derNode, bpy_str
+0018e550: 7563 742c 204e 6f64 6549 6e74 6572 6e61  uct, NodeInterna
+0018e560: 6c2c 204e 6f64 6529 3a0a 0a20 2022 2222  l, Node):..  """
 0018e570: 0a0a 2020 4164 6420 6261 636b 6772 6f75  ..  Add backgrou
 0018e580: 6e64 206c 6967 6874 2065 6d69 7373 696f  nd light emissio
 0018e590: 6e2e 0a4e 6f74 653a 2054 6869 7320 6e6f  n..Note: This no
 0018e5a0: 6465 2073 686f 756c 6420 6f6e 6c79 2062  de should only b
 0018e5b0: 6520 7573 6564 2066 6f72 2074 6865 2077  e used for the w
 0018e5c0: 6f72 6c64 2073 7572 6661 6365 206f 7574  orld surface out
 0018e5d0: 7075 740a 0a20 2022 2222 0a0a 2020 4063  put..  """..  @c
@@ -102016,17 +102016,17 @@
 0018e7f0: 2062 6c5f 726e 615f 6765 745f 7375 6263   bl_rna_get_subc
 0018e800: 6c61 7373 5f70 7928 636c 732c 2069 643a  lass_py(cls, id:
 0018e810: 2073 7472 2c20 6465 6661 756c 743a 2074   str, default: t
 0018e820: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 0018e830: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 0018e840: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 0018e850: 7320 5368 6164 6572 4e6f 6465 4265 7665  s ShaderNodeBeve
-0018e860: 6c28 6270 795f 7374 7275 6374 2c20 5368  l(bpy_struct, Sh
-0018e870: 6164 6572 4e6f 6465 2c20 4e6f 6465 2c20  aderNode, Node, 
-0018e880: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+0018e860: 6c28 5368 6164 6572 4e6f 6465 2c20 6270  l(ShaderNode, bp
+0018e870: 795f 7374 7275 6374 2c20 4e6f 6465 496e  y_struct, NodeIn
+0018e880: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 0018e890: 2020 2222 220a 0a20 2047 656e 6572 6174    """..  Generat
 0018e8a0: 6573 206e 6f72 6d61 6c73 2077 6974 6820  es normals with 
 0018e8b0: 726f 756e 6420 636f 726e 6572 732e 0a4e  round corners..N
 0018e8c0: 6f74 653a 206f 6e6c 7920 7375 7070 6f72  ote: only suppor
 0018e8d0: 7465 6420 696e 2043 7963 6c65 732c 2061  ted in Cycles, a
 0018e8e0: 6e64 206d 6179 2073 6c6f 7720 646f 776e  nd may slow down
 0018e8f0: 2072 656e 6465 7273 0a0a 2020 2222 220a   renders..  """.
@@ -102072,17 +102072,17 @@
 0018eb70: 615f 6765 745f 7375 6263 6c61 7373 5f70  a_get_subclass_p
 0018eb80: 7928 636c 732c 2069 643a 2073 7472 2c20  y(cls, id: str, 
 0018eb90: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 0018eba0: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 0018ebb0: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 0018ebc0: 202e 2e2e 0a0a 636c 6173 7320 5368 6164   .....class Shad
 0018ebd0: 6572 4e6f 6465 426c 6163 6b62 6f64 7928  erNodeBlackbody(
-0018ebe0: 6270 795f 7374 7275 6374 2c20 5368 6164  bpy_struct, Shad
-0018ebf0: 6572 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  erNode, Node, No
-0018ec00: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+0018ebe0: 5368 6164 6572 4e6f 6465 2c20 6270 795f  ShaderNode, bpy_
+0018ebf0: 7374 7275 6374 2c20 4e6f 6465 496e 7465  struct, NodeInte
+0018ec00: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 0018ec10: 2222 220a 0a20 2043 6f6e 7665 7274 2061  """..  Convert a
 0018ec20: 2062 6c61 636b 626f 6479 2074 656d 7065   blackbody tempe
 0018ec30: 7261 7475 7265 2074 6f20 616e 2052 4742  rature to an RGB
 0018ec40: 2076 616c 7565 0a0a 2020 2222 220a 0a20   value..  """.. 
 0018ec50: 2040 636c 6173 736d 6574 686f 640a 0a20   @classmethod.. 
 0018ec60: 2064 6566 2069 735f 7265 6769 7374 6572   def is_register
 0018ec70: 6564 5f6e 6f64 655f 7479 7065 2863 6c73  ed_node_type(cls
@@ -102119,18 +102119,18 @@
 0018ee60: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 0018ee70: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 0018ee80: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 0018ee90: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 0018eea0: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 0018eeb0: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 0018eec0: 6c61 7373 2053 6861 6465 724e 6f64 6542  lass ShaderNodeB
-0018eed0: 7269 6768 7443 6f6e 7472 6173 7428 6270  rightContrast(bp
-0018eee0: 795f 7374 7275 6374 2c20 5368 6164 6572  y_struct, Shader
-0018eef0: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-0018ef00: 496e 7465 726e 616c 293a 0a0a 2020 2222  Internal):..  ""
+0018eed0: 7269 6768 7443 6f6e 7472 6173 7428 5368  rightContrast(Sh
+0018eee0: 6164 6572 4e6f 6465 2c20 6270 795f 7374  aderNode, bpy_st
+0018eef0: 7275 6374 2c20 4e6f 6465 496e 7465 726e  ruct, NodeIntern
+0018ef00: 616c 2c20 4e6f 6465 293a 0a0a 2020 2222  al, Node):..  ""
 0018ef10: 220a 0a20 2043 6f6e 7472 6f6c 2074 6865  "..  Control the
 0018ef20: 2062 7269 6768 746e 6573 7320 616e 6420   brightness and 
 0018ef30: 636f 6e74 7261 7374 206f 6620 7468 6520  contrast of the 
 0018ef40: 696e 7075 7420 636f 6c6f 720a 0a20 2022  input color..  "
 0018ef50: 2222 0a0a 2020 4063 6c61 7373 6d65 7468  ""..  @classmeth
 0018ef60: 6f64 0a0a 2020 6465 6620 6973 5f72 6567  od..  def is_reg
 0018ef70: 6973 7465 7265 645f 6e6f 6465 5f74 7970  istered_node_typ
@@ -102168,17 +102168,17 @@
 0018f170: 6765 745f 7375 6263 6c61 7373 5f70 7928  get_subclass_py(
 0018f180: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 0018f190: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 0018f1a0: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 0018f1b0: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 0018f1c0: 2e2e 0a0a 636c 6173 7320 5368 6164 6572  ....class Shader
 0018f1d0: 4e6f 6465 4273 6466 416e 6973 6f74 726f  NodeBsdfAnisotro
-0018f1e0: 7069 6328 6270 795f 7374 7275 6374 2c20  pic(bpy_struct, 
-0018f1f0: 5368 6164 6572 4e6f 6465 2c20 4e6f 6465  ShaderNode, Node
-0018f200: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+0018f1e0: 7069 6328 5368 6164 6572 4e6f 6465 2c20  pic(ShaderNode, 
+0018f1f0: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+0018f200: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 0018f210: 0a0a 2020 2222 220a 0a20 2047 6c6f 7373  ..  """..  Gloss
 0018f220: 7920 7265 666c 6563 7469 6f6e 2077 6974  y reflection wit
 0018f230: 6820 7365 7061 7261 7465 2063 6f6e 7472  h separate contr
 0018f240: 6f6c 206f 7665 7220 5520 616e 6420 5620  ol over U and V 
 0018f250: 6469 7265 6374 696f 6e20 726f 7567 686e  direction roughn
 0018f260: 6573 730a 0a20 2022 2222 0a0a 2020 6469  ess..  """..  di
 0018f270: 7374 7269 6275 7469 6f6e 3a20 7374 7220  stribution: str 
@@ -102238,18 +102238,18 @@
 0018f5d0: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 0018f5e0: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 0018f5f0: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 0018f600: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 0018f610: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 0018f620: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 0018f630: 6c61 7373 2053 6861 6465 724e 6f64 6542  lass ShaderNodeB
-0018f640: 7364 6644 6966 6675 7365 2862 7079 5f73  sdfDiffuse(bpy_s
-0018f650: 7472 7563 742c 2053 6861 6465 724e 6f64  truct, ShaderNod
-0018f660: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-0018f670: 6572 6e61 6c29 3a0a 0a20 2022 2222 0a0a  ernal):..  """..
+0018f640: 7364 6644 6966 6675 7365 2853 6861 6465  sdfDiffuse(Shade
+0018f650: 724e 6f64 652c 2062 7079 5f73 7472 7563  rNode, bpy_struc
+0018f660: 742c 204e 6f64 6549 6e74 6572 6e61 6c2c  t, NodeInternal,
+0018f670: 204e 6f64 6529 3a0a 0a20 2022 2222 0a0a   Node):..  """..
 0018f680: 2020 4c61 6d62 6572 7469 616e 2061 6e64    Lambertian and
 0018f690: 204f 7265 6e2d 4e61 7961 7220 6469 6666   Oren-Nayar diff
 0018f6a0: 7573 6520 7265 666c 6563 7469 6f6e 0a0a  use reflection..
 0018f6b0: 2020 2222 220a 0a20 2040 636c 6173 736d    """..  @classm
 0018f6c0: 6574 686f 640a 0a20 2064 6566 2069 735f  ethod..  def is_
 0018f6d0: 7265 6769 7374 6572 6564 5f6e 6f64 655f  registered_node_
 0018f6e0: 7479 7065 2863 6c73 2920 2d3e 2062 6f6f  type(cls) -> boo
@@ -102286,17 +102286,17 @@
 0018f8d0: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 0018f8e0: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 0018f8f0: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 0018f900: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 0018f910: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 0018f920: 2020 2e2e 2e0a 0a63 6c61 7373 2053 6861    .....class Sha
 0018f930: 6465 724e 6f64 6542 7364 6647 6c61 7373  derNodeBsdfGlass
-0018f940: 2862 7079 5f73 7472 7563 742c 2053 6861  (bpy_struct, Sha
-0018f950: 6465 724e 6f64 652c 204e 6f64 652c 204e  derNode, Node, N
-0018f960: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+0018f940: 2853 6861 6465 724e 6f64 652c 2062 7079  (ShaderNode, bpy
+0018f950: 5f73 7472 7563 742c 204e 6f64 6549 6e74  _struct, NodeInt
+0018f960: 6572 6e61 6c2c 204e 6f64 6529 3a0a 0a20  ernal, Node):.. 
 0018f970: 2022 2222 0a0a 2020 476c 6173 732d 6c69   """..  Glass-li
 0018f980: 6b65 2073 6861 6465 7220 6d69 7869 6e67  ke shader mixing
 0018f990: 2072 6566 7261 6374 696f 6e20 616e 6420   refraction and 
 0018f9a0: 7265 666c 6563 7469 6f6e 2061 7420 6772  reflection at gr
 0018f9b0: 617a 696e 6720 616e 676c 6573 0a0a 2020  azing angles..  
 0018f9c0: 2222 220a 0a20 2064 6973 7472 6962 7574  """..  distribut
 0018f9d0: 696f 6e3a 2073 7472 203d 202e 2e2e 0a0a  ion: str = .....
@@ -102360,17 +102360,17 @@
 0018fd70: 5f72 6e61 5f67 6574 5f73 7562 636c 6173  _rna_get_subclas
 0018fd80: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 0018fd90: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 0018fda0: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 0018fdb0: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 0018fdc0: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2053      .....class S
 0018fdd0: 6861 6465 724e 6f64 6542 7364 6647 6c6f  haderNodeBsdfGlo
-0018fde0: 7373 7928 6270 795f 7374 7275 6374 2c20  ssy(bpy_struct, 
-0018fdf0: 5368 6164 6572 4e6f 6465 2c20 4e6f 6465  ShaderNode, Node
-0018fe00: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+0018fde0: 7373 7928 5368 6164 6572 4e6f 6465 2c20  ssy(ShaderNode, 
+0018fdf0: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+0018fe00: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 0018fe10: 0a0a 2020 2222 220a 0a20 2052 6566 6c65  ..  """..  Refle
 0018fe20: 6374 696f 6e20 7769 7468 206d 6963 726f  ction with micro
 0018fe30: 6661 6365 7420 6469 7374 7269 6275 7469  facet distributi
 0018fe40: 6f6e 2c20 7573 6564 2066 6f72 206d 6174  on, used for mat
 0018fe50: 6572 6961 6c73 2073 7563 6820 6173 206d  erials such as m
 0018fe60: 6574 616c 206f 7220 6d69 7272 6f72 730a  etal or mirrors.
 0018fe70: 0a20 2022 2222 0a0a 2020 6469 7374 7269  .  """..  distri
@@ -102438,17 +102438,17 @@
 00190250: 6c5f 726e 615f 6765 745f 7375 6263 6c61  l_rna_get_subcla
 00190260: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 00190270: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 00190280: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 00190290: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 001902a0: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 001902b0: 5368 6164 6572 4e6f 6465 4273 6466 4861  ShaderNodeBsdfHa
-001902c0: 6972 2862 7079 5f73 7472 7563 742c 2053  ir(bpy_struct, S
-001902d0: 6861 6465 724e 6f64 652c 204e 6f64 652c  haderNode, Node,
-001902e0: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+001902c0: 6972 2853 6861 6465 724e 6f64 652c 2062  ir(ShaderNode, b
+001902d0: 7079 5f73 7472 7563 742c 204e 6f64 6549  py_struct, NodeI
+001902e0: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 001902f0: 0a20 2022 2222 0a0a 2020 5265 666c 6563  .  """..  Reflec
 00190300: 7469 6f6e 2061 6e64 2074 7261 6e73 6d69  tion and transmi
 00190310: 7373 696f 6e20 7368 6164 6572 7320 6f70  ssion shaders op
 00190320: 7469 6d69 7a65 6420 666f 7220 6861 6972  timized for hair
 00190330: 2072 656e 6465 7269 6e67 0a0a 2020 2222   rendering..  ""
 00190340: 220a 0a20 2063 6f6d 706f 6e65 6e74 3a20  "..  component: 
 00190350: 7374 7220 3d20 2e2e 2e0a 0a20 2022 2222  str = .....  """
@@ -102503,18 +102503,18 @@
 00190660: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 00190670: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 00190680: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 00190690: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 001906a0: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 001906b0: 2020 2e2e 2e0a 0a63 6c61 7373 2053 6861    .....class Sha
 001906c0: 6465 724e 6f64 6542 7364 6648 6169 7250  derNodeBsdfHairP
-001906d0: 7269 6e63 6970 6c65 6428 6270 795f 7374  rincipled(bpy_st
-001906e0: 7275 6374 2c20 5368 6164 6572 4e6f 6465  ruct, ShaderNode
-001906f0: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-00190700: 726e 616c 293a 0a0a 2020 2222 220a 0a20  rnal):..  """.. 
+001906d0: 7269 6e63 6970 6c65 6428 5368 6164 6572  rincipled(Shader
+001906e0: 4e6f 6465 2c20 6270 795f 7374 7275 6374  Node, bpy_struct
+001906f0: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+00190700: 4e6f 6465 293a 0a0a 2020 2222 220a 0a20  Node):..  """.. 
 00190710: 2050 6879 7369 6361 6c6c 792d 6261 7365   Physically-base
 00190720: 642c 2065 6173 792d 746f 2d75 7365 2073  d, easy-to-use s
 00190730: 6861 6465 7220 666f 7220 7265 6e64 6572  hader for render
 00190740: 696e 6720 6861 6972 2061 6e64 2066 7572  ing hair and fur
 00190750: 0a0a 2020 2222 220a 0a20 2070 6172 616d  ..  """..  param
 00190760: 6574 7269 7a61 7469 6f6e 3a20 7374 7220  etrization: str 
 00190770: 3d20 2e2e 2e0a 0a20 2022 2222 0a0a 2020  = .....  """..  
@@ -102588,18 +102588,18 @@
 00190bb0: 2064 6566 2062 6c5f 726e 615f 6765 745f   def bl_rna_get_
 00190bc0: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 00190bd0: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 00190be0: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 00190bf0: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 00190c00: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 00190c10: 636c 6173 7320 5368 6164 6572 4e6f 6465  class ShaderNode
-00190c20: 4273 6466 5072 696e 6369 706c 6564 2862  BsdfPrincipled(b
-00190c30: 7079 5f73 7472 7563 742c 2053 6861 6465  py_struct, Shade
-00190c40: 724e 6f64 652c 204e 6f64 652c 204e 6f64  rNode, Node, Nod
-00190c50: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2022  eInternal):..  "
+00190c20: 4273 6466 5072 696e 6369 706c 6564 2853  BsdfPrincipled(S
+00190c30: 6861 6465 724e 6f64 652c 2062 7079 5f73  haderNode, bpy_s
+00190c40: 7472 7563 742c 204e 6f64 6549 6e74 6572  truct, NodeInter
+00190c50: 6e61 6c2c 204e 6f64 6529 3a0a 0a20 2022  nal, Node):..  "
 00190c60: 2222 0a0a 2020 5068 7973 6963 616c 6c79  ""..  Physically
 00190c70: 2d62 6173 6564 2c20 6561 7379 2d74 6f2d  -based, easy-to-
 00190c80: 7573 6520 7368 6164 6572 2066 6f72 2072  use shader for r
 00190c90: 656e 6465 7269 6e67 2073 7572 6661 6365  endering surface
 00190ca0: 206d 6174 6572 6961 6c73 2c20 6261 7365   materials, base
 00190cb0: 6420 6f6e 2074 6865 2044 6973 6e65 7920  d on the Disney 
 00190cc0: 7072 696e 6369 706c 6564 206d 6f64 656c  principled model
@@ -102691,18 +102691,18 @@
 00191220: 6620 626c 5f72 6e61 5f67 6574 5f73 7562  f bl_rna_get_sub
 00191230: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 00191240: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 00191250: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 00191260: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 00191270: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 00191280: 7373 2053 6861 6465 724e 6f64 6542 7364  ss ShaderNodeBsd
-00191290: 6652 6566 7261 6374 696f 6e28 6270 795f  fRefraction(bpy_
-001912a0: 7374 7275 6374 2c20 5368 6164 6572 4e6f  struct, ShaderNo
-001912b0: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-001912c0: 7465 726e 616c 293a 0a0a 2020 2222 220a  ternal):..  """.
+00191290: 6652 6566 7261 6374 696f 6e28 5368 6164  fRefraction(Shad
+001912a0: 6572 4e6f 6465 2c20 6270 795f 7374 7275  erNode, bpy_stru
+001912b0: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+001912c0: 2c20 4e6f 6465 293a 0a0a 2020 2222 220a  , Node):..  """.
 001912d0: 0a20 2047 6c6f 7373 7920 7265 6672 6163  .  Glossy refrac
 001912e0: 7469 6f6e 2077 6974 6820 7368 6172 7020  tion with sharp 
 001912f0: 6f72 206d 6963 726f 6661 6365 7420 6469  or microfacet di
 00191300: 7374 7269 6275 7469 6f6e 2c20 7479 7069  stribution, typi
 00191310: 6361 6c6c 7920 7573 6564 2066 6f72 206d  cally used for m
 00191320: 6174 6572 6961 6c73 2074 6861 7420 7472  aterials that tr
 00191330: 616e 736d 6974 206c 6967 6874 0a0a 2020  ansmit light..  
@@ -102758,17 +102758,17 @@
 00191650: 6620 626c 5f72 6e61 5f67 6574 5f73 7562  f bl_rna_get_sub
 00191660: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 00191670: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 00191680: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 00191690: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 001916a0: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 001916b0: 7373 2053 6861 6465 724e 6f64 6542 7364  ss ShaderNodeBsd
-001916c0: 6654 6f6f 6e28 6270 795f 7374 7275 6374  fToon(bpy_struct
-001916d0: 2c20 5368 6164 6572 4e6f 6465 2c20 4e6f  , ShaderNode, No
-001916e0: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+001916c0: 6654 6f6f 6e28 5368 6164 6572 4e6f 6465  fToon(ShaderNode
+001916d0: 2c20 6270 795f 7374 7275 6374 2c20 4e6f  , bpy_struct, No
+001916e0: 6465 496e 7465 726e 616c 2c20 4e6f 6465  deInternal, Node
 001916f0: 293a 0a0a 2020 2222 220a 0a20 2044 6966  ):..  """..  Dif
 00191700: 6675 7365 2061 6e64 2047 6c6f 7373 7920  fuse and Glossy 
 00191710: 7368 6164 6572 7320 7769 7468 2063 6172  shaders with car
 00191720: 746f 6f6e 206c 6967 6874 2065 6666 6563  toon light effec
 00191730: 7473 0a0a 2020 2222 220a 0a20 2063 6f6d  ts..  """..  com
 00191740: 706f 6e65 6e74 3a20 7374 7220 3d20 2e2e  ponent: str = ..
 00191750: 2e0a 0a20 2022 2222 0a0a 2020 546f 6f6e  ...  """..  Toon
@@ -102816,18 +102816,18 @@
 001919f0: 726e 615f 6765 745f 7375 6263 6c61 7373  rna_get_subclass
 00191a00: 5f70 7928 636c 732c 2069 643a 2073 7472  _py(cls, id: str
 00191a10: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 00191a20: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 00191a30: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 00191a40: 2020 202e 2e2e 0a0a 636c 6173 7320 5368     .....class Sh
 00191a50: 6164 6572 4e6f 6465 4273 6466 5472 616e  aderNodeBsdfTran
-00191a60: 736c 7563 656e 7428 6270 795f 7374 7275  slucent(bpy_stru
-00191a70: 6374 2c20 5368 6164 6572 4e6f 6465 2c20  ct, ShaderNode, 
-00191a80: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-00191a90: 616c 293a 0a0a 2020 2222 220a 0a20 204c  al):..  """..  L
+00191a60: 736c 7563 656e 7428 5368 6164 6572 4e6f  slucent(ShaderNo
+00191a70: 6465 2c20 6270 795f 7374 7275 6374 2c20  de, bpy_struct, 
+00191a80: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+00191a90: 6465 293a 0a0a 2020 2222 220a 0a20 204c  de):..  """..  L
 00191aa0: 616d 6265 7274 6961 6e20 6469 6666 7573  ambertian diffus
 00191ab0: 6520 7472 616e 736d 6973 7369 6f6e 0a0a  e transmission..
 00191ac0: 2020 2222 220a 0a20 2040 636c 6173 736d    """..  @classm
 00191ad0: 6574 686f 640a 0a20 2064 6566 2069 735f  ethod..  def is_
 00191ae0: 7265 6769 7374 6572 6564 5f6e 6f64 655f  registered_node_
 00191af0: 7479 7065 2863 6c73 2920 2d3e 2062 6f6f  type(cls) -> boo
 00191b00: 6c3a 0a0a 2020 2020 2222 220a 0a20 2020  l:..    """..   
@@ -102863,18 +102863,18 @@
 00191ce0: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 00191cf0: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 00191d00: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 00191d10: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 00191d20: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 00191d30: 2020 2e2e 2e0a 0a63 6c61 7373 2053 6861    .....class Sha
 00191d40: 6465 724e 6f64 6542 7364 6654 7261 6e73  derNodeBsdfTrans
-00191d50: 7061 7265 6e74 2862 7079 5f73 7472 7563  parent(bpy_struc
-00191d60: 742c 2053 6861 6465 724e 6f64 652c 204e  t, ShaderNode, N
-00191d70: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-00191d80: 6c29 3a0a 0a20 2022 2222 0a0a 2020 5472  l):..  """..  Tr
+00191d50: 7061 7265 6e74 2853 6861 6465 724e 6f64  parent(ShaderNod
+00191d60: 652c 2062 7079 5f73 7472 7563 742c 204e  e, bpy_struct, N
+00191d70: 6f64 6549 6e74 6572 6e61 6c2c 204e 6f64  odeInternal, Nod
+00191d80: 6529 3a0a 0a20 2022 2222 0a0a 2020 5472  e):..  """..  Tr
 00191d90: 616e 7370 6172 656e 6379 2077 6974 686f  ansparency witho
 00191da0: 7574 2072 6566 7261 6374 696f 6e2c 2070  ut refraction, p
 00191db0: 6173 7369 6e67 2073 7472 6169 6768 7420  assing straight 
 00191dc0: 7468 726f 7567 6820 7468 6520 7375 7266  through the surf
 00191dd0: 6163 6520 6173 2069 6620 7468 6572 6520  ace as if there 
 00191de0: 7765 7265 206e 6f20 6765 6f6d 6574 7279  were no geometry
 00191df0: 0a0a 2020 2222 220a 0a20 2040 636c 6173  ..  """..  @clas
@@ -102914,17 +102914,17 @@
 00192010: 5f72 6e61 5f67 6574 5f73 7562 636c 6173  _rna_get_subclas
 00192020: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 00192030: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 00192040: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 00192050: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 00192060: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2053      .....class S
 00192070: 6861 6465 724e 6f64 6542 7364 6656 656c  haderNodeBsdfVel
-00192080: 7665 7428 6270 795f 7374 7275 6374 2c20  vet(bpy_struct, 
-00192090: 5368 6164 6572 4e6f 6465 2c20 4e6f 6465  ShaderNode, Node
-001920a0: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+00192080: 7665 7428 5368 6164 6572 4e6f 6465 2c20  vet(ShaderNode, 
+00192090: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+001920a0: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 001920b0: 0a0a 2020 2222 220a 0a20 2052 6566 6c65  ..  """..  Refle
 001920c0: 6374 696f 6e20 666f 7220 6d61 7465 7269  ction for materi
 001920d0: 616c 7320 7375 6368 2061 7320 636c 6f74  als such as clot
 001920e0: 682e 0a54 7970 6963 616c 6c79 206d 6978  h..Typically mix
 001920f0: 6564 2077 6974 6820 6f74 6865 7220 7368  ed with other sh
 00192100: 6164 6572 7320 2873 7563 6820 6173 2061  aders (such as a
 00192110: 2044 6966 6675 7365 2053 6861 6465 7229   Diffuse Shader)
@@ -102967,18 +102967,18 @@
 00192360: 0a0a 2020 6465 6620 626c 5f72 6e61 5f67  ..  def bl_rna_g
 00192370: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 00192380: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 00192390: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 001923a0: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 001923b0: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 001923c0: 2e0a 0a63 6c61 7373 2053 6861 6465 724e  ...class ShaderN
-001923d0: 6f64 6542 756d 7028 6270 795f 7374 7275  odeBump(bpy_stru
-001923e0: 6374 2c20 5368 6164 6572 4e6f 6465 2c20  ct, ShaderNode, 
-001923f0: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-00192400: 616c 293a 0a0a 2020 2222 220a 0a20 2047  al):..  """..  G
+001923d0: 6f64 6542 756d 7028 5368 6164 6572 4e6f  odeBump(ShaderNo
+001923e0: 6465 2c20 6270 795f 7374 7275 6374 2c20  de, bpy_struct, 
+001923f0: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+00192400: 6465 293a 0a0a 2020 2222 220a 0a20 2047  de):..  """..  G
 00192410: 656e 6572 6174 6520 6120 7065 7274 7572  enerate a pertur
 00192420: 6265 6420 6e6f 726d 616c 2066 726f 6d20  bed normal from 
 00192430: 6120 6865 6967 6874 2074 6578 7475 7265  a height texture
 00192440: 2066 6f72 2062 756d 7020 6d61 7070 696e   for bump mappin
 00192450: 672e 2054 7970 6963 616c 6c79 2075 7365  g. Typically use
 00192460: 6420 666f 7220 6661 6b69 6e67 2068 6967  d for faking hig
 00192470: 686c 7920 6465 7461 696c 6564 2073 7572  hly detailed sur
@@ -103026,18 +103026,18 @@
 00192710: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 00192720: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 00192730: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 00192740: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 00192750: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 00192760: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 00192770: 6c61 7373 2053 6861 6465 724e 6f64 6543  lass ShaderNodeC
-00192780: 616d 6572 6144 6174 6128 6270 795f 7374  ameraData(bpy_st
-00192790: 7275 6374 2c20 5368 6164 6572 4e6f 6465  ruct, ShaderNode
-001927a0: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-001927b0: 726e 616c 293a 0a0a 2020 2222 220a 0a20  rnal):..  """.. 
+00192780: 616d 6572 6144 6174 6128 5368 6164 6572  ameraData(Shader
+00192790: 4e6f 6465 2c20 6270 795f 7374 7275 6374  Node, bpy_struct
+001927a0: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+001927b0: 4e6f 6465 293a 0a0a 2020 2222 220a 0a20  Node):..  """.. 
 001927c0: 2052 6574 7269 6576 6520 696e 666f 726d   Retrieve inform
 001927d0: 6174 696f 6e20 6162 6f75 7420 7468 6520  ation about the 
 001927e0: 6361 6d65 7261 2061 6e64 2068 6f77 2069  camera and how i
 001927f0: 7420 7265 6c61 7465 7320 746f 2074 6865  t relates to the
 00192800: 2063 7572 7265 6e74 2073 6861 6469 6e67   current shading
 00192810: 2070 6f69 6e74 2773 2070 6f73 6974 696f   point's positio
 00192820: 6e0a 0a20 2022 2222 0a0a 2020 4063 6c61  n..  """..  @cla
@@ -103077,17 +103077,17 @@
 00192a40: 6c5f 726e 615f 6765 745f 7375 6263 6c61  l_rna_get_subcla
 00192a50: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 00192a60: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 00192a70: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 00192a80: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 00192a90: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 00192aa0: 5368 6164 6572 4e6f 6465 436c 616d 7028  ShaderNodeClamp(
-00192ab0: 6270 795f 7374 7275 6374 2c20 5368 6164  bpy_struct, Shad
-00192ac0: 6572 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  erNode, Node, No
-00192ad0: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+00192ab0: 5368 6164 6572 4e6f 6465 2c20 6270 795f  ShaderNode, bpy_
+00192ac0: 7374 7275 6374 2c20 4e6f 6465 496e 7465  struct, NodeInte
+00192ad0: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 00192ae0: 2222 220a 0a20 2043 6c61 6d70 2061 2076  """..  Clamp a v
 00192af0: 616c 7565 2062 6574 7765 656e 2061 206d  alue between a m
 00192b00: 696e 696d 756d 2061 6e64 2061 206d 6178  inimum and a max
 00192b10: 696d 756d 0a0a 2020 2222 220a 0a20 2063  imum..  """..  c
 00192b20: 6c61 6d70 5f74 7970 653a 2073 7472 203d  lamp_type: str =
 00192b30: 202e 2e2e 0a0a 2020 4063 6c61 7373 6d65   .....  @classme
 00192b40: 7468 6f64 0a0a 2020 6465 6620 6973 5f72  thod..  def is_r
@@ -103126,17 +103126,17 @@
 00192d50: 615f 6765 745f 7375 6263 6c61 7373 5f70  a_get_subclass_p
 00192d60: 7928 636c 732c 2069 643a 2073 7472 2c20  y(cls, id: str, 
 00192d70: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 00192d80: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 00192d90: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 00192da0: 202e 2e2e 0a0a 636c 6173 7320 5368 6164   .....class Shad
 00192db0: 6572 4e6f 6465 436f 6d62 696e 6543 6f6c  erNodeCombineCol
-00192dc0: 6f72 2862 7079 5f73 7472 7563 742c 2053  or(bpy_struct, S
-00192dd0: 6861 6465 724e 6f64 652c 204e 6f64 652c  haderNode, Node,
-00192de0: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+00192dc0: 6f72 2853 6861 6465 724e 6f64 652c 2062  or(ShaderNode, b
+00192dd0: 7079 5f73 7472 7563 742c 204e 6f64 6549  py_struct, NodeI
+00192de0: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 00192df0: 0a20 2022 2222 0a0a 2020 4372 6561 7465  .  """..  Create
 00192e00: 2061 2063 6f6c 6f72 2066 726f 6d20 696e   a color from in
 00192e10: 6469 7669 6475 616c 2063 6f6d 706f 6e65  dividual compone
 00192e20: 6e74 7320 7573 696e 6720 6d75 6c74 6970  nts using multip
 00192e30: 6c65 206d 6f64 656c 730a 0a20 2022 2222  le models..  """
 00192e40: 0a0a 2020 6d6f 6465 3a20 7374 7220 3d20  ..  mode: str = 
 00192e50: 2e2e 2e0a 0a20 2022 2222 0a0a 2020 4d6f  .....  """..  Mo
@@ -103187,17 +103187,17 @@
 00193120: 5f72 6e61 5f67 6574 5f73 7562 636c 6173  _rna_get_subclas
 00193130: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 00193140: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 00193150: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 00193160: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 00193170: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2053      .....class S
 00193180: 6861 6465 724e 6f64 6543 6f6d 6269 6e65  haderNodeCombine
-00193190: 4853 5628 6270 795f 7374 7275 6374 2c20  HSV(bpy_struct, 
-001931a0: 5368 6164 6572 4e6f 6465 2c20 4e6f 6465  ShaderNode, Node
-001931b0: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+00193190: 4853 5628 5368 6164 6572 4e6f 6465 2c20  HSV(ShaderNode, 
+001931a0: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+001931b0: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 001931c0: 0a0a 2020 2222 220a 0a20 2043 7265 6174  ..  """..  Creat
 001931d0: 6520 6120 636f 6c6f 7220 6672 6f6d 2069  e a color from i
 001931e0: 7473 2068 7565 2c20 7361 7475 7261 7469  ts hue, saturati
 001931f0: 6f6e 2c20 616e 6420 7661 6c75 6520 6368  on, and value ch
 00193200: 616e 6e65 6c73 0a0a 2020 2222 220a 0a20  annels..  """.. 
 00193210: 2040 636c 6173 736d 6574 686f 640a 0a20   @classmethod.. 
 00193220: 2064 6566 2069 735f 7265 6769 7374 6572   def is_register
@@ -103235,18 +103235,18 @@
 00193420: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 00193430: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 00193440: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 00193450: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 00193460: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 00193470: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 00193480: 6c61 7373 2053 6861 6465 724e 6f64 6543  lass ShaderNodeC
-00193490: 6f6d 6269 6e65 5247 4228 6270 795f 7374  ombineRGB(bpy_st
-001934a0: 7275 6374 2c20 5368 6164 6572 4e6f 6465  ruct, ShaderNode
-001934b0: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-001934c0: 726e 616c 293a 0a0a 2020 2222 220a 0a20  rnal):..  """.. 
+00193490: 6f6d 6269 6e65 5247 4228 5368 6164 6572  ombineRGB(Shader
+001934a0: 4e6f 6465 2c20 6270 795f 7374 7275 6374  Node, bpy_struct
+001934b0: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+001934c0: 4e6f 6465 293a 0a0a 2020 2222 220a 0a20  Node):..  """.. 
 001934d0: 2047 656e 6572 6174 6520 6120 636f 6c6f   Generate a colo
 001934e0: 7220 6672 6f6d 2069 7473 2072 6564 2c20  r from its red, 
 001934f0: 6772 6565 6e2c 2061 6e64 2062 6c75 6520  green, and blue 
 00193500: 6368 616e 6e65 6c73 2028 4465 7072 6563  channels (Deprec
 00193510: 6174 6564 290a 0a20 2022 2222 0a0a 2020  ated)..  """..  
 00193520: 4063 6c61 7373 6d65 7468 6f64 0a0a 2020  @classmethod..  
 00193530: 6465 6620 6973 5f72 6567 6973 7465 7265  def is_registere
@@ -103284,18 +103284,18 @@
 00193730: 6566 2062 6c5f 726e 615f 6765 745f 7375  ef bl_rna_get_su
 00193740: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 00193750: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 00193760: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 00193770: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 00193780: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 00193790: 6173 7320 5368 6164 6572 4e6f 6465 436f  ass ShaderNodeCo
-001937a0: 6d62 696e 6558 595a 2862 7079 5f73 7472  mbineXYZ(bpy_str
-001937b0: 7563 742c 2053 6861 6465 724e 6f64 652c  uct, ShaderNode,
-001937c0: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-001937d0: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+001937a0: 6d62 696e 6558 595a 2853 6861 6465 724e  mbineXYZ(ShaderN
+001937b0: 6f64 652c 2062 7079 5f73 7472 7563 742c  ode, bpy_struct,
+001937c0: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+001937d0: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 001937e0: 4372 6561 7465 2061 2076 6563 746f 7220  Create a vector 
 001937f0: 6672 6f6d 2058 2c20 592c 2061 6e64 205a  from X, Y, and Z
 00193800: 2063 6f6d 706f 6e65 6e74 730a 0a20 2022   components..  "
 00193810: 2222 0a0a 2020 4063 6c61 7373 6d65 7468  ""..  @classmeth
 00193820: 6f64 0a0a 2020 6465 6620 6973 5f72 6567  od..  def is_reg
 00193830: 6973 7465 7265 645f 6e6f 6465 5f74 7970  istered_node_typ
 00193840: 6528 636c 7329 202d 3e20 626f 6f6c 3a0a  e(cls) -> bool:.
@@ -103332,17 +103332,17 @@
 00193a30: 6765 745f 7375 6263 6c61 7373 5f70 7928  get_subclass_py(
 00193a40: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 00193a50: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 00193a60: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 00193a70: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 00193a80: 2e2e 0a0a 636c 6173 7320 5368 6164 6572  ....class Shader
 00193a90: 4e6f 6465 4375 7374 6f6d 4772 6f75 7028  NodeCustomGroup(
-00193aa0: 6270 795f 7374 7275 6374 2c20 5368 6164  bpy_struct, Shad
-00193ab0: 6572 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  erNode, Node, No
-00193ac0: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+00193aa0: 5368 6164 6572 4e6f 6465 2c20 6270 795f  ShaderNode, bpy_
+00193ab0: 7374 7275 6374 2c20 4e6f 6465 496e 7465  struct, NodeInte
+00193ac0: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 00193ad0: 2222 220a 0a20 2043 7573 746f 6d20 5368  """..  Custom Sh
 00193ae0: 6164 6572 2047 726f 7570 204e 6f64 6520  ader Group Node 
 00193af0: 666f 7220 5079 7468 6f6e 206e 6f64 6573  for Python nodes
 00193b00: 0a0a 2020 2222 220a 0a20 206e 6f64 655f  ..  """..  node_
 00193b10: 7472 6565 3a20 4e6f 6465 5472 6565 203d  tree: NodeTree =
 00193b20: 202e 2e2e 0a0a 2020 4063 6c61 7373 6d65   .....  @classme
 00193b30: 7468 6f64 0a0a 2020 6465 6620 626c 5f72  thod..  def bl_r
@@ -103355,18 +103355,18 @@
 00193ba0: 2064 6566 2062 6c5f 726e 615f 6765 745f   def bl_rna_get_
 00193bb0: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 00193bc0: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 00193bd0: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 00193be0: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 00193bf0: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 00193c00: 636c 6173 7320 5368 6164 6572 4e6f 6465  class ShaderNode
-00193c10: 4469 7370 6c61 6365 6d65 6e74 2862 7079  Displacement(bpy
-00193c20: 5f73 7472 7563 742c 2053 6861 6465 724e  _struct, ShaderN
-00193c30: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-00193c40: 6e74 6572 6e61 6c29 3a0a 0a20 2022 2222  nternal):..  """
+00193c10: 4469 7370 6c61 6365 6d65 6e74 2853 6861  Displacement(Sha
+00193c20: 6465 724e 6f64 652c 2062 7079 5f73 7472  derNode, bpy_str
+00193c30: 7563 742c 204e 6f64 6549 6e74 6572 6e61  uct, NodeInterna
+00193c40: 6c2c 204e 6f64 6529 3a0a 0a20 2022 2222  l, Node):..  """
 00193c50: 0a0a 2020 4469 7370 6c61 6365 2074 6865  ..  Displace the
 00193c60: 2073 7572 6661 6365 2061 6c6f 6e67 2074   surface along t
 00193c70: 6865 2073 7572 6661 6365 206e 6f72 6d61  he surface norma
 00193c80: 6c0a 0a20 2022 2222 0a0a 2020 7370 6163  l..  """..  spac
 00193c90: 653a 2073 7472 203d 202e 2e2e 0a0a 2020  e: str = .....  
 00193ca0: 2222 220a 0a20 2053 7061 6365 206f 6620  """..  Space of 
 00193cb0: 7468 6520 696e 7075 7420 6865 6967 6874  the input height
@@ -103418,18 +103418,18 @@
 00193f90: 2064 6566 2062 6c5f 726e 615f 6765 745f   def bl_rna_get_
 00193fa0: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 00193fb0: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 00193fc0: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 00193fd0: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 00193fe0: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 00193ff0: 636c 6173 7320 5368 6164 6572 4e6f 6465  class ShaderNode
-00194000: 4565 7665 6553 7065 6375 6c61 7228 6270  EeveeSpecular(bp
-00194010: 795f 7374 7275 6374 2c20 5368 6164 6572  y_struct, Shader
-00194020: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-00194030: 496e 7465 726e 616c 293a 0a0a 2020 2222  Internal):..  ""
+00194000: 4565 7665 6553 7065 6375 6c61 7228 5368  EeveeSpecular(Sh
+00194010: 6164 6572 4e6f 6465 2c20 6270 795f 7374  aderNode, bpy_st
+00194020: 7275 6374 2c20 4e6f 6465 496e 7465 726e  ruct, NodeIntern
+00194030: 616c 2c20 4e6f 6465 293a 0a0a 2020 2222  al, Node):..  ""
 00194040: 220a 0a20 2053 696d 696c 6172 2074 6f20  "..  Similar to 
 00194050: 7468 6520 5072 696e 6369 706c 6564 2042  the Principled B
 00194060: 5344 4620 6e6f 6465 2062 7574 2075 7365  SDF node but use
 00194070: 7320 7468 6520 7370 6563 756c 6172 2077  s the specular w
 00194080: 6f72 6b66 6c6f 7720 696e 7374 6561 6420  orkflow instead 
 00194090: 6f66 206d 6574 616c 6c69 632c 2077 6869  of metallic, whi
 001940a0: 6368 2066 756e 6374 696f 6e73 2062 7920  ch functions by 
@@ -103477,18 +103477,18 @@
 00194340: 6f64 0a0a 2020 6465 6620 626c 5f72 6e61  od..  def bl_rna
 00194350: 5f67 6574 5f73 7562 636c 6173 735f 7079  _get_subclass_py
 00194360: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 00194370: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 00194380: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 00194390: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 001943a0: 2e2e 2e0a 0a63 6c61 7373 2053 6861 6465  .....class Shade
-001943b0: 724e 6f64 6545 6d69 7373 696f 6e28 6270  rNodeEmission(bp
-001943c0: 795f 7374 7275 6374 2c20 5368 6164 6572  y_struct, Shader
-001943d0: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-001943e0: 496e 7465 726e 616c 293a 0a0a 2020 2222  Internal):..  ""
+001943b0: 724e 6f64 6545 6d69 7373 696f 6e28 5368  rNodeEmission(Sh
+001943c0: 6164 6572 4e6f 6465 2c20 6270 795f 7374  aderNode, bpy_st
+001943d0: 7275 6374 2c20 4e6f 6465 496e 7465 726e  ruct, NodeIntern
+001943e0: 616c 2c20 4e6f 6465 293a 0a0a 2020 2222  al, Node):..  ""
 001943f0: 220a 0a20 204c 616d 6265 7274 6961 6e20  "..  Lambertian 
 00194400: 656d 6973 7369 6f6e 2073 6861 6465 720a  emission shader.
 00194410: 0a20 2022 2222 0a0a 2020 4063 6c61 7373  .  """..  @class
 00194420: 6d65 7468 6f64 0a0a 2020 6465 6620 6973  method..  def is
 00194430: 5f72 6567 6973 7465 7265 645f 6e6f 6465  _registered_node
 00194440: 5f74 7970 6528 636c 7329 202d 3e20 626f  _type(cls) -> bo
 00194450: 6f6c 3a0a 0a20 2020 2022 2222 0a0a 2020  ol:..    """..  
@@ -103524,17 +103524,17 @@
 00194630: 726e 615f 6765 745f 7375 6263 6c61 7373  rna_get_subclass
 00194640: 5f70 7928 636c 732c 2069 643a 2073 7472  _py(cls, id: str
 00194650: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 00194660: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 00194670: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 00194680: 2020 202e 2e2e 0a0a 636c 6173 7320 5368     .....class Sh
 00194690: 6164 6572 4e6f 6465 466c 6f61 7443 7572  aderNodeFloatCur
-001946a0: 7665 2862 7079 5f73 7472 7563 742c 2053  ve(bpy_struct, S
-001946b0: 6861 6465 724e 6f64 652c 204e 6f64 652c  haderNode, Node,
-001946c0: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+001946a0: 7665 2853 6861 6465 724e 6f64 652c 2062  ve(ShaderNode, b
+001946b0: 7079 5f73 7472 7563 742c 204e 6f64 6549  py_struct, NodeI
+001946c0: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 001946d0: 0a20 2022 2222 0a0a 2020 4d61 7020 616e  .  """..  Map an
 001946e0: 2069 6e70 7574 2066 6c6f 6174 2074 6f20   input float to 
 001946f0: 6120 6375 7276 6520 616e 6420 6f75 7470  a curve and outp
 00194700: 7574 7320 6120 666c 6f61 7420 7661 6c75  uts a float valu
 00194710: 650a 0a20 2022 2222 0a0a 2020 6d61 7070  e..  """..  mapp
 00194720: 696e 673a 2043 7572 7665 4d61 7070 696e  ing: CurveMappin
 00194730: 6720 3d20 2e2e 2e0a 0a20 2040 636c 6173  g = .....  @clas
@@ -103574,17 +103574,17 @@
 00194950: 5f72 6e61 5f67 6574 5f73 7562 636c 6173  _rna_get_subclas
 00194960: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 00194970: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 00194980: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 00194990: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 001949a0: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2053      .....class S
 001949b0: 6861 6465 724e 6f64 6546 7265 736e 656c  haderNodeFresnel
-001949c0: 2862 7079 5f73 7472 7563 742c 2053 6861  (bpy_struct, Sha
-001949d0: 6465 724e 6f64 652c 204e 6f64 652c 204e  derNode, Node, N
-001949e0: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+001949c0: 2853 6861 6465 724e 6f64 652c 2062 7079  (ShaderNode, bpy
+001949d0: 5f73 7472 7563 742c 204e 6f64 6549 6e74  _struct, NodeInt
+001949e0: 6572 6e61 6c2c 204e 6f64 6529 3a0a 0a20  ernal, Node):.. 
 001949f0: 2022 2222 0a0a 2020 5072 6f64 7563 6520   """..  Produce 
 00194a00: 6120 626c 656e 6469 6e67 2066 6163 746f  a blending facto
 00194a10: 7220 6465 7065 6e64 696e 6720 6f6e 2074  r depending on t
 00194a20: 6865 2061 6e67 6c65 2062 6574 7765 656e  he angle between
 00194a30: 2074 6865 2073 7572 6661 6365 206e 6f72   the surface nor
 00194a40: 6d61 6c20 616e 6420 7468 6520 7669 6577  mal and the view
 00194a50: 2064 6972 6563 7469 6f6e 2075 7369 6e67   direction using
@@ -103629,18 +103629,18 @@
 00194cc0: 640a 0a20 2064 6566 2062 6c5f 726e 615f  d..  def bl_rna_
 00194cd0: 6765 745f 7375 6263 6c61 7373 5f70 7928  get_subclass_py(
 00194ce0: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 00194cf0: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 00194d00: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 00194d10: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 00194d20: 2e2e 0a0a 636c 6173 7320 5368 6164 6572  ....class Shader
-00194d30: 4e6f 6465 4761 6d6d 6128 6270 795f 7374  NodeGamma(bpy_st
-00194d40: 7275 6374 2c20 5368 6164 6572 4e6f 6465  ruct, ShaderNode
-00194d50: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-00194d60: 726e 616c 293a 0a0a 2020 2222 220a 0a20  rnal):..  """.. 
+00194d30: 4e6f 6465 4761 6d6d 6128 5368 6164 6572  NodeGamma(Shader
+00194d40: 4e6f 6465 2c20 6270 795f 7374 7275 6374  Node, bpy_struct
+00194d50: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+00194d60: 4e6f 6465 293a 0a0a 2020 2222 220a 0a20  Node):..  """.. 
 00194d70: 2041 7070 6c79 2061 2067 616d 6d61 2063   Apply a gamma c
 00194d80: 6f72 7265 6374 696f 6e0a 0a20 2022 2222  orrection..  """
 00194d90: 0a0a 2020 4063 6c61 7373 6d65 7468 6f64  ..  @classmethod
 00194da0: 0a0a 2020 6465 6620 6973 5f72 6567 6973  ..  def is_regis
 00194db0: 7465 7265 645f 6e6f 6465 5f74 7970 6528  tered_node_type(
 00194dc0: 636c 7329 202d 3e20 626f 6f6c 3a0a 0a20  cls) -> bool:.. 
 00194dd0: 2020 2022 2222 0a0a 2020 2020 5472 7565     """..    True
@@ -103675,18 +103675,18 @@
 00194fa0: 0a20 2064 6566 2062 6c5f 726e 615f 6765  .  def bl_rna_ge
 00194fb0: 745f 7375 6263 6c61 7373 5f70 7928 636c  t_subclass_py(cl
 00194fc0: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 00194fd0: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 00194fe0: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 00194ff0: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 00195000: 0a0a 636c 6173 7320 5368 6164 6572 4e6f  ..class ShaderNo
-00195010: 6465 4772 6f75 7028 6270 795f 7374 7275  deGroup(bpy_stru
-00195020: 6374 2c20 5368 6164 6572 4e6f 6465 2c20  ct, ShaderNode, 
-00195030: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-00195040: 616c 293a 0a0a 2020 6e6f 6465 5f74 7265  al):..  node_tre
+00195010: 6465 4772 6f75 7028 5368 6164 6572 4e6f  deGroup(ShaderNo
+00195020: 6465 2c20 6270 795f 7374 7275 6374 2c20  de, bpy_struct, 
+00195030: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+00195040: 6465 293a 0a0a 2020 6e6f 6465 5f74 7265  de):..  node_tre
 00195050: 653a 204e 6f64 6554 7265 6520 3d20 2e2e  e: NodeTree = ..
 00195060: 2e0a 0a20 2040 636c 6173 736d 6574 686f  ...  @classmetho
 00195070: 640a 0a20 2064 6566 2069 735f 7265 6769  d..  def is_regi
 00195080: 7374 6572 6564 5f6e 6f64 655f 7479 7065  stered_node_type
 00195090: 2863 6c73 2920 2d3e 2062 6f6f 6c3a 0a0a  (cls) -> bool:..
 001950a0: 2020 2020 2222 220a 0a20 2020 2054 7275      """..    Tru
 001950b0: 6520 6966 2061 2072 6567 6973 7465 7265  e if a registere
@@ -103720,18 +103720,18 @@
 00195270: 0a0a 2020 6465 6620 626c 5f72 6e61 5f67  ..  def bl_rna_g
 00195280: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 00195290: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 001952a0: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 001952b0: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 001952c0: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 001952d0: 2e0a 0a63 6c61 7373 2053 6861 6465 724e  ...class ShaderN
-001952e0: 6f64 6548 6169 7249 6e66 6f28 6270 795f  odeHairInfo(bpy_
-001952f0: 7374 7275 6374 2c20 5368 6164 6572 4e6f  struct, ShaderNo
-00195300: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-00195310: 7465 726e 616c 293a 0a0a 2020 2222 220a  ternal):..  """.
+001952e0: 6f64 6548 6169 7249 6e66 6f28 5368 6164  odeHairInfo(Shad
+001952f0: 6572 4e6f 6465 2c20 6270 795f 7374 7275  erNode, bpy_stru
+00195300: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+00195310: 2c20 4e6f 6465 293a 0a0a 2020 2222 220a  , Node):..  """.
 00195320: 0a20 2052 6574 7269 6576 6520 6861 6972  .  Retrieve hair
 00195330: 2063 7572 7665 2069 6e66 6f72 6d61 7469   curve informati
 00195340: 6f6e 0a0a 2020 2222 220a 0a20 2040 636c  on..  """..  @cl
 00195350: 6173 736d 6574 686f 640a 0a20 2064 6566  assmethod..  def
 00195360: 2069 735f 7265 6769 7374 6572 6564 5f6e   is_registered_n
 00195370: 6f64 655f 7479 7065 2863 6c73 2920 2d3e  ode_type(cls) ->
 00195380: 2062 6f6f 6c3a 0a0a 2020 2020 2222 220a   bool:..    """.
@@ -103767,17 +103767,17 @@
 00195560: 626c 5f72 6e61 5f67 6574 5f73 7562 636c  bl_rna_get_subcl
 00195570: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 00195580: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 00195590: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 001955a0: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 001955b0: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 001955c0: 2053 6861 6465 724e 6f64 6548 6f6c 646f   ShaderNodeHoldo
-001955d0: 7574 2862 7079 5f73 7472 7563 742c 2053  ut(bpy_struct, S
-001955e0: 6861 6465 724e 6f64 652c 204e 6f64 652c  haderNode, Node,
-001955f0: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+001955d0: 7574 2853 6861 6465 724e 6f64 652c 2062  ut(ShaderNode, b
+001955e0: 7079 5f73 7472 7563 742c 204e 6f64 6549  py_struct, NodeI
+001955f0: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 00195600: 0a20 2022 2222 0a0a 2020 4372 6561 7465  .  """..  Create
 00195610: 2061 2022 686f 6c65 2220 696e 2074 6865   a "hole" in the
 00195620: 2069 6d61 6765 2077 6974 6820 7a65 726f   image with zero
 00195630: 2061 6c70 6861 2074 7261 6e73 7061 7265   alpha transpare
 00195640: 6e63 792c 2077 6869 6368 2069 7320 7573  ncy, which is us
 00195650: 6566 756c 2066 6f72 2063 6f6d 706f 7369  eful for composi
 00195660: 7469 6e67 2e0a 4e6f 7465 3a20 7468 6520  ting..Note: the 
@@ -103823,18 +103823,18 @@
 001958e0: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 001958f0: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 00195900: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 00195910: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 00195920: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 00195930: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 00195940: 6c61 7373 2053 6861 6465 724e 6f64 6548  lass ShaderNodeH
-00195950: 7565 5361 7475 7261 7469 6f6e 2862 7079  ueSaturation(bpy
-00195960: 5f73 7472 7563 742c 2053 6861 6465 724e  _struct, ShaderN
-00195970: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-00195980: 6e74 6572 6e61 6c29 3a0a 0a20 2022 2222  nternal):..  """
+00195950: 7565 5361 7475 7261 7469 6f6e 2853 6861  ueSaturation(Sha
+00195960: 6465 724e 6f64 652c 2062 7079 5f73 7472  derNode, bpy_str
+00195970: 7563 742c 204e 6f64 6549 6e74 6572 6e61  uct, NodeInterna
+00195980: 6c2c 204e 6f64 6529 3a0a 0a20 2022 2222  l, Node):..  """
 00195990: 0a0a 2020 4170 706c 7920 6120 636f 6c6f  ..  Apply a colo
 001959a0: 7220 7472 616e 7366 6f72 6d61 7469 6f6e  r transformation
 001959b0: 2069 6e20 7468 6520 4853 5620 636f 6c6f   in the HSV colo
 001959c0: 7220 6d6f 6465 6c0a 0a20 2022 2222 0a0a  r model..  """..
 001959d0: 2020 4063 6c61 7373 6d65 7468 6f64 0a0a    @classmethod..
 001959e0: 2020 6465 6620 6973 5f72 6567 6973 7465    def is_registe
 001959f0: 7265 645f 6e6f 6465 5f74 7970 6528 636c  red_node_type(cl
@@ -103871,18 +103871,18 @@
 00195be0: 2064 6566 2062 6c5f 726e 615f 6765 745f   def bl_rna_get_
 00195bf0: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 00195c00: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 00195c10: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 00195c20: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 00195c30: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 00195c40: 636c 6173 7320 5368 6164 6572 4e6f 6465  class ShaderNode
-00195c50: 496e 7665 7274 2862 7079 5f73 7472 7563  Invert(bpy_struc
-00195c60: 742c 2053 6861 6465 724e 6f64 652c 204e  t, ShaderNode, N
-00195c70: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-00195c80: 6c29 3a0a 0a20 2022 2222 0a0a 2020 496e  l):..  """..  In
+00195c50: 496e 7665 7274 2853 6861 6465 724e 6f64  Invert(ShaderNod
+00195c60: 652c 2062 7079 5f73 7472 7563 742c 204e  e, bpy_struct, N
+00195c70: 6f64 6549 6e74 6572 6e61 6c2c 204e 6f64  odeInternal, Nod
+00195c80: 6529 3a0a 0a20 2022 2222 0a0a 2020 496e  e):..  """..  In
 00195c90: 7665 7274 2061 2063 6f6c 6f72 2c20 7072  vert a color, pr
 00195ca0: 6f64 7563 696e 6720 6120 6e65 6761 7469  oducing a negati
 00195cb0: 7665 0a0a 2020 2222 220a 0a20 2040 636c  ve..  """..  @cl
 00195cc0: 6173 736d 6574 686f 640a 0a20 2064 6566  assmethod..  def
 00195cd0: 2069 735f 7265 6769 7374 6572 6564 5f6e   is_registered_n
 00195ce0: 6f64 655f 7479 7065 2863 6c73 2920 2d3e  ode_type(cls) ->
 00195cf0: 2062 6f6f 6c3a 0a0a 2020 2020 2222 220a   bool:..    """.
@@ -103918,18 +103918,18 @@
 00195ed0: 626c 5f72 6e61 5f67 6574 5f73 7562 636c  bl_rna_get_subcl
 00195ee0: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 00195ef0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 00195f00: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 00195f10: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 00195f20: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 00195f30: 2053 6861 6465 724e 6f64 654c 6179 6572   ShaderNodeLayer
-00195f40: 5765 6967 6874 2862 7079 5f73 7472 7563  Weight(bpy_struc
-00195f50: 742c 2053 6861 6465 724e 6f64 652c 204e  t, ShaderNode, N
-00195f60: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-00195f70: 6c29 3a0a 0a20 2022 2222 0a0a 2020 5072  l):..  """..  Pr
+00195f40: 5765 6967 6874 2853 6861 6465 724e 6f64  Weight(ShaderNod
+00195f50: 652c 2062 7079 5f73 7472 7563 742c 204e  e, bpy_struct, N
+00195f60: 6f64 6549 6e74 6572 6e61 6c2c 204e 6f64  odeInternal, Nod
+00195f70: 6529 3a0a 0a20 2022 2222 0a0a 2020 5072  e):..  """..  Pr
 00195f80: 6f64 7563 6520 6120 626c 656e 6469 6e67  oduce a blending
 00195f90: 2066 6163 746f 7220 6465 7065 6e64 696e   factor dependin
 00195fa0: 6720 6f6e 2074 6865 2061 6e67 6c65 2062  g on the angle b
 00195fb0: 6574 7765 656e 2074 6865 2073 7572 6661  etween the surfa
 00195fc0: 6365 206e 6f72 6d61 6c20 616e 6420 7468  ce normal and th
 00195fd0: 6520 7669 6577 2064 6972 6563 7469 6f6e  e view direction
 00195fe0: 2e0a 5479 7069 6361 6c6c 7920 7573 6564  ..Typically used
@@ -103973,17 +103973,17 @@
 00196240: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 00196250: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 00196260: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 00196270: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 00196280: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 00196290: 2020 2e2e 2e0a 0a63 6c61 7373 2053 6861    .....class Sha
 001962a0: 6465 724e 6f64 654c 6967 6874 4661 6c6c  derNodeLightFall
-001962b0: 6f66 6628 6270 795f 7374 7275 6374 2c20  off(bpy_struct, 
-001962c0: 5368 6164 6572 4e6f 6465 2c20 4e6f 6465  ShaderNode, Node
-001962d0: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+001962b0: 6f66 6628 5368 6164 6572 4e6f 6465 2c20  off(ShaderNode, 
+001962c0: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+001962d0: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 001962e0: 0a0a 2020 2222 220a 0a20 204d 616e 6970  ..  """..  Manip
 001962f0: 756c 6174 6520 686f 7720 6c69 6768 7420  ulate how light 
 00196300: 696e 7465 6e73 6974 7920 6465 6372 6561  intensity decrea
 00196310: 7365 7320 6f76 6572 2064 6973 7461 6e63  ses over distanc
 00196320: 652e 2054 7970 6963 616c 6c79 2075 7365  e. Typically use
 00196330: 6420 666f 7220 6e6f 6e2d 7068 7973 6963  d for non-physic
 00196340: 616c 6c79 2d62 6173 6564 2065 6666 6563  ally-based effec
@@ -104027,17 +104027,17 @@
 001965a0: 2062 6c5f 726e 615f 6765 745f 7375 6263   bl_rna_get_subc
 001965b0: 6c61 7373 5f70 7928 636c 732c 2069 643a  lass_py(cls, id:
 001965c0: 2073 7472 2c20 6465 6661 756c 743a 2074   str, default: t
 001965d0: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 001965e0: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 001965f0: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 00196600: 7320 5368 6164 6572 4e6f 6465 4c69 6768  s ShaderNodeLigh
-00196610: 7450 6174 6828 6270 795f 7374 7275 6374  tPath(bpy_struct
-00196620: 2c20 5368 6164 6572 4e6f 6465 2c20 4e6f  , ShaderNode, No
-00196630: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+00196610: 7450 6174 6828 5368 6164 6572 4e6f 6465  tPath(ShaderNode
+00196620: 2c20 6270 795f 7374 7275 6374 2c20 4e6f  , bpy_struct, No
+00196630: 6465 496e 7465 726e 616c 2c20 4e6f 6465  deInternal, Node
 00196640: 293a 0a0a 2020 2222 220a 0a20 2052 6574  ):..  """..  Ret
 00196650: 7269 6576 6520 7468 6520 7479 7065 206f  rieve the type o
 00196660: 6620 696e 636f 6d69 6e67 2072 6179 2066  f incoming ray f
 00196670: 6f72 2077 6869 6368 2074 6865 2073 6861  or which the sha
 00196680: 6465 7220 6973 2062 6569 6e67 2065 7865  der is being exe
 00196690: 6375 7465 642e 0a54 7970 6963 616c 6c79  cuted..Typically
 001966a0: 2075 7365 6420 666f 7220 6e6f 6e2d 7068   used for non-ph
@@ -104079,18 +104079,18 @@
 001968e0: 6566 2062 6c5f 726e 615f 6765 745f 7375  ef bl_rna_get_su
 001968f0: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 00196900: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 00196910: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 00196920: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 00196930: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 00196940: 6173 7320 5368 6164 6572 4e6f 6465 4d61  ass ShaderNodeMa
-00196950: 7052 616e 6765 2862 7079 5f73 7472 7563  pRange(bpy_struc
-00196960: 742c 2053 6861 6465 724e 6f64 652c 204e  t, ShaderNode, N
-00196970: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-00196980: 6c29 3a0a 0a20 2022 2222 0a0a 2020 5265  l):..  """..  Re
+00196950: 7052 616e 6765 2853 6861 6465 724e 6f64  pRange(ShaderNod
+00196960: 652c 2062 7079 5f73 7472 7563 742c 204e  e, bpy_struct, N
+00196970: 6f64 6549 6e74 6572 6e61 6c2c 204e 6f64  odeInternal, Nod
+00196980: 6529 3a0a 0a20 2022 2222 0a0a 2020 5265  e):..  """..  Re
 00196990: 6d61 7020 6120 7661 6c75 6520 6672 6f6d  map a value from
 001969a0: 2061 2072 616e 6765 2074 6f20 6120 7461   a range to a ta
 001969b0: 7267 6574 2072 616e 6765 0a0a 2020 2222  rget range..  ""
 001969c0: 220a 0a20 2063 6c61 6d70 3a20 626f 6f6c  "..  clamp: bool
 001969d0: 203d 202e 2e2e 0a0a 2020 2222 220a 0a20   = .....  """.. 
 001969e0: 2043 6c61 6d70 2074 6865 2072 6573 756c   Clamp the resul
 001969f0: 7420 746f 2074 6865 2074 6172 6765 7420  t to the target 
@@ -104144,17 +104144,17 @@
 00196cf0: 6c5f 726e 615f 6765 745f 7375 6263 6c61  l_rna_get_subcla
 00196d00: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 00196d10: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 00196d20: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 00196d30: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 00196d40: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 00196d50: 5368 6164 6572 4e6f 6465 4d61 7070 696e  ShaderNodeMappin
-00196d60: 6728 6270 795f 7374 7275 6374 2c20 5368  g(bpy_struct, Sh
-00196d70: 6164 6572 4e6f 6465 2c20 4e6f 6465 2c20  aderNode, Node, 
-00196d80: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+00196d60: 6728 5368 6164 6572 4e6f 6465 2c20 6270  g(ShaderNode, bp
+00196d70: 795f 7374 7275 6374 2c20 4e6f 6465 496e  y_struct, NodeIn
+00196d80: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 00196d90: 2020 2222 220a 0a20 2054 7261 6e73 666f    """..  Transfo
 00196da0: 726d 2074 6865 2069 6e70 7574 2076 6563  rm the input vec
 00196db0: 746f 7220 6279 2061 7070 6c79 696e 6720  tor by applying 
 00196dc0: 7472 616e 736c 6174 696f 6e2c 2072 6f74  translation, rot
 00196dd0: 6174 696f 6e2c 2061 6e64 2073 6361 6c65  ation, and scale
 00196de0: 0a0a 2020 2222 220a 0a20 2076 6563 746f  ..  """..  vecto
 00196df0: 725f 7479 7065 3a20 7374 7220 3d20 2e2e  r_type: str = ..
@@ -104198,17 +104198,17 @@
 00197050: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 00197060: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 00197070: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 00197080: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 00197090: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 001970a0: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 001970b0: 6c61 7373 2053 6861 6465 724e 6f64 654d  lass ShaderNodeM
-001970c0: 6174 6828 6270 795f 7374 7275 6374 2c20  ath(bpy_struct, 
-001970d0: 5368 6164 6572 4e6f 6465 2c20 4e6f 6465  ShaderNode, Node
-001970e0: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+001970c0: 6174 6828 5368 6164 6572 4e6f 6465 2c20  ath(ShaderNode, 
+001970d0: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+001970e0: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 001970f0: 0a0a 2020 2222 220a 0a20 2050 6572 666f  ..  """..  Perfo
 00197100: 726d 206d 6174 6820 6f70 6572 6174 696f  rm math operatio
 00197110: 6e73 0a0a 2020 2222 220a 0a20 206f 7065  ns..  """..  ope
 00197120: 7261 7469 6f6e 3a20 7374 7220 3d20 2e2e  ration: str = ..
 00197130: 2e0a 0a20 2075 7365 5f63 6c61 6d70 3a20  ...  use_clamp: 
 00197140: 626f 6f6c 203d 202e 2e2e 0a0a 2020 2222  bool = .....  ""
 00197150: 220a 0a20 2043 6c61 6d70 2072 6573 756c  "..  Clamp resul
@@ -104250,18 +104250,18 @@
 00197390: 736d 6574 686f 640a 0a20 2064 6566 2062  smethod..  def b
 001973a0: 6c5f 726e 615f 6765 745f 7375 6263 6c61  l_rna_get_subcla
 001973b0: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 001973c0: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 001973d0: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 001973e0: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 001973f0: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
-00197400: 5368 6164 6572 4e6f 6465 4d69 7828 6270  ShaderNodeMix(bp
-00197410: 795f 7374 7275 6374 2c20 5368 6164 6572  y_struct, Shader
-00197420: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-00197430: 496e 7465 726e 616c 293a 0a0a 2020 2222  Internal):..  ""
+00197400: 5368 6164 6572 4e6f 6465 4d69 7828 5368  ShaderNodeMix(Sh
+00197410: 6164 6572 4e6f 6465 2c20 6270 795f 7374  aderNode, bpy_st
+00197420: 7275 6374 2c20 4e6f 6465 496e 7465 726e  ruct, NodeIntern
+00197430: 616c 2c20 4e6f 6465 293a 0a0a 2020 2222  al, Node):..  ""
 00197440: 220a 0a20 204d 6978 2076 616c 7565 7320  "..  Mix values 
 00197450: 6279 2061 2066 6163 746f 720a 0a20 2022  by a factor..  "
 00197460: 2222 0a0a 2020 626c 656e 645f 7479 7065  ""..  blend_type
 00197470: 3a20 7374 7220 3d20 2e2e 2e0a 0a20 2063  : str = .....  c
 00197480: 6c61 6d70 5f66 6163 746f 723a 2062 6f6f  lamp_factor: boo
 00197490: 6c20 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  l = .....  """..
 001974a0: 2020 436c 616d 7020 7468 6520 6661 6374    Clamp the fact
@@ -104319,18 +104319,18 @@
 001977e0: 6f64 0a0a 2020 6465 6620 626c 5f72 6e61  od..  def bl_rna
 001977f0: 5f67 6574 5f73 7562 636c 6173 735f 7079  _get_subclass_py
 00197800: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 00197810: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 00197820: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 00197830: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 00197840: 2e2e 2e0a 0a63 6c61 7373 2053 6861 6465  .....class Shade
-00197850: 724e 6f64 654d 6978 5247 4228 6270 795f  rNodeMixRGB(bpy_
-00197860: 7374 7275 6374 2c20 5368 6164 6572 4e6f  struct, ShaderNo
-00197870: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-00197880: 7465 726e 616c 293a 0a0a 2020 2222 220a  ternal):..  """.
+00197850: 724e 6f64 654d 6978 5247 4228 5368 6164  rNodeMixRGB(Shad
+00197860: 6572 4e6f 6465 2c20 6270 795f 7374 7275  erNode, bpy_stru
+00197870: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+00197880: 2c20 4e6f 6465 293a 0a0a 2020 2222 220a  , Node):..  """.
 00197890: 0a20 204d 6978 2074 776f 2069 6e70 7574  .  Mix two input
 001978a0: 2063 6f6c 6f72 730a 0a20 2022 2222 0a0a   colors..  """..
 001978b0: 2020 626c 656e 645f 7479 7065 3a20 7374    blend_type: st
 001978c0: 7220 3d20 2e2e 2e0a 0a20 2075 7365 5f61  r = .....  use_a
 001978d0: 6c70 6861 3a20 626f 6f6c 203d 202e 2e2e  lpha: bool = ...
 001978e0: 0a0a 2020 2222 220a 0a20 2049 6e63 6c75  ..  """..  Inclu
 001978f0: 6465 2061 6c70 6861 206f 6620 7365 636f  de alpha of seco
@@ -104378,17 +104378,17 @@
 00197b90: 6c5f 726e 615f 6765 745f 7375 6263 6c61  l_rna_get_subcla
 00197ba0: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 00197bb0: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 00197bc0: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 00197bd0: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 00197be0: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 00197bf0: 5368 6164 6572 4e6f 6465 4d69 7853 6861  ShaderNodeMixSha
-00197c00: 6465 7228 6270 795f 7374 7275 6374 2c20  der(bpy_struct, 
-00197c10: 5368 6164 6572 4e6f 6465 2c20 4e6f 6465  ShaderNode, Node
-00197c20: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+00197c00: 6465 7228 5368 6164 6572 4e6f 6465 2c20  der(ShaderNode, 
+00197c10: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+00197c20: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 00197c30: 0a0a 2020 2222 220a 0a20 204d 6978 2074  ..  """..  Mix t
 00197c40: 776f 2073 6861 6465 7273 2074 6f67 6574  wo shaders toget
 00197c50: 6865 722e 2054 7970 6963 616c 6c79 2075  her. Typically u
 00197c60: 7365 6420 666f 7220 6d61 7465 7269 616c  sed for material
 00197c70: 206c 6179 6572 696e 670a 0a20 2022 2222   layering..  """
 00197c80: 0a0a 2020 4063 6c61 7373 6d65 7468 6f64  ..  @classmethod
 00197c90: 0a0a 2020 6465 6620 6973 5f72 6567 6973  ..  def is_regis
@@ -104426,18 +104426,18 @@
 00197e90: 0a20 2064 6566 2062 6c5f 726e 615f 6765  .  def bl_rna_ge
 00197ea0: 745f 7375 6263 6c61 7373 5f70 7928 636c  t_subclass_py(cl
 00197eb0: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 00197ec0: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 00197ed0: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 00197ee0: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 00197ef0: 0a0a 636c 6173 7320 5368 6164 6572 4e6f  ..class ShaderNo
-00197f00: 6465 4e65 7747 656f 6d65 7472 7928 6270  deNewGeometry(bp
-00197f10: 795f 7374 7275 6374 2c20 5368 6164 6572  y_struct, Shader
-00197f20: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-00197f30: 496e 7465 726e 616c 293a 0a0a 2020 2222  Internal):..  ""
+00197f00: 6465 4e65 7747 656f 6d65 7472 7928 5368  deNewGeometry(Sh
+00197f10: 6164 6572 4e6f 6465 2c20 6270 795f 7374  aderNode, bpy_st
+00197f20: 7275 6374 2c20 4e6f 6465 496e 7465 726e  ruct, NodeIntern
+00197f30: 616c 2c20 4e6f 6465 293a 0a0a 2020 2222  al, Node):..  ""
 00197f40: 220a 0a20 2052 6574 7269 6576 6520 6765  "..  Retrieve ge
 00197f50: 6f6d 6574 7269 6320 696e 666f 726d 6174  ometric informat
 00197f60: 696f 6e20 6162 6f75 7420 7468 6520 6375  ion about the cu
 00197f70: 7272 656e 7420 7368 6164 696e 6720 706f  rrent shading po
 00197f80: 696e 740a 0a20 2022 2222 0a0a 2020 4063  int..  """..  @c
 00197f90: 6c61 7373 6d65 7468 6f64 0a0a 2020 6465  lassmethod..  de
 00197fa0: 6620 6973 5f72 6567 6973 7465 7265 645f  f is_registered_
@@ -104475,17 +104475,17 @@
 001981a0: 2062 6c5f 726e 615f 6765 745f 7375 6263   bl_rna_get_subc
 001981b0: 6c61 7373 5f70 7928 636c 732c 2069 643a  lass_py(cls, id:
 001981c0: 2073 7472 2c20 6465 6661 756c 743a 2074   str, default: t
 001981d0: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 001981e0: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 001981f0: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 00198200: 7320 5368 6164 6572 4e6f 6465 4e6f 726d  s ShaderNodeNorm
-00198210: 616c 2862 7079 5f73 7472 7563 742c 2053  al(bpy_struct, S
-00198220: 6861 6465 724e 6f64 652c 204e 6f64 652c  haderNode, Node,
-00198230: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+00198210: 616c 2853 6861 6465 724e 6f64 652c 2062  al(ShaderNode, b
+00198220: 7079 5f73 7472 7563 742c 204e 6f64 6549  py_struct, NodeI
+00198230: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 00198240: 0a20 2022 2222 0a0a 2020 4765 6e65 7261  .  """..  Genera
 00198250: 7465 2061 206e 6f72 6d61 6c20 7665 6374  te a normal vect
 00198260: 6f72 2061 6e64 2061 2064 6f74 2070 726f  or and a dot pro
 00198270: 6475 6374 0a0a 2020 2222 220a 0a20 2040  duct..  """..  @
 00198280: 636c 6173 736d 6574 686f 640a 0a20 2064  classmethod..  d
 00198290: 6566 2069 735f 7265 6769 7374 6572 6564  ef is_registered
 001982a0: 5f6e 6f64 655f 7479 7065 2863 6c73 2920  _node_type(cls) 
@@ -104522,18 +104522,18 @@
 00198490: 6620 626c 5f72 6e61 5f67 6574 5f73 7562  f bl_rna_get_sub
 001984a0: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 001984b0: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 001984c0: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 001984d0: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 001984e0: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 001984f0: 7373 2053 6861 6465 724e 6f64 654e 6f72  ss ShaderNodeNor
-00198500: 6d61 6c4d 6170 2862 7079 5f73 7472 7563  malMap(bpy_struc
-00198510: 742c 2053 6861 6465 724e 6f64 652c 204e  t, ShaderNode, N
-00198520: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-00198530: 6c29 3a0a 0a20 2022 2222 0a0a 2020 4765  l):..  """..  Ge
+00198500: 6d61 6c4d 6170 2853 6861 6465 724e 6f64  malMap(ShaderNod
+00198510: 652c 2062 7079 5f73 7472 7563 742c 204e  e, bpy_struct, N
+00198520: 6f64 6549 6e74 6572 6e61 6c2c 204e 6f64  odeInternal, Nod
+00198530: 6529 3a0a 0a20 2022 2222 0a0a 2020 4765  e):..  """..  Ge
 00198540: 6e65 7261 7465 2061 2070 6572 7475 7262  nerate a perturb
 00198550: 6564 206e 6f72 6d61 6c20 6672 6f6d 2061  ed normal from a
 00198560: 6e20 5247 4220 6e6f 726d 616c 206d 6170  n RGB normal map
 00198570: 2069 6d61 6765 2e20 5479 7069 6361 6c6c   image. Typicall
 00198580: 7920 7573 6564 2066 6f72 2066 616b 696e  y used for fakin
 00198590: 6720 6869 6768 6c79 2064 6574 6169 6c65  g highly detaile
 001985a0: 6420 7375 7266 6163 6573 0a0a 2020 2222  d surfaces..  ""
@@ -104607,18 +104607,18 @@
 001989e0: 0a20 2064 6566 2062 6c5f 726e 615f 6765  .  def bl_rna_ge
 001989f0: 745f 7375 6263 6c61 7373 5f70 7928 636c  t_subclass_py(cl
 00198a00: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 00198a10: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 00198a20: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 00198a30: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 00198a40: 0a0a 636c 6173 7320 5368 6164 6572 4e6f  ..class ShaderNo
-00198a50: 6465 4f62 6a65 6374 496e 666f 2862 7079  deObjectInfo(bpy
-00198a60: 5f73 7472 7563 742c 2053 6861 6465 724e  _struct, ShaderN
-00198a70: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-00198a80: 6e74 6572 6e61 6c29 3a0a 0a20 2022 2222  nternal):..  """
+00198a50: 6465 4f62 6a65 6374 496e 666f 2853 6861  deObjectInfo(Sha
+00198a60: 6465 724e 6f64 652c 2062 7079 5f73 7472  derNode, bpy_str
+00198a70: 7563 742c 204e 6f64 6549 6e74 6572 6e61  uct, NodeInterna
+00198a80: 6c2c 204e 6f64 6529 3a0a 0a20 2022 2222  l, Node):..  """
 00198a90: 0a0a 2020 5265 7472 6965 7665 2069 6e66  ..  Retrieve inf
 00198aa0: 6f72 6d61 7469 6f6e 2061 626f 7574 2074  ormation about t
 00198ab0: 6865 206f 626a 6563 7420 696e 7374 616e  he object instan
 00198ac0: 6365 0a0a 2020 2222 220a 0a20 2040 636c  ce..  """..  @cl
 00198ad0: 6173 736d 6574 686f 640a 0a20 2064 6566  assmethod..  def
 00198ae0: 2069 735f 7265 6769 7374 6572 6564 5f6e   is_registered_n
 00198af0: 6f64 655f 7479 7065 2863 6c73 2920 2d3e  ode_type(cls) ->
@@ -104655,17 +104655,17 @@
 00198ce0: 626c 5f72 6e61 5f67 6574 5f73 7562 636c  bl_rna_get_subcl
 00198cf0: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 00198d00: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 00198d10: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 00198d20: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 00198d30: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 00198d40: 2053 6861 6465 724e 6f64 654f 7574 7075   ShaderNodeOutpu
-00198d50: 7441 4f56 2862 7079 5f73 7472 7563 742c  tAOV(bpy_struct,
-00198d60: 2053 6861 6465 724e 6f64 652c 204e 6f64   ShaderNode, Nod
-00198d70: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+00198d50: 7441 4f56 2853 6861 6465 724e 6f64 652c  tAOV(ShaderNode,
+00198d60: 2062 7079 5f73 7472 7563 742c 204e 6f64   bpy_struct, Nod
+00198d70: 6549 6e74 6572 6e61 6c2c 204e 6f64 6529  eInternal, Node)
 00198d80: 3a0a 0a20 2022 2222 0a0a 2020 4172 6269  :..  """..  Arbi
 00198d90: 7472 6172 7920 4f75 7470 7574 2056 6172  trary Output Var
 00198da0: 6961 626c 6573 2e0a 5072 6f76 6964 6520  iables..Provide 
 00198db0: 6375 7374 6f6d 2072 656e 6465 7220 7061  custom render pa
 00198dc0: 7373 6573 2066 6f72 2061 7262 6974 7261  sses for arbitra
 00198dd0: 7279 2073 6861 6465 7220 6e6f 6465 206f  ry shader node o
 00198de0: 7574 7075 7473 0a0a 2020 2222 220a 0a20  utputs..  """.. 
@@ -104710,18 +104710,18 @@
 00199050: 6566 2062 6c5f 726e 615f 6765 745f 7375  ef bl_rna_get_su
 00199060: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 00199070: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 00199080: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 00199090: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 001990a0: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 001990b0: 6173 7320 5368 6164 6572 4e6f 6465 4f75  ass ShaderNodeOu
-001990c0: 7470 7574 4c69 6768 7428 6270 795f 7374  tputLight(bpy_st
-001990d0: 7275 6374 2c20 5368 6164 6572 4e6f 6465  ruct, ShaderNode
-001990e0: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-001990f0: 726e 616c 293a 0a0a 2020 2222 220a 0a20  rnal):..  """.. 
+001990c0: 7470 7574 4c69 6768 7428 5368 6164 6572  tputLight(Shader
+001990d0: 4e6f 6465 2c20 6270 795f 7374 7275 6374  Node, bpy_struct
+001990e0: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+001990f0: 4e6f 6465 293a 0a0a 2020 2222 220a 0a20  Node):..  """.. 
 00199100: 204f 7574 7075 7420 6c69 6768 7420 696e   Output light in
 00199110: 666f 726d 6174 696f 6e20 746f 2061 206c  formation to a l
 00199120: 6967 6874 206f 626a 6563 740a 0a20 2022  ight object..  "
 00199130: 2222 0a0a 2020 6973 5f61 6374 6976 655f  ""..  is_active_
 00199140: 6f75 7470 7574 3a20 626f 6f6c 203d 202e  output: bool = .
 00199150: 2e2e 0a0a 2020 2222 220a 0a20 2054 7275  ....  """..  Tru
 00199160: 6520 6966 2074 6869 7320 6e6f 6465 2069  e if this node i
@@ -104784,18 +104784,18 @@
 001994f0: 626c 5f72 6e61 5f67 6574 5f73 7562 636c  bl_rna_get_subcl
 00199500: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 00199510: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 00199520: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 00199530: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 00199540: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 00199550: 2053 6861 6465 724e 6f64 654f 7574 7075   ShaderNodeOutpu
-00199560: 744c 696e 6553 7479 6c65 2862 7079 5f73  tLineStyle(bpy_s
-00199570: 7472 7563 742c 2053 6861 6465 724e 6f64  truct, ShaderNod
-00199580: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-00199590: 6572 6e61 6c29 3a0a 0a20 2062 6c65 6e64  ernal):..  blend
+00199560: 744c 696e 6553 7479 6c65 2853 6861 6465  tLineStyle(Shade
+00199570: 724e 6f64 652c 2062 7079 5f73 7472 7563  rNode, bpy_struc
+00199580: 742c 204e 6f64 6549 6e74 6572 6e61 6c2c  t, NodeInternal,
+00199590: 204e 6f64 6529 3a0a 0a20 2062 6c65 6e64   Node):..  blend
 001995a0: 5f74 7970 653a 2073 7472 203d 202e 2e2e  _type: str = ...
 001995b0: 0a0a 2020 6973 5f61 6374 6976 655f 6f75  ..  is_active_ou
 001995c0: 7470 7574 3a20 626f 6f6c 203d 202e 2e2e  tput: bool = ...
 001995d0: 0a0a 2020 2222 220a 0a20 2054 7275 6520  ..  """..  True 
 001995e0: 6966 2074 6869 7320 6e6f 6465 2069 7320  if this node is 
 001995f0: 7573 6564 2061 7320 7468 6520 6163 7469  used as the acti
 00199600: 7665 206f 7574 7075 740a 0a20 2022 2222  ve output..  """
@@ -104867,18 +104867,18 @@
 00199a20: 6c5f 726e 615f 6765 745f 7375 6263 6c61  l_rna_get_subcla
 00199a30: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 00199a40: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 00199a50: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 00199a60: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 00199a70: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 00199a80: 5368 6164 6572 4e6f 6465 4f75 7470 7574  ShaderNodeOutput
-00199a90: 4d61 7465 7269 616c 2862 7079 5f73 7472  Material(bpy_str
-00199aa0: 7563 742c 2053 6861 6465 724e 6f64 652c  uct, ShaderNode,
-00199ab0: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-00199ac0: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+00199a90: 4d61 7465 7269 616c 2853 6861 6465 724e  Material(ShaderN
+00199aa0: 6f64 652c 2062 7079 5f73 7472 7563 742c  ode, bpy_struct,
+00199ab0: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+00199ac0: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 00199ad0: 4f75 7470 7574 2073 7572 6661 6365 206d  Output surface m
 00199ae0: 6174 6572 6961 6c20 696e 666f 726d 6174  aterial informat
 00199af0: 696f 6e20 666f 7220 7573 6520 696e 2072  ion for use in r
 00199b00: 656e 6465 7269 6e67 0a0a 2020 2222 220a  endering..  """.
 00199b10: 0a20 2069 735f 6163 7469 7665 5f6f 7574  .  is_active_out
 00199b20: 7075 743a 2062 6f6f 6c20 3d20 2e2e 2e0a  put: bool = ....
 00199b30: 0a20 2022 2222 0a0a 2020 5472 7565 2069  .  """..  True i
@@ -104942,17 +104942,17 @@
 00199ed0: 726e 615f 6765 745f 7375 6263 6c61 7373  rna_get_subclass
 00199ee0: 5f70 7928 636c 732c 2069 643a 2073 7472  _py(cls, id: str
 00199ef0: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 00199f00: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 00199f10: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 00199f20: 2020 202e 2e2e 0a0a 636c 6173 7320 5368     .....class Sh
 00199f30: 6164 6572 4e6f 6465 4f75 7470 7574 576f  aderNodeOutputWo
-00199f40: 726c 6428 6270 795f 7374 7275 6374 2c20  rld(bpy_struct, 
-00199f50: 5368 6164 6572 4e6f 6465 2c20 4e6f 6465  ShaderNode, Node
-00199f60: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+00199f40: 726c 6428 5368 6164 6572 4e6f 6465 2c20  rld(ShaderNode, 
+00199f50: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+00199f60: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 00199f70: 0a0a 2020 2222 220a 0a20 204f 7574 7075  ..  """..  Outpu
 00199f80: 7420 6c69 6768 7420 636f 6c6f 7220 696e  t light color in
 00199f90: 666f 726d 6174 696f 6e20 746f 2074 6865  formation to the
 00199fa0: 2073 6365 6e65 2773 2057 6f72 6c64 0a0a   scene's World..
 00199fb0: 2020 2222 220a 0a20 2069 735f 6163 7469    """..  is_acti
 00199fc0: 7665 5f6f 7574 7075 743a 2062 6f6f 6c20  ve_output: bool 
 00199fd0: 3d20 2e2e 2e0a 0a20 2022 2222 0a0a 2020  = .....  """..  
@@ -105016,18 +105016,18 @@
 0019a370: 6566 2062 6c5f 726e 615f 6765 745f 7375  ef bl_rna_get_su
 0019a380: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 0019a390: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 0019a3a0: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 0019a3b0: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 0019a3c0: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 0019a3d0: 6173 7320 5368 6164 6572 4e6f 6465 5061  ass ShaderNodePa
-0019a3e0: 7274 6963 6c65 496e 666f 2862 7079 5f73  rticleInfo(bpy_s
-0019a3f0: 7472 7563 742c 2053 6861 6465 724e 6f64  truct, ShaderNod
-0019a400: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-0019a410: 6572 6e61 6c29 3a0a 0a20 2022 2222 0a0a  ernal):..  """..
+0019a3e0: 7274 6963 6c65 496e 666f 2853 6861 6465  rticleInfo(Shade
+0019a3f0: 724e 6f64 652c 2062 7079 5f73 7472 7563  rNode, bpy_struc
+0019a400: 742c 204e 6f64 6549 6e74 6572 6e61 6c2c  t, NodeInternal,
+0019a410: 204e 6f64 6529 3a0a 0a20 2022 2222 0a0a   Node):..  """..
 0019a420: 2020 5265 7472 6965 7665 2074 6865 2064    Retrieve the d
 0019a430: 6174 6120 6f66 2074 6865 2070 6172 7469  ata of the parti
 0019a440: 636c 6520 7468 6174 2073 7061 776e 6564  cle that spawned
 0019a450: 2074 6865 206f 626a 6563 7420 696e 7374   the object inst
 0019a460: 616e 6365 2c20 666f 7220 6578 616d 706c  ance, for exampl
 0019a470: 6520 746f 2067 6976 6520 7661 7269 6174  e to give variat
 0019a480: 696f 6e20 746f 206d 756c 7469 706c 6520  ion to multiple 
@@ -105069,18 +105069,18 @@
 0019a6c0: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 0019a6d0: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 0019a6e0: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 0019a6f0: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 0019a700: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 0019a710: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 0019a720: 6c61 7373 2053 6861 6465 724e 6f64 6550  lass ShaderNodeP
-0019a730: 6f69 6e74 496e 666f 2862 7079 5f73 7472  ointInfo(bpy_str
-0019a740: 7563 742c 2053 6861 6465 724e 6f64 652c  uct, ShaderNode,
-0019a750: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-0019a760: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+0019a730: 6f69 6e74 496e 666f 2853 6861 6465 724e  ointInfo(ShaderN
+0019a740: 6f64 652c 2062 7079 5f73 7472 7563 742c  ode, bpy_struct,
+0019a750: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+0019a760: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 0019a770: 5265 7472 6965 7665 2069 6e66 6f72 6d61  Retrieve informa
 0019a780: 7469 6f6e 2061 626f 7574 2070 6f69 6e74  tion about point
 0019a790: 7320 696e 2061 2070 6f69 6e74 2063 6c6f  s in a point clo
 0019a7a0: 7564 0a0a 2020 2222 220a 0a20 2040 636c  ud..  """..  @cl
 0019a7b0: 6173 736d 6574 686f 640a 0a20 2064 6566  assmethod..  def
 0019a7c0: 2069 735f 7265 6769 7374 6572 6564 5f6e   is_registered_n
 0019a7d0: 6f64 655f 7479 7065 2863 6c73 2920 2d3e  ode_type(cls) ->
@@ -105116,18 +105116,18 @@
 0019a9b0: 7373 6d65 7468 6f64 0a0a 2020 6465 6620  ssmethod..  def 
 0019a9c0: 626c 5f72 6e61 5f67 6574 5f73 7562 636c  bl_rna_get_subcl
 0019a9d0: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 0019a9e0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 0019a9f0: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 0019aa00: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 0019aa10: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
-0019aa20: 2053 6861 6465 724e 6f64 6552 4742 2862   ShaderNodeRGB(b
-0019aa30: 7079 5f73 7472 7563 742c 2053 6861 6465  py_struct, Shade
-0019aa40: 724e 6f64 652c 204e 6f64 652c 204e 6f64  rNode, Node, Nod
-0019aa50: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2022  eInternal):..  "
+0019aa20: 2053 6861 6465 724e 6f64 6552 4742 2853   ShaderNodeRGB(S
+0019aa30: 6861 6465 724e 6f64 652c 2062 7079 5f73  haderNode, bpy_s
+0019aa40: 7472 7563 742c 204e 6f64 6549 6e74 6572  truct, NodeInter
+0019aa50: 6e61 6c2c 204e 6f64 6529 3a0a 0a20 2022  nal, Node):..  "
 0019aa60: 2222 0a0a 2020 4120 636f 6c6f 7220 7069  ""..  A color pi
 0019aa70: 636b 6572 0a0a 2020 2222 220a 0a20 2040  cker..  """..  @
 0019aa80: 636c 6173 736d 6574 686f 640a 0a20 2064  classmethod..  d
 0019aa90: 6566 2069 735f 7265 6769 7374 6572 6564  ef is_registered
 0019aaa0: 5f6e 6f64 655f 7479 7065 2863 6c73 2920  _node_type(cls) 
 0019aab0: 2d3e 2062 6f6f 6c3a 0a0a 2020 2020 2222  -> bool:..    ""
 0019aac0: 220a 0a20 2020 2054 7275 6520 6966 2061  "..    True if a
@@ -105162,17 +105162,17 @@
 0019ac90: 6620 626c 5f72 6e61 5f67 6574 5f73 7562  f bl_rna_get_sub
 0019aca0: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 0019acb0: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 0019acc0: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 0019acd0: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 0019ace0: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 0019acf0: 7373 2053 6861 6465 724e 6f64 6552 4742  ss ShaderNodeRGB
-0019ad00: 4375 7276 6528 6270 795f 7374 7275 6374  Curve(bpy_struct
-0019ad10: 2c20 5368 6164 6572 4e6f 6465 2c20 4e6f  , ShaderNode, No
-0019ad20: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+0019ad00: 4375 7276 6528 5368 6164 6572 4e6f 6465  Curve(ShaderNode
+0019ad10: 2c20 6270 795f 7374 7275 6374 2c20 4e6f  , bpy_struct, No
+0019ad20: 6465 496e 7465 726e 616c 2c20 4e6f 6465  deInternal, Node
 0019ad30: 293a 0a0a 2020 2222 220a 0a20 2041 7070  ):..  """..  App
 0019ad40: 6c79 2063 6f6c 6f72 2063 6f72 7265 6374  ly color correct
 0019ad50: 696f 6e73 2066 6f72 2065 6163 6820 636f  ions for each co
 0019ad60: 6c6f 7220 6368 616e 6e65 6c0a 0a20 2022  lor channel..  "
 0019ad70: 2222 0a0a 2020 6d61 7070 696e 673a 2043  ""..  mapping: C
 0019ad80: 7572 7665 4d61 7070 696e 6720 3d20 2e2e  urveMapping = ..
 0019ad90: 2e0a 0a20 2040 636c 6173 736d 6574 686f  ...  @classmetho
@@ -105211,18 +105211,18 @@
 0019afa0: 0a0a 2020 6465 6620 626c 5f72 6e61 5f67  ..  def bl_rna_g
 0019afb0: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 0019afc0: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 0019afd0: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 0019afe0: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 0019aff0: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 0019b000: 2e0a 0a63 6c61 7373 2053 6861 6465 724e  ...class ShaderN
-0019b010: 6f64 6552 4742 546f 4257 2862 7079 5f73  odeRGBToBW(bpy_s
-0019b020: 7472 7563 742c 2053 6861 6465 724e 6f64  truct, ShaderNod
-0019b030: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-0019b040: 6572 6e61 6c29 3a0a 0a20 2022 2222 0a0a  ernal):..  """..
+0019b010: 6f64 6552 4742 546f 4257 2853 6861 6465  odeRGBToBW(Shade
+0019b020: 724e 6f64 652c 2062 7079 5f73 7472 7563  rNode, bpy_struc
+0019b030: 742c 204e 6f64 6549 6e74 6572 6e61 6c2c  t, NodeInternal,
+0019b040: 204e 6f64 6529 3a0a 0a20 2022 2222 0a0a   Node):..  """..
 0019b050: 2020 436f 6e76 6572 7420 6120 636f 6c6f    Convert a colo
 0019b060: 7227 7320 6c75 6d69 6e61 6e63 6520 746f  r's luminance to
 0019b070: 2061 2067 7261 7973 6361 6c65 2076 616c   a grayscale val
 0019b080: 7565 0a0a 2020 2222 220a 0a20 2040 636c  ue..  """..  @cl
 0019b090: 6173 736d 6574 686f 640a 0a20 2064 6566  assmethod..  def
 0019b0a0: 2069 735f 7265 6769 7374 6572 6564 5f6e   is_registered_n
 0019b0b0: 6f64 655f 7479 7065 2863 6c73 2920 2d3e  ode_type(cls) ->
@@ -105259,17 +105259,17 @@
 0019b2a0: 626c 5f72 6e61 5f67 6574 5f73 7562 636c  bl_rna_get_subcl
 0019b2b0: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 0019b2c0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 0019b2d0: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 0019b2e0: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 0019b2f0: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 0019b300: 2053 6861 6465 724e 6f64 6553 6372 6970   ShaderNodeScrip
-0019b310: 7428 6270 795f 7374 7275 6374 2c20 5368  t(bpy_struct, Sh
-0019b320: 6164 6572 4e6f 6465 2c20 4e6f 6465 2c20  aderNode, Node, 
-0019b330: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+0019b310: 7428 5368 6164 6572 4e6f 6465 2c20 6270  t(ShaderNode, bp
+0019b320: 795f 7374 7275 6374 2c20 4e6f 6465 496e  y_struct, NodeIn
+0019b330: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 0019b340: 2020 2222 220a 0a20 2047 656e 6572 6174    """..  Generat
 0019b350: 6520 616e 204f 534c 2073 6861 6465 7220  e an OSL shader 
 0019b360: 6672 6f6d 2061 2066 696c 6520 6f72 2074  from a file or t
 0019b370: 6578 7420 6461 7461 2d62 6c6f 636b 2e0a  ext data-block..
 0019b380: 4e6f 7465 3a20 4f53 4c20 7368 6164 6572  Note: OSL shader
 0019b390: 7320 6172 6520 6e6f 7420 7375 7070 6f72  s are not suppor
 0019b3a0: 7465 6420 6f6e 2074 6865 2047 5055 0a0a  ted on the GPU..
@@ -105348,17 +105348,17 @@
 0019b830: 615f 6765 745f 7375 6263 6c61 7373 5f70  a_get_subclass_p
 0019b840: 7928 636c 732c 2069 643a 2073 7472 2c20  y(cls, id: str, 
 0019b850: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 0019b860: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 0019b870: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 0019b880: 202e 2e2e 0a0a 636c 6173 7320 5368 6164   .....class Shad
 0019b890: 6572 4e6f 6465 5365 7061 7261 7465 436f  erNodeSeparateCo
-0019b8a0: 6c6f 7228 6270 795f 7374 7275 6374 2c20  lor(bpy_struct, 
-0019b8b0: 5368 6164 6572 4e6f 6465 2c20 4e6f 6465  ShaderNode, Node
-0019b8c0: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+0019b8a0: 6c6f 7228 5368 6164 6572 4e6f 6465 2c20  lor(ShaderNode, 
+0019b8b0: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+0019b8c0: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 0019b8d0: 0a0a 2020 2222 220a 0a20 2053 706c 6974  ..  """..  Split
 0019b8e0: 2061 2063 6f6c 6f72 2069 6e74 6f20 6974   a color into it
 0019b8f0: 7320 696e 6469 7669 6475 616c 2063 6f6d  s individual com
 0019b900: 706f 6e65 6e74 7320 7573 696e 6720 6d75  ponents using mu
 0019b910: 6c74 6970 6c65 206d 6f64 656c 730a 0a20  ltiple models.. 
 0019b920: 2022 2222 0a0a 2020 6d6f 6465 3a20 7374   """..  mode: st
 0019b930: 7220 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  r = .....  """..
@@ -105409,18 +105409,18 @@
 0019bc00: 6620 626c 5f72 6e61 5f67 6574 5f73 7562  f bl_rna_get_sub
 0019bc10: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 0019bc20: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 0019bc30: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 0019bc40: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 0019bc50: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 0019bc60: 7373 2053 6861 6465 724e 6f64 6553 6570  ss ShaderNodeSep
-0019bc70: 6172 6174 6548 5356 2862 7079 5f73 7472  arateHSV(bpy_str
-0019bc80: 7563 742c 2053 6861 6465 724e 6f64 652c  uct, ShaderNode,
-0019bc90: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-0019bca0: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+0019bc70: 6172 6174 6548 5356 2853 6861 6465 724e  arateHSV(ShaderN
+0019bc80: 6f64 652c 2062 7079 5f73 7472 7563 742c  ode, bpy_struct,
+0019bc90: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+0019bca0: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 0019bcb0: 5370 6c69 7420 6120 636f 6c6f 7220 696e  Split a color in
 0019bcc0: 746f 2069 7473 2068 7565 2c20 7361 7475  to its hue, satu
 0019bcd0: 7261 7469 6f6e 2c20 616e 6420 7661 6c75  ration, and valu
 0019bce0: 6520 6368 616e 6e65 6c73 0a0a 2020 2222  e channels..  ""
 0019bcf0: 220a 0a20 2040 636c 6173 736d 6574 686f  "..  @classmetho
 0019bd00: 640a 0a20 2064 6566 2069 735f 7265 6769  d..  def is_regi
 0019bd10: 7374 6572 6564 5f6e 6f64 655f 7479 7065  stered_node_type
@@ -105457,18 +105457,18 @@
 0019bf00: 0a0a 2020 6465 6620 626c 5f72 6e61 5f67  ..  def bl_rna_g
 0019bf10: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 0019bf20: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 0019bf30: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 0019bf40: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 0019bf50: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 0019bf60: 2e0a 0a63 6c61 7373 2053 6861 6465 724e  ...class ShaderN
-0019bf70: 6f64 6553 6570 6172 6174 6552 4742 2862  odeSeparateRGB(b
-0019bf80: 7079 5f73 7472 7563 742c 2053 6861 6465  py_struct, Shade
-0019bf90: 724e 6f64 652c 204e 6f64 652c 204e 6f64  rNode, Node, Nod
-0019bfa0: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2022  eInternal):..  "
+0019bf70: 6f64 6553 6570 6172 6174 6552 4742 2853  odeSeparateRGB(S
+0019bf80: 6861 6465 724e 6f64 652c 2062 7079 5f73  haderNode, bpy_s
+0019bf90: 7472 7563 742c 204e 6f64 6549 6e74 6572  truct, NodeInter
+0019bfa0: 6e61 6c2c 204e 6f64 6529 3a0a 0a20 2022  nal, Node):..  "
 0019bfb0: 2222 0a0a 2020 5370 6c69 7420 6120 636f  ""..  Split a co
 0019bfc0: 6c6f 7220 696e 746f 2069 7473 2072 6564  lor into its red
 0019bfd0: 2c20 6772 6565 6e2c 2061 6e64 2062 6c75  , green, and blu
 0019bfe0: 6520 6368 616e 6e65 6c73 2028 4465 7072  e channels (Depr
 0019bff0: 6563 6174 6564 290a 0a20 2022 2222 0a0a  ecated)..  """..
 0019c000: 2020 4063 6c61 7373 6d65 7468 6f64 0a0a    @classmethod..
 0019c010: 2020 6465 6620 6973 5f72 6567 6973 7465    def is_registe
@@ -105506,18 +105506,18 @@
 0019c210: 2064 6566 2062 6c5f 726e 615f 6765 745f   def bl_rna_get_
 0019c220: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 0019c230: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 0019c240: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 0019c250: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 0019c260: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 0019c270: 636c 6173 7320 5368 6164 6572 4e6f 6465  class ShaderNode
-0019c280: 5365 7061 7261 7465 5859 5a28 6270 795f  SeparateXYZ(bpy_
-0019c290: 7374 7275 6374 2c20 5368 6164 6572 4e6f  struct, ShaderNo
-0019c2a0: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-0019c2b0: 7465 726e 616c 293a 0a0a 2020 2222 220a  ternal):..  """.
+0019c280: 5365 7061 7261 7465 5859 5a28 5368 6164  SeparateXYZ(Shad
+0019c290: 6572 4e6f 6465 2c20 6270 795f 7374 7275  erNode, bpy_stru
+0019c2a0: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+0019c2b0: 2c20 4e6f 6465 293a 0a0a 2020 2222 220a  , Node):..  """.
 0019c2c0: 0a20 2053 706c 6974 2061 2076 6563 746f  .  Split a vecto
 0019c2d0: 7220 696e 746f 2069 7473 2058 2c20 592c  r into its X, Y,
 0019c2e0: 2061 6e64 205a 2063 6f6d 706f 6e65 6e74   and Z component
 0019c2f0: 730a 0a20 2022 2222 0a0a 2020 4063 6c61  s..  """..  @cla
 0019c300: 7373 6d65 7468 6f64 0a0a 2020 6465 6620  ssmethod..  def 
 0019c310: 6973 5f72 6567 6973 7465 7265 645f 6e6f  is_registered_no
 0019c320: 6465 5f74 7970 6528 636c 7329 202d 3e20  de_type(cls) -> 
@@ -105554,17 +105554,17 @@
 0019c510: 6c5f 726e 615f 6765 745f 7375 6263 6c61  l_rna_get_subcla
 0019c520: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 0019c530: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 0019c540: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 0019c550: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 0019c560: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 0019c570: 5368 6164 6572 4e6f 6465 5368 6164 6572  ShaderNodeShader
-0019c580: 546f 5247 4228 6270 795f 7374 7275 6374  ToRGB(bpy_struct
-0019c590: 2c20 5368 6164 6572 4e6f 6465 2c20 4e6f  , ShaderNode, No
-0019c5a0: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+0019c580: 546f 5247 4228 5368 6164 6572 4e6f 6465  ToRGB(ShaderNode
+0019c590: 2c20 6270 795f 7374 7275 6374 2c20 4e6f  , bpy_struct, No
+0019c5a0: 6465 496e 7465 726e 616c 2c20 4e6f 6465  deInternal, Node
 0019c5b0: 293a 0a0a 2020 2222 220a 0a20 2043 6f6e  ):..  """..  Con
 0019c5c0: 7665 7274 2072 656e 6465 7269 6e67 2065  vert rendering e
 0019c5d0: 6666 6563 7420 2873 7563 6820 6173 206c  ffect (such as l
 0019c5e0: 6967 6874 2061 6e64 2073 6861 646f 7729  ight and shadow)
 0019c5f0: 2074 6f20 636f 6c6f 722e 2054 7970 6963   to color. Typic
 0019c600: 616c 6c79 2075 7365 6420 666f 7220 6e6f  ally used for no
 0019c610: 6e2d 7068 6f74 6f72 6561 6c69 7374 6963  n-photorealistic
@@ -105610,18 +105610,18 @@
 0019c890: 7468 6f64 0a0a 2020 6465 6620 626c 5f72  thod..  def bl_r
 0019c8a0: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 0019c8b0: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 0019c8c0: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 0019c8d0: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 0019c8e0: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 0019c8f0: 2020 2e2e 2e0a 0a63 6c61 7373 2053 6861    .....class Sha
-0019c900: 6465 724e 6f64 6553 7175 6565 7a65 2862  derNodeSqueeze(b
-0019c910: 7079 5f73 7472 7563 742c 2053 6861 6465  py_struct, Shade
-0019c920: 724e 6f64 652c 204e 6f64 652c 204e 6f64  rNode, Node, Nod
-0019c930: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2040  eInternal):..  @
+0019c900: 6465 724e 6f64 6553 7175 6565 7a65 2853  derNodeSqueeze(S
+0019c910: 6861 6465 724e 6f64 652c 2062 7079 5f73  haderNode, bpy_s
+0019c920: 7472 7563 742c 204e 6f64 6549 6e74 6572  truct, NodeInter
+0019c930: 6e61 6c2c 204e 6f64 6529 3a0a 0a20 2040  nal, Node):..  @
 0019c940: 636c 6173 736d 6574 686f 640a 0a20 2064  classmethod..  d
 0019c950: 6566 2069 735f 7265 6769 7374 6572 6564  ef is_registered
 0019c960: 5f6e 6f64 655f 7479 7065 2863 6c73 2920  _node_type(cls) 
 0019c970: 2d3e 2062 6f6f 6c3a 0a0a 2020 2020 2222  -> bool:..    ""
 0019c980: 220a 0a20 2020 2054 7275 6520 6966 2061  "..    True if a
 0019c990: 2072 6567 6973 7465 7265 6420 6e6f 6465   registered node
 0019c9a0: 2074 7970 650a 0a20 2020 2022 2222 0a0a   type..    """..
@@ -105655,17 +105655,17 @@
 0019cb60: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 0019cb70: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 0019cb80: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 0019cb90: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 0019cba0: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 0019cbb0: 7373 2053 6861 6465 724e 6f64 6553 7562  ss ShaderNodeSub
 0019cbc0: 7375 7266 6163 6553 6361 7474 6572 696e  surfaceScatterin
-0019cbd0: 6728 6270 795f 7374 7275 6374 2c20 5368  g(bpy_struct, Sh
-0019cbe0: 6164 6572 4e6f 6465 2c20 4e6f 6465 2c20  aderNode, Node, 
-0019cbf0: 4e6f 6465 496e 7465 726e 616c 293a 0a0a  NodeInternal):..
+0019cbd0: 6728 5368 6164 6572 4e6f 6465 2c20 6270  g(ShaderNode, bp
+0019cbe0: 795f 7374 7275 6374 2c20 4e6f 6465 496e  y_struct, NodeIn
+0019cbf0: 7465 726e 616c 2c20 4e6f 6465 293a 0a0a  ternal, Node):..
 0019cc00: 2020 2222 220a 0a20 2053 7562 7375 7266    """..  Subsurf
 0019cc10: 6163 6520 6d75 6c74 6970 6c65 2073 6361  ace multiple sca
 0019cc20: 7474 6572 696e 6720 7368 6164 6572 2074  ttering shader t
 0019cc30: 6f20 7369 6d75 6c61 7465 206c 6967 6874  o simulate light
 0019cc40: 2065 6e74 6572 696e 6720 7468 6520 7375   entering the su
 0019cc50: 7266 6163 6520 616e 6420 626f 756e 6369  rface and bounci
 0019cc60: 6e67 2069 6e74 6572 6e61 6c6c 792e 0a54  ng internally..T
@@ -105742,17 +105742,17 @@
 0019d0d0: 726e 615f 6765 745f 7375 6263 6c61 7373  rna_get_subclass
 0019d0e0: 5f70 7928 636c 732c 2069 643a 2073 7472  _py(cls, id: str
 0019d0f0: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 0019d100: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 0019d110: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 0019d120: 2020 202e 2e2e 0a0a 636c 6173 7320 5368     .....class Sh
 0019d130: 6164 6572 4e6f 6465 5461 6e67 656e 7428  aderNodeTangent(
-0019d140: 6270 795f 7374 7275 6374 2c20 5368 6164  bpy_struct, Shad
-0019d150: 6572 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  erNode, Node, No
-0019d160: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+0019d140: 5368 6164 6572 4e6f 6465 2c20 6270 795f  ShaderNode, bpy_
+0019d150: 7374 7275 6374 2c20 4e6f 6465 496e 7465  struct, NodeInte
+0019d160: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 0019d170: 2222 220a 0a20 2047 656e 6572 6174 6520  """..  Generate 
 0019d180: 6120 7461 6e67 656e 7420 6469 7265 6374  a tangent direct
 0019d190: 696f 6e20 666f 7220 7468 6520 416e 6973  ion for the Anis
 0019d1a0: 6f74 726f 7069 6320 4253 4446 0a0a 2020  otropic BSDF..  
 0019d1b0: 2222 220a 0a20 2061 7869 733a 2073 7472  """..  axis: str
 0019d1c0: 203d 202e 2e2e 0a0a 2020 2222 220a 0a20   = .....  """.. 
 0019d1d0: 2041 7869 7320 666f 7220 7261 6469 616c   Axis for radial
@@ -105814,18 +105814,18 @@
 0019d550: 640a 0a20 2064 6566 2062 6c5f 726e 615f  d..  def bl_rna_
 0019d560: 6765 745f 7375 6263 6c61 7373 5f70 7928  get_subclass_py(
 0019d570: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 0019d580: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 0019d590: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 0019d5a0: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 0019d5b0: 2e2e 0a0a 636c 6173 7320 5368 6164 6572  ....class Shader
-0019d5c0: 4e6f 6465 5465 7842 7269 636b 2862 7079  NodeTexBrick(bpy
-0019d5d0: 5f73 7472 7563 742c 2053 6861 6465 724e  _struct, ShaderN
-0019d5e0: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-0019d5f0: 6e74 6572 6e61 6c29 3a0a 0a20 2022 2222  nternal):..  """
+0019d5c0: 4e6f 6465 5465 7842 7269 636b 2853 6861  NodeTexBrick(Sha
+0019d5d0: 6465 724e 6f64 652c 2062 7079 5f73 7472  derNode, bpy_str
+0019d5e0: 7563 742c 204e 6f64 6549 6e74 6572 6e61  uct, NodeInterna
+0019d5f0: 6c2c 204e 6f64 6529 3a0a 0a20 2022 2222  l, Node):..  """
 0019d600: 0a0a 2020 4765 6e65 7261 7465 2061 2070  ..  Generate a p
 0019d610: 726f 6365 6475 7261 6c20 7465 7874 7572  rocedural textur
 0019d620: 6520 7072 6f64 7563 696e 6720 6272 6963  e producing bric
 0019d630: 6b73 0a0a 2020 2222 220a 0a20 2063 6f6c  ks..  """..  col
 0019d640: 6f72 5f6d 6170 7069 6e67 3a20 436f 6c6f  or_mapping: Colo
 0019d650: 724d 6170 7069 6e67 203d 202e 2e2e 0a0a  rMapping = .....
 0019d660: 2020 2222 220a 0a20 2043 6f6c 6f72 206d    """..  Color m
@@ -105879,18 +105879,18 @@
 0019d960: 6566 2062 6c5f 726e 615f 6765 745f 7375  ef bl_rna_get_su
 0019d970: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 0019d980: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 0019d990: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 0019d9a0: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 0019d9b0: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 0019d9c0: 6173 7320 5368 6164 6572 4e6f 6465 5465  ass ShaderNodeTe
-0019d9d0: 7843 6865 636b 6572 2862 7079 5f73 7472  xChecker(bpy_str
-0019d9e0: 7563 742c 2053 6861 6465 724e 6f64 652c  uct, ShaderNode,
-0019d9f0: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-0019da00: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+0019d9d0: 7843 6865 636b 6572 2853 6861 6465 724e  xChecker(ShaderN
+0019d9e0: 6f64 652c 2062 7079 5f73 7472 7563 742c  ode, bpy_struct,
+0019d9f0: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+0019da00: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 0019da10: 4765 6e65 7261 7465 2061 2063 6865 636b  Generate a check
 0019da20: 6572 626f 6172 6420 7465 7874 7572 650a  erboard texture.
 0019da30: 0a20 2022 2222 0a0a 2020 636f 6c6f 725f  .  """..  color_
 0019da40: 6d61 7070 696e 673a 2043 6f6c 6f72 4d61  mapping: ColorMa
 0019da50: 7070 696e 6720 3d20 2e2e 2e0a 0a20 2022  pping = .....  "
 0019da60: 2222 0a0a 2020 436f 6c6f 7220 6d61 7070  ""..  Color mapp
 0019da70: 696e 6720 7365 7474 696e 6773 0a0a 2020  ing settings..  
@@ -105936,18 +105936,18 @@
 0019dcf0: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 0019dd00: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 0019dd10: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 0019dd20: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 0019dd30: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 0019dd40: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 0019dd50: 6c61 7373 2053 6861 6465 724e 6f64 6554  lass ShaderNodeT
-0019dd60: 6578 436f 6f72 6428 6270 795f 7374 7275  exCoord(bpy_stru
-0019dd70: 6374 2c20 5368 6164 6572 4e6f 6465 2c20  ct, ShaderNode, 
-0019dd80: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-0019dd90: 616c 293a 0a0a 2020 2222 220a 0a20 2052  al):..  """..  R
+0019dd60: 6578 436f 6f72 6428 5368 6164 6572 4e6f  exCoord(ShaderNo
+0019dd70: 6465 2c20 6270 795f 7374 7275 6374 2c20  de, bpy_struct, 
+0019dd80: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+0019dd90: 6465 293a 0a0a 2020 2222 220a 0a20 2052  de):..  """..  R
 0019dda0: 6574 7269 6576 6520 6d75 6c74 6970 6c65  etrieve multiple
 0019ddb0: 2074 7970 6573 206f 6620 7465 7874 7572   types of textur
 0019ddc0: 6520 636f 6f72 6469 6e61 7465 732e 0a54  e coordinates..T
 0019ddd0: 7970 6963 616c 6c79 2075 7365 6420 6173  ypically used as
 0019dde0: 2069 6e70 7574 7320 666f 7220 7465 7874   inputs for text
 0019ddf0: 7572 6520 6e6f 6465 730a 0a20 2022 2222  ure nodes..  """
 0019de00: 0a0a 2020 6672 6f6d 5f69 6e73 7461 6e63  ..  from_instanc
@@ -106000,17 +106000,17 @@
 0019e0f0: 5f67 6574 5f73 7562 636c 6173 735f 7079  _get_subclass_py
 0019e100: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 0019e110: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 0019e120: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 0019e130: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 0019e140: 2e2e 2e0a 0a63 6c61 7373 2053 6861 6465  .....class Shade
 0019e150: 724e 6f64 6554 6578 456e 7669 726f 6e6d  rNodeTexEnvironm
-0019e160: 656e 7428 6270 795f 7374 7275 6374 2c20  ent(bpy_struct, 
-0019e170: 5368 6164 6572 4e6f 6465 2c20 4e6f 6465  ShaderNode, Node
-0019e180: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+0019e160: 656e 7428 5368 6164 6572 4e6f 6465 2c20  ent(ShaderNode, 
+0019e170: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+0019e180: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 0019e190: 0a0a 2020 2222 220a 0a20 2053 616d 706c  ..  """..  Sampl
 0019e1a0: 6520 616e 2069 6d61 6765 2066 696c 6520  e an image file 
 0019e1b0: 6173 2061 6e20 656e 7669 726f 6e6d 656e  as an environmen
 0019e1c0: 7420 7465 7874 7572 652e 2054 7970 6963  t texture. Typic
 0019e1d0: 616c 6c79 2075 7365 6420 746f 206c 6967  ally used to lig
 0019e1e0: 6874 2074 6865 2073 6365 6e65 2077 6974  ht the scene wit
 0019e1f0: 6820 7468 6520 6261 636b 6772 6f75 6e64  h the background
@@ -106106,17 +106106,17 @@
 0019e790: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 0019e7a0: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 0019e7b0: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 0019e7c0: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 0019e7d0: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 0019e7e0: 2020 2e2e 2e0a 0a63 6c61 7373 2053 6861    .....class Sha
 0019e7f0: 6465 724e 6f64 6554 6578 4772 6164 6965  derNodeTexGradie
-0019e800: 6e74 2862 7079 5f73 7472 7563 742c 2053  nt(bpy_struct, S
-0019e810: 6861 6465 724e 6f64 652c 204e 6f64 652c  haderNode, Node,
-0019e820: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+0019e800: 6e74 2853 6861 6465 724e 6f64 652c 2062  nt(ShaderNode, b
+0019e810: 7079 5f73 7472 7563 742c 204e 6f64 6549  py_struct, NodeI
+0019e820: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 0019e830: 0a20 2022 2222 0a0a 2020 4765 6e65 7261  .  """..  Genera
 0019e840: 7465 2069 6e74 6572 706f 6c61 7465 6420  te interpolated 
 0019e850: 636f 6c6f 7220 616e 6420 696e 7465 6e73  color and intens
 0019e860: 6974 7920 7661 6c75 6573 2062 6173 6564  ity values based
 0019e870: 206f 6e20 7468 6520 696e 7075 7420 7665   on the input ve
 0019e880: 6374 6f72 0a0a 2020 2222 220a 0a20 2063  ctor..  """..  c
 0019e890: 6f6c 6f72 5f6d 6170 7069 6e67 3a20 436f  olor_mapping: Co
@@ -106200,18 +106200,18 @@
 0019ed70: 2064 6566 2062 6c5f 726e 615f 6765 745f   def bl_rna_get_
 0019ed80: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 0019ed90: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 0019eda0: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 0019edb0: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 0019edc0: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 0019edd0: 636c 6173 7320 5368 6164 6572 4e6f 6465  class ShaderNode
-0019ede0: 5465 7849 4553 2862 7079 5f73 7472 7563  TexIES(bpy_struc
-0019edf0: 742c 2053 6861 6465 724e 6f64 652c 204e  t, ShaderNode, N
-0019ee00: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-0019ee10: 6c29 3a0a 0a20 2022 2222 0a0a 2020 5573  l):..  """..  Us
+0019ede0: 5465 7849 4553 2853 6861 6465 724e 6f64  TexIES(ShaderNod
+0019edf0: 652c 2062 7079 5f73 7472 7563 742c 204e  e, bpy_struct, N
+0019ee00: 6f64 6549 6e74 6572 6e61 6c2c 204e 6f64  odeInternal, Nod
+0019ee10: 6529 3a0a 0a20 2022 2222 0a0a 2020 5573  e):..  """..  Us
 0019ee20: 6564 2074 6f20 6d61 7463 6820 7265 616c  ed to match real
 0019ee30: 2077 6f72 6c64 206c 6967 6874 7320 7769   world lights wi
 0019ee40: 7468 2049 4553 2066 696c 6573 2c20 7768  th IES files, wh
 0019ee50: 6963 6820 7374 6f72 6520 7468 6520 6469  ich store the di
 0019ee60: 7265 6374 696f 6e61 6c20 696e 7465 6e73  rectional intens
 0019ee70: 6974 7920 6469 7374 7269 6275 7469 6f6e  ity distribution
 0019ee80: 206f 6620 6c69 6768 7420 736f 7572 6365   of light source
@@ -106272,18 +106272,18 @@
 0019f1f0: 2064 6566 2062 6c5f 726e 615f 6765 745f   def bl_rna_get_
 0019f200: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 0019f210: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 0019f220: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 0019f230: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 0019f240: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 0019f250: 636c 6173 7320 5368 6164 6572 4e6f 6465  class ShaderNode
-0019f260: 5465 7849 6d61 6765 2862 7079 5f73 7472  TexImage(bpy_str
-0019f270: 7563 742c 2053 6861 6465 724e 6f64 652c  uct, ShaderNode,
-0019f280: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-0019f290: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+0019f260: 5465 7849 6d61 6765 2853 6861 6465 724e  TexImage(ShaderN
+0019f270: 6f64 652c 2062 7079 5f73 7472 7563 742c  ode, bpy_struct,
+0019f280: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+0019f290: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 0019f2a0: 5361 6d70 6c65 2061 6e20 696d 6167 6520  Sample an image 
 0019f2b0: 6669 6c65 2061 7320 6120 7465 7874 7572  file as a textur
 0019f2c0: 650a 0a20 2022 2222 0a0a 2020 636f 6c6f  e..  """..  colo
 0019f2d0: 725f 6d61 7070 696e 673a 2043 6f6c 6f72  r_mapping: Color
 0019f2e0: 4d61 7070 696e 6720 3d20 2e2e 2e0a 0a20  Mapping = ..... 
 0019f2f0: 2022 2222 0a0a 2020 436f 6c6f 7220 6d61   """..  Color ma
 0019f300: 7070 696e 6720 7365 7474 696e 6773 0a0a  pping settings..
@@ -106420,18 +106420,18 @@
 0019fb30: 6566 2062 6c5f 726e 615f 6765 745f 7375  ef bl_rna_get_su
 0019fb40: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 0019fb50: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 0019fb60: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 0019fb70: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 0019fb80: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 0019fb90: 6173 7320 5368 6164 6572 4e6f 6465 5465  ass ShaderNodeTe
-0019fba0: 784d 6167 6963 2862 7079 5f73 7472 7563  xMagic(bpy_struc
-0019fbb0: 742c 2053 6861 6465 724e 6f64 652c 204e  t, ShaderNode, N
-0019fbc0: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-0019fbd0: 6c29 3a0a 0a20 2022 2222 0a0a 2020 4765  l):..  """..  Ge
+0019fba0: 784d 6167 6963 2853 6861 6465 724e 6f64  xMagic(ShaderNod
+0019fbb0: 652c 2062 7079 5f73 7472 7563 742c 204e  e, bpy_struct, N
+0019fbc0: 6f64 6549 6e74 6572 6e61 6c2c 204e 6f64  odeInternal, Nod
+0019fbd0: 6529 3a0a 0a20 2022 2222 0a0a 2020 4765  e):..  """..  Ge
 0019fbe0: 6e65 7261 7465 2061 2070 7379 6368 6564  nerate a psyched
 0019fbf0: 656c 6963 2063 6f6c 6f72 2074 6578 7475  elic color textu
 0019fc00: 7265 0a0a 2020 2222 220a 0a20 2063 6f6c  re..  """..  col
 0019fc10: 6f72 5f6d 6170 7069 6e67 3a20 436f 6c6f  or_mapping: Colo
 0019fc20: 724d 6170 7069 6e67 203d 202e 2e2e 0a0a  rMapping = .....
 0019fc30: 2020 2222 220a 0a20 2043 6f6c 6f72 206d    """..  Color m
 0019fc40: 6170 7069 6e67 2073 6574 7469 6e67 730a  apping settings.
@@ -106483,18 +106483,18 @@
 0019ff20: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 0019ff30: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 0019ff40: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 0019ff50: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 0019ff60: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 0019ff70: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 0019ff80: 6c61 7373 2053 6861 6465 724e 6f64 6554  lass ShaderNodeT
-0019ff90: 6578 4d75 7367 7261 7665 2862 7079 5f73  exMusgrave(bpy_s
-0019ffa0: 7472 7563 742c 2053 6861 6465 724e 6f64  truct, ShaderNod
-0019ffb0: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-0019ffc0: 6572 6e61 6c29 3a0a 0a20 2022 2222 0a0a  ernal):..  """..
+0019ff90: 6578 4d75 7367 7261 7665 2853 6861 6465  exMusgrave(Shade
+0019ffa0: 724e 6f64 652c 2062 7079 5f73 7472 7563  rNode, bpy_struc
+0019ffb0: 742c 204e 6f64 6549 6e74 6572 6e61 6c2c  t, NodeInternal,
+0019ffc0: 204e 6f64 6529 3a0a 0a20 2022 2222 0a0a   Node):..  """..
 0019ffd0: 2020 4765 6e65 7261 7465 2066 7261 6374    Generate fract
 0019ffe0: 616c 2050 6572 6c69 6e20 6e6f 6973 652e  al Perlin noise.
 0019fff0: 2041 6c6c 6f77 7320 666f 7220 6772 6561   Allows for grea
 001a0000: 7465 7220 636f 6e74 726f 6c20 6f76 6572  ter control over
 001a0010: 2068 6f77 206f 6374 6176 6573 2061 7265   how octaves are
 001a0020: 2063 6f6d 6269 6e65 6420 7468 616e 2074   combined than t
 001a0030: 6865 204e 6f69 7365 2054 6578 7475 7265  he Noise Texture
@@ -106604,17 +106604,17 @@
 001a06b0: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 001a06c0: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 001a06d0: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 001a06e0: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 001a06f0: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 001a0700: 2020 2e2e 2e0a 0a63 6c61 7373 2053 6861    .....class Sha
 001a0710: 6465 724e 6f64 6554 6578 4e6f 6973 6528  derNodeTexNoise(
-001a0720: 6270 795f 7374 7275 6374 2c20 5368 6164  bpy_struct, Shad
-001a0730: 6572 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  erNode, Node, No
-001a0740: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+001a0720: 5368 6164 6572 4e6f 6465 2c20 6270 795f  ShaderNode, bpy_
+001a0730: 7374 7275 6374 2c20 4e6f 6465 496e 7465  struct, NodeInte
+001a0740: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 001a0750: 2222 220a 0a20 2047 656e 6572 6174 6520  """..  Generate 
 001a0760: 6672 6163 7461 6c20 5065 726c 696e 206e  fractal Perlin n
 001a0770: 6f69 7365 0a0a 2020 2222 220a 0a20 2063  oise..  """..  c
 001a0780: 6f6c 6f72 5f6d 6170 7069 6e67 3a20 436f  olor_mapping: Co
 001a0790: 6c6f 724d 6170 7069 6e67 203d 202e 2e2e  lorMapping = ...
 001a07a0: 0a0a 2020 2222 220a 0a20 2043 6f6c 6f72  ..  """..  Color
 001a07b0: 206d 6170 7069 6e67 2073 6574 7469 6e67   mapping setting
@@ -106682,17 +106682,17 @@
 001a0b90: 6765 745f 7375 6263 6c61 7373 5f70 7928  get_subclass_py(
 001a0ba0: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 001a0bb0: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 001a0bc0: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 001a0bd0: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 001a0be0: 2e2e 0a0a 636c 6173 7320 5368 6164 6572  ....class Shader
 001a0bf0: 4e6f 6465 5465 7850 6f69 6e74 4465 6e73  NodeTexPointDens
-001a0c00: 6974 7928 6270 795f 7374 7275 6374 2c20  ity(bpy_struct, 
-001a0c10: 5368 6164 6572 4e6f 6465 2c20 4e6f 6465  ShaderNode, Node
-001a0c20: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+001a0c00: 6974 7928 5368 6164 6572 4e6f 6465 2c20  ity(ShaderNode, 
+001a0c10: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+001a0c20: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 001a0c30: 0a0a 2020 2222 220a 0a20 2047 656e 6572  ..  """..  Gener
 001a0c40: 6174 6520 6120 766f 6c75 6d65 7472 6963  ate a volumetric
 001a0c50: 2070 6f69 6e74 2066 6f72 2065 6163 6820   point for each 
 001a0c60: 7061 7274 6963 6c65 206f 7220 7665 7274  particle or vert
 001a0c70: 6578 206f 6620 616e 6f74 6865 7220 6f62  ex of another ob
 001a0c80: 6a65 6374 0a0a 2020 2222 220a 0a20 2069  ject..  """..  i
 001a0c90: 6e74 6572 706f 6c61 7469 6f6e 3a20 7374  nterpolation: st
@@ -106862,18 +106862,18 @@
 001a16d0: 2020 6465 6620 626c 5f72 6e61 5f67 6574    def bl_rna_get
 001a16e0: 5f73 7562 636c 6173 735f 7079 2863 6c73  _subclass_py(cls
 001a16f0: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 001a1700: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 001a1710: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 001a1720: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 001a1730: 0a63 6c61 7373 2053 6861 6465 724e 6f64  .class ShaderNod
-001a1740: 6554 6578 536b 7928 6270 795f 7374 7275  eTexSky(bpy_stru
-001a1750: 6374 2c20 5368 6164 6572 4e6f 6465 2c20  ct, ShaderNode, 
-001a1760: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-001a1770: 616c 293a 0a0a 2020 2222 220a 0a20 2047  al):..  """..  G
+001a1740: 6554 6578 536b 7928 5368 6164 6572 4e6f  eTexSky(ShaderNo
+001a1750: 6465 2c20 6270 795f 7374 7275 6374 2c20  de, bpy_struct, 
+001a1760: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+001a1770: 6465 293a 0a0a 2020 2222 220a 0a20 2047  de):..  """..  G
 001a1780: 656e 6572 6174 6520 6120 7072 6f63 6564  enerate a proced
 001a1790: 7572 616c 2073 6b79 2074 6578 7475 7265  ural sky texture
 001a17a0: 0a0a 2020 2222 220a 0a20 2061 6972 5f64  ..  """..  air_d
 001a17b0: 656e 7369 7479 3a20 666c 6f61 7420 3d20  ensity: float = 
 001a17c0: 2e2e 2e0a 0a20 2022 2222 0a0a 2020 4465  .....  """..  De
 001a17d0: 6e73 6974 7920 6f66 2061 6972 206d 6f6c  nsity of air mol
 001a17e0: 6563 756c 6573 0a0a 2020 2222 220a 0a20  ecules..  """.. 
@@ -106990,17 +106990,17 @@
 001a1ed0: 726e 615f 6765 745f 7375 6263 6c61 7373  rna_get_subclass
 001a1ee0: 5f70 7928 636c 732c 2069 643a 2073 7472  _py(cls, id: str
 001a1ef0: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 001a1f00: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 001a1f10: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 001a1f20: 2020 202e 2e2e 0a0a 636c 6173 7320 5368     .....class Sh
 001a1f30: 6164 6572 4e6f 6465 5465 7856 6f72 6f6e  aderNodeTexVoron
-001a1f40: 6f69 2862 7079 5f73 7472 7563 742c 2053  oi(bpy_struct, S
-001a1f50: 6861 6465 724e 6f64 652c 204e 6f64 652c  haderNode, Node,
-001a1f60: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+001a1f40: 6f69 2853 6861 6465 724e 6f64 652c 2062  oi(ShaderNode, b
+001a1f50: 7079 5f73 7472 7563 742c 204e 6f64 6549  py_struct, NodeI
+001a1f60: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 001a1f70: 0a20 2022 2222 0a0a 2020 4765 6e65 7261  .  """..  Genera
 001a1f80: 7465 2057 6f72 6c65 7920 6e6f 6973 6520  te Worley noise 
 001a1f90: 6261 7365 6420 6f6e 2074 6865 2064 6973  based on the dis
 001a1fa0: 7461 6e63 6520 746f 2072 616e 646f 6d20  tance to random 
 001a1fb0: 706f 696e 7473 2e20 5479 7069 6361 6c6c  points. Typicall
 001a1fc0: 7920 7573 6564 2074 6f20 6765 6e65 7261  y used to genera
 001a1fd0: 7465 2074 6578 7475 7265 7320 7375 6368  te textures such
@@ -107130,18 +107130,18 @@
 001a2790: 2020 6465 6620 626c 5f72 6e61 5f67 6574    def bl_rna_get
 001a27a0: 5f73 7562 636c 6173 735f 7079 2863 6c73  _subclass_py(cls
 001a27b0: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 001a27c0: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 001a27d0: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 001a27e0: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 001a27f0: 0a63 6c61 7373 2053 6861 6465 724e 6f64  .class ShaderNod
-001a2800: 6554 6578 5761 7665 2862 7079 5f73 7472  eTexWave(bpy_str
-001a2810: 7563 742c 2053 6861 6465 724e 6f64 652c  uct, ShaderNode,
-001a2820: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-001a2830: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+001a2800: 6554 6578 5761 7665 2853 6861 6465 724e  eTexWave(ShaderN
+001a2810: 6f64 652c 2062 7079 5f73 7472 7563 742c  ode, bpy_struct,
+001a2820: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+001a2830: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 001a2840: 4765 6e65 7261 7465 2070 726f 6365 6475  Generate procedu
 001a2850: 7261 6c20 6261 6e64 7320 6f72 2072 696e  ral bands or rin
 001a2860: 6773 2077 6974 6820 6e6f 6973 650a 0a20  gs with noise.. 
 001a2870: 2022 2222 0a0a 2020 6261 6e64 735f 6469   """..  bands_di
 001a2880: 7265 6374 696f 6e3a 2073 7472 203d 202e  rection: str = .
 001a2890: 2e2e 0a0a 2020 2222 220a 0a20 202a 2060  ....  """..  * `
 001a28a0: 6058 6060 0a58 202d 2d20 4261 6e64 7320  `X``.X -- Bands 
@@ -107236,17 +107236,17 @@
 001a2e30: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 001a2e40: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 001a2e50: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 001a2e60: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 001a2e70: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 001a2e80: 2020 2e2e 2e0a 0a63 6c61 7373 2053 6861    .....class Sha
 001a2e90: 6465 724e 6f64 6554 6578 5768 6974 654e  derNodeTexWhiteN
-001a2ea0: 6f69 7365 2862 7079 5f73 7472 7563 742c  oise(bpy_struct,
-001a2eb0: 2053 6861 6465 724e 6f64 652c 204e 6f64   ShaderNode, Nod
-001a2ec0: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+001a2ea0: 6f69 7365 2853 6861 6465 724e 6f64 652c  oise(ShaderNode,
+001a2eb0: 2062 7079 5f73 7472 7563 742c 204e 6f64   bpy_struct, Nod
+001a2ec0: 6549 6e74 6572 6e61 6c2c 204e 6f64 6529  eInternal, Node)
 001a2ed0: 3a0a 0a20 2022 2222 0a0a 2020 5265 7475  :..  """..  Retu
 001a2ee0: 726e 2061 2072 616e 646f 6d20 7661 6c75  rn a random valu
 001a2ef0: 6520 6f72 2063 6f6c 6f72 2062 6173 6564  e or color based
 001a2f00: 206f 6e20 616e 2069 6e70 7574 2073 6565   on an input see
 001a2f10: 640a 0a20 2022 2222 0a0a 2020 6e6f 6973  d..  """..  nois
 001a2f20: 655f 6469 6d65 6e73 696f 6e73 3a20 7374  e_dimensions: st
 001a2f30: 7220 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  r = .....  """..
@@ -107305,18 +107305,18 @@
 001a3280: 6c5f 726e 615f 6765 745f 7375 6263 6c61  l_rna_get_subcla
 001a3290: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 001a32a0: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 001a32b0: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 001a32c0: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 001a32d0: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 001a32e0: 5368 6164 6572 4e6f 6465 5556 416c 6f6e  ShaderNodeUVAlon
-001a32f0: 6753 7472 6f6b 6528 6270 795f 7374 7275  gStroke(bpy_stru
-001a3300: 6374 2c20 5368 6164 6572 4e6f 6465 2c20  ct, ShaderNode, 
-001a3310: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-001a3320: 616c 293a 0a0a 2020 7573 655f 7469 7073  al):..  use_tips
+001a32f0: 6753 7472 6f6b 6528 5368 6164 6572 4e6f  gStroke(ShaderNo
+001a3300: 6465 2c20 6270 795f 7374 7275 6374 2c20  de, bpy_struct, 
+001a3310: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+001a3320: 6465 293a 0a0a 2020 7573 655f 7469 7073  de):..  use_tips
 001a3330: 3a20 626f 6f6c 203d 202e 2e2e 0a0a 2020  : bool = .....  
 001a3340: 2222 220a 0a20 204c 6f77 6572 2068 616c  """..  Lower hal
 001a3350: 6620 6f66 2074 6865 2074 6578 7475 7265  f of the texture
 001a3360: 2069 7320 666f 7220 7469 7073 206f 6620   is for tips of 
 001a3370: 7468 6520 7374 726f 6b65 0a0a 2020 2222  the stroke..  ""
 001a3380: 220a 0a20 2040 636c 6173 736d 6574 686f  "..  @classmetho
 001a3390: 640a 0a20 2064 6566 2069 735f 7265 6769  d..  def is_regi
@@ -107354,18 +107354,18 @@
 001a3590: 0a0a 2020 6465 6620 626c 5f72 6e61 5f67  ..  def bl_rna_g
 001a35a0: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 001a35b0: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 001a35c0: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 001a35d0: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 001a35e0: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 001a35f0: 2e0a 0a63 6c61 7373 2053 6861 6465 724e  ...class ShaderN
-001a3600: 6f64 6555 564d 6170 2862 7079 5f73 7472  odeUVMap(bpy_str
-001a3610: 7563 742c 2053 6861 6465 724e 6f64 652c  uct, ShaderNode,
-001a3620: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-001a3630: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+001a3600: 6f64 6555 564d 6170 2853 6861 6465 724e  odeUVMap(ShaderN
+001a3610: 6f64 652c 2062 7079 5f73 7472 7563 742c  ode, bpy_struct,
+001a3620: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+001a3630: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 001a3640: 5265 7472 6965 7665 2061 2055 5620 6d61  Retrieve a UV ma
 001a3650: 7020 6672 6f6d 2074 6865 2067 656f 6d65  p from the geome
 001a3660: 7472 792c 206f 7220 7468 6520 6465 6661  try, or the defa
 001a3670: 756c 7420 6661 6c6c 6261 636b 2069 6620  ult fallback if 
 001a3680: 6e6f 6e65 2069 7320 7370 6563 6966 6965  none is specifie
 001a3690: 640a 0a20 2022 2222 0a0a 2020 6672 6f6d  d..  """..  from
 001a36a0: 5f69 6e73 7461 6e63 6572 3a20 626f 6f6c  _instancer: bool
@@ -107415,17 +107415,17 @@
 001a3960: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 001a3970: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 001a3980: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 001a3990: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 001a39a0: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 001a39b0: 2020 2e2e 2e0a 0a63 6c61 7373 2053 6861    .....class Sha
 001a39c0: 6465 724e 6f64 6556 616c 546f 5247 4228  derNodeValToRGB(
-001a39d0: 6270 795f 7374 7275 6374 2c20 5368 6164  bpy_struct, Shad
-001a39e0: 6572 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  erNode, Node, No
-001a39f0: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+001a39d0: 5368 6164 6572 4e6f 6465 2c20 6270 795f  ShaderNode, bpy_
+001a39e0: 7374 7275 6374 2c20 4e6f 6465 496e 7465  struct, NodeInte
+001a39f0: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 001a3a00: 2222 220a 0a20 204d 6170 2076 616c 7565  """..  Map value
 001a3a10: 7320 746f 2063 6f6c 6f72 7320 7769 7468  s to colors with
 001a3a20: 2074 6865 2075 7365 206f 6620 6120 6772   the use of a gr
 001a3a30: 6164 6965 6e74 0a0a 2020 2222 220a 0a20  adient..  """.. 
 001a3a40: 2063 6f6c 6f72 5f72 616d 703a 2043 6f6c   color_ramp: Col
 001a3a50: 6f72 5261 6d70 203d 202e 2e2e 0a0a 2020  orRamp = .....  
 001a3a60: 4063 6c61 7373 6d65 7468 6f64 0a0a 2020  @classmethod..  
@@ -107464,17 +107464,17 @@
 001a3c70: 6566 2062 6c5f 726e 615f 6765 745f 7375  ef bl_rna_get_su
 001a3c80: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 001a3c90: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 001a3ca0: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 001a3cb0: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 001a3cc0: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 001a3cd0: 6173 7320 5368 6164 6572 4e6f 6465 5661  ass ShaderNodeVa
-001a3ce0: 6c75 6528 6270 795f 7374 7275 6374 2c20  lue(bpy_struct, 
-001a3cf0: 5368 6164 6572 4e6f 6465 2c20 4e6f 6465  ShaderNode, Node
-001a3d00: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+001a3ce0: 6c75 6528 5368 6164 6572 4e6f 6465 2c20  lue(ShaderNode, 
+001a3cf0: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+001a3d00: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 001a3d10: 0a0a 2020 2222 220a 0a20 2055 7365 6420  ..  """..  Used 
 001a3d20: 746f 2049 6e70 7574 206e 756d 6572 6963  to Input numeric
 001a3d30: 616c 2076 616c 7565 7320 746f 206f 7468  al values to oth
 001a3d40: 6572 206e 6f64 6573 2069 6e20 7468 6520  er nodes in the 
 001a3d50: 7472 6565 0a0a 2020 2222 220a 0a20 2040  tree..  """..  @
 001a3d60: 636c 6173 736d 6574 686f 640a 0a20 2064  classmethod..  d
 001a3d70: 6566 2069 735f 7265 6769 7374 6572 6564  ef is_registered
@@ -107512,18 +107512,18 @@
 001a3f70: 6620 626c 5f72 6e61 5f67 6574 5f73 7562  f bl_rna_get_sub
 001a3f80: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 001a3f90: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 001a3fa0: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 001a3fb0: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 001a3fc0: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 001a3fd0: 7373 2053 6861 6465 724e 6f64 6556 6563  ss ShaderNodeVec
-001a3fe0: 746f 7243 7572 7665 2862 7079 5f73 7472  torCurve(bpy_str
-001a3ff0: 7563 742c 2053 6861 6465 724e 6f64 652c  uct, ShaderNode,
-001a4000: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-001a4010: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+001a3fe0: 746f 7243 7572 7665 2853 6861 6465 724e  torCurve(ShaderN
+001a3ff0: 6f64 652c 2062 7079 5f73 7472 7563 742c  ode, bpy_struct,
+001a4000: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+001a4010: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 001a4020: 4d61 7020 616e 2069 6e70 7574 2076 6563  Map an input vec
 001a4030: 746f 7273 2074 6f20 6375 7276 6573 2c20  tors to curves, 
 001a4040: 7573 6564 2074 6f20 6669 6e65 2d74 756e  used to fine-tun
 001a4050: 6520 7468 6520 696e 7465 7270 6f6c 6174  e the interpolat
 001a4060: 696f 6e20 6f66 2074 6865 2069 6e70 7574  ion of the input
 001a4070: 0a0a 2020 2222 220a 0a20 206d 6170 7069  ..  """..  mappi
 001a4080: 6e67 3a20 4375 7276 654d 6170 7069 6e67  ng: CurveMapping
@@ -107564,18 +107564,18 @@
 001a42b0: 726e 615f 6765 745f 7375 6263 6c61 7373  rna_get_subclass
 001a42c0: 5f70 7928 636c 732c 2069 643a 2073 7472  _py(cls, id: str
 001a42d0: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 001a42e0: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 001a42f0: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 001a4300: 2020 202e 2e2e 0a0a 636c 6173 7320 5368     .....class Sh
 001a4310: 6164 6572 4e6f 6465 5665 6374 6f72 4469  aderNodeVectorDi
-001a4320: 7370 6c61 6365 6d65 6e74 2862 7079 5f73  splacement(bpy_s
-001a4330: 7472 7563 742c 2053 6861 6465 724e 6f64  truct, ShaderNod
-001a4340: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-001a4350: 6572 6e61 6c29 3a0a 0a20 2022 2222 0a0a  ernal):..  """..
+001a4320: 7370 6c61 6365 6d65 6e74 2853 6861 6465  splacement(Shade
+001a4330: 724e 6f64 652c 2062 7079 5f73 7472 7563  rNode, bpy_struc
+001a4340: 742c 204e 6f64 6549 6e74 6572 6e61 6c2c  t, NodeInternal,
+001a4350: 204e 6f64 6529 3a0a 0a20 2022 2222 0a0a   Node):..  """..
 001a4360: 2020 4469 7370 6c61 6365 2074 6865 2073    Displace the s
 001a4370: 7572 6661 6365 2061 6c6f 6e67 2061 6e20  urface along an 
 001a4380: 6172 6269 7472 6172 7920 6469 7265 6374  arbitrary direct
 001a4390: 696f 6e0a 0a20 2022 2222 0a0a 2020 7370  ion..  """..  sp
 001a43a0: 6163 653a 2073 7472 203d 202e 2e2e 0a0a  ace: str = .....
 001a43b0: 2020 2222 220a 0a20 2053 7061 6365 206f    """..  Space o
 001a43c0: 6620 7468 6520 696e 7075 7420 6865 6967  f the input heig
@@ -107630,17 +107630,17 @@
 001a46d0: 5f72 6e61 5f67 6574 5f73 7562 636c 6173  _rna_get_subclas
 001a46e0: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 001a46f0: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 001a4700: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 001a4710: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 001a4720: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2053      .....class S
 001a4730: 6861 6465 724e 6f64 6556 6563 746f 724d  haderNodeVectorM
-001a4740: 6174 6828 6270 795f 7374 7275 6374 2c20  ath(bpy_struct, 
-001a4750: 5368 6164 6572 4e6f 6465 2c20 4e6f 6465  ShaderNode, Node
-001a4760: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+001a4740: 6174 6828 5368 6164 6572 4e6f 6465 2c20  ath(ShaderNode, 
+001a4750: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+001a4760: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 001a4770: 0a0a 2020 2222 220a 0a20 2050 6572 666f  ..  """..  Perfo
 001a4780: 726d 2076 6563 746f 7220 6d61 7468 206f  rm vector math o
 001a4790: 7065 7261 7469 6f6e 0a0a 2020 2222 220a  peration..  """.
 001a47a0: 0a20 206f 7065 7261 7469 6f6e 3a20 7374  .  operation: st
 001a47b0: 7220 3d20 2e2e 2e0a 0a20 2040 636c 6173  r = .....  @clas
 001a47c0: 736d 6574 686f 640a 0a20 2064 6566 2069  smethod..  def i
 001a47d0: 735f 7265 6769 7374 6572 6564 5f6e 6f64  s_registered_nod
@@ -107678,17 +107678,17 @@
 001a49d0: 5f72 6e61 5f67 6574 5f73 7562 636c 6173  _rna_get_subclas
 001a49e0: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 001a49f0: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 001a4a00: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 001a4a10: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 001a4a20: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2053      .....class S
 001a4a30: 6861 6465 724e 6f64 6556 6563 746f 7252  haderNodeVectorR
-001a4a40: 6f74 6174 6528 6270 795f 7374 7275 6374  otate(bpy_struct
-001a4a50: 2c20 5368 6164 6572 4e6f 6465 2c20 4e6f  , ShaderNode, No
-001a4a60: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+001a4a40: 6f74 6174 6528 5368 6164 6572 4e6f 6465  otate(ShaderNode
+001a4a50: 2c20 6270 795f 7374 7275 6374 2c20 4e6f  , bpy_struct, No
+001a4a60: 6465 496e 7465 726e 616c 2c20 4e6f 6465  deInternal, Node
 001a4a70: 293a 0a0a 2020 2222 220a 0a20 2052 6f74  ):..  """..  Rot
 001a4a80: 6174 6520 6120 7665 6374 6f72 2061 726f  ate a vector aro
 001a4a90: 756e 6420 6120 7069 766f 7420 706f 696e  und a pivot poin
 001a4aa0: 7420 2863 656e 7465 7229 0a0a 2020 2222  t (center)..  ""
 001a4ab0: 220a 0a20 2069 6e76 6572 743a 2062 6f6f  "..  invert: boo
 001a4ac0: 6c20 3d20 2e2e 2e0a 0a20 2022 2222 0a0a  l = .....  """..
 001a4ad0: 2020 496e 7665 7274 2061 6e67 6c65 0a0a    Invert angle..
@@ -107751,18 +107751,18 @@
 001a4e60: 5f72 6e61 5f67 6574 5f73 7562 636c 6173  _rna_get_subclas
 001a4e70: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 001a4e80: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 001a4e90: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 001a4ea0: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 001a4eb0: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2053      .....class S
 001a4ec0: 6861 6465 724e 6f64 6556 6563 746f 7254  haderNodeVectorT
-001a4ed0: 7261 6e73 666f 726d 2862 7079 5f73 7472  ransform(bpy_str
-001a4ee0: 7563 742c 2053 6861 6465 724e 6f64 652c  uct, ShaderNode,
-001a4ef0: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-001a4f00: 6e61 6c29 3a0a 0a20 2022 2222 0a0a 2020  nal):..  """..  
+001a4ed0: 7261 6e73 666f 726d 2853 6861 6465 724e  ransform(ShaderN
+001a4ee0: 6f64 652c 2062 7079 5f73 7472 7563 742c  ode, bpy_struct,
+001a4ef0: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+001a4f00: 6f64 6529 3a0a 0a20 2022 2222 0a0a 2020  ode):..  """..  
 001a4f10: 436f 6e76 6572 7420 6120 7665 6374 6f72  Convert a vector
 001a4f20: 2c20 706f 696e 742c 206f 7220 6e6f 726d  , point, or norm
 001a4f30: 616c 2062 6574 7765 656e 2077 6f72 6c64  al between world
 001a4f40: 2c20 6361 6d65 7261 2c20 616e 6420 6f62  , camera, and ob
 001a4f50: 6a65 6374 2063 6f6f 7264 696e 6174 6520  ject coordinate 
 001a4f60: 7370 6163 650a 0a20 2022 2222 0a0a 2020  space..  """..  
 001a4f70: 636f 6e76 6572 745f 6672 6f6d 3a20 7374  convert_from: st
@@ -107822,18 +107822,18 @@
 001a52d0: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 001a52e0: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 001a52f0: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 001a5300: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 001a5310: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 001a5320: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 001a5330: 6c61 7373 2053 6861 6465 724e 6f64 6556  lass ShaderNodeV
-001a5340: 6572 7465 7843 6f6c 6f72 2862 7079 5f73  ertexColor(bpy_s
-001a5350: 7472 7563 742c 2053 6861 6465 724e 6f64  truct, ShaderNod
-001a5360: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-001a5370: 6572 6e61 6c29 3a0a 0a20 2022 2222 0a0a  ernal):..  """..
+001a5340: 6572 7465 7843 6f6c 6f72 2853 6861 6465  ertexColor(Shade
+001a5350: 724e 6f64 652c 2062 7079 5f73 7472 7563  rNode, bpy_struc
+001a5360: 742c 204e 6f64 6549 6e74 6572 6e61 6c2c  t, NodeInternal,
+001a5370: 204e 6f64 6529 3a0a 0a20 2022 2222 0a0a   Node):..  """..
 001a5380: 2020 5265 7472 6965 7665 2061 2063 6f6c    Retrieve a col
 001a5390: 6f72 2061 7474 7269 6275 7465 2c20 6f72  or attribute, or
 001a53a0: 2074 6865 2064 6566 6175 6c74 2066 616c   the default fal
 001a53b0: 6c62 6163 6b20 6966 206e 6f6e 6520 6973  lback if none is
 001a53c0: 2073 7065 6369 6669 6564 0a0a 2020 2222   specified..  ""
 001a53d0: 220a 0a20 206c 6179 6572 5f6e 616d 653a  "..  layer_name:
 001a53e0: 2073 7472 203d 202e 2e2e 0a0a 2020 2222   str = .....  ""
@@ -107875,18 +107875,18 @@
 001a5620: 6620 626c 5f72 6e61 5f67 6574 5f73 7562  f bl_rna_get_sub
 001a5630: 636c 6173 735f 7079 2863 6c73 2c20 6964  class_py(cls, id
 001a5640: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 001a5650: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
 001a5660: 6529 202d 3e20 7479 7069 6e67 2e54 7970  e) -> typing.Typ
 001a5670: 653a 0a0a 2020 2020 2e2e 2e0a 0a63 6c61  e:..    .....cla
 001a5680: 7373 2053 6861 6465 724e 6f64 6556 6f6c  ss ShaderNodeVol
-001a5690: 756d 6541 6273 6f72 7074 696f 6e28 6270  umeAbsorption(bp
-001a56a0: 795f 7374 7275 6374 2c20 5368 6164 6572  y_struct, Shader
-001a56b0: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-001a56c0: 496e 7465 726e 616c 293a 0a0a 2020 2222  Internal):..  ""
+001a5690: 756d 6541 6273 6f72 7074 696f 6e28 5368  umeAbsorption(Sh
+001a56a0: 6164 6572 4e6f 6465 2c20 6270 795f 7374  aderNode, bpy_st
+001a56b0: 7275 6374 2c20 4e6f 6465 496e 7465 726e  ruct, NodeIntern
+001a56c0: 616c 2c20 4e6f 6465 293a 0a0a 2020 2222  al, Node):..  ""
 001a56d0: 220a 0a20 2041 6273 6f72 6220 6c69 6768  "..  Absorb ligh
 001a56e0: 7420 6173 2069 7420 7061 7373 6573 2074  t as it passes t
 001a56f0: 6872 6f75 6768 2074 6865 2076 6f6c 756d  hrough the volum
 001a5700: 650a 0a20 2022 2222 0a0a 2020 4063 6c61  e..  """..  @cla
 001a5710: 7373 6d65 7468 6f64 0a0a 2020 6465 6620  ssmethod..  def 
 001a5720: 6973 5f72 6567 6973 7465 7265 645f 6e6f  is_registered_no
 001a5730: 6465 5f74 7970 6528 636c 7329 202d 3e20  de_type(cls) -> 
@@ -107923,17 +107923,17 @@
 001a5920: 6c5f 726e 615f 6765 745f 7375 6263 6c61  l_rna_get_subcla
 001a5930: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 001a5940: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 001a5950: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 001a5960: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 001a5970: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 001a5980: 5368 6164 6572 4e6f 6465 566f 6c75 6d65  ShaderNodeVolume
-001a5990: 496e 666f 2862 7079 5f73 7472 7563 742c  Info(bpy_struct,
-001a59a0: 2053 6861 6465 724e 6f64 652c 204e 6f64   ShaderNode, Nod
-001a59b0: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+001a5990: 496e 666f 2853 6861 6465 724e 6f64 652c  Info(ShaderNode,
+001a59a0: 2062 7079 5f73 7472 7563 742c 204e 6f64   bpy_struct, Nod
+001a59b0: 6549 6e74 6572 6e61 6c2c 204e 6f64 6529  eInternal, Node)
 001a59c0: 3a0a 0a20 2022 2222 0a0a 2020 5265 6164  :..  """..  Read
 001a59d0: 2076 6f6c 756d 6520 6461 7461 2061 7474   volume data att
 001a59e0: 7269 6275 7465 7320 6672 6f6d 2076 6f6c  ributes from vol
 001a59f0: 756d 6520 6772 6964 730a 0a20 2022 2222  ume grids..  """
 001a5a00: 0a0a 2020 4063 6c61 7373 6d65 7468 6f64  ..  @classmethod
 001a5a10: 0a0a 2020 6465 6620 6973 5f72 6567 6973  ..  def is_regis
 001a5a20: 7465 7265 645f 6e6f 6465 5f74 7970 6528  tered_node_type(
@@ -107971,17 +107971,17 @@
 001a5c20: 745f 7375 6263 6c61 7373 5f70 7928 636c  t_subclass_py(cl
 001a5c30: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 001a5c40: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 001a5c50: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 001a5c60: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 001a5c70: 0a0a 636c 6173 7320 5368 6164 6572 4e6f  ..class ShaderNo
 001a5c80: 6465 566f 6c75 6d65 5072 696e 6369 706c  deVolumePrincipl
-001a5c90: 6564 2862 7079 5f73 7472 7563 742c 2053  ed(bpy_struct, S
-001a5ca0: 6861 6465 724e 6f64 652c 204e 6f64 652c  haderNode, Node,
-001a5cb0: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+001a5c90: 6564 2853 6861 6465 724e 6f64 652c 2062  ed(ShaderNode, b
+001a5ca0: 7079 5f73 7472 7563 742c 204e 6f64 6549  py_struct, NodeI
+001a5cb0: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 001a5cc0: 0a20 2022 2222 0a0a 2020 436f 6d62 696e  .  """..  Combin
 001a5cd0: 6520 616c 6c20 766f 6c75 6d65 2073 6861  e all volume sha
 001a5ce0: 6469 6e67 2063 6f6d 706f 6e65 6e74 7320  ding components 
 001a5cf0: 696e 746f 2061 2073 696e 676c 6520 6561  into a single ea
 001a5d00: 7379 2074 6f20 7573 6520 6e6f 6465 0a0a  sy to use node..
 001a5d10: 2020 2222 220a 0a20 2040 636c 6173 736d    """..  @classm
 001a5d20: 6574 686f 640a 0a20 2064 6566 2069 735f  ethod..  def is_
@@ -108020,17 +108020,17 @@
 001a5f30: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 001a5f40: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 001a5f50: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 001a5f60: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 001a5f70: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 001a5f80: 2020 2e2e 2e0a 0a63 6c61 7373 2053 6861    .....class Sha
 001a5f90: 6465 724e 6f64 6556 6f6c 756d 6553 6361  derNodeVolumeSca
-001a5fa0: 7474 6572 2862 7079 5f73 7472 7563 742c  tter(bpy_struct,
-001a5fb0: 2053 6861 6465 724e 6f64 652c 204e 6f64   ShaderNode, Nod
-001a5fc0: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+001a5fa0: 7474 6572 2853 6861 6465 724e 6f64 652c  tter(ShaderNode,
+001a5fb0: 2062 7079 5f73 7472 7563 742c 204e 6f64   bpy_struct, Nod
+001a5fc0: 6549 6e74 6572 6e61 6c2c 204e 6f64 6529  eInternal, Node)
 001a5fd0: 3a0a 0a20 2022 2222 0a0a 2020 5363 6174  :..  """..  Scat
 001a5fe0: 7465 7220 6c69 6768 7420 6173 2069 7420  ter light as it 
 001a5ff0: 7061 7373 6573 2074 6872 6f75 6768 2074  passes through t
 001a6000: 6865 2076 6f6c 756d 652c 206f 6674 656e  he volume, often
 001a6010: 2075 7365 6420 746f 2061 6464 2066 6f67   used to add fog
 001a6020: 2074 6f20 6120 7363 656e 650a 0a20 2022   to a scene..  "
 001a6030: 2222 0a0a 2020 4063 6c61 7373 6d65 7468  ""..  @classmeth
@@ -108069,18 +108069,18 @@
 001a6240: 640a 0a20 2064 6566 2062 6c5f 726e 615f  d..  def bl_rna_
 001a6250: 6765 745f 7375 6263 6c61 7373 5f70 7928  get_subclass_py(
 001a6260: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 001a6270: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 001a6280: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 001a6290: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 001a62a0: 2e2e 0a0a 636c 6173 7320 5368 6164 6572  ....class Shader
-001a62b0: 4e6f 6465 5761 7665 6c65 6e67 7468 2862  NodeWavelength(b
-001a62c0: 7079 5f73 7472 7563 742c 2053 6861 6465  py_struct, Shade
-001a62d0: 724e 6f64 652c 204e 6f64 652c 204e 6f64  rNode, Node, Nod
-001a62e0: 6549 6e74 6572 6e61 6c29 3a0a 0a20 2022  eInternal):..  "
+001a62b0: 4e6f 6465 5761 7665 6c65 6e67 7468 2853  NodeWavelength(S
+001a62c0: 6861 6465 724e 6f64 652c 2062 7079 5f73  haderNode, bpy_s
+001a62d0: 7472 7563 742c 204e 6f64 6549 6e74 6572  truct, NodeInter
+001a62e0: 6e61 6c2c 204e 6f64 6529 3a0a 0a20 2022  nal, Node):..  "
 001a62f0: 2222 0a0a 2020 436f 6e76 6572 7420 6120  ""..  Convert a 
 001a6300: 7761 7665 6c65 6e67 7468 2076 616c 7565  wavelength value
 001a6310: 2074 6f20 616e 2052 4742 2076 616c 7565   to an RGB value
 001a6320: 0a0a 2020 2222 220a 0a20 2040 636c 6173  ..  """..  @clas
 001a6330: 736d 6574 686f 640a 0a20 2064 6566 2069  smethod..  def i
 001a6340: 735f 7265 6769 7374 6572 6564 5f6e 6f64  s_registered_nod
 001a6350: 655f 7479 7065 2863 6c73 2920 2d3e 2062  e_type(cls) -> b
@@ -108117,17 +108117,17 @@
 001a6540: 5f72 6e61 5f67 6574 5f73 7562 636c 6173  _rna_get_subclas
 001a6550: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 001a6560: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 001a6570: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 001a6580: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 001a6590: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2053      .....class S
 001a65a0: 6861 6465 724e 6f64 6557 6972 6566 7261  haderNodeWirefra
-001a65b0: 6d65 2862 7079 5f73 7472 7563 742c 2053  me(bpy_struct, S
-001a65c0: 6861 6465 724e 6f64 652c 204e 6f64 652c  haderNode, Node,
-001a65d0: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+001a65b0: 6d65 2853 6861 6465 724e 6f64 652c 2062  me(ShaderNode, b
+001a65c0: 7079 5f73 7472 7563 742c 204e 6f64 6549  py_struct, NodeI
+001a65d0: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 001a65e0: 0a20 2022 2222 0a0a 2020 5265 7472 6965  .  """..  Retrie
 001a65f0: 7665 2074 6865 2065 6467 6573 206f 6620  ve the edges of 
 001a6600: 616e 206f 626a 6563 7420 6173 2069 7420  an object as it 
 001a6610: 6170 7065 6172 7320 746f 2043 7963 6c65  appears to Cycle
 001a6620: 732e 0a4e 6f74 653a 2061 7320 6d65 7368  s..Note: as mesh
 001a6630: 6573 2061 7265 2074 7269 616e 6775 6c61  es are triangula
 001a6640: 7465 6420 6265 666f 7265 2062 6569 6e67  ted before being
@@ -108177,18 +108177,18 @@
 001a6900: 0a0a 2020 6465 6620 626c 5f72 6e61 5f67  ..  def bl_rna_g
 001a6910: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 001a6920: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 001a6930: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 001a6940: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 001a6950: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 001a6960: 2e0a 0a63 6c61 7373 2054 6578 7475 7265  ...class Texture
-001a6970: 4e6f 6465 4174 2862 7079 5f73 7472 7563  NodeAt(bpy_struc
-001a6980: 742c 2054 6578 7475 7265 4e6f 6465 2c20  t, TextureNode, 
-001a6990: 4e6f 6465 2c20 4e6f 6465 496e 7465 726e  Node, NodeIntern
-001a69a0: 616c 293a 0a0a 2020 4063 6c61 7373 6d65  al):..  @classme
+001a6970: 4e6f 6465 4174 2854 6578 7475 7265 4e6f  NodeAt(TextureNo
+001a6980: 6465 2c20 6270 795f 7374 7275 6374 2c20  de, bpy_struct, 
+001a6990: 4e6f 6465 496e 7465 726e 616c 2c20 4e6f  NodeInternal, No
+001a69a0: 6465 293a 0a0a 2020 4063 6c61 7373 6d65  de):..  @classme
 001a69b0: 7468 6f64 0a0a 2020 6465 6620 6973 5f72  thod..  def is_r
 001a69c0: 6567 6973 7465 7265 645f 6e6f 6465 5f74  egistered_node_t
 001a69d0: 7970 6528 636c 7329 202d 3e20 626f 6f6c  ype(cls) -> bool
 001a69e0: 3a0a 0a20 2020 2022 2222 0a0a 2020 2020  :..    """..    
 001a69f0: 5472 7565 2069 6620 6120 7265 6769 7374  True if a regist
 001a6a00: 6572 6564 206e 6f64 6520 7479 7065 0a0a  ered node type..
 001a6a10: 2020 2020 2222 220a 0a20 2020 202e 2e2e      """..    ...
@@ -108220,18 +108220,18 @@
 001a6bb0: 686f 640a 0a20 2064 6566 2062 6c5f 726e  hod..  def bl_rn
 001a6bc0: 615f 6765 745f 7375 6263 6c61 7373 5f70  a_get_subclass_p
 001a6bd0: 7928 636c 732c 2069 643a 2073 7472 2c20  y(cls, id: str, 
 001a6be0: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
 001a6bf0: 416e 7920 3d20 4e6f 6e65 2920 2d3e 2074  Any = None) -> t
 001a6c00: 7970 696e 672e 5479 7065 3a0a 0a20 2020  yping.Type:..   
 001a6c10: 202e 2e2e 0a0a 636c 6173 7320 5465 7874   .....class Text
-001a6c20: 7572 654e 6f64 6542 7269 636b 7328 6270  ureNodeBricks(bp
-001a6c30: 795f 7374 7275 6374 2c20 5465 7874 7572  y_struct, Textur
-001a6c40: 654e 6f64 652c 204e 6f64 652c 204e 6f64  eNode, Node, Nod
-001a6c50: 6549 6e74 6572 6e61 6c29 3a0a 0a20 206f  eInternal):..  o
+001a6c20: 7572 654e 6f64 6542 7269 636b 7328 5465  ureNodeBricks(Te
+001a6c30: 7874 7572 654e 6f64 652c 2062 7079 5f73  xtureNode, bpy_s
+001a6c40: 7472 7563 742c 204e 6f64 6549 6e74 6572  truct, NodeInter
+001a6c50: 6e61 6c2c 204e 6f64 6529 3a0a 0a20 206f  nal, Node):..  o
 001a6c60: 6666 7365 743a 2066 6c6f 6174 203d 202e  ffset: float = .
 001a6c70: 2e2e 0a0a 2020 6f66 6673 6574 5f66 7265  ....  offset_fre
 001a6c80: 7175 656e 6379 3a20 696e 7420 3d20 2e2e  quency: int = ..
 001a6c90: 2e0a 0a20 2022 2222 0a0a 2020 4f66 6673  ...  """..  Offs
 001a6ca0: 6574 2065 7665 7279 204e 2072 6f77 730a  et every N rows.
 001a6cb0: 0a20 2022 2222 0a0a 2020 7371 7561 7368  .  """..  squash
 001a6cc0: 3a20 666c 6f61 7420 3d20 2e2e 2e0a 0a20  : float = ..... 
@@ -108275,18 +108275,18 @@
 001a6f20: 0a0a 2020 6465 6620 626c 5f72 6e61 5f67  ..  def bl_rna_g
 001a6f30: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 001a6f40: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 001a6f50: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 001a6f60: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 001a6f70: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 001a6f80: 2e0a 0a63 6c61 7373 2054 6578 7475 7265  ...class Texture
-001a6f90: 4e6f 6465 4368 6563 6b65 7228 6270 795f  NodeChecker(bpy_
-001a6fa0: 7374 7275 6374 2c20 5465 7874 7572 654e  struct, TextureN
-001a6fb0: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-001a6fc0: 6e74 6572 6e61 6c29 3a0a 0a20 2040 636c  nternal):..  @cl
+001a6f90: 4e6f 6465 4368 6563 6b65 7228 5465 7874  NodeChecker(Text
+001a6fa0: 7572 654e 6f64 652c 2062 7079 5f73 7472  ureNode, bpy_str
+001a6fb0: 7563 742c 204e 6f64 6549 6e74 6572 6e61  uct, NodeInterna
+001a6fc0: 6c2c 204e 6f64 6529 3a0a 0a20 2040 636c  l, Node):..  @cl
 001a6fd0: 6173 736d 6574 686f 640a 0a20 2064 6566  assmethod..  def
 001a6fe0: 2069 735f 7265 6769 7374 6572 6564 5f6e   is_registered_n
 001a6ff0: 6f64 655f 7479 7065 2863 6c73 2920 2d3e  ode_type(cls) ->
 001a7000: 2062 6f6f 6c3a 0a0a 2020 2020 2222 220a   bool:..    """.
 001a7010: 0a20 2020 2054 7275 6520 6966 2061 2072  .    True if a r
 001a7020: 6567 6973 7465 7265 6420 6e6f 6465 2074  egistered node t
 001a7030: 7970 650a 0a20 2020 2022 2222 0a0a 2020  ype..    """..  
@@ -108319,18 +108319,18 @@
 001a71e0: 626c 5f72 6e61 5f67 6574 5f73 7562 636c  bl_rna_get_subcl
 001a71f0: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 001a7200: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 001a7210: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 001a7220: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 001a7230: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 001a7240: 2054 6578 7475 7265 4e6f 6465 436f 6d62   TextureNodeComb
-001a7250: 696e 6543 6f6c 6f72 2862 7079 5f73 7472  ineColor(bpy_str
-001a7260: 7563 742c 2054 6578 7475 7265 4e6f 6465  uct, TextureNode
-001a7270: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-001a7280: 726e 616c 293a 0a0a 2020 6d6f 6465 3a20  rnal):..  mode: 
+001a7250: 696e 6543 6f6c 6f72 2854 6578 7475 7265  ineColor(Texture
+001a7260: 4e6f 6465 2c20 6270 795f 7374 7275 6374  Node, bpy_struct
+001a7270: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+001a7280: 4e6f 6465 293a 0a0a 2020 6d6f 6465 3a20  Node):..  mode: 
 001a7290: 7374 7220 3d20 2e2e 2e0a 0a20 2022 2222  str = .....  """
 001a72a0: 0a0a 2020 4d6f 6465 206f 6620 636f 6c6f  ..  Mode of colo
 001a72b0: 7220 7072 6f63 6573 7369 6e67 0a0a 2020  r processing..  
 001a72c0: 2a20 6060 5247 4260 600a 5247 4220 2d2d  * ``RGB``.RGB --
 001a72d0: 2055 7365 2052 4742 2063 6f6c 6f72 2070   Use RGB color p
 001a72e0: 726f 6365 7373 696e 672e 0a0a 2020 2a20  rocessing...  * 
 001a72f0: 6060 4853 5660 600a 4853 5620 2d2d 2055  ``HSV``.HSV -- U
@@ -108375,18 +108375,18 @@
 001a7560: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 001a7570: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 001a7580: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 001a7590: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 001a75a0: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 001a75b0: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 001a75c0: 6c61 7373 2054 6578 7475 7265 4e6f 6465  lass TextureNode
-001a75d0: 436f 6d70 6f73 6528 6270 795f 7374 7275  Compose(bpy_stru
-001a75e0: 6374 2c20 5465 7874 7572 654e 6f64 652c  ct, TextureNode,
-001a75f0: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-001a7600: 6e61 6c29 3a0a 0a20 2040 636c 6173 736d  nal):..  @classm
+001a75d0: 436f 6d70 6f73 6528 5465 7874 7572 654e  Compose(TextureN
+001a75e0: 6f64 652c 2062 7079 5f73 7472 7563 742c  ode, bpy_struct,
+001a75f0: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+001a7600: 6f64 6529 3a0a 0a20 2040 636c 6173 736d  ode):..  @classm
 001a7610: 6574 686f 640a 0a20 2064 6566 2069 735f  ethod..  def is_
 001a7620: 7265 6769 7374 6572 6564 5f6e 6f64 655f  registered_node_
 001a7630: 7479 7065 2863 6c73 2920 2d3e 2062 6f6f  type(cls) -> boo
 001a7640: 6c3a 0a0a 2020 2020 2222 220a 0a20 2020  l:..    """..   
 001a7650: 2054 7275 6520 6966 2061 2072 6567 6973   True if a regis
 001a7660: 7465 7265 6420 6e6f 6465 2074 7970 650a  tered node type.
 001a7670: 0a20 2020 2022 2222 0a0a 2020 2020 2e2e  .    """..    ..
@@ -108419,17 +108419,17 @@
 001a7820: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 001a7830: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 001a7840: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 001a7850: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 001a7860: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 001a7870: 2020 2e2e 2e0a 0a63 6c61 7373 2054 6578    .....class Tex
 001a7880: 7475 7265 4e6f 6465 436f 6f72 6469 6e61  tureNodeCoordina
-001a7890: 7465 7328 6270 795f 7374 7275 6374 2c20  tes(bpy_struct, 
-001a78a0: 5465 7874 7572 654e 6f64 652c 204e 6f64  TextureNode, Nod
-001a78b0: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+001a7890: 7465 7328 5465 7874 7572 654e 6f64 652c  tes(TextureNode,
+001a78a0: 2062 7079 5f73 7472 7563 742c 204e 6f64   bpy_struct, Nod
+001a78b0: 6549 6e74 6572 6e61 6c2c 204e 6f64 6529  eInternal, Node)
 001a78c0: 3a0a 0a20 2040 636c 6173 736d 6574 686f  :..  @classmetho
 001a78d0: 640a 0a20 2064 6566 2069 735f 7265 6769  d..  def is_regi
 001a78e0: 7374 6572 6564 5f6e 6f64 655f 7479 7065  stered_node_type
 001a78f0: 2863 6c73 2920 2d3e 2062 6f6f 6c3a 0a0a  (cls) -> bool:..
 001a7900: 2020 2020 2222 220a 0a20 2020 2054 7275      """..    Tru
 001a7910: 6520 6966 2061 2072 6567 6973 7465 7265  e if a registere
 001a7920: 6420 6e6f 6465 2074 7970 650a 0a20 2020  d node type..   
@@ -108462,18 +108462,18 @@
 001a7ad0: 0a0a 2020 6465 6620 626c 5f72 6e61 5f67  ..  def bl_rna_g
 001a7ae0: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 001a7af0: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 001a7b00: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 001a7b10: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 001a7b20: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 001a7b30: 2e0a 0a63 6c61 7373 2054 6578 7475 7265  ...class Texture
-001a7b40: 4e6f 6465 4375 7276 6552 4742 2862 7079  NodeCurveRGB(bpy
-001a7b50: 5f73 7472 7563 742c 2054 6578 7475 7265  _struct, Texture
-001a7b60: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-001a7b70: 496e 7465 726e 616c 293a 0a0a 2020 6d61  Internal):..  ma
+001a7b40: 4e6f 6465 4375 7276 6552 4742 2854 6578  NodeCurveRGB(Tex
+001a7b50: 7475 7265 4e6f 6465 2c20 6270 795f 7374  tureNode, bpy_st
+001a7b60: 7275 6374 2c20 4e6f 6465 496e 7465 726e  ruct, NodeIntern
+001a7b70: 616c 2c20 4e6f 6465 293a 0a0a 2020 6d61  al, Node):..  ma
 001a7b80: 7070 696e 673a 2043 7572 7665 4d61 7070  pping: CurveMapp
 001a7b90: 696e 6720 3d20 2e2e 2e0a 0a20 2040 636c  ing = .....  @cl
 001a7ba0: 6173 736d 6574 686f 640a 0a20 2064 6566  assmethod..  def
 001a7bb0: 2069 735f 7265 6769 7374 6572 6564 5f6e   is_registered_n
 001a7bc0: 6f64 655f 7479 7065 2863 6c73 2920 2d3e  ode_type(cls) ->
 001a7bd0: 2062 6f6f 6c3a 0a0a 2020 2020 2222 220a   bool:..    """.
 001a7be0: 0a20 2020 2054 7275 6520 6966 2061 2072  .    True if a r
@@ -108508,18 +108508,18 @@
 001a7db0: 626c 5f72 6e61 5f67 6574 5f73 7562 636c  bl_rna_get_subcl
 001a7dc0: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 001a7dd0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 001a7de0: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 001a7df0: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 001a7e00: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 001a7e10: 2054 6578 7475 7265 4e6f 6465 4375 7276   TextureNodeCurv
-001a7e20: 6554 696d 6528 6270 795f 7374 7275 6374  eTime(bpy_struct
-001a7e30: 2c20 5465 7874 7572 654e 6f64 652c 204e  , TextureNode, N
-001a7e40: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-001a7e50: 6c29 3a0a 0a20 2063 7572 7665 3a20 4375  l):..  curve: Cu
+001a7e20: 6554 696d 6528 5465 7874 7572 654e 6f64  eTime(TextureNod
+001a7e30: 652c 2062 7079 5f73 7472 7563 742c 204e  e, bpy_struct, N
+001a7e40: 6f64 6549 6e74 6572 6e61 6c2c 204e 6f64  odeInternal, Nod
+001a7e50: 6529 3a0a 0a20 2063 7572 7665 3a20 4375  e):..  curve: Cu
 001a7e60: 7276 654d 6170 7069 6e67 203d 202e 2e2e  rveMapping = ...
 001a7e70: 0a0a 2020 6672 616d 655f 656e 643a 2069  ..  frame_end: i
 001a7e80: 6e74 203d 202e 2e2e 0a0a 2020 6672 616d  nt = .....  fram
 001a7e90: 655f 7374 6172 743a 2069 6e74 203d 202e  e_start: int = .
 001a7ea0: 2e2e 0a0a 2020 4063 6c61 7373 6d65 7468  ....  @classmeth
 001a7eb0: 6f64 0a0a 2020 6465 6620 6973 5f72 6567  od..  def is_reg
 001a7ec0: 6973 7465 7265 645f 6e6f 6465 5f74 7970  istered_node_typ
@@ -108556,18 +108556,18 @@
 001a80b0: 640a 0a20 2064 6566 2062 6c5f 726e 615f  d..  def bl_rna_
 001a80c0: 6765 745f 7375 6263 6c61 7373 5f70 7928  get_subclass_py(
 001a80d0: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 001a80e0: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 001a80f0: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 001a8100: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 001a8110: 2e2e 0a0a 636c 6173 7320 5465 7874 7572  ....class Textur
-001a8120: 654e 6f64 6544 6563 6f6d 706f 7365 2862  eNodeDecompose(b
-001a8130: 7079 5f73 7472 7563 742c 2054 6578 7475  py_struct, Textu
-001a8140: 7265 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  reNode, Node, No
-001a8150: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+001a8120: 654e 6f64 6544 6563 6f6d 706f 7365 2854  eNodeDecompose(T
+001a8130: 6578 7475 7265 4e6f 6465 2c20 6270 795f  extureNode, bpy_
+001a8140: 7374 7275 6374 2c20 4e6f 6465 496e 7465  struct, NodeInte
+001a8150: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 001a8160: 4063 6c61 7373 6d65 7468 6f64 0a0a 2020  @classmethod..  
 001a8170: 6465 6620 6973 5f72 6567 6973 7465 7265  def is_registere
 001a8180: 645f 6e6f 6465 5f74 7970 6528 636c 7329  d_node_type(cls)
 001a8190: 202d 3e20 626f 6f6c 3a0a 0a20 2020 2022   -> bool:..    "
 001a81a0: 2222 0a0a 2020 2020 5472 7565 2069 6620  ""..    True if 
 001a81b0: 6120 7265 6769 7374 6572 6564 206e 6f64  a registered nod
 001a81c0: 6520 7479 7065 0a0a 2020 2020 2222 220a  e type..    """.
@@ -108600,18 +108600,18 @@
 001a8370: 6566 2062 6c5f 726e 615f 6765 745f 7375  ef bl_rna_get_su
 001a8380: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 001a8390: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 001a83a0: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 001a83b0: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 001a83c0: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 001a83d0: 6173 7320 5465 7874 7572 654e 6f64 6544  ass TextureNodeD
-001a83e0: 6973 7461 6e63 6528 6270 795f 7374 7275  istance(bpy_stru
-001a83f0: 6374 2c20 5465 7874 7572 654e 6f64 652c  ct, TextureNode,
-001a8400: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-001a8410: 6e61 6c29 3a0a 0a20 2040 636c 6173 736d  nal):..  @classm
+001a83e0: 6973 7461 6e63 6528 5465 7874 7572 654e  istance(TextureN
+001a83f0: 6f64 652c 2062 7079 5f73 7472 7563 742c  ode, bpy_struct,
+001a8400: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+001a8410: 6f64 6529 3a0a 0a20 2040 636c 6173 736d  ode):..  @classm
 001a8420: 6574 686f 640a 0a20 2064 6566 2069 735f  ethod..  def is_
 001a8430: 7265 6769 7374 6572 6564 5f6e 6f64 655f  registered_node_
 001a8440: 7479 7065 2863 6c73 2920 2d3e 2062 6f6f  type(cls) -> boo
 001a8450: 6c3a 0a0a 2020 2020 2222 220a 0a20 2020  l:..    """..   
 001a8460: 2054 7275 6520 6966 2061 2072 6567 6973   True if a regis
 001a8470: 7465 7265 6420 6e6f 6465 2074 7970 650a  tered node type.
 001a8480: 0a20 2020 2022 2222 0a0a 2020 2020 2e2e  .    """..    ..
@@ -108643,18 +108643,18 @@
 001a8620: 7468 6f64 0a0a 2020 6465 6620 626c 5f72  thod..  def bl_r
 001a8630: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 001a8640: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 001a8650: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 001a8660: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 001a8670: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 001a8680: 2020 2e2e 2e0a 0a63 6c61 7373 2054 6578    .....class Tex
-001a8690: 7475 7265 4e6f 6465 4772 6f75 7028 6270  tureNodeGroup(bp
-001a86a0: 795f 7374 7275 6374 2c20 5465 7874 7572  y_struct, Textur
-001a86b0: 654e 6f64 652c 204e 6f64 652c 204e 6f64  eNode, Node, Nod
-001a86c0: 6549 6e74 6572 6e61 6c29 3a0a 0a20 206e  eInternal):..  n
+001a8690: 7475 7265 4e6f 6465 4772 6f75 7028 5465  tureNodeGroup(Te
+001a86a0: 7874 7572 654e 6f64 652c 2062 7079 5f73  xtureNode, bpy_s
+001a86b0: 7472 7563 742c 204e 6f64 6549 6e74 6572  truct, NodeInter
+001a86c0: 6e61 6c2c 204e 6f64 6529 3a0a 0a20 206e  nal, Node):..  n
 001a86d0: 6f64 655f 7472 6565 3a20 4e6f 6465 5472  ode_tree: NodeTr
 001a86e0: 6565 203d 202e 2e2e 0a0a 2020 4063 6c61  ee = .....  @cla
 001a86f0: 7373 6d65 7468 6f64 0a0a 2020 6465 6620  ssmethod..  def 
 001a8700: 6973 5f72 6567 6973 7465 7265 645f 6e6f  is_registered_no
 001a8710: 6465 5f74 7970 6528 636c 7329 202d 3e20  de_type(cls) -> 
 001a8720: 626f 6f6c 3a0a 0a20 2020 2022 2222 0a0a  bool:..    """..
 001a8730: 2020 2020 5472 7565 2069 6620 6120 7265      True if a re
@@ -108689,18 +108689,18 @@
 001a8900: 6c5f 726e 615f 6765 745f 7375 6263 6c61  l_rna_get_subcla
 001a8910: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 001a8920: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 001a8930: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 001a8940: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 001a8950: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 001a8960: 5465 7874 7572 654e 6f64 6548 7565 5361  TextureNodeHueSa
-001a8970: 7475 7261 7469 6f6e 2862 7079 5f73 7472  turation(bpy_str
-001a8980: 7563 742c 2054 6578 7475 7265 4e6f 6465  uct, TextureNode
-001a8990: 2c20 4e6f 6465 2c20 4e6f 6465 496e 7465  , Node, NodeInte
-001a89a0: 726e 616c 293a 0a0a 2020 4063 6c61 7373  rnal):..  @class
+001a8970: 7475 7261 7469 6f6e 2854 6578 7475 7265  turation(Texture
+001a8980: 4e6f 6465 2c20 6270 795f 7374 7275 6374  Node, bpy_struct
+001a8990: 2c20 4e6f 6465 496e 7465 726e 616c 2c20  , NodeInternal, 
+001a89a0: 4e6f 6465 293a 0a0a 2020 4063 6c61 7373  Node):..  @class
 001a89b0: 6d65 7468 6f64 0a0a 2020 6465 6620 6973  method..  def is
 001a89c0: 5f72 6567 6973 7465 7265 645f 6e6f 6465  _registered_node
 001a89d0: 5f74 7970 6528 636c 7329 202d 3e20 626f  _type(cls) -> bo
 001a89e0: 6f6c 3a0a 0a20 2020 2022 2222 0a0a 2020  ol:..    """..  
 001a89f0: 2020 5472 7565 2069 6620 6120 7265 6769    True if a regi
 001a8a00: 7374 6572 6564 206e 6f64 6520 7479 7065  stered node type
 001a8a10: 0a0a 2020 2020 2222 220a 0a20 2020 202e  ..    """..    .
@@ -108732,18 +108732,18 @@
 001a8bb0: 6574 686f 640a 0a20 2064 6566 2062 6c5f  ethod..  def bl_
 001a8bc0: 726e 615f 6765 745f 7375 6263 6c61 7373  rna_get_subclass
 001a8bd0: 5f70 7928 636c 732c 2069 643a 2073 7472  _py(cls, id: str
 001a8be0: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 001a8bf0: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 001a8c00: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 001a8c10: 2020 202e 2e2e 0a0a 636c 6173 7320 5465     .....class Te
-001a8c20: 7874 7572 654e 6f64 6549 6d61 6765 2862  xtureNodeImage(b
-001a8c30: 7079 5f73 7472 7563 742c 2054 6578 7475  py_struct, Textu
-001a8c40: 7265 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  reNode, Node, No
-001a8c50: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+001a8c20: 7874 7572 654e 6f64 6549 6d61 6765 2854  xtureNodeImage(T
+001a8c30: 6578 7475 7265 4e6f 6465 2c20 6270 795f  extureNode, bpy_
+001a8c40: 7374 7275 6374 2c20 4e6f 6465 496e 7465  struct, NodeInte
+001a8c50: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 001a8c60: 696d 6167 653a 2049 6d61 6765 203d 202e  image: Image = .
 001a8c70: 2e2e 0a0a 2020 696d 6167 655f 7573 6572  ....  image_user
 001a8c80: 3a20 496d 6167 6555 7365 7220 3d20 2e2e  : ImageUser = ..
 001a8c90: 2e0a 0a20 2022 2222 0a0a 2020 5061 7261  ...  """..  Para
 001a8ca0: 6d65 7465 7273 2064 6566 696e 696e 6720  meters defining 
 001a8cb0: 7468 6520 696d 6167 6520 6475 7261 7469  the image durati
 001a8cc0: 6f6e 2c20 6f66 6673 6574 2061 6e64 2072  on, offset and r
@@ -108785,17 +108785,17 @@
 001a8f00: 726e 615f 6765 745f 7375 6263 6c61 7373  rna_get_subclass
 001a8f10: 5f70 7928 636c 732c 2069 643a 2073 7472  _py(cls, id: str
 001a8f20: 2c20 6465 6661 756c 743a 2074 7970 696e  , default: typin
 001a8f30: 672e 416e 7920 3d20 4e6f 6e65 2920 2d3e  g.Any = None) ->
 001a8f40: 2074 7970 696e 672e 5479 7065 3a0a 0a20   typing.Type:.. 
 001a8f50: 2020 202e 2e2e 0a0a 636c 6173 7320 5465     .....class Te
 001a8f60: 7874 7572 654e 6f64 6549 6e76 6572 7428  xtureNodeInvert(
-001a8f70: 6270 795f 7374 7275 6374 2c20 5465 7874  bpy_struct, Text
-001a8f80: 7572 654e 6f64 652c 204e 6f64 652c 204e  ureNode, Node, N
-001a8f90: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+001a8f70: 5465 7874 7572 654e 6f64 652c 2062 7079  TextureNode, bpy
+001a8f80: 5f73 7472 7563 742c 204e 6f64 6549 6e74  _struct, NodeInt
+001a8f90: 6572 6e61 6c2c 204e 6f64 6529 3a0a 0a20  ernal, Node):.. 
 001a8fa0: 2040 636c 6173 736d 6574 686f 640a 0a20   @classmethod.. 
 001a8fb0: 2064 6566 2069 735f 7265 6769 7374 6572   def is_register
 001a8fc0: 6564 5f6e 6f64 655f 7479 7065 2863 6c73  ed_node_type(cls
 001a8fd0: 2920 2d3e 2062 6f6f 6c3a 0a0a 2020 2020  ) -> bool:..    
 001a8fe0: 2222 220a 0a20 2020 2054 7275 6520 6966  """..    True if
 001a8ff0: 2061 2072 6567 6973 7465 7265 6420 6e6f   a registered no
 001a9000: 6465 2074 7970 650a 0a20 2020 2022 2222  de type..    """
@@ -108828,17 +108828,17 @@
 001a91b0: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 001a91c0: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 001a91d0: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 001a91e0: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 001a91f0: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 001a9200: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 001a9210: 6c61 7373 2054 6578 7475 7265 4e6f 6465  lass TextureNode
-001a9220: 4d61 7468 2862 7079 5f73 7472 7563 742c  Math(bpy_struct,
-001a9230: 2054 6578 7475 7265 4e6f 6465 2c20 4e6f   TextureNode, No
-001a9240: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+001a9220: 4d61 7468 2854 6578 7475 7265 4e6f 6465  Math(TextureNode
+001a9230: 2c20 6270 795f 7374 7275 6374 2c20 4e6f  , bpy_struct, No
+001a9240: 6465 496e 7465 726e 616c 2c20 4e6f 6465  deInternal, Node
 001a9250: 293a 0a0a 2020 6f70 6572 6174 696f 6e3a  ):..  operation:
 001a9260: 2073 7472 203d 202e 2e2e 0a0a 2020 7573   str = .....  us
 001a9270: 655f 636c 616d 703a 2062 6f6f 6c20 3d20  e_clamp: bool = 
 001a9280: 2e2e 2e0a 0a20 2022 2222 0a0a 2020 436c  .....  """..  Cl
 001a9290: 616d 7020 7265 7375 6c74 206f 6620 7468  amp result of th
 001a92a0: 6520 6e6f 6465 2074 6f20 302e 3020 746f  e node to 0.0 to
 001a92b0: 2031 2e30 2072 616e 6765 0a0a 2020 2222   1.0 range..  ""
@@ -108878,18 +108878,18 @@
 001a94d0: 0a0a 2020 6465 6620 626c 5f72 6e61 5f67  ..  def bl_rna_g
 001a94e0: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 001a94f0: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 001a9500: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 001a9510: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 001a9520: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 001a9530: 2e0a 0a63 6c61 7373 2054 6578 7475 7265  ...class Texture
-001a9540: 4e6f 6465 4d69 7852 4742 2862 7079 5f73  NodeMixRGB(bpy_s
-001a9550: 7472 7563 742c 2054 6578 7475 7265 4e6f  truct, TextureNo
-001a9560: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-001a9570: 7465 726e 616c 293a 0a0a 2020 626c 656e  ternal):..  blen
+001a9540: 4e6f 6465 4d69 7852 4742 2854 6578 7475  NodeMixRGB(Textu
+001a9550: 7265 4e6f 6465 2c20 6270 795f 7374 7275  reNode, bpy_stru
+001a9560: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+001a9570: 2c20 4e6f 6465 293a 0a0a 2020 626c 656e  , Node):..  blen
 001a9580: 645f 7479 7065 3a20 7374 7220 3d20 2e2e  d_type: str = ..
 001a9590: 2e0a 0a20 2075 7365 5f61 6c70 6861 3a20  ...  use_alpha: 
 001a95a0: 626f 6f6c 203d 202e 2e2e 0a0a 2020 2222  bool = .....  ""
 001a95b0: 220a 0a20 2049 6e63 6c75 6465 2061 6c70  "..  Include alp
 001a95c0: 6861 206f 6620 7365 636f 6e64 2069 6e70  ha of second inp
 001a95d0: 7574 2069 6e20 7468 6973 206f 7065 7261  ut in this opera
 001a95e0: 7469 6f6e 0a0a 2020 2222 220a 0a20 2075  tion..  """..  u
@@ -108934,18 +108934,18 @@
 001a9850: 640a 0a20 2064 6566 2062 6c5f 726e 615f  d..  def bl_rna_
 001a9860: 6765 745f 7375 6263 6c61 7373 5f70 7928  get_subclass_py(
 001a9870: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 001a9880: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 001a9890: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 001a98a0: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 001a98b0: 2e2e 0a0a 636c 6173 7320 5465 7874 7572  ....class Textur
-001a98c0: 654e 6f64 654f 7574 7075 7428 6270 795f  eNodeOutput(bpy_
-001a98d0: 7374 7275 6374 2c20 5465 7874 7572 654e  struct, TextureN
-001a98e0: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-001a98f0: 6e74 6572 6e61 6c29 3a0a 0a20 2066 696c  nternal):..  fil
+001a98c0: 654e 6f64 654f 7574 7075 7428 5465 7874  eNodeOutput(Text
+001a98d0: 7572 654e 6f64 652c 2062 7079 5f73 7472  ureNode, bpy_str
+001a98e0: 7563 742c 204e 6f64 6549 6e74 6572 6e61  uct, NodeInterna
+001a98f0: 6c2c 204e 6f64 6529 3a0a 0a20 2066 696c  l, Node):..  fil
 001a9900: 6570 6174 683a 2073 7472 203d 202e 2e2e  epath: str = ...
 001a9910: 0a0a 2020 4063 6c61 7373 6d65 7468 6f64  ..  @classmethod
 001a9920: 0a0a 2020 6465 6620 6973 5f72 6567 6973  ..  def is_regis
 001a9930: 7465 7265 645f 6e6f 6465 5f74 7970 6528  tered_node_type(
 001a9940: 636c 7329 202d 3e20 626f 6f6c 3a0a 0a20  cls) -> bool:.. 
 001a9950: 2020 2022 2222 0a0a 2020 2020 5472 7565     """..    True
 001a9960: 2069 6620 6120 7265 6769 7374 6572 6564   if a registered
@@ -108979,18 +108979,18 @@
 001a9b20: 0a20 2064 6566 2062 6c5f 726e 615f 6765  .  def bl_rna_ge
 001a9b30: 745f 7375 6263 6c61 7373 5f70 7928 636c  t_subclass_py(cl
 001a9b40: 732c 2069 643a 2073 7472 2c20 6465 6661  s, id: str, defa
 001a9b50: 756c 743a 2074 7970 696e 672e 416e 7920  ult: typing.Any 
 001a9b60: 3d20 4e6f 6e65 2920 2d3e 2074 7970 696e  = None) -> typin
 001a9b70: 672e 5479 7065 3a0a 0a20 2020 202e 2e2e  g.Type:..    ...
 001a9b80: 0a0a 636c 6173 7320 5465 7874 7572 654e  ..class TextureN
-001a9b90: 6f64 6552 4742 546f 4257 2862 7079 5f73  odeRGBToBW(bpy_s
-001a9ba0: 7472 7563 742c 2054 6578 7475 7265 4e6f  truct, TextureNo
-001a9bb0: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-001a9bc0: 7465 726e 616c 293a 0a0a 2020 4063 6c61  ternal):..  @cla
+001a9b90: 6f64 6552 4742 546f 4257 2854 6578 7475  odeRGBToBW(Textu
+001a9ba0: 7265 4e6f 6465 2c20 6270 795f 7374 7275  reNode, bpy_stru
+001a9bb0: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+001a9bc0: 2c20 4e6f 6465 293a 0a0a 2020 4063 6c61  , Node):..  @cla
 001a9bd0: 7373 6d65 7468 6f64 0a0a 2020 6465 6620  ssmethod..  def 
 001a9be0: 6973 5f72 6567 6973 7465 7265 645f 6e6f  is_registered_no
 001a9bf0: 6465 5f74 7970 6528 636c 7329 202d 3e20  de_type(cls) -> 
 001a9c00: 626f 6f6c 3a0a 0a20 2020 2022 2222 0a0a  bool:..    """..
 001a9c10: 2020 2020 5472 7565 2069 6620 6120 7265      True if a re
 001a9c20: 6769 7374 6572 6564 206e 6f64 6520 7479  gistered node ty
 001a9c30: 7065 0a0a 2020 2020 2222 220a 0a20 2020  pe..    """..   
@@ -109023,17 +109023,17 @@
 001a9de0: 6c5f 726e 615f 6765 745f 7375 6263 6c61  l_rna_get_subcla
 001a9df0: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 001a9e00: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 001a9e10: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 001a9e20: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 001a9e30: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 001a9e40: 5465 7874 7572 654e 6f64 6552 6f74 6174  TextureNodeRotat
-001a9e50: 6528 6270 795f 7374 7275 6374 2c20 5465  e(bpy_struct, Te
-001a9e60: 7874 7572 654e 6f64 652c 204e 6f64 652c  xtureNode, Node,
-001a9e70: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+001a9e50: 6528 5465 7874 7572 654e 6f64 652c 2062  e(TextureNode, b
+001a9e60: 7079 5f73 7472 7563 742c 204e 6f64 6549  py_struct, NodeI
+001a9e70: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 001a9e80: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
 001a9e90: 0a20 2064 6566 2069 735f 7265 6769 7374  .  def is_regist
 001a9ea0: 6572 6564 5f6e 6f64 655f 7479 7065 2863  ered_node_type(c
 001a9eb0: 6c73 2920 2d3e 2062 6f6f 6c3a 0a0a 2020  ls) -> bool:..  
 001a9ec0: 2020 2222 220a 0a20 2020 2054 7275 6520    """..    True 
 001a9ed0: 6966 2061 2072 6567 6973 7465 7265 6420  if a registered 
 001a9ee0: 6e6f 6465 2074 7970 650a 0a20 2020 2022  node type..    "
@@ -109066,18 +109066,18 @@
 001aa090: 2020 6465 6620 626c 5f72 6e61 5f67 6574    def bl_rna_get
 001aa0a0: 5f73 7562 636c 6173 735f 7079 2863 6c73  _subclass_py(cls
 001aa0b0: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 001aa0c0: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 001aa0d0: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 001aa0e0: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 001aa0f0: 0a63 6c61 7373 2054 6578 7475 7265 4e6f  .class TextureNo
-001aa100: 6465 5363 616c 6528 6270 795f 7374 7275  deScale(bpy_stru
-001aa110: 6374 2c20 5465 7874 7572 654e 6f64 652c  ct, TextureNode,
-001aa120: 204e 6f64 652c 204e 6f64 6549 6e74 6572   Node, NodeInter
-001aa130: 6e61 6c29 3a0a 0a20 2040 636c 6173 736d  nal):..  @classm
+001aa100: 6465 5363 616c 6528 5465 7874 7572 654e  deScale(TextureN
+001aa110: 6f64 652c 2062 7079 5f73 7472 7563 742c  ode, bpy_struct,
+001aa120: 204e 6f64 6549 6e74 6572 6e61 6c2c 204e   NodeInternal, N
+001aa130: 6f64 6529 3a0a 0a20 2040 636c 6173 736d  ode):..  @classm
 001aa140: 6574 686f 640a 0a20 2064 6566 2069 735f  ethod..  def is_
 001aa150: 7265 6769 7374 6572 6564 5f6e 6f64 655f  registered_node_
 001aa160: 7479 7065 2863 6c73 2920 2d3e 2062 6f6f  type(cls) -> boo
 001aa170: 6c3a 0a0a 2020 2020 2222 220a 0a20 2020  l:..    """..   
 001aa180: 2054 7275 6520 6966 2061 2072 6567 6973   True if a regis
 001aa190: 7465 7265 6420 6e6f 6465 2074 7970 650a  tered node type.
 001aa1a0: 0a20 2020 2022 2222 0a0a 2020 2020 2e2e  .    """..    ..
@@ -109110,18 +109110,18 @@
 001aa350: 6e61 5f67 6574 5f73 7562 636c 6173 735f  na_get_subclass_
 001aa360: 7079 2863 6c73 2c20 6964 3a20 7374 722c  py(cls, id: str,
 001aa370: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
 001aa380: 2e41 6e79 203d 204e 6f6e 6529 202d 3e20  .Any = None) -> 
 001aa390: 7479 7069 6e67 2e54 7970 653a 0a0a 2020  typing.Type:..  
 001aa3a0: 2020 2e2e 2e0a 0a63 6c61 7373 2054 6578    .....class Tex
 001aa3b0: 7475 7265 4e6f 6465 5365 7061 7261 7465  tureNodeSeparate
-001aa3c0: 436f 6c6f 7228 6270 795f 7374 7275 6374  Color(bpy_struct
-001aa3d0: 2c20 5465 7874 7572 654e 6f64 652c 204e  , TextureNode, N
-001aa3e0: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-001aa3f0: 6c29 3a0a 0a20 206d 6f64 653a 2073 7472  l):..  mode: str
+001aa3c0: 436f 6c6f 7228 5465 7874 7572 654e 6f64  Color(TextureNod
+001aa3d0: 652c 2062 7079 5f73 7472 7563 742c 204e  e, bpy_struct, N
+001aa3e0: 6f64 6549 6e74 6572 6e61 6c2c 204e 6f64  odeInternal, Nod
+001aa3f0: 6529 3a0a 0a20 206d 6f64 653a 2073 7472  e):..  mode: str
 001aa400: 203d 202e 2e2e 0a0a 2020 2222 220a 0a20   = .....  """.. 
 001aa410: 204d 6f64 6520 6f66 2063 6f6c 6f72 2070   Mode of color p
 001aa420: 726f 6365 7373 696e 670a 0a20 202a 2060  rocessing..  * `
 001aa430: 6052 4742 6060 0a52 4742 202d 2d20 5573  `RGB``.RGB -- Us
 001aa440: 6520 5247 4220 636f 6c6f 7220 7072 6f63  e RGB color proc
 001aa450: 6573 7369 6e67 2e0a 0a20 202a 2060 6048  essing...  * ``H
 001aa460: 5356 6060 0a48 5356 202d 2d20 5573 6520  SV``.HSV -- Use 
@@ -109166,18 +109166,18 @@
 001aa6d0: 2062 6c5f 726e 615f 6765 745f 7375 6263   bl_rna_get_subc
 001aa6e0: 6c61 7373 5f70 7928 636c 732c 2069 643a  lass_py(cls, id:
 001aa6f0: 2073 7472 2c20 6465 6661 756c 743a 2074   str, default: t
 001aa700: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 001aa710: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 001aa720: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 001aa730: 7320 5465 7874 7572 654e 6f64 6554 6578  s TextureNodeTex
-001aa740: 426c 656e 6428 6270 795f 7374 7275 6374  Blend(bpy_struct
-001aa750: 2c20 5465 7874 7572 654e 6f64 652c 204e  , TextureNode, N
-001aa760: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-001aa770: 6c29 3a0a 0a20 2040 636c 6173 736d 6574  l):..  @classmet
+001aa740: 426c 656e 6428 5465 7874 7572 654e 6f64  Blend(TextureNod
+001aa750: 652c 2062 7079 5f73 7472 7563 742c 204e  e, bpy_struct, N
+001aa760: 6f64 6549 6e74 6572 6e61 6c2c 204e 6f64  odeInternal, Nod
+001aa770: 6529 3a0a 0a20 2040 636c 6173 736d 6574  e):..  @classmet
 001aa780: 686f 640a 0a20 2064 6566 2069 735f 7265  hod..  def is_re
 001aa790: 6769 7374 6572 6564 5f6e 6f64 655f 7479  gistered_node_ty
 001aa7a0: 7065 2863 6c73 2920 2d3e 2062 6f6f 6c3a  pe(cls) -> bool:
 001aa7b0: 0a0a 2020 2020 2222 220a 0a20 2020 2054  ..    """..    T
 001aa7c0: 7275 6520 6966 2061 2072 6567 6973 7465  rue if a registe
 001aa7d0: 7265 6420 6e6f 6465 2074 7970 650a 0a20  red node type.. 
 001aa7e0: 2020 2022 2222 0a0a 2020 2020 2e2e 2e0a     """..    ....
@@ -109210,17 +109210,17 @@
 001aa990: 5f67 6574 5f73 7562 636c 6173 735f 7079  _get_subclass_py
 001aa9a0: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 001aa9b0: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 001aa9c0: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 001aa9d0: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 001aa9e0: 2e2e 2e0a 0a63 6c61 7373 2054 6578 7475  .....class Textu
 001aa9f0: 7265 4e6f 6465 5465 7843 6c6f 7564 7328  reNodeTexClouds(
-001aaa00: 6270 795f 7374 7275 6374 2c20 5465 7874  bpy_struct, Text
-001aaa10: 7572 654e 6f64 652c 204e 6f64 652c 204e  ureNode, Node, N
-001aaa20: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+001aaa00: 5465 7874 7572 654e 6f64 652c 2062 7079  TextureNode, bpy
+001aaa10: 5f73 7472 7563 742c 204e 6f64 6549 6e74  _struct, NodeInt
+001aaa20: 6572 6e61 6c2c 204e 6f64 6529 3a0a 0a20  ernal, Node):.. 
 001aaa30: 2040 636c 6173 736d 6574 686f 640a 0a20   @classmethod.. 
 001aaa40: 2064 6566 2069 735f 7265 6769 7374 6572   def is_register
 001aaa50: 6564 5f6e 6f64 655f 7479 7065 2863 6c73  ed_node_type(cls
 001aaa60: 2920 2d3e 2062 6f6f 6c3a 0a0a 2020 2020  ) -> bool:..    
 001aaa70: 2222 220a 0a20 2020 2054 7275 6520 6966  """..    True if
 001aaa80: 2061 2072 6567 6973 7465 7265 6420 6e6f   a registered no
 001aaa90: 6465 2074 7970 650a 0a20 2020 2022 2222  de type..    """
@@ -109253,18 +109253,18 @@
 001aac40: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 001aac50: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 001aac60: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 001aac70: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 001aac80: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 001aac90: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 001aaca0: 6c61 7373 2054 6578 7475 7265 4e6f 6465  lass TextureNode
-001aacb0: 5465 7844 6973 744e 6f69 7365 2862 7079  TexDistNoise(bpy
-001aacc0: 5f73 7472 7563 742c 2054 6578 7475 7265  _struct, Texture
-001aacd0: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-001aace0: 496e 7465 726e 616c 293a 0a0a 2020 4063  Internal):..  @c
+001aacb0: 5465 7844 6973 744e 6f69 7365 2854 6578  TexDistNoise(Tex
+001aacc0: 7475 7265 4e6f 6465 2c20 6270 795f 7374  tureNode, bpy_st
+001aacd0: 7275 6374 2c20 4e6f 6465 496e 7465 726e  ruct, NodeIntern
+001aace0: 616c 2c20 4e6f 6465 293a 0a0a 2020 4063  al, Node):..  @c
 001aacf0: 6c61 7373 6d65 7468 6f64 0a0a 2020 6465  lassmethod..  de
 001aad00: 6620 6973 5f72 6567 6973 7465 7265 645f  f is_registered_
 001aad10: 6e6f 6465 5f74 7970 6528 636c 7329 202d  node_type(cls) -
 001aad20: 3e20 626f 6f6c 3a0a 0a20 2020 2022 2222  > bool:..    """
 001aad30: 0a0a 2020 2020 5472 7565 2069 6620 6120  ..    True if a 
 001aad40: 7265 6769 7374 6572 6564 206e 6f64 6520  registered node 
 001aad50: 7479 7065 0a0a 2020 2020 2222 220a 0a20  type..    """.. 
@@ -109297,18 +109297,18 @@
 001aaf00: 2062 6c5f 726e 615f 6765 745f 7375 6263   bl_rna_get_subc
 001aaf10: 6c61 7373 5f70 7928 636c 732c 2069 643a  lass_py(cls, id:
 001aaf20: 2073 7472 2c20 6465 6661 756c 743a 2074   str, default: t
 001aaf30: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
 001aaf40: 2920 2d3e 2074 7970 696e 672e 5479 7065  ) -> typing.Type
 001aaf50: 3a0a 0a20 2020 202e 2e2e 0a0a 636c 6173  :..    .....clas
 001aaf60: 7320 5465 7874 7572 654e 6f64 6554 6578  s TextureNodeTex
-001aaf70: 4d61 6769 6328 6270 795f 7374 7275 6374  Magic(bpy_struct
-001aaf80: 2c20 5465 7874 7572 654e 6f64 652c 204e  , TextureNode, N
-001aaf90: 6f64 652c 204e 6f64 6549 6e74 6572 6e61  ode, NodeInterna
-001aafa0: 6c29 3a0a 0a20 2040 636c 6173 736d 6574  l):..  @classmet
+001aaf70: 4d61 6769 6328 5465 7874 7572 654e 6f64  Magic(TextureNod
+001aaf80: 652c 2062 7079 5f73 7472 7563 742c 204e  e, bpy_struct, N
+001aaf90: 6f64 6549 6e74 6572 6e61 6c2c 204e 6f64  odeInternal, Nod
+001aafa0: 6529 3a0a 0a20 2040 636c 6173 736d 6574  e):..  @classmet
 001aafb0: 686f 640a 0a20 2064 6566 2069 735f 7265  hod..  def is_re
 001aafc0: 6769 7374 6572 6564 5f6e 6f64 655f 7479  gistered_node_ty
 001aafd0: 7065 2863 6c73 2920 2d3e 2062 6f6f 6c3a  pe(cls) -> bool:
 001aafe0: 0a0a 2020 2020 2222 220a 0a20 2020 2054  ..    """..    T
 001aaff0: 7275 6520 6966 2061 2072 6567 6973 7465  rue if a registe
 001ab000: 7265 6420 6e6f 6465 2074 7970 650a 0a20  red node type.. 
 001ab010: 2020 2022 2222 0a0a 2020 2020 2e2e 2e0a     """..    ....
@@ -109341,17 +109341,17 @@
 001ab1c0: 5f67 6574 5f73 7562 636c 6173 735f 7079  _get_subclass_py
 001ab1d0: 2863 6c73 2c20 6964 3a20 7374 722c 2064  (cls, id: str, d
 001ab1e0: 6566 6175 6c74 3a20 7479 7069 6e67 2e41  efault: typing.A
 001ab1f0: 6e79 203d 204e 6f6e 6529 202d 3e20 7479  ny = None) -> ty
 001ab200: 7069 6e67 2e54 7970 653a 0a0a 2020 2020  ping.Type:..    
 001ab210: 2e2e 2e0a 0a63 6c61 7373 2054 6578 7475  .....class Textu
 001ab220: 7265 4e6f 6465 5465 784d 6172 626c 6528  reNodeTexMarble(
-001ab230: 6270 795f 7374 7275 6374 2c20 5465 7874  bpy_struct, Text
-001ab240: 7572 654e 6f64 652c 204e 6f64 652c 204e  ureNode, Node, N
-001ab250: 6f64 6549 6e74 6572 6e61 6c29 3a0a 0a20  odeInternal):.. 
+001ab230: 5465 7874 7572 654e 6f64 652c 2062 7079  TextureNode, bpy
+001ab240: 5f73 7472 7563 742c 204e 6f64 6549 6e74  _struct, NodeInt
+001ab250: 6572 6e61 6c2c 204e 6f64 6529 3a0a 0a20  ernal, Node):.. 
 001ab260: 2040 636c 6173 736d 6574 686f 640a 0a20   @classmethod.. 
 001ab270: 2064 6566 2069 735f 7265 6769 7374 6572   def is_register
 001ab280: 6564 5f6e 6f64 655f 7479 7065 2863 6c73  ed_node_type(cls
 001ab290: 2920 2d3e 2062 6f6f 6c3a 0a0a 2020 2020  ) -> bool:..    
 001ab2a0: 2222 220a 0a20 2020 2054 7275 6520 6966  """..    True if
 001ab2b0: 2061 2072 6567 6973 7465 7265 6420 6e6f   a registered no
 001ab2c0: 6465 2074 7970 650a 0a20 2020 2022 2222  de type..    """
@@ -109384,18 +109384,18 @@
 001ab470: 6465 6620 626c 5f72 6e61 5f67 6574 5f73  def bl_rna_get_s
 001ab480: 7562 636c 6173 735f 7079 2863 6c73 2c20  ubclass_py(cls, 
 001ab490: 6964 3a20 7374 722c 2064 6566 6175 6c74  id: str, default
 001ab4a0: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
 001ab4b0: 6f6e 6529 202d 3e20 7479 7069 6e67 2e54  one) -> typing.T
 001ab4c0: 7970 653a 0a0a 2020 2020 2e2e 2e0a 0a63  ype:..    .....c
 001ab4d0: 6c61 7373 2054 6578 7475 7265 4e6f 6465  lass TextureNode
-001ab4e0: 5465 784d 7573 6772 6176 6528 6270 795f  TexMusgrave(bpy_
-001ab4f0: 7374 7275 6374 2c20 5465 7874 7572 654e  struct, TextureN
-001ab500: 6f64 652c 204e 6f64 652c 204e 6f64 6549  ode, Node, NodeI
-001ab510: 6e74 6572 6e61 6c29 3a0a 0a20 2040 636c  nternal):..  @cl
+001ab4e0: 5465 784d 7573 6772 6176 6528 5465 7874  TexMusgrave(Text
+001ab4f0: 7572 654e 6f64 652c 2062 7079 5f73 7472  ureNode, bpy_str
+001ab500: 7563 742c 204e 6f64 6549 6e74 6572 6e61  uct, NodeInterna
+001ab510: 6c2c 204e 6f64 6529 3a0a 0a20 2040 636c  l, Node):..  @cl
 001ab520: 6173 736d 6574 686f 640a 0a20 2064 6566  assmethod..  def
 001ab530: 2069 735f 7265 6769 7374 6572 6564 5f6e   is_registered_n
 001ab540: 6f64 655f 7479 7065 2863 6c73 2920 2d3e  ode_type(cls) ->
 001ab550: 2062 6f6f 6c3a 0a0a 2020 2020 2222 220a   bool:..    """.
 001ab560: 0a20 2020 2054 7275 6520 6966 2061 2072  .    True if a r
 001ab570: 6567 6973 7465 7265 6420 6e6f 6465 2074  egistered node t
 001ab580: 7970 650a 0a20 2020 2022 2222 0a0a 2020  ype..    """..  
@@ -109428,17 +109428,17 @@
 001ab730: 626c 5f72 6e61 5f67 6574 5f73 7562 636c  bl_rna_get_subcl
 001ab740: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 001ab750: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 001ab760: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 001ab770: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 001ab780: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 001ab790: 2054 6578 7475 7265 4e6f 6465 5465 784e   TextureNodeTexN
-001ab7a0: 6f69 7365 2862 7079 5f73 7472 7563 742c  oise(bpy_struct,
-001ab7b0: 2054 6578 7475 7265 4e6f 6465 2c20 4e6f   TextureNode, No
-001ab7c0: 6465 2c20 4e6f 6465 496e 7465 726e 616c  de, NodeInternal
+001ab7a0: 6f69 7365 2854 6578 7475 7265 4e6f 6465  oise(TextureNode
+001ab7b0: 2c20 6270 795f 7374 7275 6374 2c20 4e6f  , bpy_struct, No
+001ab7c0: 6465 496e 7465 726e 616c 2c20 4e6f 6465  deInternal, Node
 001ab7d0: 293a 0a0a 2020 4063 6c61 7373 6d65 7468  ):..  @classmeth
 001ab7e0: 6f64 0a0a 2020 6465 6620 6973 5f72 6567  od..  def is_reg
 001ab7f0: 6973 7465 7265 645f 6e6f 6465 5f74 7970  istered_node_typ
 001ab800: 6528 636c 7329 202d 3e20 626f 6f6c 3a0a  e(cls) -> bool:.
 001ab810: 0a20 2020 2022 2222 0a0a 2020 2020 5472  .    """..    Tr
 001ab820: 7565 2069 6620 6120 7265 6769 7374 6572  ue if a register
 001ab830: 6564 206e 6f64 6520 7479 7065 0a0a 2020  ed node type..  
@@ -109471,18 +109471,18 @@
 001ab9e0: 640a 0a20 2064 6566 2062 6c5f 726e 615f  d..  def bl_rna_
 001ab9f0: 6765 745f 7375 6263 6c61 7373 5f70 7928  get_subclass_py(
 001aba00: 636c 732c 2069 643a 2073 7472 2c20 6465  cls, id: str, de
 001aba10: 6661 756c 743a 2074 7970 696e 672e 416e  fault: typing.An
 001aba20: 7920 3d20 4e6f 6e65 2920 2d3e 2074 7970  y = None) -> typ
 001aba30: 696e 672e 5479 7065 3a0a 0a20 2020 202e  ing.Type:..    .
 001aba40: 2e2e 0a0a 636c 6173 7320 5465 7874 7572  ....class Textur
-001aba50: 654e 6f64 6554 6578 5374 7563 6369 2862  eNodeTexStucci(b
-001aba60: 7079 5f73 7472 7563 742c 2054 6578 7475  py_struct, Textu
-001aba70: 7265 4e6f 6465 2c20 4e6f 6465 2c20 4e6f  reNode, Node, No
-001aba80: 6465 496e 7465 726e 616c 293a 0a0a 2020  deInternal):..  
+001aba50: 654e 6f64 6554 6578 5374 7563 6369 2854  eNodeTexStucci(T
+001aba60: 6578 7475 7265 4e6f 6465 2c20 6270 795f  extureNode, bpy_
+001aba70: 7374 7275 6374 2c20 4e6f 6465 496e 7465  struct, NodeInte
+001aba80: 726e 616c 2c20 4e6f 6465 293a 0a0a 2020  rnal, Node):..  
 001aba90: 4063 6c61 7373 6d65 7468 6f64 0a0a 2020  @classmethod..  
 001abaa0: 6465 6620 6973 5f72 6567 6973 7465 7265  def is_registere
 001abab0: 645f 6e6f 6465 5f74 7970 6528 636c 7329  d_node_type(cls)
 001abac0: 202d 3e20 626f 6f6c 3a0a 0a20 2020 2022   -> bool:..    "
 001abad0: 2222 0a0a 2020 2020 5472 7565 2069 6620  ""..    True if 
 001abae0: 6120 7265 6769 7374 6572 6564 206e 6f64  a registered nod
 001abaf0: 6520 7479 7065 0a0a 2020 2020 2222 220a  e type..    """.
@@ -109515,18 +109515,18 @@
 001abca0: 6566 2062 6c5f 726e 615f 6765 745f 7375  ef bl_rna_get_su
 001abcb0: 6263 6c61 7373 5f70 7928 636c 732c 2069  bclass_py(cls, i
 001abcc0: 643a 2073 7472 2c20 6465 6661 756c 743a  d: str, default:
 001abcd0: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
 001abce0: 6e65 2920 2d3e 2074 7970 696e 672e 5479  ne) -> typing.Ty
 001abcf0: 7065 3a0a 0a20 2020 202e 2e2e 0a0a 636c  pe:..    .....cl
 001abd00: 6173 7320 5465 7874 7572 654e 6f64 6554  ass TextureNodeT
-001abd10: 6578 566f 726f 6e6f 6928 6270 795f 7374  exVoronoi(bpy_st
-001abd20: 7275 6374 2c20 5465 7874 7572 654e 6f64  ruct, TextureNod
-001abd30: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-001abd40: 6572 6e61 6c29 3a0a 0a20 2040 636c 6173  ernal):..  @clas
+001abd10: 6578 566f 726f 6e6f 6928 5465 7874 7572  exVoronoi(Textur
+001abd20: 654e 6f64 652c 2062 7079 5f73 7472 7563  eNode, bpy_struc
+001abd30: 742c 204e 6f64 6549 6e74 6572 6e61 6c2c  t, NodeInternal,
+001abd40: 204e 6f64 6529 3a0a 0a20 2040 636c 6173   Node):..  @clas
 001abd50: 736d 6574 686f 640a 0a20 2064 6566 2069  smethod..  def i
 001abd60: 735f 7265 6769 7374 6572 6564 5f6e 6f64  s_registered_nod
 001abd70: 655f 7479 7065 2863 6c73 2920 2d3e 2062  e_type(cls) -> b
 001abd80: 6f6f 6c3a 0a0a 2020 2020 2222 220a 0a20  ool:..    """.. 
 001abd90: 2020 2054 7275 6520 6966 2061 2072 6567     True if a reg
 001abda0: 6973 7465 7265 6420 6e6f 6465 2074 7970  istered node typ
 001abdb0: 650a 0a20 2020 2022 2222 0a0a 2020 2020  e..    """..    
@@ -109559,17 +109559,17 @@
 001abf60: 5f72 6e61 5f67 6574 5f73 7562 636c 6173  _rna_get_subclas
 001abf70: 735f 7079 2863 6c73 2c20 6964 3a20 7374  s_py(cls, id: st
 001abf80: 722c 2064 6566 6175 6c74 3a20 7479 7069  r, default: typi
 001abf90: 6e67 2e41 6e79 203d 204e 6f6e 6529 202d  ng.Any = None) -
 001abfa0: 3e20 7479 7069 6e67 2e54 7970 653a 0a0a  > typing.Type:..
 001abfb0: 2020 2020 2e2e 2e0a 0a63 6c61 7373 2054      .....class T
 001abfc0: 6578 7475 7265 4e6f 6465 5465 7857 6f6f  extureNodeTexWoo
-001abfd0: 6428 6270 795f 7374 7275 6374 2c20 5465  d(bpy_struct, Te
-001abfe0: 7874 7572 654e 6f64 652c 204e 6f64 652c  xtureNode, Node,
-001abff0: 204e 6f64 6549 6e74 6572 6e61 6c29 3a0a   NodeInternal):.
+001abfd0: 6428 5465 7874 7572 654e 6f64 652c 2062  d(TextureNode, b
+001abfe0: 7079 5f73 7472 7563 742c 204e 6f64 6549  py_struct, NodeI
+001abff0: 6e74 6572 6e61 6c2c 204e 6f64 6529 3a0a  nternal, Node):.
 001ac000: 0a20 2040 636c 6173 736d 6574 686f 640a  .  @classmethod.
 001ac010: 0a20 2064 6566 2069 735f 7265 6769 7374  .  def is_regist
 001ac020: 6572 6564 5f6e 6f64 655f 7479 7065 2863  ered_node_type(c
 001ac030: 6c73 2920 2d3e 2062 6f6f 6c3a 0a0a 2020  ls) -> bool:..  
 001ac040: 2020 2222 220a 0a20 2020 2054 7275 6520    """..    True 
 001ac050: 6966 2061 2072 6567 6973 7465 7265 6420  if a registered 
 001ac060: 6e6f 6465 2074 7970 650a 0a20 2020 2022  node type..    "
@@ -109602,18 +109602,18 @@
 001ac210: 2020 6465 6620 626c 5f72 6e61 5f67 6574    def bl_rna_get
 001ac220: 5f73 7562 636c 6173 735f 7079 2863 6c73  _subclass_py(cls
 001ac230: 2c20 6964 3a20 7374 722c 2064 6566 6175  , id: str, defau
 001ac240: 6c74 3a20 7479 7069 6e67 2e41 6e79 203d  lt: typing.Any =
 001ac250: 204e 6f6e 6529 202d 3e20 7479 7069 6e67   None) -> typing
 001ac260: 2e54 7970 653a 0a0a 2020 2020 2e2e 2e0a  .Type:..    ....
 001ac270: 0a63 6c61 7373 2054 6578 7475 7265 4e6f  .class TextureNo
-001ac280: 6465 5465 7874 7572 6528 6270 795f 7374  deTexture(bpy_st
-001ac290: 7275 6374 2c20 5465 7874 7572 654e 6f64  ruct, TextureNod
-001ac2a0: 652c 204e 6f64 652c 204e 6f64 6549 6e74  e, Node, NodeInt
-001ac2b0: 6572 6e61 6c29 3a0a 0a20 206e 6f64 655f  ernal):..  node_
+001ac280: 6465 5465 7874 7572 6528 5465 7874 7572  deTexture(Textur
+001ac290: 654e 6f64 652c 2062 7079 5f73 7472 7563  eNode, bpy_struc
+001ac2a0: 742c 204e 6f64 6549 6e74 6572 6e61 6c2c  t, NodeInternal,
+001ac2b0: 204e 6f64 6529 3a0a 0a20 206e 6f64 655f   Node):..  node_
 001ac2c0: 6f75 7470 7574 3a20 696e 7420 3d20 2e2e  output: int = ..
 001ac2d0: 2e0a 0a20 2022 2222 0a0a 2020 466f 7220  ...  """..  For 
 001ac2e0: 6e6f 6465 2d62 6173 6564 2074 6578 7475  node-based textu
 001ac2f0: 7265 732c 2077 6869 6368 206f 7574 7075  res, which outpu
 001ac300: 7420 6e6f 6465 2074 6f20 7573 650a 0a20  t node to use.. 
 001ac310: 2022 2222 0a0a 2020 7465 7874 7572 653a   """..  texture:
 001ac320: 2054 6578 7475 7265 203d 202e 2e2e 0a0a   Texture = .....
@@ -109653,18 +109653,18 @@
 001ac540: 2064 6566 2062 6c5f 726e 615f 6765 745f   def bl_rna_get_
 001ac550: 7375 6263 6c61 7373 5f70 7928 636c 732c  subclass_py(cls,
 001ac560: 2069 643a 2073 7472 2c20 6465 6661 756c   id: str, defaul
 001ac570: 743a 2074 7970 696e 672e 416e 7920 3d20  t: typing.Any = 
 001ac580: 4e6f 6e65 2920 2d3e 2074 7970 696e 672e  None) -> typing.
 001ac590: 5479 7065 3a0a 0a20 2020 202e 2e2e 0a0a  Type:..    .....
 001ac5a0: 636c 6173 7320 5465 7874 7572 654e 6f64  class TextureNod
-001ac5b0: 6554 7261 6e73 6c61 7465 2862 7079 5f73  eTranslate(bpy_s
-001ac5c0: 7472 7563 742c 2054 6578 7475 7265 4e6f  truct, TextureNo
-001ac5d0: 6465 2c20 4e6f 6465 2c20 4e6f 6465 496e  de, Node, NodeIn
-001ac5e0: 7465 726e 616c 293a 0a0a 2020 4063 6c61  ternal):..  @cla
+001ac5b0: 6554 7261 6e73 6c61 7465 2854 6578 7475  eTranslate(Textu
+001ac5c0: 7265 4e6f 6465 2c20 6270 795f 7374 7275  reNode, bpy_stru
+001ac5d0: 6374 2c20 4e6f 6465 496e 7465 726e 616c  ct, NodeInternal
+001ac5e0: 2c20 4e6f 6465 293a 0a0a 2020 4063 6c61  , Node):..  @cla
 001ac5f0: 7373 6d65 7468 6f64 0a0a 2020 6465 6620  ssmethod..  def 
 001ac600: 6973 5f72 6567 6973 7465 7265 645f 6e6f  is_registered_no
 001ac610: 6465 5f74 7970 6528 636c 7329 202d 3e20  de_type(cls) -> 
 001ac620: 626f 6f6c 3a0a 0a20 2020 2022 2222 0a0a  bool:..    """..
 001ac630: 2020 2020 5472 7565 2069 6620 6120 7265      True if a re
 001ac640: 6769 7374 6572 6564 206e 6f64 6520 7479  gistered node ty
 001ac650: 7065 0a0a 2020 2020 2222 220a 0a20 2020  pe..    """..   
@@ -109697,17 +109697,17 @@
 001ac800: 6c5f 726e 615f 6765 745f 7375 6263 6c61  l_rna_get_subcla
 001ac810: 7373 5f70 7928 636c 732c 2069 643a 2073  ss_py(cls, id: s
 001ac820: 7472 2c20 6465 6661 756c 743a 2074 7970  tr, default: typ
 001ac830: 696e 672e 416e 7920 3d20 4e6f 6e65 2920  ing.Any = None) 
 001ac840: 2d3e 2074 7970 696e 672e 5479 7065 3a0a  -> typing.Type:.
 001ac850: 0a20 2020 202e 2e2e 0a0a 636c 6173 7320  .    .....class 
 001ac860: 5465 7874 7572 654e 6f64 6556 616c 546f  TextureNodeValTo
-001ac870: 4e6f 7228 6270 795f 7374 7275 6374 2c20  Nor(bpy_struct, 
-001ac880: 5465 7874 7572 654e 6f64 652c 204e 6f64  TextureNode, Nod
-001ac890: 652c 204e 6f64 6549 6e74 6572 6e61 6c29  e, NodeInternal)
+001ac870: 4e6f 7228 5465 7874 7572 654e 6f64 652c  Nor(TextureNode,
+001ac880: 2062 7079 5f73 7472 7563 742c 204e 6f64   bpy_struct, Nod
+001ac890: 6549 6e74 6572 6e61 6c2c 204e 6f64 6529  eInternal, Node)
 001ac8a0: 3a0a 0a20 2040 636c 6173 736d 6574 686f  :..  @classmetho
 001ac8b0: 640a 0a20 2064 6566 2069 735f 7265 6769  d..  def is_regi
 001ac8c0: 7374 6572 6564 5f6e 6f64 655f 7479 7065  stered_node_type
 001ac8d0: 2863 6c73 2920 2d3e 2062 6f6f 6c3a 0a0a  (cls) -> bool:..
 001ac8e0: 2020 2020 2222 220a 0a20 2020 2054 7275      """..    Tru
 001ac8f0: 6520 6966 2061 2072 6567 6973 7465 7265  e if a registere
 001ac900: 6420 6e6f 6465 2074 7970 650a 0a20 2020  d node type..   
@@ -109740,18 +109740,18 @@
 001acab0: 0a0a 2020 6465 6620 626c 5f72 6e61 5f67  ..  def bl_rna_g
 001acac0: 6574 5f73 7562 636c 6173 735f 7079 2863  et_subclass_py(c
 001acad0: 6c73 2c20 6964 3a20 7374 722c 2064 6566  ls, id: str, def
 001acae0: 6175 6c74 3a20 7479 7069 6e67 2e41 6e79  ault: typing.Any
 001acaf0: 203d 204e 6f6e 6529 202d 3e20 7479 7069   = None) -> typi
 001acb00: 6e67 2e54 7970 653a 0a0a 2020 2020 2e2e  ng.Type:..    ..
 001acb10: 2e0a 0a63 6c61 7373 2054 6578 7475 7265  ...class Texture
-001acb20: 4e6f 6465 5661 6c54 6f52 4742 2862 7079  NodeValToRGB(bpy
-001acb30: 5f73 7472 7563 742c 2054 6578 7475 7265  _struct, Texture
-001acb40: 4e6f 6465 2c20 4e6f 6465 2c20 4e6f 6465  Node, Node, Node
-001acb50: 496e 7465 726e 616c 293a 0a0a 2020 636f  Internal):..  co
+001acb20: 4e6f 6465 5661 6c54 6f52 4742 2854 6578  NodeValToRGB(Tex
+001acb30: 7475 7265 4e6f 6465 2c20 6270 795f 7374  tureNode, bpy_st
+001acb40: 7275 6374 2c20 4e6f 6465 496e 7465 726e  ruct, NodeIntern
+001acb50: 616c 2c20 4e6f 6465 293a 0a0a 2020 636f  al, Node):..  co
 001acb60: 6c6f 725f 7261 6d70 3a20 436f 6c6f 7252  lor_ramp: ColorR
 001acb70: 616d 7020 3d20 2e2e 2e0a 0a20 2040 636c  amp = .....  @cl
 001acb80: 6173 736d 6574 686f 640a 0a20 2064 6566  assmethod..  def
 001acb90: 2069 735f 7265 6769 7374 6572 6564 5f6e   is_registered_n
 001acba0: 6f64 655f 7479 7065 2863 6c73 2920 2d3e  ode_type(cls) ->
 001acbb0: 2062 6f6f 6c3a 0a0a 2020 2020 2222 220a   bool:..    """.
 001acbc0: 0a20 2020 2054 7275 6520 6966 2061 2072  .    True if a r
@@ -109786,17 +109786,17 @@
 001acd90: 626c 5f72 6e61 5f67 6574 5f73 7562 636c  bl_rna_get_subcl
 001acda0: 6173 735f 7079 2863 6c73 2c20 6964 3a20  ass_py(cls, id: 
 001acdb0: 7374 722c 2064 6566 6175 6c74 3a20 7479  str, default: ty
 001acdc0: 7069 6e67 2e41 6e79 203d 204e 6f6e 6529  ping.Any = None)
 001acdd0: 202d 3e20 7479 7069 6e67 2e54 7970 653a   -> typing.Type:
 001acde0: 0a0a 2020 2020 2e2e 2e0a 0a63 6c61 7373  ..    .....class
 001acdf0: 2054 6578 7475 7265 4e6f 6465 5669 6577   TextureNodeView
-001ace00: 6572 2862 7079 5f73 7472 7563 742c 2054  er(bpy_struct, T
-001ace10: 6578 7475 7265 4e6f 6465 2c20 4e6f 6465  extureNode, Node
-001ace20: 2c20 4e6f 6465 496e 7465 726e 616c 293a  , NodeInternal):
+001ace00: 6572 2854 6578 7475 7265 4e6f 6465 2c20  er(TextureNode, 
+001ace10: 6270 795f 7374 7275 6374 2c20 4e6f 6465  bpy_struct, Node
+001ace20: 496e 7465 726e 616c 2c20 4e6f 6465 293a  Internal, Node):
 001ace30: 0a0a 2020 4063 6c61 7373 6d65 7468 6f64  ..  @classmethod
 001ace40: 0a0a 2020 6465 6620 6973 5f72 6567 6973  ..  def is_regis
 001ace50: 7465 7265 645f 6e6f 6465 5f74 7970 6528  tered_node_type(
 001ace60: 636c 7329 202d 3e20 626f 6f6c 3a0a 0a20  cls) -> bool:.. 
 001ace70: 2020 2022 2222 0a0a 2020 2020 5472 7565     """..    True
 001ace80: 2069 6620 6120 7265 6769 7374 6572 6564   if a registered
 001ace90: 206e 6f64 6520 7479 7065 0a0a 2020 2020   node type..
```

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/utils/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/utils/previews.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/utils/previews.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy/utils/units.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy/utils/units.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy_extras/anim_utils.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy_extras/anim_utils.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy_extras/image_utils.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy_extras/image_utils.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy_extras/io_utils.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy_extras/io_utils.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy_extras/keyconfig_utils.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy_extras/keyconfig_utils.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy_extras/mesh_utils.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy_extras/mesh_utils.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy_extras/object_utils.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy_extras/object_utils.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/bpy_extras/view3d_utils.pyi` & `blender-stubs-3.2.0.27.dev4648006602/bpy_extras/view3d_utils.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/brush_automasking_flag_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/brush_automasking_flag_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/brush_curves_sculpt_tool_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/brush_curves_sculpt_tool_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/brush_gpencil_sculpt_types_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/brush_gpencil_sculpt_types_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/brush_sculpt_tool_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/brush_sculpt_tool_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/color_sets_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/color_sets_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/constraint_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/constraint_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/context_mode_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/context_mode_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/driver_target_rotation_mode_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/driver_target_rotation_mode_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/dt_method_edge_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/dt_method_edge_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/dt_method_loop_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/dt_method_loop_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/dt_method_poly_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/dt_method_poly_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/dt_method_vertex_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/dt_method_vertex_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/dt_mix_mode_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/dt_mix_mode_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/event_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/event_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/fmodifier_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/fmodifier_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/freestyle/chainingiterators.pyi` & `blender-stubs-3.2.0.27.dev4648006602/freestyle/chainingiterators.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/freestyle/functions.pyi` & `blender-stubs-3.2.0.27.dev4648006602/freestyle/functions.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/freestyle/predicates.pyi` & `blender-stubs-3.2.0.27.dev4648006602/freestyle/predicates.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/freestyle/shaders.pyi` & `blender-stubs-3.2.0.27.dev4648006602/freestyle/shaders.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/freestyle/types.pyi` & `blender-stubs-3.2.0.27.dev4648006602/freestyle/types.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/freestyle/utils.pyi` & `blender-stubs-3.2.0.27.dev4648006602/freestyle/utils.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/gpu/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/gpu/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/gpu/capabilities.pyi` & `blender-stubs-3.2.0.27.dev4648006602/gpu/capabilities.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/gpu/matrix.pyi` & `blender-stubs-3.2.0.27.dev4648006602/gpu/matrix.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/gpu/platform.pyi` & `blender-stubs-3.2.0.27.dev4648006602/gpu/platform.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/gpu/shader.pyi` & `blender-stubs-3.2.0.27.dev4648006602/gpu/shader.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/gpu/state.pyi` & `blender-stubs-3.2.0.27.dev4648006602/gpu/state.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/gpu/texture.pyi` & `blender-stubs-3.2.0.27.dev4648006602/gpu/texture.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/gpu/types.pyi` & `blender-stubs-3.2.0.27.dev4648006602/gpu/types.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/gpu_extras/presets.pyi` & `blender-stubs-3.2.0.27.dev4648006602/gpu_extras/presets.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/icon_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/icon_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/id_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/id_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/idprop/types.pyi` & `blender-stubs-3.2.0.27.dev4648006602/idprop/types.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/image_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/image_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/imbuf/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/imbuf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/imbuf/types.pyi` & `blender-stubs-3.2.0.27.dev4648006602/imbuf/types.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/info_advanced_blender_as_bpy/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/info_advanced_blender_as_bpy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/keyframe_handle_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/keyframe_handle_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/keyframe_paste_offset_value/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/keyframe_paste_offset_value/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/keying_flag_items_api/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/keying_flag_items_api/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/linestyle_geometry_modifier_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/linestyle_geometry_modifier_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/mathutils/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/mathutils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/mathutils/bvhtree.pyi` & `blender-stubs-3.2.0.27.dev4648006602/mathutils/bvhtree.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/mathutils/geometry.pyi` & `blender-stubs-3.2.0.27.dev4648006602/mathutils/geometry.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/mathutils/kdtree.pyi` & `blender-stubs-3.2.0.27.dev4648006602/mathutils/kdtree.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/mathutils/noise.pyi` & `blender-stubs-3.2.0.27.dev4648006602/mathutils/noise.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/modifier_shrinkwrap_mode_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/modifier_shrinkwrap_mode_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/modifier_triangulate_quad_method_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/modifier_triangulate_quad_method_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/nla_mode_blend_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/nla_mode_blend_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/node_boolean_math_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/node_boolean_math_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/node_compare_operation_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/node_compare_operation_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/node_float_compare_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/node_float_compare_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/node_map_range_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/node_map_range_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/node_math_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/node_math_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/node_vec_math_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/node_vec_math_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/object_gpencil_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/object_gpencil_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/object_greasepencil_modifier_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/object_greasepencil_modifier_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/object_mode_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/object_mode_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/object_modifier_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/object_modifier_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/object_rotation_mode_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/object_rotation_mode_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/object_shaderfx_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/object_shaderfx_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/object_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/object_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/operator_context_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/operator_context_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/operator_return_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/operator_return_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/operator_type_flag_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/operator_type_flag_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/preference_section_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/preference_section_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/property_subtype_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/property_subtype_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/property_subtype_number_array_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/property_subtype_number_array_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/property_subtype_number_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/property_subtype_number_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/property_unit_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/property_unit_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/proportional_falloff_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/proportional_falloff_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/ramp_blend_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/ramp_blend_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/region_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/region_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/render_pass_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/render_pass_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/rigidbody_constraint_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/rigidbody_constraint_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/rigidbody_object_shape_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/rigidbody_object_shape_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/setup.py` & `blender-stubs-3.2.0.27.dev4648006602/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import glob
 import os
 
 from setuptools import setup
 
 app_name = "blender"
 app_version = "3.2.0"
-build_number = "4642539589"
+build_number = "4648006602"
 
 module_version = "0.2.7"
 
 name = f"{app_name.lower()}-stubs"
 
 module_version = str(sum([int(n) * 10 ** (2 - i) for i, n in enumerate(module_version.split("."))]))
```

### Comparing `blender-stubs-3.2.0.27.dev4642539589/shrinkwrap_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/shrinkwrap_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/snap_element_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/snap_element_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/space_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/space_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/stereo3d_display_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/stereo3d_display_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/subdivision_uv_smooth_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/subdivision_uv_smooth_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/texture_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/texture_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/transform_mode_types/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/transform_mode_types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/transform_orientation_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/transform_orientation_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/transform_pivot_items_full/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/transform_pivot_items_full/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/volume_grid_data_type_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/volume_grid_data_type_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/window_cursor_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/window_cursor_items/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blender-stubs-3.2.0.27.dev4642539589/workspace_object_mode_items/__init__.pyi` & `blender-stubs-3.2.0.27.dev4648006602/workspace_object_mode_items/__init__.pyi`

 * *Files identical despite different names*

