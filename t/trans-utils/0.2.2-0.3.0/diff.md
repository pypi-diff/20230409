# Comparing `tmp/trans_utils-0.2.2-py3-none-any.whl.zip` & `tmp/trans_utils-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,37 +1,69 @@
-Zip file size: 101785 bytes, number of entries: 105
--rw-r--r--  2.0 unx       50 b- defN 21-Dec-19 11:34 tutils/__init__.py
+Zip file size: 139350 bytes, number of entries: 158
+-rw-r--r--  2.0 unx       68 b- defN 23-Mar-27 08:56 tutils/__init__.py
+-rw-r--r--  2.0 unx     2281 b- defN 22-Dec-06 07:29 tutils/classify.py
 -rw-r--r--  2.0 unx     3316 b- defN 21-Sep-18 05:14 tutils/functools.py
 -rw-r--r--  2.0 unx     5771 b- defN 21-Oct-19 05:11 tutils/initializer.py
 -rw-r--r--  2.0 unx     3286 b- defN 21-Sep-23 11:39 tutils/tutils.py
+-rw-r--r--  2.0 unx       69 b- defN 22-Oct-14 07:51 tutils/contrib/__init__.py
+-rw-r--r--  2.0 unx     4641 b- defN 23-Apr-09 08:32 tutils/contrib/ddp_demo.py
+-rw-r--r--  2.0 unx      857 b- defN 22-Dec-20 09:58 tutils/contrib/debug_tools.py
+-rw-r--r--  2.0 unx       49 b- defN 22-Oct-14 08:00 tutils/contrib/fourier.py
+-rw-r--r--  2.0 unx        9 b- defN 22-Oct-22 09:06 tutils/contrib/other_package.py
+-rw-r--r--  2.0 unx      111 b- defN 22-Dec-20 09:38 tutils/contrib/pudb_debug.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Dec-06 07:04 tutils/contrib/shutils.py
+-rw-r--r--  2.0 unx      223 b- defN 22-Dec-20 11:14 tutils/contrib/tmp.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Aug-08 09:31 tutils/contrib/proj-template/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Aug-08 09:31 tutils/contrib/proj-template/code/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Aug-08 09:31 tutils/contrib/proj-template/code/configs/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Aug-08 09:31 tutils/contrib/proj-template/code/datasets/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Aug-08 09:31 tutils/contrib/proj-template/code/networks/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Aug-08 09:31 tutils/contrib/proj-template/code/scripts/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Sep-10 14:00 tutils/contrib/proj-template/code/scripts/template.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Sep-12 12:13 tutils/contrib/proj-template/code/test/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Sep-12 12:13 tutils/contrib/proj-template/code/test/datasets/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Sep-12 12:14 tutils/contrib/proj-template/code/test/networks/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Sep-12 12:14 tutils/contrib/proj-template/code/test/utils/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Aug-08 09:31 tutils/contrib/proj-template/code/tmp/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Aug-08 09:31 tutils/contrib/proj-template/code/utils/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Aug-08 09:31 tutils/contrib/proj-template/data/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Aug-08 13:06 tutils/contrib/proj-template/related_work_1/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Aug-08 13:07 tutils/contrib/proj-template/related_work_1/work1/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Aug-08 09:31 tutils/contrib/proj-template/runs/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jun-14 13:03 tutils/contrib/test/__init__.py
+-rw-r--r--  2.0 unx      227 b- defN 22-Jun-30 05:16 tutils/contrib/test/test_builtins.py
+-rw-r--r--  2.0 unx      326 b- defN 22-Jun-14 13:37 tutils/contrib/test/test_initializer.py
+-rw-r--r--  2.0 unx       50 b- defN 22-Jun-30 05:18 tutils/contrib/test/test_print.py
+-rw-r--r--  2.0 unx     1041 b- defN 22-Jun-14 13:39 tutils/contrib/test/test_pytest.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-10 10:25 tutils/mn/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Jul-05 08:46 tutils/mn/data/__init__.py
+-rw-r--r--  2.0 unx       20 b- defN 23-Mar-27 04:19 tutils/mn/data/__init__.py
 -rw-r--r--  2.0 unx      392 b- defN 21-Jun-07 13:25 tutils/mn/data/base_dataset.py
 -rw-r--r--  2.0 unx     3310 b- defN 21-Jun-07 13:25 tutils/mn/data/base_options.py
 -rw-r--r--  2.0 unx     3582 b- defN 21-Jun-24 02:14 tutils/mn/data/data_preprocess.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Jul-13 09:15 tutils/mn/data/augment/__init__.py
 -rw-r--r--  2.0 unx     5720 b- defN 21-Jun-24 02:15 tutils/mn/data/augment/augment.py
 -rw-r--r--  2.0 unx    11514 b- defN 21-Jun-24 02:15 tutils/mn/data/augment/autoaugment.py
--rw-r--r--  2.0 unx     5728 b- defN 21-Dec-30 15:09 tutils/mn/data/augment/common_2d_aug.py
+-rw-r--r--  2.0 unx     6725 b- defN 22-May-10 03:35 tutils/mn/data/augment/common_2d_aug.py
 -rw-r--r--  2.0 unx      469 b- defN 21-Jun-24 02:15 tutils/mn/data/augment/demo_monai_augment.py
 -rw-r--r--  2.0 unx      698 b- defN 21-Jun-24 02:15 tutils/mn/data/augment/edge_detection.py
 -rw-r--r--  2.0 unx     4755 b- defN 21-Jun-24 02:15 tutils/mn/data/augment/gaussian.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Jun-24 02:16 tutils/mn/data/augment/patching.py
--rw-r--r--  2.0 unx       17 b- defN 21-May-28 02:31 tutils/mn/data/tsitk/__init__.py
--rw-r--r--  2.0 unx     1662 b- defN 21-May-28 02:31 tutils/mn/data/tsitk/io.py
+-rw-r--r--  2.0 unx       45 b- defN 23-Mar-27 08:56 tutils/mn/data/tsitk/__init__.py
+-rw-r--r--  2.0 unx     1640 b- defN 23-Mar-27 08:55 tutils/mn/data/tsitk/io.py
 -rw-r--r--  2.0 unx     2335 b- defN 21-Jun-07 14:20 tutils/mn/data/tsitk/preprocess.py
 -rw-r--r--  2.0 unx        0 b- defN 21-May-28 02:31 tutils/mn/eval/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-May-28 02:31 tutils/mn/eval/radio_analysis/__init__.py
 -rw-r--r--  2.0 unx     1794 b- defN 21-May-28 02:31 tutils/mn/eval/radio_analysis/demo.py
 -rw-r--r--  2.0 unx     5394 b- defN 21-May-28 02:31 tutils/mn/eval/radio_analysis/demo_function.py
--rw-r--r--  2.0 unx     6281 b- defN 21-May-28 02:31 tutils/mn/eval/radio_analysis/example_helloFeatureClass.py
+-rw-r--r--  2.0 unx     6311 b- defN 23-Feb-23 07:29 tutils/mn/eval/radio_analysis/example_helloFeatureClass.py
 -rw-r--r--  2.0 unx       55 b- defN 21-May-28 02:31 tutils/mn/eval/radio_analysis/medical_qa.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Jul-05 08:46 tutils/mn/train/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-May-28 02:31 tutils/mn/train/models/__init__.py
--rw-r--r--  2.0 unx     5844 b- defN 21-May-28 02:31 tutils/mn/train/models/cam_model.py
+-rw-r--r--  2.0 unx     5920 b- defN 22-Sep-11 11:44 tutils/mn/train/models/cam_model.py
+-rw-r--r--  2.0 unx      593 b- defN 22-Nov-22 08:42 tutils/mn/train/models/debug_model.py
 -rw-r--r--  2.0 unx     1277 b- defN 21-May-28 02:31 tutils/mn/train/models/unet_model.py
 -rw-r--r--  2.0 unx     2735 b- defN 21-May-28 02:31 tutils/mn/train/models/unet_parts.py
 -rw-r--r--  2.0 unx      236 b- defN 21-May-28 02:31 tutils/mn/train/tloss/__init__.py
 -rw-r--r--  2.0 unx     2326 b- defN 21-May-28 02:31 tutils/mn/train/tloss/edge_loss.py
 -rw-r--r--  2.0 unx     3021 b- defN 21-Jul-13 09:15 tutils/mn/train/tloss/entropy_loss.py
 -rw-r--r--  2.0 unx     6706 b- defN 21-May-28 02:31 tutils/mn/train/tloss/infonce_loss.py
 -rw-r--r--  2.0 unx     1870 b- defN 21-May-28 02:31 tutils/mn/train/tloss/ncc_loss.py
@@ -53,55 +85,76 @@
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-12 12:14 tutils/proj-template/code/test/utils/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Aug-08 09:31 tutils/proj-template/code/tmp/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Aug-08 09:31 tutils/proj-template/code/utils/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Aug-08 09:31 tutils/proj-template/data/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Aug-08 13:06 tutils/proj-template/related_work_1/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Aug-08 13:07 tutils/proj-template/related_work_1/work1/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Aug-08 09:31 tutils/proj-template/runs/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jun-14 13:03 tutils/test/__init__.py
+-rw-r--r--  2.0 unx      227 b- defN 22-Jun-30 05:16 tutils/test/test_builtins.py
+-rw-r--r--  2.0 unx      326 b- defN 22-Jun-14 13:37 tutils/test/test_initializer.py
+-rw-r--r--  2.0 unx       50 b- defN 22-Jun-30 05:18 tutils/test/test_print.py
+-rw-r--r--  2.0 unx     1041 b- defN 22-Jun-14 13:39 tutils/test/test_pytest.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-07 08:19 tutils/tpackage/__init__.py
+-rw-r--r--  2.0 unx     9939 b- defN 23-Feb-02 13:18 tutils/tpackage/_multilogger.py
+-rw-r--r--  2.0 unx     3553 b- defN 23-Feb-02 13:03 tutils/tpackage/learner.py
+-rw-r--r--  2.0 unx     8405 b- defN 23-Feb-02 13:19 tutils/tpackage/logger.py
+-rw-r--r--  2.0 unx     3840 b- defN 23-Feb-02 13:17 tutils/tpackage/logger_utils.py
+-rw-r--r--  2.0 unx     1075 b- defN 23-Feb-07 08:19 tutils/tpackage/monitor.py
+-rw-r--r--  2.0 unx     1500 b- defN 23-Feb-07 08:21 tutils/tpackage/tester.py
+-rw-r--r--  2.0 unx    13552 b- defN 23-Feb-02 13:21 tutils/tpackage/trainer.py
+-rw-r--r--  2.0 unx     1166 b- defN 23-Feb-02 13:21 tutils/tpackage/trainer_utils.py
 -rw-r--r--  2.0 unx      249 b- defN 21-Dec-19 11:26 tutils/trainer/__init__.py
 -rw-r--r--  2.0 unx     2595 b- defN 21-Oct-08 04:01 tutils/trainer/_bad_tuner_exec.py
 -rw-r--r--  2.0 unx     9630 b- defN 21-Nov-21 06:20 tutils/trainer/ablation_exec.py
 -rw-r--r--  2.0 unx       34 b- defN 21-Oct-08 08:38 tutils/trainer/ablation_search.py
 -rw-r--r--  2.0 unx     5017 b- defN 21-Sep-09 08:06 tutils/trainer/ablation_trainer.py
 -rw-r--r--  2.0 unx     5049 b- defN 21-Sep-24 07:54 tutils/trainer/demo_ablation_trainer.py
 -rw-r--r--  2.0 unx     4610 b- defN 21-Sep-12 12:47 tutils/trainer/demo_learner_trainer.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-09 08:06 tutils/trainer/demo_train.py
 -rw-r--r--  2.0 unx     1220 b- defN 21-Oct-21 14:11 tutils/trainer/demo_train_script.py
--rw-r--r--  2.0 unx     3609 b- defN 21-Oct-30 10:52 tutils/trainer/learner.py
--rw-r--r--  2.0 unx     3522 b- defN 21-Oct-30 10:46 tutils/trainer/learner_module.py
+-rw-r--r--  2.0 unx     4189 b- defN 22-Aug-15 06:44 tutils/trainer/learner.py
+-rw-r--r--  2.0 unx     3655 b- defN 22-Oct-29 11:27 tutils/trainer/learner_module.py
 -rw-r--r--  2.0 unx     1075 b- defN 21-Dec-19 11:28 tutils/trainer/monitor.py
--rw-r--r--  2.0 unx     4072 b- defN 21-Dec-19 12:02 tutils/trainer/recorder.py
+-rw-r--r--  2.0 unx     4192 b- defN 23-Apr-03 10:49 tutils/trainer/recorder.py
 -rw-r--r--  2.0 unx      576 b- defN 21-May-28 02:31 tutils/trainer/save.py
 -rw-r--r--  2.0 unx     1071 b- defN 21-Sep-09 08:06 tutils/trainer/simple_script_helper.py
--rw-r--r--  2.0 unx     3408 b- defN 21-Nov-02 06:01 tutils/trainer/trainer.py
--rw-r--r--  2.0 unx    12684 b- defN 21-Nov-12 13:08 tutils/trainer/trainer_abstract.py
+-rw-r--r--  2.0 unx      273 b- defN 23-Apr-08 07:49 tutils/trainer/tester_abstract.py
+-rw-r--r--  2.0 unx     4184 b- defN 23-Apr-09 08:44 tutils/trainer/trainer.py
+-rw-r--r--  2.0 unx    15046 b- defN 23-Apr-09 10:50 tutils/trainer/trainer_abstract.py
 -rw-r--r--  2.0 unx     6926 b- defN 21-Nov-02 06:01 tutils/trainer/trainer_ddp.py
+-rw-r--r--  2.0 unx     2398 b- defN 23-Apr-09 09:09 tutils/trainer/trainer_ddp2.py
 -rw-r--r--  2.0 unx     5611 b- defN 21-Oct-08 04:59 tutils/trainer/tuner_exec.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Oct-26 15:07 tutils/trainer/utils/__init__.py
 -rw-r--r--  2.0 unx     1218 b- defN 21-Oct-28 02:41 tutils/trainer/utils/trainer_utils.py
 -rw-r--r--  2.0 unx      103 b- defN 21-Jun-21 08:10 tutils/tutils/NOTES.md
--rw-r--r--  2.0 unx      465 b- defN 21-Dec-20 07:32 tutils/tutils/__init__.py
+-rw-r--r--  2.0 unx      528 b- defN 23-Apr-09 10:07 tutils/tutils/__init__.py
 -rw-r--r--  2.0 unx     1623 b- defN 21-Sep-13 02:48 tutils/tutils/build_proj.py
--rw-r--r--  2.0 unx     4986 b- defN 21-Oct-12 07:46 tutils/tutils/csv_recorder.py
+-rw-r--r--  2.0 unx     4992 b- defN 22-Aug-13 08:52 tutils/tutils/csv_recorder.py
 -rw-r--r--  2.0 unx      887 b- defN 21-Sep-16 09:26 tutils/tutils/dl_utils.py
--rw-r--r--  2.0 unx     3710 b- defN 21-Dec-19 11:35 tutils/tutils/functools.py
+-rw-r--r--  2.0 unx     3174 b- defN 22-May-10 05:01 tutils/tutils/functools.py
 -rw-r--r--  2.0 unx     1495 b- defN 21-Nov-05 08:33 tutils/tutils/grad_cam.py
--rw-r--r--  2.0 unx     7514 b- defN 21-Dec-08 20:01 tutils/tutils/initializer.py
--rw-r--r--  2.0 unx    29190 b- defN 21-Dec-29 05:40 tutils/tutils/metriclogger.py
--rw-r--r--  2.0 unx     4326 b- defN 21-Dec-30 06:05 tutils/tutils/prologger.py
--rw-r--r--  2.0 unx     4057 b- defN 21-Dec-20 07:34 tutils/tutils/recorder.py
+-rw-r--r--  2.0 unx    11794 b- defN 23-Apr-09 10:11 tutils/tutils/initializer.py
+-rw-r--r--  2.0 unx     7457 b- defN 23-Apr-09 10:49 tutils/tutils/initializer_old.py
+-rw-r--r--  2.0 unx    29240 b- defN 22-Jun-30 05:14 tutils/tutils/metriclogger.py
+-rw-r--r--  2.0 unx     4361 b- defN 22-May-08 13:47 tutils/tutils/prologger.py
+-rw-r--r--  2.0 unx     4136 b- defN 22-Aug-18 08:24 tutils/tutils/recorder.py
+-rw-r--r--  2.0 unx      438 b- defN 22-Apr-16 13:18 tutils/tutils/tconfig.py
 -rw-r--r--  2.0 unx      596 b- defN 21-Sep-06 09:16 tutils/tutils/techo.py
--rw-r--r--  2.0 unx     8382 b- defN 21-Dec-19 11:35 tutils/tutils/tlogger.py
--rw-r--r--  2.0 unx     3005 b- defN 21-Dec-19 11:28 tutils/tutils/ttimer.py
--rw-r--r--  2.0 unx     3527 b- defN 21-Dec-02 08:12 tutils/tutils/tutils.py
+-rw-r--r--  2.0 unx     9946 b- defN 22-Dec-15 07:21 tutils/tutils/tlogger.py
+-rw-r--r--  2.0 unx      996 b- defN 22-Apr-16 13:14 tutils/tutils/torch_utils.py
+-rw-r--r--  2.0 unx     3044 b- defN 22-May-08 13:46 tutils/tutils/ttimer.py
+-rw-r--r--  2.0 unx     3841 b- defN 22-Dec-08 13:37 tutils/tutils/tutils.py
 -rw-r--r--  2.0 unx       93 b- defN 21-Sep-23 11:51 tutils/tutils/visualizers/__init__.py
+-rw-r--r--  2.0 unx     2254 b- defN 22-Oct-12 08:38 tutils/tutils/visualizers/draw_bar_auto_split.py
 -rw-r--r--  2.0 unx     3093 b- defN 21-Sep-22 03:19 tutils/tutils/visualizers/draw_curves.py
 -rw-r--r--  2.0 unx     1655 b- defN 21-Sep-14 13:23 tutils/tutils/visualizers/plt_print_3d.py
--rw-r--r--  2.0 unx     1761 b- defN 21-Sep-15 02:38 tutils/tutils/visualizers/print_image.py
+-rw-r--r--  2.0 unx     1969 b- defN 23-Mar-27 08:54 tutils/tutils/visualizers/print_image.py
 -rw-r--r--  2.0 unx     1949 b- defN 21-May-28 02:31 tutils/tutils/visualizers/print_landmark.py
 -rw-r--r--  2.0 unx     2817 b- defN 21-Nov-21 12:45 tutils/tutils/visualizers/tsne.py
--rw-r--r--  2.0 unx      533 b- defN 22-Jan-04 07:53 trans_utils-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jan-04 07:53 trans_utils-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx      113 b- defN 22-Jan-04 07:53 trans_utils-0.2.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 22-Jan-04 07:53 trans_utils-0.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     9408 b- defN 22-Jan-04 07:53 trans_utils-0.2.2.dist-info/RECORD
-105 files, 283788 bytes uncompressed, 86619 bytes compressed:  69.5%
+-rw-r--r--  2.0 unx    11599 b- defN 23-Apr-09 11:02 trans_utils-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      474 b- defN 23-Apr-09 11:02 trans_utils-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 11:02 trans_utils-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      112 b- defN 23-Apr-09 11:02 trans_utils-0.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-09 11:02 trans_utils-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    14281 b- defN 23-Apr-09 11:02 trans_utils-0.3.0.dist-info/RECORD
+158 files, 380387 bytes uncompressed, 116290 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -1,19 +1,112 @@
 Filename: tutils/__init__.py
 Comment: 
 
+Filename: tutils/classify.py
+Comment: 
+
 Filename: tutils/functools.py
 Comment: 
 
 Filename: tutils/initializer.py
 Comment: 
 
 Filename: tutils/tutils.py
 Comment: 
 
+Filename: tutils/contrib/__init__.py
+Comment: 
+
+Filename: tutils/contrib/ddp_demo.py
+Comment: 
+
+Filename: tutils/contrib/debug_tools.py
+Comment: 
+
+Filename: tutils/contrib/fourier.py
+Comment: 
+
+Filename: tutils/contrib/other_package.py
+Comment: 
+
+Filename: tutils/contrib/pudb_debug.py
+Comment: 
+
+Filename: tutils/contrib/shutils.py
+Comment: 
+
+Filename: tutils/contrib/tmp.py
+Comment: 
+
+Filename: tutils/contrib/proj-template/__init__.py
+Comment: 
+
+Filename: tutils/contrib/proj-template/code/__init__.py
+Comment: 
+
+Filename: tutils/contrib/proj-template/code/configs/__init__.py
+Comment: 
+
+Filename: tutils/contrib/proj-template/code/datasets/__init__.py
+Comment: 
+
+Filename: tutils/contrib/proj-template/code/networks/__init__.py
+Comment: 
+
+Filename: tutils/contrib/proj-template/code/scripts/__init__.py
+Comment: 
+
+Filename: tutils/contrib/proj-template/code/scripts/template.py
+Comment: 
+
+Filename: tutils/contrib/proj-template/code/test/__init__.py
+Comment: 
+
+Filename: tutils/contrib/proj-template/code/test/datasets/__init__.py
+Comment: 
+
+Filename: tutils/contrib/proj-template/code/test/networks/__init__.py
+Comment: 
+
+Filename: tutils/contrib/proj-template/code/test/utils/__init__.py
+Comment: 
+
+Filename: tutils/contrib/proj-template/code/tmp/__init__.py
+Comment: 
+
+Filename: tutils/contrib/proj-template/code/utils/__init__.py
+Comment: 
+
+Filename: tutils/contrib/proj-template/data/__init__.py
+Comment: 
+
+Filename: tutils/contrib/proj-template/related_work_1/__init__.py
+Comment: 
+
+Filename: tutils/contrib/proj-template/related_work_1/work1/__init__.py
+Comment: 
+
+Filename: tutils/contrib/proj-template/runs/__init__.py
+Comment: 
+
+Filename: tutils/contrib/test/__init__.py
+Comment: 
+
+Filename: tutils/contrib/test/test_builtins.py
+Comment: 
+
+Filename: tutils/contrib/test/test_initializer.py
+Comment: 
+
+Filename: tutils/contrib/test/test_print.py
+Comment: 
+
+Filename: tutils/contrib/test/test_pytest.py
+Comment: 
+
 Filename: tutils/mn/__init__.py
 Comment: 
 
 Filename: tutils/mn/data/__init__.py
 Comment: 
 
 Filename: tutils/mn/data/base_dataset.py
@@ -81,14 +174,17 @@
 
 Filename: tutils/mn/train/models/__init__.py
 Comment: 
 
 Filename: tutils/mn/train/models/cam_model.py
 Comment: 
 
+Filename: tutils/mn/train/models/debug_model.py
+Comment: 
+
 Filename: tutils/mn/train/models/unet_model.py
 Comment: 
 
 Filename: tutils/mn/train/models/unet_parts.py
 Comment: 
 
 Filename: tutils/mn/train/tloss/__init__.py
@@ -168,14 +264,56 @@
 
 Filename: tutils/proj-template/related_work_1/work1/__init__.py
 Comment: 
 
 Filename: tutils/proj-template/runs/__init__.py
 Comment: 
 
+Filename: tutils/test/__init__.py
+Comment: 
+
+Filename: tutils/test/test_builtins.py
+Comment: 
+
+Filename: tutils/test/test_initializer.py
+Comment: 
+
+Filename: tutils/test/test_print.py
+Comment: 
+
+Filename: tutils/test/test_pytest.py
+Comment: 
+
+Filename: tutils/tpackage/__init__.py
+Comment: 
+
+Filename: tutils/tpackage/_multilogger.py
+Comment: 
+
+Filename: tutils/tpackage/learner.py
+Comment: 
+
+Filename: tutils/tpackage/logger.py
+Comment: 
+
+Filename: tutils/tpackage/logger_utils.py
+Comment: 
+
+Filename: tutils/tpackage/monitor.py
+Comment: 
+
+Filename: tutils/tpackage/tester.py
+Comment: 
+
+Filename: tutils/tpackage/trainer.py
+Comment: 
+
+Filename: tutils/tpackage/trainer_utils.py
+Comment: 
+
 Filename: tutils/trainer/__init__.py
 Comment: 
 
 Filename: tutils/trainer/_bad_tuner_exec.py
 Comment: 
 
 Filename: tutils/trainer/ablation_exec.py
@@ -213,23 +351,29 @@
 
 Filename: tutils/trainer/save.py
 Comment: 
 
 Filename: tutils/trainer/simple_script_helper.py
 Comment: 
 
+Filename: tutils/trainer/tester_abstract.py
+Comment: 
+
 Filename: tutils/trainer/trainer.py
 Comment: 
 
 Filename: tutils/trainer/trainer_abstract.py
 Comment: 
 
 Filename: tutils/trainer/trainer_ddp.py
 Comment: 
 
+Filename: tutils/trainer/trainer_ddp2.py
+Comment: 
+
 Filename: tutils/trainer/tuner_exec.py
 Comment: 
 
 Filename: tutils/trainer/utils/__init__.py
 Comment: 
 
 Filename: tutils/trainer/utils/trainer_utils.py
@@ -255,38 +399,50 @@
 
 Filename: tutils/tutils/grad_cam.py
 Comment: 
 
 Filename: tutils/tutils/initializer.py
 Comment: 
 
+Filename: tutils/tutils/initializer_old.py
+Comment: 
+
 Filename: tutils/tutils/metriclogger.py
 Comment: 
 
 Filename: tutils/tutils/prologger.py
 Comment: 
 
 Filename: tutils/tutils/recorder.py
 Comment: 
 
+Filename: tutils/tutils/tconfig.py
+Comment: 
+
 Filename: tutils/tutils/techo.py
 Comment: 
 
 Filename: tutils/tutils/tlogger.py
 Comment: 
 
+Filename: tutils/tutils/torch_utils.py
+Comment: 
+
 Filename: tutils/tutils/ttimer.py
 Comment: 
 
 Filename: tutils/tutils/tutils.py
 Comment: 
 
 Filename: tutils/tutils/visualizers/__init__.py
 Comment: 
 
+Filename: tutils/tutils/visualizers/draw_bar_auto_split.py
+Comment: 
+
 Filename: tutils/tutils/visualizers/draw_curves.py
 Comment: 
 
 Filename: tutils/tutils/visualizers/plt_print_3d.py
 Comment: 
 
 Filename: tutils/tutils/visualizers/print_image.py
@@ -294,23 +450,26 @@
 
 Filename: tutils/tutils/visualizers/print_landmark.py
 Comment: 
 
 Filename: tutils/tutils/visualizers/tsne.py
 Comment: 
 
-Filename: trans_utils-0.2.2.dist-info/METADATA
+Filename: trans_utils-0.3.0.dist-info/LICENSE
+Comment: 
+
+Filename: trans_utils-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: trans_utils-0.2.2.dist-info/WHEEL
+Filename: trans_utils-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: trans_utils-0.2.2.dist-info/entry_points.txt
+Filename: trans_utils-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: trans_utils-0.2.2.dist-info/top_level.txt
+Filename: trans_utils-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: trans_utils-0.2.2.dist-info/RECORD
+Filename: trans_utils-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tutils/__init__.py

```diff
@@ -1,2 +1,3 @@
 # from tutils import *
-from tutils.tutils import *
+from tutils.tutils import *
+from .mn import *
```

## tutils/mn/data/__init__.py

```diff
@@ -0,0 +1,2 @@
+00000000: 6672 6f6d 202e 7473 6974 6b20 696d 706f  from .tsitk impo
+00000010: 7274 202a                                rt *
```

## tutils/mn/data/augment/common_2d_aug.py

```diff
@@ -138,14 +138,43 @@
         i, j, h, w = self.get_params(imgs[self.keys[0]], self.scale, self.ratio)
         for k, img in imgs.items():
             if k in self.keys:
                 imgs[k] = F.resized_crop(img, i, j, h, w, self.size, self.interpolation)
         return imgs
 
 
+class RandomAffine(transforms.RandomAffine):
+    def __init__(self, keys, *args, **kwargs) -> None:
+        self.keys = keys
+        super().__init__(*args, **kwargs)
+
+    def forward(self, imgs):
+        """
+            img (PIL Image or Tensor): Image to be transformed.
+
+        Returns:
+            PIL Image or Tensor: Affine transformed image.
+        """
+        fill = self.fill
+        if isinstance(imgs[self.keys[0]], Tensor):
+            if isinstance(fill, (int, float)):
+                fill = [float(fill)] * F.get_image_num_channels(imgs[self.keys[0]])
+            else:
+                fill = [float(f) for f in fill]
+
+        img_size = F.get_image_size(imgs[self.keys[0]])
+
+        ret = self.get_params(self.degrees, self.translate, self.scale, self.shear, img_size)
+
+        for k, img in imgs.items():
+            if k in self.keys:
+                imgs[k] = F.affine(img, *ret, interpolation=self.interpolation, fill=fill)
+        return imgs
+
+
 def usage():
     from torchvision.utils import save_image
     aug = transforms.Compose([
         RandomRotation(keys=['image', 'label'], degrees=(-10,10)),
         RandomResizedCrop(keys=['image', 'label'], size=(224,224)),
         RandomHorizontalFlip(keys=['image', 'label']),
         ColorJitter(keys=['image',], brightness=0.15, contrast=0.25),
```

## tutils/mn/data/tsitk/__init__.py

```diff
@@ -1 +1,2 @@
-from .io import *
+from .io import *
+# from .preprocess import *
```

## tutils/mn/data/tsitk/io.py

```diff
@@ -1,12 +1,10 @@
 import SimpleITK as sitk
 import numpy as np
 import os
-import sys
-import cv2
 
 # ----------------------
 # A useful package for loading radiological images
 from medpy.io import load
 
 def read2(*args, **kwargs):
     image_data, image_header = load(*args, **kwargs)
```

## tutils/mn/eval/radio_analysis/example_helloFeatureClass.py

```diff
@@ -53,14 +53,15 @@
   image, mask = imageoperations.resampleImage(image, mask, **settings)
 
 bb, correctedMask = imageoperations.checkMask(image, mask)
 if correctedMask is not None:
   mask = correctedMask
 image, mask = imageoperations.cropToTumorMask(image, mask, bb)
 
+import ipdb; ipdb.set_trace()
 #
 # Show the first order feature calculations
 #
 firstOrderFeatures = firstorder.RadiomicsFirstOrder(image, mask, **settings)
 
 # firstOrderFeatures.enableFeatureByName('Mean', True)
 firstOrderFeatures.enableAllFeatures()
```

## tutils/mn/train/models/cam_model.py

```diff
@@ -34,40 +34,42 @@
         cam = np.zeros(feature_map.shape[1:], dtype=np.float32)  # cam shape (H, W)
         weights = np.mean(grads, axis=(1, 2))  #
 
         for i, w in enumerate(weights):
             cam += w * feature_map[i, :, :]
 
         cam = np.maximum(cam, 0)
-        cam = cv2.resize(cam, (32, 32))
+        # cam = cv2.resize(cam, (32, 32))
+        
         _min = np.min(cam)
         _max = np.max(cam)
         cam -= _min
         cam /= np.max(cam)
         return {"cam":cam, "min":_min, "max":_max}
 
-    def show_on_img(self,input_img):
+    def show_on_img(self,input_img, fname='grad_feature.jpg'):
         '''
         write heatmap on target img
         :param input_img: cv2:ndarray/img_pth
         :return: save jpg
         '''
         if isinstance(input_img,str):
             input_img = cv2.imread(input_img)
         img_size = (input_img.shape[1],input_img.shape[0])
         fmap = self.feature_res[0].cpu().data.numpy().squeeze()
         grads_val = self.grad_res[0].cpu().data.numpy().squeeze()
         cam_info = self.gen_cam(fmap, grads_val)
-        cam = cam_info['cam']
+        cam = cam_info['cam'].copy()
         cam = cv2.resize(cam, img_size)
         heatmap = cv2.applyColorMap(np.uint8(255 * cam), cv2.COLORMAP_JET)/255.
         cam = heatmap + np.float32(input_img/255.)
         cam = cam / np.max(cam)*255
-        cv2.imwrite('grad_feature.jpg',cam)
-        print('save gradcam result in grad_feature.jpg')
+        cv2.imwrite(fname,cam)
+        print(f'save gradcam result in {fname}')
+        return cam_info
 
 
 def usage():
     import os
     from PIL import Image
     import torch
     import torch.nn as nn
@@ -140,15 +142,15 @@
         one_hot = torch.zeros(1, 10).scatter_(1, index, 1)
         one_hot.requires_grad = True
         class_vec = torch.sum(one_hot * output)  # one_hot = 11.8605
 
         return class_vec
 
     BASE_DIR = os.path.dirname(os.path.abspath(__file__))
-    path_img = os.path.join("cat.png")
+    path_img = os.path.join("../../../_paper_writing/corgi1.jpg")
     assert os.path.exists(path_img), f"path img: {path_img}"
     # path_net = os.path.join("./net.pth") # in this example not use
 
     classes = ('plane', 'car', 'bird', 'cat', 'deer', 'dog', 'frog', 'horse', 'ship', 'truck')
 
     # 图片读取；网络加载
     img = cv2.imread(path_img)  # H*W*C
```

## tutils/trainer/learner.py

```diff
@@ -60,52 +60,68 @@
     @abstractmethod
     def testing_step(self, data, batch_idx, **kwargs):
         pass
 
     def on_before_zero_grad(self, **kwargs):
         pass
 
+    def on_after_zero_grad(self, **kwargs):
+        pass
+
     def info(self, msg, *args, **kwargs):
         if self.logger is not None:
             self.logger.info(msg, *args, **kwargs)
         else:
             print(msg, *args, **kwargs)
 
-    def load(self, pth=None, *args, **kwargs):
+    def load(self, pth=None, force_match=False, *args, **kwargs):
         assert os.path.exists(pth)
-        print(f'Load CKPT from ``{pth}``')
-        state_dict = torch.load(pth)
-        self.net.load_state_dict(state_dict)
+        if not force_match:
+            print(f'Load CKPT from ``{pth}``')
+            state_dict = torch.load(pth)
+            self.net.load_state_dict(state_dict)
 
+        """ Force-match """
         # new_state_dict = OrderedDict()
         # for k, v in state_dict.items():
         #     if not k.startswith("module.target_encoder.net."):
         #         print("skip: ", k)
         #         continue
         #     name = k.replace("module.target_encoder.net.", "")
         #     new_state_dict[name] = v
         # self.net.load_state_dict(new_state_dict)
 
+        """ Load Partial Model
+             1. filter out unnecessary keys
+             2. overwrite entries in the existing state dict
+             3. load the new state dict
+        """
+        # model_dict = self.net.state_dict()
+        # pretrained_dict = {k: v for k, v in pretrained_dict.items() if k in model_dict}
+        # model_dict.update(pretrained_dict)
+        # self.net.load_state_dict(model_dict)
+
     def save(self, pth, *args, **kwargs):
         # Default: "/model_epoch_{}.pth".format(epoch)
         torch.save(self.net.module.state_dict(), pth)
         return True
 
     def configure_logger(self, *args, **kwargs):
         logger = MultiLogger(logdir=self.config['base']['runs_dir'],
                              mode=self.config['logger']['mode'],
                              tag=self.config['base']['tag'],
                              extag=self.config['base'].get('experiment', None),
                              action=self.config['logger'].get('action', 'k'))
         return {'logger': logger}
 
     def save_optim(self, pth, optimizer, epoch=0, *args, **kwargs):
-        stat = {'optimizer': optimizer.state_dict(), 'epoch': epoch}
-        torch.save(stat, pth)
-        return True
+        pass
+        # stat = {'optimizer': optimizer.state_dict(), 'epoch': epoch}
+        # torch.save(stat, pth)
+        # return True
         # pass
 
     def load_optim(self, optimizer, pth=None, *args):
         # state_dict = torch.load(pth)
         # optimizer.load_state_dict(state_dict['optimizer'])
         # start_epoch = state_dict.get('epoch', 0) + 1
         # return start_epoch
```

## tutils/trainer/learner_module.py

```diff
@@ -48,27 +48,31 @@
     @abstractmethod
     def testing_step(self, data, batch_idx, **kwargs):
         pass
 
     def on_before_zero_grad(self, **kwargs):
         pass
 
+    def on_after_zero_grad(self, **kwargs):
+        pass
+
     def info(self, msg, *args, **kwargs):
         if self.logger is not None:
             self.logger.info(msg, *args, **kwargs)
         else:
             print(msg, *args, **kwargs)
 
     def load(self, pth=None, *args, **kwargs):
-        assert os.path.exists(pth)
+        assert os.path.exists(pth), f"Error Path: {pth}"
         print(f'Load CKPT from ``{pth}``')
         state_dict = torch.load(pth)
         self.net.load_state_dict(state_dict)
 
         # new_state_dict = OrderedDict()
+        # state_dict = torch.load(pth)
         # for k, v in state_dict.items():
         #     if not k.startswith("module.target_encoder.net."):
         #         print("skip: ", k)
         #         continue
         #     name = k.replace("module.target_encoder.net.", "")
         #     new_state_dict[name] = v
         # self.net.load_state_dict(new_state_dict)
@@ -76,15 +80,15 @@
     def save(self, pth, *args, **kwargs):
         # Default: "/model_epoch_{}.pth".format(epoch)
         torch.save(self.net.module.state_dict(), pth)
         return True
 
     def configure_logger(self, *args, **kwargs):
         logger = MultiLogger(logdir=self.config['base']['runs_dir'],
-                             mode=self.config['logger']['mode'],
+                             mode=self.config['logger'].get('mode', None),
                              tag=self.config['base']['tag'],
                              extag=self.config['base'].get('experiment', None),
                              action=self.config['logger'].get('action', 'k'))
         return {'logger': logger}
 
     def save_optim(self, pth, optimizer, epoch=0, *args, **kwargs):
         stat = {'optimizer': optimizer.state_dict(), 'epoch': epoch}
```

## tutils/trainer/recorder.py

```diff
@@ -5,59 +5,61 @@
 import torch
 import numpy as np
 from tutils import tfunctime
 from typing import Dict, List, Tuple
 
 
 class Recorder(object):
-    def __init__(self, logger=None, config=None, reduction="mean"):
+    def __init__(self, logger=None, config=None, reduction="mean", inclusion=None):
         super(Recorder, self).__init__()
         self.logger = logger
         self.config = config
         self.loss_list = []
         self.loss_keys = None
         self.reduction = reduction
+        self.inclusion = inclusion
 
     def clear(self):
         self.loss_list.clear()
 
     def record(self, loss:dict) -> None:
         assert type(loss) == dict, f"Got {loss}"
         # print("debug record", loss)
         if self.loss_keys is None:
             self.loss_list = []
             self.loss_keys = loss.keys()
         l_list = []
         for key, value in loss.items():
-            if type(value) == torch.Tensor:
+            if isinstance(value, torch.Tensor):
                 l_list.append(value.detach().cpu().item())
-            elif type(value) in [str, bool]:
+            elif isinstance(value, (str, bool, list, dict)):
                 pass
-            elif type(value) in [np.ndarray, np.float64, np.float32, int, float]:
+            elif isinstance(value, (np.ndarray, np.float64, np.float32, int, float)):
                 l_list.append(float(value))
             else:
                 print("debug??? type Error? , got ", type(value))
                 print("debug??? ", key, value)
+                raise ValueError
                 l_list.append(float(value))
         self.loss_list.append(l_list)
 
     def _record(self, loss):
-        if type(loss) == torch.Tensor:
+        if isinstance(loss, torch.Tensor):
             loss = loss.detach().cpu().item()
             if self.loss_list is None:
                 self.loss_list = []
             self.loss_list.append(loss)
-        elif type(loss) == list:
+        elif isinstance(loss, list):
             for i, lossi in enumerate(loss):
                 if type(lossi) == torch.Tensor:
                     loss[i] = lossi.detach().cpu().item()
             if self.loss_list is None:
                 self.loss_list = []
             self.loss_list.append(loss)
-        elif type(loss) == dict:
+        elif isinstance(loss, dict):
             if self.loss_list is None:
                 self.loss_list = []
                 self.loss_keys = loss.keys
             l_list = []
             for lossi, value in loss.items():
                 if type(lossi) == torch.Tensor:
                     l_list.append(lossi.detach().cpu().item())
```

## tutils/trainer/trainer.py

```diff
@@ -1,13 +1,16 @@
 # coding: utf-8
 import torch
 import numpy as np
 from torch import nn
 from torch.utils.data import DataLoader, Dataset
 from .trainer_abstract import AbstractTrainer
+from torch.cuda.amp import autocast, GradScaler
+from tutils.tutils import tfilename, CSVLogger, MultiLogger
+from tutils.trainer.recorder import Recorder
 
 # def trainer_from_config(logger, config, tester, monitor, **kwargs):
 #     config_base = config['base']
 #     config_train = config['training']
 #     return Trainer(logger=logger,
 #                    config=config,
 #                    tester=tester,
@@ -39,15 +42,28 @@
         """
             mode:
                 ps:  Parameter Server
                 ddp: Distributed data parallel
         """
         super(Trainer, self).__init__(config, tester, monitor, rank='cuda', world_size=0)
         self.logger = logger
-
+        
+        if self.use_amp:
+            self.scalar = GradScaler()
+            print("Debug settings: use amp=",self.use_amp)
+        
+        if self.logging_available:
+            print("Logger at Process(rank=0)")
+            self.recorder = Recorder(reduction=self.recorder_mode)
+            self.recorder_test = Recorder(reduction=self.recorder_mode)
+            self.logger = None
+            self.csvlogger = CSVLogger(tfilename(self.runs_dir, "best_record"))
+            self.csvlogger_all = CSVLogger(tfilename(self.runs_dir, "all_record"))
+            self.monitor = monitor
+            self.tester = tester
 
     def init_model(self, model, trainset, **kwargs):
         assert len(trainset) > 0 , f"Got {len(trainset)}"
         self.trainloader = DataLoader(dataset=trainset,
                                       batch_size=self.batch_size,
                                       num_workers=self.num_workers,
                                       shuffle=True,
```

## tutils/trainer/trainer_abstract.py

```diff
@@ -1,75 +1,108 @@
 
 import torch
 from tutils.tutils.ttimer import tenum, timer
 from tutils.tutils import tfilename, CSVLogger, MultiLogger
 from torch.cuda.amp import autocast, GradScaler
 from tutils.trainer.recorder import Recorder
 from .utils.trainer_utils import MultiOptimizer, MultiScheduler, VoidTimer, dict_to_str, _get_time_str
+import random
+import numpy as np
 
+# torch.backends.cudnn.benchmark = True
+
+# all config settings
+
+# 'training': {
+#         'gpus': None,
+#         'ddp': {
+#             'master_addr': 'localhost',
+#             'master_port': '25807',
+#             },
+#         'num_epochs' : 2500, 
+#         'batch_size' : 8,
+#         'num_workers' : 8,
+#         'save_interval' : 50,
+#         'load_pretrain_model': False,
+#         'load_optimizer': False,
+#         'val_check_interval': 10,
+#         'use_amp': False,
+#         'training_log_interval': 1,
+#         'save_latest_only': False,
+#         'save_all_records': True,
+#     },
+
+
+def reproducibility(seed):
+    random.seed(seed)
+    np.random.seed(seed)
+    torch.manual_seed(seed)
+    torch.cuda.manual_seed(seed)
+    torch.cuda.manual_seed_all(seed)
+    torch.backends.cudnn.deterministic = True
+    torch.backends.cudnn.benchmark = False
+    torch.autograd.set_detect_anomaly(True)
 
 
 class AbstractTrainer:
     def __init__(self,
                  config,
-                 tester,
-                 monitor,
+                 logger=None,
+                 tester=None,
+                 monitor=None,
                  rank='cuda',
                  world_size=0,
                  ):
         self.config = config
         self.rank = rank
         self.world_size = world_size
         self.tester = tester
+        self.logger = None
         # base
         self.tag = config['base']['tag']
         self.runs_dir = config['base']['runs_dir']
         #
         self.max_epochs = config['training'].get('num_epochs', 400)
         self.batch_size = config["training"].get('batch_size', 4)
         self.num_workers = config['training'].get('num_workers', 0)
         self.save_interval = config['training'].get('save_interval', 50)
-
         self.load_pretrain_model = config['training'].get('load_pretrain_model', False)
         self.pretrain_model = config['training'].get('pretrain_model', None)
         self.load_optimizer = config['training'].get('load_optimizer', False)
         self.val_check_interval = config['training'].get('val_check_interval', 50)
         self.training_log_interval = config['training'].get('training_log_interval', 1)
         self.use_amp = config['training'].get('use_amp', False)
+        self.start_epoch = config['training'].get('start_epoch', 0)
+        self.save_all_records = config['training'].get('save_all_records', True)
+        self.save_mode = config['training'].get('save_mode', ['best', 'latest', 'all'])
         self.save_latest_only = config['training'].get('save_latest_only', False)
 
-        if self.rank != 'cuda' and self.world_size > 0:
-            self.master_addr = self.ddp_config.get('master_addr', 'localhost')
-            self.master_port = str(self.ddp_config.get('master_port', '25700'))
-            self.ddp_config = config['training'].get('ddp', dict())
-            self.dist_url = 'tcp://' + self.master_addr + ":" + self.master_port
-            torch.distributed.init_process_group(backend="nccl", init_method=self.dist_url,
-                                                 world_size=self.world_size, rank=self.rank)
-
         self.logging_available = (self.rank == 0 or self.rank == 'cuda')
         self.trainloader = None
         self.optimizer = None
         self.scheduler = None
-        self.init_timers()
+        
+        self.recorder_mode = config['logger'].get("recorder_reduction", "mean")
+        self.using_ddp = False
+
+        # Warning for deprecated func
+        if self.save_latest_only is True:
+            print("[Tutils] arg: save_latest_only is deprecated, please use [save_mode: ['all',  'best', 'latest'] ]")
+
+        # if self.rank != 'cuda' and self.world_size > 0:
+        #     self.ddp_config = config['training'].get('ddp', dict())
+        #     self.master_port = str(self.ddp_config.get('master_port', '25700'))
+        #     self.master_addr = self.ddp_config.get('master_addr', 'localhost')
+        #     self.dist_url = 'tcp://' + self.master_addr + ":" + self.master_port
+        #     torch.distributed.init_process_group(backend="nccl", init_method=self.dist_url,
+        #                                          world_size=self.world_size, rank=self.rank)
 
-        if self.use_amp:
-            self.scalar = GradScaler()
-            print("Debug settings: use amp=",self.use_amp)
 
         # Logging, in GPU 0
-        self.recorder_mode = config['logger'].get("recorder_reduction", "sum")
-        if self.logging_available:
-            print("Logger at Process(rank=0)")
-            self.recorder = Recorder(reduction=self.recorder_mode)
-            self.recorder_test = Recorder(reduction=self.recorder_mode)
-            self.logger = None
-            self.csvlogger = CSVLogger(tfilename(self.runs_dir, "best_record"))
-            self.monitor = monitor
-            self.tester = tester
-
+        
     def init_timers(self):
         self.timer_epoch = timer("one epoch") if self.logging_available else VoidTimer()
         self.timer_batch = timer("a batch") if self.logging_available else VoidTimer()
         self.timer_data = timer("data time") if self.logging_available else VoidTimer()
         self.timer_net = timer("net forwarding") if self.logging_available else VoidTimer()
         self.timer_eval = timer("evaluation") if self.logging_available else VoidTimer()
         self.timer_write = timer("writing files") if self.logging_available else VoidTimer()
@@ -95,62 +128,72 @@
         #     trainset, batch_size=per_device_batch_size, num_workers=self.num_worker,
         #     pin_memory=True, sampler=sampler, drop_last=True)
         # return model
         raise NotImplementedError
 
 
     def fit(self, model, trainset):
-        model = self.init_model(model, trainset)
+        model = self.init_model(model, trainset, rank=self.rank)
+        self.init_timers()
         optimizer, scheduler, start_epoch = self.configure_optim(model)
 
         for epoch in range(start_epoch, self.max_epochs):
             self.on_before_zero_grad()
             # Training
             self.timer_epoch()
             do_training_log = (epoch % self.training_log_interval == 0)
             self.train(model, self.trainloader, epoch, optimizer, scheduler, do_training_log)
 
             # epoch logger !
-            if do_training_log and self.logging_available:
-                _dict = self.recorder.cal_metrics()
-                _dict['time_total'] = self.timer_epoch()
+            if self.logging_available:
+                if do_training_log :
+                    _dict = self.recorder.cal_metrics()
+                    _dict['time_total'] = self.timer_epoch()
+
+                    # print(_dict)
+                    # assert isinstance(lr, float), f"Got lr={lr}, type: {type(lr)}"
+                    loss_str = ""
+                    for k, v in _dict.items():
+                        loss_str += "{}:{:.4f} ".format(k, v)
+                    # lr = optimizer.param_groups[0]['lr']
+                    lr = self.get_lr(optimizer)
+                    _dict['lr'] = lr
+                    loss_str += "{}:{:.6e} ".format('lr', lr)
+                    self.logger.info(f"Epoch {epoch}: {loss_str}")
+                    self.logger.add_scalars(_dict, step=epoch, tag='train')
+                    time_log_scalars = self.timer_epoch()
+                    self.on_after_training(d=_dict)
+                # Evaluation
+                if epoch % self.val_check_interval == 0 and self.logging_available:
+                    print("Note: Tester runs on <rank 0> only")
+                    if self.tester is not None:
+                        out = self.tester.test(model=model, epoch=epoch, rank=self.rank)
+                        if self.monitor is not None:
+                            best_dict = self.monitor.record(out, epoch)
+                            self.recorder_test.record({**best_dict, **out})
+                            if best_dict['isbest']:
+                                if 'best' in self.save_mode:
+                                    self.save(model, epoch, type='best')
+                                self.csvlogger.record({**best_dict, **out, "time": _get_time_str()})
+                            if self.save_all_records:
+                                self.csvlogger_all.record({**best_dict, **out, "time": _get_time_str()})
+                            self.logger.info(f"\n[*] {dict_to_str(best_dict)}[*] Epoch {epoch}: \n{dict_to_str(out)}")
+                            self.logger.add_scalars(out, step=epoch, tag='test')
+                            # if ''
+                        else:
+                            self.logger.info(f"\n[*] Epoch {epoch}: {dict_to_str(out)}")
+                        self.on_after_testing(d=out)
+                time_eval = self.timer_epoch()
+                if epoch % self.save_interval == 0 and self.logging_available:
+                    if 'latest' in self.save_mode:
+                        self.save(model, epoch, 'latest', optimizer)
+                    if 'all' in self.save_mode:
+                        self.save(model, epoch, None, optimizer)
+                    # time_save_model = self.timer_epoch()
 
-                # print(_dict)
-                # assert isinstance(lr, float), f"Got lr={lr}, type: {type(lr)}"
-                loss_str = ""
-                for k, v in _dict.items():
-                    loss_str += "{}:{:.4f} ".format(k, v)
-                # lr = optimizer.param_groups[0]['lr']
-                lr = self.get_lr(optimizer)
-                _dict['lr'] = lr
-                loss_str += "{}:{:.6e} ".format('lr', lr)
-                self.logger.info(f"Epoch {epoch}: {loss_str}")
-                self.logger.add_scalars(_dict, step=epoch, tag='train')
-                time_log_scalars = self.timer_epoch()
-            # Evaluation
-            if epoch % self.val_check_interval == 0 and self.logging_available:
-                print("Note: Tester runs on <rank 0> only")
-                if self.tester is not None:
-                    out = self.tester.test(model, epoch, self.rank)
-                    if self.monitor is not None:
-                        best_dict = self.monitor.record(out, epoch)
-                        self.recorder_test.record({**best_dict, **out})
-                        if best_dict['isbest']:
-                            self.save(model, epoch, type='best')
-                            self.csvlogger.record({**best_dict, **out, "time": _get_time_str()})
-                        self.logger.info(f"\n[*] {dict_to_str(best_dict)}[*] Epoch {epoch}: \n{dict_to_str(out)}")
-                        self.logger.add_scalars(out, step=epoch, tag='test')
-                    else:
-                        self.logger.info(f"\n[*] Epoch {epoch}: {dict_to_str(out)}")
-            time_eval = self.timer_epoch()
-            if epoch % self.save_interval == 0 and self.logging_available:
-                self.save(model, epoch, 'latest', optimizer)
-                time_save_model = self.timer_epoch()
-            # dd = {"time_train": _dict['time_total'], "time_log_scalars":time_log_scalars, "time_eval":time_eval, "time_save_model": time_save_model}
-            # print(dd)
         print("Training is Over for GPU rank ", self.rank)
         self.cleanup()
 
     def configure_optim(self, model, **kwargs):
         # Set optimizer and scheduler
         optim_configs = model.configure_optimizers()
         assert isinstance(optim_configs, dict)
@@ -160,61 +203,68 @@
         if isinstance(optimizer, list):
             optimizer = MultiOptimizer(optimizer)
         if isinstance(scheduler, list):
             scheduler = MultiScheduler(scheduler)
         if self.load_optimizer:
             start_epoch = model.load_optim(optimizer)
         else:
-            start_epoch = 0
+            start_epoch = self.start_epoch
         return optimizer, scheduler, start_epoch
 
-
     def on_before_zero_grad(self, **kwargs):
         pass
 
     def train(self, model, trainloader, epoch, optimizer, scheduler=None, do_training_log=True):
         model.train()
         out = {}
         if do_training_log and self.logging_available:
             self.recorder.clear()
             time_record = 0.1111
             self.timer_batch()
 
+        success_count = 0
+        failed_count = 0
         for load_time, batch_idx, data in tenum(trainloader):
             model.on_before_zero_grad()
             optimizer.zero_grad()
             self.timer_data()
             # training steps
             for k, v in data.items():
                 if type(v) == torch.Tensor:
                     data[k] = v.to(self.rank)
             time_data_cuda = self.timer_data()
             if self.use_amp:
                 with autocast():
                     self.timer_net()
-                    out = model.training_step(data, batch_idx)
+                    out = model.training_step(data, batch_idx, epoch=epoch)
                     assert isinstance(out, dict)
                     time_fd = self.timer_net()
                     loss = out['loss']
                     self.scalar.scale(loss).backward()
                     self.scalar.step(optimizer)
                     self.scalar.update()
                     time_bp = self.timer_net()
             else:
                 self.timer_net()
-                out = model.training_step(data, batch_idx)
+                out = model.training_step(data, batch_idx, epoch=epoch)
+                if out['loss'] is None:
+                    failed_count += 1
+                    print(f"Ignore None loss, Success Ratio: {success_count / (success_count + failed_count)}")
+                    continue
                 if torch.isnan(out['loss']):
                     print("Nan Value: ", out['loss'])
-                    raise ValueError
+                    failed_count += 1
+                    raise ValueError(f"Get loss: {out['loss']}")
                 assert isinstance(out, dict)
                 time_fd = self.timer_net()
                 loss = out['loss']
                 loss.backward()
                 optimizer.step()
                 time_bp = self.timer_net()
+                success_count += 1
 
             time_batch = self.timer_batch()
             # batch logger !
             if do_training_log and self.logging_available:
                 out['time_load'] = load_time
                 out['time_cuda'] = time_data_cuda
                 out['time_forward'] = time_fd
@@ -224,44 +274,54 @@
                 self.timer_data()
                 self.recorder.record(out)
                 time_record = self.timer_data()
             # for debug !
             if epoch == 0:
                 if self.logging_available:
                     self.logger.info("[*] Debug Checking Pipeline !!!")
-                break
+                return
+            model.on_after_zero_grad(d=out)
         if scheduler is not None:
-            scheduler.step()
-        self.on_after_training(d=out)
+            scheduler.step()        
+        if self.logging_available:
+            self.logger.info(f"Training Success Ratio: {success_count / (success_count + failed_count)}")
+    
+
+    def on_after_zero_grad(self, d, *args, **kwargs):
+        pass
 
     def on_after_training(self, d, *args, **kwargs):
         pass
 
+    def on_after_testing(self, d, *args, **kwargs):
+        pass
+
     def save(self, model, epoch, type=None, optimizer=None, **kwargs):
         if self.logging_available:
             if type is None:
-                if self.save_interval > 0 and epoch % self.save_interval == 0:
-                    save_name = "/ckpt/model_epoch_{}.pth".format(epoch)
-                    model.save(tfilename(self.runs_dir, save_name), epoch=epoch)
-                    self.logger.info(f"Epoch {epoch}: Save model to ``{save_name}``! ")
+                # if self.save_interval > 0 and epoch % self.save_interval == 0:
+                save_name = "/ckpt/model_epoch_{}.pth".format(epoch)
+                model.save(tfilename(self.runs_dir, save_name), epoch=epoch)
+                self.logger.info(f"Epoch {epoch}: Save model to ``{save_name}``! ")
             elif type == 'best':
-                save_name = "/ckpt/best_model_epoch_{}.pth".format(epoch)
-                model.save(tfilename(self.runs_dir, save_name), epoch=epoch, is_best=True)
-                self.logger.info(f"[Best model] Epoch {epoch}: Save model to ``{save_name}``! ")
+                # save_name = "/ckpt/best_model_epoch_{}.pth".format(epoch)
+                save_name2 = "/ckpt_v/model_best.pth"
+                # model.save(tfilename(self.runs_dir, save_name), epoch=epoch, is_best=True)
+                model.save(tfilename(self.runs_dir, save_name2), epoch=epoch, is_best=True)
+                self.logger.info(f"[Best model] Epoch {epoch}: Save model to ``{save_name2}``! ")
             elif type == 'latest':
                 if self.save_interval > 0 and epoch % self.save_interval == 0:
-                    save_name = "/ckpt/model_latest.pth"
+                    save_name = "/ckpt_v/model_latest.pth"
                     model.save(tfilename(self.runs_dir, save_name), epoch=epoch, is_latest=True)
                     save_optim_name = "/ckpt/optim_latest.pth"
                     model.save_optim(tfilename(self.runs_dir, save_optim_name), optimizer=optimizer, epoch=epoch)
                     self.logger.info(f"Epoch {epoch}: Save checkpoint to ``{save_name}``")
 
     def cleanup(self):
-        if self.rank != 'cuda':
-            torch.distributed.destroy_process_group()
+        pass
 
     def info(self, msg, *args, **kwargs):
         if self.logging_available:
             self.logger.info(msg, *args, **kwargs)
 
     def get_lr(self, optimizer):
         if isinstance(optimizer, MultiOptimizer):
```

## tutils/tutils/__init__.py

```diff
@@ -1,13 +1,15 @@
 from .tutils import *
 # from .timer import tenum, tfunctime
 from .ttimer import *
 # from .tlogger import trans_init, trans_args, dump_yaml
-from .tlogger import MultiLogger, MultiRecorder
+from .tlogger import MultiLogger, MultiRecorder, TBLogger
 from .techo import *
-from .initializer import trans_configure, trans_init, trans_args
+from .initializer import BASE_CONFIG, TConfig, get_logger
 from .functools import print_dict
-from .dl_utils import *
+# from .dl_utils import *
+from .torch_utils import *
 from .visualizers import *
 from .metriclogger import MetricLogger
 from .prologger import ProLogger
-from .csv_recorder import CSVLogger
+from .csv_recorder import CSVLogger
+from .recorder import Recorder
```

## tutils/tutils/csv_recorder.py

```diff
@@ -3,14 +3,15 @@
 from typing import List
 import numpy as np
 from .tutils import tfilename
 from datetime import datetime
 import os
 import csv
 import pandas as pd
+from .functools import tprint
 
 
 def _get_time_str():
     return datetime.now().strftime('%Y-%m-%d %H:%M:%S')
 
 
 class CSVLogger(object):
@@ -26,19 +27,19 @@
         self.filename = tfilename(self.logdir, name)
         self.mode = mode
         
         if mode == "w":
             if os.path.isfile(self.filename):
                 backup_name = self.filename.replace(".csv", "."+_get_time_str()+".csv")
                 shutil.move(self.filename, backup_name)
-                print(f"[CSVLogger] backup excel file `{self.filename}` to `{backup_name}`")
+                tprint(f"[CSVLogger] backup excel file `{self.filename}` to `{backup_name}`")
         elif mode == "a+":
-            print("[CSVLogger] Add data on existing CSV file!")
-            # self.previous_data = self.read_previous(logdir + "/record.csv")
-            self._keys_write_state_ = True
+            tprint("[CSVLogger] Add data on existing CSV file!")
+            if os.path.isfile(self.filename):
+                self._keys_write_state_ = True
         else:
             raise NotImplementedError
  
     def record(self, d):
         assert type(d) == dict, f"Got {type(d)}"
         # Add record time
         d['record_time'] = _get_time_str()
@@ -78,15 +79,15 @@
         # States
         self._keys_write_state_ = False
         self.filename = tfilename(self.logdir, name)
         # Backup previous file
         if os.path.isfile(self.filename):
             backup_name = self.filename.replace(".xls", "."+_get_time_str()+".xls")
             shutil.move(self.filename, backup_name)
-            print(f"[ExcelLogger] backup excel file `{self.filename}` to `{backup_name}`")
+            tprint(f"[ExcelLogger] backup excel file `{self.filename}` to `{backup_name}`")
 
         self.file = xlwt.Workbook(encoding='utf-8')
         self.table = self.file.add_sheet('data')
 
     def reset(self):
         self._keys_write_state_ = False
         self.col_index = 0
@@ -103,15 +104,15 @@
             Open sheet -> write data -> save sheet
         """
         assert type(row) == list , f"Got {type(row)}"
         i = self.col_index
         for j, v in enumerate(row):
             # standardize types
             v = self.standardize(v)
-            # print("debug ", i, j, v, type(v))
+            # tprint("debug ", i, j, v, type(v))
             self.table.write(i, j, v)
         self.col_index += 1
         self.file.save(self.filename)
 
     def standardize(self, v):
         if type(v) in [str, int, float]:
             return v
```

## tutils/tutils/functools.py

```diff
@@ -1,10 +1,22 @@
 from pathlib import Path
 from datetime import datetime
 from collections import OrderedDict
+from .tconfig import _C
+
+
+def tprint(*args, **kwargs):
+    print("[Tutils] ", end="")
+    print(*args, **kwargs)
+
+
+def dprint(*args, **kwargs):
+    if _C.TUTILS_DEBUG:
+        print("[Tutils Debug] ", end="")
+        print(*args, **kwargs)
 
 
 def _get_time_str():
     return datetime.now().strftime('%m%d-%H%M%S')
 
 
 def _clear_config(config):
@@ -60,28 +72,14 @@
             if not isinstance(v, dict):
                 _d = {**_d, **{s+k: v}}
             else:
                 _d = {**_d, **flatten_dict(d[k], s + k)}
         return _d
 
 
-# def time_now():
-#     return time.strftime("%Y%m%d-%H%M%S", time.localtime())
-
-
-# def generate_random_str(n: int = 6):
-#     ran_str = ''.join(random.sample(string.ascii_letters + string.digits, n))
-#     return ran_str
-
-
-# def generate_name():
-#     return time_now() + '-' + generate_random_str(6)
-
-
-
 def _ordereddict_to_dict(d):
     if not isinstance(d, dict):
         return d
     for k, v in d.items():
         if type(v) == OrderedDict:
             v = _ordereddict_to_dict(v)
             d[k] = dict(v)
@@ -90,59 +88,37 @@
         elif type(v) == dict:
             d[k] = _ordereddict_to_dict(v)
     return d
 
 
 
 
-
-
-
-
 ######################################################
 
-class Config(object):
-    def __init__(self):
-        super().__init__()
-        self.TUTILS_DEBUG = False
-        self.TUTILS_INFO = False
-        self.TUTILS_WARNING = True
-
-    def set_print_debug(self, setting=True):
-        self.TUTILS_DEBUG = setting
-
-    def set_print_info(self, setting=True):
-        self.TUTILS_INFO = setting
-
-    def set_print_warning(self, setting=True):
-        self.TUTILS_WARNING = setting
-
-tconfig = Config()
-
-def tprint(*s, end="\n", **kargs):
+def _tprint(*s, end="\n", **kargs):
     if len(s) > 0:
         for x in s:
             print(x, end="")
         print("", end=end)
     if len(kargs) > 0:
         for key, item in kargs.items():
             print(key, end=": ")
             print(item, end="")
         print("", end=end)
 
 
 def p(*s, end="\n", **kargs):
-    if tconfig.TUTILS_INFO or tconfig.TUTILS_DEBUG or tconfig.TUTILS_WARNING:
-        print("[Trans Info] ", end="")
-        tprint(*s, end="\n", **kargs)
+    if _C.TUTILS_INFO or _C.TUTILS_DEBUG or _C.TUTILS_WARNING:
+        print("[Tutils Info] ", end="")
+        _tprint(*s, end="\n", **kargs)
 
 
 def w(*s, end="\n", **kargs):
-    if tconfig.TUTILS_WARNING or tconfig.TUTILS_DEBUG:
-        print("[Trans Warning] ", end="")
-        tprint(*s, end="\n", **kargs)
+    if _C.TUTILS_WARNING or _C.TUTILS_DEBUG:
+        print("[Tutils Warning] ", end="")
+        _tprint(*s, end="\n", **kargs)
 
 
 def d(*s, end="\n", **kargs):
-    if tconfig.TUTILS_DEBUG:
-        print("[Trans Debug] ", end="")
-        tprint(*s, end="\n", **kargs)
+    if _C.TUTILS_DEBUG:
+        print("[Tutils Debug] ", end="")
+        _tprint(*s, end="\n", **kargs)
```

## tutils/tutils/initializer.py

```diff
@@ -16,103 +16,161 @@
 import sys
 from collections import OrderedDict
 from datetime import datetime
 import os
 
 from .tlogger import MultiLogger
 from .tutils import dump_yaml, save_script
-from .functools import _clear_config, _print_dict
 import copy
+from .functools import _clear_config, _print_dict, tprint
+from .tutils import save_script
+from typing import Any, Dict, List
+from .tutils import tfilename,_get_time_str
+
+import shutil
 
 
 
 BASE_CONFIG = {
+    # params used in Initializer
     'base': {
         'base_dir': './runs_debug/',
         'experiment': "",
         'tag': '',
         'stage': '', 
         'extag': '',
         'config': '',
         'test': False,
-        'func': '',
+        'func': 'train',
         'gpus': '',
         'ms': False,
+        'runs_dir': None, # 
         },    
+    # params used in Logger
     'logger':{
-        'mode': None, # "wandb", "tensorboard", 'csv'
+        'use_logger': True,
+        'record_mode': ["tensorboard"], # "wandb", "tensorboard", 'csv'
         'action': 'k', 
-    }
+        'logging_mode': None,
+    },
+    'training': {
+        'gpus': None,
+        'ddp': {
+            'master_addr': 'localhost',
+            'master_port': '25807',
+            },
+        'num_epochs' : 2500, 
+        'batch_size' : 8,
+        'num_workers' : 8,
+        'save_interval' : 50,
+        'load_pretrain_model': False,
+        'load_optimizer': False,
+        'val_check_interval': 10,
+        'use_amp': False,
+        'training_log_interval': 1,
+        'save_latest_only': False,
+        'save_all_records': True,
+    },
 }
 
+class TConfig:
+    def __init__(self, file, mode:str, parser, ex_config=None, clear_none=True, saving_script=True, **kwargs) -> None:
+        self.file = file
+        self.default_parser = parser
+        if mode.lower() in ['sc', 'script']:            self.mode = "sc"
+        elif mode.lower() in ['nb', 'notebook']:            self.mode = "nb"
+        elif mode.lower() in ['ddp', 'dp']:            self.mode = "ddp"
+        else:            raise ValueError(f"TypeError, Got {mode}")
+        self.logger = None
+        self.args = None
+        self.config = self._set_config(parser=parser, ex_config=ex_config, file=file, clear_none=clear_none, saving_script=saving_script)
+
+    def _set_config(self, parser=None, ex_config=None, file=None, clear_none=True, saving_script=True, **kwargs):
+        # Load configs in args
+        if self.mode == "sc":
+            args = trans_args(parser)
+            self.args = args
+            assert args is not None
+        else: args = None
+
+        # Load configs in config.yaml
+        file_config = None
+        if args is not None: 
+            if args.config is not None:
+                with open(args.config) as f:
+                    file_config = yaml.load(f, Loader=yamlloader.ordereddict.CLoader)
+
+        # Merge configs
+        config = merge_configs(args=args, file_config=file_config, ex_config=ex_config, clear_none=clear_none)
+        
+        # Setup path of runs_dir
+        if self.file is not None or file is not None:
+            parent, name = os.path.split(self.file)
+            name = name[:-3]
+            print(f"Change experiment name from {config['base']['experiment']} to {name}")
+            config['base']['experiment'] = name
+        config = _check_config(config)
+        config['base']['__INFO__']['Argv'] = "Argv: python " + ' '.join(sys.argv)
+
+        # Save scripts
+        if saving_script and file is not None:
+            print(f"Save running script to {config['base']['runs_dir']} from {file}")
+            save_script(config['base']['runs_dir'], file)
+        
+        self.config = config
+        return config
+
+    def get_logger(self, **kwargs):
+        if self.config is None:
+            raise ValueError("Please call 'TConfig.get_config(...)' first! ")
+        config = self.config
+        logger = get_logger(config)
+        config['base']['__INFO__']['logger'] = logger.record_mode
+        dump_yaml(logger, _clear_config(config), path=config['base']['runs_dir'] + "/configs/config.yaml")
+        self.logger = logger
+        return logger
+
+    def get_args(self, parser=None):
+        if self.args is None:
+            raise ValueError
+        return self.args
+    
+    def get_config(self):
+        return self.config
+    
 
-def trans_configure(config=BASE_CONFIG, file=None, **kwargs):
-    if file is not None:
-        parent, name = os.path.split(file)
-        name = name[:-3]
-        print(f"Change experiment name from {config['base']['experiment']} to {name}")
-        config['base']['experiment'] = name
-
-    # -------------  Initialize  -----------------
-    config = _check_config(config)
-    # if verbose:
-    #     print("------  Config  ------")
-    #     _print_dict(config['base'])
-    # Create Logger
+def get_logger(config):
     config_base = config['base']
     config_logger = config['logger']
-    # _print_dict(config)
     logger = MultiLogger(logdir=config_base['runs_dir'], 
-                         mode=config_logger.get('mode', None), 
-                         tag=config_base['tag'], 
-                         extag=config_base.get('experiment', None),
-                         action=config_logger.get('action', 'k')) # backup config.yaml
-    config['base']['__INFO__']['logger'] = logger.mode
-    config['base']['__INFO__']['Argv'] = "Argv: python " + ' '.join(sys.argv)
-
-    dump_yaml(logger, _clear_config(config), path=config['base']['runs_dir'] + "/config.yaml")
-    return logger, config
-
-
-def _check_config(config):    
-    config_base = config['base']
-    config['base']['tag'] = config['base']['tag'] if ('tag' in config['base'].keys()) and (config['base']['tag']!="") else str(datetime.now()).replace(' ', '-')
-    config['base']['extag'] = config['base']['extag'] if 'extag' in config['base'].keys() else None
-    config['base']['__INFO__'] = {}
-    config['base']['__INFO__']['runtime'] = str(datetime.now()).replace(' ', '-')
-
-    experiment = config['base']['experiment'] if 'experiment' in config['base'].keys() else ''
-    stage = config['base']['stage'] if 'stage' in config['base'].keys() else ''
-
-    config['base']['runs_dir'] = os.path.join(config['base']['base_dir'], experiment, config['base']['tag'], stage)
-    if not os.path.exists(config['base']['runs_dir']):
-        print(f"Make dir '{config['base']['runs_dir']}' !")
-        os.makedirs(config['base']['runs_dir'])
-    return config
-
+                        record_mode=config_logger.get('record_mode', None), 
+                        tag=config_base['tag'], 
+                        extag=config_base.get('experiment', None),
+                        action=config_logger.get('action', 'k')) # backup config.yaml
+    return logger
 
-def trans_args(parser=None):
+def trans_args(parser=None, **kwargs):
     if parser is None:
         parser = argparse.ArgumentParser(description='')
     try:
         parser.add_argument("--base_dir", type=str, default="")
     except:
-        print("Already add '--tag' ")
+        print("Already add '--base_dir' ")
+    try:
+        parser.add_argument("-c", "--config", type=str, default='./configs/config.yaml') 
+    except:
+        print("Already add '--config' ")
     try:
             parser.add_argument("-t", "--tag", type=str, default="")
     except:
         print("Already add '--tag' ")
     try:
         parser.add_argument("-et", "--extag", type=str, default="")
     except:
         print("Already add '--extag' ")
-    try:
-        parser.add_argument("-c", "--config", type=str, default='./configs/config.yaml') 
-    except:
-        print("Already add '--config' ")
     try: 
         parser.add_argument("-exp", "--experiment", type=str, default='', help="experiment name")
     except:
         print("Already add '--experiment' ")
     try:
         parser.add_argument("-st", "--stage", type=str, default="", help="stage name for multi-stage experiment ")
     except:
@@ -133,40 +191,38 @@
         parser.add_argument("--gpus", type=str, default='', help=" Turn on Multi stage mode ! ")
     except:
         print("Already add '--gpus' ")
     args = parser.parse_args()
     return args   
 
 
-def trans_init(args=None, file=None, ex_config=None, clear_none=True, **kwargs):
-    """
-    logger, config, tag, runs_dir = trans_init(args)
-    mode: "wandb", "tb" or "tensorboard", ["wandb", "tensorboard"]
-    
-    action: "d": delete the directory. Note that the deletion may fail when
-                the directory is used by tensorboard.
-                "k": keep the directory. This is useful when you resume from a
-                previous training and want the directory to look as if the
-                training was not interrupted.
-                Note that this option does not load old models or any other
-                old states for you. It simply does nothing.
-                "b" : copy the old dir
-                "n" : New an new dir by time
-    """
+def _check_config(config):    
+    config_base = config['base']
+    config['base']['tag'] = config['base']['tag'] if ('tag' in config['base'].keys()) and (config['base']['tag']!="") else str(datetime.now()).replace(' ', '-')
+    config['base']['extag'] = config['base']['extag'] if 'extag' in config['base'].keys() else None
+    config['base']['__INFO__'] = {}
+    config['base']['__INFO__']['runtime'] = str(datetime.now()).replace(' ', '-')
+
+    experiment = config['base']['experiment'] if 'experiment' in config['base'].keys() else ''
+    stage = config['base']['stage'] if 'stage' in config['base'].keys() else ''
+
+    config['base']['runs_dir'] = os.path.join(config['base']['base_dir'], experiment, config['base']['tag'], stage)
+    if not os.path.exists(config['base']['runs_dir']):
+        print(f"Make dir '{config['base']['runs_dir']}' !")
+        os.makedirs(config['base']['runs_dir'])
+    return config
+
+
+def merge_configs(args=None, file_config=None, ex_config=None, clear_none=True):
     assert isinstance(ex_config, (dict, type(None))), f"Got ex_config: {ex_config}"
-    assert isinstance(file, (str, type(None))), f"Got file: {file}"
 
     # Load yaml config file
     config=BASE_CONFIG
-    #  --------  args.config < args < ex_config  ----------
-    if args is not None: 
-        with open(args.config) as f:
-            file_config = yaml.load(f, Loader=yamlloader.ordereddict.CLoader)
-    else:
-        file_config = {}
+    #  --------  file_config < args < ex_config  ----------
+    file_config = file_config if file_config is not None else {}
     ex_config = ex_config if ex_config is not None else {}
     # Clear some vars with None or ""
     arg_dict_special = vars(copy.deepcopy(args)) if args is not None else {}
 
     if clear_none:
         file_config = _clear_config(file_config)
         arg_dict_special = _clear_config(arg_dict_special)
@@ -181,16 +237,15 @@
             config['base'][k] = arg_dict_special.pop(k)
     arg_dict = {'special': arg_dict_special}
     print("debug: arg-dict")
     _print_dict(arg_dict)
 
     # Merge ex-config to config
     config = merge_cascade_dict([config, arg_dict, ex_config])
-
-    return trans_configure(config, file=file, **kwargs)
+    return config
 
 
 def merge_cascade_dict(dicts):
     num_dict = len(dicts)
     ret_dict = {}
     for d in dicts:
         assert isinstance(d, dict), f"Got d1: {d}"
@@ -208,8 +263,80 @@
     ret_dict = {**d2, **d1}
     if isinstance(d2, dict):
         for key, value in d2.items():
             if isinstance(value, dict):
                 ret_dict[key] = _merge_two_dict(ret_dict[key], d2[key])
             else:
                 ret_dict[key] = d2[key]
-    return ret_dict 
+    return ret_dict 
+
+
+def dump_yaml(logger=None, config=None, path=None, verbose=True):
+    # Backup existing yaml file
+    assert config is not None
+    path = config['base']['runs_dir'] + "/config.yaml" if path is None else path
+    path = tfilename(path)
+    if os.path.isfile(path):
+        backup_name = path + '.' + _get_time_str()
+        shutil.move(path, backup_name)
+        if logger is not None:
+            logger.info(f"Existing yaml file '{path}' backuped to '{backup_name}' ")
+        else:
+            print(f"Existing yaml file '{path}' backuped to '{backup_name}' ")
+    with open(path, "w") as f:
+        config = _ordereddict_to_dict(config)
+        yaml.dump(config, f)
+    if verbose:
+        if logger is not None:
+            logger.info(f"Saved config.yaml to {path}")
+        else:
+            print(f"Saved config.yaml to {path}")
+
+
+def load_yaml(path):
+    with open(path) as f:
+        config = yaml.load(f, Loader=yamlloader.ordereddict.CLoader)
+    return config
+
+
+def _clear_config(config):
+    # if type(config) is dict or type(config) is OrderedDict:
+    if isinstance(config, (dict, OrderedDict)):
+        pop_key_list = []
+        for key, value in config.items():
+            # print("debug: ", key, value)
+            if value is None or value == "" or value == "None":
+                # print("debug: poped", key, value)
+                pop_key_list.append(key)
+            elif isinstance(config, (dict, OrderedDict)):
+                _clear_config(value)
+            else:
+                pass
+        for key in pop_key_list:
+            config.pop(key)
+    return config
+
+    
+def _print_dict(_dict, layer=0):
+    if isinstance(_dict, (dict, OrderedDict)):
+        for key, value in _dict.items():
+            if isinstance(value, (dict, OrderedDict)):
+                print("    "*layer, key, end=":\n")
+                _print_dict(value, layer+1)
+            else:
+                print("    "*layer, f"{key}: {value}")
+    else:
+        print("    "*layer, _dict)
+
+        
+def _ordereddict_to_dict(d):
+    if not isinstance(d, dict):
+        return d
+    for k, v in d.items():
+        if type(v) == OrderedDict:
+            v = _ordereddict_to_dict(v)
+            d[k] = dict(v)
+        elif type(v) == list:
+            d[k] = _ordereddict_to_dict(v)
+        elif type(v) == dict:
+            d[k] = _ordereddict_to_dict(v)
+    return d
```

## tutils/tutils/metriclogger.py

```diff
@@ -32,22 +32,24 @@
 
 import numpy as np
 import torch
 from torch import nn
 import torch.distributed as dist
 from PIL import ImageFilter, ImageOps
 
+from .functools import tprint
+
 
 def usage():
     from tutils import trans_args, trans_init, print_dict
     args = trans_args()
-    print(args)
+    tprint(args)
     logger, config = trans_init(args)
 
-    print(" ---------------------------------------------------------")
+    tprint(" ---------------------------------------------------------")
     print_dict(config)
 
     metriclogger = MetricLogger(logger=None)
 
     for data in metriclogger.log_every(range(20), print_freq=2, header="[trans]"):
         i = 0
         metriclogger.update(**{"ind": i, "data": data})
@@ -90,24 +92,24 @@
             return img
 
 
 def load_pretrained_weights(model, pretrained_weights, checkpoint_key, model_name, patch_size):
     if os.path.isfile(pretrained_weights):
         state_dict = torch.load(pretrained_weights, map_location="cpu")
         if checkpoint_key is not None and checkpoint_key in state_dict:
-            print(f"Take key {checkpoint_key} in provided checkpoint dict")
+            tprint(f"Take key {checkpoint_key} in provided checkpoint dict")
             state_dict = state_dict[checkpoint_key]
         # remove `module.` prefix
         state_dict = {k.replace("module.", ""): v for k, v in state_dict.items()}
         # remove `backbone.` prefix induced by multicrop wrapper
         state_dict = {k.replace("backbone.", ""): v for k, v in state_dict.items()}
         msg = model.load_state_dict(state_dict, strict=False)
-        print('Pretrained weights found at {} and loaded with msg: {}'.format(pretrained_weights, msg))
+        tprint('Pretrained weights found at {} and loaded with msg: {}'.format(pretrained_weights, msg))
     else:
-        print("Please use the `--pretrained_weights` argument to indicate the path of the checkpoint to evaluate.")
+        tprint("Please use the `--pretrained_weights` argument to indicate the path of the checkpoint to evaluate.")
         url = None
         if model_name == "vit_small" and patch_size == 16:
             url = "dino_deitsmall16_pretrain/dino_deitsmall16_pretrain.pth"
         elif model_name == "vit_small" and patch_size == 8:
             url = "dino_deitsmall8_pretrain/dino_deitsmall8_pretrain.pth"
         elif model_name == "vit_base" and patch_size == 16:
             url = "dino_vitbase16_pretrain/dino_vitbase16_pretrain.pth"
@@ -120,19 +122,19 @@
         elif model_name == "xcit_medium_24_p16":
             url = "dino_xcit_medium_24_p16_pretrain/dino_xcit_medium_24_p16_pretrain.pth"
         elif model_name == "xcit_medium_24_p8":
             url = "dino_xcit_medium_24_p8_pretrain/dino_xcit_medium_24_p8_pretrain.pth"
         elif model_name == "resnet50":
             url = "dino_resnet50_pretrain/dino_resnet50_pretrain.pth"
         if url is not None:
-            print("Since no pretrained weights have been provided, we load the reference pretrained DINO weights.")
+            tprint("Since no pretrained weights have been provided, we load the reference pretrained DINO weights.")
             state_dict = torch.hub.load_state_dict_from_url(url="https://dl.fbaipublicfiles.com/dino/" + url)
             model.load_state_dict(state_dict, strict=True)
         else:
-            print("There is no reference weights available for this model => We use random weights.")
+            tprint("There is no reference weights available for this model => We use random weights.")
 
 
 def clip_gradients(model, clip):
     norms = []
     for name, p in model.named_parameters():
         if p.grad is not None:
             param_norm = p.grad.data.norm(2)
@@ -153,35 +155,35 @@
 
 def restart_from_checkpoint(ckp_path, run_variables=None, **kwargs):
     """
     Re-start from checkpoint
     """
     if not os.path.isfile(ckp_path):
         return
-    print("Found checkpoint at {}".format(ckp_path))
+    tprint("Found checkpoint at {}".format(ckp_path))
 
     # open checkpoint file
     checkpoint = torch.load(ckp_path, map_location="cpu")
 
     # key is what to look for in the checkpoint file
     # value is the object to load
     # example: {'state_dict': model}
     for key, value in kwargs.items():
         if key in checkpoint and value is not None:
             try:
                 msg = value.load_state_dict(checkpoint[key], strict=False)
-                print("=> loaded '{}' from checkpoint '{}' with msg {}".format(key, ckp_path, msg))
+                tprint("=> loaded '{}' from checkpoint '{}' with msg {}".format(key, ckp_path, msg))
             except TypeError:
                 try:
                     msg = value.load_state_dict(checkpoint[key])
-                    print("=> loaded '{}' from checkpoint: '{}'".format(key, ckp_path))
+                    tprint("=> loaded '{}' from checkpoint: '{}'".format(key, ckp_path))
                 except ValueError:
-                    print("=> failed to load '{}' from checkpoint: '{}'".format(key, ckp_path))
+                    tprint("=> failed to load '{}' from checkpoint: '{}'".format(key, ckp_path))
         else:
-            print("=> key '{}' not found in checkpoint: '{}'".format(key, ckp_path))
+            tprint("=> key '{}' not found in checkpoint: '{}'".format(key, ckp_path))
 
     # re load variable important for the run
     if run_variables is not None:
         for var_name in run_variables:
             if var_name in checkpoint:
                 run_variables[var_name] = checkpoint[var_name]
 
@@ -415,15 +417,15 @@
         self.synchronize_between_processes()
         return {k: meter.global_avg for k, meter in self.meters.items()}
 
     def log(self, msg, *args, **kwargs):
         if self.no_print:
             return
         if self.logger is None:
-            print(msg, *args, **kwargs)
+            tprint(msg, *args, **kwargs)
         else:
             self.logger.info(msg, *args, **kwargs)
 
 
 
 def get_sha():
     cwd = os.path.dirname(os.path.abspath(__file__))
@@ -498,31 +500,31 @@
     # launched with submitit on a slurm cluster
     elif 'SLURM_PROCID' in os.environ:
         args.rank = int(os.environ['SLURM_PROCID'])
         args.gpu = args.rank % torch.cuda.device_count()
     # launched naively with `python main_dino.py`
     # we manually add MASTER_ADDR and MASTER_PORT to env variables
     elif torch.cuda.is_available():
-        print('Will run the code on one GPU.')
+        tprint('Will run the code on one GPU.')
         args.rank, args.gpu, args.world_size = 0, 0, 1
         os.environ['MASTER_ADDR'] = '127.0.0.1'
         os.environ['MASTER_PORT'] = '29500'
     else:
-        print('Does not support training without GPU.')
+        tprint('Does not support training without GPU.')
         sys.exit(1)
 
     dist.init_process_group(
         backend="nccl",
         init_method=args.dist_url,
         world_size=args.world_size,
         rank=args.rank,
     )
 
     torch.cuda.set_device(args.gpu)
-    print('| distributed init (rank {}): {}'.format(
+    tprint('| distributed init (rank {}): {}'.format(
         args.rank, args.dist_url), flush=True)
     dist.barrier()
     setup_for_distributed(args.rank == 0)
 
 
 def accuracy(output, target, topk=(1,)):
     """Computes the accuracy over the k top predictions for the specified values of k"""
@@ -699,15 +701,15 @@
         totenergy = d.sum()
 
         # sort eigenvectors with eigenvalues order
         idx = np.argsort(d)[::-1][:self.dim]
         d = d[idx]
         v = v[:, idx]
 
-        print("keeping %.2f %% of the energy" % (d.sum() / totenergy * 100.0))
+        tprint("keeping %.2f %% of the energy" % (d.sum() / totenergy * 100.0))
 
         # for the whitening
         d = np.diag(1. / d**self.whit)
 
         # principal components
         self.dvt = np.dot(d, v.T)
```

## tutils/tutils/prologger.py

```diff
@@ -1,10 +1,11 @@
 from .metriclogger import MetricLogger
 from .ttimer import timer
 from .recorder import Recorder
+from .functools import tprint
 
 
 # def usage2():
 #     from tutils import trans_args, trans_init, print_dict
 #     args = trans_args()
 #     logger, config = trans_init(args)
 #     print_dict(config)
@@ -25,15 +26,15 @@
     dataloader = range(20)
     prologger = ProLogger(metric=("mre", "dec"), epoch=10)
     # prologger = ProLogger(metric=("mre", "dec"), epoch=config['training']['epoch'], logger=logger)
     for epoch, trainlogger, dtrain, monitor in prologger:
         for data in trainlogger(dataloader):
             i = 0
             trainlogger.update(**{"ind": i, "data": data, "mre": data})
-            # print("Metriclogger logging!")
+            # tprint("Metriclogger logging!")
             d = {"ind": i, "data": data, "mre": data}
             best = monitor.record(d, epoch=epoch)
 
         # for data in testlogger(dataloader):
 
 
 class ProLogger:
@@ -67,27 +68,27 @@
         if self.metric is not None:
             assert isinstance(self.metric, tuple), f"Got {self.metric}"
             monitor = Monitor(key=self.metric[0], mode=self.metric[1])
             self.monitor = monitor
 
     def log(self, msg, *args, **kwargs):
         if self.logger is None:
-            print(msg, *args, **kwargs)
+            tprint(msg, *args, **kwargs)
         else:
             self.logger.info(msg, *args, **kwargs)
 
     def __iter__(self):
         # timer1 = timer()
         d_train = {}
         for i in range(self.num_epoch):
             t = self.timer()
             yield i, self.trainlogger, d_train, self.monitor
 
             time_run = self.timer() - t
-            # print("metriclogger.return_final_dict")
+            # tprint("metriclogger.return_final_dict")
             d_train = self.trainlogger.return_final_dict()
             d_train['running_time'] = time_run
             d_train['epoch'] = i
             d_train_str = "[Prologger] "
             for k, v in d_train.items():
                 if isinstance(v, float):
                     v = f"{v:.6f}"
@@ -111,15 +112,15 @@
             return v > self.best_value
         else:
             return v < self.best_value
 
     def record(self, d, epoch):
         isbest = self._record(d[self.key], epoch)
         if isbest:
-            print("[Monitor] `Achive New Record` ")
+            tprint("[Monitor] `Achive New Record` ")
             self.best_dict = d
         return {"isbest":isbest, "best_value":self.best_value, "best_epoch":self.best_epoch, **self.best_dict}
 
     def _record(self, v, epoch):
         if self.best_epoch is None or self.best_value is None:
             self.best_value = v
             self.best_epoch = epoch
```

## tutils/tutils/recorder.py

```diff
@@ -58,27 +58,29 @@
             l_list = []
             for lossi, value in loss.items():
                 if type(lossi) == torch.Tensor:
                     l_list.append(lossi.detach().cpu().item())
             self.loss_list.append(l_list)
 
     def cal_metrics(self):
+        len_record = len(self.loss_list)
         temp = np.array(self.loss_list)
         if self.reduction == "mean":
             res = temp.mean(axis=0)
         elif self.reduction == "sum":
             res = temp.sum(axis=0)
         else:
             raise ValueError
         # print("debug mean", mean, temp, self.loss_keys)
 
         if self.loss_keys is None:
             return None
         else:
             _dict = {k: res[i] for i, k in enumerate(self.loss_keys)}
+            _dict['num'] = len_record
             return _dict
 
 class EpochRecorder(object):
     def __init__(self, logger, config, mode="dec"):
         # mode in ["dec", "inc"]
         self.logger = logger
         self.config = config
```

## tutils/tutils/tlogger.py

```diff
@@ -17,108 +17,199 @@
 import sys
 from logging import INFO, DEBUG, WARNING, CRITICAL, ERROR
 from termcolor import colored
 # from pathlib import Path
 # import argparse
 import sys
 from collections import OrderedDict
-from .functools import _get_time_str
+from .functools import _get_time_str, tprint
+# from .tutils import tdir
+import torch
+from tensorboardX import SummaryWriter
+from .tutils import tfilename
 
 INFO = INFO
 DEBUG = DEBUG
 WARNING = WARNING
 CRITICAL = CRITICAL
 ERROR = ERROR
 
 
+class TBLogger:
+    def __init__(self, logdir, *args, **kwargs):
+        tprint(f"Use Tensorboard, log at '{os.path.join(logdir, 'tb')}'")
+        self.tb_logger = SummaryWriter(logdir=os.path.join(logdir, "tb"))
+        self.step = 0
+
+    def record(self, d, step=-1, tag='std'):
+        # debug:
+        if step < 0:
+            step = self.step
+            self.step += 1
+        to_record = {}
+        for k, v in d.items():
+            if isinstance(v, (float, int, )) or torch.is_tensor(k):
+                to_record[k] = v
+        # print("[Tuils] [TBLogger]: ", d)
+        self.tb_logger.add_scalars(tag, to_record, global_step=step)
+
+
 class MultiLogger(Logger):
-    def __init__(self, logdir, mode=None, tag="MyLogger",extag=None, level=logging.INFO, action='k', file_name='log.log'):
+    def __init__(self, 
+                 logdir, 
+                 record_mode=None, 
+                 logging_mode=None,
+                 tag="MyLogger",
+                 extag=None, 
+                 level=logging.INFO, 
+                 action='k', 
+                 file_name='log.log'):
         """
-        mode: "wandb", "tb" or "tensorboard", "csv" : ["wandb", "tensorboard", "csv"]
+        record_mode: "wandb", "tb" or "tensorboard", "csv" : ["wandb", "tensorboard", "csv"]
         """
         super(MultiLogger, self).__init__(tag)
         self.logdir = logdir
-        self.mode = "logging_only" if mode is None else mode
-        self.multi_recorder = MultiRecorder(mode, logdir, tag)
+        self.record_mode = "logging_only" if record_mode is None else record_mode
+        self.logging_mode = logging_mode
+        self.multi_recorder = MultiRecorder(record_mode, logdir, tag)
         
         # --------- Standard init        
         self.propagate = False
         self.setLevel(level)
-        handler = logging.StreamHandler()
-        # handler = logging.FileHandler('test.log', 'w', 'utf-8') # or whatever
-        handler.setFormatter(_MyFormatter(tag=tag, extag=extag, datefmt='%Y-%m-%d %H:%M:%S'))
-        self.addHandler(handler)
-        set_logger_dir(self, logdir, action, file_name, tag=tag, extag=extag)
+
+        if self.logging_mode != "file_only":
+            # Set StreamHandler, for console
+            handler = logging.StreamHandler()
+            # handler = logging.FileHandler('test.log', 'w', 'utf-8') # or whatever
+            handler.setFormatter(_MyFormatter(tag=tag, extag=extag, datefmt='%Y-%m-%d %H:%M:%S'))
+            self.addHandler(handler)
+
+        # if self.logging_mode == "file_only":
+        # Set FileHandler
+        dirname = self.set_logger_dir(tfilename(logdir, "log"), action, file_name, tag=tag, extag=extag)
+        self._set_FileHandler(os.path.join(dirname, file_name), tag=tag, extag=extag)
     
     def add_scalars(self, *args, **kwargs):
         self.multi_recorder.add_scalars(*args, **kwargs)
 
     def __call__(self, *args, **kwargs):
         return self.info(*args, **kwargs)
 
+    def _set_FileHandler(logger, path, tag=None, extag=None):
+        if os.path.isfile(path):
+            backup_name = path + '.' + _get_time_str()
+            shutil.move(path, backup_name)
+            logger.info("Existing log file '{}' backuped to '{}'".format(path, backup_name))  # noqa: F821
+        hdl = logging.FileHandler(
+            filename=path, encoding='utf-8', mode='w')
+        hdl.setFormatter(_MyFormatter(tag=tag, extag=extag, datefmt='%Y-%m-%d-%H:%M:%S', colorful=False))
+
+        _FILE_HANDLER = hdl
+        logger.addHandler(hdl)
+        logger.info("Argv: python " + ' '.join(sys.argv))
+
+    def set_logger_dir(self, dirname='log', action='k', file_name='log.log', tag=None, extag=None):
+        """
+        Set the directory for global logging.
+        Args:
+            dirname(str): log directory
+            action(str): an action of ["k","d","q"] to be performed
+                when the directory exists. Will ask user by default.
+                    "d": delete the directory. Note that the deletion may fail when
+                    the directory is used by tensorboard.
+                    "k": keep the directory. This is useful when you resume from a
+                    previous training and want the directory to look as if the
+                    training was not interrupted.
+                    Note that this option does not load old models or any other
+                    old states for you. It simply does nothing.
+                    "b" : copy the old dir
+                    "n" : New an new dir by time
+        """
+        def dir_nonempty(dirname):
+            # If directory exists and nonempty (ignore hidden files), prompt for action
+            return os.path.isdir(dirname) and len([x for x in os.listdir(dirname) if x[0] != '.'])
+
+        if dir_nonempty(dirname):
+            dirname = os.path.join(dirname, "logs")
+            if action == 'b':
+                backup_name = dirname + _get_time_str()
+                shutil.move(dirname, backup_name)
+                self.info("Directory '{}' backuped to '{}'".format(dirname, backup_name))  # noqa: F821
+            elif action == 'd':
+                shutil.rmtree(dirname, ignore_errors=True)
+                if dir_nonempty(dirname):
+                    shutil.rmtree(dirname, ignore_errors=False)
+            elif action == 'n':
+                dirname = dirname + _get_time_str()
+                self.info("Use a new log directory {}".format(dirname))  # noqa: F821
+            elif action == 'k':
+                pass
+            else:
+                raise OSError("Directory {} exits!".format(dirname))
+        _mkdir_p(dirname)
+        return dirname
+
 
 class MultiRecorder(object):
     """
         Extra Log Writer , including TensorBoard, wandb
     """
-    def __init__(self, mode, logdir, tag="Log") -> None:
+    def __init__(self, record_mode, logdir, tag="Log") -> None:
         super().__init__()
 
         self.step = -1
         self.wandb_logger = None
         self.tb_logger = None
         self.csv_logger = None
         self.text_logger = None
 
-        if mode == None: mode = []
-        if type(mode) is str: mode = [mode]
-        if "wandb" in mode:
+        if record_mode == None: record_mode = []
+        if type(record_mode) is str: record_mode = [record_mode]
+        if "wandb" in record_mode:
             import wandb
             wandb.init(project=tag)
             wandb.watch_called = False
             self.wandb_logger = wandb
-        if "tb" in mode or "tensorboard" in mode:
+        if "tb" in record_mode or "tensorboard" in record_mode:
             from tensorboardX import SummaryWriter
             if logdir is None:
-                print(f"Failed to turn on Tensorboard due to logdir=None")
+                tprint(f"Failed to turn on Tensorboard due to logdir=None")
             else:
-                print(f"Use Tensorboard, log at '{os.path.join(logdir, 'tb')}'")
-                self.tb_logger = SummaryWriter(logdir=os.path.join(logdir, "tb"))
-        # if "csv" in mode:
+                # tprint(f"Use Tensorboard, log at '{os.path.join(logdir, 'tb')}'")
+                # self.tb_logger = SummaryWriter(logdir=os.path.join(logdir, "tb"))
+                self.tb_logger = TBLogger(logdir=logdir)
+        # if "csv" in record_mode:
         #     self.csv_logger = CSVLogger(logdir=os.path.join(logdir, "csv"))
-        self.extra_logger = True if len(mode) > 0 else False
+        self.extra_logger = True if len(record_mode) > 0 else False
         
     def add_scalars(self, dicts:dict={}, step=-1, tag="train", verbose=True):
         if not self.extra_logger:
             return 
         if self.wandb_logger is not None:
             self.wandb_logger.log(dicts)
 
         if self.tb_logger is not None:
-            if step < 0:
-                step = self.step
-            self.tb_logger.add_scalars(tag, dicts, global_step=step)
+            self.tb_logger.record(d=dicts, step=step, tag=tag)
             
         self.step = self.step + 1
-
         if self.text_logger is not None:
             if verbose:
                 string = f"[tlog] Step:{self.step}  "
                 for key, value in dicts.items():
                     string += f"{key}:{value};"
                 self.info(string)
 
 
 class _MyFormatter(logging.Formatter):
     def __init__(self, tag=None, extag=None, colorful=True, *args, **kwargs):
         self.tag = tag
         self.extag = extag
         self.colorful = colorful
         extag = '-' + extag if (extag is not None and extag != '') else ''
-        # print(tag, extag)
+        # tprint(tag, extag)
         self.taginfo = self._colored_str(f'[{tag}{extag}]', 'cyan') if tag is not None else ''
         super(_MyFormatter, self).__init__(*args, **kwargs)
         
     def format(self, record):    
         if not self.colorful:
             # Logging file
             date = self._colored_str('[%(asctime)s @%(filename)s:%(lineno)d] ', 'green')
@@ -146,69 +237,14 @@
     def _colored_str(self, text, *args, **kwargs):
         if self.colorful:
             return colored(text, *args, **kwargs)
         else:
             return text
 
 
-def _set_file(logger, path, tag=None, extag=None):
-    if os.path.isfile(path):
-        backup_name = path + '.' + _get_time_str()
-        shutil.move(path, backup_name)
-        logger.info("Existing log file '{}' backuped to '{}'".format(path, backup_name))  # noqa: F821
-    hdl = logging.FileHandler(
-        filename=path, encoding='utf-8', mode='w')
-    hdl.setFormatter(_MyFormatter(tag=tag, extag=extag, datefmt='%Y-%m-%d-%H:%M:%S', colorful=False))
-
-    _FILE_HANDLER = hdl
-    logger.addHandler(hdl)
-    logger.info("Argv: python " + ' '.join(sys.argv))
-
-
-def set_logger_dir(logger, dirname='log', action='k', file_name='log.log', tag=None, extag=None):
-    """
-    Set the directory for global logging.
-    Args:
-        dirname(str): log directory
-        action(str): an action of ["k","d","q"] to be performed
-            when the directory exists. Will ask user by default.
-                "d": delete the directory. Note that the deletion may fail when
-                the directory is used by tensorboard.
-                "k": keep the directory. This is useful when you resume from a
-                previous training and want the directory to look as if the
-                training was not interrupted.
-                Note that this option does not load old models or any other
-                old states for you. It simply does nothing.
-                "b" : copy the old dir
-                "n" : New an new dir by time
-    """
-    def dir_nonempty(dirname):
-        # If directory exists and nonempty (ignore hidden files), prompt for action
-        return os.path.isdir(dirname) and len([x for x in os.listdir(dirname) if x[0] != '.'])
-
-    if dir_nonempty(dirname):
-        if action == 'b':
-            backup_name = dirname + _get_time_str()
-            shutil.move(dirname, backup_name)
-            logger.info("Directory '{}' backuped to '{}'".format(dirname, backup_name))  # noqa: F821
-        elif action == 'd':
-            shutil.rmtree(dirname, ignore_errors=True)
-            if dir_nonempty(dirname):
-                shutil.rmtree(dirname, ignore_errors=False)
-        elif action == 'n':
-            dirname = dirname + _get_time_str()
-            logger.info("Use a new log directory {}".format(dirname))  # noqa: F821
-        elif action == 'k':
-            pass
-        else:
-            raise OSError("Directory {} exits!".format(dirname))
-    _mkdir_p(dirname)
-    _set_file(logger, os.path.join(dirname, file_name), tag=tag, extag=extag)
-
-
 def _mkdir_p(dirname):
     """ Like "mkdir -p", make a dir recursively, but do nothing if the dir exists
     Args:
         dirname(str):
     """
     assert dirname is not None
     if dirname == '' or os.path.isdir(dirname):
```

## tutils/tutils/ttimer.py

```diff
@@ -1,15 +1,16 @@
 import time
 import numpy as np
 import datetime
+from .functools import tprint
 
 
 def trans_time():
     """
-        print time str of now
+        tprint time str of now
     """
     return datetime.datetime.now().strftime('%m%d-%H%M%S')
 
 
 class tenum:
     def __init__(self, iter):
         self.stop_time = time.time()
@@ -51,15 +52,15 @@
     
     def one_stop(self, verbose=False):
         self.stop_time = time.time()
         interval = self.stop_time - self.start_time
         self.start_time = self.stop_time
         self.time_list.append(interval)
         if verbose:
-            print(f"interval: {interval}")
+            tprint(f"interval: {interval}")
         return interval
     
     def stop(self):
         interval = time.time() - self.start_time
         self.start_time = time.time()
         return interval
         
@@ -87,34 +88,34 @@
             return format_result(self.sum())
         
 def tfunctime(func):
     def run(*argv, **kargs):
         t1 = time.time()
         ret = func(*argv, **kargs)
         t2 = time.time()
-        # print(f"[Function {func.__name__}] Running time:{(t2-t1):.6f}s")
+        # tprint(f"[Function {func.__name__}] Running time:{(t2-t1):.6f}s")
         return (t2-t1), ret
     return run
 
 
 def tshowtime(func):
     def run(*argv, **kargs):
         t1 = time.time()
         ret = func(*argv, **kargs)
         t2 = time.time()
-        print(f"[Function {func.__name__}] Running time:{(t2-t1):.6f}s")
+        tprint(f"[Function {func.__name__}] Running time:{(t2-t1):.6f}s")
         return ret
     return run
 
-# print(isinstance(g, Iterable)) # true
-# print(isinstance(g, Iterator)) # true
-# print(isinstance(g, Generator)) # false
+# tprint(isinstance(g, Iterable)) # true
+# tprint(isinstance(g, Iterator)) # true
+# tprint(isinstance(g, Generator)) # false
 if __name__ == "__main__":
     t1 = timer("load_time")
     t2 = timer("test_time")
     t1()
     t2()
     time.sleep(500)
     t1.stop()
     t2.stop()
-    print(t1.showavg())
-    print(t2.showsum())
+    tprint(t1.showavg())
+    tprint(t2.showsum())
```

## tutils/tutils/tutils.py

```diff
@@ -1,13 +1,13 @@
 
 import yaml
 import yamlloader
 import shutil
 import os
-from .functools import d, _get_time_str, _ordereddict_to_dict
+from .functools import d, _get_time_str, _ordereddict_to_dict, tprint
 from pathlib import Path
 from datetime import datetime
 from torchvision.utils import save_image as tv_save_image
 
 
 def save_image(tensor, fname:str="tmp/tmp.png"):
     tv_save_image(tensor, fname)
@@ -17,39 +17,47 @@
     return datetime.now().strftime('%m%d-%H%M%S')
 
 
 def save_script(runs_dir, _file_name, logger=None):
     file_path = os.path.abspath(_file_name)
     parent, name = os.path.split(_file_name)
     time = _get_time_str()
-    output_path = os.path.join(runs_dir, name)
+    output_path = tfilename(runs_dir, "scripts", name)
 
     if os.path.isfile(output_path):
         backup_name = output_path + '.' + _get_time_str()
         shutil.move(output_path, backup_name)
-        print(f"Existing yaml file '{output_path}' backuped to '{backup_name}' ")
+        tprint(f"Existing yaml file '{output_path}' backuped to '{backup_name}' ")
 
     shutil.copy(file_path, output_path)
     # with open(os.path.join(runs_dir, "save_script.log"), "a+") as f:
     #     f.write(f"Script location: {_file_name};  Time: {time}\n")
-    print(f"Saved script file: from {file_path} to {output_path}")
+    tprint(f"Saved script file: from {file_path} to {output_path}")
 
 
-def dump_yaml(logger, config, path=None, verbose=True):
+def dump_yaml(logger=None, config=None, path=None, verbose=True):
     # Backup existing yaml file
+    assert config is not None
     path = config['base']['runs_dir'] + "/config.yaml" if path is None else path
+    path = tfilename(path)
     if os.path.isfile(path):
         backup_name = path + '.' + _get_time_str()
         shutil.move(path, backup_name)
-        logger.info(f"Existing yaml file '{path}' backuped to '{backup_name}' ")
+        if logger is not None:
+            logger.info(f"Existing yaml file '{path}' backuped to '{backup_name}' ")
+        else:
+            tprint(f"Existing yaml file '{path}' backuped to '{backup_name}' ")
     with open(path, "w") as f:
         config = _ordereddict_to_dict(config)
         yaml.dump(config, f)
     if verbose:
-        logger.info(f"Saved config.yaml to {path}")
+        if logger is not None:
+            logger.info(f"Saved config.yaml to {path}")
+        else:
+            tprint(f"Saved config.yaml to {path}")
 
 
 def load_yaml(path):
     with open(path) as f:
         config = yaml.load(f, Loader=yamlloader.ordereddict.CLoader)
     return config
```

## tutils/tutils/visualizers/print_image.py

```diff
@@ -1,55 +1,59 @@
 import numpy as np
-import cv2
 import torch
 from PIL import Image
 from tutils.tutils import d
 import torchvision
+from datetime import datetime
 
 
-def save_image(img, fname="tmp/tmp.png"):
+def save_image(img, fname=None):
     """
         img type: Numpy, Tensor, PIL image
 
         Convert Img to tensor, and use torchvision.utils.save_image()
     """
+    if fname is None:
+        fname = f"./img_{datetime.now().strftime('%m%d-%H%M%S')}.png"
     if isinstance(img, torch.Tensor):
         torchvision_save(img, fname)
     elif isinstance(img, np.ndarray):
         if len(img.shape) == 3:
             img = img[np.newaxis, :, :, :]
         elif len(img.shape) == 2:
             img = img[np.newaxis, np.newaxis, :, :]
         assert len(img.shape) == 4, f"Write image shape ERROR, Got img.shape={img.shape}, fname={fname}"
         img = img.transpose((0,2,3,1))
         torchvision_save(torch.Tensor(img), fname)
     elif isinstance(img, Image.Image):
         pil_save(img, fname)
 
 
-
-def torchvision_save(tensor:torch.Tensor, fname) -> None:
+def torchvision_save(tensor:torch.Tensor, fname=None) -> None:
     """
     Recommended: 
     tensor: [b, 3, m,n], multiple images be saved in one file.
     Tips: this function times 255 to tensor
     """
-    if torch.max(tensor) > 1.0:
-        print(f"[DEBUG] tensor.max() from {tensor.max()} to {1.0}, fname={fname}")
-        tensor = tensor / tensor.max()
+    if fname is None:
+        fname = f"./img_{datetime.now().strftime('%m%d-%H%M%S')}.png"
     if tensor.min() < 0.0:
         print(f"[DEBUG] tensor.min() from {tensor.min()} to {0.0}, fname={fname}", )
-        tensor = tensor.clamp(0, 1.0)
+        tensor = tensor.clamp(0, 999)
+    if tensor.max() > 1.0:
+        print(f"[DEBUG] tensor.max() from {tensor.max()} to {1.0}, fname={fname}")
+        tensor = tensor / tensor.max()
 
     # assert torch.max(tensor) <= 1.0 and torch.min(tensor) >= 0.0, f"Error, got Max:{torch.max(tensor)}, and Min:{torch.min(tensor)}"
     torchvision.utils.save_image(tensor, fname)
     
 def pil_save(img:Image.Image, fname) -> None:
     if type(img) == np.ndarray:
         img = Image.fromarray(img)
     img.save(fname)
 
 
 def cv_save(img:np.ndarray, fname:str) -> None:
+    import cv2
     img = img.astype(np.uint8)
     cv2.imwrite(fname, img)
```

## Comparing `trans_utils-0.2.2.dist-info/RECORD` & `trans_utils-0.3.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,68 @@
-tutils/__init__.py,sha256=LOYp1idwBbsEvL3awa3WGoA9pUjIPwS8MZg31QEzWrM,50
+tutils/__init__.py,sha256=AlZteqWv75oWwrd_sYia4n4DGY96noQoNo0FybRTlV0,68
+tutils/classify.py,sha256=JU78t2AtIRYCDC0yFgBEZszWxeyzhslh92xjRgL6-ng,2281
 tutils/functools.py,sha256=pXwVrxL_eTDH2U0zZKalDMHS_FZscTcN4gg3V1WJiFA,3316
 tutils/initializer.py,sha256=Ds6EZ3_qg5qDLdZZdpmuIKB_PHdhjHxai5SXclTbFT4,5771
 tutils/tutils.py,sha256=V-5TcafNQV_OYNf3MX2EWQP1dzLkEmAhTb_gZuvHptE,3286
+tutils/contrib/__init__.py,sha256=089x8FDIyGAqmrabc_1Vvb-TKqelHVqh20ViPSSHGZI,69
+tutils/contrib/ddp_demo.py,sha256=9eYkR8KPSCCciJhaY8nfIxdf5N0JsJeu5XAalmLEjXc,4641
+tutils/contrib/debug_tools.py,sha256=AdW7K4BNiZcXqqbMbyqBiYk-JOX77QSHnpH0WjgZugY,857
+tutils/contrib/fourier.py,sha256=MiMflKy3DEgTTum94b1s_qZ5nT6Gh808LEFJ2bGicvs,49
+tutils/contrib/other_package.py,sha256=OKNrfVmECtSzAzxwbgMSX1Y_If0Z6ukMZsw5YGs7FE8,9
+tutils/contrib/pudb_debug.py,sha256=H3v4OOZ1GILYylPPspYGz4F3TdkXmPDb2rpC4uDadw0,111
+tutils/contrib/shutils.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/contrib/tmp.py,sha256=-c6UGv-bQandUw8BZVsQEEMGkBwSZi99UMF9j7FxF4M,223
+tutils/contrib/proj-template/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/contrib/proj-template/code/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/contrib/proj-template/code/configs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/contrib/proj-template/code/datasets/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/contrib/proj-template/code/networks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/contrib/proj-template/code/scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/contrib/proj-template/code/scripts/template.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/contrib/proj-template/code/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/contrib/proj-template/code/test/datasets/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/contrib/proj-template/code/test/networks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/contrib/proj-template/code/test/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/contrib/proj-template/code/tmp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/contrib/proj-template/code/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/contrib/proj-template/data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/contrib/proj-template/related_work_1/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/contrib/proj-template/related_work_1/work1/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/contrib/proj-template/runs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/contrib/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/contrib/test/test_builtins.py,sha256=D00nS3lsqL6R_AveMbHK6LoUNNfhv_c8ZFIXGZmQIwk,227
+tutils/contrib/test/test_initializer.py,sha256=z9C7RIFqSyEg0UNQUVWs2_rXOho4bzBhG2Y1mYNHgKY,326
+tutils/contrib/test/test_print.py,sha256=5LBGLd3Nxrv1ef1NUB4c1dlPtlYhu2ApzJEcjvVjUpU,50
+tutils/contrib/test/test_pytest.py,sha256=kWW7lC7stSr6fc-YgQO-EPtNazyCZbQ9CygP0jla_kc,1041
 tutils/mn/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tutils/mn/data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/mn/data/__init__.py,sha256=BY4iEENH-IJ_4JkWzI7ySbnYboFepbW0fipdYPFe3xs,20
 tutils/mn/data/base_dataset.py,sha256=oU9G0M3VcvSMwdccb6s0Rmmn_Livl1Iw991ZeSRRCas,392
 tutils/mn/data/base_options.py,sha256=rTUEUV1DtnRmZ68Sh2AO4nryHlEzaOlAfyEAJiXUGb4,3310
 tutils/mn/data/data_preprocess.py,sha256=-losc0l9b3e6EMSJQXs5OukgqUH7QSl4cIkypmejGhM,3582
 tutils/mn/data/augment/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tutils/mn/data/augment/augment.py,sha256=Hq7qDFTC6ZLe12QgV0RsdCO7nzb-qUIgcXhzRtGhuqY,5720
 tutils/mn/data/augment/autoaugment.py,sha256=ugEga_x2u8k0WW8MAcLqSa2hnxq-JhQfXh_JI4I3ebs,11514
-tutils/mn/data/augment/common_2d_aug.py,sha256=ilKYM0ksSobkeOQfB2IoXinP5IyAZ4Hho3tGNgnUXLo,5728
+tutils/mn/data/augment/common_2d_aug.py,sha256=aGgKF8pwlQ-ccGMIWD18gTeomqsd_f0ZB9qkdzk6iss,6725
 tutils/mn/data/augment/demo_monai_augment.py,sha256=hiwiy1n1K-t-ECH9vQIYWkjFikeSeLhhBdCrfjRkfmA,469
 tutils/mn/data/augment/edge_detection.py,sha256=7nZLHnw5kTHh0ER8V9oLV4ryauofryH3D-FVBmnQsuc,698
 tutils/mn/data/augment/gaussian.py,sha256=QRSQJ5NTP8QtyGZi2k547eCxUV1vx5jMB-kPg2GMkcA,4755
 tutils/mn/data/augment/patching.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tutils/mn/data/tsitk/__init__.py,sha256=b6oNqJHWoKPYsZfEr4qDFjZAzWfCJu83PvFd6_3U7lY,17
-tutils/mn/data/tsitk/io.py,sha256=b0bMEHGrVbm9jpyfBoqIxSq-nAW2vCMfcaEfDKcB-C8,1662
+tutils/mn/data/tsitk/__init__.py,sha256=G25prpwnb-Uf1aM4SOfF-wqB09C_3CNSM7evPn4TLLY,45
+tutils/mn/data/tsitk/io.py,sha256=J6hYV3u-e_beUAKI-mhcYH11NSALsaHyw67kLZz6_2w,1640
 tutils/mn/data/tsitk/preprocess.py,sha256=UfgwFxQiFyaCXSirdDRHM3BvHwLpYeFzf_t2BoXkNk0,2335
 tutils/mn/eval/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tutils/mn/eval/radio_analysis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tutils/mn/eval/radio_analysis/demo.py,sha256=vjVuDr-nqE-0-1AnYscRPwtzvD_fnAvI9AVbk6egCkY,1794
 tutils/mn/eval/radio_analysis/demo_function.py,sha256=kPWJG_EnosF-TD2OhbIqVMKwiml6kTD8OeVp9b99w2k,5394
-tutils/mn/eval/radio_analysis/example_helloFeatureClass.py,sha256=1-hU6UOhwMfowD-XA5zN0zPMpAMptqWPmRB2oy7HN0E,6281
+tutils/mn/eval/radio_analysis/example_helloFeatureClass.py,sha256=04PE60PRof2V08telJzzbzmf5-bwJH-wjmxhIy6ccEw,6311
 tutils/mn/eval/radio_analysis/medical_qa.py,sha256=szvnE_6FUoC82fDTL6TQKkEx7s9zsFQDBpqn8mS6PUs,55
 tutils/mn/train/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tutils/mn/train/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tutils/mn/train/models/cam_model.py,sha256=7ufPH2eKqfU9maQTcgt3wHaBWMbXcg8ujc_8ImokW58,5844
+tutils/mn/train/models/cam_model.py,sha256=BXGPjBhC8OS8IQQ5kqeJuyovl-y6PP3oYajmQFURMyI,5920
+tutils/mn/train/models/debug_model.py,sha256=u8uwnSKGi8m7Re7goFrL7Cu1FloauYO-9LTHwzeSQIY,593
 tutils/mn/train/models/unet_model.py,sha256=f5qUplWQnynmuA9odIEohqCJK4Ieq66pzocmhesDu4s,1277
 tutils/mn/train/models/unet_parts.py,sha256=qDrn68LJ3_N-tE6CPfBAkuDKX1iK4EfdmYL3gLsjjGc,2735
 tutils/mn/train/tloss/__init__.py,sha256=ec8Ev0k1DThWFjNE8A6ZlJ4eJEG6KQP5h2gAsy6v5F8,236
 tutils/mn/train/tloss/edge_loss.py,sha256=vAHtlD4qN5Ia33DF0Cv3pls2Smtx0CswyzvOAwiWnWE,2326
 tutils/mn/train/tloss/entropy_loss.py,sha256=Rgz9OUeDMyxXdwOUlQc_pn2uBXyOY31YGo7WAfd-2Co,3021
 tutils/mn/train/tloss/infonce_loss.py,sha256=Pz2BHfuy_Zn-HUNuposcUB87sD2QotO8F_ENS2Eryb8,6706
 tutils/mn/train/tloss/ncc_loss.py,sha256=FeQl3iFDnYgGLvsLczrxczLk9m98G-c82NRdGOydZ18,1870
@@ -52,54 +84,75 @@
 tutils/proj-template/code/test/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tutils/proj-template/code/tmp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tutils/proj-template/code/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tutils/proj-template/data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tutils/proj-template/related_work_1/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tutils/proj-template/related_work_1/work1/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tutils/proj-template/runs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/test/test_builtins.py,sha256=D00nS3lsqL6R_AveMbHK6LoUNNfhv_c8ZFIXGZmQIwk,227
+tutils/test/test_initializer.py,sha256=z9C7RIFqSyEg0UNQUVWs2_rXOho4bzBhG2Y1mYNHgKY,326
+tutils/test/test_print.py,sha256=5LBGLd3Nxrv1ef1NUB4c1dlPtlYhu2ApzJEcjvVjUpU,50
+tutils/test/test_pytest.py,sha256=kWW7lC7stSr6fc-YgQO-EPtNazyCZbQ9CygP0jla_kc,1041
+tutils/tpackage/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tutils/tpackage/_multilogger.py,sha256=DgTRUo-EfuNTH-Lk2oREV9F5rjS8dHr8TKaJVMHjJuo,9939
+tutils/tpackage/learner.py,sha256=xLJdvCz2GgsZHmUfos85a4R6dVr1OoMK0KHPyc81WBI,3553
+tutils/tpackage/logger.py,sha256=V8qqrBkUFFEH5CmUxZvaf3AaWL6m9TC43IOrDV-ixm4,8405
+tutils/tpackage/logger_utils.py,sha256=uBX8CqwE2m9LEY1EDzQwVNuB2Gbwao1FJhmddvfr1Dg,3840
+tutils/tpackage/monitor.py,sha256=eVL3J54IMfWX-PjQzVRKhaHuehIfu1h9RCCn-uVtb_U,1075
+tutils/tpackage/tester.py,sha256=nu1OoAN2Oz8w3aTN5PDsEaA_ATnCWkLd0MYfVqSN5yw,1500
+tutils/tpackage/trainer.py,sha256=UIgrLO2j2MrrBB5r9j-uCNrCAbakb-SePJo-lzMeAls,13552
+tutils/tpackage/trainer_utils.py,sha256=GPmYNfCzV0DJGNNnwhMv_HK5wqyLHoc0KlAO5cbmdfo,1166
 tutils/trainer/__init__.py,sha256=tnjXJWaHugTb3oDKcyOIGm8O4B1Qbz7SC_qzU8N7bj8,249
 tutils/trainer/_bad_tuner_exec.py,sha256=WlBiMaCyBt1-39TwolVM-qilGvpcmo9WTSlSydWKjnU,2595
 tutils/trainer/ablation_exec.py,sha256=R4MoGV2XJAJosAlyPEGSDGmzdO2ixISjYuK8QHE8Vas,9630
 tutils/trainer/ablation_search.py,sha256=WmtYZn87QvbgIDVE9Opwq7fYiaHqhh478qP7C7naAEw,34
 tutils/trainer/ablation_trainer.py,sha256=uod3cdCU22woL3Ul3nMOInNv3tpXfVQ9J5MHsJNosKs,5017
 tutils/trainer/demo_ablation_trainer.py,sha256=_mRnrrCUs8PD3yt8ywAEsgDbiQD0dApQyaXhr1vSwnA,5049
 tutils/trainer/demo_learner_trainer.py,sha256=T1gpAyC64lRxrNIdioO2CkJmFc66ahsIayAMNs0xbOM,4610
 tutils/trainer/demo_train.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tutils/trainer/demo_train_script.py,sha256=zEmKlLQ62C6-gZpapn0XSE_BUTfteG9TawS09WzUYLQ,1220
-tutils/trainer/learner.py,sha256=6B_zmNyS86zfCaO6j7Htu12dNN_MEOEAaPxdyihO2LQ,3609
-tutils/trainer/learner_module.py,sha256=WDJn1pT6FkUVYehLlJ_W_8YDZsdaMh_9TF76PRwpdWY,3522
+tutils/trainer/learner.py,sha256=ioJ4N0BNSgLZZODt4jYnti1pL-c3kKTZLOm_uZXs10c,4189
+tutils/trainer/learner_module.py,sha256=ywqIOFWFsB0vBODAswMN7Ct-RllF69OXI9iHUDV9d58,3655
 tutils/trainer/monitor.py,sha256=eVL3J54IMfWX-PjQzVRKhaHuehIfu1h9RCCn-uVtb_U,1075
-tutils/trainer/recorder.py,sha256=6Z5JRbLsETlGoueQbi6fVoQQqqlsJyRGVwgL0sKpOu8,4072
+tutils/trainer/recorder.py,sha256=HuE3LsUp4rXPUgKfBgKcBWpVPgoNoHUVcjFRvJP-RhU,4192
 tutils/trainer/save.py,sha256=L_29_xs9RurvNTmCqV3r3zvG4QzwGnVpNxeItX3ni8w,576
 tutils/trainer/simple_script_helper.py,sha256=DPoeDiP5-AsjX-QeFBXTBb1M5nxsLtE7Kqdaa4ARBic,1071
-tutils/trainer/trainer.py,sha256=_FZavOCr0ewIgwGRoFGCsVdTNo67TqwommPMea6mg5M,3408
-tutils/trainer/trainer_abstract.py,sha256=OjsJ3brcK_FGVnctdmQ-3f49ku_sHwKkTAEAbLXclVQ,12684
+tutils/trainer/tester_abstract.py,sha256=n2qYckLI660CL711cu57LVrdvqsJrZ6J3X3G7gCeeCU,273
+tutils/trainer/trainer.py,sha256=ASk0_gHkZao5i0Zty5oiCqfiaKJb1aFYXJNtB1eWF_E,4184
+tutils/trainer/trainer_abstract.py,sha256=fmMRf7qw-kJ54-x8tXFkUv5rz_YxXBIHIb8q3dJpTTs,15046
 tutils/trainer/trainer_ddp.py,sha256=lVQSG2OsPqY88Q35Yas1lc4ghThzaGUgpy6HfIYUOs4,6926
+tutils/trainer/trainer_ddp2.py,sha256=GQQMPMFZxL34nUzCWNTPGPKxRTQxLVzxfMBLmj-o04o,2398
 tutils/trainer/tuner_exec.py,sha256=XDRZm4o7RuqJG0atDRuYTJ0wv9lyU9WIdMypkWThHMM,5611
 tutils/trainer/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tutils/trainer/utils/trainer_utils.py,sha256=SpPBIJn-0umi2PapIZlSldFPofdGCSg65xb8ZPPtJDg,1218
 tutils/tutils/NOTES.md,sha256=GbLgIZmFe5f3_h_kpA4uFW6mjd2WTNzQnSqULMjbf3M,103
-tutils/tutils/__init__.py,sha256=4-IOOs4kFHI_kYnN8n2Y3INqFUBq8kBwUPBDbbXFdwc,465
+tutils/tutils/__init__.py,sha256=4q8BqwzOZ3W0a_Y7BkzMryqYN0kdZMqcm2JsR2R88kw,528
 tutils/tutils/build_proj.py,sha256=g75AkmrwOKRqyy0068XA9BJ8o4QuMd2OA_Dwsc8rL2o,1623
-tutils/tutils/csv_recorder.py,sha256=KmEwT_wmctIo73pGi0k6tyLzeTHb03AdgBRaKTjIAVA,4986
+tutils/tutils/csv_recorder.py,sha256=EfNCwP27D0NfwnOJ60fyuBFpivu9pHtXlNZxdUwdXN4,4992
 tutils/tutils/dl_utils.py,sha256=KK774SxWcx3TsaH9PGSFB-jLqI_gl3tz2a-YUwxFGfg,887
-tutils/tutils/functools.py,sha256=DOSSQxAfKvDZildbYy5PKZUin3603_Ti6P7KKCn44y4,3710
+tutils/tutils/functools.py,sha256=HX0CO719hLPMN0sQCMpCg_5F39BV00tejtU1jebK9OE,3174
 tutils/tutils/grad_cam.py,sha256=hSKYZKz26zpANWU8VNix_0vm6L836HQGyxqa_dup5hE,1495
-tutils/tutils/initializer.py,sha256=DHRKHXcM59jwaFyZ6Abz2JU5BizptgiOIQW0nI4syn8,7514
-tutils/tutils/metriclogger.py,sha256=KsDkvbnUXOY3ISKfoshF1ouAqYguDrDHx5lGueZJEBM,29190
-tutils/tutils/prologger.py,sha256=5DwwqBka_qrvbQImALmv42EXVSyZxrWpa4IyyqaZnQ0,4326
-tutils/tutils/recorder.py,sha256=93VgmQBAiw7fKeGCdFWcmxcndri3XWyjkB909WcwgZU,4057
+tutils/tutils/initializer.py,sha256=OFmKV4kOoARSTSTeqSiyupFRbhEDQPmTJPnwlOf2E5Q,11794
+tutils/tutils/initializer_old.py,sha256=meeVq55XPKd_r3UyZwoELaiLWCYzZSY66y7_EqmclpA,7457
+tutils/tutils/metriclogger.py,sha256=1el69yDP4Wms5bsbA5Lpxql410_oNuRkXafVIPngJSY,29240
+tutils/tutils/prologger.py,sha256=Uk9MjeePwB8JYzWCAyxo6X_DCn5s2EeycnpzLhmdEyQ,4361
+tutils/tutils/recorder.py,sha256=EBSq21cV8CsMILfUqpN1pNElcrUAu46yjl2PkDoAEis,4136
+tutils/tutils/tconfig.py,sha256=1hUXKRdNj8gDYFfs1iVU5cp919Y5zppP5sD9Z85LyNM,438
 tutils/tutils/techo.py,sha256=ZX31W76rchEnTRvGJCDjmre3wriM0O9dwOjcTUzjh_E,596
-tutils/tutils/tlogger.py,sha256=Z8siXYxmENF6yI33Ppk3JFVjxBQIFyc0kYCRP0ZFH0w,8382
-tutils/tutils/ttimer.py,sha256=1vvS1V6OlT1BG2T-jLHy-jp06IPznPbRMvl49CaS3t8,3005
-tutils/tutils/tutils.py,sha256=F9m2NSTLkcbcH0CG_JvL9lMvauLDVQGOhrcwnfHPEdg,3527
+tutils/tutils/tlogger.py,sha256=uBz539fMxJMwMVt7vPcK8F2ixiDtOiTwKwkCrNvVzTs,9946
+tutils/tutils/torch_utils.py,sha256=Ug8hsszfmY4B7R0tFZtvAi9CbYmQ1k3TeRiKh5vc4Ns,996
+tutils/tutils/ttimer.py,sha256=Ho-Mar6ly462JKAYzBhz3hlBwJ4KkCs4Pnm6ik61dLk,3044
+tutils/tutils/tutils.py,sha256=HATVOnBBGgmeh_5NKa2TBTtMyzxF0QMyINLLIVXDBo0,3841
 tutils/tutils/visualizers/__init__.py,sha256=PnSZfb_KRZfpHuVQ5kvxLJMr8ECi3gLZOonDoUahzjY,93
+tutils/tutils/visualizers/draw_bar_auto_split.py,sha256=1YUjQBw56rYXptlS9A-DTlmqpDXVq2aFY50pS01curc,2254
 tutils/tutils/visualizers/draw_curves.py,sha256=tpZJAtRVXKsStU6EJlXj_p-4YfhEJOBkaEH8_A3FLpQ,3093
 tutils/tutils/visualizers/plt_print_3d.py,sha256=loYLeQ6tG-4yl7Qj2O9OmeModjmbpbY4mndb4ipsqgA,1655
-tutils/tutils/visualizers/print_image.py,sha256=6qSoQmFJ7SEwe4NQ0NJNkrm4HK5XgF9jYkOxvTaikew,1761
+tutils/tutils/visualizers/print_image.py,sha256=gAQqdFDXhmG4edAkxZvM06cm9_zYlFrNDMl316LTq8g,1969
 tutils/tutils/visualizers/print_landmark.py,sha256=BCPM2XyC0n7nI88g_MVbfZ4NvosqdP44zyh0mdsImIE,1949
 tutils/tutils/visualizers/tsne.py,sha256=jG3iYkSV1y2F_xKdBfpgmCznWHfG6kXqTq8ihdv76hA,2817
-trans_utils-0.2.2.dist-info/METADATA,sha256=AdIcOR2l7goig37_DQ0-GD2qCZSdKvN4Arh-RUDx0tQ,533
-trans_utils-0.2.2.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-trans_utils-0.2.2.dist-info/entry_points.txt,sha256=WzJdMF51WcZPQk9O_XeHNwiS3scIoRs3H1nyFxFc_R0,113
-trans_utils-0.2.2.dist-info/top_level.txt,sha256=C7j1awDP_zdjrdFOK0kjReESxMSumnDfG2x1_ra_X08,7
-trans_utils-0.2.2.dist-info/RECORD,,
+trans_utils-0.3.0.dist-info/LICENSE,sha256=sKhSWis5Xte-iD2VRSR_gCEdgCx0GsRPJkksIjyOJFs,11599
+trans_utils-0.3.0.dist-info/METADATA,sha256=QCLKlAV2-gWJpiOVq3-LYONJES74mvHgK7oYRMAzJLk,474
+trans_utils-0.3.0.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+trans_utils-0.3.0.dist-info/entry_points.txt,sha256=OWqiUC73x1GjK3GeymbIK4Mo1-Pv83egBnVSQ3qFDNM,112
+trans_utils-0.3.0.dist-info/top_level.txt,sha256=C7j1awDP_zdjrdFOK0kjReESxMSumnDfG2x1_ra_X08,7
+trans_utils-0.3.0.dist-info/RECORD,,
```

