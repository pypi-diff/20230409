# Comparing `tmp/image-reward-0.92.tar.gz` & `tmp/image-reward-0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-reward-0.92.tar", last modified: Sat Apr  8 09:04:35 2023, max compression
+gzip compressed data, was "image-reward-0.93.tar", last modified: Sun Apr  9 02:43:26 2023, max compression
```

## Comparing `image-reward-0.92.tar` & `image-reward-0.93.tar`

### file list

```diff
@@ -1,21 +1,15 @@
-drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-08 09:04:35.713121 image-reward-0.92/
-drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-08 09:04:35.713121 image-reward-0.92/ImageReward/
-drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-08 09:04:35.713121 image-reward-0.92/ImageReward/BLIP/
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-06 11:43:28.000000 image-reward-0.92/ImageReward/BLIP/__init__.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     3310 2023-04-06 11:43:28.000000 image-reward-0.92/ImageReward/BLIP/blip.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     1676 2023-04-08 08:16:04.000000 image-reward-0.92/ImageReward/BLIP/blip_pretrain.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)    41505 2023-04-06 11:43:28.000000 image-reward-0.92/ImageReward/BLIP/med.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)    14068 2023-04-06 11:43:28.000000 image-reward-0.92/ImageReward/BLIP/vit.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     2338 2023-04-08 08:08:10.000000 image-reward-0.92/ImageReward/ImageReward.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       26 2023-04-06 11:43:28.000000 image-reward-0.92/ImageReward/__init__.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     5244 2023-04-08 07:59:05.000000 image-reward-0.92/ImageReward/model.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     1946 2023-04-08 09:04:35.713121 image-reward-0.92/PKG-INFO
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     3010 2023-04-07 12:33:43.000000 image-reward-0.92/README.md
-drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-08 09:04:35.713121 image-reward-0.92/image_reward.egg-info/
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     1946 2023-04-08 09:04:35.000000 image-reward-0.92/image_reward.egg-info/PKG-INFO
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)      405 2023-04-08 09:04:35.000000 image-reward-0.92/image_reward.egg-info/SOURCES.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)        1 2023-04-08 09:04:35.000000 image-reward-0.92/image_reward.egg-info/dependency_links.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       52 2023-04-08 09:04:35.000000 image-reward-0.92/image_reward.egg-info/requires.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       12 2023-04-08 09:04:35.000000 image-reward-0.92/image_reward.egg-info/top_level.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       38 2023-04-08 09:04:35.713121 image-reward-0.92/setup.cfg
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)      972 2023-04-08 09:04:26.000000 image-reward-0.92/setup.py
+drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-09 02:43:26.507453 image-reward-0.93/
+drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-09 02:43:26.503453 image-reward-0.93/ImageReward/
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     5231 2023-04-08 13:28:23.000000 image-reward-0.93/ImageReward/ImageReward.py
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       20 2023-04-08 13:29:13.000000 image-reward-0.93/ImageReward/__init__.py
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     6322 2023-04-08 14:46:39.000000 image-reward-0.93/ImageReward/utils.py
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     1946 2023-04-09 02:43:26.503453 image-reward-0.93/PKG-INFO
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     3010 2023-04-09 02:36:32.000000 image-reward-0.93/README.md
+drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-09 02:43:26.503453 image-reward-0.93/image_reward.egg-info/
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     1946 2023-04-09 02:43:26.000000 image-reward-0.93/image_reward.egg-info/PKG-INFO
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)      269 2023-04-09 02:43:26.000000 image-reward-0.93/image_reward.egg-info/SOURCES.txt
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)        1 2023-04-09 02:43:26.000000 image-reward-0.93/image_reward.egg-info/dependency_links.txt
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       52 2023-04-09 02:43:26.000000 image-reward-0.93/image_reward.egg-info/requires.txt
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       12 2023-04-09 02:43:26.000000 image-reward-0.93/image_reward.egg-info/top_level.txt
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       38 2023-04-09 02:43:26.507453 image-reward-0.93/setup.cfg
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)      972 2023-04-09 02:43:06.000000 image-reward-0.93/setup.py
```

### Comparing `image-reward-0.92/ImageReward/model.py` & `image-reward-0.93/ImageReward/ImageReward.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 * https://github.com/openai/CLIP
 * https://github.com/christophschuhmann/improved-aesthetic-predictor
 '''
 
 import torch
 import torch.nn as nn
 from PIL import Image
-from .BLIP.blip_pretrain import BLIP_Pretrain
+from .models.BLIP.blip_pretrain import BLIP_Pretrain
 from torchvision.transforms import Compose, Resize, CenterCrop, ToTensor, Normalize
 
 try:
     from torchvision.transforms import InterpolationMode
     BICUBIC = InterpolationMode.BICUBIC
 except ImportError:
     BICUBIC = Image.BICUBIC
@@ -64,15 +64,15 @@
                 nn.init.constant_(param, val=0)
         
     def forward(self, input):
         return self.layers(input)
 
 
 class ImageReward(nn.Module):
-    def __init__(self, device='cpu', med_config = "med_config.json"):
+    def __init__(self, med_config, device='cpu'):
         super().__init__()
         self.device = device
         
         self.blip = BLIP_Pretrain(image_size=224, vit='large', med_config=med_config)
         self.preprocess = _transform(224)
         self.mlp = MLP(768)
```

### Comparing `image-reward-0.92/PKG-INFO` & `image-reward-0.93/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-reward
-Version: 0.92
+Version: 0.93
 Summary: ImageReward
 Author: xujz18
 Author-email: <xjz22@mails.tsinghua.edu.cn>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `image-reward-0.92/README.md` & `image-reward-0.93/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -44,32 +44,40 @@
 rewards = [[0.5811622738838196], [0.2745276093482971], [-1.4131819009780884], [-2.029569625854492]]
           1.webp: 0.58
           2.webp: 0.27
           3.webp: -1.41
           4.webp: -2.03
 ```
 
+## Test (One Step)
+
+```bash
+$ bash ./scripts/test.sh
+```
+
 ## Test
 
 ### Setup for baselines
 
 #### Environment
 
 ```bash
 $ pip install git+https://github.com/openai/CLIP.git
 ```
 
 #### Checkpoint
 
-Models | File Paths | Download Links
---- | :---: | :---: 
-ImageReward | checkpoint/ | <a href="https://huggingface.co/THUDM/ImageReward/blob/main/ImageReward.pt">Download</a>
-CLIP Score | checkpoint/clip/ | <a href="https://openaipublic.azureedge.net/clip/models/b8cca3fd41ae0c99ba7e8951adf17d267cdb84cd88be6f7c2e0eca1737a03836/ViT-L-14.pt">Download</a>
-BLIP Score | checkpoint/blip/ | <a href="https://storage.googleapis.com/sfr-vision-language-research/BLIP/models/model_large.pth">Download</a>
-Aesthetic | checkpoint/aesthetic/ | <a href="https://github.com/christophschuhmann/improved-aesthetic-predictor/raw/main/sac%2Blogos%2Bava1-l14-linearMSE.pth">Download</a>
+* Download checkpoints to checkpoint/
+
+Models | Download Links
+--- | :---: 
+ImageReward | <a href="https://huggingface.co/THUDM/ImageReward/blob/main/ImageReward.pt">Download</a>
+CLIP Score | <a href="https://openaipublic.azureedge.net/clip/models/b8cca3fd41ae0c99ba7e8951adf17d267cdb84cd88be6f7c2e0eca1737a03836/ViT-L-14.pt">Download</a>
+BLIP Score | <a href="https://storage.googleapis.com/sfr-vision-language-research/BLIP/models/model_large.pth">Download</a>
+Aesthetic | <a href="https://github.com/christophschuhmann/improved-aesthetic-predictor/raw/main/sac%2Blogos%2Bava1-l14-linearMSE.pth">Download</a>
 
 #### Data
 
 Data | File Paths | Download Links
 --- | :---: | :---: 
 test_images | data/ | <a href="https://huggingface.co/THUDM/ImageReward/blob/main/test_images.zip">Download</a>
```

### Comparing `image-reward-0.92/image_reward.egg-info/PKG-INFO` & `image-reward-0.93/image_reward.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-reward
-Version: 0.92
+Version: 0.93
 Summary: ImageReward
 Author: xujz18
 Author-email: <xjz22@mails.tsinghua.edu.cn>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `image-reward-0.92/setup.py` & `image-reward-0.93/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (Path(__file__).parent / "README-pypi.md").read_text()
 DESCRIPTION = 'ImageReward'
 
 # 配置
 setup(
         name="image-reward", 
         py_modules = ["ImageReward"],
-        version="0.92",
+        version="0.93",
         author="xujz18",
         author_email="<xjz22@mails.tsinghua.edu.cn>",
         description=DESCRIPTION,
         long_description=long_description,
         long_description_content_type='text/markdown',
         packages=find_packages(exclude=["tests*"]),
         install_requires=[
```

