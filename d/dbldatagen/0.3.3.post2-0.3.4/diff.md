# Comparing `tmp/dbldatagen-0.3.3.post2.tar.gz` & `tmp/dbldatagen-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbldatagen-0.3.3.post2.tar", last modified: Thu Mar 23 02:56:08 2023, max compression
+gzip compressed data, was "dbldatagen-0.3.4.tar", last modified: Sun Apr  9 00:46:09 2023, max compression
```

## Comparing `dbldatagen-0.3.3.post2.tar` & `dbldatagen-0.3.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 02:56:08.188070 dbldatagen-0.3.3.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-03-23 02:56:08.188070 dbldatagen-0.3.3.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 02:56:08.184069 dbldatagen-0.3.3.post2/dbldatagen/
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    56012 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/column_generation_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/column_spec_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/data_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    56248 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/datagen_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/datarange.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/daterange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 02:56:08.184069 dbldatagen-0.3.3.post2/dbldatagen/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/distributions/beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/distributions/data_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/distributions/exponential_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/distributions/gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/distributions/normal_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/function_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/nrange.py
--rw-r--r--   0 runner    (1001) docker     (123)    15512 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/schema_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/spark_singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/text_generator_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    42149 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/text_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/dbldatagen/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 02:56:08.184069 dbldatagen-0.3.3.post2/dbldatagen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-03-23 02:56:08.000000 dbldatagen-0.3.3.post2/dbldatagen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-23 02:56:08.000000 dbldatagen-0.3.3.post2/dbldatagen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 02:56:08.000000 dbldatagen-0.3.3.post2/dbldatagen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-23 02:56:08.000000 dbldatagen-0.3.3.post2/dbldatagen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-23 02:56:08.188070 dbldatagen-0.3.3.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-03-23 02:54:24.000000 dbldatagen-0.3.3.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:46:09.159940 dbldatagen-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-04-09 00:46:09.159940 dbldatagen-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:46:09.159940 dbldatagen-0.3.4/dbldatagen/
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59230 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/column_generation_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/column_spec_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17966 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/data_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57532 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/datagen_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/datarange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/daterange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:46:09.159940 dbldatagen-0.3.4/dbldatagen/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/distributions/beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/distributions/data_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/distributions/exponential_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/distributions/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/distributions/normal_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/function_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/nrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15512 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/schema_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/spark_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/text_generator_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41986 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/text_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10827 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:46:09.159940 dbldatagen-0.3.4/dbldatagen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-04-09 00:46:09.000000 dbldatagen-0.3.4/dbldatagen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-09 00:46:09.000000 dbldatagen-0.3.4/dbldatagen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 00:46:09.000000 dbldatagen-0.3.4/dbldatagen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 00:46:09.000000 dbldatagen-0.3.4/dbldatagen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-09 00:46:09.159940 dbldatagen-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/setup.py
```

### Comparing `dbldatagen-0.3.3.post2/CHANGELOG.md` & `dbldatagen-0.3.4/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,40 @@
 # Databricks Labs Data Generator Release Notes
 
 ## Change History
 All notable changes to the Databricks Labs Data Generator will be documented in this file.
 
-### Unreleased
+### Version 0.3.4
+
+#### Changed
+* Modified option to allow for range when specifying `numFeatures` with `structType='array'` to allow generation
+  of varying number of columns
+* When generating multi-column or array valued columns, compute random seed with different name for each column
+* Additional build ordering enhancements to reduce circumstances where explicit base column must be specified
+
+#### Added
+* Scripting of data generation code from schema (Experimental)
+* Scripting of data generation code from dataframe (Experimental)
+* Added top level `random` attribute to data generator specification constructor
+
+
+### Version 0.3.3post2
 
 #### Changed
 * Fixed use of logger in _version.py and in spark_singleton.py
 * Fixed template issues 
-* Added use of prospector to build process to validate common code issues
+* Document reformatting and updates, related code comment changes
+
+### Fixed
 * Apply pandas optimizations when generating multiple columns using same `withColumn` or `withColumnSpec`
 
+### Added
+* Added use of prospector to build process to validate common code issues
+
+
 ### Version 0.3.2
 
 #### Changed
 * Adjusted column build phase separation (i.e which select statement is used to build columns) so that a 
   column with a SQL expression can refer to previously created columns without use of a `baseColumn` attribute
 * Changed build labelling to comply with PEP440
```

### Comparing `dbldatagen-0.3.3.post2/CONTRIBUTING.md` & `dbldatagen-0.3.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.3.post2/LICENSE` & `dbldatagen-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.3.post2/PKG-INFO` & `dbldatagen-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbldatagen
-Version: 0.3.3.post2
+Version: 0.3.4
 Summary: Databricks Labs -  PySpark Synthetic Data Generator
 Home-page: https://github.com/databrickslabs/data-generator
 Author: Ronan Stokes, Databricks
 License: Databricks License
 Project-URL: Databricks Labs, https://www.databricks.com/learn/labs
 Project-URL: Documentation, https://databrickslabs.github.io/dbldatagen/public_docs/index.html
 Classifier: Programming Language :: Python :: 3
@@ -27,89 +27,90 @@
 
 <!-- 
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/databrickslabs/dbldatagen.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/databrickslabs/dbldatagen/context:python)
 [![downloads](https://img.shields.io/github/downloads/databrickslabs/dbldatagen/total.svg)](https://hanadigital.github.io/grev/?user=databrickslabs&repo=dbldatagen)
 -->
 
 ## Project Description
-The `dbldatgen` Databricks Labs project is a Python library for generating synthetic data within the Databricks 
-environment using Spark. The generated data may be used for testing, benchmarking, demos and many 
+The `dbldatagen` Databricks Labs project is a Python library for generating synthetic data within the Databricks 
+environment using Spark. The generated data may be used for testing, benchmarking, demos, and many 
 other uses.
 
 It operates by defining a data generation specification in code that controls 
-how the synthetic data is to be generated.
-The specification may incorporate use of existing schemas, or create data in an adhoc fashion.
+how the synthetic data is generated.
+The specification may incorporate the use of existing schemas or create data in an ad-hoc fashion.
 
-It has no dependencies on any libraries that are not already incuded in the Databricks 
+It has no dependencies on any libraries that are not already installed in the Databricks 
 runtime, and you can use it from Scala, R or other languages by defining
 a view over the generated data.
 
 ### Feature Summary
 It supports:
 * Generating synthetic data at scale up to billions of rows within minutes using appropriately sized clusters 
-* Generating repeatable, predictable data supporting the needs for producing multiple tables, Change Data Capture, 
+* Generating repeatable, predictable data supporting the need for producing multiple tables, Change Data Capture, 
 merge and join scenarios with consistency between primary and foreign keys
 * Generating synthetic data for all of the 
 Spark SQL supported primitive types as a Spark data frame which may be persisted, 
 saved to external storage or 
 used in other computations
-* Generating ranges of dates, timestamps and numeric values
+* Generating ranges of dates, timestamps, and numeric values
 * Generation of discrete values - both numeric and text
 * Generation of values at random and based on the values of other fields 
 (either based on the `hash` of the underlying values or the values themselves)
 * Ability to specify a distribution for random data generation 
-* Generating arrays of values for ML style feature arrays
+* Generating arrays of values for ML-style feature arrays
 * Applying weights to the occurrence of values
 * Generating values to conform to a schema or independent of an existing schema
-* use of SQL expressions in test data generation
+* use of SQL expressions in synthetic data generation
 * plugin mechanism to allow use of 3rd party libraries such as Faker
 * Use within a Databricks Delta Live Tables pipeline as a synthetic data generation source
+* Generate synthetic data generation code from existing schema or data (experimental)
 
 Details of these features can be found in the online documentation  -
  [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html). 
 
 ## Documentation
 
 Please refer to the [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html) for 
 details of use and many examples.
 
 Release notes and details of the latest changes for this specific release
-can be found in the Github repository
-[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.3post2/CHANGELOG.md)
+can be found in the GitHub repository
+[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.4/CHANGELOG.md)
 
 # Installation
 
-Use `pip install dbldatagen` to install the PyPi package
+Use `pip install dbldatagen` to install the PyPi package.
 
 Within a Databricks notebook, invoke the following in a notebook cell
 ```commandline
 %pip install dbldatagen
 ```
 
-This can be invoked within a Databricks notebook, a Delta Live Tables pipeline and even works on the Databricks 
-community edition.
+The Pip install command can be invoked within a Databricks notebook, a Delta Live Tables pipeline 
+and even works on the Databricks community edition.
 
 The documentation [installation notes](https://databrickslabs.github.io/dbldatagen/public_docs/installation_notes.html) 
 contains details of installation using alternative mechanisms.
 
 ## Compatibility 
-The Databricks Labs data generator framework can be used with Pyspark 3.1.2 and Python 3.8 or later. These are 
+The Databricks Labs Data Generator framework can be used with Pyspark 3.1.2 and Python 3.8 or later. These are 
 compatible with the Databricks runtime 9.1 LTS and later releases.
 
 Older prebuilt releases are tested against Pyspark 3.0.1 (compatible with the Databricks runtime 7.3 LTS 
 or later) and built with Python 3.7.5
 
 For full library compatibility for a specific Databricks Spark release, see the Databricks 
 release notes for library compatibility
 
 - https://docs.databricks.com/release-notes/runtime/releases.html
 
-When using the Databricks Labs Data Generator on Unity Catalog enabled environments, the Data Generator requires
+When using the Databricks Labs Data Generator on "Unity Catalog" enabled environments, the Data Generator requires
 the use of `Single User` or `No Isolation Shared` access modes as some needed features are not available in `Shared` 
-mode (for example, use of 3rd party libraries). Depending on settings, `Custom` access mode may be supported.
+mode (for example, use of 3rd party libraries). Depending on settings, the `Custom` access mode may be supported.
 
 See the following documentation for more information:
 
 - https://docs.databricks.com/data-governance/unity-catalog/compute.html
 
 ## Using the Data Generator
 To use the data generator, install the library using the `%pip install` method or install the Python wheel directly 
@@ -142,38 +143,38 @@
                             
 df = df_spec.build()
 num_rows=df.count()                          
 ```
 Refer to the [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html) for further 
 examples. 
 
-The Github repository also contains further examples in the examples directory
+The GitHub repository also contains further examples in the examples directory.
 
 ## Spark and Databricks Runtime Compatibility
-The `dbldatagen` package is intended to be compatible with recent LTS versions of the Databricks runtime including 
-older LTS versions at least from 10.4 LTS and later. It also aims to be compatible with Delta Live Table runtimes 
+The `dbldatagen` package is intended to be compatible with recent LTS versions of the Databricks runtime, including 
+older LTS versions at least from 10.4 LTS and later. It also aims to be compatible with Delta Live Table runtimes, 
 including `current` and `preview`. 
 
-While we dont specifically drop support for older runtimes, changes in Pyspark APIs or
-APIs from dependent packages such as `numpy`, `pandas`, `pyarrow` and `pyparsing` make cause issues with older
+While we don't specifically drop support for older runtimes, changes in Pyspark APIs or
+APIs from dependent packages such as `numpy`, `pandas`, `pyarrow`, and `pyparsing` make cause issues with older
 runtimes. 
 
-Installing `dbldatagen` explicitly does not install releases of dependent packages so as to preserve the curated
-set of packages installed in any Databricks runtime environment.
+By design, installing `dbldatagen` does not install releases of dependent packages in order 
+to preserve the curated set of packages pre-installed in any Databricks runtime environment.
 
-When building on local environments, the `Pipfile` and requirements files are used to determine the versions 
-tested against for releases and unit tests. 
+When building on local environments, the build process uses the `Pipfile` and requirements files to determine 
+the package versions for releases and unit tests. 
 
 ## Project Support
 Please note that all projects released under [`Databricks Labs`](https://www.databricks.com/learn/labs)
  are provided for your exploration only, and are not formally supported by Databricks with Service Level Agreements 
-(SLAs).  They are provided AS-IS and we do not make any guarantees of any kind.  Please do not submit a support ticket 
+(SLAs).  They are provided AS-IS, and we do not make any guarantees of any kind.  Please do not submit a support ticket 
 relating to any issues arising from the use of these projects.
 
-Any issues discovered through the use of this project should be filed as issues on the Github Repo.  
+Any issues discovered through the use of this project should be filed as issues on the GitHub Repo.  
 They will be reviewed as time permits, but there are no formal SLAs for support.
 
 
 ## Feedback
 
 Issues with the application?  Found a bug?  Have a great idea for an addition?
 Feel free to file an [issue](https://github.com/databrickslabs/dbldatagen/issues/new).
```

### Comparing `dbldatagen-0.3.3.post2/PULL_REQUEST_TEMPLATE.md` & `dbldatagen-0.3.4/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.3.post2/README.md` & `dbldatagen-0.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,89 +15,90 @@
 
 <!-- 
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/databrickslabs/dbldatagen.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/databrickslabs/dbldatagen/context:python)
 [![downloads](https://img.shields.io/github/downloads/databrickslabs/dbldatagen/total.svg)](https://hanadigital.github.io/grev/?user=databrickslabs&repo=dbldatagen)
 -->
 
 ## Project Description
-The `dbldatgen` Databricks Labs project is a Python library for generating synthetic data within the Databricks 
-environment using Spark. The generated data may be used for testing, benchmarking, demos and many 
+The `dbldatagen` Databricks Labs project is a Python library for generating synthetic data within the Databricks 
+environment using Spark. The generated data may be used for testing, benchmarking, demos, and many 
 other uses.
 
 It operates by defining a data generation specification in code that controls 
-how the synthetic data is to be generated.
-The specification may incorporate use of existing schemas, or create data in an adhoc fashion.
+how the synthetic data is generated.
+The specification may incorporate the use of existing schemas or create data in an ad-hoc fashion.
 
-It has no dependencies on any libraries that are not already incuded in the Databricks 
+It has no dependencies on any libraries that are not already installed in the Databricks 
 runtime, and you can use it from Scala, R or other languages by defining
 a view over the generated data.
 
 ### Feature Summary
 It supports:
 * Generating synthetic data at scale up to billions of rows within minutes using appropriately sized clusters 
-* Generating repeatable, predictable data supporting the needs for producing multiple tables, Change Data Capture, 
+* Generating repeatable, predictable data supporting the need for producing multiple tables, Change Data Capture, 
 merge and join scenarios with consistency between primary and foreign keys
 * Generating synthetic data for all of the 
 Spark SQL supported primitive types as a Spark data frame which may be persisted, 
 saved to external storage or 
 used in other computations
-* Generating ranges of dates, timestamps and numeric values
+* Generating ranges of dates, timestamps, and numeric values
 * Generation of discrete values - both numeric and text
 * Generation of values at random and based on the values of other fields 
 (either based on the `hash` of the underlying values or the values themselves)
 * Ability to specify a distribution for random data generation 
-* Generating arrays of values for ML style feature arrays
+* Generating arrays of values for ML-style feature arrays
 * Applying weights to the occurrence of values
 * Generating values to conform to a schema or independent of an existing schema
-* use of SQL expressions in test data generation
+* use of SQL expressions in synthetic data generation
 * plugin mechanism to allow use of 3rd party libraries such as Faker
 * Use within a Databricks Delta Live Tables pipeline as a synthetic data generation source
+* Generate synthetic data generation code from existing schema or data (experimental)
 
 Details of these features can be found in the online documentation  -
  [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html). 
 
 ## Documentation
 
 Please refer to the [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html) for 
 details of use and many examples.
 
 Release notes and details of the latest changes for this specific release
-can be found in the Github repository
-[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.3post2/CHANGELOG.md)
+can be found in the GitHub repository
+[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.4/CHANGELOG.md)
 
 # Installation
 
-Use `pip install dbldatagen` to install the PyPi package
+Use `pip install dbldatagen` to install the PyPi package.
 
 Within a Databricks notebook, invoke the following in a notebook cell
 ```commandline
 %pip install dbldatagen
 ```
 
-This can be invoked within a Databricks notebook, a Delta Live Tables pipeline and even works on the Databricks 
-community edition.
+The Pip install command can be invoked within a Databricks notebook, a Delta Live Tables pipeline 
+and even works on the Databricks community edition.
 
 The documentation [installation notes](https://databrickslabs.github.io/dbldatagen/public_docs/installation_notes.html) 
 contains details of installation using alternative mechanisms.
 
 ## Compatibility 
-The Databricks Labs data generator framework can be used with Pyspark 3.1.2 and Python 3.8 or later. These are 
+The Databricks Labs Data Generator framework can be used with Pyspark 3.1.2 and Python 3.8 or later. These are 
 compatible with the Databricks runtime 9.1 LTS and later releases.
 
 Older prebuilt releases are tested against Pyspark 3.0.1 (compatible with the Databricks runtime 7.3 LTS 
 or later) and built with Python 3.7.5
 
 For full library compatibility for a specific Databricks Spark release, see the Databricks 
 release notes for library compatibility
 
 - https://docs.databricks.com/release-notes/runtime/releases.html
 
-When using the Databricks Labs Data Generator on Unity Catalog enabled environments, the Data Generator requires
+When using the Databricks Labs Data Generator on "Unity Catalog" enabled environments, the Data Generator requires
 the use of `Single User` or `No Isolation Shared` access modes as some needed features are not available in `Shared` 
-mode (for example, use of 3rd party libraries). Depending on settings, `Custom` access mode may be supported.
+mode (for example, use of 3rd party libraries). Depending on settings, the `Custom` access mode may be supported.
 
 See the following documentation for more information:
 
 - https://docs.databricks.com/data-governance/unity-catalog/compute.html
 
 ## Using the Data Generator
 To use the data generator, install the library using the `%pip install` method or install the Python wheel directly 
@@ -130,38 +131,38 @@
                             
 df = df_spec.build()
 num_rows=df.count()                          
 ```
 Refer to the [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html) for further 
 examples. 
 
-The Github repository also contains further examples in the examples directory
+The GitHub repository also contains further examples in the examples directory.
 
 ## Spark and Databricks Runtime Compatibility
-The `dbldatagen` package is intended to be compatible with recent LTS versions of the Databricks runtime including 
-older LTS versions at least from 10.4 LTS and later. It also aims to be compatible with Delta Live Table runtimes 
+The `dbldatagen` package is intended to be compatible with recent LTS versions of the Databricks runtime, including 
+older LTS versions at least from 10.4 LTS and later. It also aims to be compatible with Delta Live Table runtimes, 
 including `current` and `preview`. 
 
-While we dont specifically drop support for older runtimes, changes in Pyspark APIs or
-APIs from dependent packages such as `numpy`, `pandas`, `pyarrow` and `pyparsing` make cause issues with older
+While we don't specifically drop support for older runtimes, changes in Pyspark APIs or
+APIs from dependent packages such as `numpy`, `pandas`, `pyarrow`, and `pyparsing` make cause issues with older
 runtimes. 
 
-Installing `dbldatagen` explicitly does not install releases of dependent packages so as to preserve the curated
-set of packages installed in any Databricks runtime environment.
+By design, installing `dbldatagen` does not install releases of dependent packages in order 
+to preserve the curated set of packages pre-installed in any Databricks runtime environment.
 
-When building on local environments, the `Pipfile` and requirements files are used to determine the versions 
-tested against for releases and unit tests. 
+When building on local environments, the build process uses the `Pipfile` and requirements files to determine 
+the package versions for releases and unit tests. 
 
 ## Project Support
 Please note that all projects released under [`Databricks Labs`](https://www.databricks.com/learn/labs)
  are provided for your exploration only, and are not formally supported by Databricks with Service Level Agreements 
-(SLAs).  They are provided AS-IS and we do not make any guarantees of any kind.  Please do not submit a support ticket 
+(SLAs).  They are provided AS-IS, and we do not make any guarantees of any kind.  Please do not submit a support ticket 
 relating to any issues arising from the use of these projects.
 
-Any issues discovered through the use of this project should be filed as issues on the Github Repo.  
+Any issues discovered through the use of this project should be filed as issues on the GitHub Repo.  
 They will be reviewed as time permits, but there are no formal SLAs for support.
 
 
 ## Feedback
 
 Issues with the application?  Found a bug?  Have a great idea for an addition?
 Feel free to file an [issue](https://github.com/databrickslabs/dbldatagen/issues/new).
```

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/__init__.py` & `dbldatagen-0.3.4/dbldatagen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 Most of the other classes are used for internal purposes only
 """
 
 from .data_generator import DataGenerator
 from .datagen_constants import DEFAULT_RANDOM_SEED, RANDOM_SEED_RANDOM, RANDOM_SEED_FIXED, \
                                RANDOM_SEED_HASH_FIELD_NAME, MIN_PYTHON_VERSION, MIN_SPARK_VERSION
 from .utils import ensure, topologicalSort, mkBoundsList, coalesce_values, \
-    deprecated, parse_time_interval, DataGenError, split_list_matching_condition
+    deprecated, parse_time_interval, DataGenError, split_list_matching_condition, strip_margins
 from ._version import __version__
 from .column_generation_spec import ColumnGenerationSpec
 from .column_spec_options import ColumnSpecOptions
 from .data_analyzer import DataAnalyzer
 from .schema_parser import SchemaParser
 from .daterange import DateRange
 from .datarange import DataRange
```

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/_version.py` & `dbldatagen-0.3.4/dbldatagen/_version.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     r = re.compile(r'(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+){0,1}(?P<release>\D*)(?P<build>\d*)')
     major, minor, patch, release, build = r.match(version).groups()
     version_info = VersionInfo(major, minor, patch, release, build)
     logging.info("Version : %s", version_info)
     return version_info
 
 
-__version__ = "0.3.3post2"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
+__version__ = "0.3.4"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
 __version_info__ = get_version(__version__)
 
 
 def _get_spark_version(sparkVersion):
     try:
         r = re.compile(r'(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>.*)')
         major, minor, patch, release = r.match(sparkVersion).groups()
```

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/column_generation_spec.py` & `dbldatagen-0.3.4/dbldatagen/column_generation_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,24 @@
 
 import copy
 import logging
 
 from pyspark.sql.functions import col, pandas_udf
 from pyspark.sql.functions import lit, concat, rand, round as sql_round, array, expr, when, udf, \
     format_string
+
+import pyspark.sql.functions as F
+
 from pyspark.sql.types import FloatType, IntegerType, StringType, DoubleType, BooleanType, \
     TimestampType, DataType, DateType, ArrayType, MapType, StructType
 
 from .column_spec_options import ColumnSpecOptions
-from .datagen_constants import RANDOM_SEED_FIXED, RANDOM_SEED_HASH_FIELD_NAME, RANDOM_SEED_RANDOM, DEFAULT_SEED_COLUMN
+from .datagen_constants import RANDOM_SEED_FIXED, RANDOM_SEED_HASH_FIELD_NAME, RANDOM_SEED_RANDOM, \
+    DEFAULT_SEED_COLUMN, OPTION_RANDOM, OPTION_RANDOM_SEED, OPTION_RANDOM_SEED_METHOD
+
 from .daterange import DateRange
 from .distributions import Normal, DataDistribution
 from .nrange import NRange
 from .text_generators import TemplateGenerator
 from .utils import ensure, coalesce_values
 
 HASH_COMPUTE_METHOD = "hash"
@@ -52,15 +57,16 @@
     :param max: maximum value of the column
     :param step: numeric step used in column data generation
     :param prefix: string used as prefix to the column underlying value to produce a string value
     :param random: Boolean, if True, will generate random values
     :param distribution: Instance of distribution, that will control the distribution of the generated values
     :param baseColumn: String or list of strings representing columns used as basis for generating the column data
     :param randomSeed: random seed value used to generate the random value, if column data is random
-    :param randomSeedMethod: method for computing random values from the random seed
+    :param randomSeedMethod: method for computing random values from the random seed. It may take on the
+           values `fixed`, `hash_fieldname` or None
 
     :param implicit: If True, the specification for the column can be replaced by a later definition.
            If not, a later attempt to replace the definition will flag an error.
            Typically used when generating definitions automatically from a schema, or when using wildcards
            in the specification
 
     :param omit: if True, omit from the final output.
@@ -115,16 +121,16 @@
             baseColumn = self._seedColumnName
 
         # to allow for open ended extension of many column attributes, we use a few specific
         # parameters and pass the rest as keyword arguments
         supplied_options = {'name': name, 'minValue': minValue, 'type': colType,
                             'maxValue': maxValue, 'step': step,
                             'prefix': prefix, 'baseColumn': baseColumn,
-                            'random': random, 'distribution': distribution,
-                            'randomSeedMethod': randomSeedMethod, 'randomSeed': randomSeed,
+                            OPTION_RANDOM: random, 'distribution': distribution,
+                            OPTION_RANDOM_SEED_METHOD: randomSeedMethod, OPTION_RANDOM_SEED: randomSeed,
                             'omit': omit, 'nullable': nullable, 'implicit': implicit
                             }
 
         supplied_options.update(kwargs)
 
         self._csOptions = ColumnSpecOptions(supplied_options)
 
@@ -169,22 +175,22 @@
         # should be either a literal or None
         # use of a random seed method will ensure that we have repeatability of data generation
         assert randomSeed is None or type(randomSeed) in [int, float], "seed should be None or numeric"
 
         assert randomSeedMethod is None or randomSeedMethod in [RANDOM_SEED_FIXED, RANDOM_SEED_HASH_FIELD_NAME], \
             f"`randomSeedMethod` should be none or `{RANDOM_SEED_FIXED}` or `{RANDOM_SEED_HASH_FIELD_NAME}`"
 
-        self._randomSeedMethod = self['randomSeedMethod']
-        self.random = self['random']
+        self._randomSeedMethod = self[OPTION_RANDOM_SEED_METHOD]
+        self.random = self[OPTION_RANDOM]
 
         if self._randomSeedMethod == RANDOM_SEED_HASH_FIELD_NAME:
             assert self.name is not None, "field name cannot be None"
             self._randomSeed = abs(hash(self.name))
         else:
-            self._randomSeed = self["randomSeed"]
+            self._randomSeed = self[OPTION_RANDOM_SEED]
 
         # random seed method should be "fixed" or "hash_fieldname"
         if self._randomSeed is not None and self._randomSeedMethod is None:
             self._randomSeedMethod = RANDOM_SEED_FIXED
 
         # compute dependencies
         self.dependencies = self._computeBasicDependencies()
@@ -276,14 +282,79 @@
                    or
                    self.values is not None,
                    """When using an explicit distribution, provide a fully populated range or a set of values""")
 
         # set up the temporary columns needed for data generation
         self._setupTemporaryColumns()
 
+    def _temporaryRename(self, tmpName):
+        """ Create enter / exit object to support temporary renaming of column spec
+
+        This is to support the functionality:
+
+        ```
+           with columSpec._temporaryRename("test") as modifiedColumn:
+             modifiedColumn.doSomthing()
+        ```
+
+        When building array or multi-column valued columns, we rename the column definition temporarily
+        to ensure that logging, saving messages to the execution plan and random number generation based on
+        the field name work correctly
+
+        :param tmpName: temporary name for the column.
+        :return: object supporting `with columSpec._temporaryRename("test") as modifiedColumn:` semantics
+
+        .. note::
+           This does not create a copy of the column spec object
+
+        """
+        # create class for temporary rename enter / exit
+        assert tmpName is not None and len(tmpName) > 0, "method expects valid temporary name"
+
+        class RenameEnterExit:
+            def __init__(self, columnSpec, newName):
+                """ Save column spec and old name to support enter / exit semantics """
+                self._cs = columnSpec
+                self._oldName = columnSpec.name
+                self._newName = newName
+                self._randomSeed = columnSpec._randomSeed
+
+            def __enter__(self):
+                """ Return the inner column spec object """
+                self._cs.name = self._newName
+
+                if self._cs._randomSeedMethod == RANDOM_SEED_HASH_FIELD_NAME:
+                    self._cs._randomSeed = abs(hash(self._cs.name))
+
+                    if self._cs._textGenerator is not None and self._cs._randomSeed is not None:
+                        self._cs._textGenerator = self._cs._textGenerator.withRandomSeed(self._cs._randomSeed)
+
+                return self._cs
+
+            def __exit__(self, exc_type, exc_value, tb):
+                # restore old name
+                self._cs.name = self._oldName
+
+                # restore old random seed
+                self._cs._randomSeed = self._randomSeed
+
+                if self._cs._randomSeedMethod == RANDOM_SEED_HASH_FIELD_NAME:
+                    if self._cs._textGenerator is not None and self._cs._randomSeed is not None:
+                        self._cs._textGenerator = self._cs._textGenerator.withRandomSeed(self._cs._randomSeed)
+
+                if exc_type is not None:
+                    # uncomment for traceback
+                    # import traceback
+                    # traceback.print_exception(exc_type, exc_value, tb)
+                    return False
+
+                return True
+
+        return RenameEnterExit(self, tmpName)
+
     @property
     def specOptions(self):
         """ get column spec options for spec
 
         .. note::
             This is intended for testing use only.
             Option values set directly through the options dict are not supported.
@@ -316,15 +387,15 @@
     def randomSeed(self):
         """ get random seed for column spec"""
         return self._randomSeed
 
     @property
     def isRandom(self):
         """ returns True if column will be randomly generated"""
-        return self["random"]
+        return self[OPTION_RANDOM]
 
     @property
     def textGenerator(self):
         """ Get the text generator for the column spec"""
         return self._textGenerator
 
     @property
@@ -368,17 +439,16 @@
 
         For some types of test data, intermediate columns are used in the data generation process
         but dropped from the final output
         """
         if self.isWeightedValuesColumn:
             # if its a weighted values column, then create temporary for it
             # not supported for feature / array columns for now
-            ensure(self['numFeatures'] is None or self['numFeatures'] <= 1,
-                   "weighted columns not supported for multi-column or multi-feature values")
-            ensure(self['numColumns'] is None or self['numColumns'] <= 1,
+            min_num_columns, max_num_columns, struct_type = self._getMultiColumnDetails(validate=False)
+            ensure(max_num_columns is None or max_num_columns <= 1,
                    "weighted columns not supported for multi-column or multi-feature values")
             if self.random:
                 temp_name = f"_rnd_{self.name}"
                 self.dependencies.append(temp_name)
                 desc = f"adding temporary column {temp_name} required by {self.name}"
                 self._initialBuildPlan.append(desc)
                 sql_random_generator = self._getUniformRandomSQLExpression(self.name)
@@ -606,29 +676,27 @@
     @property
     def isWeightedValuesColumn(self):
         """ check if column is a weighed values column """
         return self['weights'] is not None and self.values is not None
 
     def getNames(self):
         """ get column names as list of strings"""
-        num_columns = self._csOptions.getOrElse('numColumns', 1)
-        struct_type = self._csOptions.getOrElse('structType', None)
+        min_num_columns, max_num_columns, struct_type = self._getMultiColumnDetails(validate=False)
 
-        if num_columns > 1 and struct_type is None:
-            return [f"{self.name}_{x}" for x in range(0, num_columns)]
+        if max_num_columns > 1 and struct_type is None:
+            return [f"{self.name}_{x}" for x in range(0, max_num_columns)]
         else:
             return [self.name]
 
     def getNamesAndTypes(self):
         """ get column names as list of tuples `(name, datatype)`"""
-        num_columns = self._csOptions.getOrElse('numColumns', 1)
-        struct_type = self._csOptions.getOrElse('structType', None)
+        min_num_columns, max_num_columns, struct_type = self._getMultiColumnDetails(validate=False)
 
-        if num_columns > 1 and struct_type is None:
-            return [(f"{self.name}_{x}", self.datatype) for x in range(0, num_columns)]
+        if max_num_columns > 1 and struct_type is None:
+            return [(f"{self.name}_{x}", self.datatype) for x in range(0, max_num_columns)]
         else:
             return [(self.name, self.datatype)]
 
     def keys(self):
         """ Get the keys as list of strings """
         assert self._csOptions is not None, "self._csOptions should be non-empty"
         return self._csOptions.keys()
@@ -763,51 +831,14 @@
         :param key: key name for option
         :param default: default value if option was not provided
         :return: option value or default
 
         """
         return self._csOptions.getOrElse(key, default)
 
-    def _checkProps(self, column_props):
-        """
-            check that column definition properties are recognized
-            and that the column definition has required properties
-
-        :raises: assertion or exception of checks fail
-        """
-        assert column_props is not None, "Column definition properties should be non-empty"
-        assert self.datatype is not None, "Column datatype must be specified"
-
-        if self.datatype.typeName() in self._max_type_range:
-            minValue = self['minValue']
-            maxValue = self['maxValue']
-
-            if minValue is not None and maxValue is not None:
-                effective_range = maxValue - minValue
-                if effective_range > self._max_type_range[self.datatype.typeName()]:
-                    raise ValueError("Effective range greater than range of type")
-
-        for k in column_props.keys():
-            ensure(k in ColumnSpecOptions._ALLOWED_PROPERTIES, f'invalid column option {k}')
-
-        for arg in ColumnSpecOptions._REQUIRED_PROPERTIES:
-            ensure(column_props.get(arg) is not None, f'missing column option {arg}')
-
-        for arg in ColumnSpecOptions._FORBIDDEN_PROPERTIES:
-            ensure(arg not in column_props, f'forbidden column option {arg}')
-
-        # check weights and values
-        if 'weights' in column_props:
-            ensure('values' in column_props,
-                   f"weights are only allowed for columns with values - column '{column_props['name']}' ")
-            ensure(column_props['values'] is not None and len(column_props['values']) > 0,
-                   f"weights must be associated with non-empty list of values - column '{column_props['name']}' ")
-            ensure(len(column_props['values']) == len(column_props['weights']),
-                   f"length(list of weights) != length(list of values)  - column '{column_props['name']}' ")
-
     def getPlanEntry(self):
         """ Get execution plan entry for object
 
         :returns: String representation of plan entry
         """
         desc = self['description']
         if desc is not None:
@@ -945,25 +976,25 @@
             new_def = baseval + lit(datarange.minValue)
         elif (datarange is not None) and (datarange.minValue != 0) and (datarange.minValue != 0.0):
             new_def = baseval + lit(datarange.minValue)
         else:
             new_def = baseval
         return new_def
 
-    def _makeSingleGenerationExpression(self, index=None, use_pandas_optimizations=False):
+    def _makeSingleGenerationExpression(self, index=None, use_pandas_optimizations=True):
         """ generate column data for a single column value via Spark SQL expression
 
+            :param index: for multi column generation, specifies index of column being generated
+            :param use_pandas_optimizations: if True, uses Pandas vectorized optimizations. Defaults to `True`
             :returns: spark sql `column` or expression that can be used to generate a column
         """
         self.logger.debug("building column : %s", self.name)
 
         # get key column specification properties
-        col_is_rand, cdistribution = self['random'], self['distribution']
-        base_col = self.baseColumn
-        c_begin, c_end, c_interval = self['begin'], self['end'], self['interval']
+        col_is_rand, cdistribution = self[OPTION_RANDOM], self['distribution']
         percent_nulls = self['percentNulls']
         sformat = self['format']
 
         if self._dataRange is not None:
             self._dataRange.adjustForColumnDatatype(self.datatype)
             self.executionHistory.append(f".. using effective range: {self._dataRange}")
 
@@ -1139,48 +1170,93 @@
         # check for implied ranges
         if self.values is not None:
             self._dataRange = NRange(0, len(self.values) - 1, 1)
         elif type(col_type) is BooleanType:
             self._dataRange = NRange(0, 1, 1)
         self.executionHistory.append(f".. using adjusted effective range: {self._dataRange}")
 
+    def _getMultiColumnDetails(self, validate):
+        """ Determine min and max number of columns to generate along with `structType` for columns
+            with multiple columns / features
+
+        :param validate:  If true, raises ValueError if there are bad option entries
+        :return: tuple of (min_columns, max_columns, structType
+        """
+        num_columns = self['numColumns']
+        struct_type = self['structType']
+
+        if num_columns is None:
+            num_columns = self['numFeatures']
+
+        if num_columns is None:
+            min_num_columns, max_num_columns = 1, 1
+        elif isinstance(num_columns, int):
+            min_num_columns, max_num_columns = int(num_columns), int(num_columns)
+        elif isinstance(num_columns, tuple):
+            if validate and ((len(num_columns) != 2) or not all(isinstance(c, int) for c in num_columns)):
+                raise ValueError(f"Bad value [{num_columns}] for `numColumns` / `numFeatures` attribute")
+
+            min_num_columns, max_num_columns = int(num_columns[0]), int(num_columns[1])
+
+            if validate and (min_num_columns > max_num_columns):
+                raise ValueError(f"Bad value [{num_columns}] for `numColumns` / `numFeatures` attribute")
+        else:
+            if validate:
+                raise ValueError(f"Bad value [{num_columns}] for `numColumns` / `numFeatures` attribute")
+
+            min_num_columns, max_num_columns = 1, 1
+
+        if validate and (min_num_columns != max_num_columns) and (struct_type != "array"):
+            self.logger.warning(
+                f"Varying number of features / columns specified for non-array column [{self.name}]")
+            self.logger.warning(
+                f"Lower bound for number of features / columns ignored for [{self.name}]")
+            min_num_columns = max_num_columns
+
+        return min_num_columns, max_num_columns, struct_type
+
     def makeGenerationExpressions(self):
         """ Generate structured column if multiple columns or features are specified
 
         if there are multiple columns / features specified using a single definition, it will generate
         a set of columns conforming to the same definition,
         renaming them as appropriate and combine them into a array if necessary
         (depending on the structure combination instructions)
 
             :param self: is ColumnGenerationSpec for column
             :returns: spark sql `column` or expression that can be used to generate a column
         """
-        num_columns = self['numColumns']
-        struct_type = self['structType']
-        self.executionHistory = []
+        min_num_columns, max_num_columns, struct_type = self._getMultiColumnDetails(validate=True)
 
-        if num_columns is None:
-            num_columns = self['numFeatures']
+        self.executionHistory = []
 
-        if num_columns == 1 or num_columns is None:
+        if (min_num_columns == 1) and (max_num_columns == 1):
             # record execution history for troubleshooting
             self.executionHistory.append(f"generating single column - `{self.name}` having type `{self.datatype}`")
 
             retval = self._makeSingleGenerationExpression(use_pandas_optimizations=True)
 
             # record how column was generated
             exec_step_history = ".. computed from base values - "
             exec_step_history += f"`{self.baseColumn}`, method: `{self._baseColumnComputeMethod}`"
             self.executionHistory.append(exec_step_history)
         else:
-            self.executionHistory.append(f"generating multiple columns {num_columns} - `{self['name']}`")
-            retval = [self._makeSingleGenerationExpression(x, use_pandas_optimizations=True) for x in
-                      range(num_columns)]
+            self.executionHistory.append(f"generating multiple columns {max_num_columns} - `{self.name}`")
+
+            retval = []
+
+            for ix in range(max_num_columns):
+                with self._temporaryRename(f"{self.name}_{ix}") as renamed_cs:
+                    retval.append(renamed_cs._makeSingleGenerationExpression(ix, use_pandas_optimizations=True))
 
             if struct_type == 'array':
                 self.executionHistory.append(".. converting multiple columns to array")
                 retval = array(retval)
-            else:
-                # TODO : update the output columns
-                pass
+
+                if min_num_columns != max_num_columns:
+                    column_set = ",".join(self.baseColumns)
+                    diff = max_num_columns - min_num_columns
+                    expr_str = f"{min_num_columns} + (abs(hash({column_set})) % {diff + 1})"
+
+                    retval = F.slice(retval, F.lit(1), F.expr(expr_str))
 
         return retval
```

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/column_spec_options.py` & `dbldatagen-0.3.4/dbldatagen/column_spec_options.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,33 +32,39 @@
                      As an alternative, you may use the `dataRange` parameter
 
     :param maxValue: Maximum value for range of generated value. \
                      As an alternative, you may use the `dataRange` parameter
 
     :param step: Step to use for range of generated value. As an alternative, you may use the `dataRange` parameter
 
+    :param numColumns: generate `n` columns numbered from 1 .. n-1 with same definition
+
+    :param numFeatures: generate `n` columns numbered from 0 .. n-1 with same definition. Alias for `numColumns`
+
+    :param structType: If specified as "array" and used with numColumns / numFeatures, will combine columns as array
+
     :param random: If True, will generate random values for column value. Defaults to `False`
 
     :param baseColumn: Either the string name of the base column, or a list of columns to use to
                         control data generation. The option ``baseColumns`` is an alias for ``baseColumn``.
 
     :param values: List of discrete values for the colummn. Discrete values for the column can be strings, numbers
                    or constants conforming to type of column
 
     :param weights: List of discrete weights for the colummn. Should be integer values.
                     For example, you might declare a column for status values with a weighted distribution with
-                    the following statement: \
+                    the following statement:
                     `withColumn("status", StringType(), values=['online', 'offline', 'unknown'], weights=[3,2,1])`
 
     :param percentNulls: Specifies numeric percentage of generated values to be populated with SQL `null`.
                           Value is fraction representing percentage between 0.0 and 1.0
                           For example: `percentNulls=0.12` will give approximately 12% nulls for this field in the
                           output.
-s
-    :param unique_values: Number of unique values for column.
+
+    :param uniqueValues: Number of unique values for column.
                           If the unique values are specified for a timestamp or date field, the values will be chosen
                           working back from the end of the previous month,
                           unless `begin`, `end` and `interval` parameters are specified
 
     :param begin: Beginning of range for date and timestamp fields.
                    For dates and timestamp fields, use the `begin`, `end` and `interval`
                    or `dataRange` parameters instead of `minValue`, `maxValue` and `step`
@@ -72,15 +78,15 @@
                    or `dataRange` parameters instead of `minValue`, `maxValue` and `step`
 
     :param dataRange: An instance of an `NRange` or `DateRange` object. This can be used in place of `minValue`,
                        `maxValue`, `step` or `begin`, `end`, `interval`.
 
     :param template: template controlling how text should be generated
 
-    :param text_separator: string specifying separator to be used when constructing strings with prefix and suffix
+    :param textSeparator: string specifying separator to be used when constructing strings with prefix and suffix
 
     :param prefix: string specifying prefix text to construct field from prefix and numeric value. Both `prefix` and
                    `suffix` can be used together
 
     :param suffix: string specifying suffix text to construct field from suffix and numeric value. Both `prefix` and
                    `suffix` can be used together
```

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/data_generator.py` & `dbldatagen-0.3.4/dbldatagen/data_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 import logging
 import re
 
 from pyspark.sql.types import LongType, IntegerType, StringType, StructType, StructField, DataType
 from .spark_singleton import SparkSingleton
 from .column_generation_spec import ColumnGenerationSpec
 from .datagen_constants import DEFAULT_RANDOM_SEED, RANDOM_SEED_FIXED, RANDOM_SEED_HASH_FIELD_NAME, \
-                               DEFAULT_SEED_COLUMN, SPARK_RANGE_COLUMN, MIN_SPARK_VERSION
+                               DEFAULT_SEED_COLUMN, SPARK_RANGE_COLUMN, MIN_SPARK_VERSION, \
+                               OPTION_RANDOM, OPTION_RANDOM_SEED, OPTION_RANDOM_SEED_METHOD
+
 from .utils import ensure, topologicalSort, DataGenError, deprecated, split_list_matching_condition
 from . _version import _get_spark_version
 from .schema_parser import SchemaParser
 
 _OLD_MIN_OPTION = 'min'
 _OLD_MAX_OPTION = 'max'
 
@@ -36,14 +38,15 @@
     :param startingId: = starting value for generated seed column
     :param randomSeed: = seed for random number generator
     :param partitions: = number of partitions to generate, if not provided, uses `spark.sparkContext.defaultParallelism`
     :param verbose: = if `True`, generate verbose output
     :param batchSize: = UDF batch number of rows to pass via Apache Arrow to Pandas UDFs
     :param debug: = if set to True, output debug level of information
     :param seedColumnName: = if set, this should be the name of the `seed` or logical `id` column. Defaults to `id`
+    :param random: = if set, specifies default value of `random` attribute for all columns where not set
 
     By default the seed column is named `id`. If you need to use this column name in your generated data,
     it is recommended that you use a different name for the seed column - for example `_id`.
 
     This may be specified by setting the `seedColumnName` attribute to `_id`
     """
 
@@ -59,14 +62,15 @@
     # restrict spurious messages from java gateway
     logging.getLogger("py4j").setLevel(logging.WARNING)
     #logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.NOTSET)
 
     def __init__(self, sparkSession=None, name=None, randomSeedMethod=None,
                  rows=1000000, startingId=0, randomSeed=None, partitions=None, verbose=False,
                  batchSize=None, debug=False, seedColumnName=DEFAULT_SEED_COLUMN,
+                 random=False,
                  **kwargs):
         """ Constructor for data generator object """
 
         # set up logging
         self.verbose = verbose
         self.debug = debug
 
@@ -115,14 +119,17 @@
             self.logger.warning("option 'usePandas' is deprecated - Pandas will always be used")
 
         if "generateWithSelects" in kwargs or "generateWithSelects" in kwargs:
             self.logger.warning("option 'generateWithSelects' switch is deprecated - selects will always be used")
 
         self._seedMethod = randomSeedMethod
 
+        # set default random setting
+        self._defaultRandom = random if random is not None else False
+
         if randomSeed is None:
             self._instanceRandomSeed = self._randomSeed
 
             if randomSeedMethod is None:
                 self._seedMethod = RANDOM_SEED_HASH_FIELD_NAME
             else:
                 self._seedMethod = randomSeedMethod
@@ -234,21 +241,22 @@
         """ set seed for random number generation
 
             Arguments:
             :param seedVal: - new value for the random number seed
         """
         cls._randomSeed = seedVal
 
-    @deprecated('Use `useSeed` instead')
+    @deprecated("Use `useSeed` instead")
     @classmethod
     def use_seed(cls, seedVal):
         """ set seed for random number generation
 
             Arguments:
             :param seedVal: - new value for the random number seed
+
         """
         cls._randomSeed = seedVal
 
     @classmethod
     def reset(cls):
         """ reset any state associated with the data """
         cls._nextNameIndex = 0
@@ -292,14 +300,21 @@
         return new_copy
 
     @property
     def randomSeed(self):
         """ return the data generation spec random seed"""
         return self._instanceRandomSeed
 
+    @property
+    def random(self):
+        """ return the data generation spec default random setting for columns to be used
+            when an explicit `random` attribute setting is not supplied
+        """
+        return self._defaultRandom
+
     def _markForPlanRegen(self):
         """Mark that build plan needs to be regenerated
 
         :returns: modified in-place instance of test data generator allowing for chaining of calls following
                   Builder pattern
         """
         self.buildPlanComputed = False
@@ -586,21 +601,27 @@
                          that match the column names. May be omitted.
         :param fields: a string specifying an explicit field to match , or a list of strings specifying
                        explicit fields to match. May be omitted.
         :param matchTypes: a single Spark SQL datatype or list of Spark SQL data types to match. May be omitted.
         :returns: modified in-place instance of test data generator allowing for chaining of calls following
                   Builder pattern
 
+        .. note::
+           matchTypes may also take SQL type strings or a list of SQL type strings such as "array<integer>"
+
         You may also add a variety of options to further control the test data generation process.
         For full list of options, see :doc:`/reference/api/dbldatagen.column_spec_options`.
 
         """
         if fields is not None and type(fields) is str:
             fields = [fields]
 
+        if OPTION_RANDOM not in kwargs:
+            kwargs[OPTION_RANDOM] = self._defaultRandom
+
         # add support for deprecated legacy names
         if "match_types" in kwargs:
             assert matchTypes is None, "Argument 'match_types' is deprecated, use 'matchTypes' instead"
             matchTypes = kwargs["match_types"]
             del kwargs["match_types"]  # remove the legacy option from keyword args as they will be used later
 
         if matchTypes is not None and type(matchTypes) is not list:
@@ -615,15 +636,23 @@
         effective_fields = [x for x in all_fields if
                             (fields is None or x in fields) and x != self._seedColumnName]
 
         if patterns is not None:
             effective_fields = [x for x in effective_fields for y in patterns if re.search(y, x) is not None]
 
         if matchTypes is not None:
-            effective_fields = [x for x in effective_fields for y in matchTypes
+            effective_types = []
+
+            for typ in matchTypes:
+                if isinstance(typ, str):
+                    effective_types.append(SchemaParser.columnTypeFromString(typ))
+                else:
+                    effective_types.append(typ)
+
+            effective_fields = [x for x in effective_fields for y in effective_types
                                 if self.getColumnType(x) == y]
 
         for f in effective_fields:
             self.withColumnSpec(f, implicit=True, **kwargs)
         return self
 
     def _checkColumnOrColumnList(self, columns, allowId=False):
@@ -643,15 +672,15 @@
                        f" column `{column}` must refer to defined column")
         else:
             ensure(columns in inferred_columns,
                    f" column `{columns}` must refer to defined column")
         return True
 
     def withColumnSpec(self, colName, minValue=None, maxValue=None, step=1, prefix=None,
-                       random=False, distribution=None,
+                       random=None, distribution=None,
                        implicit=False, dataRange=None, omit=False, baseColumn=None, **kwargs):
         """ add a column specification for an existing column
 
         :returns: modified in-place instance of test data generator allowing for chaining of calls
                   following Builder pattern
 
         You may also add a variety of options to further control the test data generation process.
@@ -665,14 +694,17 @@
         ensure(not self.isFieldExplicitlyDefined(colName), f"duplicate column spec for column `{colName}`")
 
         ensure(not isinstance(minValue, DataType),
                f"""unnecessary `datatype` argument specified for `withColumnSpec` for column `{colName}` -
                     Datatype parameter is only needed for `withColumn` and not permitted for `withColumnSpec`
                """)
 
+        if random is None:
+            random = self._defaultRandom
+
         # handle migration of old `min` and `max` options
         if _OLD_MIN_OPTION in kwargs:
             assert minValue is None, \
                 "Only one of `minValue` and `minValue` can be specified. Use of `minValue` is preferred"
             minValue = kwargs[_OLD_MIN_OPTION]
             kwargs.pop(_OLD_MIN_OPTION, None)
 
@@ -700,15 +732,15 @@
 
         :param colName: name of column to check for
         :returns: True if column has spec, False otherwise
         """
         return colName in self._columnSpecsByName
 
     def withColumn(self, colName, colType=StringType(), minValue=None, maxValue=None, step=1,
-                   dataRange=None, prefix=None, random=False, distribution=None,
+                   dataRange=None, prefix=None, random=None, distribution=None,
                    baseColumn=None, nullable=True,
                    omit=False, implicit=False, noWarn=False,
                    **kwargs):
         """ add a new column to the synthetic data generation specification
 
         :param colName: Name of column to add. If this conflicts with the underlying seed column (`id`), it is
                         recommended that the seed column name is customized during the construction of the data
@@ -751,14 +783,17 @@
 
         if _OLD_MAX_OPTION in kwargs:
             assert maxValue is None, \
                 "Only one of `maxValue` and `maxValue` can be specified. Use of `maxValue` is preferred"
             maxValue = kwargs[_OLD_MAX_OPTION]
             kwargs.pop(_OLD_MAX_OPTION, None)
 
+        if random is None:
+            random = self._defaultRandom
+
         new_props = {}
         new_props.update(kwargs)
 
         if type(colType) == str:
             colType = SchemaParser.columnTypeFromString(colType)
 
         self.logger.info("effective range: %s, %s, %s args: %s", minValue, maxValue, step, kwargs)
@@ -787,33 +822,33 @@
 
         new_props = {}
         new_props.update(kwargs)
 
         # if the column  has the option `random` set to true
         # then use the instance level random seed
         # otherwise use the default random seed for the class
-        if "randomSeed" in new_props:
-            effective_random_seed = new_props["randomSeed"]
-            new_props.pop("randomSeed")
-            new_props["random"] = True
+        if OPTION_RANDOM_SEED in new_props:
+            effective_random_seed = new_props[OPTION_RANDOM_SEED]
+            new_props.pop(OPTION_RANDOM_SEED)
+            new_props[OPTION_RANDOM] = True
 
             # if random seed has override but randomSeedMethod does not
             # set it to fixed
-            if "randomSeedMethod" not in new_props:
-                new_props["randomSeedMethod"] = RANDOM_SEED_FIXED
+            if OPTION_RANDOM_SEED_METHOD not in new_props:
+                new_props[OPTION_RANDOM_SEED_METHOD] = RANDOM_SEED_FIXED
 
-        elif "random" in new_props and new_props["random"]:
+        elif OPTION_RANDOM in new_props and new_props[OPTION_RANDOM]:
             effective_random_seed = self._instanceRandomSeed
         else:
             effective_random_seed = self._randomSeed
 
         # handle column level override
-        if "randomSeedMethod" in new_props:
-            effective_random_seed_method = new_props["randomSeedMethod"]
-            new_props.pop("randomSeedMethod")
+        if OPTION_RANDOM_SEED_METHOD in new_props:
+            effective_random_seed_method = new_props[OPTION_RANDOM_SEED_METHOD]
+            new_props.pop(OPTION_RANDOM_SEED_METHOD)
         else:
             effective_random_seed_method = self._seedMethod
 
         column_spec = ColumnGenerationSpec(colName, colType,
                                            baseColumn=baseColumn,
                                            implicit=implicit,
                                            omit=omit,
```

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/datagen_constants.py` & `dbldatagen-0.3.4/dbldatagen/datagen_constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,7 +32,12 @@
 # this is the column name produced by `spark.range`
 # dont change unless semantics of `spark.range` changes
 SPARK_RANGE_COLUMN = "id"
 
 # minimum versions for version checks
 MIN_PYTHON_VERSION = (3, 8)
 MIN_SPARK_VERSION = (3, 1, 2)
+
+# options for randon data generation
+OPTION_RANDOM = "random"
+OPTION_RANDOM_SEED_METHOD = "randomSeedMethod"
+OPTION_RANDOM_SEED = "randomSeed"
```

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/datarange.py` & `dbldatagen-0.3.4/dbldatagen/datarange.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/daterange.py` & `dbldatagen-0.3.4/dbldatagen/daterange.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/distributions/__init__.py` & `dbldatagen-0.3.4/dbldatagen/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/distributions/beta.py` & `dbldatagen-0.3.4/dbldatagen/distributions/beta.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/distributions/data_distribution.py` & `dbldatagen-0.3.4/dbldatagen/distributions/data_distribution.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/distributions/exponential_distribution.py` & `dbldatagen-0.3.4/dbldatagen/distributions/exponential_distribution.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/distributions/gamma.py` & `dbldatagen-0.3.4/dbldatagen/distributions/gamma.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/distributions/normal_distribution.py` & `dbldatagen-0.3.4/dbldatagen/distributions/normal_distribution.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/function_builder.py` & `dbldatagen-0.3.4/dbldatagen/function_builder.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/nrange.py` & `dbldatagen-0.3.4/dbldatagen/nrange.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/schema_parser.py` & `dbldatagen-0.3.4/dbldatagen/schema_parser.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/spark_singleton.py` & `dbldatagen-0.3.4/dbldatagen/spark_singleton.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/text_generator_plugins.py` & `dbldatagen-0.3.4/dbldatagen/text_generator_plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     class _FnCallContext:
         """ inner class to support storage of context between calls
 
             initial instances of random number generators, clients for services etc here during execution
             of the `initFn` calls
 
             :param txtGen: - reference to outer PyfnText object
+
         """
 
         def __init__(self, txtGen):
             self.textGenerator = txtGen
 
     def __init__(self, fn, init=None, initPerBatch=False, name=None, rootProperty=None):
         super().__init__()
@@ -181,15 +182,16 @@
                                    name="FakerText"))
 
     """
 
     def __init__(self, name=None):
         """
 
-        :param name:
+        :param name: name of generated object (when converted to string via ``str``)
+
         """
         self._initFn = None
         self._rootProperty = None
         self._name = "PyfuncText" if name is None else name
         self._initPerBatch = False
 
     def withInit(self, fn):
@@ -369,14 +371,15 @@
     """Generate faker text generator object using default FakerTextFactory
        instance
 
        :param mname: method name to invoke
        :param args: positional args to be passed to underlying Faker instance
        :param _lib: internal only param - library to load
        :param _rootClass: internal only param - root class to create
+       
        :returns : instance of PyfuncText for use with Faker
 
        ``fakerText("sentence")`` is same as ``FakerTextFactory()("sentence")``
     """
     defaultFactory = FakerTextFactory._getDefaultFactory(lib=_lib,
                                                          rootClass=_rootClass)
     return defaultFactory(mname, *args, **kwargs)  # pylint: disable=not-callable
```

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/text_generators.py` & `dbldatagen-0.3.4/dbldatagen/text_generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,32 +174,32 @@
     VINs, IBANs and many other structured codes.
 
     The base value is passed to the template generation and may be used in the generated text. The base value is the
     value the column would have if the template generation had not been applied.
 
     It uses the following special chars:
 
-    ========   ======================================
-    Chars      Meaning
-    ========   ======================================
-    ``\\``     Apply escape to next char.
-    v0,v1,..v9 Use base value as an array of values and substitute the `nth` element ( 0 .. 9). Always escaped.
-    x          Insert a random lowercase hex digit
-    X          Insert an uppercase random hex digit
-    d          Insert a random lowercase decimal digit
-    D          Insert an uppercase random decimal digit
-    a          Insert a random lowercase alphabetical character
-    A          Insert a random uppercase alphabetical character
-    k          Insert a random lowercase alphanumeric character
-    K          Insert a random uppercase alphanumeric character
-    n          Insert a random number between 0 .. 255 inclusive. This option must always be escaped
-    N          Insert a random number between 0 .. 65535 inclusive. This option must always be escaped
-    w          Insert a random lowercase word from the ipsum lorem word set. Always escaped
-    W          Insert a random uppercase word from the ipsum lorem word set. Always escaped
-    ========   ======================================
+    ==========  ======================================
+    Chars       Meaning
+    ==========  ======================================
+    ``\\``       Apply escape to next char.
+    v0,v1,..v9  Use base value as an array of values and substitute the `nth` element ( 0 .. 9). Always escaped.
+    x           Insert a random lowercase hex digit
+    X           Insert an uppercase random hex digit
+    d           Insert a random lowercase decimal digit
+    D           Insert an uppercase random decimal digit
+    a           Insert a random lowercase alphabetical character
+    A           Insert a random uppercase alphabetical character
+    k           Insert a random lowercase alphanumeric character
+    K           Insert a random uppercase alphanumeric character
+    n           Insert a random number between 0 .. 255 inclusive. This option must always be escaped
+    N           Insert a random number between 0 .. 65535 inclusive. This option must always be escaped
+    w           Insert a random lowercase word from the ipsum lorem word set. Always escaped
+    W           Insert a random uppercase word from the ipsum lorem word set. Always escaped
+    ==========  ======================================
 
     .. note::
               If escape is used and`escapeSpecialChars` is False, then the following
               char is assumed to have no special meaning.
 
               If the `escapeSpecialChars` option is set to True, then the following char only has its special
               meaning when preceded by an escape.
@@ -286,20 +286,14 @@
 
         # get the template metadata - this will be list of metadata entries for each template
         # for each template, metadata will be tuple of number of placeholders followed by list of random bounds
         # to be computed when replacing non static placeholder
         template_info = [self._prepareTemplateStrings(template, escapeSpecialMeaning=escapeSpecialChars)
                                     for template in self._templates]
 
-        logger = logging.getLogger(__name__)
-
-        #if logger.isEnabledFor(logging.DEBUG):
-        for ix, ti in template_info:
-            logger.info(f"templates - {ix} {ti}")
-
         self._max_placeholders = max([ x[0] for x in template_info])  # pylint: disable=consider-using-generator
         self._max_rnds_needed = max([ len(x[1]) for x in template_info])  # pylint: disable=consider-using-generator
         self._placeholders_needed = [ x[0] for x in template_info]
         self._template_rnd_bounds = [ x[1] for x in template_info]
 
     def __repr__(self):
         return f"TemplateGenerator(template='{self._template}')"
```

### Comparing `dbldatagen-0.3.3.post2/dbldatagen/utils.py` & `dbldatagen-0.3.4/dbldatagen/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 import functools
 import warnings
 from datetime import timedelta
 import re
 
 
 def deprecated(message=""):
-    ''' Define a deprecated decorator without dependencies on 3rd party libraries
+    """ Define a deprecated decorator without dependencies on 3rd party libraries
 
     Note there is a 3rd party library called `deprecated` that provides this feature but goal is to only have
     dependencies on packages already used in the Databricks runtime
-    '''
+    """
+
+    # create closure around function that follows use of the decorator
 
     def deprecated_decorator(func):
         @functools.wraps(func)
         def deprecated_func(*args, **kwargs):
             warnings.warn(f"`{func.__name__}` is a deprecated function or method. \n{message}",
                           category=DeprecationWarning, stacklevel=1)
             warnings.simplefilter('default', DeprecationWarning)
@@ -110,57 +112,72 @@
 
     The column generation dependencies are based on the value of the `baseColumn` attribute for `withColumn` or
     `withColumnSpec` statements in the data generator specification.
 
     :arg sources: list of ``(name, set(names of dependencies))`` pairs
     :arg initial_columns: force ``initial_columns`` to be computed first
     :arg flatten: if true, flatten output list
-    :returns: list of names in dependency order. If not flattened, result will be list of lists
+    :returns: list of names in dependency order separated into build phases
+
+    .. note::
+       The algorith will give preference to retaining order of inbound sequence
+       over modifying order to produce a lower number of build phases.
+
+       Overall the effect is that the input build order should be retained unless there are forward references
     """
     # generate a copy so that we can modify in place
     pending = [(name, set(deps)) for name, deps in sources]
     provided = [] if initial_columns is None else initial_columns[:]
     build_orders = [] if initial_columns is None else [initial_columns]
 
     while pending:
         next_pending = []
         gen = []
         value_emitted = False
+        defer_emitted = False
         gen_provided = []
         for entry in pending:
             name, deps = entry
             deps.difference_update(provided)
             if deps:
                 next_pending.append((name, set(deps)))
+
+                # if dependencies will be satisfied by item emitted in this round, defer output
+                if not deps.difference(gen_provided):
+                    defer_emitted = True
+            elif defer_emitted:
+                next_pending.append((name, set(deps)))
             elif name in provided:
-                value_emitted |= True
+                value_emitted = True
             else:
                 gen.append(name)
                 gen_provided.append(name)
-                value_emitted |= True
+                value_emitted = True
         provided.extend(gen_provided)
         build_orders.append(gen)
+
         if not value_emitted:
             raise ValueError(f"cyclic or missing dependency detected [{next_pending}]")
 
         pending = next_pending
 
     if flatten:
-        return [item for sublist in build_orders for item in sublist]
+        flattened_list = [item for sublist in build_orders for item in sublist]
+        return flattened_list
     else:
         return build_orders
 
 
 PATTERN_NAME_EQUALS_VALUE = re.compile(r"(\w+)\s*\=\s*([0-9]+)")
 PATTERN_VALUE_SPACE_NAME = re.compile(r"([0-9]+)\s+(\w+)")
 _WEEKS_PER_YEAR = 52
 
 
 def parse_time_interval(spec):
-    '''parse time interval from string'''
+    """parse time interval from string"""
     hours = 0
     minutes = 0
     weeks = 0
     microseconds = 0
     milliseconds = 0
     seconds = 0
     years = 0
@@ -213,18 +230,55 @@
         hours=hours,
         weeks=weeks + (years * _WEEKS_PER_YEAR)
     )
 
     return delta
 
 
+def strip_margins(s, marginChar):
+    """
+    Python equivalent of Scala stripMargins method
+    
+    Takes a string (potentially multiline) and strips all chars up and including the first occurrence of `marginChar`.
+    Used to control the formatting of generated text
+
+    `strip_margins("one\n    |two\n    |three", '|')`
+
+    will produce 
+    
+    ``
+    one 
+    two
+    three
+    ``
+
+    :param s: string to strip margins from
+    :param marginChar: character to strip 
+    :return: modified string
+    """
+    assert s is not None and type(s) is str
+    assert marginChar is not None and type(marginChar) is str
+
+    lines = s.split('\n')
+    revised_lines = []
+
+    for line in lines:
+        if marginChar in line:
+            revised_line = line[line.index(marginChar) + 1:]
+            revised_lines.append(revised_line)
+        else:
+            revised_lines.append(line)
+
+    return '\n'.join(revised_lines)
+
+
 def split_list_matching_condition(lst, cond):
     """ Split a list on elements that match a condition
 
-    This will find all matches of a specific condition in the list and split the list into sublists around the
+    This will find all matches of a specific condition in the list and split the list into sub lists around the
     element that matches this condition.
 
     It will handle multiple matches performing splits on each match.
 
     For example, the following code will produce the results below:
 
     x = ['id', 'city_name', 'id', 'city_id', 'city_pop', 'id', 'city_id', 'city_pop','city_id', 'city_pop','id']
@@ -235,29 +289,27 @@
     `[['id'], ['city_name'], ['id'], ['city_id', 'city_pop'],
      ['id'], ['city_id', 'city_pop', 'city_id', 'city_pop'], ['id']]`
 
     :arg lst: list of items to perform condition matches against
     :arg cond: lambda function or function taking single argument and returning True or False
     :returns: list of sublists
     """
+    retval = []
 
     def match_condition(matchList, matchFn):
         """Return first index of element of list matching condition"""
         if matchList is None or len(matchList) == 0:
             return -1
 
         for i, matchValue in enumerate(matchList):
             if matchFn(matchValue):
                 return i
 
         return -1
 
-    # main code
-    retval = []
-
     if lst is None:
         retval = lst
     elif len(lst) == 1:
         retval = [lst]
     else:
         ix = match_condition(lst, cond)
         if ix != -1:
```

### Comparing `dbldatagen-0.3.3.post2/dbldatagen.egg-info/PKG-INFO` & `dbldatagen-0.3.4/dbldatagen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbldatagen
-Version: 0.3.3.post2
+Version: 0.3.4
 Summary: Databricks Labs -  PySpark Synthetic Data Generator
 Home-page: https://github.com/databrickslabs/data-generator
 Author: Ronan Stokes, Databricks
 License: Databricks License
 Project-URL: Databricks Labs, https://www.databricks.com/learn/labs
 Project-URL: Documentation, https://databrickslabs.github.io/dbldatagen/public_docs/index.html
 Classifier: Programming Language :: Python :: 3
@@ -27,89 +27,90 @@
 
 <!-- 
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/databrickslabs/dbldatagen.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/databrickslabs/dbldatagen/context:python)
 [![downloads](https://img.shields.io/github/downloads/databrickslabs/dbldatagen/total.svg)](https://hanadigital.github.io/grev/?user=databrickslabs&repo=dbldatagen)
 -->
 
 ## Project Description
-The `dbldatgen` Databricks Labs project is a Python library for generating synthetic data within the Databricks 
-environment using Spark. The generated data may be used for testing, benchmarking, demos and many 
+The `dbldatagen` Databricks Labs project is a Python library for generating synthetic data within the Databricks 
+environment using Spark. The generated data may be used for testing, benchmarking, demos, and many 
 other uses.
 
 It operates by defining a data generation specification in code that controls 
-how the synthetic data is to be generated.
-The specification may incorporate use of existing schemas, or create data in an adhoc fashion.
+how the synthetic data is generated.
+The specification may incorporate the use of existing schemas or create data in an ad-hoc fashion.
 
-It has no dependencies on any libraries that are not already incuded in the Databricks 
+It has no dependencies on any libraries that are not already installed in the Databricks 
 runtime, and you can use it from Scala, R or other languages by defining
 a view over the generated data.
 
 ### Feature Summary
 It supports:
 * Generating synthetic data at scale up to billions of rows within minutes using appropriately sized clusters 
-* Generating repeatable, predictable data supporting the needs for producing multiple tables, Change Data Capture, 
+* Generating repeatable, predictable data supporting the need for producing multiple tables, Change Data Capture, 
 merge and join scenarios with consistency between primary and foreign keys
 * Generating synthetic data for all of the 
 Spark SQL supported primitive types as a Spark data frame which may be persisted, 
 saved to external storage or 
 used in other computations
-* Generating ranges of dates, timestamps and numeric values
+* Generating ranges of dates, timestamps, and numeric values
 * Generation of discrete values - both numeric and text
 * Generation of values at random and based on the values of other fields 
 (either based on the `hash` of the underlying values or the values themselves)
 * Ability to specify a distribution for random data generation 
-* Generating arrays of values for ML style feature arrays
+* Generating arrays of values for ML-style feature arrays
 * Applying weights to the occurrence of values
 * Generating values to conform to a schema or independent of an existing schema
-* use of SQL expressions in test data generation
+* use of SQL expressions in synthetic data generation
 * plugin mechanism to allow use of 3rd party libraries such as Faker
 * Use within a Databricks Delta Live Tables pipeline as a synthetic data generation source
+* Generate synthetic data generation code from existing schema or data (experimental)
 
 Details of these features can be found in the online documentation  -
  [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html). 
 
 ## Documentation
 
 Please refer to the [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html) for 
 details of use and many examples.
 
 Release notes and details of the latest changes for this specific release
-can be found in the Github repository
-[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.3post2/CHANGELOG.md)
+can be found in the GitHub repository
+[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.4/CHANGELOG.md)
 
 # Installation
 
-Use `pip install dbldatagen` to install the PyPi package
+Use `pip install dbldatagen` to install the PyPi package.
 
 Within a Databricks notebook, invoke the following in a notebook cell
 ```commandline
 %pip install dbldatagen
 ```
 
-This can be invoked within a Databricks notebook, a Delta Live Tables pipeline and even works on the Databricks 
-community edition.
+The Pip install command can be invoked within a Databricks notebook, a Delta Live Tables pipeline 
+and even works on the Databricks community edition.
 
 The documentation [installation notes](https://databrickslabs.github.io/dbldatagen/public_docs/installation_notes.html) 
 contains details of installation using alternative mechanisms.
 
 ## Compatibility 
-The Databricks Labs data generator framework can be used with Pyspark 3.1.2 and Python 3.8 or later. These are 
+The Databricks Labs Data Generator framework can be used with Pyspark 3.1.2 and Python 3.8 or later. These are 
 compatible with the Databricks runtime 9.1 LTS and later releases.
 
 Older prebuilt releases are tested against Pyspark 3.0.1 (compatible with the Databricks runtime 7.3 LTS 
 or later) and built with Python 3.7.5
 
 For full library compatibility for a specific Databricks Spark release, see the Databricks 
 release notes for library compatibility
 
 - https://docs.databricks.com/release-notes/runtime/releases.html
 
-When using the Databricks Labs Data Generator on Unity Catalog enabled environments, the Data Generator requires
+When using the Databricks Labs Data Generator on "Unity Catalog" enabled environments, the Data Generator requires
 the use of `Single User` or `No Isolation Shared` access modes as some needed features are not available in `Shared` 
-mode (for example, use of 3rd party libraries). Depending on settings, `Custom` access mode may be supported.
+mode (for example, use of 3rd party libraries). Depending on settings, the `Custom` access mode may be supported.
 
 See the following documentation for more information:
 
 - https://docs.databricks.com/data-governance/unity-catalog/compute.html
 
 ## Using the Data Generator
 To use the data generator, install the library using the `%pip install` method or install the Python wheel directly 
@@ -142,38 +143,38 @@
                             
 df = df_spec.build()
 num_rows=df.count()                          
 ```
 Refer to the [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html) for further 
 examples. 
 
-The Github repository also contains further examples in the examples directory
+The GitHub repository also contains further examples in the examples directory.
 
 ## Spark and Databricks Runtime Compatibility
-The `dbldatagen` package is intended to be compatible with recent LTS versions of the Databricks runtime including 
-older LTS versions at least from 10.4 LTS and later. It also aims to be compatible with Delta Live Table runtimes 
+The `dbldatagen` package is intended to be compatible with recent LTS versions of the Databricks runtime, including 
+older LTS versions at least from 10.4 LTS and later. It also aims to be compatible with Delta Live Table runtimes, 
 including `current` and `preview`. 
 
-While we dont specifically drop support for older runtimes, changes in Pyspark APIs or
-APIs from dependent packages such as `numpy`, `pandas`, `pyarrow` and `pyparsing` make cause issues with older
+While we don't specifically drop support for older runtimes, changes in Pyspark APIs or
+APIs from dependent packages such as `numpy`, `pandas`, `pyarrow`, and `pyparsing` make cause issues with older
 runtimes. 
 
-Installing `dbldatagen` explicitly does not install releases of dependent packages so as to preserve the curated
-set of packages installed in any Databricks runtime environment.
+By design, installing `dbldatagen` does not install releases of dependent packages in order 
+to preserve the curated set of packages pre-installed in any Databricks runtime environment.
 
-When building on local environments, the `Pipfile` and requirements files are used to determine the versions 
-tested against for releases and unit tests. 
+When building on local environments, the build process uses the `Pipfile` and requirements files to determine 
+the package versions for releases and unit tests. 
 
 ## Project Support
 Please note that all projects released under [`Databricks Labs`](https://www.databricks.com/learn/labs)
  are provided for your exploration only, and are not formally supported by Databricks with Service Level Agreements 
-(SLAs).  They are provided AS-IS and we do not make any guarantees of any kind.  Please do not submit a support ticket 
+(SLAs).  They are provided AS-IS, and we do not make any guarantees of any kind.  Please do not submit a support ticket 
 relating to any issues arising from the use of these projects.
 
-Any issues discovered through the use of this project should be filed as issues on the Github Repo.  
+Any issues discovered through the use of this project should be filed as issues on the GitHub Repo.  
 They will be reviewed as time permits, but there are no formal SLAs for support.
 
 
 ## Feedback
 
 Issues with the application?  Found a bug?  Have a great idea for an addition?
 Feel free to file an [issue](https://github.com/databrickslabs/dbldatagen/issues/new).
```

### Comparing `dbldatagen-0.3.3.post2/dbldatagen.egg-info/SOURCES.txt` & `dbldatagen-0.3.4/dbldatagen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.3.post2/setup.py` & `dbldatagen-0.3.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     The Databricks Labs Data Generator can generate realistic synthetic data sets at scale for testing, 
     benchmarking, environment validation and other purposes.
     """
 
 setuptools.setup(
     name="dbldatagen",
-    version="0.3.3post2",
+    version="0.3.4",
     author="Ronan Stokes, Databricks",
     description="Databricks Labs -  PySpark Synthetic Data Generator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/databrickslabs/data-generator",
     project_urls={
         "Databricks Labs": "https://www.databricks.com/learn/labs",
```

