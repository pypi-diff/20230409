# Comparing `tmp/sparktorch-0.1.2.tar.gz` & `tmp/sparktorch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sparktorch-0.1.2.tar", last modified: Sat Dec  7 16:20:29 2019, max compression
+gzip compressed data, was "sparktorch-0.2.0.tar", last modified: Sun Apr  9 16:44:33 2023, max compression
```

## Comparing `sparktorch-0.1.2.tar` & `sparktorch-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 derekmiller   (501) staff       (20)        0 2019-12-07 16:20:29.000000 sparktorch-0.1.2/
--rw-r--r--   0 derekmiller   (501) staff       (20)    11753 2019-12-07 16:20:29.000000 sparktorch-0.1.2/PKG-INFO
--rw-r--r--   0 derekmiller   (501) staff       (20)     9365 2019-12-04 01:40:23.000000 sparktorch-0.1.2/README.md
-drwxr-xr-x   0 derekmiller   (501) staff       (20)        0 2019-12-07 16:20:29.000000 sparktorch-0.1.2/sparktorch/
--rw-r--r--   0 derekmiller   (501) staff       (20)     4766 2019-11-30 14:39:19.000000 sparktorch-0.1.2/sparktorch/pipeline_util.py
--rw-r--r--   0 derekmiller   (501) staff       (20)     4902 2019-12-03 02:30:43.000000 sparktorch-0.1.2/sparktorch/server.py
--rw-r--r--   0 derekmiller   (501) staff       (20)     2087 2019-11-29 18:27:07.000000 sparktorch-0.1.2/sparktorch/rw_lock.py
--rw-r--r--   0 derekmiller   (501) staff       (20)     7021 2019-12-03 03:40:23.000000 sparktorch-0.1.2/sparktorch/util.py
-drwxr-xr-x   0 derekmiller   (501) staff       (20)        0 2019-12-07 16:20:29.000000 sparktorch-0.1.2/sparktorch/tests/
--rw-r--r--   0 derekmiller   (501) staff       (20)     1381 2019-12-03 02:38:04.000000 sparktorch-0.1.2/sparktorch/tests/simple_net.py
--rw-r--r--   0 derekmiller   (501) staff       (20)        0 2019-12-01 20:40:27.000000 sparktorch-0.1.2/sparktorch/tests/__init__.py
--rw-r--r--   0 derekmiller   (501) staff       (20)     6445 2019-12-07 14:54:03.000000 sparktorch-0.1.2/sparktorch/tests/test_sparktorch.py
--rw-r--r--   0 derekmiller   (501) staff       (20)      244 2019-12-04 01:34:31.000000 sparktorch-0.1.2/sparktorch/__init__.py
--rw-r--r--   0 derekmiller   (501) staff       (20)     9645 2019-12-07 14:44:32.000000 sparktorch-0.1.2/sparktorch/distributed.py
--rw-r--r--   0 derekmiller   (501) staff       (20)    11754 2019-12-04 23:54:06.000000 sparktorch-0.1.2/sparktorch/torch_distributed.py
--rw-r--r--   0 derekmiller   (501) staff       (20)     6046 2019-12-03 02:30:43.000000 sparktorch-0.1.2/sparktorch/hogwild.py
--rw-r--r--   0 derekmiller   (501) staff       (20)     2051 2019-12-04 01:47:34.000000 sparktorch-0.1.2/sparktorch/inference.py
--rw-r--r--   0 derekmiller   (501) staff       (20)     1725 2019-11-30 20:08:50.000000 sparktorch-0.1.2/sparktorch/early_stopper.py
--rw-r--r--   0 derekmiller   (501) staff       (20)      745 2019-12-07 16:20:21.000000 sparktorch-0.1.2/setup.py
-drwxr-xr-x   0 derekmiller   (501) staff       (20)        0 2019-12-07 16:20:29.000000 sparktorch-0.1.2/sparktorch.egg-info/
--rw-r--r--   0 derekmiller   (501) staff       (20)    11753 2019-12-07 16:20:29.000000 sparktorch-0.1.2/sparktorch.egg-info/PKG-INFO
--rw-r--r--   0 derekmiller   (501) staff       (20)        1 2019-12-07 16:20:29.000000 sparktorch-0.1.2/sparktorch.egg-info/not-zip-safe
--rw-r--r--   0 derekmiller   (501) staff       (20)      571 2019-12-07 16:20:29.000000 sparktorch-0.1.2/sparktorch.egg-info/SOURCES.txt
--rw-r--r--   0 derekmiller   (501) staff       (20)       26 2019-12-07 16:20:29.000000 sparktorch-0.1.2/sparktorch.egg-info/requires.txt
--rw-r--r--   0 derekmiller   (501) staff       (20)       11 2019-12-07 16:20:29.000000 sparktorch-0.1.2/sparktorch.egg-info/top_level.txt
--rw-r--r--   0 derekmiller   (501) staff       (20)        1 2019-12-07 16:20:29.000000 sparktorch-0.1.2/sparktorch.egg-info/dependency_links.txt
--rw-r--r--   0 derekmiller   (501) staff       (20)       79 2019-12-07 16:20:29.000000 sparktorch-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:44:33.431908 sparktorch-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-09 16:44:19.000000 sparktorch-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-04-09 16:44:33.431908 sparktorch-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-04-09 16:44:19.000000 sparktorch-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-09 16:44:33.431908 sparktorch-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-09 16:44:19.000000 sparktorch-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:44:33.427909 sparktorch-0.2.0/sparktorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-09 16:44:19.000000 sparktorch-0.2.0/sparktorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-04-09 16:44:19.000000 sparktorch-0.2.0/sparktorch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-09 16:44:19.000000 sparktorch-0.2.0/sparktorch/early_stopper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-09 16:44:19.000000 sparktorch-0.2.0/sparktorch/hogwild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-09 16:44:19.000000 sparktorch-0.2.0/sparktorch/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-09 16:44:19.000000 sparktorch-0.2.0/sparktorch/pipeline_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-09 16:44:19.000000 sparktorch-0.2.0/sparktorch/rw_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-09 16:44:19.000000 sparktorch-0.2.0/sparktorch/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:44:33.431908 sparktorch-0.2.0/sparktorch/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 16:44:19.000000 sparktorch-0.2.0/sparktorch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-09 16:44:19.000000 sparktorch-0.2.0/sparktorch/tests/simple_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-09 16:44:19.000000 sparktorch-0.2.0/sparktorch/tests/test_sparktorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-04-09 16:44:19.000000 sparktorch-0.2.0/sparktorch/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-09 16:44:19.000000 sparktorch-0.2.0/sparktorch/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:44:33.427909 sparktorch-0.2.0/sparktorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-04-09 16:44:33.000000 sparktorch-0.2.0/sparktorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-09 16:44:33.000000 sparktorch-0.2.0/sparktorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 16:44:33.000000 sparktorch-0.2.0/sparktorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 16:44:33.000000 sparktorch-0.2.0/sparktorch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-09 16:44:33.000000 sparktorch-0.2.0/sparktorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 16:44:33.000000 sparktorch-0.2.0/sparktorch.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sparktorch-0.1.2/PKG-INFO` & `sparktorch-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,256 +1,260 @@
 Metadata-Version: 2.1
 Name: sparktorch
-Version: 0.1.2
-Summary: Deep learning on Apache Spark with Pytorch
+Version: 0.2.0
+Summary: Distributed training of PyTorch networks on Apache Spark with ML Pipeline support
 Home-page: https://github.com/dmmiller612/sparktorch
+Download-URL: https://github.com/dmmiller612/sparktorch/archive/0.2.0.tar.gz
 Author: Derek Miller
 Author-email: dmmiller612@gmail.com
 License: MIT
-Download-URL: https://github.com/dmmiller612/sparktorch/archive/0.1.2.tar.gz
-Description: # SparkTorch
-        
-        [![Build Status](https://travis-ci.com/dmmiller612/sparktorch.svg?branch=master)](https://travis-ci.org/dmmiller612/sparktorch)
-        [![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](https://github.com/dmmiller612/sparktorch)
-        
-        This is an implementation of Pytorch on Apache Spark. The goal of this library is to provide a simple, understandable interface 
-        in distributing the training of your Pytorch model on Spark. With SparkTorch, you can easily integrate your deep 
-        learning model with a ML Spark Pipeline. Underneath the hood, SparkTorch offers two distributed training approaches 
-        through tree reductions and a parameter server. Through the api, the user can specify the style of training, whether 
-        that is distributed synchronous or hogwild.
-        
-        ## Why should I use this?
-        
-        Like SparkFlow, SparkTorch's main objective is to seamlessly work with Spark's ML Pipelines. This library provides three 
-        core components:
-        
-        * Data parallel distributed training for large datasets. SparkTorch offers distributed synchronous and asynchronous training methodologies. 
-        This is useful for training very large datasets that do not fit into a single machine.
-        * Full integration with Spark's ML library. This ensures that you can save and load pipelines with your trained model.
-        * Inference. With SparkTorch, you can load your existing trained model and run inference on billions of records 
-        in parallel. 
-        
-        On top of these features, SparkTorch can utilize barrier execution, ensuring that all executors run concurrently during 
-        training (This is required for synchronous training approaches). 
-        
-        ## Install
-        
-        Install SparkTorch via pip: `pip install sparktorch`
-        
-        SparkTorch requires Apache Spark >= 2.4.4, and has only been tested on PyTorch versions >= 1.3.0.
-        
-        ## Full Basic Example
-        
-        ```python
-        from sparktorch import serialize_torch_obj, SparkTorch
-        import torch
-        import torch.nn as nn
-        from pyspark.ml.feature import VectorAssembler
-        from pyspark.sql import SparkSession
-        from pyspark.ml.pipeline import Pipeline
-        
-        spark = SparkSession.builder.appName("examples").master('local[2]').getOrCreate()
-        df = spark.read.option("inferSchema", "true").csv('mnist_train.csv').coalesce(2)
-        
-        network = nn.Sequential(
-            nn.Linear(784, 256),
-            nn.ReLU(),
-            nn.Linear(256, 256),
-            nn.ReLU(),
-            nn.Linear(256, 10),
-            nn.Softmax(dim=1)
-        )
-        
-        # Build the pytorch object
-        torch_obj = serialize_torch_obj(
-            model=network,
-            criterion=nn.CrossEntropyLoss(),
-            optimizer=torch.optim.Adam,
-            lr=0.0001
-        )
-        
-        # Setup features
-        vector_assembler = VectorAssembler(inputCols=df.columns[1:785], outputCol='features')
-        
-        # Create a SparkTorch Model with torch distributed. Barrier execution is on by default for this mode.
-        spark_model = SparkTorch(
-            inputCol='features',
-            labelCol='_c0',
-            predictionCol='predictions',
-            torchObj=torch_obj,
-            iters=50,
-            verbose=1
-        )
-        
-        # Can be used in a pipeline and saved.
-        p = Pipeline(stages=[vector_assembler, spark_model]).fit(df)
-        p.save('simple_dnn')
-        ```
-        
-        ## Run the Examples
-        
-        You can run the examples through docker by issuing the following commands at the root of the repository:
-        ```bash
-        make docker-build
-        make docker-run-dnn
-        make docker-run-cnn
-        ```
-        
-        For the cnn example, you will need to give your docker container at least 8gb of memory.
-        
-        ## Documentation
-        
-        This is a small documentation section on how to SparkTorch. Please look at the examples library for more details.
-        
-        #### Creating a Torch Object
-        
-        To create a Torch object for training, you will need to utilize the `serialize_torch_obj` from SparkTorch. To do so, 
-        simply add your network, loss criterion, the optimizer class, and any options as a dictionary to supply to the optimizer 
-        (such as learning rate). A simple example of this is:
-        
-        ```python
-        from sparktorch import serialize_torch_obj
-        
-        torch_obj = serialize_torch_obj(
-            model=network,
-            criterion=nn.CrossEntropyLoss(),
-            optimizer=torch.optim.Adam,
-            lr=0.0001
-        )
-        ```
-        
-        When training neural networks on Spark, one issue that many face is OOM errors. To avoid this issue on the driver, you 
-        can create a torch object that is only initialized on the worker nodes. To create this object, you can set up the 
-        following:
-        
-        ```python
-        from sparktorch import serialize_torch_obj_lazy
-        
-        torch_obj = serialize_torch_obj_lazy(
-            model=Network,
-            criterion=nn.CrossEntropyLoss,
-            optimizer=torch.optim.Adam,
-            optimizer_params={'lr': 0.001},
-            model_parameters={'some_model_param': 5}
-        )
-        ``` 
-        
-        The Network in the above example must be a nn.module pytorch class. If you need parameters passed into the constructor, 
-        you can use the `model_parameters` parameter. The item will be passed in as **kwargs to the constructor. 
-        
-        NOTE: One thing to remember is that if your network is not a sequential, it will need to be saved in a separate file and
-        available in the python path. An example of this can be found in `simple_cnn.py`.
-        
-        #### Training Options
-        
-        There are two main training options with SparkTorch: `async` and `hogwild`. The async mode utilizes the torch distributed 
-        package, ensuring that the networks are in sync through each iteration. This is the most supported version. When using 
-        this option, you will need to be aware that barrier execution is enforced, meaning that the parallelism will need to match 
-        the partitions. 
-        
-        The Hogwild approach utilizes a Flask Service underneath the hood. When using Hogwild, it is strongly recommended that you use the 
-        `useBarrier` option to force barrier execution. Below are a list of parameters to SparkTorch and their meaning.
-        
-        ```
-        inputCol: Standard Spark InputCol that must be a Vector.
-        labelCol: Standard Spark Label column. Can be null.
-        torchObj: The TorchObj which is described in the `Creating a Torch Object` section.
-        iters: Number of iterations to run per partition.
-        predictionCol: The standard spark prediction column for the dataframe.
-        partitions: Ability to repartition during training.
-        acquireLock: Used in Hogwild only. Forces locking on the server.
-        verbose: Describes whether you want real time logging
-        partitionShuffles: Only used in Hogwild. Will reshuffle data after completing training.
-        port: Only used in hogwild. Server port.
-        useBarrier: Only used in hogwild. Describes whether you want barrier execution. (Async mode uses barrier by default)
-        useVectorOut: Boolean to describe if you want the model output to be a vector (Defaults to float).
-        earlyStopPatience: If greater than 0, it will enforce early stopping based on validation.
-        miniBatch: Minibatch size for training per iteration. (Randomly shuffled)
-        validationPct: Percentage to use for validation.
-        mode: which training mode to use. `synchronous` leverages torch distributed. `hogwild` currently uses the flask service.
-        device: Supply 'cpu' or 'cuda'
-        ```
-        
-        #### Saving and Loading Pipelines
-        
-        Since saving and loading custom ML Transformers in pure python has not been implemented in PySpark, an extension has been
-        added here to make that possible. In order to save a Pyspark Pipeline with Apache Spark, one will need to use the overwrite function:
-        
-        ```python
-        p = Pipeline(stages=[va, encoded, spark_model]).fit(df)
-        p.write().overwrite().save("location")
-        ```
-        
-        For loading, a Pipeline wrapper has been provided in the pipeline_utils file. An example is below:
-        
-        ```python
-        from sparktorch import PysparkPipelineWrapper
-        from pyspark.ml.pipeline import PipelineModel
-        
-        p = PysparkPipelineWrapper.unwrap(PipelineModel.load('location'))
-        ``` 
-        Then you can perform predictions, etc with:
-        
-        ```python
-        predictions = p.transform(df)
-        ```
-        
-        #### Getting the Pytorch model from the training session
-        
-        If you just want to get the Pytorch model after training, you can execute the following code:
-        
-        ```python
-        stm = SparkTorch(
-            inputCol='features',
-            labelCol='label',
-            predictionCol='predictions',
-            torchObj=network_with_params,
-            verbose=1,
-            iters=5
-        ).fit(data)
-        
-        py_model = stm.getPytorchModel()
-        ```
-        
-        
-        #### Using a pretrained Pytorch model for inference
-        
-        If you already have a trained Pytorch model, you can attach it your existing pipeline by directly creating a SparkTorchModel. 
-        This can be done by running the following:
-        
-        ```python
-        from sparktorch import create_spark_torch_model
-        
-        net = ... # Pretrained Network
-        
-        spark_torch_model = create_spark_torch_model(
-            net, 
-            inputCol='features',
-            predictionCol='predictions'
-        )
-        ```
-        
-        ## Running
-        
-        One big thing to remember is to add the `--executor cores 1` option to spark to ensure
-        each executor is only training one copy of the network. This will especially be needed for gpu training.
-        
-        ## Contributing
-        
-        Contributions are always welcome. This could be fixing a bug, changing documentation, or adding a new feature. To test 
-        new changes against existing tests, we have provided a Docker container which takes in an argument of the python version. 
-        This allows the user to check their work before pushing to Github, where travis-ci will run.
-        
-        For python 3.6
-        ```
-        docker build -t local-test --build-arg PYTHON_VERSION=3.6 .
-        docker run --rm local-test:latest bash -i -c "pytest"
-        ```
-        
-        ## Literature and Inspiration
-        
-        * Distributed training: http://seba1511.net/dist_blog/
-        * HOGWILD!: A Lock-Free Approach to Parallelizing Stochastic Gradient Descent: https://arxiv.org/pdf/1106.5730.pdf
-        * Scaling Distributed Machine Learning with the Parameter Server: https://www.cs.cmu.edu/~muli/file/parameter_server_osdi14.pdf
 Keywords: pytorch,spark,sparktorch,machine learning,deep learning
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# SparkTorch
+
+[![Build Status](https://travis-ci.com/dmmiller612/sparktorch.svg?branch=master)](https://travis-ci.org/dmmiller612/sparktorch)
+[![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](https://github.com/dmmiller612/sparktorch)
+<img src="https://img.shields.io/pypi/v/sparktorch.svg" />
+
+![SparkTorch](images/sparktorchi.png)
+
+This is an implementation of Pytorch on Apache Spark. The goal of this library is to provide a simple, understandable interface 
+in distributing the training of your Pytorch model on Spark. With SparkTorch, you can easily integrate your deep 
+learning model with a ML Spark Pipeline. Underneath the hood, SparkTorch offers two distributed training approaches 
+through tree reductions and a parameter server. Through the api, the user can specify the style of training, whether 
+that is distributed synchronous or hogwild.
+
+## Why should I use this?
+
+Like SparkFlow, SparkTorch's main objective is to seamlessly work with Spark's ML Pipelines. This library provides three 
+core components:
+
+* Data parallel distributed training for large datasets. SparkTorch offers distributed synchronous and asynchronous training methodologies. 
+This is useful for training very large datasets that do not fit into a single machine.
+* Full integration with Spark's ML library. This ensures that you can save and load pipelines with your trained model.
+* Inference. With SparkTorch, you can load your existing trained model and run inference on billions of records 
+in parallel. 
+
+On top of these features, SparkTorch can utilize barrier execution, ensuring that all executors run concurrently during 
+training (This is required for synchronous training approaches). 
+
+## Install
+
+Install SparkTorch via pip: `pip install sparktorch`
+
+SparkTorch requires Apache Spark >= 2.4.4, and has only been tested on PyTorch versions >= 1.3.0.
+
+## Full Basic Example
+
+```python
+from sparktorch import serialize_torch_obj, SparkTorch
+import torch
+import torch.nn as nn
+from pyspark.ml.feature import VectorAssembler
+from pyspark.sql import SparkSession
+from pyspark.ml.pipeline import Pipeline
+
+spark = SparkSession.builder.appName("examples").master('local[2]').getOrCreate()
+df = spark.read.option("inferSchema", "true").csv('mnist_train.csv').coalesce(2)
+
+network = nn.Sequential(
+    nn.Linear(784, 256),
+    nn.ReLU(),
+    nn.Linear(256, 256),
+    nn.ReLU(),
+    nn.Linear(256, 10),
+    nn.Softmax(dim=1)
+)
+
+# Build the pytorch object
+torch_obj = serialize_torch_obj(
+    model=network,
+    criterion=nn.CrossEntropyLoss(),
+    optimizer=torch.optim.Adam,
+    lr=0.0001
+)
+
+# Setup features
+vector_assembler = VectorAssembler(inputCols=df.columns[1:785], outputCol='features')
+
+# Create a SparkTorch Model with torch distributed. Barrier execution is on by default for this mode.
+spark_model = SparkTorch(
+    inputCol='features',
+    labelCol='_c0',
+    predictionCol='predictions',
+    torchObj=torch_obj,
+    iters=50,
+    verbose=1
+)
+
+# Can be used in a pipeline and saved.
+p = Pipeline(stages=[vector_assembler, spark_model]).fit(df)
+p.save('simple_dnn')
+```
+
+## Run the Examples
+
+You can run the examples through docker by issuing the following commands at the root of the repository:
+```bash
+make docker-build
+make docker-run-dnn
+make docker-run-cnn
+```
+
+For the cnn example, you will need to give your docker container at least 8gb of memory.
+
+## Documentation
+
+This is a small documentation section on how to SparkTorch. Please look at the examples library for more details.
+
+#### Creating a Torch Object
+
+To create a Torch object for training, you will need to utilize the `serialize_torch_obj` from SparkTorch. To do so, 
+simply add your network, loss criterion, the optimizer class, and any options as a dictionary to supply to the optimizer 
+(such as learning rate). A simple example of this is:
+
+```python
+from sparktorch import serialize_torch_obj
+
+torch_obj = serialize_torch_obj(
+    model=network,
+    criterion=nn.CrossEntropyLoss(),
+    optimizer=torch.optim.Adam,
+    lr=0.0001
+)
+```
+
+When training neural networks on Spark, one issue that many face is OOM errors. To avoid this issue on the driver, you 
+can create a torch object that is only initialized on the worker nodes. To create this object, you can set up the 
+following:
+
+```python
+from sparktorch import serialize_torch_obj_lazy
+
+torch_obj = serialize_torch_obj_lazy(
+    model=Network,
+    criterion=nn.CrossEntropyLoss,
+    optimizer=torch.optim.Adam,
+    optimizer_params={'lr': 0.001},
+    model_parameters={'some_model_param': 5}
+)
+``` 
+
+The Network in the above example must be a nn.module pytorch class. If you need parameters passed into the constructor, 
+you can use the `model_parameters` parameter. The item will be passed in as **kwargs to the constructor. 
+
+NOTE: One thing to remember is that if your network is not a sequential, it will need to be saved in a separate file and
+available in the python path. An example of this can be found in `simple_cnn.py`.
+
+#### Training Options
+
+There are two main training options with SparkTorch: `async` and `hogwild`. The async mode utilizes the torch distributed 
+package, ensuring that the networks are in sync through each iteration. This is the most supported version. When using 
+this option, you will need to be aware that barrier execution is enforced, meaning that the parallelism will need to match 
+the partitions. 
+
+The Hogwild approach utilizes a Flask Service underneath the hood. When using Hogwild, it is strongly recommended that you use the 
+`useBarrier` option to force barrier execution. Below are a list of parameters to SparkTorch and their meaning.
+
+```
+inputCol: Standard Spark InputCol that must be a Vector.
+labelCol: Standard Spark Label column. Can be null.
+torchObj: The TorchObj which is described in the `Creating a Torch Object` section.
+iters: Number of iterations to run per partition.
+predictionCol: The standard spark prediction column for the dataframe.
+partitions: Ability to repartition during training.
+acquireLock: Used in Hogwild only. Forces locking on the server.
+verbose: Describes whether you want real time logging
+partitionShuffles: Only used in Hogwild. Will reshuffle data after completing training.
+port: Only used in hogwild. Server port.
+useBarrier: Only used in hogwild. Describes whether you want barrier execution. (Async mode uses barrier by default)
+useVectorOut: Boolean to describe if you want the model output to be a vector (Defaults to float).
+earlyStopPatience: If greater than 0, it will enforce early stopping based on validation.
+miniBatch: Minibatch size for training per iteration. (Randomly shuffled)
+validationPct: Percentage to use for validation.
+mode: which training mode to use. `synchronous` leverages torch distributed. `hogwild` currently uses the flask service.
+device: Supply 'cpu' or 'cuda'
+```
+
+#### Saving and Loading Pipelines
+
+Since saving and loading custom ML Transformers in pure python has not been implemented in PySpark, an extension has been
+added here to make that possible. In order to save a Pyspark Pipeline with Apache Spark, one will need to use the overwrite function:
+
+```python
+p = Pipeline(stages=[va, encoded, spark_model]).fit(df)
+p.write().overwrite().save("location")
+```
+
+For loading, a Pipeline wrapper has been provided in the pipeline_utils file. An example is below:
+
+```python
+from sparktorch import PysparkPipelineWrapper
+from pyspark.ml.pipeline import PipelineModel
+
+p = PysparkPipelineWrapper.unwrap(PipelineModel.load('location'))
+``` 
+Then you can perform predictions, etc with:
+
+```python
+predictions = p.transform(df)
+```
+
+#### Getting the Pytorch model from the training session
+
+If you just want to get the Pytorch model after training, you can execute the following code:
+
+```python
+stm = SparkTorch(
+    inputCol='features',
+    labelCol='label',
+    predictionCol='predictions',
+    torchObj=network_with_params,
+    verbose=1,
+    iters=5
+).fit(data)
+
+py_model = stm.getPytorchModel()
+```
+
+
+#### Using a pretrained Pytorch model for inference
+
+If you already have a trained Pytorch model, you can attach it your existing pipeline by directly creating a SparkTorchModel. 
+This can be done by running the following:
+
+```python
+from sparktorch import create_spark_torch_model
+
+net = ... # Pretrained Network
+
+spark_torch_model = create_spark_torch_model(
+    net, 
+    inputCol='features',
+    predictionCol='predictions'
+)
+```
+
+## Running
+
+One big thing to remember is to add the `--executor cores 1` option to spark to ensure
+each executor is only training one copy of the network. This will especially be needed for gpu training.
+
+## Contributing
+
+Contributions are always welcome. This could be fixing a bug, changing documentation, or adding a new feature. To test 
+new changes against existing tests, we have provided a Docker container which takes in an argument of the python version. 
+This allows the user to check their work before pushing to Github, where travis-ci will run.
+
+For python 3.6
+```
+docker build -t local-test --build-arg PYTHON_VERSION=3.6 .
+docker run --rm local-test:latest bash -i -c "pytest"
+```
+
+## Literature and Inspiration
+
+* Distributed training: http://seba1511.net/dist_blog/
+* HOGWILD!: A Lock-Free Approach to Parallelizing Stochastic Gradient Descent: https://arxiv.org/pdf/1106.5730.pdf
+* Scaling Distributed Machine Learning with the Parameter Server: https://www.cs.cmu.edu/~muli/file/parameter_server_osdi14.pdf
```

### Comparing `sparktorch-0.1.2/README.md` & `sparktorch-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # SparkTorch
 
 [![Build Status](https://travis-ci.com/dmmiller612/sparktorch.svg?branch=master)](https://travis-ci.org/dmmiller612/sparktorch)
 [![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](https://github.com/dmmiller612/sparktorch)
+<img src="https://img.shields.io/pypi/v/sparktorch.svg" />
+
+![SparkTorch](images/sparktorchi.png)
 
 This is an implementation of Pytorch on Apache Spark. The goal of this library is to provide a simple, understandable interface 
 in distributing the training of your Pytorch model on Spark. With SparkTorch, you can easily integrate your deep 
 learning model with a ML Spark Pipeline. Underneath the hood, SparkTorch offers two distributed training approaches 
 through tree reductions and a parameter server. Through the api, the user can specify the style of training, whether 
 that is distributed synchronous or hogwild.
```

### Comparing `sparktorch-0.1.2/sparktorch/pipeline_util.py` & `sparktorch-0.2.0/sparktorch/pipeline_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import sys
+import zlib
+
 import dill
+from pyspark.context import SparkContext
 from pyspark.ml import Pipeline, PipelineModel
-from pyspark.ml.util import JavaMLReader, JavaMLWriter
 from pyspark.ml.feature import StopWordsRemover
+from pyspark.ml.util import JavaMLReader, JavaMLWriter
 from pyspark.ml.wrapper import JavaParams
-from pyspark.context import SparkContext
-import zlib
-import sys
 
 """
 based off below stackoverflow thread. Changes were made for performance.
 credit: https://stackoverflow.com/questions/41399399/serialize-a-custom-transformer-using-python-to-be-used-within-a-pyspark-ml-pipel
 """
```

### Comparing `sparktorch-0.1.2/sparktorch/server.py` & `sparktorch-0.2.0/sparktorch/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,25 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
+import logging
 import socket
-from torch.multiprocessing import Process
-from flask import Flask, request
+
 import dill
-from sparktorch.util import load_torch_model, TorchObj, load_base_torch
-from sparktorch.rw_lock import RWLock
+from flask import Flask, request
+from torch.multiprocessing import Process
+
 from sparktorch.early_stopper import EarlyStopping
+from sparktorch.rw_lock import RWLock
+from sparktorch.util import load_torch_model, TorchObj, load_base_torch
 
-import logging
 log = logging.getLogger('werkzeug')
 log.setLevel(logging.ERROR)
 
 
 class Server(object):
 
     def __init__(
```

### Comparing `sparktorch-0.1.2/sparktorch/rw_lock.py` & `sparktorch-0.2.0/sparktorch/rw_lock.py`

 * *Files identical despite different names*

### Comparing `sparktorch-0.1.2/sparktorch/util.py` & `sparktorch-0.2.0/sparktorch/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
+import codecs
+import collections
+import json
+from typing import Any, Dict, List, Type, Tuple
+
+import dill
 import numpy as np
 import torch
 import torch.nn as nn
 from torch.optim.optimizer import Optimizer
-import json
-import dill
-from typing import Any, Dict, List, Type, Tuple
-import collections
-import codecs
 
 TorchObj = collections.namedtuple(
     'TorchObj', ['model', 'criterion', 'optimizer', 'optimizer_params', 'is_lazy', 'model_parameters']
 )
 
 DataObj = collections.namedtuple('DataObj', ['x_train', 'y_train', 'x_val', 'y_val'])
```

### Comparing `sparktorch-0.1.2/sparktorch/tests/simple_net.py` & `sparktorch-0.2.0/sparktorch/tests/simple_net.py`

 * *Files identical despite different names*

### Comparing `sparktorch-0.1.2/sparktorch/tests/test_sparktorch.py` & `sparktorch-0.2.0/sparktorch/tests/test_sparktorch.py`

 * *Files identical despite different names*

### Comparing `sparktorch-0.1.2/sparktorch/distributed.py` & `sparktorch-0.2.0/sparktorch/distributed.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,129 +13,128 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
-from sparktorch.util import handle_features, load_torch_model, DataObj, load_base_torch
-from sparktorch.early_stopper import EarlyStopping
-from pyspark.rdd import RDD
-from typing import Dict, List, Union
+import os
+from typing import Dict, List, Union, Callable
 from uuid import uuid4
+
 import numpy as np
-from pyspark.rdd import PipelinedRDD
 import torch
-from torch.multiprocessing import Process
 import torch.distributed as dist
-from socket import gethostbyname, gethostname
+from pyspark.rdd import PipelinedRDD
+from pyspark.rdd import RDD
+from pyspark.taskcontext import BarrierTaskContext
 
-import os
+from sparktorch.early_stopper import EarlyStopping
+from sparktorch.util import handle_features, load_torch_model, DataObj, load_base_torch
 
 
-def retrieve_url() -> str:
-    return os.environ.get("SPARK_LOCAL_IP", gethostbyname(gethostname()))
+def get_available_port_port(address: str, context: BarrierTaskContext) -> int:
+    port = ""
+    if context.partitionId() == 0:
+        try:
+            import socket
 
+            sock = socket.socket()
+            sock.bind((address, 0))
+            port = sock.getsockname()[1]
+        except socket.error:
+            pass
+    available_port = context.allGather(str(port))[0]
+    if not available_port:
+        raise RuntimeError("Failed to find free port for distributed training.")
 
-def mapPartitionsWithIndex(rdd, f, preservesPartitioning=False):
-    """
-    Temporary function for barrier map partitions.
-    """
-    return PipelinedRDD(rdd, f, preservesPartitioning, isFromBarrier=True)
+    return int(available_port)
 
 
-def process_generic_model(params: List, iters: int, has_early_stop: bool = False):
+def mapPartitionsWithIndex(rdd: RDD, f: Callable, preservesPartitioning: bool = False) -> PipelinedRDD:
     """
-    Runs a mock training with zero grads. This is due to a bug where the connection gets reset with custom new groups.
-    :param params: The params of the model
-    :param iters: Iterations.
-    """
-    # Hopefully this function can go away in newer versions.
-    for i in range(iters):
-        for p in params:
-            z = torch.zeros(p)
-            dist.all_reduce(z, op=torch.distributed.ReduceOp.SUM)
+    Maps Partitions based off of the index.
 
-        if has_early_stop:
-            dist.all_reduce(torch.tensor(0.0), op=torch.distributed.ReduceOp.SUM)
-            zeros = torch.zeros(1)
-            dist.all_reduce(zeros, op=torch.distributed.ReduceOp.SUM)
-            if zeros.item() > 0:
-                break
+    :param rdd: A valid rdd.
+    :param f: Callable function with iterable.
+    :param preservesPartitioning: Whether or not to preserve partitioning
+
+    :return: A pipeline rdd.
+    """
+    return PipelinedRDD(rdd, f, preservesPartitioning, isFromBarrier=True)
 
 
 def handle_model(
     index: int,
     data: List[DataObj],
     torch_obj: Union[str, List],
-    master_url: str = '127.0.0.1',
     iters: int = 1000,
-    world_size: int = 2,
     early_stop_patience: int = -1,
     verbose: int = 1,
     mini_batch: int = -1,
     validation_pct: float = 0,
-    device: str = 'cpu'
+    device: str = 'cpu',
+    compile_mode: str = None,
 ) -> List[Dict]:
     """
     Runs the training of pytorch model, utilizing the distributed package.
 
     :param index: Partition index. Used for registering.
     :param data: The data from the partition
     :param torch_obj: The torch object string. Needs serialized
-    :param master_url: The master url for the service.
     :param iters: The iterations for training
-    :param world_size: The amount of partitions. Typically partitions + 1 for the driver
     :param verbose: whether to log the loss or not.
     :param mini_batch: Mini batch for training
     :param validation_pct: Validation percentage.
     :param device: The pytorch device to use for training. cpu/cuda
     :param early_stop_patience: Amount of patient for early stopping. -1 means don't use early stopping.
+    :param compile_mode: Torch compile option for 2.0 only.
 
     :return: A list of the model state dictionary.
     """
-
     # If a process has already been setup on the machine, kill it.
     if dist.is_initialized():
         dist.destroy_process_group()
 
+    context = BarrierTaskContext.get()
+
+    addrs = [e.address.split(":")[0] for e in context.getTaskInfos()]
+    world_size = len(addrs)
+
     # Set up the distributed server.
-    os.environ['MASTER_ADDR'] = master_url
-    os.environ['MASTER_PORT'] = '3333'
+    os.environ['MASTER_ADDR'] = str(addrs[0])
+    os.environ['MASTER_PORT'] = str(get_available_port_port(addrs[0], context))
+    os.environ['WORLD_SIZE'] = str(len(addrs))
+    os.environ['NODE_RANK'] = str(context.partitionId())
+    os.environ['RANK'] = str(context.partitionId())
 
-    dist.init_process_group('gloo', rank=index + 1, world_size=world_size)
+    dist.init_process_group('gloo', rank=index, world_size=world_size)
 
-    # Def Load model
-    if index == -1:
-        process_generic_model(torch_obj, iters, early_stop_patience > 0)
-        return []
-    else:
-        torch_obj = load_torch_model(torch_obj)
+    torch_obj = load_torch_model(torch_obj)
 
     # Loaded the model
     model = torch_obj.model.to(device)
+
+    if compile is not None:
+        torch.compile(compile_mode)
+
     model.train()
     criterion = torch_obj.criterion
     optimizer = torch_obj.optimizer
 
     # Set up early stopping
     es = EarlyStopping(patience=early_stop_patience)
     should_stop = torch.zeros(1)
     has_early_stop = early_stop_patience > 0
 
     partition_id = str(uuid4())
 
     # Process the data. Converts to x_train, y_train, x_val, y_val
     data_obj = handle_features(data, validation_pct)
 
-    # check if data is none. We will still need to register.
-    if data_obj is None or data_obj.x_train is None:
-        process_generic_model([list(p.shape) for p in model.parameters()], iters, early_stop_patience > 0)
-        return []
-
     # Passes all of the data
     x_train = data_obj.x_train.to(device)
     y_train = data_obj.y_train.to(device) if data_obj.y_train is not None else x_train
     x_val = data_obj.x_val.to(device) if data_obj.x_val is not None else None
     y_val = data_obj.y_val.to(device) if data_obj.y_val is not None else x_val
 
     for i in range(iters):
@@ -175,23 +174,23 @@
 
         # Calculate gradients
         loss.backward()
 
         # Distributed part of training.
         for param in model.parameters():
             dist.all_reduce(param.grad.data, op=torch.distributed.ReduceOp.SUM)
-            param.grad.data /= (world_size-1)
+            param.grad.data /= world_size
 
         # Processes the early stop work
         loss_distributed = None
         if has_early_stop:
             loss_to_use = val_loss if val_loss is not None else loss
 
             dist.all_reduce(loss_to_use, op=torch.distributed.ReduceOp.SUM)
-            loss_distributed = loss_to_use.item() / (world_size - 1)
+            loss_distributed = loss_to_use.item() / world_size
             stop = es.step(loss_distributed)
             if stop:
                 should_stop = should_stop + 1.0
 
             dist.all_reduce(should_stop, op=torch.distributed.ReduceOp.SUM)
             if should_stop.item() > 0:
                 break
@@ -210,68 +209,53 @@
     rdd: RDD,
     torch_obj: str,
     iters: int = 10,
     partition_shuffles: int = 1,
     verbose: int = 1,
     mini_batch: int = -1,
     validation_pct: float = 0.0,
-    world_size: int = 2,
     device: str = 'cpu',
-    early_stop_patience: int = -1
+    early_stop_patience: int = -1,
+    compile_mode: str = None,
 ) -> Dict:
     """
     Entry point to train the model in distributed fashion.
 
     :param rdd: The rdd of data to run on the model.
     :param torch_obj: The torch object as a string that includes the model and param shapes.
-    :param master_url: The main url for the driver.
     :param iters: Number of iterations for training.
-    :param partition_shuffles: Number of partition shuffles (Need to implement)
-    :param verbose: Verbosity of logs
+    :param partition_shuffles: Number of partition shuffles.
+    :param verbose: Verbosity of logs.
     :param mini_batch: Mini batch for each iteration of training.
-    :param validation_pct: How many items to validate
-    :param world_size: number of partitions.
-    :param device: pytorch device
+    :param validation_pct: How many items to validate.
+    :param device: pytorch device.
+    :param early_stop_patience: amount of patience for early stopping.
+    :param compile_mode: torch 2.0 compile mode.
 
     :return: The train dict.
     """
-    master_url = retrieve_url()
-
     torch_loaded, params = load_base_torch(torch_obj)
 
-    # Start the driver process.
-    p = Process(
-        target=handle_model,
-        args=(-1, None, params, master_url, iters, world_size, early_stop_patience)
-    )
-    p.start()
-
-    try:
-        state_dict = None
-        for i in range(partition_shuffles):
-
-            # Run model with barrier execution mode.
-            state_dict = mapPartitionsWithIndex(
-                rdd, lambda i, x: handle_model(
-                    i,
-                    x,
-                    torch_obj=torch_loaded,
-                    master_url=master_url,
-                    iters=iters,
-                    verbose=verbose,
-                    mini_batch=mini_batch,
-                    validation_pct=validation_pct,
-                    world_size=world_size,
-                    device=device,
-                    early_stop_patience=int(early_stop_patience+0)
-                )
-            ).collect()
-
-            if partition_shuffles - i > 1:
-                num_partitions = rdd.getNumPartitions()
-                rdd = rdd.repartition(num_partitions)
-
-        return state_dict[0]
-
-    finally:
-        p.terminate()
-        p.join()
+    state_dict = None
+    for i in range(partition_shuffles):
+
+        # Run model with barrier execution mode.
+        state_dict = mapPartitionsWithIndex(
+            rdd, lambda i, x: handle_model(
+                i,
+                x,
+                torch_obj=torch_loaded,
+                iters=iters,
+                verbose=verbose,
+                mini_batch=mini_batch,
+                validation_pct=validation_pct,
+                device=device,
+                early_stop_patience=int(early_stop_patience + 0),
+                compile_mode=compile_mode,
+            )
+        ).collect()
+
+        if partition_shuffles - i > 1:
+            num_partitions = rdd.getNumPartitions()
+            rdd = rdd.repartition(num_partitions)
+
+    return state_dict[0]
```

### Comparing `sparktorch-0.1.2/sparktorch/torch_distributed.py` & `sparktorch-0.2.0/sparktorch/torch_distributed.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,35 +13,36 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
-from sparktorch.pipeline_util import PysparkReaderWriter
-from sparktorch.util import DataObj, load_torch_model
-from sparktorch.server import Server
-from sparktorch.hogwild import train, get_main
-from sparktorch.distributed import train_distributed
-import numpy as np
-import torch
 import codecs
+import time
 
+import dill
+import numpy as np
+import torch
+from pyspark import SparkContext
+from pyspark import keyword_only
+from pyspark.ml import Model
+from pyspark.ml.base import Estimator
+from pyspark.ml.linalg import VectorUDT, Vectors
 from pyspark.ml.param import Param, Params, TypeConverters
 from pyspark.ml.param.shared import HasInputCol, HasPredictionCol, HasLabelCol
-from pyspark.ml.base import Estimator
-from pyspark.ml import Model
 from pyspark.ml.util import Identifiable, MLReadable, MLWritable
-from pyspark import keyword_only
-import time
 from pyspark.sql import functions as F
-import dill
 from pyspark.sql.types import DoubleType
-from pyspark.ml.linalg import VectorUDT, Vectors
-from pyspark import SparkContext
+
+from sparktorch.distributed import train_distributed
+from sparktorch.hogwild import train, get_main
+from sparktorch.pipeline_util import PysparkReaderWriter
+from sparktorch.server import Server
+from sparktorch.util import DataObj, load_torch_model
 
 
 def handle_data(input_col, label_col):
     def inner(dataset):
         res = [
             DataObj(
                 x_train=np.asarray(data[input_col].toArray()),
@@ -62,15 +63,15 @@
 
     @keyword_only
     def __init__(
         self,
         inputCol=None,
         predictionCol=None,
         modStr=None,
-        useVectorOut=None
+        useVectorOut=None,
     ):
         super().__init__()
         self._setDefault(
             inputCol='encoded',
             predictionCol='predicted',
             modStr='',
             useVectorOut=False
@@ -80,15 +81,15 @@
 
     @keyword_only
     def setParams(
         self,
         inputCol=None,
         predictionCol=None,
         modStr=None,
-        useVectorOut=None
+        useVectorOut=None,
     ):
         kwargs = self._input_kwargs
         return self._set(**kwargs)
 
     def getPytorchModel(self):
         mod_str = self.getOrDefault(self.modStr)
         return dill.loads(codecs.decode(mod_str.encode(), "base64"))
@@ -111,16 +112,18 @@
 
         def predict_float(data):
             features = data.toArray().reshape((1, len(data)))
             x_data = torch.from_numpy(features).float()
             model = model_broadcast.value
             model.eval()
             raw_prediction = model(x_data).detach().numpy().flatten()
+
             if len(raw_prediction) > 1:
                 return float(np.argmax(raw_prediction))
+
             return float(raw_prediction[0])
 
         if use_vector_out:
             udfGenerateCode = F.udf(predict_vec, VectorUDT())
         else:
             udfGenerateCode = F.udf(predict_float, DoubleType())
 
@@ -133,29 +136,29 @@
     HasPredictionCol,
     HasLabelCol,
     PysparkReaderWriter,
     MLReadable,
     MLWritable,
     Identifiable
 ):
-
     torchObj = Param(Params._dummy(), "torchObj", "The serialized torch object", typeConverter=TypeConverters.toString)
     mode = Param(Params._dummy(), "mode", "The training mode", typeConverter=TypeConverters.toString)
     device = Param(Params._dummy(), "device", "", typeConverter=TypeConverters.toString)
     iters = Param(Params._dummy(), "iters", "", typeConverter=TypeConverters.toInt)
     partitions = Param(Params._dummy(), "partitions", "", typeConverter=TypeConverters.toInt)
     verbose = Param(Params._dummy(), "verbose", "", typeConverter=TypeConverters.toInt)
     acquireLock = Param(Params._dummy(), "acquireLock", "", typeConverter=TypeConverters.toBoolean)
     partitionShuffles = Param(Params._dummy(), "partitionShuffles", "", typeConverter=TypeConverters.toInt)
     port = Param(Params._dummy(), "port", "", typeConverter=TypeConverters.toInt)
     useBarrier = Param(Params._dummy(), "useBarrier", "", typeConverter=TypeConverters.toBoolean)
     useVectorOut = Param(Params._dummy(), "useVectorOut", "", typeConverter=TypeConverters.toBoolean)
     earlyStopPatience = Param(Params._dummy(), "earlyStopPatience", "", typeConverter=TypeConverters.toInt)
     miniBatch = Param(Params._dummy(), "miniBatch", "", typeConverter=TypeConverters.toInt)
     validationPct = Param(Params._dummy(), "validationPct", "", typeConverter=TypeConverters.toFloat)
+    compileMode = Param(Params._dummy(), "compileMode", "", typeConverter=TypeConverters.toString)
 
     @keyword_only
     def __init__(
         self,
         inputCol=None,
         labelCol=None,
         torchObj=None,
@@ -168,15 +171,16 @@
         port=None,
         useBarrier=None,
         useVectorOut=None,
         earlyStopPatience=None,
         miniBatch=None,
         validationPct=None,
         mode=None,
-        device=None
+        device=None,
+        compileMode=None,
     ):
         super().__init__()
         self._setDefault(
             inputCol='features',
             labelCol=None,
             torchObj='',
             iters=10,
@@ -188,15 +192,16 @@
             port=3000,
             useBarrier=False,
             useVectorOut=False,
             earlyStopPatience=-1,
             miniBatch=-1,
             validationPct=0.0,
             mode='synchronous',
-            device='cpu'
+            device='cpu',
+            compileMode=None,
         )
         kwargs = self._input_kwargs
         self.setParams(**kwargs)
 
     @keyword_only
     def setParams(
         self,
@@ -212,15 +217,16 @@
         port=None,
         useBarrier=None,
         useVectorOut=None,
         earlyStopPatience=None,
         miniBatch=None,
         validationPct=None,
         mode=None,
-        device=None
+        device=None,
+        compileMode=None,
     ):
         kwargs = self._input_kwargs
         return self._set(**kwargs)
 
     def getTorchObj(self):
         return self.getOrDefault(self.torchObj)
 
@@ -259,14 +265,17 @@
 
     def getMode(self):
         return self.getOrDefault(self.mode)
 
     def getDevice(self):
         return self.getOrDefault(self.device)
 
+    def getCompileMode(self):
+        return self.getOrDefault(self.compileMode)
+
     def _fit(self, dataset):
         inp_col = self.getInputCol()
         label = self.getLabelCol()
         prediction = self.getPredictionCol()
 
         torch_obj = self.getTorchObj()
         iters = self.getIters()
@@ -278,40 +287,40 @@
         barrier = self.getBarrier()
         use_vector_out = self.getVectorOut()
         early_stop_patience = self.getEarlyStopPatience()
         mini_batch = self.getMiniBatch()
         validation_pct = self.getValidationPct()
         mode = self.getMode()
         device = self.getDevice()
+        compile_mode = self.getCompileMode()
 
         rdd = dataset.rdd.mapPartitions(handle_data(inp_col, label))
 
         if partitions > 0:
             rdd = rdd.repartition(partitions)
 
         partitions = partitions if partitions > 0 else rdd.getNumPartitions()
 
-        master_url = SparkContext._active_spark_context.getConf().get("spark.driver.host").__str__()
-
         if mode == 'synchronous':
 
             state_dict = train_distributed(
                 rdd=rdd,
                 torch_obj=torch_obj,
                 iters=iters,
                 partition_shuffles=1,
                 verbose=verbose,
                 mini_batch=mini_batch,
                 validation_pct=validation_pct,
-                world_size=partitions+1,
                 device=device,
-                early_stop_patience=early_stop_patience
+                early_stop_patience=early_stop_patience,
+                compile_mode=compile_mode,
             )
 
         elif mode == 'hogwild':
+            master_url = SparkContext._active_spark_context.getConf().get("spark.driver.host").__str__()
 
             if barrier:
                 rdd = rdd.barrier()
 
             server = Server(
                 torch_obj=torch_obj,
                 master_url=master_url + ":" + str(port),
```

### Comparing `sparktorch-0.1.2/sparktorch/hogwild.py` & `sparktorch-0.2.0/sparktorch/hogwild.py`

 * *Files identical despite different names*

### Comparing `sparktorch-0.1.2/sparktorch/inference.py` & `sparktorch-0.2.0/sparktorch/inference.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from sparktorch.torch_distributed import SparkTorchModel
-import torch.nn as nn
 import codecs
+
 import dill
+import torch.nn as nn
 from pyspark.ml.pipeline import PipelineModel
 
+from sparktorch.torch_distributed import SparkTorchModel
+
 
 def convert_to_serialized_torch(network: nn.Module) -> str:
     """
     Converts an existing torch network to a serialized string.
 
     :param network: a nn.Module that you want to serialize
     :return: Returns the serialized torch model.
@@ -26,15 +28,14 @@
 
     :param network: an already trained network
     :param inputCol: The spark dataframe input column
     :param predictionCol: The spark dataframe prediction columns
     :param useVectorOut: Determines whether the output should return a spark vector
     :return: Returns a SparkTorchModel
     """
-
     return SparkTorchModel(
         inputCol=inputCol,
         predictionCol=predictionCol,
         modStr=convert_to_serialized_torch(network),
         useVectorOut=useVectorOut
     )
 
@@ -52,10 +53,9 @@
     :param network: Pytorch Network
     :param pipeline_model: An existing spark pipeline model (This is a fitted pipeline)
     :param inputCol: The input column to the dataframe for the pytorch network
     :param predictionCol: The prediction column.
     :param useVectorOut: option to use a vector output.
     :return: a spark PipelineModel
     """
-
     spark_model = create_spark_torch_model(network, inputCol, predictionCol, useVectorOut)
     return PipelineModel(stages=[pipeline_model, spark_model])
```

### Comparing `sparktorch-0.1.2/sparktorch/early_stopper.py` & `sparktorch-0.2.0/sparktorch/early_stopper.py`

 * *Files identical despite different names*

### Comparing `sparktorch-0.1.2/setup.py` & `sparktorch-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 from setuptools import find_packages
 
 setup(name='sparktorch',
-      version='0.1.2',
-      description='Deep learning on Apache Spark with Pytorch',
-      keywords = ['pytorch', 'spark', 'sparktorch', 'machine learning', 'deep learning'],
+      version='0.2.0',
+      description='Distributed training of PyTorch networks on Apache Spark with ML Pipeline support',
+      keywords=['pytorch', 'spark', 'sparktorch', 'machine learning', 'deep learning'],
       url='https://github.com/dmmiller612/sparktorch',
-      download_url='https://github.com/dmmiller612/sparktorch/archive/0.1.2.tar.gz',
+      download_url='https://github.com/dmmiller612/sparktorch/archive/0.2.0.tar.gz',
       author='Derek Miller',
       author_email='dmmiller612@gmail.com',
       long_description=open("README.md", "r", encoding='utf-8').read(),
       long_description_content_type="text/markdown",
       install_requires=['torch', 'flask', 'requests', 'dill'],
       license='MIT',
       packages=find_packages(),
```

### Comparing `sparktorch-0.1.2/sparktorch.egg-info/PKG-INFO` & `sparktorch-0.2.0/sparktorch.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,256 +1,260 @@
 Metadata-Version: 2.1
 Name: sparktorch
-Version: 0.1.2
-Summary: Deep learning on Apache Spark with Pytorch
+Version: 0.2.0
+Summary: Distributed training of PyTorch networks on Apache Spark with ML Pipeline support
 Home-page: https://github.com/dmmiller612/sparktorch
+Download-URL: https://github.com/dmmiller612/sparktorch/archive/0.2.0.tar.gz
 Author: Derek Miller
 Author-email: dmmiller612@gmail.com
 License: MIT
-Download-URL: https://github.com/dmmiller612/sparktorch/archive/0.1.2.tar.gz
-Description: # SparkTorch
-        
-        [![Build Status](https://travis-ci.com/dmmiller612/sparktorch.svg?branch=master)](https://travis-ci.org/dmmiller612/sparktorch)
-        [![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](https://github.com/dmmiller612/sparktorch)
-        
-        This is an implementation of Pytorch on Apache Spark. The goal of this library is to provide a simple, understandable interface 
-        in distributing the training of your Pytorch model on Spark. With SparkTorch, you can easily integrate your deep 
-        learning model with a ML Spark Pipeline. Underneath the hood, SparkTorch offers two distributed training approaches 
-        through tree reductions and a parameter server. Through the api, the user can specify the style of training, whether 
-        that is distributed synchronous or hogwild.
-        
-        ## Why should I use this?
-        
-        Like SparkFlow, SparkTorch's main objective is to seamlessly work with Spark's ML Pipelines. This library provides three 
-        core components:
-        
-        * Data parallel distributed training for large datasets. SparkTorch offers distributed synchronous and asynchronous training methodologies. 
-        This is useful for training very large datasets that do not fit into a single machine.
-        * Full integration with Spark's ML library. This ensures that you can save and load pipelines with your trained model.
-        * Inference. With SparkTorch, you can load your existing trained model and run inference on billions of records 
-        in parallel. 
-        
-        On top of these features, SparkTorch can utilize barrier execution, ensuring that all executors run concurrently during 
-        training (This is required for synchronous training approaches). 
-        
-        ## Install
-        
-        Install SparkTorch via pip: `pip install sparktorch`
-        
-        SparkTorch requires Apache Spark >= 2.4.4, and has only been tested on PyTorch versions >= 1.3.0.
-        
-        ## Full Basic Example
-        
-        ```python
-        from sparktorch import serialize_torch_obj, SparkTorch
-        import torch
-        import torch.nn as nn
-        from pyspark.ml.feature import VectorAssembler
-        from pyspark.sql import SparkSession
-        from pyspark.ml.pipeline import Pipeline
-        
-        spark = SparkSession.builder.appName("examples").master('local[2]').getOrCreate()
-        df = spark.read.option("inferSchema", "true").csv('mnist_train.csv').coalesce(2)
-        
-        network = nn.Sequential(
-            nn.Linear(784, 256),
-            nn.ReLU(),
-            nn.Linear(256, 256),
-            nn.ReLU(),
-            nn.Linear(256, 10),
-            nn.Softmax(dim=1)
-        )
-        
-        # Build the pytorch object
-        torch_obj = serialize_torch_obj(
-            model=network,
-            criterion=nn.CrossEntropyLoss(),
-            optimizer=torch.optim.Adam,
-            lr=0.0001
-        )
-        
-        # Setup features
-        vector_assembler = VectorAssembler(inputCols=df.columns[1:785], outputCol='features')
-        
-        # Create a SparkTorch Model with torch distributed. Barrier execution is on by default for this mode.
-        spark_model = SparkTorch(
-            inputCol='features',
-            labelCol='_c0',
-            predictionCol='predictions',
-            torchObj=torch_obj,
-            iters=50,
-            verbose=1
-        )
-        
-        # Can be used in a pipeline and saved.
-        p = Pipeline(stages=[vector_assembler, spark_model]).fit(df)
-        p.save('simple_dnn')
-        ```
-        
-        ## Run the Examples
-        
-        You can run the examples through docker by issuing the following commands at the root of the repository:
-        ```bash
-        make docker-build
-        make docker-run-dnn
-        make docker-run-cnn
-        ```
-        
-        For the cnn example, you will need to give your docker container at least 8gb of memory.
-        
-        ## Documentation
-        
-        This is a small documentation section on how to SparkTorch. Please look at the examples library for more details.
-        
-        #### Creating a Torch Object
-        
-        To create a Torch object for training, you will need to utilize the `serialize_torch_obj` from SparkTorch. To do so, 
-        simply add your network, loss criterion, the optimizer class, and any options as a dictionary to supply to the optimizer 
-        (such as learning rate). A simple example of this is:
-        
-        ```python
-        from sparktorch import serialize_torch_obj
-        
-        torch_obj = serialize_torch_obj(
-            model=network,
-            criterion=nn.CrossEntropyLoss(),
-            optimizer=torch.optim.Adam,
-            lr=0.0001
-        )
-        ```
-        
-        When training neural networks on Spark, one issue that many face is OOM errors. To avoid this issue on the driver, you 
-        can create a torch object that is only initialized on the worker nodes. To create this object, you can set up the 
-        following:
-        
-        ```python
-        from sparktorch import serialize_torch_obj_lazy
-        
-        torch_obj = serialize_torch_obj_lazy(
-            model=Network,
-            criterion=nn.CrossEntropyLoss,
-            optimizer=torch.optim.Adam,
-            optimizer_params={'lr': 0.001},
-            model_parameters={'some_model_param': 5}
-        )
-        ``` 
-        
-        The Network in the above example must be a nn.module pytorch class. If you need parameters passed into the constructor, 
-        you can use the `model_parameters` parameter. The item will be passed in as **kwargs to the constructor. 
-        
-        NOTE: One thing to remember is that if your network is not a sequential, it will need to be saved in a separate file and
-        available in the python path. An example of this can be found in `simple_cnn.py`.
-        
-        #### Training Options
-        
-        There are two main training options with SparkTorch: `async` and `hogwild`. The async mode utilizes the torch distributed 
-        package, ensuring that the networks are in sync through each iteration. This is the most supported version. When using 
-        this option, you will need to be aware that barrier execution is enforced, meaning that the parallelism will need to match 
-        the partitions. 
-        
-        The Hogwild approach utilizes a Flask Service underneath the hood. When using Hogwild, it is strongly recommended that you use the 
-        `useBarrier` option to force barrier execution. Below are a list of parameters to SparkTorch and their meaning.
-        
-        ```
-        inputCol: Standard Spark InputCol that must be a Vector.
-        labelCol: Standard Spark Label column. Can be null.
-        torchObj: The TorchObj which is described in the `Creating a Torch Object` section.
-        iters: Number of iterations to run per partition.
-        predictionCol: The standard spark prediction column for the dataframe.
-        partitions: Ability to repartition during training.
-        acquireLock: Used in Hogwild only. Forces locking on the server.
-        verbose: Describes whether you want real time logging
-        partitionShuffles: Only used in Hogwild. Will reshuffle data after completing training.
-        port: Only used in hogwild. Server port.
-        useBarrier: Only used in hogwild. Describes whether you want barrier execution. (Async mode uses barrier by default)
-        useVectorOut: Boolean to describe if you want the model output to be a vector (Defaults to float).
-        earlyStopPatience: If greater than 0, it will enforce early stopping based on validation.
-        miniBatch: Minibatch size for training per iteration. (Randomly shuffled)
-        validationPct: Percentage to use for validation.
-        mode: which training mode to use. `synchronous` leverages torch distributed. `hogwild` currently uses the flask service.
-        device: Supply 'cpu' or 'cuda'
-        ```
-        
-        #### Saving and Loading Pipelines
-        
-        Since saving and loading custom ML Transformers in pure python has not been implemented in PySpark, an extension has been
-        added here to make that possible. In order to save a Pyspark Pipeline with Apache Spark, one will need to use the overwrite function:
-        
-        ```python
-        p = Pipeline(stages=[va, encoded, spark_model]).fit(df)
-        p.write().overwrite().save("location")
-        ```
-        
-        For loading, a Pipeline wrapper has been provided in the pipeline_utils file. An example is below:
-        
-        ```python
-        from sparktorch import PysparkPipelineWrapper
-        from pyspark.ml.pipeline import PipelineModel
-        
-        p = PysparkPipelineWrapper.unwrap(PipelineModel.load('location'))
-        ``` 
-        Then you can perform predictions, etc with:
-        
-        ```python
-        predictions = p.transform(df)
-        ```
-        
-        #### Getting the Pytorch model from the training session
-        
-        If you just want to get the Pytorch model after training, you can execute the following code:
-        
-        ```python
-        stm = SparkTorch(
-            inputCol='features',
-            labelCol='label',
-            predictionCol='predictions',
-            torchObj=network_with_params,
-            verbose=1,
-            iters=5
-        ).fit(data)
-        
-        py_model = stm.getPytorchModel()
-        ```
-        
-        
-        #### Using a pretrained Pytorch model for inference
-        
-        If you already have a trained Pytorch model, you can attach it your existing pipeline by directly creating a SparkTorchModel. 
-        This can be done by running the following:
-        
-        ```python
-        from sparktorch import create_spark_torch_model
-        
-        net = ... # Pretrained Network
-        
-        spark_torch_model = create_spark_torch_model(
-            net, 
-            inputCol='features',
-            predictionCol='predictions'
-        )
-        ```
-        
-        ## Running
-        
-        One big thing to remember is to add the `--executor cores 1` option to spark to ensure
-        each executor is only training one copy of the network. This will especially be needed for gpu training.
-        
-        ## Contributing
-        
-        Contributions are always welcome. This could be fixing a bug, changing documentation, or adding a new feature. To test 
-        new changes against existing tests, we have provided a Docker container which takes in an argument of the python version. 
-        This allows the user to check their work before pushing to Github, where travis-ci will run.
-        
-        For python 3.6
-        ```
-        docker build -t local-test --build-arg PYTHON_VERSION=3.6 .
-        docker run --rm local-test:latest bash -i -c "pytest"
-        ```
-        
-        ## Literature and Inspiration
-        
-        * Distributed training: http://seba1511.net/dist_blog/
-        * HOGWILD!: A Lock-Free Approach to Parallelizing Stochastic Gradient Descent: https://arxiv.org/pdf/1106.5730.pdf
-        * Scaling Distributed Machine Learning with the Parameter Server: https://www.cs.cmu.edu/~muli/file/parameter_server_osdi14.pdf
 Keywords: pytorch,spark,sparktorch,machine learning,deep learning
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# SparkTorch
+
+[![Build Status](https://travis-ci.com/dmmiller612/sparktorch.svg?branch=master)](https://travis-ci.org/dmmiller612/sparktorch)
+[![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](https://github.com/dmmiller612/sparktorch)
+<img src="https://img.shields.io/pypi/v/sparktorch.svg" />
+
+![SparkTorch](images/sparktorchi.png)
+
+This is an implementation of Pytorch on Apache Spark. The goal of this library is to provide a simple, understandable interface 
+in distributing the training of your Pytorch model on Spark. With SparkTorch, you can easily integrate your deep 
+learning model with a ML Spark Pipeline. Underneath the hood, SparkTorch offers two distributed training approaches 
+through tree reductions and a parameter server. Through the api, the user can specify the style of training, whether 
+that is distributed synchronous or hogwild.
+
+## Why should I use this?
+
+Like SparkFlow, SparkTorch's main objective is to seamlessly work with Spark's ML Pipelines. This library provides three 
+core components:
+
+* Data parallel distributed training for large datasets. SparkTorch offers distributed synchronous and asynchronous training methodologies. 
+This is useful for training very large datasets that do not fit into a single machine.
+* Full integration with Spark's ML library. This ensures that you can save and load pipelines with your trained model.
+* Inference. With SparkTorch, you can load your existing trained model and run inference on billions of records 
+in parallel. 
+
+On top of these features, SparkTorch can utilize barrier execution, ensuring that all executors run concurrently during 
+training (This is required for synchronous training approaches). 
+
+## Install
+
+Install SparkTorch via pip: `pip install sparktorch`
+
+SparkTorch requires Apache Spark >= 2.4.4, and has only been tested on PyTorch versions >= 1.3.0.
+
+## Full Basic Example
+
+```python
+from sparktorch import serialize_torch_obj, SparkTorch
+import torch
+import torch.nn as nn
+from pyspark.ml.feature import VectorAssembler
+from pyspark.sql import SparkSession
+from pyspark.ml.pipeline import Pipeline
+
+spark = SparkSession.builder.appName("examples").master('local[2]').getOrCreate()
+df = spark.read.option("inferSchema", "true").csv('mnist_train.csv').coalesce(2)
+
+network = nn.Sequential(
+    nn.Linear(784, 256),
+    nn.ReLU(),
+    nn.Linear(256, 256),
+    nn.ReLU(),
+    nn.Linear(256, 10),
+    nn.Softmax(dim=1)
+)
+
+# Build the pytorch object
+torch_obj = serialize_torch_obj(
+    model=network,
+    criterion=nn.CrossEntropyLoss(),
+    optimizer=torch.optim.Adam,
+    lr=0.0001
+)
+
+# Setup features
+vector_assembler = VectorAssembler(inputCols=df.columns[1:785], outputCol='features')
+
+# Create a SparkTorch Model with torch distributed. Barrier execution is on by default for this mode.
+spark_model = SparkTorch(
+    inputCol='features',
+    labelCol='_c0',
+    predictionCol='predictions',
+    torchObj=torch_obj,
+    iters=50,
+    verbose=1
+)
+
+# Can be used in a pipeline and saved.
+p = Pipeline(stages=[vector_assembler, spark_model]).fit(df)
+p.save('simple_dnn')
+```
+
+## Run the Examples
+
+You can run the examples through docker by issuing the following commands at the root of the repository:
+```bash
+make docker-build
+make docker-run-dnn
+make docker-run-cnn
+```
+
+For the cnn example, you will need to give your docker container at least 8gb of memory.
+
+## Documentation
+
+This is a small documentation section on how to SparkTorch. Please look at the examples library for more details.
+
+#### Creating a Torch Object
+
+To create a Torch object for training, you will need to utilize the `serialize_torch_obj` from SparkTorch. To do so, 
+simply add your network, loss criterion, the optimizer class, and any options as a dictionary to supply to the optimizer 
+(such as learning rate). A simple example of this is:
+
+```python
+from sparktorch import serialize_torch_obj
+
+torch_obj = serialize_torch_obj(
+    model=network,
+    criterion=nn.CrossEntropyLoss(),
+    optimizer=torch.optim.Adam,
+    lr=0.0001
+)
+```
+
+When training neural networks on Spark, one issue that many face is OOM errors. To avoid this issue on the driver, you 
+can create a torch object that is only initialized on the worker nodes. To create this object, you can set up the 
+following:
+
+```python
+from sparktorch import serialize_torch_obj_lazy
+
+torch_obj = serialize_torch_obj_lazy(
+    model=Network,
+    criterion=nn.CrossEntropyLoss,
+    optimizer=torch.optim.Adam,
+    optimizer_params={'lr': 0.001},
+    model_parameters={'some_model_param': 5}
+)
+``` 
+
+The Network in the above example must be a nn.module pytorch class. If you need parameters passed into the constructor, 
+you can use the `model_parameters` parameter. The item will be passed in as **kwargs to the constructor. 
+
+NOTE: One thing to remember is that if your network is not a sequential, it will need to be saved in a separate file and
+available in the python path. An example of this can be found in `simple_cnn.py`.
+
+#### Training Options
+
+There are two main training options with SparkTorch: `async` and `hogwild`. The async mode utilizes the torch distributed 
+package, ensuring that the networks are in sync through each iteration. This is the most supported version. When using 
+this option, you will need to be aware that barrier execution is enforced, meaning that the parallelism will need to match 
+the partitions. 
+
+The Hogwild approach utilizes a Flask Service underneath the hood. When using Hogwild, it is strongly recommended that you use the 
+`useBarrier` option to force barrier execution. Below are a list of parameters to SparkTorch and their meaning.
+
+```
+inputCol: Standard Spark InputCol that must be a Vector.
+labelCol: Standard Spark Label column. Can be null.
+torchObj: The TorchObj which is described in the `Creating a Torch Object` section.
+iters: Number of iterations to run per partition.
+predictionCol: The standard spark prediction column for the dataframe.
+partitions: Ability to repartition during training.
+acquireLock: Used in Hogwild only. Forces locking on the server.
+verbose: Describes whether you want real time logging
+partitionShuffles: Only used in Hogwild. Will reshuffle data after completing training.
+port: Only used in hogwild. Server port.
+useBarrier: Only used in hogwild. Describes whether you want barrier execution. (Async mode uses barrier by default)
+useVectorOut: Boolean to describe if you want the model output to be a vector (Defaults to float).
+earlyStopPatience: If greater than 0, it will enforce early stopping based on validation.
+miniBatch: Minibatch size for training per iteration. (Randomly shuffled)
+validationPct: Percentage to use for validation.
+mode: which training mode to use. `synchronous` leverages torch distributed. `hogwild` currently uses the flask service.
+device: Supply 'cpu' or 'cuda'
+```
+
+#### Saving and Loading Pipelines
+
+Since saving and loading custom ML Transformers in pure python has not been implemented in PySpark, an extension has been
+added here to make that possible. In order to save a Pyspark Pipeline with Apache Spark, one will need to use the overwrite function:
+
+```python
+p = Pipeline(stages=[va, encoded, spark_model]).fit(df)
+p.write().overwrite().save("location")
+```
+
+For loading, a Pipeline wrapper has been provided in the pipeline_utils file. An example is below:
+
+```python
+from sparktorch import PysparkPipelineWrapper
+from pyspark.ml.pipeline import PipelineModel
+
+p = PysparkPipelineWrapper.unwrap(PipelineModel.load('location'))
+``` 
+Then you can perform predictions, etc with:
+
+```python
+predictions = p.transform(df)
+```
+
+#### Getting the Pytorch model from the training session
+
+If you just want to get the Pytorch model after training, you can execute the following code:
+
+```python
+stm = SparkTorch(
+    inputCol='features',
+    labelCol='label',
+    predictionCol='predictions',
+    torchObj=network_with_params,
+    verbose=1,
+    iters=5
+).fit(data)
+
+py_model = stm.getPytorchModel()
+```
+
+
+#### Using a pretrained Pytorch model for inference
+
+If you already have a trained Pytorch model, you can attach it your existing pipeline by directly creating a SparkTorchModel. 
+This can be done by running the following:
+
+```python
+from sparktorch import create_spark_torch_model
+
+net = ... # Pretrained Network
+
+spark_torch_model = create_spark_torch_model(
+    net, 
+    inputCol='features',
+    predictionCol='predictions'
+)
+```
+
+## Running
+
+One big thing to remember is to add the `--executor cores 1` option to spark to ensure
+each executor is only training one copy of the network. This will especially be needed for gpu training.
+
+## Contributing
+
+Contributions are always welcome. This could be fixing a bug, changing documentation, or adding a new feature. To test 
+new changes against existing tests, we have provided a Docker container which takes in an argument of the python version. 
+This allows the user to check their work before pushing to Github, where travis-ci will run.
+
+For python 3.6
+```
+docker build -t local-test --build-arg PYTHON_VERSION=3.6 .
+docker run --rm local-test:latest bash -i -c "pytest"
+```
+
+## Literature and Inspiration
+
+* Distributed training: http://seba1511.net/dist_blog/
+* HOGWILD!: A Lock-Free Approach to Parallelizing Stochastic Gradient Descent: https://arxiv.org/pdf/1106.5730.pdf
+* Scaling Distributed Machine Learning with the Parameter Server: https://www.cs.cmu.edu/~muli/file/parameter_server_osdi14.pdf
```

### Comparing `sparktorch-0.1.2/sparktorch.egg-info/SOURCES.txt` & `sparktorch-0.2.0/sparktorch.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 sparktorch/__init__.py
 sparktorch/distributed.py
 sparktorch/early_stopper.py
 sparktorch/hogwild.py
```

