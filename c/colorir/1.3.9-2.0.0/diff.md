# Comparing `tmp/colorir-1.3.9.tar.gz` & `tmp/colorir-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorir-1.3.9.tar", last modified: Sat Aug 13 06:38:48 2022, max compression
+gzip compressed data, was "colorir-2.0.0.tar", last modified: Sun Apr  9 06:08:26 2023, max compression
```

## Comparing `colorir-1.3.9.tar` & `colorir-2.0.0.tar`

### file list

```diff
@@ -1,63 +1,215 @@
-drwxrwxrwx   0        0        0        0 2022-08-13 06:38:48.743477 colorir-1.3.9/
--rw-rw-rw-   0        0        0     1067 2020-05-30 22:00:43.000000 colorir-1.3.9/LICENSE.txt
--rw-rw-rw-   0        0        0      188 2022-07-28 05:48:34.000000 colorir-1.3.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1997 2022-08-13 06:38:48.743477 colorir-1.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     1558 2022-07-24 04:23:53.000000 colorir-1.3.9/README.rst
-drwxrwxrwx   0        0        0        0 2022-08-13 06:38:48.644512 colorir-1.3.9/colorir/
--rw-rw-rw-   0        0        0      151 2022-08-13 06:38:25.000000 colorir-1.3.9/colorir/__init__.py
--rw-rw-rw-   0        0        0      615 2022-04-25 02:31:31.000000 colorir-1.3.9/colorir/__main__.py
-drwxrwxrwx   0        0        0        0 2022-08-13 06:38:48.719512 colorir-1.3.9/colorir/builtin_palettes/
--rw-rw-rw-   0        0        0      147 2022-07-24 04:23:53.000000 colorir-1.3.9/colorir/builtin_palettes/accent.spalette
--rw-rw-rw-   0        0        0      298 2022-04-21 22:35:31.000000 colorir-1.3.9/colorir/builtin_palettes/basic.palette
--rw-rw-rw-   0        0        0     4581 2022-04-21 22:35:31.000000 colorir-1.3.9/colorir/builtin_palettes/css.palette
--rw-rw-rw-   0        0        0      147 2022-07-24 04:23:53.000000 colorir-1.3.9/colorir/builtin_palettes/dark2.spalette
--rw-rw-rw-   0        0        0      477 2022-04-21 22:35:31.000000 colorir-1.3.9/colorir/builtin_palettes/fluorescent.palette
--rw-rw-rw-   0        0        0      478 2022-04-21 22:35:31.000000 colorir-1.3.9/colorir/builtin_palettes/gem_tones.palette
--rw-rw-rw-   0        0        0      522 2022-04-21 22:35:31.000000 colorir-1.3.9/colorir/builtin_palettes/heads_n_tails.palette
--rw-rw-rw-   0        0        0      870 2022-04-21 22:35:31.000000 colorir-1.3.9/colorir/builtin_palettes/magic_scent.palette
--rw-rw-rw-   0        0        0      533 2022-04-21 22:35:31.000000 colorir-1.3.9/colorir/builtin_palettes/metallic_fx.palette
--rw-rw-rw-   0        0        0      234 2022-04-21 22:35:31.000000 colorir-1.3.9/colorir/builtin_palettes/mystic_forest.palette
--rw-rw-rw-   0        0        0      219 2022-07-24 04:23:53.000000 colorir-1.3.9/colorir/builtin_palettes/paired.spalette
--rw-rw-rw-   0        0        0      816 2022-08-05 03:22:53.000000 colorir-1.3.9/colorir/builtin_palettes/pantone_years.palette
--rw-rw-rw-   0        0        0      165 2022-07-24 04:23:53.000000 colorir-1.3.9/colorir/builtin_palettes/pastel1.spalette
--rw-rw-rw-   0        0        0      147 2022-07-24 04:23:53.000000 colorir-1.3.9/colorir/builtin_palettes/pastel2.spalette
--rw-rw-rw-   0        0        0     2087 2022-08-05 03:02:56.000000 colorir-1.3.9/colorir/builtin_palettes/pigments.palette
--rw-rw-rw-   0        0        0      193 2022-04-25 00:35:32.000000 colorir-1.3.9/colorir/builtin_palettes/rainbow.palette
--rw-rw-rw-   0        0        0      165 2022-07-24 04:23:53.000000 colorir-1.3.9/colorir/builtin_palettes/set1.spalette
--rw-rw-rw-   0        0        0      147 2022-07-24 04:23:53.000000 colorir-1.3.9/colorir/builtin_palettes/set2.spalette
--rw-rw-rw-   0        0        0      219 2022-07-24 04:23:53.000000 colorir-1.3.9/colorir/builtin_palettes/set3.spalette
--rw-rw-rw-   0        0        0      542 2022-04-21 22:35:31.000000 colorir-1.3.9/colorir/builtin_palettes/silly_scents.palette
--rw-rw-rw-   0        0        0      801 2022-04-21 22:35:31.000000 colorir-1.3.9/colorir/builtin_palettes/silver_swirls.palette
--rw-rw-rw-   0        0        0      299 2022-08-04 18:05:39.000000 colorir-1.3.9/colorir/builtin_palettes/tab10.palette
--rw-rw-rw-   0        0        0      363 2022-07-24 04:23:53.000000 colorir-1.3.9/colorir/builtin_palettes/tab20.spalette
--rw-rw-rw-   0        0        0      363 2022-07-24 04:23:53.000000 colorir-1.3.9/colorir/builtin_palettes/tab20b.spalette
--rw-rw-rw-   0        0        0      363 2022-07-24 04:23:53.000000 colorir-1.3.9/colorir/builtin_palettes/tab20c.spalette
--rw-rw-rw-   0        0        0      523 2022-04-21 22:35:31.000000 colorir-1.3.9/colorir/builtin_palettes/world_flags.palette
--rw-rw-rw-   0        0        0    32183 2022-07-30 02:11:41.000000 colorir-1.3.9/colorir/color_class.py
--rw-rw-rw-   0        0        0    10264 2022-08-13 06:37:32.000000 colorir-1.3.9/colorir/color_format.py
--rw-rw-rw-   0        0        0      752 2022-07-24 04:23:53.000000 colorir-1.3.9/colorir/config.py
-drwxrwxrwx   0        0        0        0 2022-08-13 06:38:48.730536 colorir-1.3.9/colorir/examples/
--rw-rw-rw-   0        0        0     3149 2022-07-30 04:47:42.000000 colorir-1.3.9/colorir/examples/color_picker.py
--rw-rw-rw-   0        0        0     1665 2022-08-13 06:36:59.000000 colorir-1.3.9/colorir/examples/color_wheel.py
-drwxrwxrwx   0        0        0        0 2022-08-13 06:38:48.733484 colorir-1.3.9/colorir/examples/ex_palettes/
--rw-rw-rw-   0        0        0      392 2022-04-22 08:41:53.000000 colorir-1.3.9/colorir/examples/ex_palettes/turtles.palette
--rw-rw-rw-   0        0        0      833 2022-04-24 15:55:58.000000 colorir-1.3.9/colorir/examples/simple_pygame.py
--rw-rw-rw-   0        0        0      253 2022-04-24 15:55:58.000000 colorir-1.3.9/colorir/examples/simple_turtle_1.py
--rw-rw-rw-   0        0        0      436 2022-04-24 15:55:58.000000 colorir-1.3.9/colorir/examples/simple_turtle_2.py
--rw-rw-rw-   0        0        0     7472 2022-08-13 06:32:00.000000 colorir-1.3.9/colorir/gradient.py
--rw-rw-rw-   0        0        0    35859 2022-08-09 00:34:14.000000 colorir-1.3.9/colorir/palette.py
-drwxrwxrwx   0        0        0        0 2022-08-13 06:38:48.735480 colorir-1.3.9/colorir/palettes/
--rw-rw-rw-   0        0        0        0 2022-04-22 15:10:59.000000 colorir-1.3.9/colorir/palettes/.empty
--rw-rw-rw-   0        0        0     9734 2022-08-13 06:20:49.000000 colorir-1.3.9/colorir/utils.py
-drwxrwxrwx   0        0        0        0 2022-08-13 06:38:48.667519 colorir-1.3.9/colorir.egg-info/
--rw-rw-rw-   0        0        0     1997 2022-08-13 06:38:48.000000 colorir-1.3.9/colorir.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1770 2022-08-13 06:38:48.000000 colorir-1.3.9/colorir.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-13 06:38:48.000000 colorir-1.3.9/colorir.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2022-08-13 06:38:48.000000 colorir-1.3.9/colorir.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-08-13 06:38:48.000000 colorir-1.3.9/colorir.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-13 06:38:48.744480 colorir-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0      712 2022-08-13 06:38:25.000000 colorir-1.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-13 06:38:48.741479 colorir-1.3.9/tests/
--rw-rw-rw-   0        0        0      236 2022-04-20 02:41:43.000000 colorir-1.3.9/tests/test_color_format.py
--rw-rw-rw-   0        0        0      228 2022-04-21 19:25:50.000000 colorir-1.3.9/tests/test_gradient.py
--rw-rw-rw-   0        0        0     3606 2022-06-14 15:07:24.000000 colorir-1.3.9/tests/test_palette.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:08:26.842364 colorir-2.0.0/
+-rw-rw-rw-   0        0        0     1067 2020-05-30 22:00:43.000000 colorir-2.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      188 2022-07-28 05:48:34.000000 colorir-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2702 2023-04-09 06:08:26.842364 colorir-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2284 2023-04-09 05:42:57.000000 colorir-2.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-09 06:08:26.370179 colorir-2.0.0/colorir/
+-rw-rw-rw-   0        0        0      179 2023-04-06 19:42:03.000000 colorir-2.0.0/colorir/__init__.py
+-rw-rw-rw-   0        0        0      605 2023-02-27 01:21:37.000000 colorir-2.0.0/colorir/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:08:26.732445 colorir-2.0.0/colorir/builtin_palettes/
+-rw-rw-rw-   0        0        0      147 2022-07-24 04:23:53.000000 colorir-2.0.0/colorir/builtin_palettes/accent.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/afmhot.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/ag_grnyl.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/ag_sunset.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/algae.spalette
+-rw-rw-rw-   0        0        0      471 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/alphabet.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/amp.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/antique.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/armyrose.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/autumn.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/balance.spalette
+-rw-rw-rw-   0        0        0      298 2022-04-21 22:35:31.000000 colorir-2.0.0/colorir/builtin_palettes/basic.palette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/binary.spalette
+-rw-rw-rw-   0        0        0       93 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/blackbody.spalette
+-rw-rw-rw-   0        0        0       39 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/bluered.spalette
+-rw-rw-rw-   0        0        0      165 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/blues.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/blugrn.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/bluyl.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/bold.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/bone.spalette
+-rw-rw-rw-   0        0        0      201 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/brbg.spalette
+-rw-rw-rw-   0        0        0      183 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/bright.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/brwnyl.spalette
+-rw-rw-rw-   0        0        0      165 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/bugn.spalette
+-rw-rw-rw-   0        0        0      165 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/bupu.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/burg.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/burgyl.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/bwr.spalette
+-rw-rw-rw-   0        0        0      201 2023-02-26 18:31:26.000000 colorir-2.0.0/colorir/builtin_palettes/carnival.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/cividis.spalette
+-rw-rw-rw-   0        0        0      183 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/colorblind.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/cool.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/coolwarm.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/copper.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/crest.spalette
+-rw-rw-rw-   0        0        0     4581 2022-04-21 22:35:31.000000 colorir-2.0.0/colorir/builtin_palettes/css.palette
+-rw-rw-rw-   0        0        0      381 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/cubehelix.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/curl.spalette
+-rw-rw-rw-   0        0        0      183 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/d3.spalette
+-rw-rw-rw-   0        0        0      183 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/dark.spalette
+-rw-rw-rw-   0        0        0      147 2022-07-24 04:23:53.000000 colorir-2.0.0/colorir/builtin_palettes/dark2.spalette
+-rw-rw-rw-   0        0        0      435 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/dark24.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/darkmint.spalette
+-rw-rw-rw-   0        0        0      183 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/deep.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/delta.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/dense.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/earth.spalette
+-rw-rw-rw-   0        0        0      309 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/edge.spalette
+-rw-rw-rw-   0        0        0      111 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/electric.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/emrld.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/fall.spalette
+-rw-rw-rw-   0        0        0      133 2022-08-13 19:42:11.000000 colorir-2.0.0/colorir/builtin_palettes/fire.palette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/flare.spalette
+-rw-rw-rw-   0        0        0      477 2022-04-21 22:35:31.000000 colorir-2.0.0/colorir/builtin_palettes/fluorescent.palette
+-rw-rw-rw-   0        0        0      183 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/g10.spalette
+-rw-rw-rw-   0        0        0      478 2022-04-21 22:35:31.000000 colorir-2.0.0/colorir/builtin_palettes/gem_tones.palette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/geyser.spalette
+-rw-rw-rw-   0        0        0      381 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/gist_earth.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/gist_gray.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/gist_heat.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/gist_yarg.spalette
+-rw-rw-rw-   0        0        0      165 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/gnbu.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/gray.spalette
+-rw-rw-rw-   0        0        0      165 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/greens.spalette
+-rw-rw-rw-   0        0        0      165 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/greys.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/haline.spalette
+-rw-rw-rw-   0        0        0      522 2022-04-21 22:35:31.000000 colorir-2.0.0/colorir/builtin_palettes/heads_n_tails.palette
+-rw-rw-rw-   0        0        0      381 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/hot.spalette
+-rw-rw-rw-   0        0        0      381 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/hsv.spalette
+-rw-rw-rw-   0        0        0       57 2022-08-13 18:32:19.000000 colorir-2.0.0/colorir/builtin_palettes/hyacinth_macaw.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:07.000000 colorir-2.0.0/colorir/builtin_palettes/ice.spalette
+-rw-rw-rw-   0        0        0      381 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/icefire.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/inferno.spalette
+-rw-rw-rw-   0        0        0      381 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/jet.spalette
+-rw-rw-rw-   0        0        0      435 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/light24.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/magenta.spalette
+-rw-rw-rw-   0        0        0      870 2022-04-21 22:35:31.000000 colorir-2.0.0/colorir/builtin_palettes/magic_scent.palette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/magma.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/mako.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/matter.spalette
+-rw-rw-rw-   0        0        0      533 2022-04-21 22:35:31.000000 colorir-2.0.0/colorir/builtin_palettes/metallic_fx.palette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/mint.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/mpl_rainbow.spalette
+-rw-rw-rw-   0        0        0      309 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/mrybm.spalette
+-rw-rw-rw-   0        0        0      183 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/muted.spalette
+-rw-rw-rw-   0        0        0      309 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/mygbm.spalette
+-rw-rw-rw-   0        0        0      234 2022-04-21 22:35:31.000000 colorir-2.0.0/colorir/builtin_palettes/mystic_forest.palette
+-rw-rw-rw-   0        0        0      381 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/ocean.spalette
+-rw-rw-rw-   0        0        0      165 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/oranges.spalette
+-rw-rw-rw-   0        0        0      165 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/orrd.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/oryel.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/oxy.spalette
+-rw-rw-rw-   0        0        0      219 2022-07-24 04:23:53.000000 colorir-2.0.0/colorir/builtin_palettes/paired.spalette
+-rw-rw-rw-   0        0        0      816 2022-08-05 03:22:53.000000 colorir-2.0.0/colorir/builtin_palettes/pantone_years.palette
+-rw-rw-rw-   0        0        0      154 2022-08-14 07:00:30.000000 colorir-2.0.0/colorir/builtin_palettes/passion.palette
+-rw-rw-rw-   0        0        0      183 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/pastel.spalette
+-rw-rw-rw-   0        0        0      165 2022-07-24 04:23:53.000000 colorir-2.0.0/colorir/builtin_palettes/pastel1.spalette
+-rw-rw-rw-   0        0        0      147 2022-07-24 04:23:53.000000 colorir-2.0.0/colorir/builtin_palettes/pastel2.spalette
+-rw-rw-rw-   0        0        0      156 2022-08-14 06:24:15.000000 colorir-2.0.0/colorir/builtin_palettes/peace.palette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/peach.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/phase.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/picnic.spalette
+-rw-rw-rw-   0        0        0     2087 2022-08-05 03:02:56.000000 colorir-2.0.0/colorir/builtin_palettes/pigments.palette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/pink.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/pinkyl.spalette
+-rw-rw-rw-   0        0        0      201 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/piyg.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/plasma.spalette
+-rw-rw-rw-   0        0        0      183 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/plotly.spalette
+-rw-rw-rw-   0        0        0      237 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/plotly3.spalette
+-rw-rw-rw-   0        0        0      309 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/plotly_icefire.spalette
+-rw-rw-rw-   0        0        0       93 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/portland.spalette
+-rw-rw-rw-   0        0        0       75 2022-08-13 18:34:59.000000 colorir-2.0.0/colorir/builtin_palettes/precious_tanager.spalette
+-rw-rw-rw-   0        0        0      201 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/prgn.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/prism.spalette
+-rw-rw-rw-   0        0        0      165 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/pubu.spalette
+-rw-rw-rw-   0        0        0      165 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/pubugn.spalette
+-rw-rw-rw-   0        0        0      201 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/puor.spalette
+-rw-rw-rw-   0        0        0      165 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/purd.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/purp.spalette
+-rw-rw-rw-   0        0        0      165 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/purples.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/purpor.spalette
+-rw-rw-rw-   0        0        0      193 2022-04-25 00:35:32.000000 colorir-2.0.0/colorir/builtin_palettes/rainbow.palette
+-rw-rw-rw-   0        0        0      201 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/rdbu.spalette
+-rw-rw-rw-   0        0        0      201 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/rdgy.spalette
+-rw-rw-rw-   0        0        0      165 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/rdpu.spalette
+-rw-rw-rw-   0        0        0      201 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/rdylbu.spalette
+-rw-rw-rw-   0        0        0      201 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/rdylgn.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/redor.spalette
+-rw-rw-rw-   0        0        0      165 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/reds.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/rocket.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/safe.spalette
+-rw-rw-rw-   0        0        0       75 2022-08-13 18:37:31.000000 colorir-2.0.0/colorir/builtin_palettes/scarlet_macaw.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/seismic.spalette
+-rw-rw-rw-   0        0        0      165 2022-07-24 04:23:53.000000 colorir-2.0.0/colorir/builtin_palettes/set1.spalette
+-rw-rw-rw-   0        0        0      147 2022-07-24 04:23:53.000000 colorir-2.0.0/colorir/builtin_palettes/set2.spalette
+-rw-rw-rw-   0        0        0      219 2022-07-24 04:23:53.000000 colorir-2.0.0/colorir/builtin_palettes/set3.spalette
+-rw-rw-rw-   0        0        0      542 2022-04-21 22:35:31.000000 colorir-2.0.0/colorir/builtin_palettes/silly_scents.palette
+-rw-rw-rw-   0        0        0      801 2022-04-21 22:35:31.000000 colorir-2.0.0/colorir/builtin_palettes/silver_swirls.palette
+-rw-rw-rw-   0        0        0      179 2022-08-15 04:02:01.000000 colorir-2.0.0/colorir/builtin_palettes/sky.palette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/solar.spalette
+-rw-rw-rw-   0        0        0      201 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/spectral.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/speed.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/spring.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/summer.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/sunset.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/sunsetdark.spalette
+-rw-rw-rw-   0        0        0      183 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/t10.spalette
+-rw-rw-rw-   0        0        0      299 2022-08-04 18:05:39.000000 colorir-2.0.0/colorir/builtin_palettes/tab10.palette
+-rw-rw-rw-   0        0        0      363 2022-07-24 04:23:53.000000 colorir-2.0.0/colorir/builtin_palettes/tab20.spalette
+-rw-rw-rw-   0        0        0      363 2022-07-24 04:23:53.000000 colorir-2.0.0/colorir/builtin_palettes/tab20b.spalette
+-rw-rw-rw-   0        0        0      363 2022-07-24 04:23:53.000000 colorir-2.0.0/colorir/builtin_palettes/tab20c.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/teal.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/tealgrn.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/tealrose.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/tempo.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/temps.spalette
+-rw-rw-rw-   0        0        0      381 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/terrain.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/thermal.spalette
+-rw-rw-rw-   0        0        0       75 2022-08-13 18:39:06.000000 colorir-2.0.0/colorir/builtin_palettes/toco_toucan.spalette
+-rw-rw-rw-   0        0        0      129 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/tropic.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/turbid.spalette
+-rw-rw-rw-   0        0        0      381 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/turbo.spalette
+-rw-rw-rw-   0        0        0      381 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/twilight.spalette
+-rw-rw-rw-   0        0        0      381 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/twilight_shifted.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/viridis.spalette
+-rw-rw-rw-   0        0        0      219 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/vivid.spalette
+-rw-rw-rw-   0        0        0      381 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/vlag.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/winter.spalette
+-rw-rw-rw-   0        0        0      201 2023-03-19 21:13:08.000000 colorir-2.0.0/colorir/builtin_palettes/wistia.spalette
+-rw-rw-rw-   0        0        0      523 2022-04-21 22:35:31.000000 colorir-2.0.0/colorir/builtin_palettes/world_flags.palette
+-rw-rw-rw-   0        0        0      165 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/ylgn.spalette
+-rw-rw-rw-   0        0        0      165 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/ylgnbu.spalette
+-rw-rw-rw-   0        0        0      165 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/ylorbr.spalette
+-rw-rw-rw-   0        0        0      165 2022-08-16 15:09:54.000000 colorir-2.0.0/colorir/builtin_palettes/ylorrd.spalette
+-rw-rw-rw-   0        0        0    37470 2023-04-09 05:21:50.000000 colorir-2.0.0/colorir/color_class.py
+-rw-rw-rw-   0        0        0    10592 2023-04-06 19:37:30.000000 colorir-2.0.0/colorir/color_format.py
+-rw-rw-rw-   0        0        0     1203 2022-08-15 00:47:56.000000 colorir-2.0.0/colorir/config.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:08:26.795002 colorir-2.0.0/colorir/examples/
+-rw-rw-rw-   0        0        0     3153 2023-02-19 15:25:11.000000 colorir-2.0.0/colorir/examples/color_picker.py
+-rw-rw-rw-   0        0        0     1749 2023-02-27 01:16:13.000000 colorir-2.0.0/colorir/examples/color_wheel.py
+-rw-rw-rw-   0        0        0     1559 2023-04-08 01:12:27.000000 colorir-2.0.0/colorir/examples/custom_palettes.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:08:26.826730 colorir-2.0.0/colorir/examples/ex_palettes/
+-rw-rw-rw-   0        0        0      392 2022-04-22 08:41:53.000000 colorir-2.0.0/colorir/examples/ex_palettes/turtle.palette
+-rw-rw-rw-   0        0        0     4619 2023-03-23 20:08:17.000000 colorir-2.0.0/colorir/examples/gapminder.csv
+-rw-rw-rw-   0        0        0     7955 2023-04-08 19:47:35.000000 colorir-2.0.0/colorir/examples/palette_picker.py
+-rw-rw-rw-   0        0        0     5079 2023-03-23 18:14:52.000000 colorir-2.0.0/colorir/examples/surface_data.csv
+-rw-rw-rw-   0        0        0    13836 2023-04-08 01:13:53.000000 colorir-2.0.0/colorir/gradient.py
+-rw-rw-rw-   0        0        0    40421 2023-04-09 05:14:23.000000 colorir-2.0.0/colorir/palette.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:08:26.826730 colorir-2.0.0/colorir/palettes/
+-rw-rw-rw-   0        0        0        0 2022-04-22 15:11:10.000000 colorir-2.0.0/colorir/palettes/.empty
+-rw-rw-rw-   0        0        0     2661 2023-02-25 19:52:14.000000 colorir-2.0.0/colorir/tkinter_utils.py
+-rw-rw-rw-   0        0        0    14971 2023-04-09 06:06:44.000000 colorir-2.0.0/colorir/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:08:26.402137 colorir-2.0.0/colorir.egg-info/
+-rw-rw-rw-   0        0        0     2702 2023-04-09 06:08:26.000000 colorir-2.0.0/colorir.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7929 2023-04-09 06:08:26.000000 colorir-2.0.0/colorir.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 06:08:26.000000 colorir-2.0.0/colorir.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-09 06:08:26.000000 colorir-2.0.0/colorir.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-09 06:08:26.000000 colorir-2.0.0/colorir.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 06:08:26.842364 colorir-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-04-06 19:42:03.000000 colorir-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:08:26.842364 colorir-2.0.0/tests/
+-rw-rw-rw-   0        0        0     3117 2023-02-25 19:52:14.000000 colorir-2.0.0/tests/test_color_class.py
+-rw-rw-rw-   0        0        0      264 2022-08-15 01:32:54.000000 colorir-2.0.0/tests/test_color_format.py
+-rw-rw-rw-   0        0        0      260 2022-08-15 01:32:54.000000 colorir-2.0.0/tests/test_gradient.py
+-rw-rw-rw-   0        0        0     3479 2023-02-26 02:55:17.000000 colorir-2.0.0/tests/test_palette.py
+-rw-rw-rw-   0        0        0      441 2023-02-25 19:52:14.000000 colorir-2.0.0/tests/test_utils.py
```

### Comparing `colorir-1.3.9/LICENSE.txt` & `colorir-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `colorir-1.3.9/PKG-INFO` & `colorir-2.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,81 @@
 Metadata-Version: 2.1
 Name: colorir
-Version: 1.3.9
+Version: 2.0.0
 Summary: A python package for easy management of colors and palettes.
 Home-page: https://github.com/aleferna12/colorir
 Author: aleferna
 Author-email: alexandrepchfernandes@gmail.com
 License: MIT
 Project-URL: Documentation, https://colorir.readthedocs.io/en/latest/
-Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 .. note::
 
     colorir is still in its early days and slight modifications to the API may happen between versions.
 
 What is colorir?
 ----------------
 
-colorir is a package developed to unify your workflow with colors across different projects.
+colorir is a package that allows users to manipulate colors and palettes.
 
 With colorir you can:
 
-- Keep a unified selection of colors you like and use them in your different projects;
-- Use these colors directly as input for other graphical or web frameworks;
+- Create palettes and save them to use in different projects;
+- Have access to a curated selection of unique color palettes and color names;
 - Easily convert between different color systems and formats;
 - Create gradients between colors and sample from them;
 - Easily visualize swatches of colors in the terminal;
-- And much more!
+- Pass color values directly as input for other graphical or web frameworks;
+- And more!
 
 colorir was designed to be your best friend when dealing with colors so that you won't ever need to write this kind of code again:
 
 .. code-block:: python
 
     BLACK = (0, 0, 0)
     WHITE = (255, 255, 255)
     CSS_ALICEBLUE = (240, 248, 255)
-    COOL_PURPLE = (11, 0, 51)
-    MY_FAVORITE_GREEN = (113, 180, 141)
-    TOP_NOTCH_RED = (131, 34, 50)
-    # ... unnecessarily long and ugly list of colors
+    BACKGROUND_COLOR = (11, 0, 51)
+    FONT_COLOR = (113, 180, 141)
+    LINE_PLOT_COLOR = (131, 34, 50)
+    # ... long and ugly list of colors
 
 Getting Started
 ---------------
 
 Getting started with colorir can be as simple as:
 
 .. code-block:: python
 
-    import tkinter as tk
-    from colorir import *
+    sky = Palette.load("sky")  # Loads a previously created palette called sky
+    sky_grad = PolarGrad([sky.sunrise, sky.highnoon])  # Creates a gradient from the color "sunrise" to the color "highnoon"
+    swatch(sky)  # Shows colorir objects in the terminal
+    swatch(sky_grad)
 
-    colors = Palette.load()  # Load colors
+This code should print both the palette and the gradient directly in your terminal:
 
-    win = tk.Tk()
-    win.configure(bg=colors.magicmint)  # Set background to 'magicmint' color
-    win.mainloop()
+.. image:: docs/source/images/readme_sky.png
 
-.. image:: readme_example.png
+Colorir can be used to interpolate and manipulate colors in many different color systems,
+such as CIELab and HCLab (LCHab).
 
-For more information (including use-cases and examples), see colorir's documentation `here <https://colorir.readthedocs.io/en/latest/>`_.
+Now let's make a gray scale version of the sky palette and save it to use later on
+another project:
+
+.. code-block:: python
+
+    gray_sky = sky.grayscale()
+    gray_sky.save("gray_sky")
+
+Now the gray_sky palette can be loaded with from a different script:
 
+.. code-block:: python
+
+    gray_sky = Palette.load("gray_sky")
+    swatch(gray_sky)
+
+.. image:: docs/source/images/readme_gray_sky.png
+
+For more information (including use-cases and examples), see colorir's documentation `here <https://colorir.readthedocs.io/en/latest/>`_.
```

### Comparing `colorir-1.3.9/README.rst` & `colorir-2.0.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,68 @@
 .. note::
 
     colorir is still in its early days and slight modifications to the API may happen between versions.
 
 What is colorir?
 ----------------
 
-colorir is a package developed to unify your workflow with colors across different projects.
+colorir is a package that allows users to manipulate colors and palettes.
 
 With colorir you can:
 
-- Keep a unified selection of colors you like and use them in your different projects;
-- Use these colors directly as input for other graphical or web frameworks;
+- Create palettes and save them to use in different projects;
+- Have access to a curated selection of unique color palettes and color names;
 - Easily convert between different color systems and formats;
 - Create gradients between colors and sample from them;
 - Easily visualize swatches of colors in the terminal;
-- And much more!
+- Pass color values directly as input for other graphical or web frameworks;
+- And more!
 
 colorir was designed to be your best friend when dealing with colors so that you won't ever need to write this kind of code again:
 
 .. code-block:: python
 
     BLACK = (0, 0, 0)
     WHITE = (255, 255, 255)
     CSS_ALICEBLUE = (240, 248, 255)
-    COOL_PURPLE = (11, 0, 51)
-    MY_FAVORITE_GREEN = (113, 180, 141)
-    TOP_NOTCH_RED = (131, 34, 50)
-    # ... unnecessarily long and ugly list of colors
+    BACKGROUND_COLOR = (11, 0, 51)
+    FONT_COLOR = (113, 180, 141)
+    LINE_PLOT_COLOR = (131, 34, 50)
+    # ... long and ugly list of colors
 
 Getting Started
 ---------------
 
 Getting started with colorir can be as simple as:
 
 .. code-block:: python
 
-    import tkinter as tk
-    from colorir import *
+    sky = Palette.load("sky")  # Loads a previously created palette called sky
+    sky_grad = PolarGrad([sky.sunrise, sky.highnoon])  # Creates a gradient from the color "sunrise" to the color "highnoon"
+    swatch(sky)  # Shows colorir objects in the terminal
+    swatch(sky_grad)
 
-    colors = Palette.load()  # Load colors
+This code should print both the palette and the gradient directly in your terminal:
 
-    win = tk.Tk()
-    win.configure(bg=colors.magicmint)  # Set background to 'magicmint' color
-    win.mainloop()
+.. image:: docs/source/images/readme_sky.png
 
-.. image:: readme_example.png
+Colorir can be used to interpolate and manipulate colors in many different color systems,
+such as CIELab and HCLab (LCHab).
+
+Now let's make a gray scale version of the sky palette and save it to use later on
+another project:
+
+.. code-block:: python
+
+    gray_sky = sky.grayscale()
+    gray_sky.save("gray_sky")
+
+Now the gray_sky palette can be loaded with from a different script:
+
+.. code-block:: python
+
+    gray_sky = Palette.load("gray_sky")
+    swatch(gray_sky)
+
+.. image:: docs/source/images/readme_gray_sky.png
 
 For more information (including use-cases and examples), see colorir's documentation `here <https://colorir.readthedocs.io/en/latest/>`_.
```

### Comparing `colorir-1.3.9/colorir/builtin_palettes/css.palette` & `colorir-2.0.0/colorir/builtin_palettes/css.palette`

 * *Files identical despite different names*

### Comparing `colorir-1.3.9/colorir/builtin_palettes/heads_n_tails.palette` & `colorir-2.0.0/colorir/builtin_palettes/heads_n_tails.palette`

 * *Files identical despite different names*

### Comparing `colorir-1.3.9/colorir/builtin_palettes/magic_scent.palette` & `colorir-2.0.0/colorir/builtin_palettes/magic_scent.palette`

 * *Files identical despite different names*

### Comparing `colorir-1.3.9/colorir/builtin_palettes/metallic_fx.palette` & `colorir-2.0.0/colorir/builtin_palettes/metallic_fx.palette`

 * *Files identical despite different names*

### Comparing `colorir-1.3.9/colorir/builtin_palettes/pantone_years.palette` & `colorir-2.0.0/colorir/builtin_palettes/pantone_years.palette`

 * *Files identical despite different names*

### Comparing `colorir-1.3.9/colorir/builtin_palettes/pigments.palette` & `colorir-2.0.0/colorir/builtin_palettes/pigments.palette`

 * *Files identical despite different names*

### Comparing `colorir-1.3.9/colorir/builtin_palettes/silly_scents.palette` & `colorir-2.0.0/colorir/builtin_palettes/silly_scents.palette`

 * *Files identical despite different names*

### Comparing `colorir-1.3.9/colorir/builtin_palettes/silver_swirls.palette` & `colorir-2.0.0/colorir/builtin_palettes/silver_swirls.palette`

 * *Files identical despite different names*

### Comparing `colorir-1.3.9/colorir/builtin_palettes/world_flags.palette` & `colorir-2.0.0/colorir/builtin_palettes/world_flags.palette`

 * *Files identical despite different names*

### Comparing `colorir-1.3.9/colorir/color_class.py` & `colorir-2.0.0/colorir/color_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,51 +2,71 @@
 
 This module contains different classes that represent a few of the most common color spaces [#]_.
 Colors can be compared, converted to and passed as arguments to different classes.
 
 Examples:
     Create some colors and compare them:
 
-    >>> sRGB(255, 0, 0) == HSL(0, 1 , 0.5)
+    >>> RGB(1, 0, 0) == HSL(0, 1 , 0.5)
     True
 
     Convert an RGB color to CMYK:
 
-    >>> rgb_red = sRGB(255, 0, 0)
+    >>> rgb_red = RGB(1, 0, 0)
     >>> rgb_red.cmyk()
     CMYK(0.0, 1.0, 1.0, 0.0)
 
+    Color arithmetic makes it easy to change the properties of a color.
+    The operations are performed element-wise in the format of the color used as the right operand,
+    allowing specific color components to be changed in the color on the left of the operator.
+    If the right operand is not a color, but rather a tuple, than the left color is not converted
+    prior to the operation being performed.
+
+    Add some CIE lightness to the color black (right operand is CIELab, meaning that the Hex color will be converted
+    to CIELab before adding 50 to its lighness value and then converted back to Hex):
+
+    >>> Hex("#000000") + CIELab(50, 0, 0)
+    Hex('#777777')
+
+    Make a red 50% less saturated by multiplying its saturation component by 0.5 (here no conversion is performed
+    because the right operand is a tuple rather than a color class):
+
+    >>> HSV(0.0, 1.0, 1.0) * (1, 0.5, 1)
+    HSV(0.0, 0.5, 1.0)
+
 References:
     .. [#] Wikipedia at https://en.wikipedia.org/wiki/Color_model.
 """
 import abc
 import colorsys
+import operator
 import numpy as np
-from typing import List
+from typing import List, Union
 from colormath.color_objects import LabColor, LuvColor, LCHuvColor, sRGBColor, LCHabColor, \
     CMYColor, CMYKColor
 from colormath.color_conversions import convert_color
 
 import colorir
 
 __all__ = [
+    "ColorLike",
     "ColorBase",
     "ColorTupleBase",
     "ColorPolarBase",
+    "RGB",
     "sRGB",
     "HSV",
     "HSL",
     "CMY",
     "CMYK",
     "CIELuv",
     "CIELab",
     "HCLuv",
     "HCLab",
-    "Hex",
-    "HexRGB"
+    "Hex"
 ]
 
 
 class ColorBase(metaclass=abc.ABCMeta):
     """Base class from which all color classes inherit.
 
     Notes:
@@ -57,30 +77,60 @@
 
     # Factory method to be called when reading the palette files or reconstructing colors
     @classmethod
     @abc.abstractmethod
     def _from_rgba(cls, rgba, **kwargs):
         pass
 
+    @property
+    def format(self) -> "colorir.color_format.ColorFormat":
+        """Returns a :class:`~colorir.color_format.ColorFormat` representing the format of this
+        color object."""
+        format_ = {param: getattr(self, param) for param in self._format_params}
+        return colorir.color_format.ColorFormat(self.__class__, **format_)
+
     def __eq__(self, other):
-        return all(self._rgba == other._rgba) if isinstance(other, ColorBase) else False
+        try:
+            if not isinstance(other, ColorBase):
+                other = colorir.config.DEFAULT_COLOR_FORMAT.format(other)
+            return all(np.rint(self._rgba) == np.rint(other._rgba))
+        except colorir.color_format.FormatError:
+            return NotImplemented
 
     def __hash__(self):
         return hash(tuple(self._rgba))
 
-    def get_format(self) -> "colorir.color_format.ColorFormat":
-        """Returns a :class:`~colorir.color_format.ColorFormat` representing the format of this
-        color object."""
-        format_ = {param: getattr(self, param) for param in self._format_params}
-        return colorir.color_format.ColorFormat(self.__class__, **format_)
+    def __invert__(self):
+        """Gets the inverse RGB of this color."""
+        return self.format._from_rgba(np.append(255 - self._rgba[:-1], self._rgba[-1]))
+
+    def __mod__(self, other):
+        """Blends two colors at 50% using :func:`colorir.utils.blend()`."""
+        return colorir.blend(self, other)
+
+    def __add__(self, other):
+        """Adds two colors or a color (as the left operand) and a tuple (as the right operand) together."""
+        return self._arithm_func(other, operator.add)
+
+    def __sub__(self, other):
+        """Subtracts one color from another or a tuple (the right operand) from a color (the left operand)."""
+        return self._arithm_func(other, operator.sub)
+
+    def __mul__(self, other):
+        """Multiplies two colors or a color (as the left operand) and a tuple (as the right operand) together."""
+        return self._arithm_func(other, operator.mul)
+
+    def __truediv__(self, other):
+        """Divides two colors or a color (as the left operand) and a tuple (as the right operand) together."""
+        return self._arithm_func(other, operator.truediv)
 
     def grayscale(self):
-        """Converts this color to a grayscale representation in the same format using CIELuv
+        """Converts this color to a grayscale representation in the same format using CIE
         lightness component."""
-        return self.get_format().format(CIELuv(self.cieluv().l, 0, 0))
+        return self.format.format(CIELuv(self.cieluv().l, 0, 0))
 
     def hex(self, **kwargs) -> "Hex":
         """Converts the current color to a hexadecimal representation.
 
         Args:
             **kwargs: Keyword arguments wrapped in this function will be passed on to the
                 :class:`Hex` constructor.
@@ -164,21 +214,28 @@
 
         Args:
             **kwargs: Keyword arguments wrapped in this function will be passed on to the
                 :class:`HCLab` constructor.
         """
         return HCLab._from_rgba(self._rgba, **kwargs)
 
+    def _arithm_func(self, other, foo):
+        if not isinstance(other, ColorTupleBase):
+            raise ValueError("operations are only possible if one of the colors is tuple-based")
+        vals = tuple(map(foo, other.format.format(self), other))
+        return self.format.format(other.format.format(vals))
+
 
 class ColorTupleBase(ColorBase, tuple, metaclass=abc.ABCMeta):
     """Base class from which all color classes that are represented by tuples inherit.
 
     Notes:
         This class is abstract and should not be instantiated.
     """
+
     @abc.abstractmethod
     def __new__(cls, specs, a, rgba, include_a, round_to):
         specs = list(specs)
         if round_to == 0:
             specs = [round(val) for val in specs]
             a = round(a)
         elif round_to > 0:
@@ -191,43 +248,75 @@
         obj.include_a = include_a
         obj.round_to = round_to
         obj._rgba = np.rint(rgba).astype(int)
         obj._format_params = ["include_a", "round_to"]
 
         return obj
 
-    def __repr__(self):
-        return f"{self.__class__.__name__}{tuple.__repr__(self)}"
-
-    # It would be very dangerous to change str conversion as the target framework could call it
-    # expecting (255, 0, 0) and get sRGB(255, 0, 0)
+    # It would be dangerous to change str conversion as the target framework could call it
+    # expecting (255, 0, 0) and get RGB(255, 0, 0)
     def __str__(self):
         return tuple.__repr__(self)
 
-    def __eq__(self, other):
-        if isinstance(other, ColorBase):
-            return ColorBase.__eq__(self, other)
-        return tuple.__eq__(self, other)
+    def __repr__(self):
+        if colorir.config.REPR_STYLE == "traditional":
+            return f"{self.__class__.__name__}{tuple.__repr__(self)}"
+        if colorir.config.REPR_STYLE == "inherit":
+            return str(self)
+        return colorir.utils.swatch(self, file=None)
 
     def __hash__(self):
         return ColorBase.__hash__(self)
 
+    def __eq__(self, other):
+        colorbase_eq = ColorBase.__eq__(self, other)
+        # If other is ColorBase than we trust the result of eq
+        if isinstance(other, ColorBase):
+            return colorbase_eq
+        # Otherwise we also try tuple.__eq__
+        return any([colorbase_eq is True, tuple.__eq__(self, other) is True])
+
+    def __add__(self, other):
+        if not isinstance(other, ColorTupleBase):
+            return self._tup_arithm_func(other, operator.add)
+        return ColorBase.__add__(self, other)
+
+    def __sub__(self, other):
+        if not isinstance(other, ColorTupleBase):
+            return self._tup_arithm_func(other, operator.sub)
+        return ColorBase.__sub__(self, other)
+
+    def __mul__(self, other):
+        if not isinstance(other, ColorTupleBase):
+            return self._tup_arithm_func(other, operator.mul)
+        return ColorBase.__mul__(self, other)
+
+    def __truediv__(self, other):
+        if not isinstance(other, ColorTupleBase):
+            return self._tup_arithm_func(other, operator.truediv)
+        return ColorBase.__truediv__(self, other)
+
+    # If right side of the operator is not a tuple-based color, we perform the operation element-wise
+    def _tup_arithm_func(self, other, foo):
+        vals = tuple(map(foo, self, other))
+        return self.format.format(vals)
+
+
 
 class ColorPolarBase(ColorTupleBase, metaclass=abc.ABCMeta):
-    """Base class from which all color classes that are represented by tuples and have a hue
-     component in polar coordinates inherit.
+    """Mixin tag indicating that the color contains a polar HUE component.
 
     Notes:
         This class is abstract and should not be instantiated.
     """
     h: float
     max_h: float
 
 
-class sRGB(ColorTupleBase):
+class RGB(ColorTupleBase):
     """Represents a color in the RGB color space [#]_.
 
     References:
         .. [#] Wikipedia at https://en.wikipedia.org/wiki/SRGB.
 
     Args:
         r: Red component of the color.
@@ -236,68 +325,82 @@
         a: Opacity component of the color. Defaults to ``None``, which means it will be the same
             as the `max_rgba` parameter.
         max_rgb: What is the maximum value for the `r`, `g` and `b` components. Some common
             values for this parameter would be 255 or 1.
         max_a : What is the maximum value for the `a` component. Some common
             values for this parameter would be 100 or 1.
         include_a: Whether to include the opacity parameter `a` in the constructed tuple.
-            Setting it to ``True`` may result in an object such as :code:`sRGB(255, 255, 0,
-            255)` instead of :code:`sRGB(255, 255, 0)`, for exemple.
+            Setting it to ``True`` may result in an object such as :code:`RGB(255, 255, 0,
+            255)` instead of :code:`RGB(255, 255, 0)`, for example.
         round_to: Rounds the value of each color component to this many decimal places. Setting
             this parameter to 0 ensures that the components will be of type `int`. -1
             means that the components won't be rounded at all.
+        linear: Whether the values are linear RGB or sRGB. It is strongly advised not to keep values as
+            linear RGB, but it can be useful for quick conversions.
     """
+
     def __new__(cls,
                 r: float,
                 g: float,
                 b: float,
                 a: float = None,
-                max_rgb=255,
+                max_rgb=1,
                 max_a=1,
                 include_a=False,
-                round_to=0):
+                round_to=-1,
+                linear=False):
         if a is None:
             a = max_a
         elif not 0 <= a <= max_a:
             raise ValueError("'a' must be greater than 0 and smaller than 'max_a'")
         if not all(0 <= spec <= max_rgb for spec in (r, g, b)):
             raise ValueError("'r', 'g' and 'b' must be greater than 0 and smaller than 'max_rgb'")
 
-        rgba = np.array((r, g, b, a), dtype=float) * 255
+        rgba = np.array((r, g, b, a), dtype=float)
         rgba[:3] /= max_rgb
         rgba[-1] /= max_a
+        if linear:
+            rgba = colorir.utils._to_srgb(rgba)
+        rgba *= 255
 
         obj = super().__new__(
             cls,
             (r, g, b),
             a,
             rgba,
             include_a=include_a,
             round_to=round_to
         )
         obj.r, obj.g, obj.b = obj[:3]
         obj.max_rgb = max_rgb
         obj.max_a = max_a
-        obj._format_params += ["max_rgb", "max_a"]
+        obj.linear = linear
+        obj._format_params += ["max_rgb", "max_a", "linear"]
 
         return obj
 
     @classmethod
-    def _from_rgba(cls, rgba, max_rgb=255, max_a=1, include_a=False, round_to=0):
-        rgba_ = np.array(rgba) / 255 * max_rgb
+    def _from_rgba(cls, rgba, max_rgb=1, max_a=1, include_a=False, round_to=-1, linear=False):
+        rgb = rgba / 255
+        if linear:
+            rgb = colorir.utils._to_linear_rgb(rgb)
+        rgb = rgb[:-1]
+        rgb *= max_rgb
 
         obj = super().__new__(cls,
-                              rgba_[:3],
-                              rgba_[-1],
+                              rgb,
+                              rgba[-1] / 255 * max_a,
                               rgba,
                               include_a=include_a,
                               round_to=round_to)
         obj.r, obj.g, obj.b = obj[:3]
         obj.max_rgb = max_rgb
         obj.max_a = max_a
+        obj.linear = linear
+        obj._format_params += ["max_rgb", "max_a", "linear"]
         return obj
 
 
 class HSL(ColorPolarBase):
     """Represents a color in the HSL color space [#]_.
 
     .. [#] Wikipedia at https://en.wikipedia.org/wiki/HSL_and_HSV.
@@ -315,14 +418,15 @@
         include_a: Whether to include the opacity parameter `a` in the constructed tuple.
             Setting it to ``True`` may result in an object such as :code:`HSL(360, 1, 0,
             1)` instead of :code:`HSL(360, 1, 0)`, for exemple.
         round_to: Rounds the value of each color component to this many decimal places. Setting
             this parameter to 0 ensures that the components will be of type `int`. -1
             means that the components won't be rounded at all.
     """
+
     def __new__(cls,
                 h: float,
                 s: float,
                 l: float,
                 a: float = None,
                 max_h=360,
                 max_sla=1,
@@ -386,14 +490,15 @@
         include_a: Whether to include the opacity parameter `a` in the constructed tuple.
             Setting it to ``True`` may result in an object such as :code:`HSV(360, 1, 0,
             1)` instead of :code:`HSV(360, 1, 0)`, for exemple.
         round_to: Rounds the value of each color component to this many decimal places. Setting
             this parameter to 0 ensures that the components will be of type `int`. -1
             means that the components won't be rounded at all.
     """
+
     def __new__(cls,
                 h: float,
                 s: float,
                 v: float,
                 a: float = None,
                 max_h=360,
                 max_sva=1,
@@ -456,14 +561,15 @@
         include_a: Whether to include the opacity parameter `a` in the constructed tuple.
             Setting it to ``True`` may result in an object such as :code:`CMYK(1, 1, 0,
             1)` instead of :code:`CMYK(1, 1, 0)`, for exemple.
         round_to: Rounds the value of each color component to this many decimal places. Setting
             this parameter to 0 ensures that the components will be of type `int`. The default,
             -1, means that the components won't be rounded at all.
     """
+
     def __new__(cls, c: float, m: float, y: float, k: float, a: float = None, max_cmyka=1,
                 include_a=False,
                 round_to=-1):
         if a is None:
             a = max_cmyka
         if not all(0 <= spec <= max_cmyka for spec in (c, m, y, k, a)):
             raise ValueError("'c', 'm', 'y', 'k', and 'a' must be greater than 0 and smaller than "
@@ -525,14 +631,15 @@
         include_a: Whether to include the opacity parameter `a` in the constructed tuple.
             Setting it to ``True`` may result in an object such as :code:`CMY(1, 1, 0,
             1)` instead of :code:`CMY(1, 1, 0)`, for exemple.
         round_to: Rounds the value of each color component to this many decimal places. Setting
             this parameter to 0 ensures that the components will be of type `int`. The default,
             -1, means that the components won't be rounded at all.
     """
+
     def __new__(cls,
                 c: float,
                 m: float,
                 y: float,
                 a: float = None,
                 max_cmya=1,
                 include_a=False,
@@ -689,15 +796,15 @@
                               (h, c, l),
                               a,
                               rgba,
                               include_a=include_a,
                               round_to=round_to)
         obj.h, obj.c, obj.l = obj[:3]
         obj.max_h = max_h
-        obj.max_sla = max_a
+        obj.max_a = max_a
         obj._format_params += ["max_h", "max_a"]
 
         return obj
 
     @classmethod
     def _from_rgba(cls, rgba, max_h=360, max_a=1, include_a=False, round_to=-1):
         hcl = convert_color(
@@ -737,24 +844,23 @@
             LCHabColor(l, c, h / max_h * 360 % 360, illuminant="d65"),
             sRGBColor
         )
         rgba = (rgb.clamped_rgb_r * 255,
                 rgb.clamped_rgb_g * 255,
                 rgb.clamped_rgb_b * 255,
                 a / max_a * 255)
-
         obj = super().__new__(cls,
                               (h, c, l),
                               a,
                               rgba,
                               include_a=include_a,
                               round_to=round_to)
         obj.h, obj.c, obj.l = obj[:3]
         obj.max_h = max_h
-        obj.max_sla = max_a
+        obj.max_a = max_a
         obj._format_params += ["max_h", "max_a"]
 
         return obj
 
     @classmethod
     def _from_rgba(cls, rgba, max_h=360, max_a=1, include_a=False, round_to=-1):
         hcl = convert_color(
@@ -776,26 +882,28 @@
         obj.max_h = max_h
         obj.max_a = max_a
         obj._format_params += ["max_h", "max_a"]
 
         return obj
 
 
+# noinspection PyCallingNonCallable
 class Hex(ColorBase, str):
     """Represents a color in the RGB color space [#]_ as a hexadecimal string.
 
     Is mostly used for representing colors in web applications [#]_.
 
     References:
         .. [#] Wikipedia at https://en.wikipedia.org/wiki/SRGB.
         .. [#] Wikipedia at https://en.wikipedia.org/wiki/Web_colors
 
     Args:
         hex_str: Hexadecimal string from which the :class:`Hex` instance will be built.
-            May or may not include a "#" character in its beginning.
+            The format can be a string of 6 digits, 8 digits (with an alpha specifier in the beginning or the end),
+            or 3 digits, optionally including a '#' character.
         uppercase: Whether the color will be represented in uppercase or lowercase.
         include_a: Whether to include the opacity parameter `a` in the constructed string.
             Setting it to ``True`` may result in an object such as :code:`Hex('#ffffff00')`
             instead of :code:`Hex('#ffff00')`, for exemple.
         tail_a: Whether the alpha component is present in the tail or head of the hex string. Used
             only if `hex_str` includes an alpha component or `include_a` is ``True``.
 
@@ -805,23 +913,26 @@
 
         >>> Hex("#FF0000", include_hash=False)
         Hex('ff0000')
 
         >>> Hex("ff0000", include_a=True, tail_a=True)
         Hex('#ff0000ff')
     """
+
     def __new__(cls,
                 hex_str: str,
                 uppercase=False,
                 include_hash=True,
                 include_a=False,
                 tail_a=False):
         hex_str = hex_str.lstrip("#")
-        if not 6 <= len(hex_str) <= 9:
-            raise ValueError("'hex_str' length must be between 6 and 9 (inclusive)")
+        if len(hex_str) not in (3, 6, 8):
+            raise ValueError("'hex_str' length must be 3, 6 or 8 (excluding the optional '#')")
+        if len(hex_str) == 3:
+            hex_str = "".join(i + j for i, j in zip(hex_str, hex_str))
         if len(hex_str) < 8:
             i = 0
             a = 255
         elif tail_a:
             i = 0
             a = int(hex_str[-2:], 16)
         else:
@@ -859,26 +970,37 @@
         obj.include_hash = include_hash
         obj.include_a = include_a
         obj.tail_a = tail_a
         obj._rgba = np.rint(rgba).astype(int)
         obj._format_params = ["uppercase", "include_hash", "include_a", "tail_a"]
         return obj
 
-    def __repr__(self):
-        return f"{self.__class__.__name__}({str.__repr__(self)})"
-
-    # It would be very dangerous to change str conversion as the target framework could call it
+    # It would be dangerous to change str conversion as the target framework could call it
     # expecting #ff0000 and get Hex('#ff0000')
     def __str__(self):
         return str.__str__(self)
 
-    def __eq__(self, other):
-        if isinstance(other, ColorBase):
-            return ColorBase.__eq__(self, other)
-        return str.__eq__(self, other)
+    def __repr__(self):
+        if colorir.config.REPR_STYLE == "traditional":
+            return f"{self.__class__.__name__}({str.__repr__(self)})"
+        if colorir.config.REPR_STYLE == "inherit":
+            return str(self)
+        return colorir.utils.swatch(self, file=None)
 
     def __hash__(self):
         return ColorBase.__hash__(self)
 
+    def __eq__(self, other):
+        colorbase_eq = ColorBase.__eq__(self, other)
+        # If other is ColorBase than we trust the result of eq
+        if isinstance(other, ColorBase):
+            return colorbase_eq
+        # Otherwise we also try str.__eq__
+        return any([colorbase_eq is True, str.__eq__(self, other) is True])
+
+
+# Aliases
+HexRGB = Hex
+sRGB = RGB
 
-# Alias
-HexRGB = Hex
+ColorLike = Union[ColorBase, str, tuple]
+"""Type constant that describes common representations of colors in python."""
```

### Comparing `colorir-1.3.9/colorir/color_format.py` & `colorir-2.0.0/colorir/color_format.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Color format specifications for creating and interpreting representations of colors.
 
 Often only describing a color system is not enough when dealing with libraries and frameworks
 specifications. For example, both Kivy [1]_ and PyGame [2]_ use mostly RGB colors as inputs when
 building applications. However, Kivy expects the colors to have a maximum value of 1, while PyGame
 expects it to be 255. To bridge these expectations and allow the use of the same set of colors for
 multiple projects across different frameworks, the :class:`ColorFormat` class was created.
-This class can be used to build strictly defined formats which allows the creation and
+This class can be used to build strictly defined formats which act as a template for the creation and
 interpretation of colors using :meth:`ColorFormat.new_color()` and :meth:`ColorFormat.format()`
 respectively.
 
 Interpreting color-like objects
 -------------------------------
 
 Most functions and classes of colorir can take as a parameter a type called
@@ -84,44 +84,40 @@
     To change the default color format to a custom or pre-built color format, take
     a look at :data:`config.DEFAULT_COLOR_FORMAT <colorir.config.DEFAULT_COLOR_FORMAT>`.
 
 References:
     .. [1] Kivy: Cross-platform Python Framework for NUI Development at https://kivy.org/.
     .. [2] PyGame library at https://www.pygame.org/.
 """
-from typing import Type, Union, NewType
-
+from typing import Type
 from . import color_class
 
 __all__ = [
-    "ColorLike",
     "ColorFormat",
+    "FormatError",
     "PYGAME_COLOR_FORMAT",
     "TKINTER_COLOR_FORMAT",
     "KIVY_COLOR_FORMAT",
     "WEB_COLOR_FORMAT",
     "MATPLOTLIB_COLOR_FORMAT"
 ]
 
-ColorLike = NewType("ColorLike", Union["color_class.ColorBase", str, tuple, list])
-"""Type constant that describes common representations of colors in python."""
-
 
 class ColorFormat:
     """Class to create color format specifications.
 
     Args:
         color_sys: The color system that is the basis of this color format.
         format_kwargs: Keyword arguments that further specify the color format. These are specific
             to each color system and can be consulted in their respective documentations.
 
     Examples:
         >>> c_format = ColorFormat(color_class.sRGB, max_rgb=1)
         >>> c_format.new_color(1, 0, 0)
-        sRGB(1, 0, 0)
+        RGB(1, 0, 0)
 
         For more examples see the documentation of the :mod:`~colorir.color_format` module.
     """
     def __init__(self, color_sys: Type["color_class.ColorBase"], **format_kwargs):
         self.color_sys = color_sys
         self.format_params = format_kwargs
 
@@ -149,71 +145,88 @@
 
         Examples:
             >>> c_format = ColorFormat(color_class.sRGB,
             ...                        max_rgb=1,
             ...                        max_a=1,
             ...                        include_a=True)
             >>> c_format.new_color(1, 0, 0)
-            sRGB(1, 0, 0, 1)
+            RGB(1, 0, 0, 1)
         """
         kwargs.update(self.format_params)
         return self.color_sys(*args, **kwargs)
 
     # Factory method to be called when reading the palette files or reconstructing colors
     def _from_rgba(self, rgba):
         return self.color_sys._from_rgba(rgba, **self.format_params)
 
-    def format(self, color: ColorLike) -> "color_class.ColorBase":
+    def format(self, color: "color_class.ColorLike") -> "color_class.ColorBase":
         """Tries to format a color-like object into this color format.
 
         Because there are multiple implementations of tuple-based color systems, the `color`
         parameter is always allowed to be a subclass of :class:`~colorir.color_class.ColorBase` or
         a hex string with length == 6, but can only be a tuple if :attr:`ColorFormat.color_sys` is
         a tuple-based color system, such as :class:`~colorir.color_class.sRGB` for example.
 
         Examples:
             >>> rgb_format = ColorFormat(color_class.sRGB, round_to=0)
             >>> rgb_format.format("#ff0000")
-            sRGB(255, 0, 0)
-            >>> rgb_format.format((255, 0, 0))
-            sRGB(255, 0, 0)
+            RGB(1, 0, 0)
+            >>> rgb_format.format((1, 0, 0))
+            RGB(1, 0, 0)
             >>> hex_format = ColorFormat(color_class.Hex)
             >>> hex_format.format("#ff0000")
             Hex('#ff0000')
-            >>> hex_format.format((255, 0, 0)) # Can't understand how to parse this tuple
+            >>> hex_format.format((1, 0, 0)) # Can't understand how to parse this tuple
             Traceback (most recent call last):
               ...
-            ValueError: tried to interpret a tuple-formatted color object with a Hex ColorFormat
+            colorir.color_format.FormatError: tried to interpret a tuple-formatted color with a Hex-based ColorFormat
 
         Args:
             color: The value of the color to be formatted. Can be an instance of any
                 :mod:`~colorir.color_class` class or, alternatively, a color-like object that
                 resembles the format of the color you want to format.
         """
         if isinstance(color, color_class.ColorBase):
-            return self._from_rgba(color._rgba)
-        elif isinstance(color, str):
-            # Try to preserve input options (none implemented now but who knows)
+            with _wrap_format_error():
+                return self._from_rgba(color._rgba)
+        if isinstance(color, str):
+            # Try to preserve input options
             if self.color_sys == color_class.Hex:
-                return self.new_color(color)
+                with _wrap_format_error():
+                    return self.new_color(color)
             # No alpha in the string, safe to interpret with Hex
             if len(color) < 8:
                 # Fallback to Hex default args
-                return self._from_rgba(color_class.Hex(color)._rgba)
-            raise ValueError("tried to interpret a string-formatted color that contains an alpha"
-                             "component with a non-Hex ColorFormat")
-        if self.color_sys != color_class.Hex:
-            # Assume that the color system is tuple-based
-            return self.new_color(*color)
-        else:
-            raise ValueError("tried to interpret a tuple-formatted color object with a Hex "
-                             "ColorFormat")
+                with _wrap_format_error():
+                    return self._from_rgba(color_class.Hex(color)._rgba)
+            raise FormatError("tried to interpret a string-formatted color that contains an alpha"
+                              "component with a non-Hex ColorFormat")
+        if hasattr(color, "__iter__"):
+            if self.color_sys == color_class.Hex:
+                raise FormatError("tried to interpret a tuple-formatted color with a Hex-based ColorFormat")
+            with _wrap_format_error():
+                return self.new_color(*color)
+        raise FormatError()
+
+
+class FormatError(Exception):
+    def __init__(self, message="An error occurred when trying to format this color"):
+        super().__init__(message)
+
+
+class _wrap_format_error:
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if exc_type is not None:
+            raise FormatError()
 
 
-PYGAME_COLOR_FORMAT = ColorFormat(color_sys=color_class.sRGB, max_rgb=255, max_a=255, round_to=0)
+PYGAME_COLOR_FORMAT = ColorFormat(color_sys=color_class.RGB, max_rgb=255, max_a=255, round_to=0)
 """Color format compatible with PyGame standards."""
 
 KIVY_COLOR_FORMAT = ColorFormat(color_sys=color_class.sRGB,
                                 max_rgb=1,
                                 max_a=1,
                                 round_to=-1,
                                 include_a=True)
```

### Comparing `colorir-1.3.9/colorir/examples/color_picker.py` & `colorir-2.0.0/colorir/examples/color_picker.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,14 @@
         self.update_idletasks()
         self.canvas.configure(scrollregion=self.canvas.bbox('all'))
 
 
 class FramedButton(tk.Frame):
     def __init__(self, parent, width, height, *args, **kwargs):
         super().__init__(parent, width=width, height=height)
-        self.pack_propagate(0)
+        self.pack_propagate(False)
         self.button = tk.Button(self, *args, **kwargs)
         self.button.pack(fill=tk.BOTH, expand=1)
 
 
 win = Window()
 win.mainloop()
```

### Comparing `colorir-1.3.9/colorir/examples/color_wheel.py` & `colorir-2.0.0/colorir/examples/color_wheel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from kivy.config import Config
 Config.set('graphics', 'width', '400')
 Config.set('graphics', 'height', '400')
 from kivy.app import App
-from kivy.graphics import Ellipse, Color
+from kivy.graphics import Ellipse, Rectangle, Color
 from kivy.uix.widget import Widget
 from colorir import config, KIVY_COLOR_FORMAT, Grad, HSV
 
 # Define the default color format to work with kivy
 config.DEFAULT_COLOR_FORMAT = KIVY_COLOR_FORMAT
 
 # You can play around with these variables to change the appearance of the color wheel
@@ -16,14 +16,16 @@
 
 class WheelScreen(Widget):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         iter_angle = 360 / ELLIPSE_STEPS
         with self.canvas:
+            Rectangle(pos=(0, 0), size=(400, 400))  # Draw background
+
             for j in range(ELLIPSE_SEGMENTS + 1):
                 s = 1 - j / ELLIPSE_SEGMENTS
                 # Sample colors throughout the hue range for this saturation
                 outer_colors = Grad(
                     [HSV(0, s, 1), HSV(355, s, 1)],
                     color_sys=HSV
                 ).n_colors(ELLIPSE_STEPS)
```

### Comparing `colorir-1.3.9/colorir/palette.py` & `colorir-2.0.0/colorir/palette.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,76 +4,75 @@
 projects. In this context, a palette should be understood as any collection of colors that
 can be grouped due to a common feature, not only colors that necessarily "look good" together.
 
 Every color in a :class:`Palette` has a name associated with it. If unnamed colors are better fit
 to your particular use case, you may want to use a :class:`StackPalette` instead.
 
 Examples:
-    Create a palette with the color red:
+    Create a palette:
 
     >>> palette = Palette(red="#ff0000")
 
-    Add the color blue:
+    Add colors:
 
     >>> palette.add("blue", "#0000ff")
 
-    Get the value for red:
+    Get the value of colors:
 
     >>> palette.red
     Hex('#ff0000')
 
-    Get names of all colors:
-
-    >>> palette.color_names
-    ['red', 'blue']
-
-    Remove red:
+    Remove colors:
 
     >>> palette.remove("red")
     >>> "red" in palette.color_names
     False
 
-    Name the palette and save it to the default directory:
+    Save a palette:
 
-    >>> palette.name = "single_blue"
-    >>> palette.save()
+    >>> palette.save(name="single_blue")
 
-    Load it again from elsewhere later:
+    Load saved palettes:
 
     >>> palette = Palette.load("single_blue")
+
+    Concatenate two palettes together:
+
+    >>> Palette(red="f00", blue="00f") & Palette(green="0f0", yellow="0ff")
+    Palette(red=#ff0000, blue=#0000ff, green=#00ff00, yellow=#00ffff)
 """
 import abc
 import json
 import os
+import numpy as np
 from pathlib import Path
-from typing import Union, List
+from typing import Union, List, Dict, Iterable
 from warnings import warn
-
 from . import config
 from . import utils
-from .color_class import ColorBase, sRGB, HSL, HSV
-from .color_format import ColorFormat, ColorLike
+from .color_class import ColorBase, RGB, HSL, HSV, ColorLike
+from .color_format import ColorFormat
+from .gradient import Grad
 
 _throw_exception = object()
 _builtin_palettes_dir = Path(__file__).resolve().parent / "builtin_palettes"
 
 __all__ = [
     "Palette",
     "StackPalette",
     "find_palettes",
     "delete_palette"
 ]
 
 
 class PaletteBase(metaclass=abc.ABCMeta):
-    def __init__(self, name=None, color_format=None):
+    def __init__(self, color_format=None):
         if color_format is None:
             color_format = config.DEFAULT_COLOR_FORMAT
 
-        self.name = name
         self._color_format = color_format
 
     @property
     @abc.abstractmethod
     def colors(self):
         """A list of all color values currently stored in the palette."""
         pass
@@ -85,66 +84,25 @@
 
     @color_format.setter
     @abc.abstractmethod
     def color_format(self, color_format):
         self._color_format = color_format
 
     def __len__(self):
+        """Returns the number of colors in the palette."""
         return len(self.colors)
 
     def __contains__(self, item):
+        """Returns ```True`` if the color is found in the palette and ``False`` otherwise."""
         return self.color_format.format(item) in self.colors
 
     def __iter__(self):
+        """Iterates over the colors in the palette."""
         return iter(self.colors)
 
-    def most_similar(self, color: ColorLike, n=1, method="CIE76"):
-        """Finds the `n` most similar colors to `color` in this palette.
-
-        Args:
-            color: The value of the color of reference. Can be an instance of any
-                :mod:`~colorir.color_class` class or, alternatively, a color-like object that
-                resembles the color to which others will be compared in search of similar results.
-            n: How many similar colors to be retrieved. -1 means all colors from the palette will
-                be returned from most similar to least.
-            method: Method for calculating color distance. See the documentation of
-                :func:`~colorir.utils.color_dist()`.
-
-        Examples:
-            >>> palette = Palette(red="#ff0000", blue="#0000ff")
-            >>> palette.most_similar("#880000")
-            Hex('#ff0000')
-
-        Returns:
-            A single :class:`~colorir.color_class.ColorBase` if `n` == 1 or a list of
-            :class:`~colorir.color_class.ColorBase` if `n` != 1. If the return type is a list, the
-            colors will be ordered from most similar to least.
-        """
-        color = self.color_format.format(color)
-        closest = sorted(self.colors,
-                         key=lambda color2: utils.color_dist(color, color2, method=method))
-        if n == 1:
-            return closest[0]
-        elif n < 0:
-            n = len(self)
-        return closest[:n]
-
-    def to_cmap(self, N: int = None):
-        """Converts this palette into a matplotlib ListedColormap.
-
-        Args:
-            N: Passed down to ListedColormap constructor.
-        """
-        from matplotlib.colors import ListedColormap
-
-        colors = [color.hex(include_a=True, tail_a=True) for color in self.colors]
-        if self.name is None:
-            return ListedColormap(colors, N=N)
-        return ListedColormap(colors, N=N, name=self.name)
-
 
 class Palette(PaletteBase):
     """Class that holds colors values associated with names.
 
     Examples:
         >>> palette = Palette(red="#ff0000") # Uses default color format
         >>> palette.red
@@ -156,18 +114,25 @@
         name: Name of the palette which will be used to save it with :meth:`Palette.save()`.
         color_format: Color format specifying how the colors of this :class:`Palette` should be
             stored. Defaults to the value specified in
             :const:`config.DEFAULT_COLOR_FORMAT <colorir.config.DEFAULT_COLOR_FORMAT>`.
         colors: Colors that will be stored in this palette.
     """
     def __init__(self,
-                 name: str = None,
+                 colors: Union["Palette", Dict[str, ColorLike]] = None,
                  color_format: ColorFormat = None,
-                 **colors: ColorLike):
-        super().__init__(name, color_format)
+                 **color_kwargs: ColorLike):
+        super().__init__(color_format)
+        if colors is None:
+            colors = color_kwargs
+        elif color_kwargs:
+            raise ValueError("colors can be passed either through the 'colors' parameter or through kwargs "
+                             "but not both")
+        if isinstance(colors, Palette):
+            colors = colors.to_dict()
 
         self._color_dict = {}
         for k, v in colors.items():
             self.add(k, v)
 
     @property
     def colors(self) -> List[ColorBase]:
@@ -189,111 +154,162 @@
                             for c_name, c_value in self._color_dict.items()}
 
     @classmethod
     def load(cls,
              palettes: Union[str, List[str]] = None,
              palettes_dir: str = None,
              search_builtins=True,
-             name: str = None,
+             search_cwd=True,
              color_format: ColorFormat = None,
-             warnings=True):
+             warnings=True) -> "Palette":
         """Factory method that loads previously created palettes into a :class:`Palette` instance.
 
         A palette is a file containing json-formatted information about colors that ends with the
         '.palette' extension. You should not create such files manually but rather through the
         :meth:`Palette.save()` method.
 
         If multiple palettes define different color values under the same name, only the first one
         will be kept. You can define the order in which the palettes are loaded by ordering them in
         the `palettes` parameter. By default this occurrence logs a warning, but this behaviour can
         be changed through the `warnings` parameter.
 
         Args:
             palettes: List of palettes located in the location represented by `palettes_dir` that
                 should be loaded by this :class:`Palette` instance. Additionally may include
-                built-in palettes such as 'css' if `search_builtins` is set to ``True``. If this
-                parameter is a string, the :attr:`Palette.name` will be inferred from it. By
+                built-in palettes such as 'css' if `search_builtins` is set to ``True``. By
                 default, loads all palettes found in the specified directory.
             palettes_dir: The directory from which the palettes specified in the `palettes`
                 parameter will be loaded. Defaults to the value specified in
                 :data:`config.DEFAULT_PALETTES_DIR <colorir.config.DEFAULT_PALETTES_DIR>`.
-            search_builtins: Whether `palettes` also includes built-in palettes such as 'css' or
-                'basic'. Set to ``False`` to ensure only palette files found in `palettes_dir` are
-                loaded.
-            name: Name of the palette which will be used to save it with the
-                :meth:`Palette.save()`. If the `palettes` parameter is a single string, defaults
-                to that.
+            search_builtins: Whether `palettes` may also include built-in palettes such as 'css'
+                or 'basic'.
+            search_cwd: Whether `palettes` may also include palettes located in the current
+                working directory.
             color_format: Color format specifying how the colors of this :class:`Palette` should be
                 stored. Defaults to the value specified in
                 :data:`config.DEFAULT_COLOR_FORMAT <colorir.config.DEFAULT_COLOR_FORMAT>`.
             warnings: Whether to emit a warning if two colors with the same name but different
                 color values were found in the `palettes`.
 
         Examples:
             Loads the default CSS palette:
 
             >>> css_palette = Palette.load('css')
 
-            Loads both the basic and fluorescent palettes into a new palette called 'colorful':
+            Loads both the basic and fluorescent palettes into a new palette:
 
-            >>> colorful = Palette.load(['basic', 'fluorescent'], name='colorful')
+            >>> colorful = Palette.load(['basic', 'fluorescent'])
         """
         if palettes_dir is None:
             palettes_dir = config.DEFAULT_PALETTES_DIR
         palettes_dir = [palettes_dir]
         if search_builtins:
             palettes_dir.append(_builtin_palettes_dir)
+        if search_cwd:
+            palettes_dir.append(os.getcwd())
         if isinstance(palettes, str):
-            if name is None:
-                name = palettes
             palettes = [palettes]
 
         found_palettes = {}
         for path in palettes_dir:
             path = Path(path)
             palette_files = path.glob("*.palette")
             for palette_file in palette_files:
                 palette_name = palette_file.name.replace(".palette", '')
                 found_palettes[palette_name] = json.loads(palette_file.read_text())
 
-        palette_obj = cls(name=name, color_format=color_format)
-        if palettes is None: palettes = list(found_palettes)
+        palette_obj = cls(color_format=color_format)
+        if palettes is None:
+            palettes = list(found_palettes)
         # Reiterates based on user input order
         for palette_name in palettes:
             for c_name, c_rgba in found_palettes[palette_name].items():
-                c_rgba = (int(c_rgba[3:5], 16),
-                          int(c_rgba[5:7], 16),
-                          int(c_rgba[7:9], 16),
-                          int(c_rgba[1:3], 16))
+                c_rgba = np.array([int(c_rgba[3:5], 16),
+                                   int(c_rgba[5:7], 16),
+                                   int(c_rgba[7:9], 16),
+                                   int(c_rgba[1:3], 16)])
                 new_color = palette_obj.color_format._from_rgba(c_rgba)
-                old_color = palette_obj.get_color(c_name, new_color)
-                if new_color != old_color and warnings:
+                old_color = palette_obj.get_color(c_name, None)
+                if old_color is None:
+                    palette_obj.add(c_name, new_color)
+                elif new_color != old_color and warnings:
                     warn(
                         f"a discrepancy was detected when adding color '{c_name}' "
                         f"({new_color}) from palette named '{palette_name}': '{c_name}' is "
                         f"already present with a different value ({old_color})")
-                else:
-                    palette_obj.add(c_name, new_color)
         return palette_obj
 
     def __getattr__(self, item):
-        return self._color_dict[item]
+        return self.get_color(item)
+
+    def __getitem__(self, item):
+        if isinstance(item, str):
+            return self.get_color(item)
+        elif isinstance(item, list):
+            pal = Palette(color_format=self.color_format)
+            pal._color_dict = {c_name: self._color_dict[c_name] for c_name in item}
+            return pal
+        raise TypeError(f"'Palette' indices must be 'str' or 'list', not '{type(item)}'")
+
+    def __setitem__(self, key, value):
+        if not isinstance(key, str):
+            raise TypeError("key must be a string")
+        if key in self._color_dict:
+            self.update(key, value)
+            return
+        self.add(key, value)
+
+    def __delitem__(self, key):
+        self.remove(key)
+
+    def __dir__(self) -> List[str]:
+        return dir(Palette) + list(self.__dict__) + list(self._color_dict.keys())
+
+    def __str__(self):
+        colors_str = ', '.join(
+            f"{c_name}={str(c_val)}" for c_name, c_val in self._color_dict.items()
+        )
+        return f"{self.__class__.__name__}({colors_str})"
 
     def __repr__(self):
-        name_str = self.name + ", " if self.name else ""
-        color_strs = [f"{c_name}={c_val.__repr__()}" for c_name, c_val in self._color_dict.items()]
-        return f"{self.__class__.__name__}({name_str}{', '.join(color_strs)})"
+        if config.REPR_STYLE in ["traditional", "inherit"]:
+            return str(self)
+        return utils.swatch(self, file=None)
 
     def __eq__(self, other):
         return self._color_dict.items() == other._color_dict.items()
 
-    def __add__(self, other):
-        for c_name in other.color_names:
-            self.add(c_name, other.get_color(c_name))
-        return self
+    def __and__(self, other):
+        """Join two palettes sequentially.
+
+        Repeated color names wil raise an exception.
+
+        Examples:
+
+            >>> Palette(red="ff0000") & Palette(blue="0000ff")
+            Palette(red=#ff0000, blue=#0000ff)
+        """
+        pal = Palette(self, color_format=self.color_format)
+        for c_name, c_val in other.to_dict().items():
+            pal.add(c_name, c_val)
+        return pal
+
+    def __invert__(self):
+        """Returns a copy of this object but with its colors inverted in RGB space.
+
+        Examples:
+
+            >>> palette = Palette(red="ff0000", yellow="ffff00")
+            >>> ~palette
+            Palette(red=#00ffff, yellow=#0000ff)
+        """
+        pal = Palette(color_format=self.color_format)
+        for c_name, c_val in self.to_dict().items():
+            pal.add(c_name, ~c_val)
+        return pal
 
     def get_color(self,
                   name: Union[str, List[str]],
                   fallback=_throw_exception) -> Union[ColorBase, List[ColorBase]]:
         """Retrieves one or more colors from the :class:`Palette` given their names.
 
         Args:
@@ -401,204 +417,234 @@
     def remove(self, name):
         """Removes a color from the palette.
 
         Args:
             name: Name of the color to be removed.
 
         Examples:
-            >>> palette = Palette(red=sRGB(255, 0, 0))
+            >>> palette = Palette(red=RGB(1, 0, 0))
             >>> palette.remove("red")
             >>> "red" in palette.color_names
             False
         """
         if name in self._color_dict:
             del self._color_dict[name]
         else:
             raise ValueError(f"provided 'name' parameter is not a color stored in this 'Palette'")
 
-    def save(self, palettes_dir: str = None):
+    def save(self, name: str, palettes_dir: str = None):
         """Saves the changes made to this :class:`Palette` instance.
 
         If this method is not called after modifications made by :meth:`Palette.add()`,
         :meth:`Palette.update()` and :meth:`Palette.remove()`, the modifications on the palette
         will not be permanent.
 
         Examples:
             Loads both the basic and fluorescent palettes into a new palette called 'colorful':
 
-            >>> colorful = Palette.load(['basic', 'fluorescent'], name='colorful')
+            >>> colorful = Palette.load(['basic', 'fluorescent'])
 
             Save the palette to the default palette directory:
 
-            >>> colorful.save()
+            >>> colorful.save(name='colorful')
         """
-        if self.name is None:
-            raise AttributeError(
-                "the 'name' attribute of a 'Palette' instance must be defined to save it")
         if palettes_dir is None:
             palettes_dir = config.DEFAULT_PALETTES_DIR
-        with open(Path(palettes_dir) / (self.name + ".palette"), "w") as file:
+        with open(Path(palettes_dir) / (name + ".palette"), "w") as file:
             formatted_colors = {}
             for c_name, c_val in self._color_dict.items():
                 c_rgba = c_val.hex(include_a=True, tail_a=False)
                 formatted_colors[c_name] = c_rgba
             json.dump(formatted_colors, file, indent=4)
 
     def to_stackpalette(self) -> "StackPalette":
         """Converts this palette into a :class:`StackPalette`."""
-        return StackPalette(self.name, self.color_format, *self._color_dict.values())
+        return StackPalette(colors=self._color_dict.values(), color_format=self.color_format)
 
     def to_dict(self):
         """Converts this palette into a python `dict`."""
         return dict(self._color_dict)
 
+    def grayscale(self):
+        """Returns a copy of this object but with its colors in grayscale.
+
+        Examples:
+
+            >>> palette = Palette(red="ff0000", yellow="ffff00")
+            >>> palette.grayscale()
+            Palette(red=#7f7f7f, yellow=#f7f7f7)
+        """
+        pal = Palette(color_format=self.color_format)
+        for c_name, c_val in self.to_dict().items():
+            pal.add(c_name, c_val.grayscale())
+        return pal
+
+    def most_similar(self, color: ColorLike, n=1, method="CIE76"):
+        """Finds the `n` most similar colors to `color` in this palette.
+
+        Args:
+            color: The value of the color of reference.
+            n: How many colors to be retrieved from most similar to least. -1 means all colors will be returned.
+            method: Method for calculating color distance. See the documentation of the function `color_dist`.
+
+        Examples:
+            >>> palette = Palette(red="#ff0000", blue="#0000ff")
+            >>> palette.most_similar("#880000")
+            ('red', Hex('#ff0000'))
+
+        Returns:
+            A tuple (color_name, color) if `n` == 1 or a `Palette` if `n` != 1.
+        """
+        closest = sorted(zip(self.color_names, self.colors),
+                         key=lambda tup: utils.color_dist(color, tup[1], method))
+        if n == 1:
+            return closest[0]
+        if n < 1:
+            n = len(self)
+        pal = Palette(color_format=self.color_format)
+        pal._color_dict = dict(closest[:n])
+        return pal
+
 
 class StackPalette(PaletteBase):
     """Class that handles anonymous indexed colors stored as a stack.
 
     This class may be used as a replacement for :class:`Palette` when the name of the colors is
     irrelevant.
 
     Examples:
-        >>> spalette = StackPalette("elementary", None, "ff0000", "00ff00", "0000ff")
+        >>> spalette = StackPalette(["ff0000", "00ff00", "0000ff"])
         >>> spalette[0]
         Hex('#ff0000')
 
     Args:
-        name: Name of the palette which will be used to save it with
-            :meth:`StackPalette.save()`.
         color_format: Color format specifying how the colors of this :class:`StackPalette` should
             be stored. Defaults to the value specified in
             :data:`config.DEFAULT_COLOR_FORMAT <colorir.config.DEFAULT_COLOR_FORMAT>`.
         colors: Colors that will be stored in this palette.
     """
 
     def __init__(self,
-                 name: str = None,
-                 color_format: ColorFormat = None,
-                 *colors: ColorLike):
-        super().__init__(name=name, color_format=color_format)
+                 colors: Iterable[ColorLike] = None,
+                 color_format: ColorFormat = None):
+        super().__init__(color_format=color_format)
+        if colors is None:
+            colors = []
 
         self._color_stack = []
         for color in colors:
             self.add(color)
 
     @property
     def colors(self) -> List[ColorBase]:
         """colors: A list of all color values currently stored in the :class:`StackPalette`."""
         return list(self._color_stack)
 
     @PaletteBase.color_format.setter
     def color_format(self, color_format):
         PaletteBase.color_format.fset(self, color_format)
-
         self._color_stack = [color_format._from_rgba(color._rgba) for color in self._color_stack]
 
     @classmethod
     def load(cls,
              palettes: Union[str, List[str]] = None,
              palettes_dir: str = None,
              search_builtins=True,
-             name: str = None,
-             color_format: ColorFormat = None):
+             search_cwd=True,
+             color_format: ColorFormat = None) -> "StackPalette":
         """Factory method that loads previously created stack palettes into a
         :class:`StackPalette` instance.
 
         A stack palette is a file containing json-formatted information about colors that ends
         with the '.spalette' extension. You should not create such files manually but rather
         through the :meth:`StackPalette.save()` method.
 
         Examples:
             Load a stack palette called "project_interface" from the default directory:
 
             >>> spalette = StackPalette.load("project_interface")  # doctest: +SKIP
 
         Args:
             palettes: List of stack palettes located in the location represented by `palettes_dir`
-                that should be loaded by this :class:`StackPalette` instance. If this parameter is
-                a string, the :attr:`StackPalette.name` will be inferred from it. By default,
+                that should be loaded by this :class:`StackPalette` instance. By default,
                 loads all palettes found in the specified directory.
             palettes_dir: The directory from which the palettes specified in the `palettes`
                 parameter will be loaded. Defaults to the value specified in
                 :data:`config.DEFAULT_PALETTES_DIR <colorir.config.DEFAULT_PALETTES_DIR>`.
-            search_builtins: Whether `palettes` also includes built-in palettes such as 'tab10' or
-                'dark2'. Set to ``False`` to ensure only palette files found in `palettes_dir` are
-                loaded.
-            name: Name of the palette which will be used to save it with the
-                :meth:`StackPalette.save()`. If the `palettes` parameter is a single string,
-                defaults to that.
+            search_builtins: Whether `palettes` may also include built-in palettes such as 'tab10'
+                or 'dark2'.
+            search_cwd: Whether `palettes` may also include palettes located in the current
+                working directory.
             color_format: Color format specifying how the colors of this :class:`Palette` should be
                 stored. Defaults to the value specified in
                 :data:`config.DEFAULT_COLOR_FORMAT <colorir.config.DEFAULT_COLOR_FORMAT>`.
         """
         if palettes_dir is None:
             palettes_dir = config.DEFAULT_PALETTES_DIR
         palettes_dir = [palettes_dir]
         if search_builtins:
             palettes_dir.append(_builtin_palettes_dir)
+        if search_cwd:
+            palettes_dir.append(os.getcwd())
         if isinstance(palettes, str):
-            if name is None:
-                name = palettes
             palettes = [palettes]
 
         found_palettes = {}
         for path in palettes_dir:
             path = Path(path)
             palette_files = path.glob("*.spalette")
             for palette_file in palette_files:
                 palette_name = palette_file.name.replace(".spalette", '')
                 found_palettes[palette_name] = json.loads(palette_file.read_text())
 
-        palette_obj = cls(name=name, color_format=color_format)
-        if palettes is None: palettes = list(found_palettes)
+        palette_obj = cls(color_format=color_format)
+        if palettes is None:
+            palettes = list(found_palettes)
         # Reiterates based on user input order
         for palette_name in palettes:
             for c_rgba in found_palettes[palette_name]:
-                c_rgba = (int(c_rgba[3:5], 16),
-                          int(c_rgba[5:7], 16),
-                          int(c_rgba[7:9], 16),
-                          int(c_rgba[1:3], 16))
+                c_rgba = np.array([int(c_rgba[3:5], 16),
+                                   int(c_rgba[5:7], 16),
+                                   int(c_rgba[7:9], 16),
+                                   int(c_rgba[1:3], 16)])
                 new_color = palette_obj.color_format._from_rgba(c_rgba)
                 palette_obj.add(new_color)
         return palette_obj
 
     # TODO enhance to allow different color systems and variance param (prob. 1.4.0)
     @classmethod
     def new_complementary(cls,
                           n: int,
                           color: ColorLike = None,
-                          name: str = None,
                           color_format: ColorFormat = None):
         """Creates a new palette with `n` complementary colors.
 
         Colors are considered complementary if they are interspaced in the additive HUE color
         wheel.
 
         Examples:
              Make a palette from red and its complementary color, cyan:
 
-             >>> spalette = StackPalette.new_complementary(2, sRGB(255, 0, 0))
+             >>> spalette = StackPalette.new_complementary(2, RGB(1, 0, 0))
              >>> spalette
-             StackPalette(Hex('#ff0000'), Hex('#00ffff'))
+             StackPalette([#ff0000, #00ffff])
 
              Make a tetradic palette of random colors:
 
              >>> spalette = StackPalette.new_complementary(4)
 
         Args:
             n: The number of colors in the new palette.
             color: A color from which the others will be generated against. By default, a color is
                 randomly chosen.
-            name: Name of the palette which will be used to save it with
-                :meth:`StackPalette.save()`.
             color_format: Color format specifying how the colors of this :class:`StackPalette`
                 should be stored. Defaults to the value specified in
                 :data:`config.DEFAULT_COLOR_FORMAT <colorir.config.DEFAULT_COLOR_FORMAT>`.
         """
-        n_spalette = cls(name=name, color_format=color_format)
+        n_spalette = cls(color_format=color_format)
         if color is None:
             hsv = utils.random_color(color_format=ColorFormat(HSV, max_h=360))
         else:
             hsv = n_spalette.color_format.format(color).hsv(max_h=360)
 
         step = 360 / n
         for i in range(n):
@@ -608,26 +654,25 @@
 
     @classmethod
     def new_analogous(cls,
                       n: int,
                       sections=12,
                       start=0,
                       color: ColorLike = None,
-                      name: str = None,
                       color_format: ColorFormat = None):
         """Creates a new palette with `n` analogous colors.
 
         Colors are considered analogous if they are side-by-side in the additive HUE color wheel.
 
         Examples:
              Make a palette from red and its analogous color, orange:
 
-             >>> spalette = StackPalette.new_analogous(2, start=1, color=sRGB(255, 0, 0))
+             >>> spalette = StackPalette.new_analogous(2, start=1, color=RGB(1, 0, 0))
              >>> spalette
-             StackPalette(Hex('#ff0000'), Hex('#ff8000'))
+             StackPalette([#ff0000, #ff8000])
 
              Make a palette of four similar colors:
 
              >>> spalette = StackPalette.new_analogous(4, sections=24)
 
         Args:
             n: The number of colors in the new palette.
@@ -636,16 +681,14 @@
                 be.
             start: Where the color described in the 'color' parameter will be placed with respect
                 to the others. If '0', 'color' will be in the center of the generated palette, and
                 colors will be sampled from both its sides in the HUE wheel. If '1', colors will
                 be sampled clockwise from 'color'. If '-1', they will be sampled counter-clockwise.
             color: A color from which the others will be generated against. By default, a color is
                 randomly chosen.
-            name: Name of the palette which will be used to save it with
-                :meth:`StackPalette.save()`.
             color_format: Color format specifying how the colors of this :class:`StackPalette`
                 should be stored. Defaults to the value specified in
                 :data:`config.DEFAULT_COLOR_FORMAT <colorir.config.DEFAULT_COLOR_FORMAT>`.
         """
         if n > sections:
             raise ValueError("'n' parameter cannot be larger than 'sections' parameter")
         if start == 0:
@@ -654,62 +697,113 @@
         elif start == 1:
             iterator = range(n)
         elif start == -1:
             iterator = range(-n + 1, 1)
         else:
             raise ValueError("'starting_point' must be either 0, 1 or -1")
 
-        n_spalette = cls(name=name, color_format=color_format)
+        n_spalette = cls(color_format=color_format)
         if color is None:
             hsv = utils.random_color(color_format=ColorFormat(HSV, max_h=360))
         else:
             hsv = n_spalette.color_format.format(color).hsv(max_h=360)
 
         step = 360 / sections
         for index, i in enumerate(iterator):
             hue = (hsv[0] + i * step) % 360
             n_spalette.add(HSV(hue, hsv[1], hsv[2]))
         return n_spalette
 
-    def __getitem__(self, item: int):
-        return self._color_stack[item]
+    def __getitem__(self, item):
+        if isinstance(item, int):
+            return self._color_stack[item]
+        if isinstance(item, list):
+            pal = StackPalette(color_format=self.color_format)
+            pal._color_stack = [self._color_stack[i] for i in item]
+            return pal
+        if isinstance(item, slice):
+            indexes = list(range(*item.indices(len(self))))
+            return self[indexes]
+        raise TypeError(f"'StackPalette' indices must be 'int', 'list' or 'slice', not '{type(item)}'")
+
+    def __setitem__(self, key, value):
+        if isinstance(key, int):
+            self.update(key, value)
+        elif isinstance(key, list):
+            if len(key) != len(value):
+                raise ValueError("length of indexes and provided values must match")
+            for i, val in zip(key, value):
+                self.update(i, val)
+        elif isinstance(key, slice):
+            indexes = list(range(*key.indices(len(self))))
+            self[indexes] = value
+        else:
+            raise TypeError("index must be 'int', 'list' or 'slice'")
+
+    def __str__(self):
+        colors_str = ', '.join(str(c_val) for c_val in self._color_stack)
+        return f"{self.__class__.__name__}([{colors_str}])"
 
     def __repr__(self):
-        name_str = self.name + ", " if self.name else ""
-        return f"{self.__class__.__name__}({name_str}" \
-               f"{', '.join(c_val.__repr__() for c_val in self._color_stack)})"
+        if config.REPR_STYLE in ["traditional", "inherit"]:
+            return str(self)
+        return utils.swatch(self, file=None)
 
     def __eq__(self, other):
         return self._color_stack == other._color_stack
 
-    def __add__(self, other):
-        for color in other:
-            self.add(color)
-        return self
+    def __and__(self, other):
+        """Join two palettes sequentially.
 
-    def swap(self, index1: int, index2: int):
-        """Swap the places of two colors in the palette.
+        Examples:
 
-        Can be used to reorganize the palette if needed.
+            >>> StackPalette(["ff0000"]) & StackPalette(["0000ff"])
+            StackPalette([#ff0000, #0000ff])
+        """
+        c_list = self.colors + other.colors
+        return StackPalette(c_list, color_format=self.color_format)
+
+    def __invert__(self):
+        """Returns a copy of this object but with its colors inverted in RGB space.
 
         Examples:
-            >>> spalette = StackPalette(None, None, "ff0000", "0000ff")
-            >>> spalette
-            StackPalette(Hex('#ff0000'), Hex('#0000ff'))
-            >>> spalette.swap(0, 1)
-            >>> spalette
-            StackPalette(Hex('#0000ff'), Hex('#ff0000'))
+
+            >>> spalette = StackPalette(["ff0000", "ffff00"])
+            >>> ~spalette
+            StackPalette([#00ffff, #0000ff])
+        """
+        pal = StackPalette(color_format=self.color_format)
+        for color in self.colors:
+            pal.add(~color)
+        return pal
+
+    def resize(self, n: int, repeat=False, grad_class=Grad, **kwargs):
+        """Resizes the palette to be `n` elements long by interpolating or repeating colors.
 
         Args:
-            index1: The index of the first color.
-            index2: The index of the second color.
+            repeat: If ``True``, repeats the colors intead of interpolating them to reach the length goal.
+            grad_class: Which gradient class to use for interpolation.
+            n: Number of elements in the final palette.
+            kwargs: Key-word arguments passed down to the internal gradient object.
+
+        Examples:
+
+            >>> StackPalette(["000000", "ffffff"]).resize(3)
+            StackPalette([#000000, #777777, #ffffff])
+            >>> StackPalette(["000000", "ffffff"]).resize(3, repeat=True)
+            StackPalette([#000000, #ffffff, #000000])
+
+        Returns:
+            A resized copy of this stack palette.
         """
-        c_temp = self._color_stack[index1]
-        self._color_stack[index1] = self._color_stack[index2]
-        self._color_stack[index2] = c_temp
+        if repeat:
+            color_indices = [i % len(self) for i in range(n)]
+            return self[color_indices]
+        colors = grad_class(colors=self.colors, **kwargs).n_colors(n)
+        return StackPalette(colors=colors, color_format=self.color_format)
 
     def add(self, color: ColorLike):
         """Adds a color to the end of the stack palette.
 
         Colors can only be added to the last index of the stack palette, just like in a normal
         stack.
 
@@ -736,15 +830,15 @@
             color: The value of the color to be updated. Can be an instance of any
                 :mod:`~colorir.color_class` class or, alternatively, a color-like object that
                 resembles the format of the color you want to update.
 
         Examples:
             Create a slightly dark shade of red:
 
-            >>> spalette = StackPalette(None, None, "dd0000")
+            >>> spalette = StackPalette(["dd0000"])
             >>> spalette[0]
             Hex('#dd0000')
 
             Change it to be even a bit darker:
 
             >>> spalette.update(0, "800000")
             >>> spalette[0]
@@ -755,43 +849,39 @@
     def remove(self):
         """Removes a color from the end of the palette.
 
         Colors can only be removed from the last index of the stack palette, just like in a normal
         stack.
 
         Examples:
-            >>> spalette = StackPalette(None, None, "#ff0000")
+            >>> spalette = StackPalette(["#ff0000"])
             >>> "#ff0000" in spalette
             True
             >>> spalette.remove()
             >>> "#ff0000" in spalette
             False
         """
         self._color_stack.pop()
 
-    def save(self, palettes_dir: str = None):
+    def save(self, name: str, palettes_dir: str = None):
         """Saves the changes made to this :class:`StackPalette` instance.
 
         If this method is not called after modifications made by :meth:`StackPalette.add()`,
         :meth:`StackPalette.update()` and :meth:`StackPalette.remove()`, the modifications on the
         palette will not be permanent.
 
         Examples:
             Create a new :class:`StackPalette` and save it to the current directory:
 
-            >>> spalette = StackPalette("elementary", None, "ff0000", "00ff00", "0000ff")
-            >>> spalette.save()
+            >>> spalette = StackPalette(["ff0000", "00ff00", "0000ff"])
+            >>> spalette.save(name="elementary")
         """
-        if self.name is None:
-            raise AttributeError(
-                "the 'name' attribute of a 'StackPalette' instance must be defined to save it"
-            )
         if palettes_dir is None:
             palettes_dir = config.DEFAULT_PALETTES_DIR
-        with open(Path(palettes_dir) / (self.name + ".spalette"), "w") as file:
+        with open(Path(palettes_dir) / (name + ".spalette"), "w") as file:
             formatted_colors = []
             for c_val in self._color_stack:
                 c_rgba = tuple(spec for spec in c_val._rgba)
                 c_rgba = "#%02x" % c_rgba[-1] + "%02x%02x%02x" % c_rgba[:3]
                 formatted_colors.append(c_rgba)
             json.dump(formatted_colors, file, indent=4)
 
@@ -799,39 +889,84 @@
         """Converts this stack palette into a :class:`Palette`.
 
         Args:
             names: Names that will be given to the colors in the same order they appear in this
                 stack palette.
         """
         if len(names) == len(set(names)) == len(self._color_stack):
-            return Palette(self.name, self.color_format, **dict(zip(names, self._color_stack)))
+            return Palette(dict(zip(names, self._color_stack)), color_format=self.color_format)
         raise ValueError("'names' must have the same length as this 'StackPalette' and no "
                          "duplicates")
 
+    def grayscale(self):
+        """Returns a copy of this object but with its colors in grayscale.
+
+        Examples:
+
+            >>> spalette = StackPalette(["ff0000", "ffff00"])
+            >>> spalette.grayscale()
+            StackPalette([#7f7f7f, #f7f7f7])
+        """
+        pal = StackPalette(color_format=self.color_format)
+        for color in self.colors:
+            pal.add(color.grayscale())
+        return pal
+
+    def most_similar(self, color: ColorLike, n=1, method="CIE76"):
+        """Finds the `n` most similar colors to `color` in this palette.
+
+        Args:
+            color: The value of the color of reference.
+            n: How many colors to be retrieved from most similar to least. -1 means all colors will be returned.
+            method: Method for calculating color distance. See the documentation of `color_dist`.
+
+        Examples:
+            >>> palette = StackPalette(["#ff0000", "#0000ff"])
+            >>> palette.most_similar("#880000")
+            Hex('#ff0000')
+
+        Returns:
+            A single color object if `n` == 1 or a `StackPalette` if `n` != 1.
+        """
+        color = self.color_format.format(color)
+        closest = sorted(self.colors,
+                         key=lambda color2: utils.color_dist(color, color2, method=method))
+        if n == 1:
+            return closest[0]
+        pal = StackPalette(color_format=self.color_format)
+        pal._color_stack = closest
+        if n < 0:
+            return pal
+        return pal[:n]
+
 
 def find_palettes(palettes_dir: str = None,
                   search_builtins=True,
+                  search_cwd=True,
                   kind=(Palette, StackPalette)) -> List[str]:
     """Returns the names of the palettes found in `directory`.
 
     Args:
         palettes_dir: The directory from which the palettes will be searched for. Defaults to the
             value specified in
             :data:`config.DEFAULT_PALETTES_DIR <colorir.config.DEFAULT_PALETTES_DIR>`.
         search_builtins: Whether to also include built-in palettes such as 'css' or
             'basic' in the search.
+        search_cwd: Whether to also search palettes in the current working directory.
         kind: The kinds of palettes to include in the search. Can be either :class:`Palette`,
             :class:`StackPalette`, or a list of any of those.
     """
     if palettes_dir is None:
         palettes_dir = config.DEFAULT_PALETTES_DIR
     if isinstance(palettes_dir, str):
         palettes_dir = [palettes_dir]
     if search_builtins:
         palettes_dir.append(_builtin_palettes_dir)
+    if search_cwd:
+        palettes_dir.append(os.getcwd())
     globs = []
     if not isinstance(kind, (tuple, list)):
         kind = [kind]
     if Palette in kind:
         globs.append("*.palette")
     if StackPalette in kind:
         globs.append("*.spalette")
@@ -863,8 +998,8 @@
     path = Path(palettes_dir)
     palettes = list(path.glob(f"{palette}.*"))
     if len(palettes) == 1:
         os.remove(path / palettes[0])
     elif len(palettes) == 0:
         raise ValueError(f"couldn't find palette '{palette}' in '{palettes_dir}'")
     else:
-        raise ValueError(f"palette name '{palette}' is ambiguous (more than one palette share it)")
+        raise ValueError(f"palette name '{palette}' is ambiguous (more than one palette share it)")
```

### Comparing `colorir-1.3.9/colorir/utils.py` & `colorir-2.0.0/colorir/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,246 @@
 import os
+import sys
+import numpy as np
 from math import sqrt
 from random import randint
-from typing import Union, List
+from typing import List, Iterable, get_args
 from colormath.color_conversions import convert_color
 from colormath.color_diff import *
 from colormath.color_objects import sRGBColor, LabColor
 
 from . import config
 from . import palette
-from .color_class import ColorBase, HCLab
-from .color_format import ColorLike, ColorFormat
+from .color_class import ColorBase, HCLab, ColorLike
+from .color_format import ColorFormat
 from .gradient import Grad
 
+# Patch asscalar
+np.asscalar = lambda a: a.item()
+
 __all__ = [
     "swatch",
+    "show",
     "simplified_dist",
     "color_dist",
     "random_color",
     "color_str",
-    "hue_sort_key"
+    "hue_sort_key",
+    "hue_sorted",
+    "grayscale",
+    "inverse",
+    "blend"
 ]
 
 
-def swatch(obj: Union[ColorLike, List[ColorLike], "palette.Palette", "palette.StackPalette"],
+def blend(color1, color2, perc=0.5, grad_class=Grad, **kwargs):
+    return grad_class([color1, color2], **kwargs).perc(perc)
+
+
+def grayscale(obj):
+    """Returns a grayscale representation of a colorir object"""
+    if isinstance(obj, list):
+        return [color.grayscale() for color in obj]
+    # Assume single colorlike
+    elif isinstance(obj, get_args(ColorLike)):
+        obj = config.DEFAULT_COLOR_FORMAT.format(obj)
+    return obj.grayscale()
+
+
+def inverse(obj):
+    """Returns an RGB-inverted representation of a colorir object"""
+    if isinstance(obj, list):
+        return [~color for color in obj]
+    # Assume single colorlike
+    elif isinstance(obj, get_args(ColorLike)):
+        obj = config.DEFAULT_COLOR_FORMAT.format(obj)
+    return ~obj
+
+
+def swatch(obj,
            colored_text=True,
            width=3,
            height=1,
-           tabular=True):
-    """Prints swatches of `obj` in the terminal with colored text.
+           tabular=True,
+           file=sys.stdout):
+    """Swatches a colorir object in the terminal.
 
     Each swatch consists of a rectangle of a color followed by its value (and name if known).
 
     Args:
         obj: What will be represented in the terminal. Is either a single color, a list of colors,
             a :class:`~colorir.palette.Palette`, a :class:`~colorir.palette.StackPalette` or a
             subclass of :class:`~colorir.gradient.Grad`.
         colored_text: Whether the text that follows the colored rectangles should also be colored.
         width: The width (in space characters) of the colored rectangles.
         height: The height (in number of lines) of the colored rectangles.
         tabular: Whether the colored rectangle, color name and color value should be printed each
             in its separate column. Only used if `obj` is a :class:`~colorir.palette.Palette`.
+        file: If ``None`` returns the swatch as a string. Otherwise, this argument must be a file object and
+            is passed to `print`.
     """
-    # Assume single ColorLike
-    if isinstance(obj, (ColorBase, str, tuple)):
-        obj = [obj]
-    elif isinstance(obj, Grad):
+    longest_name = None
+    if isinstance(obj, Grad):
         # Seven steps for each color transition = 7 * (n - 1) - (n - 2)
         obj = obj.n_colors(6 * len(obj.colors) - 5, include_ends=True)
     elif isinstance(obj, palette.Palette):
         longest_name = max([len(name) for name in obj.color_names])
+    # Assume single ColorLike
+    elif not isinstance(obj, (list, palette.StackPalette)):
+        obj = [obj]
     # Needed to make Windows understand "\33" (https://stackoverflow.com/questions/12492810/python-
     # how-can-i-make-the-ansi-escape-codes-to-work-also-in-windows)
     os.system("")
+    ret_str = ""
     for i, c_val in enumerate(obj):
         rect_str = color_str(" " * width, bg_color=c_val)
         val_str = f" {c_val}"
-        if isinstance(obj, palette.Palette):
+        if longest_name is not None:
             name = obj.color_names[i]
             spacing = tabular * " " * (longest_name - len(name))
             val_str = ' ' + name + spacing + val_str
         if colored_text:
             val_str = color_str(val_str, fg_color=c_val)
-        print(rect_str + val_str)
+        ret_str += rect_str + val_str + '\n'
         for _ in range(height - 1):
-            print(rect_str)
+            ret_str += rect_str + '\n'
+    ret_str = ret_str.strip("\n")
+    if file is None:
+        return ret_str
+    print(ret_str, file=file)
+
 
+def show(obj,
+         width=None,
+         height=None,
+         interactive=None,
+         inline=True):
+    """Shows a colorir object inlined on a Jupyter notebook or using tkinter.
 
-# Implemented this way rather than a sort_colors function because it can be combined with
-# other keys (see color_picker example)
-def hue_sort_key(hue_classes=1,
+    Args:
+        inline: If running on a Jupyter notebook, whether to display the object inline.
+            Requires Pillow to be installed.
+        obj:
+        width:
+        height:
+        interactive: Whether clicking of the screen will copy the color value
+            to the clipboard and swatch the color on the terminal. Setting this
+            parameter to ``False`` results is a dramatic speed-up. By default,
+            is set to ``True`` for small objects (less than 100 colors) and
+            ``False`` otherwise. Only has an effect if not running on a
+            Jupyter notebook with `inline` == ``True``.
+    """
+    if inline:
+        try:
+            from IPython.display import display
+            # For some reason this function is not in globals()... so we gotta try it
+            if get_ipython().__class__.__name__ == "ZMQInteractiveShell":
+                display(make_image(obj, width, height))
+                return
+        except (ImportError, NameError):
+            pass
+        show_tkinter(obj, width, height, interactive)
+
+
+def show_tkinter(obj, width, height, interactive):
+    import tkinter as tk
+    from . import tkinter_utils as tku
+
+    win = tk.Tk()
+    win.resizable(False, False)
+
+    max_width = win.winfo_screenwidth() * 0.8
+    max_height = win.winfo_screenheight() * 0.8
+
+    if isinstance(obj, Grad):
+        if width is None:
+            width = min(max_width, max(0.4 * max_width, 50 * len(obj.colors)))
+        if height is None:
+            height = 0.1 * max_height
+        width, height = int(width), int(height)
+
+        # Each button is two pixels wide to make the widget lighter
+        colors = obj.n_colors(round(width / 2))
+        color_names = None
+    else:
+        if isinstance(obj, palette.Palette):
+            colors = obj.colors
+            color_names = obj.color_names
+        elif isinstance(obj, (palette.StackPalette, list)):
+            colors = list(obj)
+            color_names = None
+        else:
+            colors = [config.DEFAULT_COLOR_FORMAT.format(obj)]
+            color_names = None
+
+        if height is None:
+            height = 0.1 * max_height
+        if width is None:
+            width = min(max_width, len(colors) * height)
+        width, height = int(width), int(height)
+
+    if interactive is None:
+        interactive = True if len(colors) < 100 else False
+    if interactive:
+        wgt = tku.PaletteWidget(
+            win,
+            colors,
+            color_names=color_names,
+            width=width,
+            height=height
+        )
+    else:
+        wgt = tku.StaticPaletteWidget(
+            win,
+            colors,
+            width=width,
+            height=height
+        )
+    wgt.pack()
+    win.mainloop()
+
+
+def make_image(obj, width, height):
+    from PIL import Image
+
+    if height is None:
+        height = 64
+    if isinstance(obj, Grad):
+        if width is None:
+            width = 512
+        colors = obj.n_colors(width)
+    else:
+        if not isinstance(obj, (palette.PaletteBase, list)):
+            obj = [config.DEFAULT_COLOR_FORMAT.format(obj)]
+        colors = list(obj)
+        if width is None:
+            width = height * len(colors)
+    img = np.array([config.DEFAULT_COLOR_FORMAT.format(color)._rgba for color in colors], dtype="uint8")
+    # Add height dim
+    img = np.reshape(img, (1, img.shape[0], 4))
+    img = img.repeat(height, axis=0).repeat(width // len(colors), axis=1)
+    return Image.fromarray(img, "RGBA")
+
+
+def hue_sort_key(hue_classes=None,
                  gray_thresh=12.0,
                  gray_start=True,
                  alt_lum=False,
                  invert_lum=False):
     """Returns a function that can be used as a key for python's 'sort' and 'sorted' in order to
     sort color-like objects by their hue component.
 
     Examples:
         >>> sorted(["0000ff", "ff0000",  "000000", "00ff00", "ffffff"], key=hue_sort_key())
         ['000000', 'ffffff', 'ff0000', '00ff00', '0000ff']
 
     Args:
         hue_classes: Number hue categories. Inside each hue category colors will be sorted by
-            luminance rather than hue.
+            luminance rather than hue. When ``None``, colors are sorted only according to
+            their hue.
         gray_thresh: Chroma threshold bellow which a color will be considered a shade of gray.
         gray_start: Whether the colors considered shades of gray will be grouped at the start or
             end of the sorted iterable.
         alt_lum: Whether to alternate luminance values with each hue class transition. Only has an
             effect if `hue_classes` > 1.
         invert_lum: By default, sorting within hue classes happen from darker to lighter colors.
             This parameter allows inverting this patern, thus starting with light colors and going
@@ -101,28 +255,38 @@
     def sort_key(color):
         interpreted = color_format.format(color)
         h, c, l = HCLab._from_rgba(interpreted._rgba, max_h=1)
         if c < gray_thresh:
             h = gray_hue
             if not gray_start and alt_lum and hue_classes % 2 == 1:
                 l *= -1
-        elif hue_classes > 1:
+        elif hue_classes is not None:
             h = int(h * hue_classes)
             if alt_lum and h % 2 == (not gray_start):
                 l *= -1
 
-        if hue_classes == 1:
+        if hue_classes is None:
             return h
         if invert_lum:
             l *= -1
         return h, l
 
     return sort_key
 
 
+def hue_sorted(colors: Iterable[ColorLike], **kwargs) -> List[ColorLike]:
+    """Sort colors by their hue values. See :func:`~colorir.utils.hue_sort_key` for the arguments docs.
+
+    Returns:
+        A list of sorted colors.
+    """
+    key = hue_sort_key(**kwargs)
+    return sorted(colors, key=key)
+
+
 def simplified_dist(color1: ColorLike,
                     color2: ColorLike):
     """Calculates the perceived distance between two colors.
 
     There are many methods to approach the similarity of colors mathematically. The
     algorithm implemented in this function [#]_ tries to provide balance between efficiency and
     accuracy by using a weighted euclidian distance formula in the RGB color space.
@@ -143,16 +307,16 @@
         color2 = color_format.format(color2)
     rgba1, rgba2 = color1._rgba, color2._rgba
     avg_r = (rgba1[0] + rgba2[0]) / (2 * 255)
     d_r = rgba1[0] - rgba2[0]
     d_g = rgba1[1] - rgba2[1]
     d_b = rgba1[2] - rgba2[2]
     return sqrt((2 + avg_r) * d_r ** 2
-                 + 4 * d_g ** 2
-                 + (3 - avg_r) * d_b ** 2)
+                + 4 * d_g ** 2
+                + (3 - avg_r) * d_b ** 2)
 
 
 # TODO doc (mention 2000 not working properly in colormath and kwargs for delta-e funcs)
 def color_dist(color1: ColorLike, color2: ColorLike, method="CIE76"):
     if method == "simplified":
         return simplified_dist(color1, color2)
 
@@ -226,24 +390,18 @@
         rgba = config.DEFAULT_COLOR_FORMAT.format(bg_color)._rgba
         string = f"\033[48;2;{rgba[0]};{rgba[1]};{rgba[2]}m" + string + "\33[0m"
     return string
 
 
 # https://entropymine.com/imageworsener/srgbformula/
 def _to_linear_rgb(rgba):
-    rgba = list(rgba)
-    for i in range(3):
-        if rgba[i] <= 255 * 0.04045:
-            rgba[i] /= 12.92
-        else:
-            rgba[i] = 255 * pow(((rgba[i] / 255 + 0.055) / 1.055), 2.4)
-    return tuple(rgba)
+    """rgba must be in range 0-1"""
+    srgb = np.array(rgba[:-1])
+    lrgb = np.where(srgb <= 0.04045, srgb / 12.92, ((srgb + 0.055) / 1.055) ** 2.4)
+    return np.pad(lrgb, [(0, 1)], constant_values=rgba[-1])
 
 
 def _to_srgb(rgba):
-    rgba = list(rgba)
-    for i in range(3):
-        if rgba[i] <= 255 * 0.0031308:
-            rgba[i] *= 12.92
-        else:
-            rgba[i] = 255 * (1.055 * pow(rgba[i] / 255, 1/2.4) - 0.055)
-    return tuple(rgba)
+    """rgba must be in range 0-1"""
+    lrgb = np.array(rgba[:-1])
+    srgb = np.where(lrgb <= 0.0031308, lrgb * 12.92, 1.055 * lrgb ** (1 / 2.4) - 0.055)
+    return np.pad(srgb, [(0, 1)], constant_values=rgba[-1])
```

### Comparing `colorir-1.3.9/colorir.egg-info/PKG-INFO` & `colorir-2.0.0/colorir.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,81 @@
 Metadata-Version: 2.1
 Name: colorir
-Version: 1.3.9
+Version: 2.0.0
 Summary: A python package for easy management of colors and palettes.
 Home-page: https://github.com/aleferna12/colorir
 Author: aleferna
 Author-email: alexandrepchfernandes@gmail.com
 License: MIT
 Project-URL: Documentation, https://colorir.readthedocs.io/en/latest/
-Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 .. note::
 
     colorir is still in its early days and slight modifications to the API may happen between versions.
 
 What is colorir?
 ----------------
 
-colorir is a package developed to unify your workflow with colors across different projects.
+colorir is a package that allows users to manipulate colors and palettes.
 
 With colorir you can:
 
-- Keep a unified selection of colors you like and use them in your different projects;
-- Use these colors directly as input for other graphical or web frameworks;
+- Create palettes and save them to use in different projects;
+- Have access to a curated selection of unique color palettes and color names;
 - Easily convert between different color systems and formats;
 - Create gradients between colors and sample from them;
 - Easily visualize swatches of colors in the terminal;
-- And much more!
+- Pass color values directly as input for other graphical or web frameworks;
+- And more!
 
 colorir was designed to be your best friend when dealing with colors so that you won't ever need to write this kind of code again:
 
 .. code-block:: python
 
     BLACK = (0, 0, 0)
     WHITE = (255, 255, 255)
     CSS_ALICEBLUE = (240, 248, 255)
-    COOL_PURPLE = (11, 0, 51)
-    MY_FAVORITE_GREEN = (113, 180, 141)
-    TOP_NOTCH_RED = (131, 34, 50)
-    # ... unnecessarily long and ugly list of colors
+    BACKGROUND_COLOR = (11, 0, 51)
+    FONT_COLOR = (113, 180, 141)
+    LINE_PLOT_COLOR = (131, 34, 50)
+    # ... long and ugly list of colors
 
 Getting Started
 ---------------
 
 Getting started with colorir can be as simple as:
 
 .. code-block:: python
 
-    import tkinter as tk
-    from colorir import *
+    sky = Palette.load("sky")  # Loads a previously created palette called sky
+    sky_grad = PolarGrad([sky.sunrise, sky.highnoon])  # Creates a gradient from the color "sunrise" to the color "highnoon"
+    swatch(sky)  # Shows colorir objects in the terminal
+    swatch(sky_grad)
 
-    colors = Palette.load()  # Load colors
+This code should print both the palette and the gradient directly in your terminal:
 
-    win = tk.Tk()
-    win.configure(bg=colors.magicmint)  # Set background to 'magicmint' color
-    win.mainloop()
+.. image:: docs/source/images/readme_sky.png
 
-.. image:: readme_example.png
+Colorir can be used to interpolate and manipulate colors in many different color systems,
+such as CIELab and HCLab (LCHab).
 
-For more information (including use-cases and examples), see colorir's documentation `here <https://colorir.readthedocs.io/en/latest/>`_.
+Now let's make a gray scale version of the sky palette and save it to use later on
+another project:
+
+.. code-block:: python
+
+    gray_sky = sky.grayscale()
+    gray_sky.save("gray_sky")
+
+Now the gray_sky palette can be loaded with from a different script:
 
+.. code-block:: python
+
+    gray_sky = Palette.load("gray_sky")
+    swatch(gray_sky)
+
+.. image:: docs/source/images/readme_gray_sky.png
+
+For more information (including use-cases and examples), see colorir's documentation `here <https://colorir.readthedocs.io/en/latest/>`_.
```

### Comparing `colorir-1.3.9/setup.py` & `colorir-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE/"README.rst").read_text()
 
 setup(
     name="colorir",
-    version="1.3.9",
+    version="2.0.0",
     packages=["colorir"],
     url="https://github.com/aleferna12/colorir",
     license="MIT",
     author="aleferna",
     author_email="alexandrepchfernandes@gmail.com",
     description="A python package for easy management of colors and palettes.",
     long_description=README,
     long_description_content_type="text/x-rst",
     project_urls={"Documentation": "https://colorir.readthedocs.io/en/latest/"},
     include_package_data=True,
     python_requires=">=3.8",
-    install_requires=["colormath", "numpy<1.23.0"]
-)
+    install_requires=["colormath", "numpy"]
+)
```

### Comparing `colorir-1.3.9/tests/test_palette.py` & `colorir-2.0.0/tests/test_palette.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,84 +1,86 @@
 import doctest
 import unittest
 from pathlib import Path
 from random import randint
 import re
 
-from colorir import palette, config, Palette, StackPalette, HSV, find_palettes, delete_palette
+from colorir import *
+
+config.REPR_STYLE = "traditional"
 config.DEFAULT_PALETTES_DIR = str(Path(__file__).resolve().parent / "test_palettes")
 # Clear test palette directory
 for file in Path(config.DEFAULT_PALETTES_DIR).glob("*"):
     # Keep original test files, remove others
     if re.search(r"test\d", file.name) is None:
         file.unlink()
 
 
 class TestPalette(unittest.TestCase):
-    def test_add_op(self):
-        pal = Palette(c1="ffffff") + Palette(c2="000000")
+    def test_and_op(self):
+        pal = Palette(c1="ffffff") & Palette(c2="000000")
         self.assertEqual(pal, Palette(c1="ffffff", c2="000000"))
 
     def test_save_load(self):
         colors = {f"c{i}": "%02x%02x%02x" % (randint(0, 255), randint(0, 255), randint(0, 255))
                   for i in range(250)}
-        pal = Palette("test_sl", None, **colors)
-        pal.save()
+        pal = Palette(colors)
+        pal.save(name="test_sl")
         pal2 = Palette.load("test_sl")
         self.assertEqual(pal, pal2)
 
     def test_load_warns(self):
         with self.assertWarns(Warning):
             Palette.load(palettes=["test1", "test2"], search_builtins=False)
 
 
 class TestSwatchPalette(unittest.TestCase):
-    def test_add_op(self):
-        spal = StackPalette(None, None, "ffffff") + StackPalette(None, None, "000000")
-        self.assertEqual(spal, StackPalette(None, None, "ffffff", "000000"))
+    def test_and_op(self):
+        spal = StackPalette(["ffffff"]) & StackPalette(["000000"])
+        self.assertEqual(spal, StackPalette(["ffffff", "000000"]))
 
     def test_save_load(self):
         colors = ["%02x%02x%02x" % (randint(0, 255), randint(0, 255), randint(0, 255))
                   for _ in range(250)]
-        spal = StackPalette("test_sl", None, *colors)
-        spal.save()
+        spal = StackPalette(colors)
+        spal.save(name="test_sl")
         spal2 = StackPalette.load("test_sl")
         self.assertEqual(spal, spal2)
 
     def test_complementary(self):
         red = "ff0000"
         spal = StackPalette.new_complementary(3, red)
-        self.assertEqual(spal, StackPalette(None, None, red, "00ff00", "0000ff"))
+        self.assertEqual(spal, StackPalette([red, "00ff00", "0000ff"]))
 
     def test_analogous(self):
         red = HSV(0, 1, 1)
         # Center, clockwise and counter-clockwise generation
         c_spal = StackPalette.new_analogous(3, color=red)
         cw_spal = StackPalette.new_analogous(3, color=red, start=1)
         ccw_spal = StackPalette.new_analogous(3, color=red, start=-1)
-        self.assertEqual(c_spal, StackPalette(None, None, HSV(330, 1, 1), red, HSV(30, 1, 1)))
-        self.assertEqual(cw_spal, StackPalette(None, None, red, HSV(30, 1, 1), HSV(60, 1, 1)))
-        self.assertEqual(ccw_spal, StackPalette(None, None, HSV(300, 1, 1), HSV(330, 1, 1), red))
+        self.assertEqual(c_spal, StackPalette([HSV(330, 1, 1), red, HSV(30, 1, 1)]))
+        self.assertEqual(cw_spal, StackPalette([red, HSV(30, 1, 1), HSV(60, 1, 1)]))
+        self.assertEqual(ccw_spal, StackPalette([HSV(300, 1, 1), HSV(330, 1, 1), red]))
         # Larger hue wheel sections
         wide_spal = StackPalette.new_analogous(3, sections=3, color=red)
-        self.assertEqual(wide_spal, StackPalette(None, None, HSV(240, 1, 1), red, HSV(120, 1, 1)))
+        self.assertEqual(wide_spal, StackPalette([HSV(240, 1, 1), red, HSV(120, 1, 1)]))
 
 
 class TestOtherFunctions(unittest.TestCase):
     def test_find_palettes(self):
         all_pals = find_palettes(search_builtins=False)
         self.assertEqual(all_pals, ['test1', 'test2', 'test3'])
         pals = find_palettes(search_builtins=False, kind=Palette)
         self.assertEqual(pals, ['test1', 'test2'])
         spals = find_palettes(search_builtins=False, kind=StackPalette)
         self.assertEqual(spals, ['test3'])
 
     def test_delete_palette(self):
-        n_pal = Palette("test_del", red="ff0000")
-        n_pal.save()
+        n_pal = Palette(red="ff0000")
+        n_pal.save("test_del")
         self.assertIn("test_del", find_palettes())
         delete_palette("test_del")
         self.assertNotIn("test_del", find_palettes())
 
 
 def load_tests(loader, tests, ignore):
     tests.addTests(doctest.DocTestSuite(palette))
```

