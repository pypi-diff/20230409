# Comparing `tmp/usda-0.0.19.tar.gz` & `tmp/usda-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usda-0.0.19.tar", last modified: Sun Apr  9 05:18:43 2023, max compression
+gzip compressed data, was "usda-0.0.20.tar", last modified: Sun Apr  9 05:35:28 2023, max compression
```

## Comparing `usda-0.0.19.tar` & `usda-0.0.20.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.513522 usda-0.0.19/
--rw-rw-rw-   0        0        0     1084 2022-10-07 01:27:44.000000 usda-0.0.19/LICENSE
--rw-rw-rw-   0        0        0     1563 2023-04-09 05:18:43.508519 usda-0.0.19/PKG-INFO
--rw-rw-rw-   0        0        0       63 2022-10-24 05:51:49.000000 usda-0.0.19/README.rst
--rw-rw-rw-   0        0        0       42 2023-04-09 05:18:43.513522 usda-0.0.19/setup.cfg
--rw-rw-rw-   0        0        0     4152 2023-03-18 11:11:09.000000 usda-0.0.19/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.004519 usda-0.0.19/src/
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.048519 usda-0.0.19/src/usda/
--rw-rw-rw-   0        0        0      516 2023-04-09 05:17:48.000000 usda-0.0.19/src/usda/__init__.py
--rw-rw-rw-   0        0        0      731 2022-10-16 01:25:29.000000 usda-0.0.19/src/usda/_min_dependencies.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.101519 usda-0.0.19/src/usda/data_process/
--rw-rw-rw-   0        0        0     1147 2023-03-26 03:42:04.000000 usda-0.0.19/src/usda/data_process/__init__.py
--rw-rw-rw-   0        0        0     2125 2022-10-22 01:48:58.000000 usda-0.0.19/src/usda/data_process/_geoinfodata_conversion.py
--rw-rw-rw-   0        0        0    14577 2022-10-28 01:52:51.000000 usda-0.0.19/src/usda/data_process/_image_pixel_sampling_zoom.py
--rw-rw-rw-   0        0        0     1425 2022-10-31 06:03:57.000000 usda-0.0.19/src/usda/data_process/_kitti_dataprocess.py
--rw-rw-rw-   0        0        0     2037 2022-10-26 01:37:19.000000 usda-0.0.19/src/usda/data_process/_landsat_dataprocess.py
--rw-rw-rw-   0        0        0     1854 2023-03-26 07:52:38.000000 usda-0.0.19/src/usda/data_process/_naip_dataprocess.py
--rw-rw-rw-   0        0        0     6348 2022-10-22 00:18:38.000000 usda-0.0.19/src/usda/data_process/_osm_dataprocess.py
--rw-rw-rw-   0        0        0     1085 2023-02-11 08:44:30.000000 usda-0.0.19/src/usda/data_process/_raster_dataprocess.py
--rw-rw-rw-   0        0        0     1332 2022-10-30 06:27:55.000000 usda-0.0.19/src/usda/data_process/_tiler_calculation.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.192520 usda-0.0.19/src/usda/data_visualization/
--rw-rw-rw-   0        0        0     3166 2023-03-17 02:59:30.000000 usda-0.0.19/src/usda/data_visualization/__init__.py
--rw-rw-rw-   0        0        0     5300 2023-02-17 02:29:25.000000 usda-0.0.19/src/usda/data_visualization/_chart_custom.py
--rw-rw-rw-   0        0        0     2351 2022-11-02 07:56:57.000000 usda-0.0.19/src/usda/data_visualization/_colors.py
--rw-rw-rw-   0        0        0     3221 2022-10-29 07:58:07.000000 usda-0.0.19/src/usda/data_visualization/_dynamic_streetView_visual_perception.py
--rw-rw-rw-   0        0        0     3557 2023-02-19 14:47:51.000000 usda-0.0.19/src/usda/data_visualization/_gdf_plot.py
--rw-rw-rw-   0        0        0      952 2022-10-28 11:19:32.000000 usda-0.0.19/src/usda/data_visualization/_gif_show.py
--rw-rw-rw-   0        0        0     2347 2022-10-28 06:34:44.000000 usda-0.0.19/src/usda/data_visualization/_graphic_drawing.py
--rw-rw-rw-   0        0        0     4787 2022-10-31 05:36:51.000000 usda-0.0.19/src/usda/data_visualization/_image_process.py
--rw-rw-rw-   0        0        0     8500 2022-10-29 06:42:38.000000 usda-0.0.19/src/usda/data_visualization/_img_feature_extraction.py
--rw-rw-rw-   0        0        0     7196 2022-10-30 12:18:06.000000 usda-0.0.19/src/usda/data_visualization/_img_theme_color.py
--rw-rw-rw-   0        0        0     2846 2022-10-30 11:18:24.000000 usda-0.0.19/src/usda/data_visualization/_imgs_layout_show.py
--rw-rw-rw-   0        0        0     4174 2023-03-15 02:00:19.000000 usda-0.0.19/src/usda/data_visualization/_imgs_show.py
--rw-rw-rw-   0        0        0      822 2022-11-02 06:07:14.000000 usda-0.0.19/src/usda/data_visualization/_knee_line_graph.py
--rw-rw-rw-   0        0        0     7393 2022-10-29 08:23:53.000000 usda-0.0.19/src/usda/data_visualization/_moving_average_inflection.py
--rw-rw-rw-   0        0        0     3176 2023-02-24 07:31:39.000000 usda-0.0.19/src/usda/data_visualization/_panorama_show.py
--rw-rw-rw-   0        0        0     8051 2023-03-19 04:08:53.000000 usda-0.0.19/src/usda/data_visualization/_plot_single_function.py
--rw-rw-rw-   0        0        0     2310 2022-10-28 01:13:41.000000 usda-0.0.19/src/usda/data_visualization/_raster_percentile_slider.py
--rw-rw-rw-   0        0        0     1224 2022-10-28 00:45:13.000000 usda-0.0.19/src/usda/data_visualization/_raster_show.py
--rw-rw-rw-   0        0        0     2130 2022-10-28 06:32:06.000000 usda-0.0.19/src/usda/data_visualization/_stats_charts.py
--rw-rw-rw-   0        0        0     2666 2022-10-30 07:27:14.000000 usda-0.0.19/src/usda/data_visualization/_superpixel_segmentation_show.py
--rw-rw-rw-   0        0        0     1577 2022-10-22 23:37:39.000000 usda-0.0.19/src/usda/data_visualization/_table_show.py
--rw-rw-rw-   0        0        0     1673 2022-11-02 06:07:23.000000 usda-0.0.19/src/usda/data_visualization/_tile_show.py
--rw-rw-rw-   0        0        0     4464 2020-07-17 02:38:10.000000 usda-0.0.19/src/usda/data_visualization/data_generator.py
--rw-rw-rw-   0        0        0    10263 2020-07-17 02:38:10.000000 usda-0.0.19/src/usda/data_visualization/knee_locator.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.210520 usda-0.0.19/src/usda/database/
--rw-rw-rw-   0        0        0      839 2023-03-21 05:11:06.000000 usda-0.0.19/src/usda/database/__init__.py
--rw-rw-rw-   0        0        0      693 2022-10-30 12:15:41.000000 usda-0.0.19/src/usda/database/_data_file_rw.py
--rw-rw-rw-   0        0        0     4636 2023-03-21 05:10:00.000000 usda-0.0.19/src/usda/database/_data_format_conversion.py
--rw-rw-rw-   0        0        0     5605 2023-03-21 05:08:27.000000 usda-0.0.19/src/usda/database/_database.py
--rw-rw-rw-   0        0        0     1384 2022-10-28 08:27:55.000000 usda-0.0.19/src/usda/database/_read_matlab_fig.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.234520 usda-0.0.19/src/usda/datasets/
--rw-rw-rw-   0        0        0     1594 2023-03-13 12:31:06.000000 usda-0.0.19/src/usda/datasets/__init__.py
--rw-rw-rw-   0        0        0    17136 2023-03-13 12:40:56.000000 usda-0.0.19/src/usda/datasets/_artificial_data.py
--rw-rw-rw-   0        0        0    19730 2023-03-14 01:14:44.000000 usda-0.0.19/src/usda/datasets/_base.py
--rw-rw-rw-   0        0        0     2745 2022-10-31 05:44:19.000000 usda-0.0.19/src/usda/datasets/_dataset_info.py
--rw-rw-rw-   0        0        0     2681 2022-10-30 11:21:33.000000 usda-0.0.19/src/usda/datasets/_img_info.py
--rw-rw-rw-   0        0        0     2806 2022-10-30 10:50:28.000000 usda-0.0.19/src/usda/datasets/_kml_info.py
--rw-rw-rw-   0        0        0     1547 2022-10-30 07:02:03.000000 usda-0.0.19/src/usda/datasets/_rs_image.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.265521 usda-0.0.19/src/usda/datasets/data/
--rw-rw-rw-   0        0        0      125 2022-08-21 07:11:20.000000 usda-0.0.19/src/usda/datasets/data/__init__.py
--rw-rw-rw-   0        0        0     1224 2022-10-19 04:41:26.000000 usda-0.0.19/src/usda/datasets/data/bowling_contest_cartoon_statistic.pickle
--rw-rw-rw-   0        0        0      950 2023-02-23 02:44:29.000000 usda-0.0.19/src/usda/datasets/data/evaluation_criteria_raw_values.pickle
--rw-rw-rw-   0        0        0     8356 2023-03-13 12:16:36.000000 usda-0.0.19/src/usda/datasets/data/jisperveld_data.pickle
--rw-rw-rw-   0        0        0     1486 2023-02-27 14:21:28.000000 usda-0.0.19/src/usda/datasets/data/microclimate_in_office_rooms.pickle
--rw-rw-rw-   0        0        0     1089 2022-10-19 01:41:55.000000 usda-0.0.19/src/usda/datasets/data/ramen_price_cartoon_statistic.pickle
--rw-rw-rw-   0        0        0     2123 2022-10-15 01:16:56.000000 usda-0.0.19/src/usda/datasets/data/sales_data_cartoon_database.pickle
--rw-rw-rw-   0        0        0     1352 2023-02-24 07:53:38.000000 usda-0.0.19/src/usda/datasets/data/sustainability_attributes4electricity_generation_tech.pickle
--rw-rw-rw-   0        0        0     1340 2022-10-19 05:00:19.000000 usda-0.0.19/src/usda/datasets/data/test_score_cartoon_statistic.pickle
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.286519 usda-0.0.19/src/usda/geodata_process/
--rw-rw-rw-   0        0        0     1349 2023-03-26 01:38:53.000000 usda-0.0.19/src/usda/geodata_process/__init__.py
--rw-rw-rw-   0        0        0     4314 2023-03-22 05:01:49.000000 usda-0.0.19/src/usda/geodata_process/_quadrat.py
--rw-rw-rw-   0        0        0     6535 2023-03-22 16:40:23.000000 usda-0.0.19/src/usda/geodata_process/_raster_dataprocess.py
--rw-rw-rw-   0        0        0     6633 2023-03-22 14:50:33.000000 usda-0.0.19/src/usda/geodata_process/_raster_stats.py
--rw-rw-rw-   0        0        0     6661 2023-03-21 13:11:59.000000 usda-0.0.19/src/usda/geodata_process/_rasterize.py
--rw-rw-rw-   0        0        0     3080 2023-03-22 01:53:07.000000 usda-0.0.19/src/usda/geodata_process/_rio_tiler.py
--rw-rw-rw-   0        0        0     3340 2023-03-22 04:59:15.000000 usda-0.0.19/src/usda/geodata_process/_sample_pts.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.295521 usda-0.0.19/src/usda/indices/
--rw-rw-rw-   0        0        0      189 2022-10-26 06:14:56.000000 usda-0.0.19/src/usda/indices/__init__.py
--rw-rw-rw-   0        0        0      574 2022-10-26 06:15:29.000000 usda-0.0.19/src/usda/indices/_rs_indices.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.303520 usda-0.0.19/src/usda/maths/
--rw-rw-rw-   0        0        0      557 2022-10-26 03:06:13.000000 usda-0.0.19/src/usda/maths/__init__.py
--rw-rw-rw-   0        0        0     4335 2022-10-26 02:53:02.000000 usda-0.0.19/src/usda/maths/_algebra.py
--rw-rw-rw-   0        0        0     1519 2022-10-26 03:05:19.000000 usda-0.0.19/src/usda/maths/_geometric_calculation.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.345520 usda-0.0.19/src/usda/meta_heuristics/
--rw-rw-rw-   0        0        0      843 2023-03-19 01:33:28.000000 usda-0.0.19/src/usda/meta_heuristics/__init__.py
--rw-rw-rw-   0        0        0     5889 2023-03-18 13:00:33.000000 usda-0.0.19/src/usda/meta_heuristics/_cuckoo_s.py
--rw-rw-rw-   0        0        0     4919 2023-03-19 01:22:52.000000 usda-0.0.19/src/usda/meta_heuristics/_firefly_a.py
--rw-rw-rw-   0        0        0    11373 2023-03-10 03:50:42.000000 usda-0.0.19/src/usda/meta_heuristics/_ga.py
--rw-rw-rw-   0        0        0    13840 2023-03-15 22:13:00.000000 usda-0.0.19/src/usda/meta_heuristics/_ga_2d.py
--rw-rw-rw-   0        0        0    14213 2023-03-16 01:38:05.000000 usda-0.0.19/src/usda/meta_heuristics/_ga_2d_fixed_map.py
--rw-rw-rw-   0        0        0    15440 2023-03-15 14:33:57.000000 usda-0.0.19/src/usda/meta_heuristics/_ga_2d_testing_1.py
--rw-rw-rw-   0        0        0    25287 2023-03-17 02:56:06.000000 usda-0.0.19/src/usda/meta_heuristics/_ga_2d_testing_2.py
--rw-rw-rw-   0        0        0     4177 2023-03-10 02:05:28.000000 usda-0.0.19/src/usda/meta_heuristics/_ga_SegaranT.py
--rw-rw-rw-   0        0        0     7982 2023-03-01 00:42:26.000000 usda-0.0.19/src/usda/meta_heuristics/_gwo.py
--rw-rw-rw-   0        0        0     5251 2023-03-17 04:06:12.000000 usda-0.0.19/src/usda/meta_heuristics/_pso.py
--rw-rw-rw-   0        0        0     7564 2023-03-18 04:30:41.000000 usda-0.0.19/src/usda/meta_heuristics/_pso_2d.py
--rw-rw-rw-   0        0        0     8467 2023-03-18 05:15:54.000000 usda-0.0.19/src/usda/meta_heuristics/_pso_2d_testing.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.392521 usda-0.0.19/src/usda/models/
--rw-rw-rw-   0        0        0     2110 2023-03-24 10:49:29.000000 usda-0.0.19/src/usda/models/__init__.py
--rw-rw-rw-   0        0        0     3873 2022-10-31 06:56:19.000000 usda-0.0.19/src/usda/models/_bow_feature_builder.py
--rw-rw-rw-   0        0        0     1014 2023-03-24 02:28:49.000000 usda-0.0.19/src/usda/models/_clustering.py
--rw-rw-rw-   0        0        0     3105 2022-10-25 01:59:30.000000 usda-0.0.19/src/usda/models/_computational_performance.py
--rw-rw-rw-   0        0        0     1897 2022-10-28 08:34:08.000000 usda-0.0.19/src/usda/models/_curve_segmentation.py
--rw-rw-rw-   0        0        0     3928 2022-10-31 07:59:05.000000 usda-0.0.19/src/usda/models/_decision_tree.py
--rw-rw-rw-   0        0        0     5811 2022-10-28 08:15:41.000000 usda-0.0.19/src/usda/models/_dim1_convolution.py
--rw-rw-rw-   0        0        0     2676 2022-10-31 07:41:49.000000 usda-0.0.19/src/usda/models/_entropy.py
--rw-rw-rw-   0        0        0     1458 2023-03-24 10:49:05.000000 usda-0.0.19/src/usda/models/_global_local_autocorrelation.py
--rw-rw-rw-   0        0        0     1427 2022-11-02 06:11:04.000000 usda-0.0.19/src/usda/models/_image_tag_extractor.py
--rw-rw-rw-   0        0        0      869 2022-10-31 07:16:43.000000 usda-0.0.19/src/usda/models/_label_encoder.py
--rw-rw-rw-   0        0        0     1022 2022-10-25 01:02:56.000000 usda-0.0.19/src/usda/models/_neighbors.py
--rw-rw-rw-   0        0        0     1422 2022-10-31 08:30:25.000000 usda-0.0.19/src/usda/models/_random_forest_classifier.py
--rw-rw-rw-   0        0        0    11923 2022-10-28 11:44:45.000000 usda-0.0.19/src/usda/models/_sir_model.py
--rw-rw-rw-   0        0        0     3200 2022-10-30 07:33:05.000000 usda-0.0.19/src/usda/models/_superpixel_segmentation.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.400519 usda-0.0.19/src/usda/net/
--rw-rw-rw-   0        0        0      120 2023-04-05 02:07:48.000000 usda-0.0.19/src/usda/net/_.py
--rw-rw-rw-   0        0        0      856 2023-04-05 02:18:09.000000 usda-0.0.19/src/usda/net/__init__.py
--rw-rw-rw-   0        0        0    28490 2023-04-05 02:16:39.000000 usda-0.0.19/src/usda/net/_networks_pix2pix.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.411519 usda-0.0.19/src/usda/network/
--rw-rw-rw-   0        0        0      404 2023-04-01 07:37:21.000000 usda-0.0.19/src/usda/network/__init__.py
--rw-rw-rw-   0        0        0     4050 2023-03-10 11:37:13.000000 usda-0.0.19/src/usda/network/_g_drawing.py
--rw-rw-rw-   0        0        0     2896 2023-04-01 07:46:50.000000 usda-0.0.19/src/usda/network/_pt_pattern.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.436519 usda-0.0.19/src/usda/pattern_signature/
--rw-rw-rw-   0        0        0     1340 2023-03-24 06:18:07.000000 usda-0.0.19/src/usda/pattern_signature/__init__.py
--rw-rw-rw-   0        0        0     5975 2023-02-12 02:57:51.000000 usda-0.0.19/src/usda/pattern_signature/_distance_metric.py
--rw-rw-rw-   0        0        0     1182 2023-02-09 14:05:16.000000 usda-0.0.19/src/usda/pattern_signature/_grid_neighbors_xy_finder.py
--rw-rw-rw-   0        0        0     8778 2023-02-19 14:00:29.000000 usda-0.0.19/src/usda/pattern_signature/_img_region_growing.py
--rw-rw-rw-   0        0        0    20197 2023-02-19 13:21:56.000000 usda-0.0.19/src/usda/pattern_signature/_pattern_module.py
--rw-rw-rw-   0        0        0     7729 2023-03-24 07:51:30.000000 usda-0.0.19/src/usda/pattern_signature/_signature.py
--rw-rw-rw-   0        0        0     3191 2023-02-12 09:54:49.000000 usda-0.0.19/src/usda/pattern_signature/_signature2distance_integration.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.454520 usda-0.0.19/src/usda/stats/
--rw-rw-rw-   0        0        0     1011 2022-10-24 05:16:26.000000 usda-0.0.19/src/usda/stats/__init__.py
--rw-rw-rw-   0        0        0     3501 2022-10-20 03:25:19.000000 usda-0.0.19/src/usda/stats/_descriptive_stats.py
--rw-rw-rw-   0        0        0     2233 2022-10-22 02:45:57.000000 usda-0.0.19/src/usda/stats/_kde.py
--rw-rw-rw-   0        0        0      778 2022-10-20 03:57:18.000000 usda-0.0.19/src/usda/stats/_outlier.py
--rw-rw-rw-   0        0        0    10793 2022-10-24 05:19:28.000000 usda-0.0.19/src/usda/stats/_regression.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.458519 usda-0.0.19/src/usda/tools/
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.463521 usda-0.0.19/src/usda/tools/DL_layers_visualizer/
--rw-rw-rw-   0        0        0     1064 2023-04-08 15:24:36.000000 usda-0.0.19/src/usda/tools/DL_layers_visualizer/DL_layers_visualizer.py
--rw-rw-rw-   0        0        0      196 2023-04-07 11:25:06.000000 usda-0.0.19/src/usda/tools/DL_layers_visualizer/__init__.py
--rw-rw-rw-   0        0        0      196 2023-04-06 11:45:47.000000 usda-0.0.19/src/usda/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.493521 usda-0.0.19/src/usda/utils/
--rw-rw-rw-   0        0        0     1073 2023-02-24 02:03:24.000000 usda-0.0.19/src/usda/utils/__init__.py
--rw-rw-rw-   0        0        0     1497 2022-10-17 01:46:32.000000 usda-0.0.19/src/usda/utils/_bunch.py
--rw-rw-rw-   0        0        0     5197 2022-10-18 07:06:26.000000 usda-0.0.19/src/usda/utils/_coordinate_transformation.py
--rw-rw-rw-   0        0        0     3970 2023-02-23 09:40:47.000000 usda-0.0.19/src/usda/utils/_df_process.py
--rw-rw-rw-   0        0        0     2938 2022-10-17 01:57:17.000000 usda-0.0.19/src/usda/utils/_displayable_path.py
--rw-rw-rw-   0        0        0     1857 2022-10-26 01:31:31.000000 usda-0.0.19/src/usda/utils/_file_structure.py
--rw-rw-rw-   0        0        0     3992 2023-02-24 02:02:45.000000 usda-0.0.19/src/usda/utils/_gadgets.py
--rw-rw-rw-   0        0        0      606 2022-10-22 00:35:56.000000 usda-0.0.19/src/usda/utils/_operating_time.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.505519 usda-0.0.19/src/usda/weight/
--rw-rw-rw-   0        0        0     1014 2023-03-03 07:14:29.000000 usda-0.0.19/src/usda/weight/__init__.py
--rw-rw-rw-   0        0        0    38486 2023-03-03 07:13:35.000000 usda-0.0.19/src/usda/weight/_decision_rule.py
--rw-rw-rw-   0        0        0     2745 2023-02-23 12:30:34.000000 usda-0.0.19/src/usda/weight/_entropy_weight.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:18:43.066521 usda-0.0.19/src/usda.egg-info/
--rw-rw-rw-   0        0        0     1563 2023-04-09 05:18:42.000000 usda-0.0.19/src/usda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5385 2023-04-09 05:18:42.000000 usda-0.0.19/src/usda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 05:18:42.000000 usda-0.0.19/src/usda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-10-16 07:33:50.000000 usda-0.0.19/src/usda.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       55 2023-04-09 05:18:42.000000 usda-0.0.19/src/usda.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-09 05:18:42.000000 usda-0.0.19/src/usda.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.715225 usda-0.0.20/
+-rw-rw-rw-   0        0        0     1084 2022-10-07 01:27:44.000000 usda-0.0.20/LICENSE
+-rw-rw-rw-   0        0        0     1563 2023-04-09 05:35:28.710217 usda-0.0.20/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2022-10-24 05:51:49.000000 usda-0.0.20/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-09 05:35:28.715225 usda-0.0.20/setup.cfg
+-rw-rw-rw-   0        0        0     4152 2023-03-18 11:11:09.000000 usda-0.0.20/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.232215 usda-0.0.20/src/
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.273221 usda-0.0.20/src/usda/
+-rw-rw-rw-   0        0        0      562 2023-04-09 05:35:21.000000 usda-0.0.20/src/usda/__init__.py
+-rw-rw-rw-   0        0        0      731 2022-10-16 01:25:29.000000 usda-0.0.20/src/usda/_min_dependencies.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.327217 usda-0.0.20/src/usda/data_process/
+-rw-rw-rw-   0        0        0     1147 2023-03-26 03:42:04.000000 usda-0.0.20/src/usda/data_process/__init__.py
+-rw-rw-rw-   0        0        0     2125 2022-10-22 01:48:58.000000 usda-0.0.20/src/usda/data_process/_geoinfodata_conversion.py
+-rw-rw-rw-   0        0        0    14577 2022-10-28 01:52:51.000000 usda-0.0.20/src/usda/data_process/_image_pixel_sampling_zoom.py
+-rw-rw-rw-   0        0        0     1425 2022-10-31 06:03:57.000000 usda-0.0.20/src/usda/data_process/_kitti_dataprocess.py
+-rw-rw-rw-   0        0        0     2037 2022-10-26 01:37:19.000000 usda-0.0.20/src/usda/data_process/_landsat_dataprocess.py
+-rw-rw-rw-   0        0        0     1854 2023-03-26 07:52:38.000000 usda-0.0.20/src/usda/data_process/_naip_dataprocess.py
+-rw-rw-rw-   0        0        0     6348 2022-10-22 00:18:38.000000 usda-0.0.20/src/usda/data_process/_osm_dataprocess.py
+-rw-rw-rw-   0        0        0     1085 2023-02-11 08:44:30.000000 usda-0.0.20/src/usda/data_process/_raster_dataprocess.py
+-rw-rw-rw-   0        0        0     1332 2022-10-30 06:27:55.000000 usda-0.0.20/src/usda/data_process/_tiler_calculation.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.397241 usda-0.0.20/src/usda/data_visualization/
+-rw-rw-rw-   0        0        0     3166 2023-03-17 02:59:30.000000 usda-0.0.20/src/usda/data_visualization/__init__.py
+-rw-rw-rw-   0        0        0     5300 2023-02-17 02:29:25.000000 usda-0.0.20/src/usda/data_visualization/_chart_custom.py
+-rw-rw-rw-   0        0        0     2351 2022-11-02 07:56:57.000000 usda-0.0.20/src/usda/data_visualization/_colors.py
+-rw-rw-rw-   0        0        0     3221 2022-10-29 07:58:07.000000 usda-0.0.20/src/usda/data_visualization/_dynamic_streetView_visual_perception.py
+-rw-rw-rw-   0        0        0     3557 2023-02-19 14:47:51.000000 usda-0.0.20/src/usda/data_visualization/_gdf_plot.py
+-rw-rw-rw-   0        0        0      952 2022-10-28 11:19:32.000000 usda-0.0.20/src/usda/data_visualization/_gif_show.py
+-rw-rw-rw-   0        0        0     2347 2022-10-28 06:34:44.000000 usda-0.0.20/src/usda/data_visualization/_graphic_drawing.py
+-rw-rw-rw-   0        0        0     4787 2022-10-31 05:36:51.000000 usda-0.0.20/src/usda/data_visualization/_image_process.py
+-rw-rw-rw-   0        0        0     8500 2022-10-29 06:42:38.000000 usda-0.0.20/src/usda/data_visualization/_img_feature_extraction.py
+-rw-rw-rw-   0        0        0     7196 2022-10-30 12:18:06.000000 usda-0.0.20/src/usda/data_visualization/_img_theme_color.py
+-rw-rw-rw-   0        0        0     2846 2022-10-30 11:18:24.000000 usda-0.0.20/src/usda/data_visualization/_imgs_layout_show.py
+-rw-rw-rw-   0        0        0     4174 2023-03-15 02:00:19.000000 usda-0.0.20/src/usda/data_visualization/_imgs_show.py
+-rw-rw-rw-   0        0        0      822 2022-11-02 06:07:14.000000 usda-0.0.20/src/usda/data_visualization/_knee_line_graph.py
+-rw-rw-rw-   0        0        0     7393 2022-10-29 08:23:53.000000 usda-0.0.20/src/usda/data_visualization/_moving_average_inflection.py
+-rw-rw-rw-   0        0        0     3176 2023-02-24 07:31:39.000000 usda-0.0.20/src/usda/data_visualization/_panorama_show.py
+-rw-rw-rw-   0        0        0     8051 2023-03-19 04:08:53.000000 usda-0.0.20/src/usda/data_visualization/_plot_single_function.py
+-rw-rw-rw-   0        0        0     2310 2022-10-28 01:13:41.000000 usda-0.0.20/src/usda/data_visualization/_raster_percentile_slider.py
+-rw-rw-rw-   0        0        0     1224 2022-10-28 00:45:13.000000 usda-0.0.20/src/usda/data_visualization/_raster_show.py
+-rw-rw-rw-   0        0        0     2130 2022-10-28 06:32:06.000000 usda-0.0.20/src/usda/data_visualization/_stats_charts.py
+-rw-rw-rw-   0        0        0     2666 2022-10-30 07:27:14.000000 usda-0.0.20/src/usda/data_visualization/_superpixel_segmentation_show.py
+-rw-rw-rw-   0        0        0     1577 2022-10-22 23:37:39.000000 usda-0.0.20/src/usda/data_visualization/_table_show.py
+-rw-rw-rw-   0        0        0     1673 2022-11-02 06:07:23.000000 usda-0.0.20/src/usda/data_visualization/_tile_show.py
+-rw-rw-rw-   0        0        0     4464 2020-07-17 02:38:10.000000 usda-0.0.20/src/usda/data_visualization/data_generator.py
+-rw-rw-rw-   0        0        0    10263 2020-07-17 02:38:10.000000 usda-0.0.20/src/usda/data_visualization/knee_locator.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.412215 usda-0.0.20/src/usda/database/
+-rw-rw-rw-   0        0        0      839 2023-03-21 05:11:06.000000 usda-0.0.20/src/usda/database/__init__.py
+-rw-rw-rw-   0        0        0      693 2022-10-30 12:15:41.000000 usda-0.0.20/src/usda/database/_data_file_rw.py
+-rw-rw-rw-   0        0        0     4636 2023-03-21 05:10:00.000000 usda-0.0.20/src/usda/database/_data_format_conversion.py
+-rw-rw-rw-   0        0        0     5605 2023-03-21 05:08:27.000000 usda-0.0.20/src/usda/database/_database.py
+-rw-rw-rw-   0        0        0     1384 2022-10-28 08:27:55.000000 usda-0.0.20/src/usda/database/_read_matlab_fig.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.435242 usda-0.0.20/src/usda/datasets/
+-rw-rw-rw-   0        0        0     1594 2023-03-13 12:31:06.000000 usda-0.0.20/src/usda/datasets/__init__.py
+-rw-rw-rw-   0        0        0    17136 2023-03-13 12:40:56.000000 usda-0.0.20/src/usda/datasets/_artificial_data.py
+-rw-rw-rw-   0        0        0    19730 2023-03-14 01:14:44.000000 usda-0.0.20/src/usda/datasets/_base.py
+-rw-rw-rw-   0        0        0     2745 2022-10-31 05:44:19.000000 usda-0.0.20/src/usda/datasets/_dataset_info.py
+-rw-rw-rw-   0        0        0     2681 2022-10-30 11:21:33.000000 usda-0.0.20/src/usda/datasets/_img_info.py
+-rw-rw-rw-   0        0        0     2806 2022-10-30 10:50:28.000000 usda-0.0.20/src/usda/datasets/_kml_info.py
+-rw-rw-rw-   0        0        0     1547 2022-10-30 07:02:03.000000 usda-0.0.20/src/usda/datasets/_rs_image.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.460218 usda-0.0.20/src/usda/datasets/data/
+-rw-rw-rw-   0        0        0      125 2022-08-21 07:11:20.000000 usda-0.0.20/src/usda/datasets/data/__init__.py
+-rw-rw-rw-   0        0        0     1224 2022-10-19 04:41:26.000000 usda-0.0.20/src/usda/datasets/data/bowling_contest_cartoon_statistic.pickle
+-rw-rw-rw-   0        0        0      950 2023-02-23 02:44:29.000000 usda-0.0.20/src/usda/datasets/data/evaluation_criteria_raw_values.pickle
+-rw-rw-rw-   0        0        0     8356 2023-03-13 12:16:36.000000 usda-0.0.20/src/usda/datasets/data/jisperveld_data.pickle
+-rw-rw-rw-   0        0        0     1486 2023-02-27 14:21:28.000000 usda-0.0.20/src/usda/datasets/data/microclimate_in_office_rooms.pickle
+-rw-rw-rw-   0        0        0     1089 2022-10-19 01:41:55.000000 usda-0.0.20/src/usda/datasets/data/ramen_price_cartoon_statistic.pickle
+-rw-rw-rw-   0        0        0     2123 2022-10-15 01:16:56.000000 usda-0.0.20/src/usda/datasets/data/sales_data_cartoon_database.pickle
+-rw-rw-rw-   0        0        0     1352 2023-02-24 07:53:38.000000 usda-0.0.20/src/usda/datasets/data/sustainability_attributes4electricity_generation_tech.pickle
+-rw-rw-rw-   0        0        0     1340 2022-10-19 05:00:19.000000 usda-0.0.20/src/usda/datasets/data/test_score_cartoon_statistic.pickle
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.483218 usda-0.0.20/src/usda/geodata_process/
+-rw-rw-rw-   0        0        0     1349 2023-03-26 01:38:53.000000 usda-0.0.20/src/usda/geodata_process/__init__.py
+-rw-rw-rw-   0        0        0     4314 2023-03-22 05:01:49.000000 usda-0.0.20/src/usda/geodata_process/_quadrat.py
+-rw-rw-rw-   0        0        0     6535 2023-03-22 16:40:23.000000 usda-0.0.20/src/usda/geodata_process/_raster_dataprocess.py
+-rw-rw-rw-   0        0        0     6633 2023-03-22 14:50:33.000000 usda-0.0.20/src/usda/geodata_process/_raster_stats.py
+-rw-rw-rw-   0        0        0     6661 2023-03-21 13:11:59.000000 usda-0.0.20/src/usda/geodata_process/_rasterize.py
+-rw-rw-rw-   0        0        0     3080 2023-03-22 01:53:07.000000 usda-0.0.20/src/usda/geodata_process/_rio_tiler.py
+-rw-rw-rw-   0        0        0     3340 2023-03-22 04:59:15.000000 usda-0.0.20/src/usda/geodata_process/_sample_pts.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.488252 usda-0.0.20/src/usda/indices/
+-rw-rw-rw-   0        0        0      189 2022-10-26 06:14:56.000000 usda-0.0.20/src/usda/indices/__init__.py
+-rw-rw-rw-   0        0        0      574 2022-10-26 06:15:29.000000 usda-0.0.20/src/usda/indices/_rs_indices.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.499243 usda-0.0.20/src/usda/maths/
+-rw-rw-rw-   0        0        0      557 2022-10-26 03:06:13.000000 usda-0.0.20/src/usda/maths/__init__.py
+-rw-rw-rw-   0        0        0     4335 2022-10-26 02:53:02.000000 usda-0.0.20/src/usda/maths/_algebra.py
+-rw-rw-rw-   0        0        0     1519 2022-10-26 03:05:19.000000 usda-0.0.20/src/usda/maths/_geometric_calculation.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.541218 usda-0.0.20/src/usda/meta_heuristics/
+-rw-rw-rw-   0        0        0      843 2023-03-19 01:33:28.000000 usda-0.0.20/src/usda/meta_heuristics/__init__.py
+-rw-rw-rw-   0        0        0     5889 2023-03-18 13:00:33.000000 usda-0.0.20/src/usda/meta_heuristics/_cuckoo_s.py
+-rw-rw-rw-   0        0        0     4919 2023-03-19 01:22:52.000000 usda-0.0.20/src/usda/meta_heuristics/_firefly_a.py
+-rw-rw-rw-   0        0        0    11373 2023-03-10 03:50:42.000000 usda-0.0.20/src/usda/meta_heuristics/_ga.py
+-rw-rw-rw-   0        0        0    13840 2023-03-15 22:13:00.000000 usda-0.0.20/src/usda/meta_heuristics/_ga_2d.py
+-rw-rw-rw-   0        0        0    14213 2023-03-16 01:38:05.000000 usda-0.0.20/src/usda/meta_heuristics/_ga_2d_fixed_map.py
+-rw-rw-rw-   0        0        0    15440 2023-03-15 14:33:57.000000 usda-0.0.20/src/usda/meta_heuristics/_ga_2d_testing_1.py
+-rw-rw-rw-   0        0        0    25287 2023-03-17 02:56:06.000000 usda-0.0.20/src/usda/meta_heuristics/_ga_2d_testing_2.py
+-rw-rw-rw-   0        0        0     4177 2023-03-10 02:05:28.000000 usda-0.0.20/src/usda/meta_heuristics/_ga_SegaranT.py
+-rw-rw-rw-   0        0        0     7982 2023-03-01 00:42:26.000000 usda-0.0.20/src/usda/meta_heuristics/_gwo.py
+-rw-rw-rw-   0        0        0     5251 2023-03-17 04:06:12.000000 usda-0.0.20/src/usda/meta_heuristics/_pso.py
+-rw-rw-rw-   0        0        0     7564 2023-03-18 04:30:41.000000 usda-0.0.20/src/usda/meta_heuristics/_pso_2d.py
+-rw-rw-rw-   0        0        0     8467 2023-03-18 05:15:54.000000 usda-0.0.20/src/usda/meta_heuristics/_pso_2d_testing.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.596216 usda-0.0.20/src/usda/models/
+-rw-rw-rw-   0        0        0     2110 2023-03-24 10:49:29.000000 usda-0.0.20/src/usda/models/__init__.py
+-rw-rw-rw-   0        0        0     3873 2022-10-31 06:56:19.000000 usda-0.0.20/src/usda/models/_bow_feature_builder.py
+-rw-rw-rw-   0        0        0     1014 2023-03-24 02:28:49.000000 usda-0.0.20/src/usda/models/_clustering.py
+-rw-rw-rw-   0        0        0     3105 2022-10-25 01:59:30.000000 usda-0.0.20/src/usda/models/_computational_performance.py
+-rw-rw-rw-   0        0        0     1897 2022-10-28 08:34:08.000000 usda-0.0.20/src/usda/models/_curve_segmentation.py
+-rw-rw-rw-   0        0        0     3928 2022-10-31 07:59:05.000000 usda-0.0.20/src/usda/models/_decision_tree.py
+-rw-rw-rw-   0        0        0     5811 2022-10-28 08:15:41.000000 usda-0.0.20/src/usda/models/_dim1_convolution.py
+-rw-rw-rw-   0        0        0     2676 2022-10-31 07:41:49.000000 usda-0.0.20/src/usda/models/_entropy.py
+-rw-rw-rw-   0        0        0     1458 2023-03-24 10:49:05.000000 usda-0.0.20/src/usda/models/_global_local_autocorrelation.py
+-rw-rw-rw-   0        0        0     1427 2022-11-02 06:11:04.000000 usda-0.0.20/src/usda/models/_image_tag_extractor.py
+-rw-rw-rw-   0        0        0      869 2022-10-31 07:16:43.000000 usda-0.0.20/src/usda/models/_label_encoder.py
+-rw-rw-rw-   0        0        0     1022 2022-10-25 01:02:56.000000 usda-0.0.20/src/usda/models/_neighbors.py
+-rw-rw-rw-   0        0        0     1422 2022-10-31 08:30:25.000000 usda-0.0.20/src/usda/models/_random_forest_classifier.py
+-rw-rw-rw-   0        0        0    11923 2022-10-28 11:44:45.000000 usda-0.0.20/src/usda/models/_sir_model.py
+-rw-rw-rw-   0        0        0     3200 2022-10-30 07:33:05.000000 usda-0.0.20/src/usda/models/_superpixel_segmentation.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.608218 usda-0.0.20/src/usda/net/
+-rw-rw-rw-   0        0        0      120 2023-04-05 02:07:48.000000 usda-0.0.20/src/usda/net/_.py
+-rw-rw-rw-   0        0        0      856 2023-04-05 02:18:09.000000 usda-0.0.20/src/usda/net/__init__.py
+-rw-rw-rw-   0        0        0    28490 2023-04-05 02:16:39.000000 usda-0.0.20/src/usda/net/_networks_pix2pix.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.623221 usda-0.0.20/src/usda/network/
+-rw-rw-rw-   0        0        0      404 2023-04-01 07:37:21.000000 usda-0.0.20/src/usda/network/__init__.py
+-rw-rw-rw-   0        0        0     4050 2023-03-10 11:37:13.000000 usda-0.0.20/src/usda/network/_g_drawing.py
+-rw-rw-rw-   0        0        0     2896 2023-04-01 07:46:50.000000 usda-0.0.20/src/usda/network/_pt_pattern.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.646216 usda-0.0.20/src/usda/pattern_signature/
+-rw-rw-rw-   0        0        0     1340 2023-03-24 06:18:07.000000 usda-0.0.20/src/usda/pattern_signature/__init__.py
+-rw-rw-rw-   0        0        0     5975 2023-02-12 02:57:51.000000 usda-0.0.20/src/usda/pattern_signature/_distance_metric.py
+-rw-rw-rw-   0        0        0     1182 2023-02-09 14:05:16.000000 usda-0.0.20/src/usda/pattern_signature/_grid_neighbors_xy_finder.py
+-rw-rw-rw-   0        0        0     8778 2023-02-19 14:00:29.000000 usda-0.0.20/src/usda/pattern_signature/_img_region_growing.py
+-rw-rw-rw-   0        0        0    20197 2023-02-19 13:21:56.000000 usda-0.0.20/src/usda/pattern_signature/_pattern_module.py
+-rw-rw-rw-   0        0        0     7729 2023-03-24 07:51:30.000000 usda-0.0.20/src/usda/pattern_signature/_signature.py
+-rw-rw-rw-   0        0        0     3191 2023-02-12 09:54:49.000000 usda-0.0.20/src/usda/pattern_signature/_signature2distance_integration.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.662216 usda-0.0.20/src/usda/stats/
+-rw-rw-rw-   0        0        0     1011 2022-10-24 05:16:26.000000 usda-0.0.20/src/usda/stats/__init__.py
+-rw-rw-rw-   0        0        0     3501 2022-10-20 03:25:19.000000 usda-0.0.20/src/usda/stats/_descriptive_stats.py
+-rw-rw-rw-   0        0        0     2233 2022-10-22 02:45:57.000000 usda-0.0.20/src/usda/stats/_kde.py
+-rw-rw-rw-   0        0        0      778 2022-10-20 03:57:18.000000 usda-0.0.20/src/usda/stats/_outlier.py
+-rw-rw-rw-   0        0        0    10793 2022-10-24 05:19:28.000000 usda-0.0.20/src/usda/stats/_regression.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.667222 usda-0.0.20/src/usda/tools/
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.673222 usda-0.0.20/src/usda/tools/DL_layers_visualizer/
+-rw-rw-rw-   0        0        0     1064 2023-04-08 15:24:36.000000 usda-0.0.20/src/usda/tools/DL_layers_visualizer/DL_layers_visualizer.py
+-rw-rw-rw-   0        0        0      196 2023-04-07 11:25:06.000000 usda-0.0.20/src/usda/tools/DL_layers_visualizer/__init__.py
+-rw-rw-rw-   0        0        0      196 2023-04-06 11:45:47.000000 usda-0.0.20/src/usda/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.699216 usda-0.0.20/src/usda/utils/
+-rw-rw-rw-   0        0        0     1073 2023-02-24 02:03:24.000000 usda-0.0.20/src/usda/utils/__init__.py
+-rw-rw-rw-   0        0        0     1497 2022-10-17 01:46:32.000000 usda-0.0.20/src/usda/utils/_bunch.py
+-rw-rw-rw-   0        0        0     5197 2022-10-18 07:06:26.000000 usda-0.0.20/src/usda/utils/_coordinate_transformation.py
+-rw-rw-rw-   0        0        0     3970 2023-02-23 09:40:47.000000 usda-0.0.20/src/usda/utils/_df_process.py
+-rw-rw-rw-   0        0        0     2938 2022-10-17 01:57:17.000000 usda-0.0.20/src/usda/utils/_displayable_path.py
+-rw-rw-rw-   0        0        0     1857 2022-10-26 01:31:31.000000 usda-0.0.20/src/usda/utils/_file_structure.py
+-rw-rw-rw-   0        0        0     3992 2023-02-24 02:02:45.000000 usda-0.0.20/src/usda/utils/_gadgets.py
+-rw-rw-rw-   0        0        0      606 2022-10-22 00:35:56.000000 usda-0.0.20/src/usda/utils/_operating_time.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.707214 usda-0.0.20/src/usda/weight/
+-rw-rw-rw-   0        0        0     1014 2023-03-03 07:14:29.000000 usda-0.0.20/src/usda/weight/__init__.py
+-rw-rw-rw-   0        0        0    38486 2023-03-03 07:13:35.000000 usda-0.0.20/src/usda/weight/_decision_rule.py
+-rw-rw-rw-   0        0        0     2745 2023-02-23 12:30:34.000000 usda-0.0.20/src/usda/weight/_entropy_weight.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:35:28.298215 usda-0.0.20/src/usda.egg-info/
+-rw-rw-rw-   0        0        0     1563 2023-04-09 05:35:27.000000 usda-0.0.20/src/usda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5385 2023-04-09 05:35:28.000000 usda-0.0.20/src/usda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 05:35:27.000000 usda-0.0.20/src/usda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-10-16 07:33:50.000000 usda-0.0.20/src/usda.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       55 2023-04-09 05:35:27.000000 usda-0.0.20/src/usda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-09 05:35:27.000000 usda-0.0.20/src/usda.egg-info/top_level.txt
```

### Comparing `usda-0.0.19/LICENSE` & `usda-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/PKG-INFO` & `usda-0.0.20/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usda
-Version: 0.0.19
+Version: 0.0.20
 Summary: A set of python modules for Urban Spatial Data Analysis Method (USDA)
 Home-page: https://richiebao.github.io/USDA_PyPI
 Download-URL: https://github.com/richieBao/USDA_PyPI
 Maintainer: Richie Bao
 Maintainer-email: richiebao@outlook.com
 License: new BSD
 Project-URL: Documentation, https://richiebao.github.io/USDA_PyPI
```

### Comparing `usda-0.0.19/setup.py` & `usda-0.0.20/setup.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/__init__.py` & `usda-0.0.20/src/usda/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 
 @author: Richie Bao-caDesign设计(cadesign.cn)
 
 python setup.py sdist
 twine upload dist/usda-0.0.17.tar.gz
 """
 
-__version__ = "0.0.19"
+__version__ = "0.0.20"
 
 __all__ = [
+    "data_process"
     "datasets",
     "database",
     "utils",
     "data_visualization",
     "stats",
     "data_process",
     "geodata_process",
@@ -22,9 +23,11 @@
     "maths",
     "indices",
     "pattern_signature",
     "weight",
     "meta_heuristics",
     "network",
     "random_walk",
+    "net",
+    "tools",
     ]
```

### Comparing `usda-0.0.19/src/usda/_min_dependencies.py` & `usda-0.0.20/src/usda/_min_dependencies.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_process/__init__.py` & `usda-0.0.20/src/usda/data_process/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_process/_geoinfodata_conversion.py` & `usda-0.0.20/src/usda/data_process/_geoinfodata_conversion.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_process/_image_pixel_sampling_zoom.py` & `usda-0.0.20/src/usda/data_process/_image_pixel_sampling_zoom.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_process/_kitti_dataprocess.py` & `usda-0.0.20/src/usda/data_process/_kitti_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_process/_landsat_dataprocess.py` & `usda-0.0.20/src/usda/data_process/_landsat_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_process/_naip_dataprocess.py` & `usda-0.0.20/src/usda/data_process/_naip_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_process/_osm_dataprocess.py` & `usda-0.0.20/src/usda/data_process/_osm_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_process/_raster_dataprocess.py` & `usda-0.0.20/src/usda/data_process/_raster_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_process/_tiler_calculation.py` & `usda-0.0.20/src/usda/data_process/_tiler_calculation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/__init__.py` & `usda-0.0.20/src/usda/data_visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_chart_custom.py` & `usda-0.0.20/src/usda/data_visualization/_chart_custom.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_colors.py` & `usda-0.0.20/src/usda/data_visualization/_colors.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_dynamic_streetView_visual_perception.py` & `usda-0.0.20/src/usda/data_visualization/_dynamic_streetView_visual_perception.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_gdf_plot.py` & `usda-0.0.20/src/usda/data_visualization/_gdf_plot.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_gif_show.py` & `usda-0.0.20/src/usda/data_visualization/_gif_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_graphic_drawing.py` & `usda-0.0.20/src/usda/data_visualization/_graphic_drawing.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_image_process.py` & `usda-0.0.20/src/usda/data_visualization/_image_process.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_img_feature_extraction.py` & `usda-0.0.20/src/usda/data_visualization/_img_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_img_theme_color.py` & `usda-0.0.20/src/usda/data_visualization/_img_theme_color.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_imgs_layout_show.py` & `usda-0.0.20/src/usda/data_visualization/_imgs_layout_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_imgs_show.py` & `usda-0.0.20/src/usda/data_visualization/_imgs_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_knee_line_graph.py` & `usda-0.0.20/src/usda/data_visualization/_knee_line_graph.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_moving_average_inflection.py` & `usda-0.0.20/src/usda/data_visualization/_moving_average_inflection.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_panorama_show.py` & `usda-0.0.20/src/usda/data_visualization/_panorama_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_plot_single_function.py` & `usda-0.0.20/src/usda/data_visualization/_plot_single_function.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_raster_percentile_slider.py` & `usda-0.0.20/src/usda/data_visualization/_raster_percentile_slider.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_raster_show.py` & `usda-0.0.20/src/usda/data_visualization/_raster_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_stats_charts.py` & `usda-0.0.20/src/usda/data_visualization/_stats_charts.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_superpixel_segmentation_show.py` & `usda-0.0.20/src/usda/data_visualization/_superpixel_segmentation_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_table_show.py` & `usda-0.0.20/src/usda/data_visualization/_table_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/_tile_show.py` & `usda-0.0.20/src/usda/data_visualization/_tile_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/data_generator.py` & `usda-0.0.20/src/usda/data_visualization/data_generator.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/data_visualization/knee_locator.py` & `usda-0.0.20/src/usda/data_visualization/knee_locator.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/database/__init__.py` & `usda-0.0.20/src/usda/database/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/database/_data_file_rw.py` & `usda-0.0.20/src/usda/database/_data_file_rw.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/database/_data_format_conversion.py` & `usda-0.0.20/src/usda/database/_data_format_conversion.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/database/_database.py` & `usda-0.0.20/src/usda/database/_database.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/database/_read_matlab_fig.py` & `usda-0.0.20/src/usda/database/_read_matlab_fig.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/datasets/__init__.py` & `usda-0.0.20/src/usda/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/datasets/_artificial_data.py` & `usda-0.0.20/src/usda/datasets/_artificial_data.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/datasets/_base.py` & `usda-0.0.20/src/usda/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/datasets/_dataset_info.py` & `usda-0.0.20/src/usda/datasets/_dataset_info.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/datasets/_img_info.py` & `usda-0.0.20/src/usda/datasets/_img_info.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/datasets/_kml_info.py` & `usda-0.0.20/src/usda/datasets/_kml_info.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/datasets/_rs_image.py` & `usda-0.0.20/src/usda/datasets/_rs_image.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/datasets/data/bowling_contest_cartoon_statistic.pickle` & `usda-0.0.20/src/usda/datasets/data/bowling_contest_cartoon_statistic.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/datasets/data/evaluation_criteria_raw_values.pickle` & `usda-0.0.20/src/usda/datasets/data/evaluation_criteria_raw_values.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/datasets/data/jisperveld_data.pickle` & `usda-0.0.20/src/usda/datasets/data/jisperveld_data.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/datasets/data/microclimate_in_office_rooms.pickle` & `usda-0.0.20/src/usda/datasets/data/microclimate_in_office_rooms.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/datasets/data/ramen_price_cartoon_statistic.pickle` & `usda-0.0.20/src/usda/datasets/data/ramen_price_cartoon_statistic.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/datasets/data/sales_data_cartoon_database.pickle` & `usda-0.0.20/src/usda/datasets/data/sales_data_cartoon_database.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/datasets/data/sustainability_attributes4electricity_generation_tech.pickle` & `usda-0.0.20/src/usda/datasets/data/sustainability_attributes4electricity_generation_tech.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/datasets/data/test_score_cartoon_statistic.pickle` & `usda-0.0.20/src/usda/datasets/data/test_score_cartoon_statistic.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/geodata_process/__init__.py` & `usda-0.0.20/src/usda/geodata_process/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/geodata_process/_quadrat.py` & `usda-0.0.20/src/usda/geodata_process/_quadrat.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/geodata_process/_raster_dataprocess.py` & `usda-0.0.20/src/usda/geodata_process/_raster_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/geodata_process/_raster_stats.py` & `usda-0.0.20/src/usda/geodata_process/_raster_stats.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/geodata_process/_rasterize.py` & `usda-0.0.20/src/usda/geodata_process/_rasterize.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/geodata_process/_rio_tiler.py` & `usda-0.0.20/src/usda/geodata_process/_rio_tiler.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/geodata_process/_sample_pts.py` & `usda-0.0.20/src/usda/geodata_process/_sample_pts.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/indices/_rs_indices.py` & `usda-0.0.20/src/usda/indices/_rs_indices.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/maths/__init__.py` & `usda-0.0.20/src/usda/maths/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/maths/_algebra.py` & `usda-0.0.20/src/usda/maths/_algebra.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/maths/_geometric_calculation.py` & `usda-0.0.20/src/usda/maths/_geometric_calculation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/meta_heuristics/__init__.py` & `usda-0.0.20/src/usda/meta_heuristics/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/meta_heuristics/_cuckoo_s.py` & `usda-0.0.20/src/usda/meta_heuristics/_cuckoo_s.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/meta_heuristics/_firefly_a.py` & `usda-0.0.20/src/usda/meta_heuristics/_firefly_a.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/meta_heuristics/_ga.py` & `usda-0.0.20/src/usda/meta_heuristics/_ga.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/meta_heuristics/_ga_2d.py` & `usda-0.0.20/src/usda/meta_heuristics/_ga_2d.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/meta_heuristics/_ga_2d_fixed_map.py` & `usda-0.0.20/src/usda/meta_heuristics/_ga_2d_fixed_map.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/meta_heuristics/_ga_2d_testing_1.py` & `usda-0.0.20/src/usda/meta_heuristics/_ga_2d_testing_1.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/meta_heuristics/_ga_2d_testing_2.py` & `usda-0.0.20/src/usda/meta_heuristics/_ga_2d_testing_2.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/meta_heuristics/_ga_SegaranT.py` & `usda-0.0.20/src/usda/meta_heuristics/_ga_SegaranT.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/meta_heuristics/_gwo.py` & `usda-0.0.20/src/usda/meta_heuristics/_gwo.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/meta_heuristics/_pso.py` & `usda-0.0.20/src/usda/meta_heuristics/_pso.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/meta_heuristics/_pso_2d.py` & `usda-0.0.20/src/usda/meta_heuristics/_pso_2d.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/meta_heuristics/_pso_2d_testing.py` & `usda-0.0.20/src/usda/meta_heuristics/_pso_2d_testing.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/models/__init__.py` & `usda-0.0.20/src/usda/models/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/models/_bow_feature_builder.py` & `usda-0.0.20/src/usda/models/_bow_feature_builder.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/models/_clustering.py` & `usda-0.0.20/src/usda/models/_clustering.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/models/_computational_performance.py` & `usda-0.0.20/src/usda/models/_computational_performance.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/models/_curve_segmentation.py` & `usda-0.0.20/src/usda/models/_curve_segmentation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/models/_decision_tree.py` & `usda-0.0.20/src/usda/models/_decision_tree.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/models/_dim1_convolution.py` & `usda-0.0.20/src/usda/models/_dim1_convolution.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/models/_entropy.py` & `usda-0.0.20/src/usda/models/_entropy.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/models/_global_local_autocorrelation.py` & `usda-0.0.20/src/usda/models/_global_local_autocorrelation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/models/_image_tag_extractor.py` & `usda-0.0.20/src/usda/models/_image_tag_extractor.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/models/_label_encoder.py` & `usda-0.0.20/src/usda/models/_label_encoder.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/models/_neighbors.py` & `usda-0.0.20/src/usda/models/_neighbors.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/models/_random_forest_classifier.py` & `usda-0.0.20/src/usda/models/_random_forest_classifier.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/models/_sir_model.py` & `usda-0.0.20/src/usda/models/_sir_model.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/models/_superpixel_segmentation.py` & `usda-0.0.20/src/usda/models/_superpixel_segmentation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/net/__init__.py` & `usda-0.0.20/src/usda/net/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/net/_networks_pix2pix.py` & `usda-0.0.20/src/usda/net/_networks_pix2pix.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/network/_g_drawing.py` & `usda-0.0.20/src/usda/network/_g_drawing.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/network/_pt_pattern.py` & `usda-0.0.20/src/usda/network/_pt_pattern.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/pattern_signature/__init__.py` & `usda-0.0.20/src/usda/pattern_signature/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/pattern_signature/_distance_metric.py` & `usda-0.0.20/src/usda/pattern_signature/_distance_metric.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/pattern_signature/_grid_neighbors_xy_finder.py` & `usda-0.0.20/src/usda/pattern_signature/_grid_neighbors_xy_finder.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/pattern_signature/_img_region_growing.py` & `usda-0.0.20/src/usda/pattern_signature/_img_region_growing.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/pattern_signature/_pattern_module.py` & `usda-0.0.20/src/usda/pattern_signature/_pattern_module.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/pattern_signature/_signature.py` & `usda-0.0.20/src/usda/pattern_signature/_signature.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/pattern_signature/_signature2distance_integration.py` & `usda-0.0.20/src/usda/pattern_signature/_signature2distance_integration.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/stats/__init__.py` & `usda-0.0.20/src/usda/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/stats/_descriptive_stats.py` & `usda-0.0.20/src/usda/stats/_descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/stats/_kde.py` & `usda-0.0.20/src/usda/stats/_kde.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/stats/_outlier.py` & `usda-0.0.20/src/usda/stats/_outlier.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/stats/_regression.py` & `usda-0.0.20/src/usda/stats/_regression.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/tools/DL_layers_visualizer/DL_layers_visualizer.py` & `usda-0.0.20/src/usda/tools/DL_layers_visualizer/DL_layers_visualizer.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/utils/__init__.py` & `usda-0.0.20/src/usda/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/utils/_bunch.py` & `usda-0.0.20/src/usda/utils/_bunch.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/utils/_coordinate_transformation.py` & `usda-0.0.20/src/usda/utils/_coordinate_transformation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/utils/_df_process.py` & `usda-0.0.20/src/usda/utils/_df_process.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/utils/_displayable_path.py` & `usda-0.0.20/src/usda/utils/_displayable_path.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/utils/_file_structure.py` & `usda-0.0.20/src/usda/utils/_file_structure.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/utils/_gadgets.py` & `usda-0.0.20/src/usda/utils/_gadgets.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/utils/_operating_time.py` & `usda-0.0.20/src/usda/utils/_operating_time.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/weight/__init__.py` & `usda-0.0.20/src/usda/weight/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/weight/_decision_rule.py` & `usda-0.0.20/src/usda/weight/_decision_rule.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda/weight/_entropy_weight.py` & `usda-0.0.20/src/usda/weight/_entropy_weight.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.19/src/usda.egg-info/PKG-INFO` & `usda-0.0.20/src/usda.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usda
-Version: 0.0.19
+Version: 0.0.20
 Summary: A set of python modules for Urban Spatial Data Analysis Method (USDA)
 Home-page: https://richiebao.github.io/USDA_PyPI
 Download-URL: https://github.com/richieBao/USDA_PyPI
 Maintainer: Richie Bao
 Maintainer-email: richiebao@outlook.com
 License: new BSD
 Project-URL: Documentation, https://richiebao.github.io/USDA_PyPI
```

### Comparing `usda-0.0.19/src/usda.egg-info/SOURCES.txt` & `usda-0.0.20/src/usda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

