# Comparing `tmp/test_yolo-0.0.11-py3-none-any.whl.zip` & `tmp/test_yolo-0.0.12-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 97929 bytes, number of entries: 29
+Zip file size: 97913 bytes, number of entries: 29
 -rw-r--r--  2.0 unx       49 b- defN 23-Apr-09 08:12 test_yolo/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-21 10:25 test_yolo/detect.py
 -rw-r--r--  2.0 unx      238 b- defN 22-Sep-21 10:16 test_yolo/load_utils.py
 -rw-r--r--  2.0 unx    14484 b- defN 22-Sep-21 10:57 test_yolo/model_utils.py
 -rw-r--r--  2.0 unx        6 b- defN 22-Aug-18 08:56 test_yolo/models/__init__.py
--rw-r--r--  2.0 unx    84459 b- defN 22-Aug-18 09:19 test_yolo/models/common.py
--rw-r--r--  2.0 unx    10290 b- defN 22-Aug-18 09:15 test_yolo/models/experimental.py
--rw-r--r--  2.0 unx    40083 b- defN 22-Sep-21 11:00 test_yolo/models/yolo.py
+-rw-r--r--  2.0 unx    84439 b- defN 23-Apr-09 08:22 test_yolo/models/common.py
+-rw-r--r--  2.0 unx    10285 b- defN 23-Apr-09 08:23 test_yolo/models/experimental.py
+-rw-r--r--  2.0 unx    40053 b- defN 23-Apr-09 08:24 test_yolo/models/yolo.py
 -rw-r--r--  2.0 unx       92 b- defN 22-Aug-18 09:18 test_yolo/utils/__init__.py
 -rw-r--r--  2.0 unx     2248 b- defN 22-Aug-18 08:56 test_yolo/utils/activations.py
 -rw-r--r--  2.0 unx     5616 b- defN 22-Aug-18 08:56 test_yolo/utils/add_nms.py
 -rw-r--r--  2.0 unx     7142 b- defN 22-Aug-18 09:17 test_yolo/utils/autoanchor.py
 -rw-r--r--  2.0 unx    56222 b- defN 22-Sep-21 10:54 test_yolo/utils/datasets.py
 -rw-r--r--  2.0 unx    36806 b- defN 22-Aug-18 09:01 test_yolo/utils/general.py
 -rw-r--r--  2.0 unx     3302 b- defN 22-Aug-18 08:56 test_yolo/utils/google_utils.py
@@ -19,13 +19,13 @@
 -rw-r--r--  2.0 unx    20944 b- defN 22-Aug-18 09:02 test_yolo/utils/plots.py
 -rw-r--r--  2.0 unx    15467 b- defN 22-Aug-22 11:37 test_yolo/utils/torch_utils.py
 -rw-r--r--  2.0 unx        5 b- defN 22-Aug-18 08:56 test_yolo/utils/aws/__init__.py
 -rw-r--r--  2.0 unx     1112 b- defN 22-Aug-18 09:13 test_yolo/utils/aws/resume.py
 -rw-r--r--  2.0 unx        6 b- defN 22-Aug-18 08:56 test_yolo/utils/wandb_logging/__init__.py
 -rw-r--r--  2.0 unx      815 b- defN 22-Aug-18 08:56 test_yolo/utils/wandb_logging/log_dataset.py
 -rw-r--r--  2.0 unx    16265 b- defN 22-Aug-18 08:56 test_yolo/utils/wandb_logging/wandb_utils.py
--rw-rw-r--  2.0 unx     1062 b- defN 23-Apr-09 08:13 test_yolo-0.0.11.dist-info/LICENSE
--rw-r--r--  2.0 unx     3269 b- defN 23-Apr-09 08:13 test_yolo-0.0.11.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 08:13 test_yolo-0.0.11.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-09 08:13 test_yolo-0.0.11.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2446 b- defN 23-Apr-09 08:13 test_yolo-0.0.11.dist-info/RECORD
-29 files, 406433 bytes uncompressed, 93985 bytes compressed:  76.9%
+-rw-rw-r--  2.0 unx     1062 b- defN 23-Apr-09 08:25 test_yolo-0.0.12.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3269 b- defN 23-Apr-09 08:25 test_yolo-0.0.12.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 08:25 test_yolo-0.0.12.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-09 08:25 test_yolo-0.0.12.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2446 b- defN 23-Apr-09 08:25 test_yolo-0.0.12.dist-info/RECORD
+29 files, 406378 bytes uncompressed, 93969 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -66,23 +66,23 @@
 
 Filename: test_yolo/utils/wandb_logging/log_dataset.py
 Comment: 
 
 Filename: test_yolo/utils/wandb_logging/wandb_utils.py
 Comment: 
 
-Filename: test_yolo-0.0.11.dist-info/LICENSE
+Filename: test_yolo-0.0.12.dist-info/LICENSE
 Comment: 
 
-Filename: test_yolo-0.0.11.dist-info/METADATA
+Filename: test_yolo-0.0.12.dist-info/METADATA
 Comment: 
 
-Filename: test_yolo-0.0.11.dist-info/WHEEL
+Filename: test_yolo-0.0.12.dist-info/WHEEL
 Comment: 
 
-Filename: test_yolo-0.0.11.dist-info/top_level.txt
+Filename: test_yolo-0.0.12.dist-info/top_level.txt
 Comment: 
 
-Filename: test_yolo-0.0.11.dist-info/RECORD
+Filename: test_yolo-0.0.12.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## test_yolo/models/common.py

```diff
@@ -9,18 +9,18 @@
 import torch.nn as nn
 import torch.nn.functional as F
 from torchvision.ops import DeformConv2d
 from PIL import Image
 from torch.cuda import amp
 import sys
 
-from yolov7_package.utils.datasets import letterbox
-from yolov7_package.utils.general import non_max_suppression, make_divisible, scale_coords, increment_path, xyxy2xywh
-from yolov7_package.utils.plots import color_list, plot_one_box
-from yolov7_package.utils.torch_utils import time_synchronized
+from test_yolo.utils.datasets import letterbox
+from test_yolo.utils.general import non_max_suppression, make_divisible, scale_coords, increment_path, xyxy2xywh
+from test_yolo.utils.plots import color_list, plot_one_box
+from test_yolo.utils.torch_utils import time_synchronized
 
 
 ##### basic ####
 
 def autopad(k, p=None):  # kernel, padding
     # Pad to 'same'
     if p is None:
```

## test_yolo/models/experimental.py

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import random
 import torch
 import torch.nn as nn
 
 from .common import Conv, DWConv
-from yolov7_package.utils.google_utils import attempt_download
+from test_yolo.utils.google_utils import attempt_download
 
 
 class CrossConv(nn.Module):
     # Cross Convolution Downsample
     def __init__(self, c1, c2, k=3, s=1, g=1, e=1.0, shortcut=False):
         # ch_in, ch_out, kernel, stride, groups, expansion, shortcut
         super(CrossConv, self).__init__()
```

## test_yolo/models/yolo.py

```diff
@@ -2,21 +2,21 @@
 import logging
 import sys
 from copy import deepcopy
 
 sys.path.append('./')  # to run '$ python *.py' files in subdirectories
 logger = logging.getLogger(__name__)
 import torch
-from yolov7_package.models.common import *
-from yolov7_package.models.experimental import *
-from yolov7_package.utils import check_anchor_order
-from yolov7_package.utils import make_divisible, check_file, set_logging
-from yolov7_package.utils import time_synchronized, fuse_conv_and_bn, model_info, scale_img, initialize_weights, \
+from test_yolo.models.common import *
+from test_yolo.models.experimental import *
+from test_yolo.utils import check_anchor_order
+from test_yolo.utils import make_divisible, check_file, set_logging
+from test_yolo.utils import time_synchronized, fuse_conv_and_bn, model_info, scale_img, initialize_weights, \
     select_device, copy_attr
-from yolov7_package.utils.loss import SigmoidBin
+from test_yolo.utils.loss import SigmoidBin
 
 try:
     import thop  # for FLOPS computation
 except ImportError:
     thop = None
```

## Comparing `test_yolo-0.0.11.dist-info/LICENSE` & `test_yolo-0.0.12.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `test_yolo-0.0.11.dist-info/METADATA` & `test_yolo-0.0.12.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-yolo
-Version: 0.0.11
+Version: 0.0.12
 Summary: Bindings for yolov7 in one class
 Home-page: https://github.com/maxwolf8852/yolov7_package.git
 Author: Maxim Volkovskiy
 Author-email: maxwolf8852@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `test_yolo-0.0.11.dist-info/RECORD` & `test_yolo-0.0.12.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 test_yolo/__init__.py,sha256=IEX5qbCfSfH2qSfsOo33dG48pUc2PmDE_66xWnlqeCA,49
 test_yolo/detect.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test_yolo/load_utils.py,sha256=nmulu5GjXnYMcRpwr-PoQp1MU7EvE1h9rur70BxQW7Y,238
 test_yolo/model_utils.py,sha256=qgejYk3ucGQboqJEdEdFPv7APDLnEptPvRm22sVeBLE,14484
 test_yolo/models/__init__.py,sha256=BIYCj6TRzGWCEbYG5ZNaTHQ4am6c9QVbgS80hLG0blc,6
-test_yolo/models/common.py,sha256=cTtVefnJfbQihKbJ0vi_pDkrZ9Q2M87dtu9L3LXsb8U,84459
-test_yolo/models/experimental.py,sha256=cDY_rb1kLSWyGfQ3Biwsk-bQMnw9gAFqMztQZ5Zvbv0,10290
-test_yolo/models/yolo.py,sha256=eHxSL6srTCvO-76N6hE13bUIhWYamWxjOuUW3W7cwcE,40083
+test_yolo/models/common.py,sha256=DDBaD_pNB7pvYMY-cCp2ZCavCftlatVN7MC4Qg8f4zo,84439
+test_yolo/models/experimental.py,sha256=COJBc1GEM78GCklloPwP-6aunQOd4_xRsjA36YgYKLY,10285
+test_yolo/models/yolo.py,sha256=qCfQpMbco7zny0HKhk-NkQ8C9l_mgwK4Ra8nxbz3DHg,40053
 test_yolo/utils/__init__.py,sha256=E7r7w3Pw-fK_Tj9HhwcXcEJ56SUyOEZQ4PNbwyB65Es,92
 test_yolo/utils/activations.py,sha256=C5sJHUqEBU0uHN4pOMBFi1xlxl01TV2l1iFu0cR_Y4c,2248
 test_yolo/utils/add_nms.py,sha256=rJtI4xb_3jU7NMoheGMkEbML5KGeP9OUpMMjP0BhZlQ,5616
 test_yolo/utils/autoanchor.py,sha256=qB5nyYQPxWx-d98FpuoblF1rVMcC7LgTRv-1BxKXd_s,7142
 test_yolo/utils/datasets.py,sha256=zT7hejw7Wq-PsRVe_fo10yhyqyvAvGlgveWpw4W5qJA,56222
 test_yolo/utils/general.py,sha256=ZnMPKQIe-CPgHpR_F1oF3-NoacPyKYMJHM1GIwhJ51Q,36806
 test_yolo/utils/google_utils.py,sha256=j9LaBlTkfhFEBjcF9oevdWtFFwke4QiE15JjIcHG7e0,3302
@@ -18,12 +18,12 @@
 test_yolo/utils/plots.py,sha256=Czpuq4HYIZztIzSRNpusuXrnAHyq_VE_TybjuLybrL4,20944
 test_yolo/utils/torch_utils.py,sha256=7r4uhQSYmEChWUrNENskL0_ujH-DbEoFQEgoL32eqWw,15467
 test_yolo/utils/aws/__init__.py,sha256=GAMHpH0PAwUCxr_GSctfv1fxgkqvy9mpU1FBafhJmkk,5
 test_yolo/utils/aws/resume.py,sha256=B0GvCUzMxCA0uKWZwfyFxAbr6Rss5FG9ETf5yOh8Wuc,1112
 test_yolo/utils/wandb_logging/__init__.py,sha256=BIYCj6TRzGWCEbYG5ZNaTHQ4am6c9QVbgS80hLG0blc,6
 test_yolo/utils/wandb_logging/log_dataset.py,sha256=5LydLM7wFuLKrzW7UTgUovK-OuWHCwRIoWoKMKHbSag,815
 test_yolo/utils/wandb_logging/wandb_utils.py,sha256=aJLCp542HTWk6yXygizIkCSeTobYoK2ajQ6cce5OFqI,16265
-test_yolo-0.0.11.dist-info/LICENSE,sha256=IlU2zzPZa0Z3DTTluArAr-vnftTkdKuJR4Uo-lFV9E4,1062
-test_yolo-0.0.11.dist-info/METADATA,sha256=8PdXvjexQteBpzqiOFE7x_GH0Bpi1x9IXwnTh17bS0E,3269
-test_yolo-0.0.11.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-test_yolo-0.0.11.dist-info/top_level.txt,sha256=6yZONYUtmu1g7R6EL_f6zTsMjXlWvwiZ0qipI9nhaAg,10
-test_yolo-0.0.11.dist-info/RECORD,,
+test_yolo-0.0.12.dist-info/LICENSE,sha256=IlU2zzPZa0Z3DTTluArAr-vnftTkdKuJR4Uo-lFV9E4,1062
+test_yolo-0.0.12.dist-info/METADATA,sha256=AIzfn5WhKCQxJS8GEYUvAdj7HpKjmdtAhh3pd8GTVHA,3269
+test_yolo-0.0.12.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+test_yolo-0.0.12.dist-info/top_level.txt,sha256=6yZONYUtmu1g7R6EL_f6zTsMjXlWvwiZ0qipI9nhaAg,10
+test_yolo-0.0.12.dist-info/RECORD,,
```

