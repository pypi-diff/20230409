# Comparing `tmp/noisegrad-0.0.1.tar.gz` & `tmp/noisegrad-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noisegrad-0.0.1.tar", last modified: Sun Apr  9 18:51:40 2023, max compression
+gzip compressed data, was "noisegrad-0.0.2.tar", last modified: Sun Apr  9 19:08:35 2023, max compression
```

## Comparing `noisegrad-0.0.1.tar` & `noisegrad-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1146 2023-04-09 18:51:31.214189 noisegrad-0.0.1/LICENSE.md
--rw-r--r--   0        0        0     1440 2023-04-09 18:51:31.214189 noisegrad-0.0.1/README.md
--rw-r--r--   0        0        0      124 2023-04-09 18:51:31.222189 noisegrad-0.0.1/noisegrad/__init__.py
--rw-r--r--   0        0        0     2943 2023-04-09 18:51:31.222189 noisegrad-0.0.1/noisegrad/explainers.py
--rw-r--r--   0        0        0     6557 2023-04-09 18:51:31.222189 noisegrad-0.0.1/noisegrad/noisegrad.py
--rw-r--r--   0        0        0       64 2023-04-09 18:51:31.222189 noisegrad-0.0.1/noisegrad/py.typed
--rw-r--r--   0        0        0     2575 2023-04-09 18:51:31.222189 noisegrad-0.0.1/noisegrad/utils.py
--rw-r--r--   0        0        0     6691 2023-04-09 18:51:31.222189 noisegrad-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3175 1970-01-01 00:00:00.000000 noisegrad-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1146 2023-04-09 19:08:19.538401 noisegrad-0.0.2/LICENSE.md
+-rw-r--r--   0        0        0     1985 2023-04-09 19:08:19.538401 noisegrad-0.0.2/README.md
+-rw-r--r--   0        0        0      124 2023-04-09 19:08:19.546401 noisegrad-0.0.2/noisegrad/__init__.py
+-rw-r--r--   0        0        0     2943 2023-04-09 19:08:19.546401 noisegrad-0.0.2/noisegrad/explainers.py
+-rw-r--r--   0        0        0     6645 2023-04-09 19:08:19.546401 noisegrad-0.0.2/noisegrad/noisegrad.py
+-rw-r--r--   0        0        0       64 2023-04-09 19:08:19.546401 noisegrad-0.0.2/noisegrad/py.typed
+-rw-r--r--   0        0        0     2575 2023-04-09 19:08:19.546401 noisegrad-0.0.2/noisegrad/utils.py
+-rw-r--r--   0        0        0     6357 2023-04-09 19:08:19.546401 noisegrad-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3720 1970-01-01 00:00:00.000000 noisegrad-0.0.2/PKG-INFO
```

### Comparing `noisegrad-0.0.1/LICENSE.md` & `noisegrad-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `noisegrad-0.0.1/noisegrad/explainers.py` & `noisegrad-0.0.2/noisegrad/explainers.py`

 * *Files identical despite different names*

### Comparing `noisegrad-0.0.1/noisegrad/noisegrad.py` & `noisegrad-0.0.2/noisegrad/noisegrad.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from __future__ import annotations
 
-from typing import Callable, Literal, NamedTuple
+from typing import Callable, Literal, NamedTuple, Protocol
 
 import torch
 import torch.nn as nn
 from tqdm.auto import tqdm
 
 NoiseType = Literal["multiplicative", "additive"]
-ExplanationFn = Callable[[nn.Module, torch.Tensor, torch.Tensor], torch.Tensor]
+
+
+class ExplanationFn(Protocol):
+
+    def __call__(self, mode: nn.Module, x_batch: torch.Tensor, y_batch: torch.Tensor, *args, **kwargs) -> torch.Tensor: ...
 
 
 class NoiseGradConfig(NamedTuple):
     """
     mean:
         Mean of normal distribution, from which noise added to weights is sampled.
     std:
```

### Comparing `noisegrad-0.0.1/noisegrad/utils.py` & `noisegrad-0.0.2/noisegrad/utils.py`

 * *Files identical despite different names*

### Comparing `noisegrad-0.0.1/pyproject.toml` & `noisegrad-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "noisegrad"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.1"  # Required
+version = "0.0.2"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "A explanation enhancement method."  # Optional
 
 # This is an optional longer description of your project that represents
@@ -148,24 +148,14 @@
 #"Source" = "https://github.com/pypa/sampleproject/"
 
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
 #[project.scripts]  # Optional
 #sample = "sample:main"
 
-# This is configuration specific to the `setuptools` build backend.
-# If you are using a different build backend, you will need to change this.
-[tool.setuptools]
-# If there are data files included in your packages that need to be
-# installed, specify them here.
-#package-data = {"sample" = ["*.dat"]}
-packages = [
-    "noisegrad",
-]
-
 [build-system]
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
 requires = ["flit-core >= 3.4"]
 build-backend = "flit_core.buildapi"
```

### Comparing `noisegrad-0.0.1/PKG-INFO` & `noisegrad-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisegrad
-Version: 0.0.1
+Version: 0.0.2
 Summary: A explanation enhancement method.
 Keywords: explainable ai,xai,machine learning,deep learning
 Author-email: Kirill Bykov <kirill.bykov@campus.tu-berlin.de>, Anna Hedström <anna.hedstroem@tu-berlin.de>, Shinichi Nakajima <nakajima@tu-berlin.de>, "Marina M.-C. Höhne" <marina.hoehne@tu-berlin.de>, Artem Sereda <artem.sereda@campus.tu-berlin.de>
 Maintainer-email: Kirill Bykov <kirill.bykov@campus.tu-berlin.de>, Anna Hedström <anna.hedstroem@tu-berlin.de>, Artem Sereda <artem.sereda@campus.tu-berlin.de>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
@@ -38,38 +38,54 @@
   <i>Pytorch implementation</i>
 </p>
 
 --------------
 
 Pytorch implementation for **"NoiseGrad: enhancing explanations by introducing stochasticity to model weights"**. The paper introduces two novel methods `NoiseGrad` and `FusionGrad` which both improves attribution-based explanations by introducing stochasticity to the model parameters. See arXiv preprint: https://arxiv.org/abs/2106.10185.
 
-<p align="center">
-  <img src="samples/resulting_explanation.png" alt="Visualization of baseline, NoiseGrad and NoiseGrad++ explanations using (Integrated Gradient) as XAI method." width="512"/>
-</p>
+![](https://raw.githubusercontent.com/understandable-machine-intelligence-lab/NoiseGrad/master/samples/resulting_explanation.png)
 
 ## Cite this paper
 
 To cite this paper use following Bibtex annotation:
 
 	@misc{bykov2021noisegrad,
 	      title={NoiseGrad: enhancing explanations by introducing stochasticity to model weights},
 	      author={Kirill Bykov and Anna Hedström and Shinichi Nakajima and Marina M. -C. Höhne},
 	      year={2021},
 	      eprint={2106.10185},
 	      archivePrefix={arXiv},
 	      primaryClass={cs.LG}}
 
-## Requirements
+## Installation
 
 To install requirements:
 
 ```setup
-pip install -r requirements.txt
+pip install noisegrad
 ```
 
 All experiments were conducted with Python 3.6.9.
 
-## Code structure
+## Minimal Example, for more detailed ones, please refer to `examples/`
+```python
+from noisegrad import NoiseGrad, NoiseGradConfig, NoiseGradPlusPlus, NoiseGradPlusPlusConfig
+from noisegrad.explainers import intgrad_explainer
+
+# Initialize NoiseGrad: enhance any explanation function!
+noisegrad = NoiseGrad(NoiseGradConfig(n=5))
+
+# Initialize NoiseGrad++: enhance any explanation function!
+noisegradp = NoiseGradPlusPlus(NoiseGradPlusPlusConfig(n=5, m=5))
+
+# Get baseline explanation.
+expl_base = intgrad_explainer(model, x, y)
+
+# Get NoiseGrad explanation.
+expl_ng = noisegrad.enhance_explanation(model, x, y, intgrad_explainer)
+
+# Get NoiseGrad++ explanation.
+expl_ngp = noisegradp.enhance_explanation(model, x, y, intgrad_explainer)
+```
 
-The source code can be found in the `src/` folder and an example notebook in `examples/` folder.
```

