# Comparing `tmp/mmcif-0.80.1.tar.gz` & `tmp/mmcif-0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcif-0.80.1.tar", last modified: Sun Dec  4 17:10:26 2022, max compression
+gzip compressed data, was "mmcif-0.81.tar", last modified: Sat Apr  8 23:44:22 2023, max compression
```

## Comparing `mmcif-0.80.1.tar` & `mmcif-0.81.tar`

### file list

```diff
@@ -1,730 +1,730 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.697708 mmcif-0.80.1/
--rw-r--r--   0 runner     (501) staff       (20)    12721 2022-12-04 17:03:33.000000 mmcif-0.80.1/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     6303 2022-12-04 17:03:33.000000 mmcif-0.80.1/HISTORY.txt
--rw-r--r--   0 runner     (501) staff       (20)      552 2022-12-04 17:03:33.000000 mmcif-0.80.1/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      441 2022-12-04 17:03:33.000000 mmcif-0.80.1/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     2781 2022-12-04 17:10:26.697179 mmcif-0.80.1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2075 2022-12-04 17:03:33.000000 mmcif-0.80.1/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.916639 mmcif-0.80.1/mmcif/
--rw-r--r--   0 runner     (501) staff       (20)      186 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.931821 mmcif-0.80.1/mmcif/api/
--rw-r--r--   0 runner     (501) staff       (20)    21941 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/api/DataCategory.py
--rw-r--r--   0 runner     (501) staff       (20)    17192 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/api/DataCategoryBase.py
--rw-r--r--   0 runner     (501) staff       (20)    13272 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/api/DataCategoryFormatted.py
--rw-r--r--   0 runner     (501) staff       (20)     9789 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/api/DataCategoryTyped.py
--rw-r--r--   0 runner     (501) staff       (20)    10128 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/api/DictMethodRunner.py
--rw-r--r--   0 runner     (501) staff       (20)    85436 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/api/DictionaryApi.py
--rw-r--r--   0 runner     (501) staff       (20)    24778 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/api/DictionaryInclude.py
--rw-r--r--   0 runner     (501) staff       (20)     3844 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/api/Method.py
--rw-r--r--   0 runner     (501) staff       (20)     5017 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/api/MethodUtils.py
--rw-r--r--   0 runner     (501) staff       (20)    10640 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/api/PdbxContainers.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/api/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.932906 mmcif-0.80.1/mmcif/core/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/core/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.973345 mmcif-0.80.1/mmcif/io/
--rw-r--r--   0 runner     (501) staff       (20)    19023 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/io/BinaryCifReader.py
--rw-r--r--   0 runner     (501) staff       (20)    18735 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/io/BinaryCifWriter.py
--rw-r--r--   0 runner     (501) staff       (20)     2922 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/io/BuildDictionaryExec.py
--rw-r--r--   0 runner     (501) staff       (20)     1551 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/io/CifFile.py
--rw-r--r--   0 runner     (501) staff       (20)    12704 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/io/IoAdapterBase.py
--rw-r--r--   0 runner     (501) staff       (20)    18753 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/io/IoAdapterCore.py
--rw-r--r--   0 runner     (501) staff       (20)    13995 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/io/IoAdapterPy.py
--rw-r--r--   0 runner     (501) staff       (20)      524 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/io/PdbxExceptions.py
--rw-r--r--   0 runner     (501) staff       (20)    18397 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/io/PdbxReader.py
--rw-r--r--   0 runner     (501) staff       (20)    11640 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/io/PdbxWriter.py
--rw-r--r--   0 runner     (501) staff       (20)      183 2022-12-04 17:03:33.000000 mmcif-0.80.1/mmcif/io/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.920212 mmcif-0.80.1/mmcif.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2781 2022-12-04 17:10:25.000000 mmcif-0.80.1/mmcif.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    29562 2022-12-04 17:10:25.000000 mmcif-0.80.1/mmcif.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-12-04 17:10:25.000000 mmcif-0.80.1/mmcif.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       69 2022-12-04 17:10:25.000000 mmcif-0.80.1/mmcif.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-12-04 17:04:39.000000 mmcif-0.80.1/mmcif.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)      130 2022-12-04 17:10:25.000000 mmcif-0.80.1/mmcif.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        6 2022-12-04 17:10:25.000000 mmcif-0.80.1/mmcif.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.899639 mmcif-0.80.1/modules/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.883452 mmcif-0.80.1/modules/cc-regex/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.980817 mmcif-0.80.1/modules/cc-regex/include/
--rw-r--r--   0 runner     (501) staff       (20)      943 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cc-regex/include/cclass.h
--rw-r--r--   0 runner     (501) staff       (20)     2057 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cc-regex/include/cname.h
--rw-r--r--   0 runner     (501) staff       (20)      329 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cc-regex/include/debug.ih
--rw-r--r--   0 runner     (501) staff       (20)     1379 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cc-regex/include/engine.ih
--rw-r--r--   0 runner     (501) staff       (20)      500 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cc-regex/include/main.ih
--rw-r--r--   0 runner     (501) staff       (20)     2723 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cc-regex/include/regcomp.ih
--rw-r--r--   0 runner     (501) staff       (20)      267 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cc-regex/include/regerror.ih
--rw-r--r--   0 runner     (501) staff       (20)     1891 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cc-regex/include/regex.h
--rw-r--r--   0 runner     (501) staff       (20)     5365 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cc-regex/include/regex2.h
--rw-r--r--   0 runner     (501) staff       (20)      500 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cc-regex/include/utils.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.986850 mmcif-0.80.1/modules/cc-regex/src/
--rw-r--r--   0 runner     (501) staff       (20)     5092 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cc-regex/src/debug.c
--rw-r--r--   0 runner     (501) staff       (20)    25587 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cc-regex/src/engine.c
--rw-r--r--   0 runner     (501) staff       (20)    11193 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cc-regex/src/main.c
--rw-r--r--   0 runner     (501) staff       (20)     1825 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cc-regex/src/mkh
--rw-r--r--   0 runner     (501) staff       (20)    37342 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cc-regex/src/regcomp.c
--rw-r--r--   0 runner     (501) staff       (20)     3212 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cc-regex/src/regerror.c
--rw-r--r--   0 runner     (501) staff       (20)     4259 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cc-regex/src/regexec.c
--rw-r--r--   0 runner     (501) staff       (20)      736 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cc-regex/src/regfree.c
--rw-r--r--   0 runner     (501) staff       (20)     7061 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cc-regex/src/split.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.885016 mmcif-0.80.1/modules/cpp-cif-file/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.994272 mmcif-0.80.1/modules/cpp-cif-file/include/
--rw-r--r--   0 runner     (501) staff       (20)     1746 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-file/include/CifDataInfo.h
--rw-r--r--   0 runner     (501) staff       (20)      617 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-file/include/CifExcept.h
--rw-r--r--   0 runner     (501) staff       (20)    23567 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-file/include/CifFile.h
--rw-r--r--   0 runner     (501) staff       (20)     1945 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-file/include/CifParentChild.h
--rw-r--r--   0 runner     (501) staff       (20)     5484 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-file/include/DicFile.h
--rw-r--r--   0 runner     (501) staff       (20)     2782 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-file/include/ParentChild.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.999358 mmcif-0.80.1/modules/cpp-cif-file/src/
--rw-r--r--   0 runner     (501) staff       (20)     6274 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-file/src/CifDataInfo.C
--rw-r--r--   0 runner     (501) staff       (20)    34845 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-file/src/CifExcept.C
--rw-r--r--   0 runner     (501) staff       (20)    85572 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-file/src/CifFile.C
--rw-r--r--   0 runner     (501) staff       (20)    32174 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-file/src/CifParentChild.C
--rw-r--r--   0 runner     (501) staff       (20)    47643 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-file/src/DicFile.C
--rw-r--r--   0 runner     (501) staff       (20)    23231 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-file/src/ParentChild.C
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.884242 mmcif-0.80.1/modules/cpp-cif-file-util/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.988279 mmcif-0.80.1/modules/cpp-cif-file-util/include/
--rw-r--r--   0 runner     (501) staff       (20)     3264 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-file-util/include/CifCorrector.h
--rw-r--r--   0 runner     (501) staff       (20)     2444 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-file-util/include/CifFileUtil.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.989878 mmcif-0.80.1/modules/cpp-cif-file-util/src/
--rw-r--r--   0 runner     (501) staff       (20)    47136 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-file-util/src/CifCorrector.C
--rw-r--r--   0 runner     (501) staff       (20)     4509 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-file-util/src/CifFileUtil.C
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.886006 mmcif-0.80.1/modules/cpp-cif-parser/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.005670 mmcif-0.80.1/modules/cpp-cif-parser/include/
--rw-r--r--   0 runner     (501) staff       (20)     1518 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-parser/include/CifFileReadDef.h
--rw-r--r--   0 runner     (501) staff       (20)     6318 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-parser/include/CifParserBase.h
--rw-r--r--   0 runner     (501) staff       (20)      898 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-parser/include/CifParserInt.h
--rw-r--r--   0 runner     (501) staff       (20)     1390 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-parser/include/CifScannerBase.h
--rw-r--r--   0 runner     (501) staff       (20)      750 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-parser/include/CifScannerInt.h
--rw-r--r--   0 runner     (501) staff       (20)     6970 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-parser/include/DICParserBase.h
--rw-r--r--   0 runner     (501) staff       (20)     1032 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-parser/include/DICParserInt.h
--rw-r--r--   0 runner     (501) staff       (20)     1471 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-parser/include/DICScannerBase.h
--rw-r--r--   0 runner     (501) staff       (20)      912 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-parser/include/DICScannerInt.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.014582 mmcif-0.80.1/modules/cpp-cif-parser/src/
--rw-r--r--   0 runner     (501) staff       (20)     3768 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-parser/src/CifFileReadDef.C
--rw-r--r--   0 runner     (501) staff       (20)     2206 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-parser/src/CifParser.y
--rw-r--r--   0 runner     (501) staff       (20)    23419 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-parser/src/CifParserBase.C
--rw-r--r--   0 runner     (501) staff       (20)     2475 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-parser/src/CifScanner.l
--rw-r--r--   0 runner     (501) staff       (20)     9603 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-parser/src/CifScannerBase.C
--rw-r--r--   0 runner     (501) staff       (20)     2376 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-parser/src/DICParser.y
--rw-r--r--   0 runner     (501) staff       (20)    41071 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-parser/src/DICParserBase.C
--rw-r--r--   0 runner     (501) staff       (20)     2985 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-parser/src/DICScanner.l
--rw-r--r--   0 runner     (501) staff       (20)    10258 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-cif-parser/src/DICScannerBase.C
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.886778 mmcif-0.80.1/modules/cpp-common/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.026530 mmcif-0.80.1/modules/cpp-common/include/
--rw-r--r--   0 runner     (501) staff       (20)      520 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/include/BlockIO.h
--rwxr-xr-x   0 runner     (501) staff       (20)     2398 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/include/CifDefs.h
--rw-r--r--   0 runner     (501) staff       (20)     6737 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/include/CifString.h
--rw-r--r--   0 runner     (501) staff       (20)     2901 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/include/DataInfo.h
--rw-r--r--   0 runner     (501) staff       (20)     3175 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/include/Exceptions.h
--rw-r--r--   0 runner     (501) staff       (20)      635 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/include/GenCont.h
--rw-r--r--   0 runner     (501) staff       (20)     6109 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/include/GenString.h
--rw-r--r--   0 runner     (501) staff       (20)      484 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/include/RcsbFile.h
--rw-r--r--   0 runner     (501) staff       (20)      335 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/include/RcsbPlatform.h
--rw-r--r--   0 runner     (501) staff       (20)     5664 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/include/Serializer.h
--rw-r--r--   0 runner     (501) staff       (20)     2665 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/include/mapped_ptr_vector.h
--rw-r--r--   0 runner     (501) staff       (20)     1543 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/include/mapped_vector.h
--rw-r--r--   0 runner     (501) staff       (20)      210 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/include/rcsb_math.h
--rw-r--r--   0 runner     (501) staff       (20)      617 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/include/rcsb_types.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.034274 mmcif-0.80.1/modules/cpp-common/src/
--rw-r--r--   0 runner     (501) staff       (20)     1240 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/src/BlockIO.C
--rw-r--r--   0 runner     (501) staff       (20)    10498 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/src/CifString.C
--rw-r--r--   0 runner     (501) staff       (20)     9606 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/src/DataInfo.C
--rw-r--r--   0 runner     (501) staff       (20)     2314 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/src/Exceptions.C
--rwxr-xr-x   0 runner     (501) staff       (20)     1085 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/src/GenCont.C
--rw-r--r--   0 runner     (501) staff       (20)    14827 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/src/GenString.C
--rwxr-xr-x   0 runner     (501) staff       (20)     1236 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/src/RcsbFile.C
--rwxr-xr-x   0 runner     (501) staff       (20)      356 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/src/RcsbPlatform.C
--rwxr-xr-x   0 runner     (501) staff       (20)    40038 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/src/Serializer.C
--rw-r--r--   0 runner     (501) staff       (20)    10675 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/src/mapped_ptr_vector.C
--rw-r--r--   0 runner     (501) staff       (20)     5759 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-common/src/mapped_vector.C
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.887322 mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.041091 mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/
--rw-r--r--   0 runner     (501) staff       (20)     2072 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifDataInfo.cpp
--rw-r--r--   0 runner     (501) staff       (20)    12223 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFile.cpp
--rw-r--r--   0 runner     (501) staff       (20)     3130 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFileReadDef.cpp
--rw-r--r--   0 runner     (501) staff       (20)     3592 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFileUtil.cpp
--rw-r--r--   0 runner     (501) staff       (20)     3791 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wrapDicFile.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2003 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wrapDictDataInfo.cpp
--rw-r--r--   0 runner     (501) staff       (20)    14081 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wrapISTable.cpp
--rw-r--r--   0 runner     (501) staff       (20)     6137 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wrapTableFile.cpp
--rw-r--r--   0 runner     (501) staff       (20)      690 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wrapmmciflib.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1017 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wraprcsb_types.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.889103 mmcif-0.80.1/modules/cpp-dict-obj-file/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.044675 mmcif-0.80.1/modules/cpp-dict-obj-file/include/
--rw-r--r--   0 runner     (501) staff       (20)     1437 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-dict-obj-file/include/DictDataInfo.h
--rw-r--r--   0 runner     (501) staff       (20)     7726 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-dict-obj-file/include/DictObjCont.h
--rw-r--r--   0 runner     (501) staff       (20)     4564 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-dict-obj-file/include/DictObjContInfo.h
--rw-r--r--   0 runner     (501) staff       (20)     5597 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-dict-obj-file/include/DictObjFile.h
--rw-r--r--   0 runner     (501) staff       (20)      876 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-dict-obj-file/include/DictParentChild.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.054098 mmcif-0.80.1/modules/cpp-dict-obj-file/src/
--rw-r--r--   0 runner     (501) staff       (20)     3975 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-dict-obj-file/src/DictDataInfo.C
--rw-r--r--   0 runner     (501) staff       (20)    19477 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-dict-obj-file/src/DictObjCont.C
--rw-r--r--   0 runner     (501) staff       (20)    12717 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-dict-obj-file/src/DictObjContInfo.C
--rw-r--r--   0 runner     (501) staff       (20)     6349 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-dict-obj-file/src/DictObjFile.C
--rw-r--r--   0 runner     (501) staff       (20)     1979 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-dict-obj-file/src/DictObjFileCreator.C
--rw-r--r--   0 runner     (501) staff       (20)      741 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-dict-obj-file/src/DictObjFileReader.C
--rw-r--r--   0 runner     (501) staff       (20)    13027 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-dict-obj-file/src/DictObjFileSelectiveReader.C
--rw-r--r--   0 runner     (501) staff       (20)     8311 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-dict-obj-file/src/DictParentChild.C
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.889583 mmcif-0.80.1/modules/cpp-mmciflib-test/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.079176 mmcif-0.80.1/modules/cpp-mmciflib-test/src/
--rwxr-xr-x   0 runner     (501) staff       (20)     1333 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/BigCifTest.C
--rwxr-xr-x   0 runner     (501) staff       (20)     5347 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/CifDiff.C
--rwxr-xr-x   0 runner     (501) staff       (20)     3115 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/CifInfo.C
--rwxr-xr-x   0 runner     (501) staff       (20)     2788 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/CifReader.C
--rwxr-xr-x   0 runner     (501) staff       (20)     2673 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/DataChecking.C
--rwxr-xr-x   0 runner     (501) staff       (20)     1929 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/DictInfo.C
--rwxr-xr-x   0 runner     (501) staff       (20)     1894 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest1.C
--rwxr-xr-x   0 runner     (501) staff       (20)     1073 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest10.C
--rwxr-xr-x   0 runner     (501) staff       (20)     2061 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest11.C
--rwxr-xr-x   0 runner     (501) staff       (20)     2406 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest12.C
--rwxr-xr-x   0 runner     (501) staff       (20)      539 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest13.C
--rwxr-xr-x   0 runner     (501) staff       (20)     3930 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest14.C
--rwxr-xr-x   0 runner     (501) staff       (20)     3211 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest2.C
--rwxr-xr-x   0 runner     (501) staff       (20)     1385 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest3.C
--rwxr-xr-x   0 runner     (501) staff       (20)     2410 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest4.C
--rwxr-xr-x   0 runner     (501) staff       (20)     1417 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest5.C
--rwxr-xr-x   0 runner     (501) staff       (20)     1174 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest6.C
--rwxr-xr-x   0 runner     (501) staff       (20)     1863 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest7.C
--rwxr-xr-x   0 runner     (501) staff       (20)      406 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest8.C
--rwxr-xr-x   0 runner     (501) staff       (20)      611 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest9.C
--rwxr-xr-x   0 runner     (501) staff       (20)     1316 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/GroupTableTest2.C
--rwxr-xr-x   0 runner     (501) staff       (20)      582 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/SdbReader.C
--rwxr-xr-x   0 runner     (501) staff       (20)     1519 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/checkdictionary.C
--rwxr-xr-x   0 runner     (501) staff       (20)      655 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/cpp-mmciflib-test/src/selective-reading.C
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.890549 mmcif-0.80.1/modules/cpp-tables/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.083586 mmcif-0.80.1/modules/cpp-tables/include/
--rw-r--r--   0 runner     (501) staff       (20)    52000 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-tables/include/ISTable.h
--rw-r--r--   0 runner     (501) staff       (20)    44528 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-tables/include/ITTable.h
--rw-r--r--   0 runner     (501) staff       (20)    20019 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-tables/include/TTable.h
--rw-r--r--   0 runner     (501) staff       (20)     1270 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-tables/include/TableError.h
--rw-r--r--   0 runner     (501) staff       (20)    21422 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-tables/include/TableFile.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.086802 mmcif-0.80.1/modules/cpp-tables/src/
--rw-r--r--   0 runner     (501) staff       (20)    77385 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-tables/src/ISTable.C
--rw-r--r--   0 runner     (501) staff       (20)    43788 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-tables/src/ITTable.C
--rw-r--r--   0 runner     (501) staff       (20)    15437 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-tables/src/TTable.C
--rw-r--r--   0 runner     (501) staff       (20)    26031 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/cpp-tables/src/TableFile.C
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.106692 mmcif-0.80.1/modules/pybind11/
--rw-r--r--   0 runner     (501) staff       (20)     1271 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.appveyor.yml
--rw-r--r--   0 runner     (501) staff       (20)      996 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.clang-format
--rw-r--r--   0 runner     (501) staff       (20)     2605 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.clang-tidy
--rw-r--r--   0 runner     (501) staff       (20)     2196 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.cmake-format.yaml
--rw-r--r--   0 runner     (501) staff       (20)     1308 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.codespell-ignore-lines
--rw-r--r--   0 runner     (501) staff       (20)       44 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.git
--rw-r--r--   0 runner     (501) staff       (20)       18 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.gitattributes
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.110667 mmcif-0.80.1/modules/pybind11/.github/
--rw-r--r--   0 runner     (501) staff       (20)      182 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.github/CODEOWNERS
--rw-r--r--   0 runner     (501) staff       (20)    15271 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.111757 mmcif-0.80.1/modules/pybind11/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner     (501) staff       (20)     2016 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner     (501) staff       (20)      328 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner     (501) staff       (20)      162 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.github/dependabot.yml
--rw-r--r--   0 runner     (501) staff       (20)      116 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.github/labeler.yml
--rw-r--r--   0 runner     (501) staff       (20)       50 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.github/labeler_merged.yml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.112285 mmcif-0.80.1/modules/pybind11/.github/matchers/
--rw-r--r--   0 runner     (501) staff       (20)      668 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.github/matchers/pylint.json
--rw-r--r--   0 runner     (501) staff       (20)      645 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.github/pull_request_template.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.115976 mmcif-0.80.1/modules/pybind11/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)    28486 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.github/workflows/ci.yml
--rw-r--r--   0 runner     (501) staff       (20)     2095 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.github/workflows/configure.yml
--rw-r--r--   0 runner     (501) staff       (20)     1419 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.github/workflows/format.yml
--rw-r--r--   0 runner     (501) staff       (20)      333 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.github/workflows/labeler.yml
--rw-r--r--   0 runner     (501) staff       (20)     2558 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.github/workflows/pip.yml
--rw-r--r--   0 runner     (501) staff       (20)     2837 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.github/workflows/upstream.yml
--rw-r--r--   0 runner     (501) staff       (20)      487 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)     4331 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.pre-commit-config.yaml
--rw-r--r--   0 runner     (501) staff       (20)       62 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/.readthedocs.yml
--rw-r--r--   0 runner     (501) staff       (20)    11911 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     1684 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      223 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     7686 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/README.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.130596 mmcif-0.80.1/modules/pybind11/docs/
--rw-r--r--   0 runner     (501) staff       (20)      607 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/Doxyfile
--rw-r--r--   0 runner     (501) staff       (20)     7417 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/Makefile
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.892684 mmcif-0.80.1/modules/pybind11/docs/_static/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.131199 mmcif-0.80.1/modules/pybind11/docs/_static/css/
--rw-r--r--   0 runner     (501) staff       (20)       37 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/_static/css/custom.css
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.134831 mmcif-0.80.1/modules/pybind11/docs/advanced/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.139457 mmcif-0.80.1/modules/pybind11/docs/advanced/cast/
--rw-r--r--   0 runner     (501) staff       (20)     3937 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/advanced/cast/chrono.rst
--rw-r--r--   0 runner     (501) staff       (20)     3429 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/advanced/cast/custom.rst
--rw-r--r--   0 runner     (501) staff       (20)    14283 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/advanced/cast/eigen.rst
--rw-r--r--   0 runner     (501) staff       (20)     3889 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/advanced/cast/functional.rst
--rw-r--r--   0 runner     (501) staff       (20)     1556 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/advanced/cast/index.rst
--rw-r--r--   0 runner     (501) staff       (20)    12371 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/advanced/cast/overview.rst
--rw-r--r--   0 runner     (501) staff       (20)     9586 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/advanced/cast/stl.rst
--rw-r--r--   0 runner     (501) staff       (20)     8863 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/advanced/cast/strings.rst
--rw-r--r--   0 runner     (501) staff       (20)    47796 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/advanced/classes.rst
--rw-r--r--   0 runner     (501) staff       (20)     8453 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/advanced/embedding.rst
--rw-r--r--   0 runner     (501) staff       (20)    17772 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/advanced/exceptions.rst
--rw-r--r--   0 runner     (501) staff       (20)    26729 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/advanced/functions.rst
--rw-r--r--   0 runner     (501) staff       (20)    13634 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/advanced/misc.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.141909 mmcif-0.80.1/modules/pybind11/docs/advanced/pycpp/
--rw-r--r--   0 runner     (501) staff       (20)      278 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/advanced/pycpp/index.rst
--rw-r--r--   0 runner     (501) staff       (20)    17161 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/advanced/pycpp/numpy.rst
--rw-r--r--   0 runner     (501) staff       (20)     9030 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/advanced/pycpp/object.rst
--rw-r--r--   0 runner     (501) staff       (20)     5710 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/advanced/pycpp/utilities.rst
--rw-r--r--   0 runner     (501) staff       (20)     6377 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/advanced/smart_ptrs.rst
--rw-r--r--   0 runner     (501) staff       (20)     9240 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/basics.rst
--rw-r--r--   0 runner     (501) staff       (20)     2856 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/benchmark.py
--rw-r--r--   0 runner     (501) staff       (20)     3168 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/benchmark.rst
--rw-r--r--   0 runner     (501) staff       (20)   111105 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/changelog.rst
--rw-r--r--   0 runner     (501) staff       (20)    16380 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/classes.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.142625 mmcif-0.80.1/modules/pybind11/docs/cmake/
--rw-r--r--   0 runner     (501) staff       (20)      273 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/cmake/index.rst
--rw-r--r--   0 runner     (501) staff       (20)    25777 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/compiling.rst
--rw-r--r--   0 runner     (501) staff       (20)    11559 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/conf.py
--rw-r--r--   0 runner     (501) staff       (20)    13177 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/faq.rst
--rw-r--r--   0 runner     (501) staff       (20)      613 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/index.rst
--rw-r--r--   0 runner     (501) staff       (20)     3277 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/installing.rst
--rw-r--r--   0 runner     (501) staff       (20)     3079 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/limitations.rst
--rw-r--r--   0 runner     (501) staff       (20)    61034 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/pybind11-logo.png
--rw-r--r--   0 runner     (501) staff       (20)    44653 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/pybind11_vs_boost_python1.png
--rw-r--r--   0 runner     (501) staff       (20)    87708 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-r--r--   0 runner     (501) staff       (20)    41121 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/pybind11_vs_boost_python2.png
--rw-r--r--   0 runner     (501) staff       (20)    85853 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-r--r--   0 runner     (501) staff       (20)     2647 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/reference.rst
--rw-r--r--   0 runner     (501) staff       (20)     4414 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/release.rst
--rw-r--r--   0 runner     (501) staff       (20)      149 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/requirements.txt
--rw-r--r--   0 runner     (501) staff       (20)    23489 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/docs/upgrade.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.894192 mmcif-0.80.1/modules/pybind11/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.156057 mmcif-0.80.1/modules/pybind11/include/pybind11/
--rw-r--r--   0 runner     (501) staff       (20)    23979 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner     (501) staff       (20)     7069 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner     (501) staff       (20)    65638 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner     (501) staff       (20)     8458 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner     (501) staff       (20)      120 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner     (501) staff       (20)     2096 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.160992 mmcif-0.80.1/modules/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner     (501) staff       (20)    28251 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner     (501) staff       (20)    50369 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner     (501) staff       (20)     5491 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner     (501) staff       (20)    17981 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner     (501) staff       (20)    25057 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner     (501) staff       (20)    42266 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner     (501) staff       (20)     1625 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner     (501) staff       (20)    32147 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner     (501) staff       (20)    11792 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner     (501) staff       (20)     4731 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner     (501) staff       (20)     4695 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner     (501) staff       (20)     8262 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner     (501) staff       (20)     8862 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner     (501) staff       (20)    79524 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner     (501) staff       (20)     9103 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner     (501) staff       (20)     2181 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner     (501) staff       (20)   125761 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner     (501) staff       (20)    93848 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.161553 mmcif-0.80.1/modules/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner     (501) staff       (20)     4185 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner     (501) staff       (20)    15337 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner     (501) staff       (20)    27013 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 runner     (501) staff       (20)     2765 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/noxfile.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.164967 mmcif-0.80.1/modules/pybind11/pybind11/
--rw-r--r--   0 runner     (501) staff       (20)      414 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/pybind11/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1360 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/pybind11/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)      228 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/pybind11/_version.py
--rw-r--r--   0 runner     (501) staff       (20)     1226 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/pybind11/commands.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/pybind11/py.typed
--rw-r--r--   0 runner     (501) staff       (20)    17609 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0 runner     (501) staff       (20)     1261 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)     1622 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     4877 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.228479 mmcif-0.80.1/modules/pybind11/tests/
--rw-r--r--   0 runner     (501) staff       (20)    20608 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     5006 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/conftest.py
--rw-r--r--   0 runner     (501) staff       (20)    11736 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/constructor_stats.h
--rw-r--r--   0 runner     (501) staff       (20)     3578 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/cross_module_gil_utils.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1776 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/cross_module_interleaved_error_already_set.cpp
--rw-r--r--   0 runner     (501) staff       (20)      940 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/env.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.229980 mmcif-0.80.1/modules/pybind11/tests/extra_python_package/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/extra_python_package/pytest.ini
--rw-r--r--   0 runner     (501) staff       (20)     8142 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/extra_python_package/test_files.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.233227 mmcif-0.80.1/modules/pybind11/tests/extra_setuptools/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/extra_setuptools/pytest.ini
--rw-r--r--   0 runner     (501) staff       (20)     4153 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0 runner     (501) staff       (20)     2847 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/local_bindings.h
--rw-r--r--   0 runner     (501) staff       (20)     5743 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/object.h
--rw-r--r--   0 runner     (501) staff       (20)     6264 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-r--r--   0 runner     (501) staff       (20)     4517 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/pybind11_tests.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2685 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/pybind11_tests.h
--rw-r--r--   0 runner     (501) staff       (20)      768 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/pytest.ini
--rw-r--r--   0 runner     (501) staff       (20)      600 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/requirements.txt
--rw-r--r--   0 runner     (501) staff       (20)      855 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_async.cpp
--rw-r--r--   0 runner     (501) staff       (20)      534 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_async.py
--rw-r--r--   0 runner     (501) staff       (20)     8567 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_buffers.cpp
--rw-r--r--   0 runner     (501) staff       (20)     4841 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_buffers.py
--rw-r--r--   0 runner     (501) staff       (20)    15990 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_builtin_casters.cpp
--rw-r--r--   0 runner     (501) staff       (20)    17245 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_builtin_casters.py
--rw-r--r--   0 runner     (501) staff       (20)     4118 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_call_policies.cpp
--rw-r--r--   0 runner     (501) staff       (20)     6549 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_call_policies.py
--rw-r--r--   0 runner     (501) staff       (20)     9243 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_callbacks.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5906 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_callbacks.py
--rw-r--r--   0 runner     (501) staff       (20)     3370 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_chrono.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5695 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_chrono.py
--rw-r--r--   0 runner     (501) staff       (20)    24803 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_class.cpp
--rw-r--r--   0 runner     (501) staff       (20)    14575 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_class.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.239072 mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner     (501) staff       (20)     2639 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      673 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/embed.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.239697 mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner     (501) staff       (20)     1171 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.240327 mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner     (501) staff       (20)     1293 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.241514 mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner     (501) staff       (20)     1685 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      152 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/main.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.242170 mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner     (501) staff       (20)     1353 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.243003 mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner     (501) staff       (20)     1163 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.243715 mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner     (501) staff       (20)     1368 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      198 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/test.py
--rw-r--r--   0 runner     (501) staff       (20)     3831 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_const_name.cpp
--rw-r--r--   0 runner     (501) staff       (20)      589 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_const_name.py
--rw-r--r--   0 runner     (501) staff       (20)     5853 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_constants_and_functions.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1498 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_constants_and_functions.py
--rw-r--r--   0 runner     (501) staff       (20)    10886 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_copy_move.cpp
--rw-r--r--   0 runner     (501) staff       (20)     4796 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_copy_move.py
--rw-r--r--   0 runner     (501) staff       (20)     7280 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_custom_type_casters.cpp
--rw-r--r--   0 runner     (501) staff       (20)     3980 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_custom_type_casters.py
--rw-r--r--   0 runner     (501) staff       (20)     1259 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_custom_type_setup.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1089 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_custom_type_setup.py
--rw-r--r--   0 runner     (501) staff       (20)     2816 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_docstring_options.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1606 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_docstring_options.py
--rw-r--r--   0 runner     (501) staff       (20)    19409 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_eigen.cpp
--rw-r--r--   0 runner     (501) staff       (20)    28860 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_eigen.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.249153 mmcif-0.80.1/modules/pybind11/tests/test_embed/
--rw-r--r--   0 runner     (501) staff       (20)     1798 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_embed/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     1338 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_embed/catch.cpp
--rw-r--r--   0 runner     (501) staff       (20)      543 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_embed/external_module.cpp
--rw-r--r--   0 runner     (501) staff       (20)    14260 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_embed/test_interpreter.cpp
--rw-r--r--   0 runner     (501) staff       (20)      237 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_embed/test_interpreter.py
--rw-r--r--   0 runner     (501) staff       (20)      275 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_embed/test_trampoline.py
--rw-r--r--   0 runner     (501) staff       (20)     5722 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_enum.cpp
--rw-r--r--   0 runner     (501) staff       (20)     8903 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_enum.py
--rw-r--r--   0 runner     (501) staff       (20)     3168 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_eval.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1143 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_eval.py
--rw-r--r--   0 runner     (501) staff       (20)      119 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_eval_call.py
--rw-r--r--   0 runner     (501) staff       (20)    11904 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_exceptions.cpp
--rw-r--r--   0 runner     (501) staff       (20)      399 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_exceptions.h
--rw-r--r--   0 runner     (501) staff       (20)    12702 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_exceptions.py
--rw-r--r--   0 runner     (501) staff       (20)    18155 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_factory_constructors.cpp
--rw-r--r--   0 runner     (501) staff       (20)    16519 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_factory_constructors.py
--rw-r--r--   0 runner     (501) staff       (20)     5311 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_gil_scoped.cpp
--rw-r--r--   0 runner     (501) staff       (20)     8565 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_gil_scoped.py
--rw-r--r--   0 runner     (501) staff       (20)     3960 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_iostream.cpp
--rw-r--r--   0 runner     (501) staff       (20)     7286 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_iostream.py
--rw-r--r--   0 runner     (501) staff       (20)     9535 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-r--r--   0 runner     (501) staff       (20)    13757 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_kwargs_and_defaults.py
--rw-r--r--   0 runner     (501) staff       (20)     4401 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_local_bindings.cpp
--rw-r--r--   0 runner     (501) staff       (20)     8049 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_local_bindings.py
--rw-r--r--   0 runner     (501) staff       (20)    21388 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_methods_and_attributes.cpp
--rw-r--r--   0 runner     (501) staff       (20)    18134 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_methods_and_attributes.py
--rw-r--r--   0 runner     (501) staff       (20)     4121 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_modules.cpp
--rw-r--r--   0 runner     (501) staff       (20)     4191 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_modules.py
--rw-r--r--   0 runner     (501) staff       (20)    12305 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_multiple_inheritance.cpp
--rw-r--r--   0 runner     (501) staff       (20)    11874 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_multiple_inheritance.py
--rw-r--r--   0 runner     (501) staff       (20)    19800 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_numpy_array.cpp
--rw-r--r--   0 runner     (501) staff       (20)    20228 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_numpy_array.py
--rw-r--r--   0 runner     (501) staff       (20)    21114 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_numpy_dtypes.cpp
--rw-r--r--   0 runner     (501) staff       (20)    14394 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_numpy_dtypes.py
--rw-r--r--   0 runner     (501) staff       (20)     4487 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_numpy_vectorize.cpp
--rw-r--r--   0 runner     (501) staff       (20)     9686 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_numpy_vectorize.py
--rw-r--r--   0 runner     (501) staff       (20)     2777 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_opaque_types.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1847 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_opaque_types.py
--rw-r--r--   0 runner     (501) staff       (20)     9463 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_operator_overloading.cpp
--rw-r--r--   0 runner     (501) staff       (20)     4333 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_operator_overloading.py
--rw-r--r--   0 runner     (501) staff       (20)     6719 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_pickling.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2720 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_pickling.py
--rw-r--r--   0 runner     (501) staff       (20)    30650 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_pytypes.cpp
--rw-r--r--   0 runner     (501) staff       (20)    23467 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_pytypes.py
--rw-r--r--   0 runner     (501) staff       (20)    21153 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_sequences_and_iterators.cpp
--rw-r--r--   0 runner     (501) staff       (20)     8021 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_sequences_and_iterators.py
--rw-r--r--   0 runner     (501) staff       (20)    18898 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_smart_ptr.cpp
--rw-r--r--   0 runner     (501) staff       (20)     9530 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_smart_ptr.py
--rw-r--r--   0 runner     (501) staff       (20)    21587 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_stl.cpp
--rw-r--r--   0 runner     (501) staff       (20)    12235 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_stl.py
--rw-r--r--   0 runner     (501) staff       (20)     4622 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_stl_binders.cpp
--rw-r--r--   0 runner     (501) staff       (20)     7912 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_stl_binders.py
--rw-r--r--   0 runner     (501) staff       (20)     4617 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-r--r--   0 runner     (501) staff       (20)      741 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_tagbased_polymorphic.py
--rw-r--r--   0 runner     (501) staff       (20)     1855 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_thread.cpp
--rw-r--r--   0 runner     (501) staff       (20)      826 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_thread.py
--rw-r--r--   0 runner     (501) staff       (20)      603 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_union.cpp
--rw-r--r--   0 runner     (501) staff       (20)      148 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_union.py
--rw-r--r--   0 runner     (501) staff       (20)    22983 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_virtual_functions.cpp
--rw-r--r--   0 runner     (501) staff       (20)    12919 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/test_virtual_functions.py
--rw-r--r--   0 runner     (501) staff       (20)     3226 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/valgrind-numpy-scipy.supp
--rw-r--r--   0 runner     (501) staff       (20)     2657 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tests/valgrind-python.supp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.267024 mmcif-0.80.1/modules/pybind11/tools/
--rw-r--r--   0 runner     (501) staff       (20)     2350 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner     (501) staff       (20)     3105 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner     (501) staff       (20)    11103 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner     (501) staff       (20)      817 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0 runner     (501) staff       (20)     1423 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tools/check-style.sh
--rw-r--r--   0 runner     (501) staff       (20)      952 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner     (501) staff       (20)     1040 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 runner     (501) staff       (20)     1031 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1282 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner     (501) staff       (20)      196 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 runner     (501) staff       (20)    13487 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner     (501) staff       (20)     6930 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner     (501) staff       (20)     8955 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner     (501) staff       (20)     8359 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner     (501) staff       (20)       94 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)     1965 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner     (501) staff       (20)     1139 2022-12-04 17:03:38.000000 mmcif-0.80.1/modules/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.277112 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/
--rw-r--r--   0 runner     (501) staff       (20)     1304 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.appveyor.yml
--rw-r--r--   0 runner     (501) staff       (20)      523 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.clang-format
--rw-r--r--   0 runner     (501) staff       (20)      242 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.clang-tidy
--rw-r--r--   0 runner     (501) staff       (20)     2196 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.cmake-format.yaml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.280325 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/
--rw-r--r--   0 runner     (501) staff       (20)    14415 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.283494 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner     (501) staff       (20)     1270 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner     (501) staff       (20)      172 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner     (501) staff       (20)      669 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner     (501) staff       (20)     1180 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner     (501) staff       (20)      559 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/dependabot.yml
--rw-r--r--   0 runner     (501) staff       (20)      116 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/labeler.yml
--rw-r--r--   0 runner     (501) staff       (20)       50 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/labeler_merged.yml
--rw-r--r--   0 runner     (501) staff       (20)      404 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/pull_request_template.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.288808 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)    24508 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/workflows/ci.yml
--rw-r--r--   0 runner     (501) staff       (20)     2117 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/workflows/configure.yml
--rw-r--r--   0 runner     (501) staff       (20)     1090 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/workflows/format.yml
--rw-r--r--   0 runner     (501) staff       (20)      333 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/workflows/labeler.yml
--rw-r--r--   0 runner     (501) staff       (20)     2497 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/workflows/pip.yml
--rw-r--r--   0 runner     (501) staff       (20)      452 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)     2460 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.pre-commit-config.yaml
--rw-r--r--   0 runner     (501) staff       (20)       62 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.readthedocs.yml
--rw-r--r--   0 runner     (501) staff       (20)    10438 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     1684 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      256 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     8064 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/README.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.320028 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/
--rw-r--r--   0 runner     (501) staff       (20)      705 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/Doxyfile
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.325200 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/_static/
--rw-r--r--   0 runner     (501) staff       (20)      254 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/_static/theme_overrides.css
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.347818 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.357843 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/cast/
--rw-r--r--   0 runner     (501) staff       (20)     3937 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/cast/chrono.rst
--rw-r--r--   0 runner     (501) staff       (20)     3398 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/cast/custom.rst
--rw-r--r--   0 runner     (501) staff       (20)    14288 2022-12-04 17:03:33.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/cast/eigen.rst
--rw-r--r--   0 runner     (501) staff       (20)     3889 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/cast/functional.rst
--rw-r--r--   0 runner     (501) staff       (20)     1556 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/cast/index.rst
--rw-r--r--   0 runner     (501) staff       (20)    11680 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/cast/overview.rst
--rw-r--r--   0 runner     (501) staff       (20)     9703 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/cast/stl.rst
--rw-r--r--   0 runner     (501) staff       (20)     9372 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/cast/strings.rst
--rw-r--r--   0 runner     (501) staff       (20)    45878 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/classes.rst
--rw-r--r--   0 runner     (501) staff       (20)     8420 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/embedding.rst
--rw-r--r--   0 runner     (501) staff       (20)    14171 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/exceptions.rst
--rw-r--r--   0 runner     (501) staff       (20)    25082 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/functions.rst
--rw-r--r--   0 runner     (501) staff       (20)    12444 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/misc.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.371047 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/
--rw-r--r--   0 runner     (501) staff       (20)      278 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/index.rst
--rw-r--r--   0 runner     (501) staff       (20)    16538 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/numpy.rst
--rw-r--r--   0 runner     (501) staff       (20)     7878 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/object.rst
--rw-r--r--   0 runner     (501) staff       (20)     5125 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/utilities.rst
--rw-r--r--   0 runner     (501) staff       (20)     6366 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/smart_ptrs.rst
--rw-r--r--   0 runner     (501) staff       (20)     9369 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/basics.rst
--rw-r--r--   0 runner     (501) staff       (20)     2974 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/benchmark.py
--rw-r--r--   0 runner     (501) staff       (20)     3168 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/benchmark.rst
--rw-r--r--   0 runner     (501) staff       (20)    74047 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/changelog.rst
--rw-r--r--   0 runner     (501) staff       (20)    16122 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/classes.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.372182 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/cmake/
--rw-r--r--   0 runner     (501) staff       (20)      273 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/cmake/index.rst
--rw-r--r--   0 runner     (501) staff       (20)    25511 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/compiling.rst
--rw-r--r--   0 runner     (501) staff       (20)    12095 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/conf.py
--rw-r--r--   0 runner     (501) staff       (20)    14593 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/faq.rst
--rw-r--r--   0 runner     (501) staff       (20)      613 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/index.rst
--rw-r--r--   0 runner     (501) staff       (20)     3277 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/installing.rst
--rw-r--r--   0 runner     (501) staff       (20)     3062 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/limitations.rst
--rw-r--r--   0 runner     (501) staff       (20)    58510 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/pybind11-logo.png
--rw-r--r--   0 runner     (501) staff       (20)    44653 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python1.png
--rw-r--r--   0 runner     (501) staff       (20)    87708 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python1.svg
--rw-r--r--   0 runner     (501) staff       (20)    41121 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python2.png
--rw-r--r--   0 runner     (501) staff       (20)    85853 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python2.svg
--rw-r--r--   0 runner     (501) staff       (20)     2511 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/reference.rst
--rw-r--r--   0 runner     (501) staff       (20)     4028 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/release.rst
--rw-r--r--   0 runner     (501) staff       (20)      168 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/requirements.txt
--rw-r--r--   0 runner     (501) staff       (20)    23059 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/upgrade.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:25.903268 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.396526 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/
--rw-r--r--   0 runner     (501) staff       (20)    21412 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/attr.h
--rw-r--r--   0 runner     (501) staff       (20)     6118 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/buffer_info.h
--rw-r--r--   0 runner     (501) staff       (20)    57522 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/cast.h
--rw-r--r--   0 runner     (501) staff       (20)     8516 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/chrono.h
--rw-r--r--   0 runner     (501) staff       (20)      120 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/common.h
--rw-r--r--   0 runner     (501) staff       (20)     2037 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/complex.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.401539 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/detail/
--rw-r--r--   0 runner     (501) staff       (20)    27823 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/detail/class.h
--rw-r--r--   0 runner     (501) staff       (20)    42083 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/detail/common.h
--rw-r--r--   0 runner     (501) staff       (20)     3602 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/detail/descr.h
--rw-r--r--   0 runner     (501) staff       (20)    16397 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/detail/init.h
--rw-r--r--   0 runner     (501) staff       (20)    16375 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/detail/internals.h
--rw-r--r--   0 runner     (501) staff       (20)    40663 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner     (501) staff       (20)     1486 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner     (501) staff       (20)    29086 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/eigen.h
--rw-r--r--   0 runner     (501) staff       (20)     7843 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/embed.h
--rw-r--r--   0 runner     (501) staff       (20)     5079 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/eval.h
--rw-r--r--   0 runner     (501) staff       (20)     3709 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/functional.h
--rw-r--r--   0 runner     (501) staff       (20)     6532 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/gil.h
--rw-r--r--   0 runner     (501) staff       (20)     6084 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/iostream.h
--rw-r--r--   0 runner     (501) staff       (20)    69820 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/numpy.h
--rw-r--r--   0 runner     (501) staff       (20)     9085 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/operators.h
--rw-r--r--   0 runner     (501) staff       (20)     2049 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/options.h
--rw-r--r--   0 runner     (501) staff       (20)   105679 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/pybind11.h
--rw-r--r--   0 runner     (501) staff       (20)    67597 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/pytypes.h
--rw-r--r--   0 runner     (501) staff       (20)    14162 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/stl.h
--rw-r--r--   0 runner     (501) staff       (20)    23912 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.406588 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/pybind11/
--rw-r--r--   0 runner     (501) staff       (20)      217 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/pybind11/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1158 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/pybind11/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)      207 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/pybind11/_version.py
--rw-r--r--   0 runner     (501) staff       (20)      137 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/pybind11/_version.pyi
--rw-r--r--   0 runner     (501) staff       (20)      663 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/pybind11/commands.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/pybind11/py.typed
--rw-r--r--   0 runner     (501) staff       (20)    15167 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/pybind11/setup_helpers.py
--rw-r--r--   0 runner     (501) staff       (20)     1899 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/pybind11/setup_helpers.pyi
--rw-r--r--   0 runner     (501) staff       (20)      118 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)     2185 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     3499 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.479708 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/
--rw-r--r--   0 runner     (501) staff       (20)    15372 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     4841 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/conftest.py
--rw-r--r--   0 runner     (501) staff       (20)    11157 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/constructor_stats.h
--rw-r--r--   0 runner     (501) staff       (20)     1819 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/cross_module_gil_utils.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1022 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/env.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.480864 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/extra_python_package/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/extra_python_package/pytest.ini
--rw-r--r--   0 runner     (501) staff       (20)     7154 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/extra_python_package/test_files.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.482123 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/extra_setuptools/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/extra_setuptools/pytest.ini
--rw-r--r--   0 runner     (501) staff       (20)     2581 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0 runner     (501) staff       (20)     2144 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/local_bindings.h
--rw-r--r--   0 runner     (501) staff       (20)     5389 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/object.h
--rw-r--r--   0 runner     (501) staff       (20)     5285 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/pybind11_cross_module_tests.cpp
--rw-r--r--   0 runner     (501) staff       (20)     3647 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/pybind11_tests.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2733 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/pybind11_tests.h
--rw-r--r--   0 runner     (501) staff       (20)      693 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/pytest.ini
--rw-r--r--   0 runner     (501) staff       (20)      843 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/requirements.txt
--rw-r--r--   0 runner     (501) staff       (20)      864 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_async.cpp
--rw-r--r--   0 runner     (501) staff       (20)      558 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_async.py
--rw-r--r--   0 runner     (501) staff       (20)     8048 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_buffers.cpp
--rw-r--r--   0 runner     (501) staff       (20)     4946 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_buffers.py
--rw-r--r--   0 runner     (501) staff       (20)    13475 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_builtin_casters.cpp
--rw-r--r--   0 runner     (501) staff       (20)    17617 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_builtin_casters.py
--rw-r--r--   0 runner     (501) staff       (20)     3702 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_call_policies.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5728 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_call_policies.py
--rw-r--r--   0 runner     (501) staff       (20)     6754 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_callbacks.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5447 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_callbacks.py
--rw-r--r--   0 runner     (501) staff       (20)     3406 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_chrono.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5726 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_chrono.py
--rw-r--r--   0 runner     (501) staff       (20)    21548 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_class.cpp
--rw-r--r--   0 runner     (501) staff       (20)    14273 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_class.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.485337 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/
--rw-r--r--   0 runner     (501) staff       (20)     2639 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      656 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/embed.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.485924 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner     (501) staff       (20)     1175 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.486549 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner     (501) staff       (20)     1259 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.487519 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner     (501) staff       (20)     1653 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      152 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/main.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.488225 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner     (501) staff       (20)     1357 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.488906 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner     (501) staff       (20)     1126 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.489399 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner     (501) staff       (20)     1333 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      166 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/test.py
--rw-r--r--   0 runner     (501) staff       (20)     5346 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_constants_and_functions.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1522 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_constants_and_functions.py
--rw-r--r--   0 runner     (501) staff       (20)     9629 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_copy_move.cpp
--rw-r--r--   0 runner     (501) staff       (20)     4645 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_copy_move.py
--rw-r--r--   0 runner     (501) staff       (20)     5513 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_custom_type_casters.cpp
--rw-r--r--   0 runner     (501) staff       (20)     4015 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_custom_type_casters.py
--rw-r--r--   0 runner     (501) staff       (20)     2514 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_docstring_options.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1630 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_docstring_options.py
--rw-r--r--   0 runner     (501) staff       (20)    16867 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_eigen.cpp
--rw-r--r--   0 runner     (501) staff       (20)    28282 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_eigen.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.492337 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_embed/
--rw-r--r--   0 runner     (501) staff       (20)     1758 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_embed/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      637 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_embed/catch.cpp
--rw-r--r--   0 runner     (501) staff       (20)      554 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_embed/external_module.cpp
--rw-r--r--   0 runner     (501) staff       (20)    10209 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_embed/test_interpreter.cpp
--rw-r--r--   0 runner     (501) staff       (20)      219 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_embed/test_interpreter.py
--rw-r--r--   0 runner     (501) staff       (20)     2610 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_enum.cpp
--rw-r--r--   0 runner     (501) staff       (20)     7694 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_enum.py
--rw-r--r--   0 runner     (501) staff       (20)     2628 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_eval.cpp
--rw-r--r--   0 runner     (501) staff       (20)      768 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_eval.py
--rw-r--r--   0 runner     (501) staff       (20)      143 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_eval_call.py
--rw-r--r--   0 runner     (501) staff       (20)     7862 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_exceptions.cpp
--rw-r--r--   0 runner     (501) staff       (20)     6753 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_exceptions.py
--rw-r--r--   0 runner     (501) staff       (20)    16562 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_factory_constructors.cpp
--rw-r--r--   0 runner     (501) staff       (20)    16731 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_factory_constructors.py
--rw-r--r--   0 runner     (501) staff       (20)     1760 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_gil_scoped.cpp
--rw-r--r--   0 runner     (501) staff       (20)     3128 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_gil_scoped.py
--rw-r--r--   0 runner     (501) staff       (20)     3381 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_iostream.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5799 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_iostream.py
--rw-r--r--   0 runner     (501) staff       (20)     6489 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_kwargs_and_defaults.cpp
--rw-r--r--   0 runner     (501) staff       (20)    10048 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_kwargs_and_defaults.py
--rw-r--r--   0 runner     (501) staff       (20)     4333 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_local_bindings.cpp
--rw-r--r--   0 runner     (501) staff       (20)     8102 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_local_bindings.py
--rw-r--r--   0 runner     (501) staff       (20)    19446 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_methods_and_attributes.cpp
--rw-r--r--   0 runner     (501) staff       (20)    17310 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_methods_and_attributes.py
--rw-r--r--   0 runner     (501) staff       (20)     3742 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_modules.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2841 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_modules.py
--rw-r--r--   0 runner     (501) staff       (20)     9148 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_multiple_inheritance.cpp
--rw-r--r--   0 runner     (501) staff       (20)     9495 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_multiple_inheritance.py
--rw-r--r--   0 runner     (501) staff       (20)    17781 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_numpy_array.cpp
--rw-r--r--   0 runner     (501) staff       (20)    18647 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_numpy_array.py
--rw-r--r--   0 runner     (501) staff       (20)    18421 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_numpy_dtypes.cpp
--rw-r--r--   0 runner     (501) staff       (20)    13614 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_numpy_dtypes.py
--rw-r--r--   0 runner     (501) staff       (20)     3832 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_numpy_vectorize.cpp
--rw-r--r--   0 runner     (501) staff       (20)     9709 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_numpy_vectorize.py
--rw-r--r--   0 runner     (501) staff       (20)     2731 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_opaque_types.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1906 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_opaque_types.py
--rw-r--r--   0 runner     (501) staff       (20)     8431 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_operator_overloading.cpp
--rw-r--r--   0 runner     (501) staff       (20)     4136 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_operator_overloading.py
--rw-r--r--   0 runner     (501) staff       (20)     4945 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_pickling.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1191 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_pickling.py
--rw-r--r--   0 runner     (501) staff       (20)    14656 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_pytypes.cpp
--rw-r--r--   0 runner     (501) staff       (20)    16590 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_pytypes.py
--rw-r--r--   0 runner     (501) staff       (20)    13120 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_sequences_and_iterators.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5966 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_sequences_and_iterators.py
--rw-r--r--   0 runner     (501) staff       (20)    18187 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_smart_ptr.cpp
--rw-r--r--   0 runner     (501) staff       (20)     9620 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_smart_ptr.py
--rw-r--r--   0 runner     (501) staff       (20)    12793 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_stl.cpp
--rw-r--r--   0 runner     (501) staff       (20)     8557 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_stl.py
--rw-r--r--   0 runner     (501) staff       (20)     4403 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_stl_binders.cpp
--rw-r--r--   0 runner     (501) staff       (20)     7182 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_stl_binders.py
--rw-r--r--   0 runner     (501) staff       (20)     4458 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_tagbased_polymorphic.cpp
--rw-r--r--   0 runner     (501) staff       (20)      765 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_tagbased_polymorphic.py
--rw-r--r--   0 runner     (501) staff       (20)      603 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_union.cpp
--rw-r--r--   0 runner     (501) staff       (20)      172 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_union.py
--rw-r--r--   0 runner     (501) staff       (20)    18454 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_virtual_functions.cpp
--rw-r--r--   0 runner     (501) staff       (20)    11646 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_virtual_functions.py
--rw-r--r--   0 runner     (501) staff       (20)     3238 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/valgrind-numpy-scipy.supp
--rw-r--r--   0 runner     (501) staff       (20)     2657 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/valgrind-python.supp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-12-04 17:10:26.696089 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/
--rw-r--r--   0 runner     (501) staff       (20)     2295 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/FindCatch.cmake
--rw-r--r--   0 runner     (501) staff       (20)     3105 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/FindEigen3.cmake
--rw-r--r--   0 runner     (501) staff       (20)     9977 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 runner     (501) staff       (20)     1427 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/check-style.sh
--rw-r--r--   0 runner     (501) staff       (20)      952 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner     (501) staff       (20)     1121 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/libsize.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1202 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/make_changelog.py
--rw-r--r--   0 runner     (501) staff       (20)    14164 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/pybind11Common.cmake
--rw-r--r--   0 runner     (501) staff       (20)     7010 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner     (501) staff       (20)     9173 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner     (501) staff       (20)     7276 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/pybind11Tools.cmake
--rw-r--r--   0 runner     (501) staff       (20)       94 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)     1822 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/setup_global.py.in
--rw-r--r--   0 runner     (501) staff       (20)      915 2022-12-04 17:03:34.000000 mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/setup_main.py.in
--rw-r--r--   0 runner     (501) staff       (20)      120 2022-12-04 17:03:34.000000 mmcif-0.80.1/requirements-doc.txt
--rw-r--r--   0 runner     (501) staff       (20)       13 2022-12-04 17:03:34.000000 mmcif-0.80.1/requirements-test.txt
--rw-r--r--   0 runner     (501) staff       (20)       36 2022-12-04 17:03:34.000000 mmcif-0.80.1/requirements.txt
--rw-r--r--   0 runner     (501) staff       (20)       38 2022-12-04 17:10:26.697930 mmcif-0.80.1/setup.cfg
--rwxr-xr-x   0 runner     (501) staff       (20)     6673 2022-12-04 17:03:34.000000 mmcif-0.80.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.646404 mmcif-0.81/
+-rw-r--r--   0 vsts      (1001) docker     (122)    12721 2023-04-08 23:40:38.000000 mmcif-0.81/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     6419 2023-04-08 23:40:38.000000 mmcif-0.81/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-04-08 23:40:38.000000 mmcif-0.81/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      441 2023-04-08 23:40:38.000000 mmcif-0.81/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     2779 2023-04-08 23:44:22.646404 mmcif-0.81/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     2075 2023-04-08 23:40:38.000000 mmcif-0.81/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.562403 mmcif-0.81/mmcif/
+-rw-r--r--   0 vsts      (1001) docker     (122)      184 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.566403 mmcif-0.81/mmcif/api/
+-rw-r--r--   0 vsts      (1001) docker     (122)    21941 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/api/DataCategory.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17192 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/api/DataCategoryBase.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13272 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/api/DataCategoryFormatted.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9789 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/api/DataCategoryTyped.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10128 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/api/DictMethodRunner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    85436 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/api/DictionaryApi.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    24778 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/api/DictionaryInclude.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3844 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/api/Method.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5017 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/api/MethodUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10640 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/api/PdbxContainers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/api/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.566403 mmcif-0.81/mmcif/core/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/core/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.566403 mmcif-0.81/mmcif/io/
+-rw-r--r--   0 vsts      (1001) docker     (122)    19023 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/io/BinaryCifReader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18735 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/io/BinaryCifWriter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2922 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/io/BuildDictionaryExec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1551 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/io/CifFile.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12704 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/io/IoAdapterBase.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18753 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/io/IoAdapterCore.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13995 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/io/IoAdapterPy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      524 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/io/PdbxExceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18397 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/io/PdbxReader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11640 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/io/PdbxWriter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-04-08 23:40:38.000000 mmcif-0.81/mmcif/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.566403 mmcif-0.81/mmcif.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2779 2023-04-08 23:44:22.000000 mmcif-0.81/mmcif.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    29562 2023-04-08 23:44:22.000000 mmcif-0.81/mmcif.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-08 23:44:22.000000 mmcif-0.81/mmcif.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       69 2023-04-08 23:44:22.000000 mmcif-0.81/mmcif.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-08 23:41:00.000000 mmcif-0.81/mmcif.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      130 2023-04-08 23:44:22.000000 mmcif-0.81/mmcif.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        6 2023-04-08 23:44:22.000000 mmcif-0.81/mmcif.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.562403 mmcif-0.81/modules/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.558403 mmcif-0.81/modules/cc-regex/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.570403 mmcif-0.81/modules/cc-regex/include/
+-rw-r--r--   0 vsts      (1001) docker     (122)      943 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cc-regex/include/cclass.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2057 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cc-regex/include/cname.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      329 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cc-regex/include/debug.ih
+-rw-r--r--   0 vsts      (1001) docker     (122)     1379 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cc-regex/include/engine.ih
+-rw-r--r--   0 vsts      (1001) docker     (122)      500 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cc-regex/include/main.ih
+-rw-r--r--   0 vsts      (1001) docker     (122)     2723 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cc-regex/include/regcomp.ih
+-rw-r--r--   0 vsts      (1001) docker     (122)      267 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cc-regex/include/regerror.ih
+-rw-r--r--   0 vsts      (1001) docker     (122)     1891 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cc-regex/include/regex.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5365 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cc-regex/include/regex2.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      500 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cc-regex/include/utils.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.570403 mmcif-0.81/modules/cc-regex/src/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5092 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cc-regex/src/debug.c
+-rw-r--r--   0 vsts      (1001) docker     (122)    25587 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cc-regex/src/engine.c
+-rw-r--r--   0 vsts      (1001) docker     (122)    11193 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cc-regex/src/main.c
+-rw-r--r--   0 vsts      (1001) docker     (122)     1825 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cc-regex/src/mkh
+-rw-r--r--   0 vsts      (1001) docker     (122)    37342 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cc-regex/src/regcomp.c
+-rw-r--r--   0 vsts      (1001) docker     (122)     3212 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cc-regex/src/regerror.c
+-rw-r--r--   0 vsts      (1001) docker     (122)     4259 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cc-regex/src/regexec.c
+-rw-r--r--   0 vsts      (1001) docker     (122)      736 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cc-regex/src/regfree.c
+-rw-r--r--   0 vsts      (1001) docker     (122)     7061 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cc-regex/src/split.c
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.558403 mmcif-0.81/modules/cpp-cif-file/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.570403 mmcif-0.81/modules/cpp-cif-file/include/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1746 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-file/include/CifDataInfo.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      617 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-file/include/CifExcept.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    23567 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-file/include/CifFile.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1945 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-file/include/CifParentChild.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5484 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-file/include/DicFile.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2782 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-file/include/ParentChild.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.570403 mmcif-0.81/modules/cpp-cif-file/src/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6274 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-file/src/CifDataInfo.C
+-rw-r--r--   0 vsts      (1001) docker     (122)    34845 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-file/src/CifExcept.C
+-rw-r--r--   0 vsts      (1001) docker     (122)    85656 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-file/src/CifFile.C
+-rw-r--r--   0 vsts      (1001) docker     (122)    32174 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-file/src/CifParentChild.C
+-rw-r--r--   0 vsts      (1001) docker     (122)    47643 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-file/src/DicFile.C
+-rw-r--r--   0 vsts      (1001) docker     (122)    23231 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-file/src/ParentChild.C
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.558403 mmcif-0.81/modules/cpp-cif-file-util/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.570403 mmcif-0.81/modules/cpp-cif-file-util/include/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3264 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-file-util/include/CifCorrector.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2444 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-file-util/include/CifFileUtil.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.570403 mmcif-0.81/modules/cpp-cif-file-util/src/
+-rw-r--r--   0 vsts      (1001) docker     (122)    47136 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-file-util/src/CifCorrector.C
+-rw-r--r--   0 vsts      (1001) docker     (122)     4509 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-file-util/src/CifFileUtil.C
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.558403 mmcif-0.81/modules/cpp-cif-parser/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.574403 mmcif-0.81/modules/cpp-cif-parser/include/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1518 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-parser/include/CifFileReadDef.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6318 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-parser/include/CifParserBase.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      898 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-parser/include/CifParserInt.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1390 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-parser/include/CifScannerBase.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      750 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-parser/include/CifScannerInt.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6970 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-parser/include/DICParserBase.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1032 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-parser/include/DICParserInt.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1471 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-parser/include/DICScannerBase.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      912 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-parser/include/DICScannerInt.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.574403 mmcif-0.81/modules/cpp-cif-parser/src/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3768 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-parser/src/CifFileReadDef.C
+-rw-r--r--   0 vsts      (1001) docker     (122)     2206 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-parser/src/CifParser.y
+-rw-r--r--   0 vsts      (1001) docker     (122)    23419 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-parser/src/CifParserBase.C
+-rw-r--r--   0 vsts      (1001) docker     (122)     2475 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-parser/src/CifScanner.l
+-rw-r--r--   0 vsts      (1001) docker     (122)     9603 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-parser/src/CifScannerBase.C
+-rw-r--r--   0 vsts      (1001) docker     (122)     2376 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-parser/src/DICParser.y
+-rw-r--r--   0 vsts      (1001) docker     (122)    41071 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-parser/src/DICParserBase.C
+-rw-r--r--   0 vsts      (1001) docker     (122)     2985 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-parser/src/DICScanner.l
+-rw-r--r--   0 vsts      (1001) docker     (122)    10258 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-cif-parser/src/DICScannerBase.C
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.558403 mmcif-0.81/modules/cpp-common/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.574403 mmcif-0.81/modules/cpp-common/include/
+-rw-r--r--   0 vsts      (1001) docker     (122)      520 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/include/BlockIO.h
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2398 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/include/CifDefs.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6737 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/include/CifString.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2901 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/include/DataInfo.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3175 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/include/Exceptions.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      635 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/include/GenCont.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6109 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/include/GenString.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      484 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/include/RcsbFile.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      335 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/include/RcsbPlatform.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5664 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/include/Serializer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2665 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/include/mapped_ptr_vector.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1543 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/include/mapped_vector.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      210 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/include/rcsb_math.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      617 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/include/rcsb_types.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.578403 mmcif-0.81/modules/cpp-common/src/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1240 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/src/BlockIO.C
+-rw-r--r--   0 vsts      (1001) docker     (122)    10498 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/src/CifString.C
+-rw-r--r--   0 vsts      (1001) docker     (122)     9606 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/src/DataInfo.C
+-rw-r--r--   0 vsts      (1001) docker     (122)     2314 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/src/Exceptions.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1085 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/src/GenCont.C
+-rw-r--r--   0 vsts      (1001) docker     (122)    14827 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/src/GenString.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1236 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/src/RcsbFile.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      356 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/src/RcsbPlatform.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)    40038 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/src/Serializer.C
+-rw-r--r--   0 vsts      (1001) docker     (122)    10675 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/src/mapped_ptr_vector.C
+-rw-r--r--   0 vsts      (1001) docker     (122)     5759 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-common/src/mapped_vector.C
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.558403 mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.578403 mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2072 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifDataInfo.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    12223 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFile.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     3130 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFileReadDef.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     3592 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFileUtil.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     3791 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wrapDicFile.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     2003 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wrapDictDataInfo.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    14081 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wrapISTable.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     6137 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wrapTableFile.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      690 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wrapmmciflib.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1017 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wraprcsb_types.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.558403 mmcif-0.81/modules/cpp-dict-obj-file/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.578403 mmcif-0.81/modules/cpp-dict-obj-file/include/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1437 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-dict-obj-file/include/DictDataInfo.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7726 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-dict-obj-file/include/DictObjCont.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     4564 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-dict-obj-file/include/DictObjContInfo.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5597 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-dict-obj-file/include/DictObjFile.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      876 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-dict-obj-file/include/DictParentChild.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.578403 mmcif-0.81/modules/cpp-dict-obj-file/src/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3975 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-dict-obj-file/src/DictDataInfo.C
+-rw-r--r--   0 vsts      (1001) docker     (122)    19477 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-dict-obj-file/src/DictObjCont.C
+-rw-r--r--   0 vsts      (1001) docker     (122)    12717 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-dict-obj-file/src/DictObjContInfo.C
+-rw-r--r--   0 vsts      (1001) docker     (122)     6349 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-dict-obj-file/src/DictObjFile.C
+-rw-r--r--   0 vsts      (1001) docker     (122)     1979 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-dict-obj-file/src/DictObjFileCreator.C
+-rw-r--r--   0 vsts      (1001) docker     (122)      741 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-dict-obj-file/src/DictObjFileReader.C
+-rw-r--r--   0 vsts      (1001) docker     (122)    13027 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-dict-obj-file/src/DictObjFileSelectiveReader.C
+-rw-r--r--   0 vsts      (1001) docker     (122)     8311 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-dict-obj-file/src/DictParentChild.C
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.558403 mmcif-0.81/modules/cpp-mmciflib-test/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.582403 mmcif-0.81/modules/cpp-mmciflib-test/src/
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1333 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/BigCifTest.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     5347 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/CifDiff.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     3115 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/CifInfo.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2788 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/CifReader.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2673 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/DataChecking.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1929 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/DictInfo.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1894 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest1.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1073 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest10.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2061 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest11.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2406 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest12.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      539 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest13.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     3930 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest14.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     3211 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest2.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1385 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest3.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2410 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest4.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1417 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest5.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1174 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest6.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1863 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest7.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      406 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest8.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      611 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest9.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1316 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/GroupTableTest2.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      582 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/SdbReader.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1519 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/checkdictionary.C
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      655 2023-04-08 23:40:38.000000 mmcif-0.81/modules/cpp-mmciflib-test/src/selective-reading.C
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.558403 mmcif-0.81/modules/cpp-tables/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.582403 mmcif-0.81/modules/cpp-tables/include/
+-rw-r--r--   0 vsts      (1001) docker     (122)    52000 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-tables/include/ISTable.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    44528 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-tables/include/ITTable.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    20019 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-tables/include/TTable.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1270 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-tables/include/TableError.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    21422 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-tables/include/TableFile.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.582403 mmcif-0.81/modules/cpp-tables/src/
+-rw-r--r--   0 vsts      (1001) docker     (122)    77385 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-tables/src/ISTable.C
+-rw-r--r--   0 vsts      (1001) docker     (122)    43788 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-tables/src/ITTable.C
+-rw-r--r--   0 vsts      (1001) docker     (122)    15437 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-tables/src/TTable.C
+-rw-r--r--   0 vsts      (1001) docker     (122)    26031 2023-04-08 23:40:41.000000 mmcif-0.81/modules/cpp-tables/src/TableFile.C
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.586403 mmcif-0.81/modules/pybind11/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1271 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.appveyor.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      996 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.clang-format
+-rw-r--r--   0 vsts      (1001) docker     (122)     2605 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.clang-tidy
+-rw-r--r--   0 vsts      (1001) docker     (122)     2196 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.cmake-format.yaml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1308 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.codespell-ignore-lines
+-rw-r--r--   0 vsts      (1001) docker     (122)       44 2023-04-08 23:40:41.000000 mmcif-0.81/modules/pybind11/.git
+-rw-r--r--   0 vsts      (1001) docker     (122)       18 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.gitattributes
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.586403 mmcif-0.81/modules/pybind11/.github/
+-rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.github/CODEOWNERS
+-rw-r--r--   0 vsts      (1001) docker     (122)    15271 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.github/CONTRIBUTING.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.586403 mmcif-0.81/modules/pybind11/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2016 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      328 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      162 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.github/dependabot.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      116 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.github/labeler.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)       50 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.github/labeler_merged.yml
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.586403 mmcif-0.81/modules/pybind11/.github/matchers/
+-rw-r--r--   0 vsts      (1001) docker     (122)      668 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.github/matchers/pylint.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      645 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.github/pull_request_template.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.586403 mmcif-0.81/modules/pybind11/.github/workflows/
+-rw-r--r--   0 vsts      (1001) docker     (122)    28486 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.github/workflows/ci.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)     2095 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.github/workflows/configure.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1419 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.github/workflows/format.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      333 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.github/workflows/labeler.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)     2558 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.github/workflows/pip.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)     2837 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.github/workflows/upstream.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      487 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (122)     4331 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/.readthedocs.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)    11911 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     1684 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      223 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     7686 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/README.rst
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.590403 mmcif-0.81/modules/pybind11/docs/
+-rw-r--r--   0 vsts      (1001) docker     (122)      607 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/Doxyfile
+-rw-r--r--   0 vsts      (1001) docker     (122)     7417 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/Makefile
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.558403 mmcif-0.81/modules/pybind11/docs/_static/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.590403 mmcif-0.81/modules/pybind11/docs/_static/css/
+-rw-r--r--   0 vsts      (1001) docker     (122)       37 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/_static/css/custom.css
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.594403 mmcif-0.81/modules/pybind11/docs/advanced/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.594403 mmcif-0.81/modules/pybind11/docs/advanced/cast/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3937 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/advanced/cast/chrono.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     3429 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/advanced/cast/custom.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    14283 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/advanced/cast/eigen.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     3889 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/advanced/cast/functional.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     1556 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/advanced/cast/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    12371 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/advanced/cast/overview.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     9586 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/advanced/cast/stl.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     8863 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/advanced/cast/strings.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    47796 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/advanced/classes.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     8453 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/advanced/embedding.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    17772 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/advanced/exceptions.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    26729 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/advanced/functions.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    13634 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/advanced/misc.rst
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.594403 mmcif-0.81/modules/pybind11/docs/advanced/pycpp/
+-rw-r--r--   0 vsts      (1001) docker     (122)      278 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/advanced/pycpp/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    17161 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     9030 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/advanced/pycpp/object.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     5710 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     6377 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     9240 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/basics.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     2856 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/benchmark.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3168 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/benchmark.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)   111105 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/changelog.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    16380 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/classes.rst
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.594403 mmcif-0.81/modules/pybind11/docs/cmake/
+-rw-r--r--   0 vsts      (1001) docker     (122)      273 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/cmake/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    25777 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/compiling.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    11559 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/conf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13177 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/faq.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)      613 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     3277 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/installing.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     3079 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/limitations.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    61034 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/pybind11-logo.png
+-rw-r--r--   0 vsts      (1001) docker     (122)    44653 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0 vsts      (1001) docker     (122)    87708 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0 vsts      (1001) docker     (122)    41121 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0 vsts      (1001) docker     (122)    85853 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0 vsts      (1001) docker     (122)     2647 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/reference.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     4414 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/release.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)      149 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    23489 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/docs/upgrade.rst
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.558403 mmcif-0.81/modules/pybind11/include/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.598403 mmcif-0.81/modules/pybind11/include/pybind11/
+-rw-r--r--   0 vsts      (1001) docker     (122)    23979 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7069 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    65638 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     8458 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/common.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2096 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.598403 mmcif-0.81/modules/pybind11/include/pybind11/detail/
+-rw-r--r--   0 vsts      (1001) docker     (122)    28251 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    50369 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5491 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    17981 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    25057 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    42266 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1625 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    32147 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    11792 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     4731 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     4695 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     8262 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     8862 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    79524 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     9103 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2181 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/options.h
+-rw-r--r--   0 vsts      (1001) docker     (122)   125761 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    93848 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.598403 mmcif-0.81/modules/pybind11/include/pybind11/stl/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4185 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    15337 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    27013 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2765 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/noxfile.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.598403 mmcif-0.81/modules/pybind11/pybind11/
+-rw-r--r--   0 vsts      (1001) docker     (122)      414 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/pybind11/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1360 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/pybind11/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      228 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/pybind11/_version.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1226 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/pybind11/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/pybind11/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (122)    17609 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1261 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1622 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     4877 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.610403 mmcif-0.81/modules/pybind11/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)    20608 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     5006 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11736 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/constructor_stats.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3578 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1776 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/cross_module_interleaved_error_already_set.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      940 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/env.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.614403 mmcif-0.81/modules/pybind11/tests/extra_python_package/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/extra_python_package/pytest.ini
+-rw-r--r--   0 vsts      (1001) docker     (122)     8142 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/extra_python_package/test_files.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.614403 mmcif-0.81/modules/pybind11/tests/extra_setuptools/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0 vsts      (1001) docker     (122)     4153 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2847 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/local_bindings.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5743 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/object.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6264 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4517 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/pybind11_tests.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     2685 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      768 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/pytest.ini
+-rw-r--r--   0 vsts      (1001) docker     (122)      600 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      855 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_async.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      534 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_async.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8567 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_buffers.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4841 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_buffers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15990 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_builtin_casters.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    17245 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4118 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_call_policies.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     6549 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_call_policies.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9243 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_callbacks.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     5906 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_callbacks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3370 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_chrono.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     5695 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_chrono.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    24803 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_class.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    14575 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_class.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.614403 mmcif-0.81/modules/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2639 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      673 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_cmake_build/embed.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.614403 mmcif-0.81/modules/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1171 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.614403 mmcif-0.81/modules/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1293 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.614403 mmcif-0.81/modules/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1685 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      152 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_cmake_build/main.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.614403 mmcif-0.81/modules/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1353 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.614403 mmcif-0.81/modules/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1163 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.614403 mmcif-0.81/modules/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1368 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      198 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3831 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_const_name.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      589 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_const_name.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5853 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_constants_and_functions.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1498 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10886 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_copy_move.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4796 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_copy_move.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7280 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_custom_type_casters.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     3980 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1259 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_custom_type_setup.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1089 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_custom_type_setup.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2816 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_docstring_options.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1606 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19409 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_eigen.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    28860 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_eigen.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.614403 mmcif-0.81/modules/pybind11/tests/test_embed/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1798 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     1338 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_embed/catch.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      543 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_embed/external_module.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    14260 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      237 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      275 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_embed/test_trampoline.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5722 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_enum.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     8903 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_enum.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3168 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_eval.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1143 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_eval.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      119 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_eval_call.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11904 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_exceptions.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      399 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_exceptions.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12702 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18155 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_factory_constructors.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    16519 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5311 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_gil_scoped.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     8565 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3960 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_iostream.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     7286 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_iostream.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9535 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    13757 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4401 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_local_bindings.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     8049 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21388 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    18134 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4121 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_modules.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4191 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_modules.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12305 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    11874 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19800 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_numpy_array.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    20228 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21114 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    14394 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4487 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     9686 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2777 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_opaque_types.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1847 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9463 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_operator_overloading.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4333 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6719 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_pickling.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     2720 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_pickling.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    30650 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_pytypes.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    23467 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_pytypes.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21153 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     8021 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18898 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_smart_ptr.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     9530 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21587 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_stl.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    12235 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_stl.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4622 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_stl_binders.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     7912 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4617 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      741 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1855 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_thread.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      826 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_thread.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      603 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_union.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      148 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_union.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    22983 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_virtual_functions.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    12919 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/test_virtual_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3226 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0 vsts      (1001) docker     (122)     2657 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tests/valgrind-python.supp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.618403 mmcif-0.81/modules/pybind11/tools/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2350 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 vsts      (1001) docker     (122)     3105 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 vsts      (1001) docker     (122)    11103 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 vsts      (1001) docker     (122)      817 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1423 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tools/check-style.sh
+-rw-r--r--   0 vsts      (1001) docker     (122)      952 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1040 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1031 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tools/libsize.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1282 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tools/make_changelog.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      196 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    13487 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 vsts      (1001) docker     (122)     6930 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     8955 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 vsts      (1001) docker     (122)     8359 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 vsts      (1001) docker     (122)       94 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tools/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1965 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1139 2023-04-08 23:40:42.000000 mmcif-0.81/modules/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.618403 mmcif-0.81/modules/pybind11_2_6_3_dev1/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1304 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.appveyor.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      523 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.clang-format
+-rw-r--r--   0 vsts      (1001) docker     (122)      242 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.clang-tidy
+-rw-r--r--   0 vsts      (1001) docker     (122)     2196 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.cmake-format.yaml
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.618403 mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/
+-rw-r--r--   0 vsts      (1001) docker     (122)    14415 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/CONTRIBUTING.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.618403 mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1270 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      172 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      669 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     1180 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      559 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/dependabot.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      116 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/labeler.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)       50 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/labeler_merged.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      404 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/pull_request_template.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.622403 mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/workflows/
+-rw-r--r--   0 vsts      (1001) docker     (122)    24508 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/workflows/ci.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)     2117 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/workflows/configure.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1090 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/workflows/format.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      333 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/workflows/labeler.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)     2497 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/workflows/pip.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      452 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (122)     2460 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.pre-commit-config.yaml
+-rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/.readthedocs.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)    10438 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     1684 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     8064 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/README.rst
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.622403 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/
+-rw-r--r--   0 vsts      (1001) docker     (122)      705 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/Doxyfile
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.622403 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/_static/
+-rw-r--r--   0 vsts      (1001) docker     (122)      254 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/_static/theme_overrides.css
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.626403 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.626403 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/cast/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3937 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/cast/chrono.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     3398 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/cast/custom.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    14288 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/cast/eigen.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     3889 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/cast/functional.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     1556 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/cast/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    11680 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/cast/overview.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     9703 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/cast/stl.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     9372 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/cast/strings.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    45878 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/classes.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     8420 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/embedding.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    14171 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/exceptions.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    25082 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/functions.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    12444 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/misc.rst
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.626403 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/
+-rw-r--r--   0 vsts      (1001) docker     (122)      278 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    16538 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     7878 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/object.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     5125 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     6366 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     9369 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/basics.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     2974 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/benchmark.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3168 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/benchmark.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    74047 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/changelog.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    16122 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/classes.rst
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.626403 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/cmake/
+-rw-r--r--   0 vsts      (1001) docker     (122)      273 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/cmake/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    25511 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/compiling.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    12095 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/conf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14593 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/faq.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)      613 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     3277 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/installing.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     3062 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/limitations.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    58510 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/pybind11-logo.png
+-rw-r--r--   0 vsts      (1001) docker     (122)    44653 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0 vsts      (1001) docker     (122)    87708 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0 vsts      (1001) docker     (122)    41121 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0 vsts      (1001) docker     (122)    85853 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0 vsts      (1001) docker     (122)     2511 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/reference.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     4028 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/release.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)      168 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    23059 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/upgrade.rst
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.562403 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.630403 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/
+-rw-r--r--   0 vsts      (1001) docker     (122)    21412 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/attr.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6118 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/buffer_info.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    57522 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/cast.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     8516 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/chrono.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/common.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2037 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/complex.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.630403 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/detail/
+-rw-r--r--   0 vsts      (1001) docker     (122)    27823 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/detail/class.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    42083 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/detail/common.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3602 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/detail/descr.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    16397 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/detail/init.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    16375 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/detail/internals.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    40663 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1486 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/detail/typeid.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    29086 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/eigen.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7843 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/embed.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5079 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/eval.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3709 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/functional.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6532 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/gil.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6084 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/iostream.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    69820 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/numpy.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     9085 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/operators.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2049 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/options.h
+-rw-r--r--   0 vsts      (1001) docker     (122)   105679 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/pybind11.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    67597 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/pytypes.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    14162 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/stl.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    23912 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/stl_bind.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.630403 mmcif-0.81/modules/pybind11_2_6_3_dev1/pybind11/
+-rw-r--r--   0 vsts      (1001) docker     (122)      217 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/pybind11/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1158 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/pybind11/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      207 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/pybind11/_version.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      137 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/pybind11/_version.pyi
+-rw-r--r--   0 vsts      (1001) docker     (122)      663 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/pybind11/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/pybind11/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (122)    15167 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/pybind11/setup_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1899 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/pybind11/setup_helpers.pyi
+-rw-r--r--   0 vsts      (1001) docker     (122)      118 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     2185 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     3499 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.642403 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)    15372 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     4841 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11157 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/constructor_stats.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1819 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1022 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/env.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.642403 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/extra_python_package/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/extra_python_package/pytest.ini
+-rw-r--r--   0 vsts      (1001) docker     (122)     7154 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/extra_python_package/test_files.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.642403 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/extra_setuptools/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0 vsts      (1001) docker     (122)     2581 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2144 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/local_bindings.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5389 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/object.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5285 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     3647 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/pybind11_tests.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     2733 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/pybind11_tests.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      693 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/pytest.ini
+-rw-r--r--   0 vsts      (1001) docker     (122)      843 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      864 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_async.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      558 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_async.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8048 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_buffers.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4946 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_buffers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13475 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_builtin_casters.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    17617 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_builtin_casters.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3702 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_call_policies.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     5728 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_call_policies.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6754 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_callbacks.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     5447 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_callbacks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3406 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_chrono.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     5726 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_chrono.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21548 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_class.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    14273 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_class.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.646404 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2639 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      656 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/embed.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.646404 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1175 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.646404 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1259 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.646404 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1653 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      152 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/main.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.646404 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1357 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.646404 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1126 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.646404 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1333 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/test.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5346 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_constants_and_functions.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1522 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_constants_and_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9629 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_copy_move.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4645 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_copy_move.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5513 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_custom_type_casters.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4015 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_custom_type_casters.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2514 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_docstring_options.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1630 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_docstring_options.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16867 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_eigen.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    28282 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_eigen.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.646404 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_embed/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1758 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      637 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_embed/catch.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      554 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_embed/external_module.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    10209 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      219 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_embed/test_interpreter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2610 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_enum.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     7694 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_enum.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2628 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_eval.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      768 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_eval.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      143 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_eval_call.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7862 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_exceptions.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     6753 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16562 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_factory_constructors.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    16731 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_factory_constructors.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1760 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_gil_scoped.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     3128 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_gil_scoped.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3381 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_iostream.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     5799 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_iostream.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6489 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    10048 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4333 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_local_bindings.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     8102 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_local_bindings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19446 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    17310 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_methods_and_attributes.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3742 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_modules.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     2841 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_modules.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9148 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     9495 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_multiple_inheritance.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17781 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_numpy_array.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    18647 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_numpy_array.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18421 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    13614 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_numpy_dtypes.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3832 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     9709 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_numpy_vectorize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2731 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_opaque_types.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1906 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_opaque_types.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8431 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_operator_overloading.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4136 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_operator_overloading.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4945 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_pickling.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1191 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_pickling.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14656 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_pytypes.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    16590 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_pytypes.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13120 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     5966 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_sequences_and_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18187 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_smart_ptr.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     9620 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_smart_ptr.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12793 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_stl.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     8557 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_stl.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4403 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_stl_binders.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     7182 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_stl_binders.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4458 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      765 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      603 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_union.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      172 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_union.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18454 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_virtual_functions.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    11646 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_virtual_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3238 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0 vsts      (1001) docker     (122)     2657 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/valgrind-python.supp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-08 23:44:22.646404 mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2295 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/FindCatch.cmake
+-rw-r--r--   0 vsts      (1001) docker     (122)     3105 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/FindEigen3.cmake
+-rw-r--r--   0 vsts      (1001) docker     (122)     9977 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1427 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/check-style.sh
+-rw-r--r--   0 vsts      (1001) docker     (122)      952 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1121 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/libsize.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1202 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/make_changelog.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14164 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/pybind11Common.cmake
+-rw-r--r--   0 vsts      (1001) docker     (122)     7010 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/pybind11Config.cmake.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     9173 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/pybind11NewTools.cmake
+-rw-r--r--   0 vsts      (1001) docker     (122)     7276 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/pybind11Tools.cmake
+-rw-r--r--   0 vsts      (1001) docker     (122)       94 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1822 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/setup_global.py.in
+-rw-r--r--   0 vsts      (1001) docker     (122)      915 2023-04-08 23:40:39.000000 mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/setup_main.py.in
+-rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-04-08 23:40:39.000000 mmcif-0.81/requirements-doc.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       13 2023-04-08 23:40:39.000000 mmcif-0.81/requirements-test.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       36 2023-04-08 23:40:39.000000 mmcif-0.81/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-04-08 23:44:22.650404 mmcif-0.81/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     6673 2023-04-08 23:40:39.000000 mmcif-0.81/setup.py
```

### Comparing `mmcif-0.80.1/CMakeLists.txt` & `mmcif-0.81/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/HISTORY.txt` & `mmcif-0.81/HISTORY.txt`

 * *Files 8% similar despite different names*

```diff
@@ -72,7 +72,8 @@
 11-Oct-2021    V0.75 - Add the dictionary API instance as a keyword argument to any invoked method in DictMethodRunner()
 06-Apr-2022    V0.76 - Add doubleQuotingFlag parameter in IoAdapterCore.writeFile() method
 08-Aug-2022    V0.77 - Upgrade macOS version for Azure and tox tasks
 04-Sep-2022    V0.78 - Ensure that data values starting with "stop_" are quoted. Pull in latest versions of modules.
 05-Sep-2022    V0.79 - For IoAdapterPy readFile() method, support timeout parameter for remote URLs
 04-Dec-2022    V0.80 - Add support for Python 3.11
 04-Dec-2022    V0.80.1 - Correct non-wheel build of legacy python
+08-Apr-2023    V0.81 - When using C++ writer, a string with a tab in middle with no other whitespace must be quoted
```

### Comparing `mmcif-0.80.1/LICENSE` & `mmcif-0.81/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/PKG-INFO` & `mmcif-0.81/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcif
-Version: 0.80.1
+Version: 0.81
 Summary: mmCIF Core Access Library
 Home-page: http://mmcif.wwpdb.org
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `mmcif-0.80.1/README.md` & `mmcif-0.81/README.md`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/api/DataCategory.py` & `mmcif-0.81/mmcif/api/DataCategory.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/api/DataCategoryBase.py` & `mmcif-0.81/mmcif/api/DataCategoryBase.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/api/DataCategoryFormatted.py` & `mmcif-0.81/mmcif/api/DataCategoryFormatted.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/api/DataCategoryTyped.py` & `mmcif-0.81/mmcif/api/DataCategoryTyped.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/api/DictMethodRunner.py` & `mmcif-0.81/mmcif/api/DictMethodRunner.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/api/DictionaryApi.py` & `mmcif-0.81/mmcif/api/DictionaryApi.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/api/DictionaryInclude.py` & `mmcif-0.81/mmcif/api/DictionaryInclude.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/api/Method.py` & `mmcif-0.81/mmcif/api/Method.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/api/MethodUtils.py` & `mmcif-0.81/mmcif/api/MethodUtils.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/api/PdbxContainers.py` & `mmcif-0.81/mmcif/api/PdbxContainers.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/io/BinaryCifReader.py` & `mmcif-0.81/mmcif/io/BinaryCifReader.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/io/BinaryCifWriter.py` & `mmcif-0.81/mmcif/io/BinaryCifWriter.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/io/BuildDictionaryExec.py` & `mmcif-0.81/mmcif/io/BuildDictionaryExec.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/io/CifFile.py` & `mmcif-0.81/mmcif/io/CifFile.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/io/IoAdapterBase.py` & `mmcif-0.81/mmcif/io/IoAdapterBase.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/io/IoAdapterCore.py` & `mmcif-0.81/mmcif/io/IoAdapterCore.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/io/IoAdapterPy.py` & `mmcif-0.81/mmcif/io/IoAdapterPy.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/io/PdbxExceptions.py` & `mmcif-0.81/mmcif/io/PdbxExceptions.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/io/PdbxReader.py` & `mmcif-0.81/mmcif/io/PdbxReader.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif/io/PdbxWriter.py` & `mmcif-0.81/mmcif/io/PdbxWriter.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/mmcif.egg-info/PKG-INFO` & `mmcif-0.81/mmcif.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcif
-Version: 0.80.1
+Version: 0.81
 Summary: mmCIF Core Access Library
 Home-page: http://mmcif.wwpdb.org
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `mmcif-0.80.1/mmcif.egg-info/SOURCES.txt` & `mmcif-0.81/mmcif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cc-regex/include/cclass.h` & `mmcif-0.81/modules/cc-regex/include/cclass.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cc-regex/include/cname.h` & `mmcif-0.81/modules/cc-regex/include/cname.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cc-regex/include/engine.ih` & `mmcif-0.81/modules/cc-regex/include/engine.ih`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cc-regex/include/regcomp.ih` & `mmcif-0.81/modules/cc-regex/include/regcomp.ih`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cc-regex/include/regex.h` & `mmcif-0.81/modules/cc-regex/include/regex.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cc-regex/include/regex2.h` & `mmcif-0.81/modules/cc-regex/include/regex2.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cc-regex/src/debug.c` & `mmcif-0.81/modules/cc-regex/src/debug.c`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cc-regex/src/engine.c` & `mmcif-0.81/modules/cc-regex/src/engine.c`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cc-regex/src/main.c` & `mmcif-0.81/modules/cc-regex/src/main.c`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cc-regex/src/mkh` & `mmcif-0.81/modules/cc-regex/src/mkh`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cc-regex/src/regcomp.c` & `mmcif-0.81/modules/cc-regex/src/regcomp.c`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cc-regex/src/regerror.c` & `mmcif-0.81/modules/cc-regex/src/regerror.c`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cc-regex/src/regexec.c` & `mmcif-0.81/modules/cc-regex/src/regexec.c`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cc-regex/src/regfree.c` & `mmcif-0.81/modules/cc-regex/src/regfree.c`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cc-regex/src/split.c` & `mmcif-0.81/modules/cc-regex/src/split.c`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-file/include/CifDataInfo.h` & `mmcif-0.81/modules/cpp-cif-file/include/CifDataInfo.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-file/include/CifExcept.h` & `mmcif-0.81/modules/cpp-cif-file/include/CifExcept.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-file/include/CifFile.h` & `mmcif-0.81/modules/cpp-cif-file/include/CifFile.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-file/include/CifParentChild.h` & `mmcif-0.81/modules/cpp-cif-file/include/CifParentChild.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-file/include/DicFile.h` & `mmcif-0.81/modules/cpp-cif-file/include/DicFile.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-file/include/ParentChild.h` & `mmcif-0.81/modules/cpp-cif-file/include/ParentChild.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-file/src/CifDataInfo.C` & `mmcif-0.81/modules/cpp-cif-file/src/CifDataInfo.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-file/src/CifExcept.C` & `mmcif-0.81/modules/cpp-cif-file/src/CifExcept.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-file/src/CifFile.C` & `mmcif-0.81/modules/cpp-cif-file/src/CifFile.C`

 * *Files 0% similar despite different names*

```diff
@@ -409,14 +409,17 @@
       return(1);
 
   for (unsigned int i = 0; i < itemValue.size(); i++)
   {
       if (itemValue[i] == ' ')
           return(1);
 
+      if (itemValue[i] == '\t')
+          return(1);
+      
       if (itemValue[i] == '\n')
           return(1);
 
       if (itemValue[i] == '\'' || itemValue[i] == '\"')
           return(1);
 
       if (i == 0)
@@ -609,15 +612,15 @@
     embeddedDoubleQuotes = false;
     bool specialChars = false;
 
     string multipleWordQuotes = _quotes;
 
     for (unsigned int i = 0; i < str_len; i++)
     {
-        if (itemValue[i] == ' ')
+        if (itemValue[i] == ' ' || itemValue[i] == '\t')
             multipleWord = true;
         else if (itemValue[i] == '\n')
             multipleLine = true;
         else if (itemValue[i] == '\'')
         {
             embeddedSingleQuotes = true;
             embeddedQuotes = true;
```

### Comparing `mmcif-0.80.1/modules/cpp-cif-file/src/CifParentChild.C` & `mmcif-0.81/modules/cpp-cif-file/src/CifParentChild.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-file/src/DicFile.C` & `mmcif-0.81/modules/cpp-cif-file/src/DicFile.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-file/src/ParentChild.C` & `mmcif-0.81/modules/cpp-cif-file/src/ParentChild.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-file-util/include/CifCorrector.h` & `mmcif-0.81/modules/cpp-cif-file-util/include/CifCorrector.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-file-util/include/CifFileUtil.h` & `mmcif-0.81/modules/cpp-cif-file-util/include/CifFileUtil.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-file-util/src/CifCorrector.C` & `mmcif-0.81/modules/cpp-cif-file-util/src/CifCorrector.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-file-util/src/CifFileUtil.C` & `mmcif-0.81/modules/cpp-cif-file-util/src/CifFileUtil.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-parser/include/CifFileReadDef.h` & `mmcif-0.81/modules/cpp-cif-parser/include/CifFileReadDef.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-parser/include/CifParserBase.h` & `mmcif-0.81/modules/cpp-cif-parser/include/CifParserBase.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-parser/include/CifParserInt.h` & `mmcif-0.81/modules/cpp-cif-parser/include/CifParserInt.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-parser/include/CifScannerBase.h` & `mmcif-0.81/modules/cpp-cif-parser/include/CifScannerBase.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-parser/include/CifScannerInt.h` & `mmcif-0.81/modules/cpp-cif-parser/include/CifScannerInt.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-parser/include/DICParserBase.h` & `mmcif-0.81/modules/cpp-cif-parser/include/DICParserBase.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-parser/include/DICParserInt.h` & `mmcif-0.81/modules/cpp-cif-parser/include/DICParserInt.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-parser/include/DICScannerBase.h` & `mmcif-0.81/modules/cpp-cif-parser/include/DICScannerBase.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-parser/include/DICScannerInt.h` & `mmcif-0.81/modules/cpp-cif-parser/include/DICScannerInt.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-parser/src/CifFileReadDef.C` & `mmcif-0.81/modules/cpp-cif-parser/src/CifFileReadDef.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-parser/src/CifParser.y` & `mmcif-0.81/modules/cpp-cif-parser/src/CifParser.y`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-parser/src/CifParserBase.C` & `mmcif-0.81/modules/cpp-cif-parser/src/CifParserBase.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-parser/src/CifScanner.l` & `mmcif-0.81/modules/cpp-cif-parser/src/CifScanner.l`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-parser/src/CifScannerBase.C` & `mmcif-0.81/modules/cpp-cif-parser/src/CifScannerBase.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-parser/src/DICParser.y` & `mmcif-0.81/modules/cpp-cif-parser/src/DICParser.y`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-parser/src/DICParserBase.C` & `mmcif-0.81/modules/cpp-cif-parser/src/DICParserBase.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-parser/src/DICScanner.l` & `mmcif-0.81/modules/cpp-cif-parser/src/DICScanner.l`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-cif-parser/src/DICScannerBase.C` & `mmcif-0.81/modules/cpp-cif-parser/src/DICScannerBase.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/include/BlockIO.h` & `mmcif-0.81/modules/cpp-common/include/BlockIO.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/include/CifDefs.h` & `mmcif-0.81/modules/cpp-common/include/CifDefs.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/include/CifString.h` & `mmcif-0.81/modules/cpp-common/include/CifString.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/include/DataInfo.h` & `mmcif-0.81/modules/cpp-common/include/DataInfo.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/include/Exceptions.h` & `mmcif-0.81/modules/cpp-common/include/Exceptions.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/include/GenCont.h` & `mmcif-0.81/modules/cpp-common/include/GenCont.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/include/GenString.h` & `mmcif-0.81/modules/cpp-common/include/GenString.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/include/Serializer.h` & `mmcif-0.81/modules/cpp-common/include/Serializer.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/include/mapped_ptr_vector.h` & `mmcif-0.81/modules/cpp-common/include/mapped_ptr_vector.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/include/mapped_vector.h` & `mmcif-0.81/modules/cpp-common/include/mapped_vector.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/include/rcsb_types.h` & `mmcif-0.81/modules/cpp-common/include/rcsb_types.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/src/BlockIO.C` & `mmcif-0.81/modules/cpp-common/src/BlockIO.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/src/CifString.C` & `mmcif-0.81/modules/cpp-common/src/CifString.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/src/DataInfo.C` & `mmcif-0.81/modules/cpp-common/src/DataInfo.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/src/Exceptions.C` & `mmcif-0.81/modules/cpp-common/src/Exceptions.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/src/GenCont.C` & `mmcif-0.81/modules/cpp-common/src/GenCont.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/src/GenString.C` & `mmcif-0.81/modules/cpp-common/src/GenString.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/src/RcsbFile.C` & `mmcif-0.81/modules/cpp-common/src/RcsbFile.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/src/Serializer.C` & `mmcif-0.81/modules/cpp-common/src/Serializer.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/src/mapped_ptr_vector.C` & `mmcif-0.81/modules/cpp-common/src/mapped_ptr_vector.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-common/src/mapped_vector.C` & `mmcif-0.81/modules/cpp-common/src/mapped_vector.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifDataInfo.cpp` & `mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifDataInfo.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFile.cpp` & `mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFile.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFileReadDef.cpp` & `mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFileReadDef.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFileUtil.cpp` & `mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFileUtil.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wrapDicFile.cpp` & `mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wrapDicFile.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wrapDictDataInfo.cpp` & `mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wrapDictDataInfo.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wrapISTable.cpp` & `mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wrapISTable.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wrapTableFile.cpp` & `mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wrapTableFile.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wrapmmciflib.cpp` & `mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wrapmmciflib.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-core-mmciflib-wrapper-gen/src/wraprcsb_types.cpp` & `mmcif-0.81/modules/cpp-core-mmciflib-wrapper-gen/src/wraprcsb_types.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-dict-obj-file/include/DictDataInfo.h` & `mmcif-0.81/modules/cpp-dict-obj-file/include/DictDataInfo.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-dict-obj-file/include/DictObjCont.h` & `mmcif-0.81/modules/cpp-dict-obj-file/include/DictObjCont.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-dict-obj-file/include/DictObjContInfo.h` & `mmcif-0.81/modules/cpp-dict-obj-file/include/DictObjContInfo.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-dict-obj-file/include/DictObjFile.h` & `mmcif-0.81/modules/cpp-dict-obj-file/include/DictObjFile.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-dict-obj-file/include/DictParentChild.h` & `mmcif-0.81/modules/cpp-dict-obj-file/include/DictParentChild.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-dict-obj-file/src/DictDataInfo.C` & `mmcif-0.81/modules/cpp-dict-obj-file/src/DictDataInfo.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-dict-obj-file/src/DictObjCont.C` & `mmcif-0.81/modules/cpp-dict-obj-file/src/DictObjCont.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-dict-obj-file/src/DictObjContInfo.C` & `mmcif-0.81/modules/cpp-dict-obj-file/src/DictObjContInfo.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-dict-obj-file/src/DictObjFile.C` & `mmcif-0.81/modules/cpp-dict-obj-file/src/DictObjFile.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-dict-obj-file/src/DictObjFileCreator.C` & `mmcif-0.81/modules/cpp-dict-obj-file/src/DictObjFileCreator.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-dict-obj-file/src/DictObjFileReader.C` & `mmcif-0.81/modules/cpp-dict-obj-file/src/DictObjFileReader.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-dict-obj-file/src/DictObjFileSelectiveReader.C` & `mmcif-0.81/modules/cpp-dict-obj-file/src/DictObjFileSelectiveReader.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-dict-obj-file/src/DictParentChild.C` & `mmcif-0.81/modules/cpp-dict-obj-file/src/DictParentChild.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/BigCifTest.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/BigCifTest.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/CifDiff.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/CifDiff.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/CifInfo.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/CifInfo.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/CifReader.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/CifReader.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/DataChecking.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/DataChecking.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/DictInfo.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/DictInfo.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest1.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest1.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest10.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest10.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest11.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest11.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest12.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest12.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest13.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest13.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest14.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest14.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest2.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest2.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest3.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest3.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest4.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest4.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest5.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest5.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest6.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest6.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest7.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest7.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/FOtest9.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/FOtest9.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/GroupTableTest2.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/GroupTableTest2.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/SdbReader.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/SdbReader.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/checkdictionary.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/checkdictionary.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-mmciflib-test/src/selective-reading.C` & `mmcif-0.81/modules/cpp-mmciflib-test/src/selective-reading.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-tables/include/ISTable.h` & `mmcif-0.81/modules/cpp-tables/include/ISTable.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-tables/include/ITTable.h` & `mmcif-0.81/modules/cpp-tables/include/ITTable.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-tables/include/TTable.h` & `mmcif-0.81/modules/cpp-tables/include/TTable.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-tables/include/TableError.h` & `mmcif-0.81/modules/cpp-tables/include/TableError.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-tables/include/TableFile.h` & `mmcif-0.81/modules/cpp-tables/include/TableFile.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-tables/src/ISTable.C` & `mmcif-0.81/modules/cpp-tables/src/ISTable.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-tables/src/ITTable.C` & `mmcif-0.81/modules/cpp-tables/src/ITTable.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-tables/src/TTable.C` & `mmcif-0.81/modules/cpp-tables/src/TTable.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/cpp-tables/src/TableFile.C` & `mmcif-0.81/modules/cpp-tables/src/TableFile.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/.appveyor.yml` & `mmcif-0.81/modules/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/.clang-format` & `mmcif-0.81/modules/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/.clang-tidy` & `mmcif-0.81/modules/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/.cmake-format.yaml` & `mmcif-0.81/modules/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/.codespell-ignore-lines` & `mmcif-0.81/modules/pybind11/.codespell-ignore-lines`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/.github/CONTRIBUTING.md` & `mmcif-0.81/modules/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml` & `mmcif-0.81/modules/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/.github/matchers/pylint.json` & `mmcif-0.81/modules/pybind11/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/.github/pull_request_template.md` & `mmcif-0.81/modules/pybind11/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/.github/workflows/ci.yml` & `mmcif-0.81/modules/pybind11/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/.github/workflows/configure.yml` & `mmcif-0.81/modules/pybind11/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/.github/workflows/format.yml` & `mmcif-0.81/modules/pybind11/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/.github/workflows/pip.yml` & `mmcif-0.81/modules/pybind11/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/.github/workflows/upstream.yml` & `mmcif-0.81/modules/pybind11/.github/workflows/upstream.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/.pre-commit-config.yaml` & `mmcif-0.81/modules/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/CMakeLists.txt` & `mmcif-0.81/modules/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/LICENSE` & `mmcif-0.81/modules/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/README.rst` & `mmcif-0.81/modules/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/Doxyfile` & `mmcif-0.81/modules/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/Makefile` & `mmcif-0.81/modules/pybind11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/advanced/cast/chrono.rst` & `mmcif-0.81/modules/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/advanced/cast/custom.rst` & `mmcif-0.81/modules/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/advanced/cast/eigen.rst` & `mmcif-0.81/modules/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/advanced/cast/functional.rst` & `mmcif-0.81/modules/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/advanced/cast/index.rst` & `mmcif-0.81/modules/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/advanced/cast/overview.rst` & `mmcif-0.81/modules/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/advanced/cast/stl.rst` & `mmcif-0.81/modules/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/advanced/cast/strings.rst` & `mmcif-0.81/modules/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/advanced/classes.rst` & `mmcif-0.81/modules/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/advanced/embedding.rst` & `mmcif-0.81/modules/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/advanced/exceptions.rst` & `mmcif-0.81/modules/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/advanced/functions.rst` & `mmcif-0.81/modules/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/advanced/misc.rst` & `mmcif-0.81/modules/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/advanced/pycpp/numpy.rst` & `mmcif-0.81/modules/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/advanced/pycpp/object.rst` & `mmcif-0.81/modules/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/advanced/pycpp/utilities.rst` & `mmcif-0.81/modules/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/advanced/smart_ptrs.rst` & `mmcif-0.81/modules/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/basics.rst` & `mmcif-0.81/modules/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/benchmark.py` & `mmcif-0.81/modules/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/benchmark.rst` & `mmcif-0.81/modules/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/changelog.rst` & `mmcif-0.81/modules/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/classes.rst` & `mmcif-0.81/modules/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/compiling.rst` & `mmcif-0.81/modules/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/conf.py` & `mmcif-0.81/modules/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/faq.rst` & `mmcif-0.81/modules/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/index.rst` & `mmcif-0.81/modules/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/installing.rst` & `mmcif-0.81/modules/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/limitations.rst` & `mmcif-0.81/modules/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/pybind11-logo.png` & `mmcif-0.81/modules/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/pybind11_vs_boost_python1.png` & `mmcif-0.81/modules/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/pybind11_vs_boost_python1.svg` & `mmcif-0.81/modules/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/pybind11_vs_boost_python2.png` & `mmcif-0.81/modules/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/pybind11_vs_boost_python2.svg` & `mmcif-0.81/modules/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/reference.rst` & `mmcif-0.81/modules/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/release.rst` & `mmcif-0.81/modules/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/docs/upgrade.rst` & `mmcif-0.81/modules/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/attr.h` & `mmcif-0.81/modules/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/buffer_info.h` & `mmcif-0.81/modules/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/cast.h` & `mmcif-0.81/modules/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/chrono.h` & `mmcif-0.81/modules/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/complex.h` & `mmcif-0.81/modules/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/detail/class.h` & `mmcif-0.81/modules/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/detail/common.h` & `mmcif-0.81/modules/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/detail/descr.h` & `mmcif-0.81/modules/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/detail/init.h` & `mmcif-0.81/modules/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/detail/internals.h` & `mmcif-0.81/modules/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/detail/type_caster_base.h` & `mmcif-0.81/modules/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/detail/typeid.h` & `mmcif-0.81/modules/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/eigen.h` & `mmcif-0.81/modules/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/embed.h` & `mmcif-0.81/modules/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/eval.h` & `mmcif-0.81/modules/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/functional.h` & `mmcif-0.81/modules/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/gil.h` & `mmcif-0.81/modules/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/iostream.h` & `mmcif-0.81/modules/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/numpy.h` & `mmcif-0.81/modules/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/operators.h` & `mmcif-0.81/modules/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/options.h` & `mmcif-0.81/modules/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/pybind11.h` & `mmcif-0.81/modules/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/pytypes.h` & `mmcif-0.81/modules/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/stl/filesystem.h` & `mmcif-0.81/modules/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/stl.h` & `mmcif-0.81/modules/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/include/pybind11/stl_bind.h` & `mmcif-0.81/modules/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/noxfile.py` & `mmcif-0.81/modules/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/pybind11/__main__.py` & `mmcif-0.81/modules/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/pybind11/commands.py` & `mmcif-0.81/modules/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/pybind11/setup_helpers.py` & `mmcif-0.81/modules/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/pyproject.toml` & `mmcif-0.81/modules/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/setup.cfg` & `mmcif-0.81/modules/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/setup.py` & `mmcif-0.81/modules/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/CMakeLists.txt` & `mmcif-0.81/modules/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/conftest.py` & `mmcif-0.81/modules/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/constructor_stats.h` & `mmcif-0.81/modules/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/cross_module_gil_utils.cpp` & `mmcif-0.81/modules/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/cross_module_interleaved_error_already_set.cpp` & `mmcif-0.81/modules/pybind11/tests/cross_module_interleaved_error_already_set.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/env.py` & `mmcif-0.81/modules/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/extra_python_package/test_files.py` & `mmcif-0.81/modules/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/extra_setuptools/test_setuphelper.py` & `mmcif-0.81/modules/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/local_bindings.h` & `mmcif-0.81/modules/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/object.h` & `mmcif-0.81/modules/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/pybind11_cross_module_tests.cpp` & `mmcif-0.81/modules/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/pybind11_tests.cpp` & `mmcif-0.81/modules/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/pybind11_tests.h` & `mmcif-0.81/modules/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/pytest.ini` & `mmcif-0.81/modules/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/requirements.txt` & `mmcif-0.81/modules/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_async.cpp` & `mmcif-0.81/modules/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_async.py` & `mmcif-0.81/modules/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_buffers.cpp` & `mmcif-0.81/modules/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_buffers.py` & `mmcif-0.81/modules/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_builtin_casters.cpp` & `mmcif-0.81/modules/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_builtin_casters.py` & `mmcif-0.81/modules/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_call_policies.cpp` & `mmcif-0.81/modules/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_call_policies.py` & `mmcif-0.81/modules/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_callbacks.cpp` & `mmcif-0.81/modules/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_callbacks.py` & `mmcif-0.81/modules/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_chrono.cpp` & `mmcif-0.81/modules/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_chrono.py` & `mmcif-0.81/modules/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_class.cpp` & `mmcif-0.81/modules/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_class.py` & `mmcif-0.81/modules/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/CMakeLists.txt` & `mmcif-0.81/modules/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/embed.cpp` & `mmcif-0.81/modules/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `mmcif-0.81/modules/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `mmcif-0.81/modules/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `mmcif-0.81/modules/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `mmcif-0.81/modules/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `mmcif-0.81/modules/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `mmcif-0.81/modules/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_const_name.cpp` & `mmcif-0.81/modules/pybind11/tests/test_const_name.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_const_name.py` & `mmcif-0.81/modules/pybind11/tests/test_const_name.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_constants_and_functions.cpp` & `mmcif-0.81/modules/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_constants_and_functions.py` & `mmcif-0.81/modules/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_copy_move.cpp` & `mmcif-0.81/modules/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_copy_move.py` & `mmcif-0.81/modules/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_custom_type_casters.cpp` & `mmcif-0.81/modules/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_custom_type_casters.py` & `mmcif-0.81/modules/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_custom_type_setup.cpp` & `mmcif-0.81/modules/pybind11/tests/test_custom_type_setup.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_custom_type_setup.py` & `mmcif-0.81/modules/pybind11/tests/test_custom_type_setup.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_docstring_options.cpp` & `mmcif-0.81/modules/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_docstring_options.py` & `mmcif-0.81/modules/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_eigen.cpp` & `mmcif-0.81/modules/pybind11/tests/test_eigen.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_eigen.py` & `mmcif-0.81/modules/pybind11/tests/test_eigen.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_embed/CMakeLists.txt` & `mmcif-0.81/modules/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_embed/catch.cpp` & `mmcif-0.81/modules/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_embed/external_module.cpp` & `mmcif-0.81/modules/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_embed/test_interpreter.cpp` & `mmcif-0.81/modules/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_enum.cpp` & `mmcif-0.81/modules/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_enum.py` & `mmcif-0.81/modules/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_eval.cpp` & `mmcif-0.81/modules/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_eval.py` & `mmcif-0.81/modules/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_exceptions.cpp` & `mmcif-0.81/modules/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_exceptions.py` & `mmcif-0.81/modules/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_factory_constructors.cpp` & `mmcif-0.81/modules/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_factory_constructors.py` & `mmcif-0.81/modules/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_gil_scoped.cpp` & `mmcif-0.81/modules/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_gil_scoped.py` & `mmcif-0.81/modules/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_iostream.cpp` & `mmcif-0.81/modules/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_iostream.py` & `mmcif-0.81/modules/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_kwargs_and_defaults.cpp` & `mmcif-0.81/modules/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_kwargs_and_defaults.py` & `mmcif-0.81/modules/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_local_bindings.cpp` & `mmcif-0.81/modules/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_local_bindings.py` & `mmcif-0.81/modules/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_methods_and_attributes.cpp` & `mmcif-0.81/modules/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_methods_and_attributes.py` & `mmcif-0.81/modules/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_modules.cpp` & `mmcif-0.81/modules/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_modules.py` & `mmcif-0.81/modules/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_multiple_inheritance.cpp` & `mmcif-0.81/modules/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_multiple_inheritance.py` & `mmcif-0.81/modules/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_numpy_array.cpp` & `mmcif-0.81/modules/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_numpy_array.py` & `mmcif-0.81/modules/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_numpy_dtypes.cpp` & `mmcif-0.81/modules/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_numpy_dtypes.py` & `mmcif-0.81/modules/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_numpy_vectorize.cpp` & `mmcif-0.81/modules/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_numpy_vectorize.py` & `mmcif-0.81/modules/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_opaque_types.cpp` & `mmcif-0.81/modules/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_opaque_types.py` & `mmcif-0.81/modules/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_operator_overloading.cpp` & `mmcif-0.81/modules/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_operator_overloading.py` & `mmcif-0.81/modules/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_pickling.cpp` & `mmcif-0.81/modules/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_pickling.py` & `mmcif-0.81/modules/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_pytypes.cpp` & `mmcif-0.81/modules/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_pytypes.py` & `mmcif-0.81/modules/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_sequences_and_iterators.cpp` & `mmcif-0.81/modules/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_sequences_and_iterators.py` & `mmcif-0.81/modules/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_smart_ptr.cpp` & `mmcif-0.81/modules/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_smart_ptr.py` & `mmcif-0.81/modules/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_stl.cpp` & `mmcif-0.81/modules/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_stl.py` & `mmcif-0.81/modules/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_stl_binders.cpp` & `mmcif-0.81/modules/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_stl_binders.py` & `mmcif-0.81/modules/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_tagbased_polymorphic.cpp` & `mmcif-0.81/modules/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_tagbased_polymorphic.py` & `mmcif-0.81/modules/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_thread.cpp` & `mmcif-0.81/modules/pybind11/tests/test_thread.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_thread.py` & `mmcif-0.81/modules/pybind11/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_union.cpp` & `mmcif-0.81/modules/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_virtual_functions.cpp` & `mmcif-0.81/modules/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/test_virtual_functions.py` & `mmcif-0.81/modules/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/valgrind-numpy-scipy.supp` & `mmcif-0.81/modules/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tests/valgrind-python.supp` & `mmcif-0.81/modules/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tools/FindCatch.cmake` & `mmcif-0.81/modules/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tools/FindEigen3.cmake` & `mmcif-0.81/modules/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tools/FindPythonLibsNew.cmake` & `mmcif-0.81/modules/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tools/JoinPaths.cmake` & `mmcif-0.81/modules/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tools/check-style.sh` & `mmcif-0.81/modules/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tools/cmake_uninstall.cmake.in` & `mmcif-0.81/modules/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tools/codespell_ignore_lines_from_errors.py` & `mmcif-0.81/modules/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tools/libsize.py` & `mmcif-0.81/modules/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tools/make_changelog.py` & `mmcif-0.81/modules/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tools/pybind11Common.cmake` & `mmcif-0.81/modules/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tools/pybind11Config.cmake.in` & `mmcif-0.81/modules/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tools/pybind11NewTools.cmake` & `mmcif-0.81/modules/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tools/pybind11Tools.cmake` & `mmcif-0.81/modules/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tools/setup_global.py.in` & `mmcif-0.81/modules/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11/tools/setup_main.py.in` & `mmcif-0.81/modules/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.appveyor.yml` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.clang-format` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/.clang-format`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.cmake-format.yaml` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/CONTRIBUTING.md` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/bug-report.md` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/feature-request.md` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/question.md` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/dependabot.yml` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/workflows/ci.yml` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/workflows/configure.yml` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/workflows/format.yml` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.github/workflows/pip.yml` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/.pre-commit-config.yaml` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/CMakeLists.txt` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/LICENSE` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/README.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/README.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/Doxyfile` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/cast/chrono.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/cast/custom.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/cast/eigen.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/cast/functional.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/cast/index.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/cast/overview.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/cast/stl.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/cast/strings.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/classes.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/embedding.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/exceptions.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/functions.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/misc.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/numpy.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/object.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/utilities.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/advanced/smart_ptrs.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/basics.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/benchmark.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/benchmark.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/changelog.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/classes.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/compiling.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/conf.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/faq.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/index.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/installing.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/limitations.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/pybind11-logo.png` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python1.png` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python1.svg` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python2.png` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python2.svg` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/reference.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/release.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/release.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/docs/upgrade.rst` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/attr.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/buffer_info.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/cast.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/chrono.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/complex.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/detail/class.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/detail/common.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/detail/descr.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/detail/init.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/detail/internals.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/detail/type_caster_base.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/detail/typeid.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/eigen.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/embed.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/eval.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/functional.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/gil.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/iostream.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/numpy.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/operators.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/options.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/pybind11.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/pytypes.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/stl.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/include/pybind11/stl_bind.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/pybind11/__main__.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/pybind11/commands.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/pybind11/setup_helpers.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/pybind11/setup_helpers.pyi` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/pybind11/setup_helpers.pyi`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/setup.cfg` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/setup.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/setup.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/CMakeLists.txt` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/conftest.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/constructor_stats.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/cross_module_gil_utils.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/env.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/env.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/extra_python_package/test_files.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/extra_setuptools/test_setuphelper.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/local_bindings.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/object.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/object.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/pybind11_cross_module_tests.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/pybind11_tests.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/pybind11_tests.h` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/pytest.ini` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/requirements.txt` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_async.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_async.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_buffers.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_buffers.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_builtin_casters.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_builtin_casters.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_call_policies.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_call_policies.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_callbacks.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_callbacks.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_chrono.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_chrono.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_class.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_class.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/CMakeLists.txt` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/embed.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_function/CMakeLists.txt` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_target/CMakeLists.txt` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_constants_and_functions.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_constants_and_functions.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_copy_move.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_copy_move.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_custom_type_casters.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_custom_type_casters.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_docstring_options.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_docstring_options.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_eigen.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_eigen.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_eigen.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_eigen.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_embed/CMakeLists.txt` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_embed/catch.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_embed/external_module.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_embed/test_interpreter.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_enum.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_enum.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_eval.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_eval.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_exceptions.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_exceptions.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_factory_constructors.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_factory_constructors.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_gil_scoped.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_gil_scoped.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_iostream.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_iostream.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_kwargs_and_defaults.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_kwargs_and_defaults.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_local_bindings.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_local_bindings.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_methods_and_attributes.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_methods_and_attributes.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_modules.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_modules.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_multiple_inheritance.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_multiple_inheritance.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_numpy_array.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_numpy_array.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_numpy_dtypes.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_numpy_dtypes.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_numpy_vectorize.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_numpy_vectorize.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_opaque_types.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_opaque_types.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_operator_overloading.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_operator_overloading.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_pickling.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_pickling.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_pytypes.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_pytypes.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_sequences_and_iterators.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_sequences_and_iterators.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_smart_ptr.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_smart_ptr.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_stl.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_stl.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_stl_binders.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_stl_binders.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_tagbased_polymorphic.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_tagbased_polymorphic.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_union.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_virtual_functions.cpp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/test_virtual_functions.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/valgrind-numpy-scipy.supp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tests/valgrind-python.supp` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/FindCatch.cmake` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/FindEigen3.cmake` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/FindPythonLibsNew.cmake` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/check-style.sh` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/cmake_uninstall.cmake.in` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/libsize.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/make_changelog.py` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/pybind11Common.cmake` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/pybind11Config.cmake.in` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/pybind11NewTools.cmake` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/pybind11Tools.cmake` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/setup_global.py.in` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/modules/pybind11_2_6_3_dev1/tools/setup_main.py.in` & `mmcif-0.81/modules/pybind11_2_6_3_dev1/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `mmcif-0.80.1/setup.py` & `mmcif-0.81/setup.py`

 * *Files identical despite different names*

