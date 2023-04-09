# Comparing `tmp/usda-0.0.18.tar.gz` & `tmp/usda-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usda-0.0.18.tar", last modified: Thu Feb 23 02:45:53 2023, max compression
+gzip compressed data, was "usda-0.0.19.tar", last modified: Sun Apr  9 05:18:43 2023, max compression
```

## Comparing `usda-0.0.18.tar` & `usda-0.0.19.tar`

### file list

```diff
@@ -1,118 +1,161 @@
-drwxrwxrwx   0        0        0        0 2023-02-23 02:45:53.674365 usda-0.0.18/
--rw-rw-rw-   0        0        0     1084 2022-10-07 01:27:44.000000 usda-0.0.18/LICENSE
--rw-rw-rw-   0        0        0     1563 2023-02-23 02:45:53.671366 usda-0.0.18/PKG-INFO
--rw-rw-rw-   0        0        0       63 2022-10-24 05:51:49.000000 usda-0.0.18/README.rst
--rw-rw-rw-   0        0        0       42 2023-02-23 02:45:53.674365 usda-0.0.18/setup.cfg
--rw-rw-rw-   0        0        0     4132 2022-10-22 08:24:06.000000 usda-0.0.18/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-23 02:45:53.350365 usda-0.0.18/src/
-drwxrwxrwx   0        0        0        0 2023-02-23 02:45:53.377401 usda-0.0.18/src/usda/
--rw-rw-rw-   0        0        0      441 2023-02-23 00:53:12.000000 usda-0.0.18/src/usda/__init__.py
--rw-rw-rw-   0        0        0      731 2022-10-16 01:25:29.000000 usda-0.0.18/src/usda/_min_dependencies.py
-drwxrwxrwx   0        0        0        0 2023-02-23 02:45:53.414365 usda-0.0.18/src/usda/data_process/
--rw-rw-rw-   0        0        0      922 2023-02-11 08:27:04.000000 usda-0.0.18/src/usda/data_process/__init__.py
--rw-rw-rw-   0        0        0     2125 2022-10-22 01:48:58.000000 usda-0.0.18/src/usda/data_process/_geoinfodata_conversion.py
--rw-rw-rw-   0        0        0    14577 2022-10-28 01:52:51.000000 usda-0.0.18/src/usda/data_process/_image_pixel_sampling_zoom.py
--rw-rw-rw-   0        0        0     1425 2022-10-31 06:03:57.000000 usda-0.0.18/src/usda/data_process/_kitti_dataprocess.py
--rw-rw-rw-   0        0        0     2037 2022-10-26 01:37:19.000000 usda-0.0.18/src/usda/data_process/_landsat_dataprocess.py
--rw-rw-rw-   0        0        0     6348 2022-10-22 00:18:38.000000 usda-0.0.18/src/usda/data_process/_osm_dataprocess.py
--rw-rw-rw-   0        0        0     1085 2023-02-11 08:44:30.000000 usda-0.0.18/src/usda/data_process/_raster_dataprocess.py
--rw-rw-rw-   0        0        0     1332 2022-10-30 06:27:55.000000 usda-0.0.18/src/usda/data_process/_tiler_calculation.py
-drwxrwxrwx   0        0        0        0 2023-02-23 02:45:53.476366 usda-0.0.18/src/usda/data_visualization/
--rw-rw-rw-   0        0        0     2997 2023-02-19 14:45:35.000000 usda-0.0.18/src/usda/data_visualization/__init__.py
--rw-rw-rw-   0        0        0     5300 2023-02-17 02:29:25.000000 usda-0.0.18/src/usda/data_visualization/_chart_custom.py
--rw-rw-rw-   0        0        0     2351 2022-11-02 07:56:57.000000 usda-0.0.18/src/usda/data_visualization/_colors.py
--rw-rw-rw-   0        0        0     3221 2022-10-29 07:58:07.000000 usda-0.0.18/src/usda/data_visualization/_dynamic_streetView_visual_perception.py
--rw-rw-rw-   0        0        0     3557 2023-02-19 14:47:51.000000 usda-0.0.18/src/usda/data_visualization/_gdf_plot.py
--rw-rw-rw-   0        0        0      952 2022-10-28 11:19:32.000000 usda-0.0.18/src/usda/data_visualization/_gif_show.py
--rw-rw-rw-   0        0        0     2347 2022-10-28 06:34:44.000000 usda-0.0.18/src/usda/data_visualization/_graphic_drawing.py
--rw-rw-rw-   0        0        0     4787 2022-10-31 05:36:51.000000 usda-0.0.18/src/usda/data_visualization/_image_process.py
--rw-rw-rw-   0        0        0     8500 2022-10-29 06:42:38.000000 usda-0.0.18/src/usda/data_visualization/_img_feature_extraction.py
--rw-rw-rw-   0        0        0     7196 2022-10-30 12:18:06.000000 usda-0.0.18/src/usda/data_visualization/_img_theme_color.py
--rw-rw-rw-   0        0        0     2846 2022-10-30 11:18:24.000000 usda-0.0.18/src/usda/data_visualization/_imgs_layout_show.py
--rw-rw-rw-   0        0        0     4122 2023-02-15 06:27:03.000000 usda-0.0.18/src/usda/data_visualization/_imgs_show.py
--rw-rw-rw-   0        0        0      822 2022-11-02 06:07:14.000000 usda-0.0.18/src/usda/data_visualization/_knee_line_graph.py
--rw-rw-rw-   0        0        0     7393 2022-10-29 08:23:53.000000 usda-0.0.18/src/usda/data_visualization/_moving_average_inflection.py
--rw-rw-rw-   0        0        0     2310 2022-10-28 01:13:41.000000 usda-0.0.18/src/usda/data_visualization/_raster_percentile_slider.py
--rw-rw-rw-   0        0        0     1224 2022-10-28 00:45:13.000000 usda-0.0.18/src/usda/data_visualization/_raster_show.py
--rw-rw-rw-   0        0        0     2130 2022-10-28 06:32:06.000000 usda-0.0.18/src/usda/data_visualization/_stats_charts.py
--rw-rw-rw-   0        0        0     2666 2022-10-30 07:27:14.000000 usda-0.0.18/src/usda/data_visualization/_superpixel_segmentation_show.py
--rw-rw-rw-   0        0        0     1577 2022-10-22 23:37:39.000000 usda-0.0.18/src/usda/data_visualization/_table_show.py
--rw-rw-rw-   0        0        0     1673 2022-11-02 06:07:23.000000 usda-0.0.18/src/usda/data_visualization/_tile_show.py
--rw-rw-rw-   0        0        0     4464 2020-07-17 02:38:10.000000 usda-0.0.18/src/usda/data_visualization/data_generator.py
--rw-rw-rw-   0        0        0    10263 2020-07-17 02:38:10.000000 usda-0.0.18/src/usda/data_visualization/knee_locator.py
-drwxrwxrwx   0        0        0        0 2023-02-23 02:45:53.491366 usda-0.0.18/src/usda/database/
--rw-rw-rw-   0        0        0      663 2022-10-30 12:16:19.000000 usda-0.0.18/src/usda/database/__init__.py
--rw-rw-rw-   0        0        0      693 2022-10-30 12:15:41.000000 usda-0.0.18/src/usda/database/_data_file_rw.py
--rw-rw-rw-   0        0        0     3990 2022-10-18 13:55:09.000000 usda-0.0.18/src/usda/database/_data_format_conversion.py
--rw-rw-rw-   0        0        0     3677 2022-10-18 09:46:45.000000 usda-0.0.18/src/usda/database/_database.py
--rw-rw-rw-   0        0        0     1384 2022-10-28 08:27:55.000000 usda-0.0.18/src/usda/database/_read_matlab_fig.py
-drwxrwxrwx   0        0        0        0 2023-02-23 02:45:53.511364 usda-0.0.18/src/usda/datasets/
--rw-rw-rw-   0        0        0     1283 2023-02-23 00:41:30.000000 usda-0.0.18/src/usda/datasets/__init__.py
--rw-rw-rw-   0        0        0     5608 2023-02-23 02:43:57.000000 usda-0.0.18/src/usda/datasets/_artificial_data.py
--rw-rw-rw-   0        0        0    15178 2023-02-23 02:45:34.000000 usda-0.0.18/src/usda/datasets/_base.py
--rw-rw-rw-   0        0        0     2745 2022-10-31 05:44:19.000000 usda-0.0.18/src/usda/datasets/_dataset_info.py
--rw-rw-rw-   0        0        0     2681 2022-10-30 11:21:33.000000 usda-0.0.18/src/usda/datasets/_img_info.py
--rw-rw-rw-   0        0        0     2806 2022-10-30 10:50:28.000000 usda-0.0.18/src/usda/datasets/_kml_info.py
--rw-rw-rw-   0        0        0     1547 2022-10-30 07:02:03.000000 usda-0.0.18/src/usda/datasets/_rs_image.py
-drwxrwxrwx   0        0        0        0 2023-02-23 02:45:53.532365 usda-0.0.18/src/usda/datasets/data/
--rw-rw-rw-   0        0        0      125 2022-08-21 07:11:20.000000 usda-0.0.18/src/usda/datasets/data/__init__.py
--rw-rw-rw-   0        0        0     1224 2022-10-19 04:41:26.000000 usda-0.0.18/src/usda/datasets/data/bowling_contest_cartoon_statistic.pickle
--rw-rw-rw-   0        0        0      950 2023-02-23 02:44:29.000000 usda-0.0.18/src/usda/datasets/data/evaluation_criteria_raw_values.pickle
--rw-rw-rw-   0        0        0     1089 2022-10-19 01:41:55.000000 usda-0.0.18/src/usda/datasets/data/ramen_price_cartoon_statistic.pickle
--rw-rw-rw-   0        0        0     2123 2022-10-15 01:16:56.000000 usda-0.0.18/src/usda/datasets/data/sales_data_cartoon_database.pickle
--rw-rw-rw-   0        0        0     1340 2022-10-19 05:00:19.000000 usda-0.0.18/src/usda/datasets/data/test_score_cartoon_statistic.pickle
-drwxrwxrwx   0        0        0        0 2023-02-23 02:45:53.542366 usda-0.0.18/src/usda/geodata_process/
--rw-rw-rw-   0        0        0      572 2023-02-19 12:23:23.000000 usda-0.0.18/src/usda/geodata_process/__init__.py
--rw-rw-rw-   0        0        0     3167 2023-02-11 09:17:10.000000 usda-0.0.18/src/usda/geodata_process/_quadrat.py
--rw-rw-rw-   0        0        0     4152 2023-02-19 12:22:55.000000 usda-0.0.18/src/usda/geodata_process/_raster_dataprocess.py
-drwxrwxrwx   0        0        0        0 2023-02-23 02:45:53.547366 usda-0.0.18/src/usda/indices/
--rw-rw-rw-   0        0        0      189 2022-10-26 06:14:56.000000 usda-0.0.18/src/usda/indices/__init__.py
--rw-rw-rw-   0        0        0      574 2022-10-26 06:15:29.000000 usda-0.0.18/src/usda/indices/_rs_indices.py
-drwxrwxrwx   0        0        0        0 2023-02-23 02:45:53.557366 usda-0.0.18/src/usda/maths/
--rw-rw-rw-   0        0        0      557 2022-10-26 03:06:13.000000 usda-0.0.18/src/usda/maths/__init__.py
--rw-rw-rw-   0        0        0     4335 2022-10-26 02:53:02.000000 usda-0.0.18/src/usda/maths/_algebra.py
--rw-rw-rw-   0        0        0     1519 2022-10-26 03:05:19.000000 usda-0.0.18/src/usda/maths/_geometric_calculation.py
-drwxrwxrwx   0        0        0        0 2023-02-23 02:45:53.601366 usda-0.0.18/src/usda/models/
--rw-rw-rw-   0        0        0     1876 2022-11-02 10:07:51.000000 usda-0.0.18/src/usda/models/__init__.py
--rw-rw-rw-   0        0        0     3873 2022-10-31 06:56:19.000000 usda-0.0.18/src/usda/models/_bow_feature_builder.py
--rw-rw-rw-   0        0        0     3105 2022-10-25 01:59:30.000000 usda-0.0.18/src/usda/models/_computational_performance.py
--rw-rw-rw-   0        0        0     1897 2022-10-28 08:34:08.000000 usda-0.0.18/src/usda/models/_curve_segmentation.py
--rw-rw-rw-   0        0        0     3928 2022-10-31 07:59:05.000000 usda-0.0.18/src/usda/models/_decision_tree.py
--rw-rw-rw-   0        0        0     5811 2022-10-28 08:15:41.000000 usda-0.0.18/src/usda/models/_dim1_convolution.py
--rw-rw-rw-   0        0        0     2676 2022-10-31 07:41:49.000000 usda-0.0.18/src/usda/models/_entropy.py
--rw-rw-rw-   0        0        0     1427 2022-11-02 06:11:04.000000 usda-0.0.18/src/usda/models/_image_tag_extractor.py
--rw-rw-rw-   0        0        0      869 2022-10-31 07:16:43.000000 usda-0.0.18/src/usda/models/_label_encoder.py
--rw-rw-rw-   0        0        0     1022 2022-10-25 01:02:56.000000 usda-0.0.18/src/usda/models/_neighbors.py
--rw-rw-rw-   0        0        0     1422 2022-10-31 08:30:25.000000 usda-0.0.18/src/usda/models/_random_forest_classifier.py
--rw-rw-rw-   0        0        0    11923 2022-10-28 11:44:45.000000 usda-0.0.18/src/usda/models/_sir_model.py
--rw-rw-rw-   0        0        0     3200 2022-10-30 07:33:05.000000 usda-0.0.18/src/usda/models/_superpixel_segmentation.py
-drwxrwxrwx   0        0        0        0 2023-02-23 02:45:53.623363 usda-0.0.18/src/usda/pattern_signature/
--rw-rw-rw-   0        0        0     1265 2023-02-19 13:43:40.000000 usda-0.0.18/src/usda/pattern_signature/__init__.py
--rw-rw-rw-   0        0        0     5975 2023-02-12 02:57:51.000000 usda-0.0.18/src/usda/pattern_signature/_distance_metric.py
--rw-rw-rw-   0        0        0     1182 2023-02-09 14:05:16.000000 usda-0.0.18/src/usda/pattern_signature/_grid_neighbors_xy_finder.py
--rw-rw-rw-   0        0        0     8778 2023-02-19 14:00:29.000000 usda-0.0.18/src/usda/pattern_signature/_img_region_growing.py
--rw-rw-rw-   0        0        0    20197 2023-02-19 13:21:56.000000 usda-0.0.18/src/usda/pattern_signature/_pattern_module.py
--rw-rw-rw-   0        0        0     6662 2023-02-17 02:48:45.000000 usda-0.0.18/src/usda/pattern_signature/_signature.py
--rw-rw-rw-   0        0        0     3191 2023-02-12 09:54:49.000000 usda-0.0.18/src/usda/pattern_signature/_signature2distance_integration.py
-drwxrwxrwx   0        0        0        0 2023-02-23 02:45:53.638366 usda-0.0.18/src/usda/stats/
--rw-rw-rw-   0        0        0     1011 2022-10-24 05:16:26.000000 usda-0.0.18/src/usda/stats/__init__.py
--rw-rw-rw-   0        0        0     3501 2022-10-20 03:25:19.000000 usda-0.0.18/src/usda/stats/_descriptive_stats.py
--rw-rw-rw-   0        0        0     2233 2022-10-22 02:45:57.000000 usda-0.0.18/src/usda/stats/_kde.py
--rw-rw-rw-   0        0        0      778 2022-10-20 03:57:18.000000 usda-0.0.18/src/usda/stats/_outlier.py
--rw-rw-rw-   0        0        0    10793 2022-10-24 05:19:28.000000 usda-0.0.18/src/usda/stats/_regression.py
-drwxrwxrwx   0        0        0        0 2023-02-23 02:45:53.667367 usda-0.0.18/src/usda/utils/
--rw-rw-rw-   0        0        0      960 2023-02-12 06:58:00.000000 usda-0.0.18/src/usda/utils/__init__.py
--rw-rw-rw-   0        0        0     1497 2022-10-17 01:46:32.000000 usda-0.0.18/src/usda/utils/_bunch.py
--rw-rw-rw-   0        0        0     5197 2022-10-18 07:06:26.000000 usda-0.0.18/src/usda/utils/_coordinate_transformation.py
--rw-rw-rw-   0        0        0     3134 2023-02-12 07:00:21.000000 usda-0.0.18/src/usda/utils/_df_process.py
--rw-rw-rw-   0        0        0     2938 2022-10-17 01:57:17.000000 usda-0.0.18/src/usda/utils/_displayable_path.py
--rw-rw-rw-   0        0        0     1857 2022-10-26 01:31:31.000000 usda-0.0.18/src/usda/utils/_file_structure.py
--rw-rw-rw-   0        0        0     1342 2023-02-12 02:14:47.000000 usda-0.0.18/src/usda/utils/_gadgets.py
--rw-rw-rw-   0        0        0      606 2022-10-22 00:35:56.000000 usda-0.0.18/src/usda/utils/_operating_time.py
-drwxrwxrwx   0        0        0        0 2023-02-23 02:45:53.390367 usda-0.0.18/src/usda.egg-info/
--rw-rw-rw-   0        0        0     1563 2023-02-23 02:45:52.000000 usda-0.0.18/src/usda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3910 2023-02-23 02:45:53.000000 usda-0.0.18/src/usda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-23 02:45:52.000000 usda-0.0.18/src/usda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-10-16 07:33:50.000000 usda-0.0.18/src/usda.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       55 2023-02-23 02:45:52.000000 usda-0.0.18/src/usda.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-02-23 02:45:52.000000 usda-0.0.18/src/usda.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.513522 usda-0.0.19/
+-rw-rw-rw-   0        0        0     1084 2022-10-07 01:27:44.000000 usda-0.0.19/LICENSE
+-rw-rw-rw-   0        0        0     1563 2023-04-09 05:18:43.508519 usda-0.0.19/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2022-10-24 05:51:49.000000 usda-0.0.19/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-09 05:18:43.513522 usda-0.0.19/setup.cfg
+-rw-rw-rw-   0        0        0     4152 2023-03-18 11:11:09.000000 usda-0.0.19/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.004519 usda-0.0.19/src/
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.048519 usda-0.0.19/src/usda/
+-rw-rw-rw-   0        0        0      516 2023-04-09 05:17:48.000000 usda-0.0.19/src/usda/__init__.py
+-rw-rw-rw-   0        0        0      731 2022-10-16 01:25:29.000000 usda-0.0.19/src/usda/_min_dependencies.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.101519 usda-0.0.19/src/usda/data_process/
+-rw-rw-rw-   0        0        0     1147 2023-03-26 03:42:04.000000 usda-0.0.19/src/usda/data_process/__init__.py
+-rw-rw-rw-   0        0        0     2125 2022-10-22 01:48:58.000000 usda-0.0.19/src/usda/data_process/_geoinfodata_conversion.py
+-rw-rw-rw-   0        0        0    14577 2022-10-28 01:52:51.000000 usda-0.0.19/src/usda/data_process/_image_pixel_sampling_zoom.py
+-rw-rw-rw-   0        0        0     1425 2022-10-31 06:03:57.000000 usda-0.0.19/src/usda/data_process/_kitti_dataprocess.py
+-rw-rw-rw-   0        0        0     2037 2022-10-26 01:37:19.000000 usda-0.0.19/src/usda/data_process/_landsat_dataprocess.py
+-rw-rw-rw-   0        0        0     1854 2023-03-26 07:52:38.000000 usda-0.0.19/src/usda/data_process/_naip_dataprocess.py
+-rw-rw-rw-   0        0        0     6348 2022-10-22 00:18:38.000000 usda-0.0.19/src/usda/data_process/_osm_dataprocess.py
+-rw-rw-rw-   0        0        0     1085 2023-02-11 08:44:30.000000 usda-0.0.19/src/usda/data_process/_raster_dataprocess.py
+-rw-rw-rw-   0        0        0     1332 2022-10-30 06:27:55.000000 usda-0.0.19/src/usda/data_process/_tiler_calculation.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.192520 usda-0.0.19/src/usda/data_visualization/
+-rw-rw-rw-   0        0        0     3166 2023-03-17 02:59:30.000000 usda-0.0.19/src/usda/data_visualization/__init__.py
+-rw-rw-rw-   0        0        0     5300 2023-02-17 02:29:25.000000 usda-0.0.19/src/usda/data_visualization/_chart_custom.py
+-rw-rw-rw-   0        0        0     2351 2022-11-02 07:56:57.000000 usda-0.0.19/src/usda/data_visualization/_colors.py
+-rw-rw-rw-   0        0        0     3221 2022-10-29 07:58:07.000000 usda-0.0.19/src/usda/data_visualization/_dynamic_streetView_visual_perception.py
+-rw-rw-rw-   0        0        0     3557 2023-02-19 14:47:51.000000 usda-0.0.19/src/usda/data_visualization/_gdf_plot.py
+-rw-rw-rw-   0        0        0      952 2022-10-28 11:19:32.000000 usda-0.0.19/src/usda/data_visualization/_gif_show.py
+-rw-rw-rw-   0        0        0     2347 2022-10-28 06:34:44.000000 usda-0.0.19/src/usda/data_visualization/_graphic_drawing.py
+-rw-rw-rw-   0        0        0     4787 2022-10-31 05:36:51.000000 usda-0.0.19/src/usda/data_visualization/_image_process.py
+-rw-rw-rw-   0        0        0     8500 2022-10-29 06:42:38.000000 usda-0.0.19/src/usda/data_visualization/_img_feature_extraction.py
+-rw-rw-rw-   0        0        0     7196 2022-10-30 12:18:06.000000 usda-0.0.19/src/usda/data_visualization/_img_theme_color.py
+-rw-rw-rw-   0        0        0     2846 2022-10-30 11:18:24.000000 usda-0.0.19/src/usda/data_visualization/_imgs_layout_show.py
+-rw-rw-rw-   0        0        0     4174 2023-03-15 02:00:19.000000 usda-0.0.19/src/usda/data_visualization/_imgs_show.py
+-rw-rw-rw-   0        0        0      822 2022-11-02 06:07:14.000000 usda-0.0.19/src/usda/data_visualization/_knee_line_graph.py
+-rw-rw-rw-   0        0        0     7393 2022-10-29 08:23:53.000000 usda-0.0.19/src/usda/data_visualization/_moving_average_inflection.py
+-rw-rw-rw-   0        0        0     3176 2023-02-24 07:31:39.000000 usda-0.0.19/src/usda/data_visualization/_panorama_show.py
+-rw-rw-rw-   0        0        0     8051 2023-03-19 04:08:53.000000 usda-0.0.19/src/usda/data_visualization/_plot_single_function.py
+-rw-rw-rw-   0        0        0     2310 2022-10-28 01:13:41.000000 usda-0.0.19/src/usda/data_visualization/_raster_percentile_slider.py
+-rw-rw-rw-   0        0        0     1224 2022-10-28 00:45:13.000000 usda-0.0.19/src/usda/data_visualization/_raster_show.py
+-rw-rw-rw-   0        0        0     2130 2022-10-28 06:32:06.000000 usda-0.0.19/src/usda/data_visualization/_stats_charts.py
+-rw-rw-rw-   0        0        0     2666 2022-10-30 07:27:14.000000 usda-0.0.19/src/usda/data_visualization/_superpixel_segmentation_show.py
+-rw-rw-rw-   0        0        0     1577 2022-10-22 23:37:39.000000 usda-0.0.19/src/usda/data_visualization/_table_show.py
+-rw-rw-rw-   0        0        0     1673 2022-11-02 06:07:23.000000 usda-0.0.19/src/usda/data_visualization/_tile_show.py
+-rw-rw-rw-   0        0        0     4464 2020-07-17 02:38:10.000000 usda-0.0.19/src/usda/data_visualization/data_generator.py
+-rw-rw-rw-   0        0        0    10263 2020-07-17 02:38:10.000000 usda-0.0.19/src/usda/data_visualization/knee_locator.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.210520 usda-0.0.19/src/usda/database/
+-rw-rw-rw-   0        0        0      839 2023-03-21 05:11:06.000000 usda-0.0.19/src/usda/database/__init__.py
+-rw-rw-rw-   0        0        0      693 2022-10-30 12:15:41.000000 usda-0.0.19/src/usda/database/_data_file_rw.py
+-rw-rw-rw-   0        0        0     4636 2023-03-21 05:10:00.000000 usda-0.0.19/src/usda/database/_data_format_conversion.py
+-rw-rw-rw-   0        0        0     5605 2023-03-21 05:08:27.000000 usda-0.0.19/src/usda/database/_database.py
+-rw-rw-rw-   0        0        0     1384 2022-10-28 08:27:55.000000 usda-0.0.19/src/usda/database/_read_matlab_fig.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.234520 usda-0.0.19/src/usda/datasets/
+-rw-rw-rw-   0        0        0     1594 2023-03-13 12:31:06.000000 usda-0.0.19/src/usda/datasets/__init__.py
+-rw-rw-rw-   0        0        0    17136 2023-03-13 12:40:56.000000 usda-0.0.19/src/usda/datasets/_artificial_data.py
+-rw-rw-rw-   0        0        0    19730 2023-03-14 01:14:44.000000 usda-0.0.19/src/usda/datasets/_base.py
+-rw-rw-rw-   0        0        0     2745 2022-10-31 05:44:19.000000 usda-0.0.19/src/usda/datasets/_dataset_info.py
+-rw-rw-rw-   0        0        0     2681 2022-10-30 11:21:33.000000 usda-0.0.19/src/usda/datasets/_img_info.py
+-rw-rw-rw-   0        0        0     2806 2022-10-30 10:50:28.000000 usda-0.0.19/src/usda/datasets/_kml_info.py
+-rw-rw-rw-   0        0        0     1547 2022-10-30 07:02:03.000000 usda-0.0.19/src/usda/datasets/_rs_image.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.265521 usda-0.0.19/src/usda/datasets/data/
+-rw-rw-rw-   0        0        0      125 2022-08-21 07:11:20.000000 usda-0.0.19/src/usda/datasets/data/__init__.py
+-rw-rw-rw-   0        0        0     1224 2022-10-19 04:41:26.000000 usda-0.0.19/src/usda/datasets/data/bowling_contest_cartoon_statistic.pickle
+-rw-rw-rw-   0        0        0      950 2023-02-23 02:44:29.000000 usda-0.0.19/src/usda/datasets/data/evaluation_criteria_raw_values.pickle
+-rw-rw-rw-   0        0        0     8356 2023-03-13 12:16:36.000000 usda-0.0.19/src/usda/datasets/data/jisperveld_data.pickle
+-rw-rw-rw-   0        0        0     1486 2023-02-27 14:21:28.000000 usda-0.0.19/src/usda/datasets/data/microclimate_in_office_rooms.pickle
+-rw-rw-rw-   0        0        0     1089 2022-10-19 01:41:55.000000 usda-0.0.19/src/usda/datasets/data/ramen_price_cartoon_statistic.pickle
+-rw-rw-rw-   0        0        0     2123 2022-10-15 01:16:56.000000 usda-0.0.19/src/usda/datasets/data/sales_data_cartoon_database.pickle
+-rw-rw-rw-   0        0        0     1352 2023-02-24 07:53:38.000000 usda-0.0.19/src/usda/datasets/data/sustainability_attributes4electricity_generation_tech.pickle
+-rw-rw-rw-   0        0        0     1340 2022-10-19 05:00:19.000000 usda-0.0.19/src/usda/datasets/data/test_score_cartoon_statistic.pickle
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.286519 usda-0.0.19/src/usda/geodata_process/
+-rw-rw-rw-   0        0        0     1349 2023-03-26 01:38:53.000000 usda-0.0.19/src/usda/geodata_process/__init__.py
+-rw-rw-rw-   0        0        0     4314 2023-03-22 05:01:49.000000 usda-0.0.19/src/usda/geodata_process/_quadrat.py
+-rw-rw-rw-   0        0        0     6535 2023-03-22 16:40:23.000000 usda-0.0.19/src/usda/geodata_process/_raster_dataprocess.py
+-rw-rw-rw-   0        0        0     6633 2023-03-22 14:50:33.000000 usda-0.0.19/src/usda/geodata_process/_raster_stats.py
+-rw-rw-rw-   0        0        0     6661 2023-03-21 13:11:59.000000 usda-0.0.19/src/usda/geodata_process/_rasterize.py
+-rw-rw-rw-   0        0        0     3080 2023-03-22 01:53:07.000000 usda-0.0.19/src/usda/geodata_process/_rio_tiler.py
+-rw-rw-rw-   0        0        0     3340 2023-03-22 04:59:15.000000 usda-0.0.19/src/usda/geodata_process/_sample_pts.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.295521 usda-0.0.19/src/usda/indices/
+-rw-rw-rw-   0        0        0      189 2022-10-26 06:14:56.000000 usda-0.0.19/src/usda/indices/__init__.py
+-rw-rw-rw-   0        0        0      574 2022-10-26 06:15:29.000000 usda-0.0.19/src/usda/indices/_rs_indices.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.303520 usda-0.0.19/src/usda/maths/
+-rw-rw-rw-   0        0        0      557 2022-10-26 03:06:13.000000 usda-0.0.19/src/usda/maths/__init__.py
+-rw-rw-rw-   0        0        0     4335 2022-10-26 02:53:02.000000 usda-0.0.19/src/usda/maths/_algebra.py
+-rw-rw-rw-   0        0        0     1519 2022-10-26 03:05:19.000000 usda-0.0.19/src/usda/maths/_geometric_calculation.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.345520 usda-0.0.19/src/usda/meta_heuristics/
+-rw-rw-rw-   0        0        0      843 2023-03-19 01:33:28.000000 usda-0.0.19/src/usda/meta_heuristics/__init__.py
+-rw-rw-rw-   0        0        0     5889 2023-03-18 13:00:33.000000 usda-0.0.19/src/usda/meta_heuristics/_cuckoo_s.py
+-rw-rw-rw-   0        0        0     4919 2023-03-19 01:22:52.000000 usda-0.0.19/src/usda/meta_heuristics/_firefly_a.py
+-rw-rw-rw-   0        0        0    11373 2023-03-10 03:50:42.000000 usda-0.0.19/src/usda/meta_heuristics/_ga.py
+-rw-rw-rw-   0        0        0    13840 2023-03-15 22:13:00.000000 usda-0.0.19/src/usda/meta_heuristics/_ga_2d.py
+-rw-rw-rw-   0        0        0    14213 2023-03-16 01:38:05.000000 usda-0.0.19/src/usda/meta_heuristics/_ga_2d_fixed_map.py
+-rw-rw-rw-   0        0        0    15440 2023-03-15 14:33:57.000000 usda-0.0.19/src/usda/meta_heuristics/_ga_2d_testing_1.py
+-rw-rw-rw-   0        0        0    25287 2023-03-17 02:56:06.000000 usda-0.0.19/src/usda/meta_heuristics/_ga_2d_testing_2.py
+-rw-rw-rw-   0        0        0     4177 2023-03-10 02:05:28.000000 usda-0.0.19/src/usda/meta_heuristics/_ga_SegaranT.py
+-rw-rw-rw-   0        0        0     7982 2023-03-01 00:42:26.000000 usda-0.0.19/src/usda/meta_heuristics/_gwo.py
+-rw-rw-rw-   0        0        0     5251 2023-03-17 04:06:12.000000 usda-0.0.19/src/usda/meta_heuristics/_pso.py
+-rw-rw-rw-   0        0        0     7564 2023-03-18 04:30:41.000000 usda-0.0.19/src/usda/meta_heuristics/_pso_2d.py
+-rw-rw-rw-   0        0        0     8467 2023-03-18 05:15:54.000000 usda-0.0.19/src/usda/meta_heuristics/_pso_2d_testing.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.392521 usda-0.0.19/src/usda/models/
+-rw-rw-rw-   0        0        0     2110 2023-03-24 10:49:29.000000 usda-0.0.19/src/usda/models/__init__.py
+-rw-rw-rw-   0        0        0     3873 2022-10-31 06:56:19.000000 usda-0.0.19/src/usda/models/_bow_feature_builder.py
+-rw-rw-rw-   0        0        0     1014 2023-03-24 02:28:49.000000 usda-0.0.19/src/usda/models/_clustering.py
+-rw-rw-rw-   0        0        0     3105 2022-10-25 01:59:30.000000 usda-0.0.19/src/usda/models/_computational_performance.py
+-rw-rw-rw-   0        0        0     1897 2022-10-28 08:34:08.000000 usda-0.0.19/src/usda/models/_curve_segmentation.py
+-rw-rw-rw-   0        0        0     3928 2022-10-31 07:59:05.000000 usda-0.0.19/src/usda/models/_decision_tree.py
+-rw-rw-rw-   0        0        0     5811 2022-10-28 08:15:41.000000 usda-0.0.19/src/usda/models/_dim1_convolution.py
+-rw-rw-rw-   0        0        0     2676 2022-10-31 07:41:49.000000 usda-0.0.19/src/usda/models/_entropy.py
+-rw-rw-rw-   0        0        0     1458 2023-03-24 10:49:05.000000 usda-0.0.19/src/usda/models/_global_local_autocorrelation.py
+-rw-rw-rw-   0        0        0     1427 2022-11-02 06:11:04.000000 usda-0.0.19/src/usda/models/_image_tag_extractor.py
+-rw-rw-rw-   0        0        0      869 2022-10-31 07:16:43.000000 usda-0.0.19/src/usda/models/_label_encoder.py
+-rw-rw-rw-   0        0        0     1022 2022-10-25 01:02:56.000000 usda-0.0.19/src/usda/models/_neighbors.py
+-rw-rw-rw-   0        0        0     1422 2022-10-31 08:30:25.000000 usda-0.0.19/src/usda/models/_random_forest_classifier.py
+-rw-rw-rw-   0        0        0    11923 2022-10-28 11:44:45.000000 usda-0.0.19/src/usda/models/_sir_model.py
+-rw-rw-rw-   0        0        0     3200 2022-10-30 07:33:05.000000 usda-0.0.19/src/usda/models/_superpixel_segmentation.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.400519 usda-0.0.19/src/usda/net/
+-rw-rw-rw-   0        0        0      120 2023-04-05 02:07:48.000000 usda-0.0.19/src/usda/net/_.py
+-rw-rw-rw-   0        0        0      856 2023-04-05 02:18:09.000000 usda-0.0.19/src/usda/net/__init__.py
+-rw-rw-rw-   0        0        0    28490 2023-04-05 02:16:39.000000 usda-0.0.19/src/usda/net/_networks_pix2pix.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.411519 usda-0.0.19/src/usda/network/
+-rw-rw-rw-   0        0        0      404 2023-04-01 07:37:21.000000 usda-0.0.19/src/usda/network/__init__.py
+-rw-rw-rw-   0        0        0     4050 2023-03-10 11:37:13.000000 usda-0.0.19/src/usda/network/_g_drawing.py
+-rw-rw-rw-   0        0        0     2896 2023-04-01 07:46:50.000000 usda-0.0.19/src/usda/network/_pt_pattern.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.436519 usda-0.0.19/src/usda/pattern_signature/
+-rw-rw-rw-   0        0        0     1340 2023-03-24 06:18:07.000000 usda-0.0.19/src/usda/pattern_signature/__init__.py
+-rw-rw-rw-   0        0        0     5975 2023-02-12 02:57:51.000000 usda-0.0.19/src/usda/pattern_signature/_distance_metric.py
+-rw-rw-rw-   0        0        0     1182 2023-02-09 14:05:16.000000 usda-0.0.19/src/usda/pattern_signature/_grid_neighbors_xy_finder.py
+-rw-rw-rw-   0        0        0     8778 2023-02-19 14:00:29.000000 usda-0.0.19/src/usda/pattern_signature/_img_region_growing.py
+-rw-rw-rw-   0        0        0    20197 2023-02-19 13:21:56.000000 usda-0.0.19/src/usda/pattern_signature/_pattern_module.py
+-rw-rw-rw-   0        0        0     7729 2023-03-24 07:51:30.000000 usda-0.0.19/src/usda/pattern_signature/_signature.py
+-rw-rw-rw-   0        0        0     3191 2023-02-12 09:54:49.000000 usda-0.0.19/src/usda/pattern_signature/_signature2distance_integration.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.454520 usda-0.0.19/src/usda/stats/
+-rw-rw-rw-   0        0        0     1011 2022-10-24 05:16:26.000000 usda-0.0.19/src/usda/stats/__init__.py
+-rw-rw-rw-   0        0        0     3501 2022-10-20 03:25:19.000000 usda-0.0.19/src/usda/stats/_descriptive_stats.py
+-rw-rw-rw-   0        0        0     2233 2022-10-22 02:45:57.000000 usda-0.0.19/src/usda/stats/_kde.py
+-rw-rw-rw-   0        0        0      778 2022-10-20 03:57:18.000000 usda-0.0.19/src/usda/stats/_outlier.py
+-rw-rw-rw-   0        0        0    10793 2022-10-24 05:19:28.000000 usda-0.0.19/src/usda/stats/_regression.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.458519 usda-0.0.19/src/usda/tools/
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.463521 usda-0.0.19/src/usda/tools/DL_layers_visualizer/
+-rw-rw-rw-   0        0        0     1064 2023-04-08 15:24:36.000000 usda-0.0.19/src/usda/tools/DL_layers_visualizer/DL_layers_visualizer.py
+-rw-rw-rw-   0        0        0      196 2023-04-07 11:25:06.000000 usda-0.0.19/src/usda/tools/DL_layers_visualizer/__init__.py
+-rw-rw-rw-   0        0        0      196 2023-04-06 11:45:47.000000 usda-0.0.19/src/usda/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.493521 usda-0.0.19/src/usda/utils/
+-rw-rw-rw-   0        0        0     1073 2023-02-24 02:03:24.000000 usda-0.0.19/src/usda/utils/__init__.py
+-rw-rw-rw-   0        0        0     1497 2022-10-17 01:46:32.000000 usda-0.0.19/src/usda/utils/_bunch.py
+-rw-rw-rw-   0        0        0     5197 2022-10-18 07:06:26.000000 usda-0.0.19/src/usda/utils/_coordinate_transformation.py
+-rw-rw-rw-   0        0        0     3970 2023-02-23 09:40:47.000000 usda-0.0.19/src/usda/utils/_df_process.py
+-rw-rw-rw-   0        0        0     2938 2022-10-17 01:57:17.000000 usda-0.0.19/src/usda/utils/_displayable_path.py
+-rw-rw-rw-   0        0        0     1857 2022-10-26 01:31:31.000000 usda-0.0.19/src/usda/utils/_file_structure.py
+-rw-rw-rw-   0        0        0     3992 2023-02-24 02:02:45.000000 usda-0.0.19/src/usda/utils/_gadgets.py
+-rw-rw-rw-   0        0        0      606 2022-10-22 00:35:56.000000 usda-0.0.19/src/usda/utils/_operating_time.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.505519 usda-0.0.19/src/usda/weight/
+-rw-rw-rw-   0        0        0     1014 2023-03-03 07:14:29.000000 usda-0.0.19/src/usda/weight/__init__.py
+-rw-rw-rw-   0        0        0    38486 2023-03-03 07:13:35.000000 usda-0.0.19/src/usda/weight/_decision_rule.py
+-rw-rw-rw-   0        0        0     2745 2023-02-23 12:30:34.000000 usda-0.0.19/src/usda/weight/_entropy_weight.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.066521 usda-0.0.19/src/usda.egg-info/
+-rw-rw-rw-   0        0        0     1563 2023-04-09 05:18:42.000000 usda-0.0.19/src/usda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5385 2023-04-09 05:18:42.000000 usda-0.0.19/src/usda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 05:18:42.000000 usda-0.0.19/src/usda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-10-16 07:33:50.000000 usda-0.0.19/src/usda.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       55 2023-04-09 05:18:42.000000 usda-0.0.19/src/usda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-09 05:18:42.000000 usda-0.0.19/src/usda.egg-info/top_level.txt
```

### Comparing `usda-0.0.18/LICENSE` & `usda-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/PKG-INFO` & `usda-0.0.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usda
-Version: 0.0.18
+Version: 0.0.19
 Summary: A set of python modules for Urban Spatial Data Analysis Method (USDA)
 Home-page: https://richiebao.github.io/USDA_PyPI
 Download-URL: https://github.com/richieBao/USDA_PyPI
 Maintainer: Richie Bao
 Maintainer-email: richiebao@outlook.com
 License: new BSD
 Project-URL: Documentation, https://richiebao.github.io/USDA_PyPI
```

### Comparing `usda-0.0.18/setup.py` & `usda-0.0.19/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 Created on Sun Aug 21 14:57:02 2022
 
 @author: Richie Bao-caDesign设计(cadesign.cn)
 
 python setup.py sdist
 twine upload dist/usda-0.0.15.tar.gz
 """
-from setuptools import setup,find_packages,find_namespace_packages
+# Extension,setup,
+from setuptools import find_packages,find_namespace_packages,setup
 import src.usda._min_dependencies as min_deps 
 
 DISTNAME="usda"
 MAINTAINER="Richie Bao"
 MAINTAINER_EMAIL="richiebao@outlook.com"
 DESCRIPTION="A set of python modules for Urban Spatial Data Analysis Method (USDA)"
 LICENSE="new BSD"
```

### Comparing `usda-0.0.18/src/usda/_min_dependencies.py` & `usda-0.0.19/src/usda/_min_dependencies.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_process/__init__.py` & `usda-0.0.19/src/usda/data_process/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,25 +13,32 @@
 from ._raster_dataprocess import raster_clip
 from ._image_pixel_sampling_zoom import image_pixel_sampling
 
 from ._tiler_calculation import deg2num
 from ._tiler_calculation import centroid
 from ._kitti_dataprocess import KITTI_info2sqlite
 
-from ._quadrat import pt_coordi_transform
+from ._naip_dataprocess import remove_bbox
+from ._naip_dataprocess import naip_preprocess
+from ._naip_dataprocess import naip_rd
+from ._naip_dataprocess import naip_dividedby255
 
 __all__ = [
     "shpPolygon2OsmosisTxt",
     "osmHandler",
     "save_osm",
     "pts2raster",
     "raster_clip",
     "image_pixel_sampling",
     "deg2num",
     "centroid",
     "KITTI_info2sqlite",
     "LandsatMTL_info",
     "pt_coordi_transform",
+    "remove_bbox",
+    "naip_preprocess",
+    "naip_dividedby255",
+    "naip_rd",
     ]
```

### Comparing `usda-0.0.18/src/usda/data_process/_geoinfodata_conversion.py` & `usda-0.0.19/src/usda/data_process/_geoinfodata_conversion.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_process/_image_pixel_sampling_zoom.py` & `usda-0.0.19/src/usda/data_process/_image_pixel_sampling_zoom.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_process/_kitti_dataprocess.py` & `usda-0.0.19/src/usda/data_process/_kitti_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_process/_landsat_dataprocess.py` & `usda-0.0.19/src/usda/data_process/_landsat_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_process/_osm_dataprocess.py` & `usda-0.0.19/src/usda/data_process/_osm_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_process/_raster_dataprocess.py` & `usda-0.0.19/src/usda/data_process/_raster_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_process/_tiler_calculation.py` & `usda-0.0.19/src/usda/data_process/_tiler_calculation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/__init__.py` & `usda-0.0.19/src/usda/data_visualization/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 from ._imgs_layout_show import imgs_layoutShow_FPList
 from ._img_theme_color import img_theme_color
 from ._img_theme_color import themeColor_impression
 from ._chart_custom import boxplot_custom
 from ._chart_custom import  histogram_3d
 
 from ._gdf_plot import gdf_plot_annotate
+from ._panorama_show import sphere_panorama_label
+
+from ._plot_single_function import plot_single_function
 
 
 __all__ = [
     "plotly_table",
     "print_html",
     "probability_graph",
     "demo_con_style",
@@ -80,14 +83,16 @@
     "imgs_compression_cv",
     "boxplot_custom",
     "SIFT_detection",
     "feature_matching",
     "segMasks_layoutShow",
     "histogram_3d",
     "gdf_plot_annotate",
+    "sphere_panorama_label",
+    "plot_single_function",
     ]
```

### Comparing `usda-0.0.18/src/usda/data_visualization/_chart_custom.py` & `usda-0.0.19/src/usda/data_visualization/_chart_custom.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/_colors.py` & `usda-0.0.19/src/usda/data_visualization/_colors.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/_dynamic_streetView_visual_perception.py` & `usda-0.0.19/src/usda/data_visualization/_dynamic_streetView_visual_perception.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/_gdf_plot.py` & `usda-0.0.19/src/usda/data_visualization/_gdf_plot.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/_gif_show.py` & `usda-0.0.19/src/usda/data_visualization/_gif_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/_graphic_drawing.py` & `usda-0.0.19/src/usda/data_visualization/_graphic_drawing.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/_image_process.py` & `usda-0.0.19/src/usda/data_visualization/_image_process.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/_img_feature_extraction.py` & `usda-0.0.19/src/usda/data_visualization/_img_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/_img_theme_color.py` & `usda-0.0.19/src/usda/data_visualization/_img_theme_color.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/_imgs_layout_show.py` & `usda-0.0.19/src/usda/data_visualization/_imgs_layout_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/_imgs_show.py` & `usda-0.0.19/src/usda/data_visualization/_imgs_show.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,25 +89,26 @@
     '''    
     args=dict(figsize=(10,10),
               cmap='Accent',
               text_color='white',
               dtype='int',
               random_seed=None,
               fontsize=5,
+              norm=None,
               )    
     args.update(kwargs)
     
     if args['random_seed']:
         np.random.seed(args['random_seed'])
         cmap=matplotlib.colors.ListedColormap (np.random.rand(256,3))
     else:
-        cmap=args['cmap']
+        cmap=args['cmap']        
     
     fig,ax=plt.subplots(1,1,figsize=args['figsize']) 
-    ax.imshow(array_2d,cmap=cmap)
+    ax.imshow(array_2d,cmap=cmap,norm=args['norm'])
     
     if label:
         nx,ny=array_2d.shape
         x=np.linspace(0, nx-1, nx)
         y=np.linspace(0, ny-1, ny)
         xv, yv=np.meshgrid(x, y)
```

### Comparing `usda-0.0.18/src/usda/data_visualization/_knee_line_graph.py` & `usda-0.0.19/src/usda/data_visualization/_knee_line_graph.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/_moving_average_inflection.py` & `usda-0.0.19/src/usda/data_visualization/_moving_average_inflection.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/_raster_percentile_slider.py` & `usda-0.0.19/src/usda/data_visualization/_raster_percentile_slider.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/_raster_show.py` & `usda-0.0.19/src/usda/data_visualization/_raster_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/_stats_charts.py` & `usda-0.0.19/src/usda/data_visualization/_stats_charts.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/_superpixel_segmentation_show.py` & `usda-0.0.19/src/usda/data_visualization/_superpixel_segmentation_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/_table_show.py` & `usda-0.0.19/src/usda/data_visualization/_table_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/_tile_show.py` & `usda-0.0.19/src/usda/data_visualization/_tile_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/data_generator.py` & `usda-0.0.19/src/usda/data_visualization/data_generator.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/data_visualization/knee_locator.py` & `usda-0.0.19/src/usda/data_visualization/knee_locator.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/database/__init__.py` & `usda-0.0.19/src/usda/database/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,26 +4,34 @@
 
 @author: Richie Bao-caDesign设计(cadesign.cn)
 """
 from ._database import df2SQLite
 from ._database import SQLite2df
 from ._database import gpd2postSQL
 from ._database import postSQL2gpd
+from ._database import df2postSQL
+from ._database import postSQL2df
+
 
 from ._data_format_conversion import csv2df
 from ._data_format_conversion import poi_csv2GeoDF_batch
+from ._data_format_conversion import json2gdf
+
 from ._read_matlab_fig import read_MatLabFig_type_A
 from ._data_file_rw import save_as_json
 
 __all__=[
     "df2SQLite",    
     "SQLite2df",
     "gpd2postSQL",
     "postSQL2gpd",
     "csv2df",
     "poi_csv2GeoDF_batch",
     "read_MatLabFig_type_A",
     "save_as_json",
+    "df2postSQL",
+    "postSQL2df",
+    "json2gdf",
     ]
```

### Comparing `usda-0.0.18/src/usda/database/_data_file_rw.py` & `usda-0.0.19/src/usda/database/_data_file_rw.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/database/_data_format_conversion.py` & `usda-0.0.19/src/usda/database/_data_format_conversion.py`

 * *Files 13% similar despite different names*

```diff
@@ -89,7 +89,33 @@
     poisInAll_gdf2shp=poisInAll_gdf.reset_index() # 不指定level参数，例如Level=0，会把多重索引中的所有索引转换为列
     poisInAll_gdf2shp.rename(columns={
         'location_lat':'lat', 'location_lng':'lng',
         'detail_info_tag':'tag','detail_info_overall_rating':'rating', 'detail_info_price':'price'},inplace=True)
     poisInAll_gdf2shp.to_file(save_path['shp'],encoding='utf-8')
         
     return poisInAll_gdf
+
+def json2gdf(json_fn,numeric_columns=None,epsg=None):
+    '''
+    读取.geojson(json)文件为GeoDataFrame格式文件，选择配置投影
+
+    Parameters
+    ----------
+    json_fn : string
+        文件路径.
+    epsg : int, optional
+        坐标投影系统，epsg编号. The default is None.
+
+    Returns
+    -------
+    gdf : GeoDataFrmae
+        转换后的GeoDataFrame格式文件.
+
+    '''    
+    gdf=gpd.read_file(json_fn)
+    if epsg:
+        gdf.to_crs(epsg,inplace=True)   
+    print("fields_{}".format(gdf.columns))    
+    if numeric_columns:
+        gdf=gdf.astype(numeric_columns)
+
+    return gdf
```

### Comparing `usda-0.0.18/src/usda/database/_database.py` & `usda-0.0.19/src/usda/database/_database.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # -*- coding: utf-8 -*-
 """
 Created on Thu Oct 13 19:00:53 2022
 
 @author: richie bao
 """
-from sqlalchemy import create_engine
+from sqlalchemy import create_engine,text
 import pandas as pd
 import geopandas as gpd
 
-
 def df2SQLite(db_fp, df, table_name, method='fail'):    
     '''
     function - 把pandas DataFrame格式数据写入数据库（同时创建表）
     
     Paras:
         db_fp - 数据库链接；string
         df - 待写入数据库的DataFrame格式数据；DataFrame
@@ -75,15 +74,45 @@
         geom_col='geometry' - 几何对象，常规默认字段为'geometry'；string
         **kwargs - 连接数据库相关信息，包括myusername（数据库的用户名），mypassword（用户密钥），mydatabase（数据库名）；string
     Returns:
         读取的表数据；GeoDataFrame
     '''
 
     engine=create_engine("postgresql://{myusername}:{mypassword}@localhost:5432/{mydatabase}".format(myusername=kwargs['myusername'],mypassword=kwargs['mypassword'],mydatabase=kwargs['mydatabase']))  
-    gdf=gpd.read_postgis(table_name, con=engine,geom_col=geom_col)
+    sql=f"SELECT * FROM {table_name}"
+    gdf=gpd.read_postgis(sql=text(sql), con=engine.connect(),geom_col=geom_col)
     print("_"*50)
     print('The data has been read from PostgreSQL database. The table name is {}.'.format(table_name))    
     return gdf          
                 
-        
+def df2postSQL(df,table_name,if_exists='replace',**kwargs):
+    '''
+    function - 将DataFrame格式数据写入PostgreSQL数据库
+    
+    Paras:
+        df - DataFrame格式数据
+        table_name - 写入数据库中的表名
+        **kwargs - 连接数据库相关信息，包括myusername（数据库的用户名），mypassword（用户密钥），mydatabase（数据库名）
+    '''    
+    #The URI should start with postgresql:// instead of postgres://. SQLAlchemy used to accept both, but has removed support for the postgres name.
+    engine=create_engine("postgresql://{myusername}:{mypassword}@localhost:5432/{mydatabase}".format(myusername=kwargs['myusername'],mypassword=kwargs['mypassword'],mydatabase=kwargs['mydatabase']))  
+    conn=engine.connect()
+    df.to_sql(table_name, con=conn, if_exists=if_exists,index=False)    
+    # gdf.to_postgis(table_name, con=engine, if_exists='replace', index=False,)  
+    print("_"*50)    
+    print('The GeoDataFrame has been written to the PostgreSQL database.The table name is {}.'.format(table_name))   
 
+def postSQL2df(table_name,**kwargs):    
+    '''
+    function - 读取PostgreSQL数据库中的表为DataFrame格式数据
     
+    Paras:
+        table_name - 待读取数据库中的表名
+        **kwargs - 连接数据库相关信息，包括myusername（数据库的用户名），mypassword（用户密钥），mydatabase（数据库名）
+    '''    
+    engine=create_engine("postgresql://{myusername}:{mypassword}@localhost:5432/{mydatabase}".format(myusername=kwargs['myusername'],mypassword=kwargs['mypassword'],mydatabase=kwargs['mydatabase']))  
+    conn=engine.connect()
+    df=pd.read_sql('SELECT * FROM {}'.format(table_name), conn)
+
+    print("_"*50)
+    print('The data has been read from PostgreSQL database. The table name is {}.'.format(table_name))    
+    return df
```

### Comparing `usda-0.0.18/src/usda/database/_read_matlab_fig.py` & `usda-0.0.19/src/usda/database/_read_matlab_fig.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/datasets/__init__.py` & `usda-0.0.19/src/usda/datasets/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 from ._base import load_bowling_contest_cartoon_statistic
 from ._base import load_test_score_cartoon_statistic
 from ._base import baiduPOI_dataCrawler
 from ._base import baiduPOI_dataCrawler_circle
 from ._base import baiduPOI_batchCrawler
 from ._base import generate_categorical_2darray
 from ._base import load_evaluation_criteria_raw_values
+from ._base import load_sustainability_attributes4electricity_generation_tech
+from ._base import load_microclimate_in_office_rooms
+from ._base import load_jisperveld_data
 
 from ._dataset_info import KITTI_info
 from ._dataset_info import KITTI_info_gap
 from ._rs_image import Sentinel2_bandFNs
 from ._kml_info import kml_coordiExtraction
 from ._img_info import img_exif_info
 
@@ -31,10 +34,13 @@
     "KITTI_info",
     "KITTI_info_gap",
     "Sentinel2_bandFNs",
     "kml_coordiExtraction",
     "img_exif_info",
     "generate_categorical_2darray",
     "load_evaluation_criteria_raw_values",
+    "load_sustainability_attributes4electricity_generation_tech",
+    "load_microclimate_in_office_rooms",
+    'load_jisperveld_data'
     ]
```

### Comparing `usda-0.0.18/src/usda/datasets/_base.py` & `usda-0.0.19/src/usda/datasets/_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -361,13 +361,107 @@
 
     '''
     
     data_file_name="evaluation_criteria_raw_values.pickle" 
     with resources.open_binary(data_module,data_file_name) as data_file:
         evaluation_criteria_raw_values=pd.read_pickle(data_file)  
     return Bunch(data=evaluation_criteria_raw_values, name=data_file_name)
- 
+
+def load_sustainability_attributes4electricity_generation_tech(data_module=DATA_MODULE):
+    '''
+    来自于： Şahin, M. A comprehensive analysis of weighting and multicriteria methods in the context of sustainable energy. International Journal of Environmental Science and Technology 18, 1591–1616 (2021).
+
+    Parameters
+    ----------
+    data_module : string
+        数据所在文件夹. The default is DATA_MODULE.
+
+    Returns
+    -------
+    TYPE
+        DESCRIPTION.
+
+    '''
+    
+    data_file_name="sustainability_attributes4electricity_generation_tech.pickle" 
+    with resources.open_binary(data_module,data_file_name) as data_file:
+        data=pd.read_pickle(data_file)  
+    return Bunch(data=data, name=data_file_name) 
+
+def load_microclimate_in_office_rooms(data_module=DATA_MODULE):
+    data_file_name="microclimate_in_office_rooms.pickle" 
+    with resources.open_binary(data_module,data_file_name) as data_file:
+        data=pd.read_pickle(data_file)  
+    measurement_units=[r'm3/h', r'%', r'°C', r'lx', r'm/s', r'°C']
+    optimisation_direction=[r'max',r'max',r'max',r'max',r'min',r'min']
+    weight_of_criteria=[0.21, 0.16, 0.26, 0.17, 0.12, 0.08] 
+    optimal_value=[15, 50, 24.5, 400, 0.05, 5] 
+    
+    return Bunch(data=data, 
+                 name=data_file_name,
+                 measurement_units=measurement_units,
+                 optimisation_direction=optimisation_direction,
+                 weight_of_criteria=weight_of_criteria,
+                 optimal_value=optimal_value) 
+    
+def load_jisperveld_data(data_module=DATA_MODULE):
+    '''
+    来自于： Janssen, R., van Herwijnen, M., Stewart, T. J. & Aerts, J. C. J. H. Multiobjective decision support for land-use planning. Environ Plann B Plann Des 35, 740–756 (2008).
+
+    Parameters
+    ----------
+    data_module : string
+        数据所在文件夹. The default is DATA_MODULE.
+
+    Returns
+    -------
+    TYPE
+        DESCRIPTION.
+
+    '''    
+    
+    data_file_name="jisperveld_data.pickle" 
+    with resources.open_binary(data_module,data_file_name) as data_file:
+        data=pd.read_pickle(data_file)     
+        
+    nature_recreation_vals={'nature_value':{'intensive_agriculture':4, 'extensive_agriculture':'nature_vals', 'residence':3,'industry':1,'recreation_day_trips':5,'recreation_overnight':5,'wet_natural_area':'nature_vals','water_recreational_use':7, 'water_limited_access':'nature_vals'},
+                            'recreational_value':{'intensive_agriculture':6, 'extensive_agriculture':'nature_vals', 'residence':3,'industry':1,'recreation_day_trips':'recreation_b','recreation_overnight':'recreation_c','wet_natural_area':7,'water_recreational_use':'recreation_b', 'water_limited_access':1}}
+    nature_recreation_vals_df=pd.DataFrame(nature_recreation_vals)     
+    
+    
+    lu_conversion_cost=np.array([[0,-75,150,150,-225,0,-150,-300,-300],
+          [75,0,150,150,-150,75,-75,-225,-225],
+          [np.nan,np.nan,0,np.nan,-10000,-10000,np.nan,np.nan,np.nan],
+          [np.nan,np.nan,np.nan,0,-10000,-10000,np.nan,np.nan,np.nan],
+          [150,75,3,300,0,150,0,-150,-150],
+          [0,-75,150,150,-150,0,-150,-300,-230],
+          [np.nan,75,225,225,-75,150,0,-75,-75],
+          [100,100,np.nan,np.nan,np.nan,np.nan,0,0,15],
+          [100,100,np.nan,np.nan,np.nan,np.nan,0,0,0]])
+    cols=['intensive_agriculture', 'extensive_agriculture','residence', 'industry','recreation_day_trips','recreation_overnight','wet_natural_area','water_recreational_use', 'water_limited_access']
+    lu_conversion_cost_df=pd.DataFrame(lu_conversion_cost,index=cols,columns=cols)
+            
+    return Bunch(
+        lu=data['lu'],
+        nature_vals=data['nature_vals'],
+        recreation_b=data['recreation_b'],
+        recreation_c=data['recreation_c'],
+        fixed_LU=data['fixed_LU'],
+        lu_name={1:'intensive_agriculture',
+                 2:'extensive_agriculture',
+                 3:'residence',
+                 4:'industry',
+                 5:'recreation_day_trips',
+                 6:'recreation_overnight',
+                 7:'wet_natural_area',
+                 8:'water_recreational_use',
+                 9:'water_limited_access'},        
+        nature_recreation_vals=nature_recreation_vals_df,
+        lu_conversion_cost=lu_conversion_cost_df,
+        data_name_lst=['lu','recreation_b','recreation_c','fixed_LU','nature_recreation_vals','lu_conversion_cost'],)
+        
 
 if __name__=="__main__":
     pass
     # sales_data_cartoon_databas=load_sales_data_cartoon_database()
     # df=ArithmeticErrorload_evaluation_criteria_raw_values
+    # load_jisperveld_data()
```

### Comparing `usda-0.0.18/src/usda/datasets/_dataset_info.py` & `usda-0.0.19/src/usda/datasets/_dataset_info.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/datasets/_img_info.py` & `usda-0.0.19/src/usda/datasets/_img_info.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/datasets/_kml_info.py` & `usda-0.0.19/src/usda/datasets/_kml_info.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/datasets/_rs_image.py` & `usda-0.0.19/src/usda/datasets/_rs_image.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/datasets/data/bowling_contest_cartoon_statistic.pickle` & `usda-0.0.19/src/usda/datasets/data/bowling_contest_cartoon_statistic.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/datasets/data/evaluation_criteria_raw_values.pickle` & `usda-0.0.19/src/usda/datasets/data/evaluation_criteria_raw_values.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/datasets/data/ramen_price_cartoon_statistic.pickle` & `usda-0.0.19/src/usda/datasets/data/ramen_price_cartoon_statistic.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/datasets/data/sales_data_cartoon_database.pickle` & `usda-0.0.19/src/usda/datasets/data/sales_data_cartoon_database.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/datasets/data/test_score_cartoon_statistic.pickle` & `usda-0.0.19/src/usda/datasets/data/test_score_cartoon_statistic.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/geodata_process/_raster_dataprocess.py` & `usda-0.0.19/src/usda/geodata_process/_raster_dataprocess.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 @author: richie bao
 """
 import rasterio as rio
 from rasterio.windows import Window
 from osgeo import gdal, ogr, osr
 from rasterio.warp import calculate_default_transform, reproject, Resampling
 
+import rasterio,glob,os
+from rasterio.merge import merge
+
 def rio_read_subset(fn,lbNrt_coordinates):
     '''
     指定左下角和右上角坐标，部分读取栅格数据
 
     Parameters
     ----------
     fn : string
@@ -121,7 +124,75 @@
                     source=rio.band(src, i),
                     destination=rio.band(dst, i),
                     src_transform=src.transform,
                     src_crs=src.crs,
                     dst_transform=transform,
                     dst_crs=dst_crs,
                     resampling=Resampling.nearest)         
+
+def raster_mosaic(dir_path,out_fp,dtype=None):
+    '''
+    function - 合并多个栅格为一个
+    
+    Paras:
+        dir_path - 栅格根目录
+        out-fp - 保存路径
+    
+    return:
+        out_trans - 返回变换信息
+    '''
+    
+    #迁移rasterio提供的定义数组最小数据类型的函数
+    def get_minimum_int_dtype(values):
+        """
+        Uses range checking to determine the minimum integer data type required
+        to represent values.
+
+        :param values: numpy array
+        :return: named data type that can be later used to create a numpy dtype
+        """
+
+        min_value = values.min()
+        max_value = values.max()
+
+        if min_value >= 0:
+            if max_value <= 255:
+                return rasterio.uint8
+            elif max_value <= 65535:
+                return rasterio.uint16
+            elif max_value <= 4294967295:
+                return rasterio.uint32
+        elif min_value >= -32768 and max_value <= 32767:
+            return rasterio.int16
+        elif min_value >= -2147483648 and max_value <= 2147483647:
+            return rasterio.int32
+    
+    search_criteria = "*.tif" #搜寻所要合并的栅格.tif文件
+    fp_pattern=os.path.join(dir_path, search_criteria)
+    fps=glob.glob(fp_pattern) #使用glob库搜索指定模式的文件
+    src_files_to_mosaic=[]
+    for fp in fps:
+        src=rasterio.open(fp)
+        src_files_to_mosaic.append(src)    
+    mosaic,out_trans=merge(src_files_to_mosaic)  #merge函数返回一个栅格数组，以及转换信息   
+    
+    #获得元数据
+    out_meta=src.meta.copy()
+    #更新元数据
+    if dtype:
+        data_type=dtype
+    else:
+        data_type=get_minimum_int_dtype(mosaic)
+    out_meta.update({"driver": "GTiff",
+                     "height": mosaic.shape[1],
+                     "width": mosaic.shape[2],
+                     "transform": out_trans,
+                     #通过压缩和配置存储类型，减小存储文件大小
+                     "compress":'lzw',
+                     "dtype":data_type, 
+                      }
+                    )      
+    
+    with rasterio.open(out_fp, "w", **out_meta) as dest:
+        dest.write(mosaic.astype(data_type))     
+    
+    return out_trans
```

### Comparing `usda-0.0.18/src/usda/indices/_rs_indices.py` & `usda-0.0.19/src/usda/indices/_rs_indices.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/maths/__init__.py` & `usda-0.0.19/src/usda/maths/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/maths/_algebra.py` & `usda-0.0.19/src/usda/maths/_algebra.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/maths/_geometric_calculation.py` & `usda-0.0.19/src/usda/maths/_geometric_calculation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/models/__init__.py` & `usda-0.0.19/src/usda/models/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 from ._bow_feature_builder import feature_builder_BOW
 from ._label_encoder import df_multiColumns_LabelEncoder
 from ._entropy import entropy_compomnent
 from ._entropy import IG
 from ._decision_tree import decisionTree_structure
 from ._random_forest_classifier import ERF_trainer
 from ._image_tag_extractor import ImageTag_extractor
+from ._clustering import clustering_minibatchkmeans_selectkbest_ns
+from ._global_local_autocorrelation import moran_local_autocorrelation_gdf
 
 __all__=[
     "k_neighbors_entire",
     "PolynomialFeatures_regularization",
     "dim1_convolution_SubplotAnimation",
     "G_T_type_1",
     "F_T_type_1",
@@ -45,11 +47,13 @@
     "df_multiColumns_LabelEncoder",
     "entropy_compomnent",
     "IG",
     "decisionTree_structure",
     "ERF_trainer",
     "ImageTag_extractor",
     "SIR_spatialPropagating",
+    "clustering_minibatchkmeans_selectkbest_ns",
+    "moran_local_autocorrelation_gdf",
     ]
```

### Comparing `usda-0.0.18/src/usda/models/_bow_feature_builder.py` & `usda-0.0.19/src/usda/models/_bow_feature_builder.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/models/_computational_performance.py` & `usda-0.0.19/src/usda/models/_computational_performance.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/models/_curve_segmentation.py` & `usda-0.0.19/src/usda/models/_curve_segmentation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/models/_decision_tree.py` & `usda-0.0.19/src/usda/models/_decision_tree.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/models/_dim1_convolution.py` & `usda-0.0.19/src/usda/models/_dim1_convolution.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/models/_entropy.py` & `usda-0.0.19/src/usda/models/_entropy.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/models/_image_tag_extractor.py` & `usda-0.0.19/src/usda/models/_image_tag_extractor.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/models/_label_encoder.py` & `usda-0.0.19/src/usda/models/_label_encoder.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/models/_neighbors.py` & `usda-0.0.19/src/usda/models/_neighbors.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/models/_random_forest_classifier.py` & `usda-0.0.19/src/usda/models/_random_forest_classifier.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/models/_sir_model.py` & `usda-0.0.19/src/usda/models/_sir_model.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/models/_superpixel_segmentation.py` & `usda-0.0.19/src/usda/models/_superpixel_segmentation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/pattern_signature/__init__.py` & `usda-0.0.19/src/usda/pattern_signature/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 @author: richie bao
 """
 from ._signature import lexsort_based
 from ._signature import class_clumpSize_histogram
 from ._signature import class_co_occurrence
 from ._signature import class_decomposition
+from ._signature import group_bins_histogram
 from ._grid_neighbors_xy_finder import GridNghFinder
 
 from ._distance_metric import Distances
 from ._signature2distance_integration import signature2distance_integrating
 from ._pattern_module import pattern_search
 from ._pattern_module import pattern_compare
 # from ._pattern_module import pattern_reference_distance
@@ -31,12 +32,13 @@
     "pattern_search",
     "pattern_compare",
     # "pattern_reference_distance", # deprecated
     "Pattern_segment_regionGrow",
     "Categorical_data_region_growing",
     "Img_regionGrow",
     "Img_gray_regionGrow",
+    "group_bins_histogram",
     ]
```

### Comparing `usda-0.0.18/src/usda/pattern_signature/_distance_metric.py` & `usda-0.0.19/src/usda/pattern_signature/_distance_metric.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/pattern_signature/_grid_neighbors_xy_finder.py` & `usda-0.0.19/src/usda/pattern_signature/_grid_neighbors_xy_finder.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/pattern_signature/_img_region_growing.py` & `usda-0.0.19/src/usda/pattern_signature/_img_region_growing.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/pattern_signature/_pattern_module.py` & `usda-0.0.19/src/usda/pattern_signature/_pattern_module.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/pattern_signature/_signature.py` & `usda-0.0.19/src/usda/pattern_signature/_signature.py`

 * *Files 12% similar despite different names*

```diff
@@ -174,8 +174,40 @@
         tags_classified_df=pd.DataFrame.from_records(tags_classified_lst)       
         tags_classified_frequency_df=pd.DataFrame({col:tags_classified_df[col].value_counts().sort_index(ascending=True).to_dict() for col in tags_classified_df.columns})
         tags_classified_all_levels[i]=tags_classified_frequency_df
    
     tags_classified_all_levels_concat=pd.concat(tags_classified_all_levels)
     
     return tags_classified_all_levels_concat.fillna(0)
+
+def group_bins_histogram(df,cols,by,bins):
+    '''
+    统计给定列（属性），给定bin的频数（直方图）
+
+    Parameters
+    ----------
+    df : DataFrame
+        数据.
+    cols : list[str]
+        用于计算的列名，含用于分组的列名.
+    by : str
+        用于分组的列名.
+    bins : list[numerical]
+        列表区间，划分的宽度为(a,b].
+
+    Returns
+    -------
+    cluster_bins_histogram_dict : dict[]
+        按组按bin统计频数结果，键为分组值，值为DataFrame，含个区间的频数.
+
+    '''
+    
+    cluster_num=df[by].value_counts().to_dict()
+    cluster_bins=df[cols].groupby(by, group_keys=True).apply(lambda x:{i:pd.cut(x[i],bins).value_counts() for i in x.columns})
+    cluster_bins_histogram_dict={}
+    for idx,row in cluster_bins.iteritems():
+        bins_fre_df=pd.DataFrame(row)
+        bins_fre_df.drop(columns=[by],inplace=True)
+        cluster_bins_histogram_dict[idx]=bins_fre_df/cluster_num[idx]        
+        
+    return cluster_bins_histogram_dict
```

### Comparing `usda-0.0.18/src/usda/pattern_signature/_signature2distance_integration.py` & `usda-0.0.19/src/usda/pattern_signature/_signature2distance_integration.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/stats/__init__.py` & `usda-0.0.19/src/usda/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/stats/_descriptive_stats.py` & `usda-0.0.19/src/usda/stats/_descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/stats/_kde.py` & `usda-0.0.19/src/usda/stats/_kde.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/stats/_outlier.py` & `usda-0.0.19/src/usda/stats/_outlier.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/stats/_regression.py` & `usda-0.0.19/src/usda/stats/_regression.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/utils/__init__.py` & `usda-0.0.19/src/usda/utils/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 from ._operating_time import start_time
 from ._operating_time import duration
 
 from ._gadgets import variable_name
 from ._gadgets import lst_index_split
 from ._gadgets import flatten_lst
 from ._gadgets import nestedlst_insert
+from ._gadgets import AttrDict
 
 from ._df_process import complete_dataframe_rowcols
 from ._df_process import xy_to_matrix
 from ._df_process import matrix_to_xy
+from ._df_process import df_normalize
 
 __all__=[
     "Bunch",
     "DisplayablePath",
     "filePath_extraction",
     "fp_sort",
     "start_time",
@@ -32,8 +34,11 @@
     "variable_name",
     "lst_index_split",
     "flatten_lst",
     "nestedlst_insert",
     "complete_dataframe_rowcols",
     "xy_to_matrix",
     "matrix_to_xy",
-    ]
+    "df_normalize",
+    "AttrDict",
+    ]
+
```

### Comparing `usda-0.0.18/src/usda/utils/_bunch.py` & `usda-0.0.19/src/usda/utils/_bunch.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/utils/_coordinate_transformation.py` & `usda-0.0.19/src/usda/utils/_coordinate_transformation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/utils/_df_process.py` & `usda-0.0.19/src/usda/utils/_df_process.py`

 * *Files 23% similar despite different names*

```diff
@@ -99,8 +99,33 @@
     xy=(
         df.where(bool_index).stack().reset_index()
         if reset_index
         else df.where(bool_index).stack()
     )
     if reset_index:
         xy.columns=columns or ["row", "col", "val"]
-    return xy
+    return xy
+
+def df_normalize(df,feature_range=(-1, 1)):
+    '''
+    对DataFrame格式数据，逐列执行标准化
+    Parameters
+    ----------
+    df : DataFrame
+        待执行标准化的数据.
+    feature_range : tuple, optional
+        标准化后的数值范围. The default is (-1, 1).
+    Returns
+    -------
+    result : DataFrame
+        逐列标准化后的数据.
+    '''
+    from sklearn.preprocessing import MinMaxScaler
+    scaler=MinMaxScaler(feature_range=feature_range)
+    
+    result = df.copy()
+    for feature_name in df.columns:
+        # max_value=df[feature_name].max()
+        # min_value=df[feature_name].min()
+        # result[feature_name]=(df[feature_name] - min_value) / (max_value - min_value)
+        result[feature_name]=scaler.fit_transform(df[[feature_name]])
+    return result
```

### Comparing `usda-0.0.18/src/usda/utils/_displayable_path.py` & `usda-0.0.19/src/usda/utils/_displayable_path.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/utils/_file_structure.py` & `usda-0.0.19/src/usda/utils/_file_structure.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda/utils/_operating_time.py` & `usda-0.0.19/src/usda/utils/_operating_time.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.18/src/usda.egg-info/PKG-INFO` & `usda-0.0.19/src/usda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usda
-Version: 0.0.18
+Version: 0.0.19
 Summary: A set of python modules for Urban Spatial Data Analysis Method (USDA)
 Home-page: https://richiebao.github.io/USDA_PyPI
 Download-URL: https://github.com/richieBao/USDA_PyPI
 Maintainer: Richie Bao
 Maintainer-email: richiebao@outlook.com
 License: new BSD
 Project-URL: Documentation, https://richiebao.github.io/USDA_PyPI
```

### Comparing `usda-0.0.18/src/usda.egg-info/SOURCES.txt` & `usda-0.0.19/src/usda.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/usda.egg-info/requires.txt
 src/usda.egg-info/top_level.txt
 src/usda/data_process/__init__.py
 src/usda/data_process/_geoinfodata_conversion.py
 src/usda/data_process/_image_pixel_sampling_zoom.py
 src/usda/data_process/_kitti_dataprocess.py
 src/usda/data_process/_landsat_dataprocess.py
+src/usda/data_process/_naip_dataprocess.py
 src/usda/data_process/_osm_dataprocess.py
 src/usda/data_process/_raster_dataprocess.py
 src/usda/data_process/_tiler_calculation.py
 src/usda/data_visualization/__init__.py
 src/usda/data_visualization/_chart_custom.py
 src/usda/data_visualization/_colors.py
 src/usda/data_visualization/_dynamic_streetView_visual_perception.py
@@ -27,14 +28,16 @@
 src/usda/data_visualization/_image_process.py
 src/usda/data_visualization/_img_feature_extraction.py
 src/usda/data_visualization/_img_theme_color.py
 src/usda/data_visualization/_imgs_layout_show.py
 src/usda/data_visualization/_imgs_show.py
 src/usda/data_visualization/_knee_line_graph.py
 src/usda/data_visualization/_moving_average_inflection.py
+src/usda/data_visualization/_panorama_show.py
+src/usda/data_visualization/_plot_single_function.py
 src/usda/data_visualization/_raster_percentile_slider.py
 src/usda/data_visualization/_raster_show.py
 src/usda/data_visualization/_stats_charts.py
 src/usda/data_visualization/_superpixel_segmentation_show.py
 src/usda/data_visualization/_table_show.py
 src/usda/data_visualization/_tile_show.py
 src/usda/data_visualization/data_generator.py
@@ -50,51 +53,85 @@
 src/usda/datasets/_dataset_info.py
 src/usda/datasets/_img_info.py
 src/usda/datasets/_kml_info.py
 src/usda/datasets/_rs_image.py
 src/usda/datasets/data/__init__.py
 src/usda/datasets/data/bowling_contest_cartoon_statistic.pickle
 src/usda/datasets/data/evaluation_criteria_raw_values.pickle
+src/usda/datasets/data/jisperveld_data.pickle
+src/usda/datasets/data/microclimate_in_office_rooms.pickle
 src/usda/datasets/data/ramen_price_cartoon_statistic.pickle
 src/usda/datasets/data/sales_data_cartoon_database.pickle
+src/usda/datasets/data/sustainability_attributes4electricity_generation_tech.pickle
 src/usda/datasets/data/test_score_cartoon_statistic.pickle
 src/usda/geodata_process/__init__.py
 src/usda/geodata_process/_quadrat.py
 src/usda/geodata_process/_raster_dataprocess.py
+src/usda/geodata_process/_raster_stats.py
+src/usda/geodata_process/_rasterize.py
+src/usda/geodata_process/_rio_tiler.py
+src/usda/geodata_process/_sample_pts.py
 src/usda/indices/__init__.py
 src/usda/indices/_rs_indices.py
 src/usda/maths/__init__.py
 src/usda/maths/_algebra.py
 src/usda/maths/_geometric_calculation.py
+src/usda/meta_heuristics/__init__.py
+src/usda/meta_heuristics/_cuckoo_s.py
+src/usda/meta_heuristics/_firefly_a.py
+src/usda/meta_heuristics/_ga.py
+src/usda/meta_heuristics/_ga_2d.py
+src/usda/meta_heuristics/_ga_2d_fixed_map.py
+src/usda/meta_heuristics/_ga_2d_testing_1.py
+src/usda/meta_heuristics/_ga_2d_testing_2.py
+src/usda/meta_heuristics/_ga_SegaranT.py
+src/usda/meta_heuristics/_gwo.py
+src/usda/meta_heuristics/_pso.py
+src/usda/meta_heuristics/_pso_2d.py
+src/usda/meta_heuristics/_pso_2d_testing.py
 src/usda/models/__init__.py
 src/usda/models/_bow_feature_builder.py
+src/usda/models/_clustering.py
 src/usda/models/_computational_performance.py
 src/usda/models/_curve_segmentation.py
 src/usda/models/_decision_tree.py
 src/usda/models/_dim1_convolution.py
 src/usda/models/_entropy.py
+src/usda/models/_global_local_autocorrelation.py
 src/usda/models/_image_tag_extractor.py
 src/usda/models/_label_encoder.py
 src/usda/models/_neighbors.py
 src/usda/models/_random_forest_classifier.py
 src/usda/models/_sir_model.py
 src/usda/models/_superpixel_segmentation.py
+src/usda/net/_.py
+src/usda/net/__init__.py
+src/usda/net/_networks_pix2pix.py
+src/usda/network/__init__.py
+src/usda/network/_g_drawing.py
+src/usda/network/_pt_pattern.py
 src/usda/pattern_signature/__init__.py
 src/usda/pattern_signature/_distance_metric.py
 src/usda/pattern_signature/_grid_neighbors_xy_finder.py
 src/usda/pattern_signature/_img_region_growing.py
 src/usda/pattern_signature/_pattern_module.py
 src/usda/pattern_signature/_signature.py
 src/usda/pattern_signature/_signature2distance_integration.py
 src/usda/stats/__init__.py
 src/usda/stats/_descriptive_stats.py
 src/usda/stats/_kde.py
 src/usda/stats/_outlier.py
 src/usda/stats/_regression.py
+src/usda/tools/__init__.py
+src/usda/tools/DL_layers_visualizer/DL_layers_visualizer.py
+src/usda/tools/DL_layers_visualizer/__init__.py
 src/usda/utils/__init__.py
 src/usda/utils/_bunch.py
 src/usda/utils/_coordinate_transformation.py
 src/usda/utils/_df_process.py
 src/usda/utils/_displayable_path.py
 src/usda/utils/_file_structure.py
 src/usda/utils/_gadgets.py
-src/usda/utils/_operating_time.py
+src/usda/utils/_operating_time.py
+src/usda/weight/__init__.py
+src/usda/weight/_decision_rule.py
+src/usda/weight/_entropy_weight.py
```

