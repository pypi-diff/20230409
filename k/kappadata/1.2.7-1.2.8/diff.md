# Comparing `tmp/kappadata-1.2.7.tar.gz` & `tmp/kappadata-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kappadata-1.2.7.tar", last modified: Fri Apr  7 15:03:27 2023, max compression
+gzip compressed data, was "kappadata-1.2.8.tar", last modified: Sun Apr  9 01:03:19 2023, max compression
```

## Comparing `kappadata-1.2.7.tar` & `kappadata-1.2.8.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.389539 kappadata-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-07 15:01:07.000000 kappadata-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-07 15:03:27.389539 kappadata-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-04-07 15:01:07.000000 kappadata-1.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.373539 kappadata-1.2.7/kappadata/
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-04-07 15:03:12.000000 kappadata-1.2.7/kappadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.373539 kappadata-1.2.7/kappadata/caching/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/caching/cached_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/caching/shared_dict_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.373539 kappadata-1.2.7/kappadata/collators/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/collators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.373539 kappadata-1.2.7/kappadata/collators/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/collators/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/collators/base/kd_collator_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/collators/base/kd_compose_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/collators/base/kd_single_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/collators/kd_mix_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/collators/pad_sequences_collator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.373539 kappadata-1.2.7/kappadata/common/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.373539 kappadata-1.2.7/kappadata/common/collators/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/collators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/collators/mae_finetune_mix_collator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.373539 kappadata-1.2.7/kappadata/common/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/datasets/kd_image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.373539 kappadata-1.2.7/kappadata/common/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/transforms/byol_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/transforms/imagenet_minaug_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/transforms/imagenet_noaug_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/transforms/mae_finetune_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.377539 kappadata-1.2.7/kappadata/common/transforms/norm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/transforms/norm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/transforms/norm/kd_cifar100_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/transforms/norm/kd_cifar10_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/transforms/norm/kd_image_net_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.377539 kappadata-1.2.7/kappadata/common/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.377539 kappadata-1.2.7/kappadata/common/wrappers/sample_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/wrappers/sample_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/wrappers/sample_wrappers/byol_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.377539 kappadata-1.2.7/kappadata/copying/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/copying/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/copying/image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.377539 kappadata-1.2.7/kappadata/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/datasets/kd_concat_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/datasets/kd_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/datasets/kd_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/datasets/kd_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/error_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.377539 kappadata-1.2.7/kappadata/loading/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/loading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/loading/image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.377539 kappadata-1.2.7/kappadata/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/samplers/infinite_batch_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/samplers/interleaved_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.381539 kappadata-1.2.7/kappadata/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/add_gaussian_noise_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.381539 kappadata-1.2.7/kappadata/transforms/base/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/base/kd_compose_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/base/kd_identity_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/base/kd_random_apply_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/base/kd_scheduled_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/base/kd_stochastic_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/base/kd_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/image_pos_embed_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/image_pos_embed_sincos.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_bucketize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_gaussian_blur_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_gaussian_blur_tv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_rand_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_rand_augment_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_random_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_random_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_random_erasing.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_random_gaussian_blur_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_random_gaussian_blur_tv.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_random_grayscale.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_random_horizontal_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_random_resized_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_random_solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_rearrange.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/kd_solarize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.381539 kappadata-1.2.7/kappadata/transforms/norm/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/norm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.381539 kappadata-1.2.7/kappadata/transforms/norm/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/norm/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/norm/base/kd_norm_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/norm/kd_image_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/norm/kd_image_range_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/patchify_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/patchwise_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/patchwise_random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/patchwise_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/save_state_to_context_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/transforms/unpatchify_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.385539 kappadata-1.2.7/kappadata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/utils/class_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/utils/color_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/utils/magnitude_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/utils/multi_crop_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/utils/one_hot.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/utils/param_checking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/utils/pos_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/utils/save_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/utils/transform_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.385539 kappadata-1.2.7/kappadata/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.385539 kappadata-1.2.7/kappadata/wrappers/dataset_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/dataset_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/dataset_wrappers/shuffle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/dataset_wrappers/subset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/mode_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.385539 kappadata-1.2.7/kappadata/wrappers/sample_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/sample_wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.389539 kappadata-1.2.7/kappadata/wrappers/sample_wrappers/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/sample_wrappers/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/sample_wrappers/kd_mix_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/sample_wrappers/one_hot_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/sample_wrappers/source_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/sample_wrappers/target_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/sample_wrappers/x_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/sample_wrappers/y_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-07 15:01:07.000000 kappadata-1.2.7/kappadata/wrappers/torch_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:03:27.373539 kappadata-1.2.7/kappadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-07 15:03:27.000000 kappadata-1.2.7/kappadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-07 15:03:27.000000 kappadata-1.2.7/kappadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 15:03:27.000000 kappadata-1.2.7/kappadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 15:03:27.000000 kappadata-1.2.7/kappadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 15:03:27.000000 kappadata-1.2.7/kappadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-07 15:01:07.000000 kappadata-1.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-07 15:03:27.389539 kappadata-1.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.023927 kappadata-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-09 01:00:29.000000 kappadata-1.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-09 01:03:19.023927 kappadata-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-04-09 01:00:29.000000 kappadata-1.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.967926 kappadata-1.2.8/kappadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-04-09 01:03:00.000000 kappadata-1.2.8/kappadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.971926 kappadata-1.2.8/kappadata/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/caching/cached_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/caching/shared_dict_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.971926 kappadata-1.2.8/kappadata/collators/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/collators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.975926 kappadata-1.2.8/kappadata/collators/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/collators/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/collators/base/kd_collator_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/collators/base/kd_compose_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/collators/base/kd_single_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/collators/kd_mix_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/collators/pad_sequences_collator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.975926 kappadata-1.2.8/kappadata/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.975926 kappadata-1.2.8/kappadata/common/collators/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/collators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/collators/mae_finetune_mix_collator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.975926 kappadata-1.2.8/kappadata/common/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/datasets/kd_image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.979926 kappadata-1.2.8/kappadata/common/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/transforms/byol_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/transforms/imagenet_minaug_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/transforms/imagenet_noaug_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/transforms/mae_finetune_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.979926 kappadata-1.2.8/kappadata/common/transforms/norm/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/transforms/norm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/transforms/norm/kd_cifar100_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/transforms/norm/kd_cifar10_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/transforms/norm/kd_image_net_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.979926 kappadata-1.2.8/kappadata/common/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.983926 kappadata-1.2.8/kappadata/common/wrappers/sample_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/wrappers/sample_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/wrappers/sample_wrappers/byol_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.983926 kappadata-1.2.8/kappadata/copying/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/copying/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/copying/image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.987926 kappadata-1.2.8/kappadata/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/datasets/kd_concat_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/datasets/kd_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/datasets/kd_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/datasets/kd_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/error_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.987926 kappadata-1.2.8/kappadata/loading/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/loading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/loading/image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.987926 kappadata-1.2.8/kappadata/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/samplers/infinite_batch_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/samplers/interleaved_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.003927 kappadata-1.2.8/kappadata/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/add_gaussian_noise_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.007927 kappadata-1.2.8/kappadata/transforms/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/base/kd_compose_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/base/kd_identity_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/base/kd_random_apply_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/base/kd_scheduled_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/base/kd_stochastic_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/base/kd_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/image_pos_embed_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/image_pos_embed_sincos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_bucketize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_gaussian_blur_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_gaussian_blur_tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_rand_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_rand_augment_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_erasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_gaussian_blur_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_gaussian_blur_tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_horizontal_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_resized_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_rearrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_solarize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.007927 kappadata-1.2.8/kappadata/transforms/norm/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/norm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.007927 kappadata-1.2.8/kappadata/transforms/norm/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/norm/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/norm/base/kd_norm_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/norm/kd_image_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/norm/kd_image_range_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/patchify_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/patchwise_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/patchwise_random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/patchwise_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/save_state_to_context_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/unpatchify_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.015927 kappadata-1.2.8/kappadata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/class_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/color_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/magnitude_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/multi_crop_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/one_hot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/param_checking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/pos_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/save_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/transform_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.015927 kappadata-1.2.8/kappadata/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.019927 kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/shuffle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/subset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/mode_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.023927 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.023927 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/kd_mix_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/one_hot_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/source_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/target_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/x_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/y_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/torch_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.967926 kappadata-1.2.8/kappadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-09 01:03:18.000000 kappadata-1.2.8/kappadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-09 01:03:18.000000 kappadata-1.2.8/kappadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 01:03:18.000000 kappadata-1.2.8/kappadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-09 01:03:18.000000 kappadata-1.2.8/kappadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 01:03:18.000000 kappadata-1.2.8/kappadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-09 01:00:29.000000 kappadata-1.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-09 01:03:19.023927 kappadata-1.2.8/setup.cfg
```

### Comparing `kappadata-1.2.7/LICENSE` & `kappadata-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/PKG-INFO` & `kappadata-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappadata
-Version: 1.2.7
+Version: 1.2.8
 Summary: pytorch dataset wrappers for in-memory caching
 Home-page: https://github.com/BenediktAlkin/KappaData
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaData
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kappadata-1.2.7/README.md` & `kappadata-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/__init__.py` & `kappadata-1.2.8/kappadata/__init__.py`

 * *Files identical despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.2.7"
+__version__ = "1.2.8"
 
 import kappadata.caching
 import kappadata.common
 import kappadata.copying
 import kappadata.datasets
 import kappadata.loading
 import kappadata.transforms
```

### Comparing `kappadata-1.2.7/kappadata/caching/cached_dataset.py` & `kappadata-1.2.8/kappadata/caching/cached_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/caching/shared_dict_dataset.py` & `kappadata-1.2.8/kappadata/caching/shared_dict_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/collators/base/kd_collator_base.py` & `kappadata-1.2.8/kappadata/collators/base/kd_collator_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/collators/base/kd_compose_collator.py` & `kappadata-1.2.8/kappadata/collators/base/kd_compose_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/collators/base/kd_single_collator.py` & `kappadata-1.2.8/kappadata/collators/base/kd_single_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/collators/kd_mix_collator.py` & `kappadata-1.2.8/kappadata/collators/kd_mix_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/collators/pad_sequences_collator.py` & `kappadata-1.2.8/kappadata/collators/pad_sequences_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/common/__init__.py` & `kappadata-1.2.8/kappadata/common/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import kappadata.common.transforms
 import kappadata.common.wrappers
 # collators
 from .collators import MAEFinetuneMixCollator
 # datasets
 from .datasets.kd_image_folder import KDImageFolder
 # transforms
-from .transforms import BYOLTransform0, BYOLTransform1
+from .transforms import BYOLTransform, BYOLTransform0, BYOLTransform1
 from .transforms import MAEFinetuneTransform
 from .transforms.norm.kd_cifar100_norm import KDCifar100Norm
 # norm
 from .transforms.norm.kd_cifar10_norm import KDCifar10Norm
 from .transforms.norm.kd_image_net_norm import KDImageNetNorm
 # wrappers
 from .wrappers import (
```

### Comparing `kappadata-1.2.7/kappadata/common/datasets/kd_image_folder.py` & `kappadata-1.2.8/kappadata/common/datasets/kd_image_folder.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,13 +28,12 @@
         x = self.transform(x, ctx=ctx)
         return x
 
     # noinspection PyUnusedLocal
     def getitem_class(self, idx, ctx=None):
         return self.dataset.targets[idx]
 
-    @property
-    def n_classes(self):
-        return len(self.dataset.classes)
+    def getshape_class(self):
+        return len(self.dataset.classes),
 
     def __len__(self):
         return len(self.dataset)
```

### Comparing `kappadata-1.2.7/kappadata/common/transforms/imagenet_minaug_transforms.py` & `kappadata-1.2.8/kappadata/common/transforms/imagenet_minaug_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/common/transforms/imagenet_noaug_transforms.py` & `kappadata-1.2.8/kappadata/common/transforms/imagenet_noaug_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/common/transforms/mae_finetune_transform.py` & `kappadata-1.2.8/kappadata/common/transforms/mae_finetune_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py` & `kappadata-1.2.8/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py` & `kappadata-1.2.8/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py` & `kappadata-1.2.8/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/copying/image_folder.py` & `kappadata-1.2.8/kappadata/copying/image_folder.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/datasets/kd_concat_dataset.py` & `kappadata-1.2.8/kappadata/datasets/kd_concat_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/datasets/kd_dataset.py` & `kappadata-1.2.8/kappadata/datasets/kd_wrapper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,61 @@
-import logging
-
-from torch.utils.data import Dataset
-
 from kappadata.errors import UseModeWrapperException
+from .kd_dataset import KDDataset
 
 
-class KDDataset(Dataset):
-    def __init__(self):
+class KDWrapper(KDDataset):
+    def __init__(self, dataset: KDDataset, ctx_prefix: str = None):
         super().__init__()
-        self.logger = logging.getLogger(type(self).__name__)
+        self.dataset = dataset
+        self.ctx_prefix = ctx_prefix or type(self).__name__
+        # children should overwrite _worker_init_fn
+        assert type(self).worker_init_fn == KDWrapper.worker_init_fn
 
     def __len__(self):
-        raise NotImplementedError
+        return len(self.dataset)
 
-    def __enter__(self):
-        return self
+    def __getattr__(self, item):
+        if item == "dataset":
+            return getattr(super(), item)
+        return getattr(self.dataset, item)
 
-    def __exit__(self, *_):
-        self.dispose()
+    def __getitem__(self, idx):
+        raise UseModeWrapperException
 
     def dispose(self):
-        """ release resources occupied by dataset (e.g. filehandles) """
-        pass
+        self.dataset.dispose()
 
     @property
     def root_dataset(self):
-        return self
+        # KDDataset implements root_dataset -> __getitem__ doesn't trigger
+        return self.dataset.root_dataset
 
-    @staticmethod
-    def has_wrapper(wrapper):
-        return False
-
-    @staticmethod
-    def has_wrapper_type(wrapper_type):
-        return False
+    def has_wrapper(self, wrapper):
+        if self == wrapper:
+            return True
+        return self.dataset.has_wrapper(wrapper)
+
+    def has_wrapper_type(self, wrapper_type):
+        if type(self) == wrapper_type:
+            return True
+        return self.dataset.has_wrapper_type(wrapper_type)
 
     @property
     def all_wrappers(self):
-        return []
+        return [self] + self.dataset.all_wrappers
 
     @property
     def all_wrapper_types(self):
-        return []
-
-    def get_wrapper_of_type(self, wrapper_type):
-        wrappers = self.get_wrappers_of_type(wrapper_type)
-        if len(wrappers) == 0:
-            return None
-        assert len(wrappers) == 1
-        return wrappers[0]
+        return [type(self)] + self.dataset.all_wrapper_types
 
     def get_wrappers_of_type(self, wrapper_type):
-        return []
+        wrappers = self.dataset.get_wrappers_of_type(wrapper_type)
+        if type(self) == wrapper_type:
+            return [self] + wrappers
+        return wrappers
 
     def worker_init_fn(self, rank, **kwargs):
-        pass
+        self._worker_init_fn(rank, **kwargs)
+        self.dataset.worker_init_fn(rank, **kwargs)
 
-    def __getitem__(self, idx):
-        raise UseModeWrapperException
+    def _worker_init_fn(self, rank, **kwargs):
+        pass
```

### Comparing `kappadata-1.2.7/kappadata/datasets/kd_subset.py` & `kappadata-1.2.8/kappadata/datasets/kd_subset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/factory.py` & `kappadata-1.2.8/kappadata/factory.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/samplers/infinite_batch_sampler.py` & `kappadata-1.2.8/kappadata/samplers/infinite_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/samplers/interleaved_sampler.py` & `kappadata-1.2.8/kappadata/samplers/interleaved_sampler.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,24 @@
 class InterleavedSamplerConfig:
     sampler: object
     every_n_epochs: int = None
     every_n_updates: int = None
     every_n_samples: int = None
     collator: callable = None
 
+    def __str__(self):
+        interval_strs = []
+        if self.every_n_epochs is not None:
+            interval_strs.append(f"every_n_epochs={self.every_n_epochs}")
+        if self.every_n_updates is not None:
+            interval_strs.append(f"every_n_updates={self.every_n_updates}")
+        if self.every_n_samples is not None:
+            interval_strs.append(f"every_n_samples={self.every_n_samples}")
+        return f"{type(self).__name__}({','.join(interval_strs)})"
+
 
 class InterleavedSampler:
     def __init__(
             self,
             main_sampler,
             batch_size,
             configs=None,
```

### Comparing `kappadata-1.2.7/kappadata/transforms/__init__.py` & `kappadata-1.2.8/kappadata/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/add_gaussian_noise_transform.py` & `kappadata-1.2.8/kappadata/transforms/add_gaussian_noise_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/base/kd_compose_transform.py` & `kappadata-1.2.8/kappadata/transforms/base/kd_compose_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/base/kd_random_apply_base.py` & `kappadata-1.2.8/kappadata/transforms/base/kd_random_apply_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/base/kd_scheduled_transform.py` & `kappadata-1.2.8/kappadata/transforms/base/kd_scheduled_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/base/kd_transform.py` & `kappadata-1.2.8/kappadata/transforms/base/kd_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/image_pos_embed_grid.py` & `kappadata-1.2.8/kappadata/transforms/image_pos_embed_grid.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/image_pos_embed_sincos.py` & `kappadata-1.2.8/kappadata/transforms/image_pos_embed_sincos.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/kd_bucketize.py` & `kappadata-1.2.8/kappadata/transforms/kd_bucketize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/kd_color_jitter.py` & `kappadata-1.2.8/kappadata/transforms/kd_color_jitter.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/kd_gaussian_blur_pil.py` & `kappadata-1.2.8/kappadata/transforms/kd_gaussian_blur_pil.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/kd_gaussian_blur_tv.py` & `kappadata-1.2.8/kappadata/transforms/kd_gaussian_blur_tv.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/kd_rand_augment.py` & `kappadata-1.2.8/kappadata/transforms/kd_rand_augment.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/kd_random_color_jitter.py` & `kappadata-1.2.8/kappadata/transforms/kd_random_color_jitter.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/kd_random_crop.py` & `kappadata-1.2.8/kappadata/transforms/kd_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/kd_random_erasing.py` & `kappadata-1.2.8/kappadata/transforms/kd_random_erasing.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/kd_random_gaussian_blur_pil.py` & `kappadata-1.2.8/kappadata/transforms/kd_random_gaussian_blur_pil.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/kd_random_gaussian_blur_tv.py` & `kappadata-1.2.8/kappadata/transforms/kd_random_gaussian_blur_tv.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/kd_random_grayscale.py` & `kappadata-1.2.8/kappadata/transforms/kd_random_grayscale.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/kd_random_resized_crop.py` & `kappadata-1.2.8/kappadata/transforms/kd_random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/kd_random_rotation.py` & `kappadata-1.2.8/kappadata/transforms/kd_random_rotation.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/kd_random_solarize.py` & `kappadata-1.2.8/kappadata/transforms/kd_random_solarize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/kd_resize.py` & `kappadata-1.2.8/kappadata/transforms/kd_resize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/kd_solarize.py` & `kappadata-1.2.8/kappadata/transforms/kd_solarize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/norm/base/kd_norm_base.py` & `kappadata-1.2.8/kappadata/transforms/norm/base/kd_norm_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/norm/kd_image_norm.py` & `kappadata-1.2.8/kappadata/transforms/norm/kd_image_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/norm/kd_image_range_norm.py` & `kappadata-1.2.8/kappadata/transforms/norm/kd_image_range_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/patchify_image.py` & `kappadata-1.2.8/kappadata/transforms/patchify_image.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/patchwise_norm.py` & `kappadata-1.2.8/kappadata/transforms/patchwise_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/transforms/patchwise_random_rotation.py` & `kappadata-1.2.8/kappadata/transforms/patchwise_random_rotation.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/utils/class_counts.py` & `kappadata-1.2.8/kappadata/utils/class_counts.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,18 +17,18 @@
     unique_classes, unique_counts = classes.unique(return_counts=True)
     counts[unique_classes] = unique_counts
     return counts
 
 
 def get_class_counts_from_dataset(dataset):
     classes = [dataset.getitem_class(i) for i in range(len(dataset))]
-    return get_class_counts(classes=classes, n_classes=dataset.n_classes)
+    return get_class_counts(classes=classes, n_classes=dataset.getdim_class())
 
 
 def get_class_counts_and_indices(dataset):
     # TODO inefficient implementation (e.g. https://stackoverflow.com/questions/30003068/how-to-get-a-list-of-all-indices-of-repeated-elements-in-a-numpy-array)
     classes = np.array([dataset.getitem_class(i) for i in range(len(dataset))])
-    counts = get_class_counts(classes=classes, n_classes=dataset.n_classes)
+    counts = get_class_counts(classes=classes, n_classes=dataset.getdim_class())
     indices = []
-    for i in range(dataset.n_classes):
+    for i in range(dataset.getdim_class()):
         indices.append((classes == i).nonzero()[0])
     return counts, indices
```

### Comparing `kappadata-1.2.7/kappadata/utils/color_histogram.py` & `kappadata-1.2.8/kappadata/utils/color_histogram.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/utils/magnitude_sampler.py` & `kappadata-1.2.8/kappadata/utils/magnitude_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/utils/multi_crop_utils.py` & `kappadata-1.2.8/kappadata/utils/multi_crop_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/utils/pos_embed.py` & `kappadata-1.2.8/kappadata/utils/pos_embed.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/utils/save_image.py` & `kappadata-1.2.8/kappadata/utils/save_image.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/utils/transform_utils.py` & `kappadata-1.2.8/kappadata/utils/transform_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py` & `kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py` & `kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             # create indices from start/end index
             assert start_index is None or isinstance(start_index, int)
             assert end_index is None or isinstance(end_index, int)
             end_index = end_index or len(dataset)
             end_index = min(end_index, len(dataset))
             start_index = start_index or 0
             assert start_index <= end_index
-            for i in range(dataset.n_classes):
+            for i in range(dataset.getdim_class()):
                 if check_enough_samples:
                     assert counts[i] >= end_index, too_little_samples_for_class(i, counts[i], end_index)
                 if start_index >= counts[i]:
                     continue
                 cur_end_index = min(end_index, counts[i])
                 sub_indices += all_indices[i][start_index:cur_end_index].tolist()
         elif start_percent is not None or end_percent is not None:
@@ -37,15 +37,15 @@
             assert start_index is None and end_index is None
             assert start_percent is not None or end_percent is not None
             assert start_percent is None or (isinstance(start_percent, (float, int)) and 0. <= start_percent <= 1.)
             assert end_percent is None or (isinstance(end_percent, (float, int)) and 0. <= end_percent <= 1.)
             start_percent = start_percent or 0.
             end_percent = end_percent or 1.
             assert start_percent <= end_percent
-            for i in range(dataset.n_classes):
+            for i in range(dataset.getdim_class()):
                 start_index = int(start_percent * counts[i])
                 end_index = int(end_percent * counts[i])
                 sub_indices += all_indices[i][start_index:end_index].tolist()
         else:
             raise NotImplementedError
 
         super().__init__(dataset=dataset, indices=sub_indices)
```

### Comparing `kappadata-1.2.7/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py` & `kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             classes = dataset.getall_class()
             if isinstance(classes, np.ndarray):
                 classes = torch.from_numpy(classes)
             elif not torch.is_tensor(classes):
                 classes = torch.tensor(classes)
         else:
             classes = torch.tensor([dataset.getitem_class(i) for i in range(len(dataset))])
-        class_counts = get_class_counts(classes, dataset.n_classes)
+        class_counts = get_class_counts(classes, dataset.getdim_class())
         max_class_count = torch.max(class_counts)
         indices = torch.arange(len(dataset), dtype=torch.long)
         if self.strategy == "multiply":
             # append miniority classes as long as they are not bigger than the majority class
             for i in range(len(class_counts)):
                 # if class is not contained in dataset -> cant multiply sample
                 if class_counts[i] == 0:
```

### Comparing `kappadata-1.2.7/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py` & `kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py` & `kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/wrappers/dataset_wrappers/subset_wrapper.py` & `kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/subset_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/wrappers/mode_wrapper.py` & `kappadata-1.2.8/kappadata/wrappers/mode_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py` & `kappadata-1.2.8/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/wrappers/sample_wrappers/kd_mix_wrapper.py` & `kappadata-1.2.8/kappadata/wrappers/sample_wrappers/kd_mix_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,12 +115,12 @@
 
     def getitem_class(self, idx, ctx=None):
         _, idx2, lamb, _, _ = self._shared(idx, ctx=ctx)
         y = self.dataset.getitem_class(idx, ctx=ctx)
         if idx2 == -1:
             return y
         y2 = self.dataset.getitem_class(idx2, ctx={})
-        y = to_one_hot_vector(y, n_classes=self.dataset.n_classes)
-        y2 = to_one_hot_vector(y2, n_classes=self.dataset.n_classes)
+        y = to_one_hot_vector(y, n_classes=self.dataset.getdim_class())
+        y2 = to_one_hot_vector(y2, n_classes=self.dataset.getdim_class())
 
         y.mul_(lamb).add_(y2.mul_(1. - lamb))
         return y
```

### Comparing `kappadata-1.2.7/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py` & `kappadata-1.2.8/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py` & `kappadata-1.2.8/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,13 @@
         super().__init__(dataset=dataset)
         assert isinstance(smoothing, (int, float)) and 0. < smoothing < 1.
         self.smoothing = smoothing
 
     def getitem_class(self, idx, ctx=None):
         y = self.dataset.getitem_class(idx, ctx)
         assert isinstance(y, int) or (torch.is_tensor(y) and y.ndim == 0)
-        n_classes = self.dataset.n_classes
+        n_classes = self.dataset.getdim_class()
         off_value = self.smoothing / n_classes
         on_value = 1. - self.smoothing + off_value
         y_vector = torch.full(size=(n_classes,), fill_value=off_value)
         y_vector[y] = on_value
         return y_vector
```

### Comparing `kappadata-1.2.7/kappadata/wrappers/torch_wrapper.py` & `kappadata-1.2.8/kappadata/wrappers/torch_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/kappadata.egg-info/PKG-INFO` & `kappadata-1.2.8/kappadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappadata
-Version: 1.2.7
+Version: 1.2.8
 Summary: pytorch dataset wrappers for in-memory caching
 Home-page: https://github.com/BenediktAlkin/KappaData
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaData
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kappadata-1.2.7/kappadata.egg-info/SOURCES.txt` & `kappadata-1.2.8/kappadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.7/setup.cfg` & `kappadata-1.2.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.2.7
+version = 1.2.8
 name = kappadata
 description = pytorch dataset wrappers for in-memory caching
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BenediktAlkin/KappaData
 project_urls = 
 	Source Code = https://github.com/BenediktAlkin/KappaData
```

