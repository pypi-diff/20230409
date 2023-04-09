# Comparing `tmp/apache-age-community-detection-0.1.3.tar.gz` & `tmp/apache-age-community-detection-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-age-community-detection-0.1.3.tar", last modified: Sun Apr  9 13:41:59 2023, max compression
+gzip compressed data, was "apache-age-community-detection-0.1.4.tar", last modified: Sun Apr  9 16:20:08 2023, max compression
```

## Comparing `apache-age-community-detection-0.1.3.tar` & `apache-age-community-detection-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:41:59.131273 apache-age-community-detection-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-09 13:41:59.131273 apache-age-community-detection-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:41:59.131273 apache-age-community-detection-0.1.3/age_community_detection/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/age_community_detection/Check.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/age_community_detection/Exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/age_community_detection/Graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/age_community_detection/Lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/age_community_detection/VERSION.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/age_community_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:41:59.131273 apache-age-community-detection-0.1.3/age_community_detection/lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)    17112 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/age_community_detection/lib/library.dll
--rwxr-xr-x   0 runner    (1001) docker     (123)    17112 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/age_community_detection/lib/library.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:41:59.131273 apache-age-community-detection-0.1.3/apache_age_community_detection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-09 13:41:59.000000 apache-age-community-detection-0.1.3/apache_age_community_detection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-09 13:41:59.000000 apache-age-community-detection-0.1.3/apache_age_community_detection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 13:41:59.000000 apache-age-community-detection-0.1.3/apache_age_community_detection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 13:41:59.000000 apache-age-community-detection-0.1.3/apache_age_community_detection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-09 13:41:59.000000 apache-age-community-detection-0.1.3/apache_age_community_detection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 13:41:59.131273 apache-age-community-detection-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:20:08.378665 apache-age-community-detection-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-09 16:19:57.000000 apache-age-community-detection-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-09 16:20:08.378665 apache-age-community-detection-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-09 16:19:57.000000 apache-age-community-detection-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:20:08.374665 apache-age-community-detection-0.1.4/age_community_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-09 16:19:57.000000 apache-age-community-detection-0.1.4/age_community_detection/Check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-09 16:19:57.000000 apache-age-community-detection-0.1.4/age_community_detection/Exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 16:19:57.000000 apache-age-community-detection-0.1.4/age_community_detection/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-09 16:19:57.000000 apache-age-community-detection-0.1.4/age_community_detection/Lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-09 16:19:57.000000 apache-age-community-detection-0.1.4/age_community_detection/VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-09 16:19:57.000000 apache-age-community-detection-0.1.4/age_community_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:20:08.374665 apache-age-community-detection-0.1.4/age_community_detection/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17160 2023-04-09 16:19:57.000000 apache-age-community-detection-0.1.4/age_community_detection/lib/library.dll
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17160 2023-04-09 16:19:57.000000 apache-age-community-detection-0.1.4/age_community_detection/lib/library.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:20:08.378665 apache-age-community-detection-0.1.4/apache_age_community_detection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-09 16:20:08.000000 apache-age-community-detection-0.1.4/apache_age_community_detection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-09 16:20:08.000000 apache-age-community-detection-0.1.4/apache_age_community_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 16:20:08.000000 apache-age-community-detection-0.1.4/apache_age_community_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-09 16:20:08.000000 apache-age-community-detection-0.1.4/apache_age_community_detection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 16:20:08.378665 apache-age-community-detection-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-09 16:19:57.000000 apache-age-community-detection-0.1.4/setup.py
```

### Comparing `apache-age-community-detection-0.1.3/LICENSE` & `apache-age-community-detection-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.3/PKG-INFO` & `apache-age-community-detection-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-age-community-detection
-Version: 0.1.3
+Version: 0.1.4
 Summary: Detection of Community by maximizing modularity
 Home-page: https://github.com/Munmud/Community-Detection-Modularity
 Author: Moontasir Mahmood
 Author-email: moontasir042@gmail.com
 License: Apache2.0
 Keywords: Community-Detection,Modularity,Reichardt and Bornholdt,Newman,partition network,k means cluster
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `apache-age-community-detection-0.1.3/README.md` & `apache-age-community-detection-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.3/age_community_detection/Check.py` & `apache-age-community-detection-0.1.4/age_community_detection/Check.py`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.3/age_community_detection/Exception.py` & `apache-age-community-detection-0.1.4/age_community_detection/Exception.py`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.3/age_community_detection/Graph.py` & `apache-age-community-detection-0.1.4/age_community_detection/Graph.py`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.3/age_community_detection/lib/library.dll` & `apache-age-community-detection-0.1.4/age_community_detection/lib/library.dll`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 8% similar despite different names*

#### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              DYN (Shared object file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          64 (bytes into file)
-  Start of section headers:          15192 (bytes into file)
+  Start of section headers:          15240 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           56 (bytes)
   Number of program headers:         11
   Size of section headers:           64 (bytes)
   Number of section headers:         30
   Section header string table index: 29
```

#### readelf --wide --program-header {}

```diff
@@ -1,23 +1,23 @@
 
 Elf file type is DYN (Shared object file)
 Entry point 0x0
 There are 11 program headers, starting at offset 64
 
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
-  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x000ca0 0x000ca0 R   0x1000
-  LOAD           0x001000 0x0000000000001000 0x0000000000001000 0x000e31 0x000e31 R E 0x1000
-  LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x0003f4 0x0003f4 R   0x1000
+  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x000ce0 0x000ce0 R   0x1000
+  LOAD           0x001000 0x0000000000001000 0x0000000000001000 0x000e4d 0x000e4d R E 0x1000
+  LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x00040c 0x00040c R   0x1000
   LOAD           0x002e00 0x0000000000003e00 0x0000000000003e00 0x0002f8 0x000300 RW  0x1000
   DYNAMIC        0x002e10 0x0000000000003e10 0x0000000000003e10 0x0001d0 0x0001d0 RW  0x8
   NOTE           0x0002a8 0x00000000000002a8 0x00000000000002a8 0x000020 0x000020 R   0x8
   NOTE           0x0002c8 0x00000000000002c8 0x00000000000002c8 0x000024 0x000024 R   0x4
   GNU_PROPERTY   0x0002a8 0x00000000000002a8 0x00000000000002a8 0x000020 0x000020 R   0x8
-  GNU_EH_FRAME   0x002068 0x0000000000002068 0x0000000000002068 0x00008c 0x00008c R   0x4
+  GNU_EH_FRAME   0x002068 0x0000000000002068 0x0000000000002068 0x000094 0x000094 R   0x4
   GNU_STACK      0x000000 0x0000000000000000 0x0000000000000000 0x000000 0x000000 RW  0x10
   GNU_RELRO      0x002e00 0x0000000000003e00 0x0000000000003e00 0x000200 0x000200 R   0x1
 
  Section to Segment mapping:
   Segment Sections...
    00     .note.gnu.property .note.gnu.build-id .gnu.hash .dynsym .dynstr .gnu.version .gnu.version_r .rela.dyn .rela.plt 
    01     .init .plt .plt.got .plt.sec .text .fini
```

#### readelf --wide --sections {}

```diff
@@ -1,39 +1,39 @@
-There are 30 section headers, starting at offset 0x3b58:
+There are 30 section headers, starting at offset 0x3b88:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .note.gnu.property NOTE            00000000000002a8 0002a8 000020 00   A  0   0  8
   [ 2] .note.gnu.build-id NOTE            00000000000002c8 0002c8 000024 00   A  0   0  4
-  [ 3] .gnu.hash         GNU_HASH        00000000000002f0 0002f0 000060 00   A  4   0  8
-  [ 4] .dynsym           DYNSYM          0000000000000350 000350 000330 18   A  5   1  8
-  [ 5] .dynstr           STRTAB          0000000000000680 000680 00026a 00   A  0   0  1
-  [ 6] .gnu.version      VERSYM          00000000000008ea 0008ea 000044 02   A  4   0  2
-  [ 7] .gnu.version_r    VERNEED         0000000000000930 000930 000040 00   A  5   1  8
-  [ 8] .rela.dyn         RELA            0000000000000970 000970 0000a8 18   A  4   0  8
-  [ 9] .rela.plt         RELA            0000000000000a18 000a18 000288 18  AI  4  23  8
+  [ 3] .gnu.hash         GNU_HASH        00000000000002f0 0002f0 000064 00   A  4   0  8
+  [ 4] .dynsym           DYNSYM          0000000000000358 000358 000348 18   A  5   1  8
+  [ 5] .dynstr           STRTAB          00000000000006a0 0006a0 000283 00   A  0   0  1
+  [ 6] .gnu.version      VERSYM          0000000000000924 000924 000046 02   A  4   0  2
+  [ 7] .gnu.version_r    VERNEED         0000000000000970 000970 000040 00   A  5   1  8
+  [ 8] .rela.dyn         RELA            00000000000009b0 0009b0 0000a8 18   A  4   0  8
+  [ 9] .rela.plt         RELA            0000000000000a58 000a58 000288 18  AI  4  23  8
   [10] .init             PROGBITS        0000000000001000 001000 00001b 00  AX  0   0  4
   [11] .plt              PROGBITS        0000000000001020 001020 0001c0 10  AX  0   0 16
   [12] .plt.got          PROGBITS        00000000000011e0 0011e0 000010 10  AX  0   0 16
   [13] .plt.sec          PROGBITS        00000000000011f0 0011f0 0001b0 10  AX  0   0 16
-  [14] .text             PROGBITS        00000000000013a0 0013a0 000a82 00  AX  0   0 16
-  [15] .fini             PROGBITS        0000000000001e24 001e24 00000d 00  AX  0   0  4
+  [14] .text             PROGBITS        00000000000013a0 0013a0 000a9d 00  AX  0   0 16
+  [15] .fini             PROGBITS        0000000000001e40 001e40 00000d 00  AX  0   0  4
   [16] .rodata           PROGBITS        0000000000002000 002000 000068 00   A  0   0  8
-  [17] .eh_frame_hdr     PROGBITS        0000000000002068 002068 00008c 00   A  0   0  4
-  [18] .eh_frame         PROGBITS        00000000000020f8 0020f8 0002fc 00   A  0   0  8
+  [17] .eh_frame_hdr     PROGBITS        0000000000002068 002068 000094 00   A  0   0  4
+  [18] .eh_frame         PROGBITS        0000000000002100 002100 00030c 00   A  0   0  8
   [19] .init_array       INIT_ARRAY      0000000000003e00 002e00 000008 08  WA  0   0  8
   [20] .fini_array       FINI_ARRAY      0000000000003e08 002e08 000008 08  WA  0   0  8
   [21] .dynamic          DYNAMIC         0000000000003e10 002e10 0001d0 10  WA  5   0  8
   [22] .got              PROGBITS        0000000000003fe0 002fe0 000020 08  WA  0   0  8
   [23] .got.plt          PROGBITS        0000000000004000 003000 0000f0 08  WA  0   0  8
   [24] .data             PROGBITS        00000000000040f0 0030f0 000008 00  WA  0   0  8
   [25] .bss              NOBITS          00000000000040f8 0030f8 000008 00  WA  0   0  1
   [26] .comment          PROGBITS        0000000000000000 0030f8 00002b 01  MS  0   0  1
-  [27] .symtab           SYMTAB          0000000000000000 003128 000558 18     28  24  8
-  [28] .strtab           STRTAB          0000000000000000 003680 0003c5 00      0   0  1
-  [29] .shstrtab         STRTAB          0000000000000000 003a45 00010d 00      0   0  1
+  [27] .symtab           SYMTAB          0000000000000000 003128 000570 18     28  24  8
+  [28] .strtab           STRTAB          0000000000000000 003698 0003de 00      0   0  1
+  [29] .shstrtab         STRTAB          0000000000000000 003a76 00010d 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

#### readelf --wide --symbols {}

```diff
@@ -1,9 +1,9 @@
 
-Symbol table '.dynsym' contains 34 entries:
+Symbol table '.dynsym' contains 35 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_eigen_symmv_alloc
      2: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
      3: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@GLIBC_2.2.5 (2)
      4: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __printf_chk@GLIBC_2.3.4 (3)
      5: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_alloc
@@ -19,79 +19,81 @@
     15: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_eigen_symmv_free
     16: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_free
     17: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_view_array
     18: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_vector_free
     19: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail@GLIBC_2.4 (4)
     20: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_column
     21: 00000000000015ef   159 FUNC    GLOBAL DEFAULT   14 create_2d_array
-    22: 00000000000019a7   146 FUNC    GLOBAL DEFAULT   14 create_adj_matrix
-    23: 0000000000001aa4    40 FUNC    GLOBAL DEFAULT   14 final_community_assignment
-    24: 0000000000001459   282 FUNC    GLOBAL DEFAULT   14 getModularityMatrix
-    25: 0000000000001d5f   195 FUNC    GLOBAL DEFAULT   14 get_community
+    22: 000000000000179e    18 FUNC    GLOBAL DEFAULT   14 free_1d_array
+    23: 00000000000019b9   146 FUNC    GLOBAL DEFAULT   14 create_adj_matrix
+    24: 0000000000001ab6    40 FUNC    GLOBAL DEFAULT   14 final_community_assignment
+    25: 0000000000001459   282 FUNC    GLOBAL DEFAULT   14 getModularityMatrix
     26: 000000000000168e    57 FUNC    GLOBAL DEFAULT   14 create_1d_array_int
-    27: 0000000000001acc   659 FUNC    GLOBAL DEFAULT   14 divide_community
+    27: 0000000000001ade   659 FUNC    GLOBAL DEFAULT   14 divide_community
     28: 00000000000015b6    57 FUNC    GLOBAL DEFAULT   14 create_1d_array
-    29: 000000000000179e   521 FUNC    GLOBAL DEFAULT   14 getEigenVector
+    29: 00000000000017b0   521 FUNC    GLOBAL DEFAULT   14 getEigenVector
     30: 0000000000001573    67 FUNC    GLOBAL DEFAULT   14 modularityScore
-    31: 0000000000001a39   107 FUNC    GLOBAL DEFAULT   14 separate_adj_matrix
-    32: 0000000000001766    56 FUNC    GLOBAL DEFAULT   14 free_2d_array
-    33: 00000000000016c7   159 FUNC    GLOBAL DEFAULT   14 create_2d_array_int
+    31: 0000000000001d71   204 FUNC    GLOBAL DEFAULT   14 get_community_assignment
+    32: 0000000000001a4b   107 FUNC    GLOBAL DEFAULT   14 separate_adj_matrix
+    33: 0000000000001766    56 FUNC    GLOBAL DEFAULT   14 free_2d_array
+    34: 00000000000016c7   159 FUNC    GLOBAL DEFAULT   14 create_2d_array_int
 
-Symbol table '.symtab' contains 57 entries:
+Symbol table '.symtab' contains 58 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
      2: 00000000000013a0     0 FUNC    LOCAL  DEFAULT   14 deregister_tm_clones
      3: 00000000000013d0     0 FUNC    LOCAL  DEFAULT   14 register_tm_clones
      4: 0000000000001410     0 FUNC    LOCAL  DEFAULT   14 __do_global_dtors_aux
      5: 00000000000040f8     1 OBJECT  LOCAL  DEFAULT   25 completed.0
      6: 0000000000003e08     0 OBJECT  LOCAL  DEFAULT   20 __do_global_dtors_aux_fini_array_entry
      7: 0000000000001450     0 FUNC    LOCAL  DEFAULT   14 frame_dummy
      8: 0000000000003e00     0 OBJECT  LOCAL  DEFAULT   19 __frame_dummy_init_array_entry
      9: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS modularity.c
     10: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS memory.c
     11: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS eigen.c
     12: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS community_detection.c
-    13: 0000000000001acc   659 FUNC    LOCAL  DEFAULT   14 divide_community.localalias
+    13: 0000000000001ade   659 FUNC    LOCAL  DEFAULT   14 divide_community.localalias
     14: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
-    15: 00000000000023f0     0 OBJECT  LOCAL  DEFAULT   18 __FRAME_END__
+    15: 0000000000002408     0 OBJECT  LOCAL  DEFAULT   18 __FRAME_END__
     16: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
     17: 0000000000002068     0 NOTYPE  LOCAL  DEFAULT   17 __GNU_EH_FRAME_HDR
-    18: 0000000000001e24     0 FUNC    LOCAL  DEFAULT   15 _fini
+    18: 0000000000001e40     0 FUNC    LOCAL  DEFAULT   15 _fini
     19: 0000000000004000     0 OBJECT  LOCAL  DEFAULT   23 _GLOBAL_OFFSET_TABLE_
     20: 00000000000040f8     0 OBJECT  LOCAL  DEFAULT   24 __TMC_END__
     21: 00000000000040f0     0 OBJECT  LOCAL  DEFAULT   24 __dso_handle
     22: 0000000000003e10     0 OBJECT  LOCAL  DEFAULT   21 _DYNAMIC
     23: 0000000000001000     0 FUNC    LOCAL  DEFAULT   10 _init
     24: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_eigen_symmv_alloc
-    25: 0000000000001d5f   195 FUNC    GLOBAL DEFAULT   14 get_community
-    26: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
-    27: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@GLIBC_2.2.5
-    28: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __printf_chk@GLIBC_2.3.4
-    29: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_alloc
-    30: 000000000000179e   521 FUNC    GLOBAL DEFAULT   14 getEigenVector
-    31: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@GLIBC_2.2.5
-    32: 00000000000015ef   159 FUNC    GLOBAL DEFAULT   14 create_2d_array
-    33: 0000000000001573    67 FUNC    GLOBAL DEFAULT   14 modularityScore
-    34: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
-    35: 000000000000168e    57 FUNC    GLOBAL DEFAULT   14 create_1d_array_int
-    36: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_eigen_symmv_sort
-    37: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_eigen_symmv
+    25: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
+    26: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@GLIBC_2.2.5
+    27: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __printf_chk@GLIBC_2.3.4
+    28: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_alloc
+    29: 00000000000017b0   521 FUNC    GLOBAL DEFAULT   14 getEigenVector
+    30: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@GLIBC_2.2.5
+    31: 00000000000015ef   159 FUNC    GLOBAL DEFAULT   14 create_2d_array
+    32: 0000000000001573    67 FUNC    GLOBAL DEFAULT   14 modularityScore
+    33: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
+    34: 000000000000168e    57 FUNC    GLOBAL DEFAULT   14 create_1d_array_int
+    35: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_eigen_symmv_sort
+    36: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_eigen_symmv
+    37: 0000000000001d71   204 FUNC    GLOBAL DEFAULT   14 get_community_assignment
     38: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@GLIBC_2.2.5
     39: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
     40: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_vector_alloc
     41: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5
     42: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_vector_get
-    43: 0000000000001a39   107 FUNC    GLOBAL DEFAULT   14 separate_adj_matrix
+    43: 0000000000001a4b   107 FUNC    GLOBAL DEFAULT   14 separate_adj_matrix
     44: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_eigen_symmv_free
     45: 0000000000001766    56 FUNC    GLOBAL DEFAULT   14 free_2d_array
-    46: 00000000000016c7   159 FUNC    GLOBAL DEFAULT   14 create_2d_array_int
-    47: 00000000000019a7   146 FUNC    GLOBAL DEFAULT   14 create_adj_matrix
-    48: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_free
-    49: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_view_array
-    50: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_vector_free
-    51: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail@GLIBC_2.4
-    52: 0000000000001aa4    40 FUNC    GLOBAL DEFAULT   14 final_community_assignment
-    53: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_column
-    54: 0000000000001acc   659 FUNC    GLOBAL DEFAULT   14 divide_community
-    55: 0000000000001459   282 FUNC    GLOBAL DEFAULT   14 getModularityMatrix
-    56: 00000000000015b6    57 FUNC    GLOBAL DEFAULT   14 create_1d_array
+    46: 000000000000179e    18 FUNC    GLOBAL DEFAULT   14 free_1d_array
+    47: 00000000000016c7   159 FUNC    GLOBAL DEFAULT   14 create_2d_array_int
+    48: 00000000000019b9   146 FUNC    GLOBAL DEFAULT   14 create_adj_matrix
+    49: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_free
+    50: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_view_array
+    51: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_vector_free
+    52: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail@GLIBC_2.4
+    53: 0000000000001ab6    40 FUNC    GLOBAL DEFAULT   14 final_community_assignment
+    54: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_column
+    55: 0000000000001ade   659 FUNC    GLOBAL DEFAULT   14 divide_community
+    56: 0000000000001459   282 FUNC    GLOBAL DEFAULT   14 getModularityMatrix
+    57: 00000000000015b6    57 FUNC    GLOBAL DEFAULT   14 create_1d_array
```

#### readelf --wide --relocs {}

```diff
@@ -1,40 +1,40 @@
 
-Relocation section '.rela.dyn' at offset 0x970 contains 7 entries:
+Relocation section '.rela.dyn' at offset 0x9b0 contains 7 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000003e00  0000000000000008 R_X86_64_RELATIVE                         1450
 0000000000003e08  0000000000000008 R_X86_64_RELATIVE                         1410
 00000000000040f0  0000000000000008 R_X86_64_RELATIVE                         40f0
 0000000000003fe0  0000000200000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
 0000000000003fe8  0000000700000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
 0000000000003ff0  0000000b00000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
 0000000000003ff8  0000000d00000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
 
-Relocation section '.rela.plt' at offset 0xa18 contains 27 entries:
+Relocation section '.rela.plt' at offset 0xa58 contains 27 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000004018  0000000100000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_eigen_symmv_alloc + 0
 0000000000004020  0000000300000007 R_X86_64_JUMP_SLOT     0000000000000000 exit@GLIBC_2.2.5 + 0
 0000000000004028  0000000400000007 R_X86_64_JUMP_SLOT     0000000000000000 __printf_chk@GLIBC_2.3.4 + 0
 0000000000004030  0000000500000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_matrix_alloc + 0
-0000000000004038  0000001d00000007 R_X86_64_JUMP_SLOT     000000000000179e getEigenVector + 0
+0000000000004038  0000001d00000007 R_X86_64_JUMP_SLOT     00000000000017b0 getEigenVector + 0
 0000000000004040  0000000600000007 R_X86_64_JUMP_SLOT     0000000000000000 malloc@GLIBC_2.2.5 + 0
 0000000000004048  0000001500000007 R_X86_64_JUMP_SLOT     00000000000015ef create_2d_array + 0
 0000000000004050  0000001e00000007 R_X86_64_JUMP_SLOT     0000000000001573 modularityScore + 0
 0000000000004058  0000001a00000007 R_X86_64_JUMP_SLOT     000000000000168e create_1d_array_int + 0
 0000000000004060  0000000800000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_eigen_symmv_sort + 0
 0000000000004068  0000000900000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_eigen_symmv + 0
 0000000000004070  0000000a00000007 R_X86_64_JUMP_SLOT     0000000000000000 free@GLIBC_2.2.5 + 0
 0000000000004078  0000000c00000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_vector_alloc + 0
 0000000000004080  0000000e00000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_vector_get + 0
-0000000000004088  0000001f00000007 R_X86_64_JUMP_SLOT     0000000000001a39 separate_adj_matrix + 0
+0000000000004088  0000002000000007 R_X86_64_JUMP_SLOT     0000000000001a4b separate_adj_matrix + 0
 0000000000004090  0000000f00000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_eigen_symmv_free + 0
-0000000000004098  0000002000000007 R_X86_64_JUMP_SLOT     0000000000001766 free_2d_array + 0
-00000000000040a0  0000001600000007 R_X86_64_JUMP_SLOT     00000000000019a7 create_adj_matrix + 0
+0000000000004098  0000002100000007 R_X86_64_JUMP_SLOT     0000000000001766 free_2d_array + 0
+00000000000040a0  0000001700000007 R_X86_64_JUMP_SLOT     00000000000019b9 create_adj_matrix + 0
 00000000000040a8  0000001000000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_matrix_free + 0
 00000000000040b0  0000001100000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_matrix_view_array + 0
 00000000000040b8  0000001200000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_vector_free + 0
 00000000000040c0  0000001300000007 R_X86_64_JUMP_SLOT     0000000000000000 __stack_chk_fail@GLIBC_2.4 + 0
-00000000000040c8  0000001700000007 R_X86_64_JUMP_SLOT     0000000000001aa4 final_community_assignment + 0
+00000000000040c8  0000001800000007 R_X86_64_JUMP_SLOT     0000000000001ab6 final_community_assignment + 0
 00000000000040d0  0000001400000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_matrix_column + 0
-00000000000040d8  0000001b00000007 R_X86_64_JUMP_SLOT     0000000000001acc divide_community + 0
-00000000000040e0  0000001800000007 R_X86_64_JUMP_SLOT     0000000000001459 getModularityMatrix + 0
+00000000000040d8  0000001b00000007 R_X86_64_JUMP_SLOT     0000000000001ade divide_community + 0
+00000000000040e0  0000001900000007 R_X86_64_JUMP_SLOT     0000000000001459 getModularityMatrix + 0
 00000000000040e8  0000001c00000007 R_X86_64_JUMP_SLOT     00000000000015b6 create_1d_array + 0
```

#### readelf --wide --dynamic {}

```diff
@@ -1,28 +1,28 @@
 
 Dynamic section at offset 0x2e10 contains 25 entries:
   Tag        Type                         Name/Value
  0x0000000000000001 (NEEDED)             Shared library: [libgsl.so.27]
  0x0000000000000001 (NEEDED)             Shared library: [libc.so.6]
  0x000000000000000c (INIT)               0x1000
- 0x000000000000000d (FINI)               0x1e24
+ 0x000000000000000d (FINI)               0x1e40
  0x0000000000000019 (INIT_ARRAY)         0x3e00
  0x000000000000001b (INIT_ARRAYSZ)       8 (bytes)
  0x000000000000001a (FINI_ARRAY)         0x3e08
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x2f0
- 0x0000000000000005 (STRTAB)             0x680
- 0x0000000000000006 (SYMTAB)             0x350
- 0x000000000000000a (STRSZ)              618 (bytes)
+ 0x0000000000000005 (STRTAB)             0x6a0
+ 0x0000000000000006 (SYMTAB)             0x358
+ 0x000000000000000a (STRSZ)              643 (bytes)
  0x000000000000000b (SYMENT)             24 (bytes)
  0x0000000000000003 (PLTGOT)             0x4000
  0x0000000000000002 (PLTRELSZ)           648 (bytes)
  0x0000000000000014 (PLTREL)             RELA
- 0x0000000000000017 (JMPREL)             0xa18
- 0x0000000000000007 (RELA)               0x970
+ 0x0000000000000017 (JMPREL)             0xa58
+ 0x0000000000000007 (RELA)               0x9b0
  0x0000000000000008 (RELASZ)             168 (bytes)
  0x0000000000000009 (RELAENT)            24 (bytes)
- 0x000000006ffffffe (VERNEED)            0x930
+ 0x000000006ffffffe (VERNEED)            0x970
  0x000000006fffffff (VERNEEDNUM)         1
- 0x000000006ffffff0 (VERSYM)             0x8ea
+ 0x000000006ffffff0 (VERSYM)             0x924
  0x000000006ffffff9 (RELACOUNT)          3
  0x0000000000000000 (NULL)               0x0
```

#### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 35efb6cd1413500676f713c5d7cf3a7cf99a2f6c
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: ef20d6395907f869f04d1c7ca5de280d7c0830df
```

#### readelf --wide --version-info {}

```diff
@@ -1,19 +1,19 @@
 
-Version symbols section '.gnu.version' contains 34 entries:
- Addr: 0x00000000000008ea  Offset: 0x000008ea  Link: 4 (.dynsym)
+Version symbols section '.gnu.version' contains 35 entries:
+ Addr: 0x0000000000000924  Offset: 0x00000924  Link: 4 (.dynsym)
   000:   0 (*local*)       1 (*global*)      1 (*global*)      2 (GLIBC_2.2.5)
   004:   3 (GLIBC_2.3.4)   1 (*global*)      2 (GLIBC_2.2.5)   1 (*global*)   
   008:   1 (*global*)      1 (*global*)      2 (GLIBC_2.2.5)   1 (*global*)   
   00c:   1 (*global*)      2 (GLIBC_2.2.5)   1 (*global*)      1 (*global*)   
   010:   1 (*global*)      1 (*global*)      1 (*global*)      4 (GLIBC_2.4)  
   014:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   018:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   01c:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
-  020:   1 (*global*)      1 (*global*)   
+  020:   1 (*global*)      1 (*global*)      1 (*global*)   
 
 Version needs section '.gnu.version_r' contains 1 entry:
- Addr: 0x0000000000000930  Offset: 0x00000930  Link: 5 (.dynstr)
+ Addr: 0x0000000000000970  Offset: 0x00000970  Link: 5 (.dynstr)
   000000: Version: 1  File: libc.so.6  Cnt: 3
   0x0010:   Name: GLIBC_2.4  Flags: none  Version: 4
   0x0020:   Name: GLIBC_2.3.4  Flags: none  Version: 3
   0x0030:   Name: GLIBC_2.2.5  Flags: none  Version: 2
```

#### readelf --wide --debug-dump=frames {}

```diff
@@ -154,15 +154,15 @@
   DW_CFA_def_cfa_offset: 16
   DW_CFA_advance_loc: 2 to 000000000000172a
   DW_CFA_def_cfa_offset: 8
   DW_CFA_advance_loc: 1 to 000000000000172b
   DW_CFA_restore_state
   DW_CFA_nop
 
-00000170 000000000000002c 00000174 FDE cie=00000000 pc=0000000000001766..000000000000179e
+00000170 0000000000000028 00000174 FDE cie=00000000 pc=0000000000001766..000000000000179e
   DW_CFA_advance_loc: 6 to 000000000000176c
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r12 (r12) at cfa-16
   DW_CFA_advance_loc: 1 to 000000000000176d
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r6 (rbp) at cfa-24
   DW_CFA_advance_loc: 1 to 000000000000176e
@@ -173,182 +173,184 @@
   DW_CFA_advance_loc: 1 to 000000000000179b
   DW_CFA_def_cfa_offset: 16
   DW_CFA_advance_loc: 2 to 000000000000179d
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
+
+0000019c 0000000000000018 000001a0 FDE cie=00000000 pc=000000000000179e..00000000000017b0
+  DW_CFA_advance_loc: 8 to 00000000000017a6
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 9 to 00000000000017af
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000001a0 000000000000004c 000001a4 FDE cie=00000000 pc=000000000000179e..00000000000019a7
-  DW_CFA_advance_loc: 6 to 00000000000017a4
+000001b8 000000000000004c 000001bc FDE cie=00000000 pc=00000000000017b0..00000000000019b9
+  DW_CFA_advance_loc: 6 to 00000000000017b6
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 00000000000017a6
+  DW_CFA_advance_loc: 2 to 00000000000017b8
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 00000000000017a8
+  DW_CFA_advance_loc: 2 to 00000000000017ba
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 00000000000017aa
+  DW_CFA_advance_loc: 2 to 00000000000017bc
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 00000000000017ab
+  DW_CFA_advance_loc: 1 to 00000000000017bd
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 00000000000017ac
+  DW_CFA_advance_loc: 1 to 00000000000017be
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 00000000000017b3
+  DW_CFA_advance_loc: 7 to 00000000000017c5
   DW_CFA_def_cfa_offset: 192
-  DW_CFA_advance_loc2: 349 to 0000000000001910
+  DW_CFA_advance_loc2: 349 to 0000000000001922
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000001911
+  DW_CFA_advance_loc: 1 to 0000000000001923
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000001912
+  DW_CFA_advance_loc: 1 to 0000000000001924
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000001914
+  DW_CFA_advance_loc: 2 to 0000000000001926
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000001916
+  DW_CFA_advance_loc: 2 to 0000000000001928
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000001918
+  DW_CFA_advance_loc: 2 to 000000000000192a
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000191a
+  DW_CFA_advance_loc: 2 to 000000000000192c
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000000000000191b
+  DW_CFA_advance_loc: 1 to 000000000000192d
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000001f0 0000000000000028 000001f4 FDE cie=00000000 pc=00000000000019a7..0000000000001a39
-  DW_CFA_advance_loc: 6 to 00000000000019ad
+00000208 0000000000000028 0000020c FDE cie=00000000 pc=00000000000019b9..0000000000001a4b
+  DW_CFA_advance_loc: 6 to 00000000000019bf
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r12 (r12) at cfa-16
-  DW_CFA_advance_loc: 1 to 00000000000019ae
+  DW_CFA_advance_loc: 1 to 00000000000019c0
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r6 (rbp) at cfa-24
-  DW_CFA_advance_loc: 1 to 00000000000019af
+  DW_CFA_advance_loc: 1 to 00000000000019c1
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r3 (rbx) at cfa-32
-  DW_CFA_advance_loc1: 134 to 0000000000001a35
+  DW_CFA_advance_loc1: 134 to 0000000000001a47
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 1 to 0000000000001a36
+  DW_CFA_advance_loc: 1 to 0000000000001a48
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000001a38
+  DW_CFA_advance_loc: 2 to 0000000000001a4a
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
 
-0000021c 0000000000000028 00000220 FDE cie=00000000 pc=0000000000001a39..0000000000001aa4
-  DW_CFA_advance_loc: 6 to 0000000000001a3f
+00000234 0000000000000028 00000238 FDE cie=00000000 pc=0000000000001a4b..0000000000001ab6
+  DW_CFA_advance_loc: 6 to 0000000000001a51
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r12 (r12) at cfa-16
-  DW_CFA_advance_loc: 1 to 0000000000001a40
+  DW_CFA_advance_loc: 1 to 0000000000001a52
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r6 (rbp) at cfa-24
-  DW_CFA_advance_loc: 1 to 0000000000001a41
+  DW_CFA_advance_loc: 1 to 0000000000001a53
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r3 (rbx) at cfa-32
-  DW_CFA_advance_loc1: 95 to 0000000000001aa0
+  DW_CFA_advance_loc1: 95 to 0000000000001ab2
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 1 to 0000000000001aa1
+  DW_CFA_advance_loc: 1 to 0000000000001ab3
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000001aa3
+  DW_CFA_advance_loc: 2 to 0000000000001ab5
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000248 0000000000000010 0000024c FDE cie=00000000 pc=0000000000001aa4..0000000000001acc
+00000260 0000000000000010 00000264 FDE cie=00000000 pc=0000000000001ab6..0000000000001ade
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000025c 000000000000004c 00000260 FDE cie=00000000 pc=0000000000001acc..0000000000001d5f
-  DW_CFA_advance_loc: 6 to 0000000000001ad2
+00000274 000000000000004c 00000278 FDE cie=00000000 pc=0000000000001ade..0000000000001d71
+  DW_CFA_advance_loc: 6 to 0000000000001ae4
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000001ad4
+  DW_CFA_advance_loc: 2 to 0000000000001ae6
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 0000000000001ad6
+  DW_CFA_advance_loc: 2 to 0000000000001ae8
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 0000000000001ad8
+  DW_CFA_advance_loc: 2 to 0000000000001aea
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000001ad9
+  DW_CFA_advance_loc: 1 to 0000000000001aeb
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 0000000000001ada
+  DW_CFA_advance_loc: 1 to 0000000000001aec
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 4 to 0000000000001ade
+  DW_CFA_advance_loc: 4 to 0000000000001af0
   DW_CFA_def_cfa_offset: 144
-  DW_CFA_advance_loc2: 509 to 0000000000001cdb
+  DW_CFA_advance_loc2: 509 to 0000000000001ced
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000001cdc
+  DW_CFA_advance_loc: 1 to 0000000000001cee
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000001cdd
+  DW_CFA_advance_loc: 1 to 0000000000001cef
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000001cdf
+  DW_CFA_advance_loc: 2 to 0000000000001cf1
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000001ce1
+  DW_CFA_advance_loc: 2 to 0000000000001cf3
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000001ce3
+  DW_CFA_advance_loc: 2 to 0000000000001cf5
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000001ce5
+  DW_CFA_advance_loc: 2 to 0000000000001cf7
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000001ce6
+  DW_CFA_advance_loc: 1 to 0000000000001cf8
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000002ac 0000000000000048 000002b0 FDE cie=00000000 pc=0000000000001d5f..0000000000001e22
-  DW_CFA_advance_loc: 6 to 0000000000001d65
+000002c4 0000000000000040 000002c8 FDE cie=00000000 pc=0000000000001d71..0000000000001e3d
+  DW_CFA_advance_loc: 6 to 0000000000001d77
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000001d67
+  DW_CFA_offset: r14 (r14) at cfa-16
+  DW_CFA_advance_loc: 2 to 0000000000001d79
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 0000000000001d69
+  DW_CFA_offset: r13 (r13) at cfa-24
+  DW_CFA_advance_loc: 2 to 0000000000001d7b
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 0000000000001d6b
+  DW_CFA_offset: r12 (r12) at cfa-32
+  DW_CFA_advance_loc: 1 to 0000000000001d7c
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000001d6c
+  DW_CFA_offset: r6 (rbp) at cfa-40
+  DW_CFA_advance_loc: 1 to 0000000000001d7d
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 0000000000001d6d
-  DW_CFA_def_cfa_offset: 56
-  DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 4 to 0000000000001d71
-  DW_CFA_def_cfa_offset: 80
-  DW_CFA_advance_loc1: 161 to 0000000000001e12
+  DW_CFA_offset: r3 (rbx) at cfa-48
+  DW_CFA_advance_loc: 4 to 0000000000001d81
+  DW_CFA_def_cfa_offset: 64
+  DW_CFA_advance_loc1: 174 to 0000000000001e2f
   DW_CFA_remember_state
-  DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000001e13
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000001e14
+  DW_CFA_advance_loc: 1 to 0000000000001e30
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000001e16
+  DW_CFA_advance_loc: 1 to 0000000000001e31
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000001e18
+  DW_CFA_advance_loc: 2 to 0000000000001e33
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000001e1a
+  DW_CFA_advance_loc: 2 to 0000000000001e35
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000001e1c
+  DW_CFA_advance_loc: 2 to 0000000000001e37
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000001e1d
+  DW_CFA_advance_loc: 1 to 0000000000001e38
   DW_CFA_restore_state
   DW_CFA_nop
 
-000002f8 ZERO terminator
+00000308 ZERO terminator
```

#### strings --all --bytes=8 {}

```diff
@@ -6,14 +6,15 @@
 create_1d_array
 create_2d_array
 modularityScore
 __printf_chk
 create_1d_array_int
 create_2d_array_int
 free_2d_array
+free_1d_array
 getEigenVector
 gsl_matrix_view_array
 gsl_vector_alloc
 gsl_matrix_alloc
 gsl_eigen_symmv_alloc
 gsl_eigen_symmv
 gsl_eigen_symmv_free
@@ -23,26 +24,26 @@
 gsl_vector_free
 gsl_matrix_free
 __stack_chk_fail
 create_adj_matrix
 separate_adj_matrix
 final_community_assignment
 divide_community
-get_community
+get_community_assignment
 libgsl.so.27
 libc.so.6
 GLIBC_2.4
 GLIBC_2.3.4
 GLIBC_2.2.5
 AWAVAUATUSH
 []A\A]A^A_
 AWAVAUATUSH
 X[]A\A]A^A_
-AWAVAUATUSH
-[]A\A]A^A_
+AVAUATUSH
+[]A\A]A^
 Error: Memory allocation failed.
 Error: Failed to allocate memory for 2D array.
 GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
 completed.0
@@ -56,35 +57,36 @@
 __FRAME_END__
 __GNU_EH_FRAME_HDR
 _GLOBAL_OFFSET_TABLE_
 __TMC_END__
 __dso_handle
 _DYNAMIC
 gsl_eigen_symmv_alloc
-get_community
 __gmon_start__
 exit@GLIBC_2.2.5
 __printf_chk@GLIBC_2.3.4
 gsl_matrix_alloc
 getEigenVector
 malloc@GLIBC_2.2.5
 create_2d_array
 modularityScore
 _ITM_deregisterTMCloneTable
 create_1d_array_int
 gsl_eigen_symmv_sort
 gsl_eigen_symmv
+get_community_assignment
 free@GLIBC_2.2.5
 _ITM_registerTMCloneTable
 gsl_vector_alloc
 __cxa_finalize@GLIBC_2.2.5
 gsl_vector_get
 separate_adj_matrix
 gsl_eigen_symmv_free
 free_2d_array
+free_1d_array
 create_2d_array_int
 create_adj_matrix
 gsl_matrix_free
 gsl_matrix_view_array
 gsl_vector_free
 __stack_chk_fail@GLIBC_2.4
 final_community_assignment
```

#### readelf --wide --decompress --hex-dump=.gnu.hash {}

```diff
@@ -1,9 +1,10 @@
 
 Hex dump of section '.gnu.hash':
   0x000002f0 03000000 15000000 02000000 07000000 ................
-  0x00000300 00404030 84002008 d3180254 000a5000 .@@0.. ....T..P.
-  0x00000310 15000000 19000000 1d000000 4ce3bf58 ............L..X
-  0x00000320 3a2743c6 ca687799 c500c2a5 687a26e4 :'C..hw.....hz&.
+  0x00000300 00404030 84002008 d3180254 82084202 .@@0.. ....T..B.
+  0x00000310 15000000 1a000000 1d000000 4ce3bf58 ............L..X
+  0x00000320 f8b33478 3a2743c6 ca687799 c500c2a5 ..4x:'C..hw.....
   0x00000330 34319b80 5e1bfcde 6b0e7e6c 40c0dcf3 41..^...k.~l@...
-  0x00000340 ea4303c3 9c939ad3 da887664 978e8eb1 .C........vd....
+  0x00000340 ea4303c3 e0788354 9c939ad3 da887664 .C...x.T......vd
+  0x00000350 978e8eb1                            ....
```

#### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -1,42 +1,44 @@
 
 Hex dump of section '.dynstr':
-  0x00000680 005f5f67 6d6f6e5f 73746172 745f5f00 .__gmon_start__.
-  0x00000690 5f49544d 5f646572 65676973 74657254 _ITM_deregisterT
-  0x000006a0 4d436c6f 6e655461 626c6500 5f49544d MCloneTable._ITM
-  0x000006b0 5f726567 69737465 72544d43 6c6f6e65 _registerTMClone
-  0x000006c0 5461626c 65005f5f 6378615f 66696e61 Table.__cxa_fina
-  0x000006d0 6c697a65 00676574 4d6f6475 6c617269 lize.getModulari
-  0x000006e0 74794d61 74726978 00637265 6174655f tyMatrix.create_
-  0x000006f0 31645f61 72726179 00637265 6174655f 1d_array.create_
-  0x00000700 32645f61 72726179 006d6f64 756c6172 2d_array.modular
-  0x00000710 69747953 636f7265 006d616c 6c6f6300 ityScore.malloc.
-  0x00000720 5f5f7072 696e7466 5f63686b 00657869 __printf_chk.exi
-  0x00000730 74006372 65617465 5f31645f 61727261 t.create_1d_arra
-  0x00000740 795f696e 74006372 65617465 5f32645f y_int.create_2d_
-  0x00000750 61727261 795f696e 74006672 65655f32 array_int.free_2
-  0x00000760 645f6172 72617900 67657445 6967656e d_array.getEigen
-  0x00000770 56656374 6f720067 736c5f6d 61747269 Vector.gsl_matri
-  0x00000780 785f7669 65775f61 72726179 0067736c x_view_array.gsl
-  0x00000790 5f766563 746f725f 616c6c6f 63006773 _vector_alloc.gs
-  0x000007a0 6c5f6d61 74726978 5f616c6c 6f630067 l_matrix_alloc.g
-  0x000007b0 736c5f65 6967656e 5f73796d 6d765f61 sl_eigen_symmv_a
-  0x000007c0 6c6c6f63 0067736c 5f656967 656e5f73 lloc.gsl_eigen_s
-  0x000007d0 796d6d76 0067736c 5f656967 656e5f73 ymmv.gsl_eigen_s
-  0x000007e0 796d6d76 5f667265 65006773 6c5f6569 ymmv_free.gsl_ei
-  0x000007f0 67656e5f 73796d6d 765f736f 72740067 gen_symmv_sort.g
-  0x00000800 736c5f6d 61747269 785f636f 6c756d6e sl_matrix_column
-  0x00000810 0067736c 5f766563 746f725f 67657400 .gsl_vector_get.
-  0x00000820 67736c5f 76656374 6f725f66 72656500 gsl_vector_free.
-  0x00000830 67736c5f 6d617472 69785f66 72656500 gsl_matrix_free.
-  0x00000840 5f5f7374 61636b5f 63686b5f 6661696c __stack_chk_fail
-  0x00000850 00637265 6174655f 61646a5f 6d617472 .create_adj_matr
-  0x00000860 69780073 65706172 6174655f 61646a5f ix.separate_adj_
-  0x00000870 6d617472 69780066 696e616c 5f636f6d matrix.final_com
-  0x00000880 6d756e69 74795f61 73736967 6e6d656e munity_assignmen
-  0x00000890 74006469 76696465 5f636f6d 6d756e69 t.divide_communi
-  0x000008a0 74790067 65745f63 6f6d6d75 6e697479 ty.get_community
-  0x000008b0 006c6962 67736c2e 736f2e32 37006c69 .libgsl.so.27.li
-  0x000008c0 62632e73 6f2e3600 474c4942 435f322e bc.so.6.GLIBC_2.
-  0x000008d0 3400474c 4942435f 322e332e 3400474c 4.GLIBC_2.3.4.GL
-  0x000008e0 4942435f 322e322e 3500              IBC_2.2.5.
+  0x000006a0 005f5f67 6d6f6e5f 73746172 745f5f00 .__gmon_start__.
+  0x000006b0 5f49544d 5f646572 65676973 74657254 _ITM_deregisterT
+  0x000006c0 4d436c6f 6e655461 626c6500 5f49544d MCloneTable._ITM
+  0x000006d0 5f726567 69737465 72544d43 6c6f6e65 _registerTMClone
+  0x000006e0 5461626c 65005f5f 6378615f 66696e61 Table.__cxa_fina
+  0x000006f0 6c697a65 00676574 4d6f6475 6c617269 lize.getModulari
+  0x00000700 74794d61 74726978 00637265 6174655f tyMatrix.create_
+  0x00000710 31645f61 72726179 00637265 6174655f 1d_array.create_
+  0x00000720 32645f61 72726179 006d6f64 756c6172 2d_array.modular
+  0x00000730 69747953 636f7265 006d616c 6c6f6300 ityScore.malloc.
+  0x00000740 5f5f7072 696e7466 5f63686b 00657869 __printf_chk.exi
+  0x00000750 74006372 65617465 5f31645f 61727261 t.create_1d_arra
+  0x00000760 795f696e 74006372 65617465 5f32645f y_int.create_2d_
+  0x00000770 61727261 795f696e 74006672 65655f32 array_int.free_2
+  0x00000780 645f6172 72617900 66726565 5f31645f d_array.free_1d_
+  0x00000790 61727261 79006765 74456967 656e5665 array.getEigenVe
+  0x000007a0 63746f72 0067736c 5f6d6174 7269785f ctor.gsl_matrix_
+  0x000007b0 76696577 5f617272 61790067 736c5f76 view_array.gsl_v
+  0x000007c0 6563746f 725f616c 6c6f6300 67736c5f ector_alloc.gsl_
+  0x000007d0 6d617472 69785f61 6c6c6f63 0067736c matrix_alloc.gsl
+  0x000007e0 5f656967 656e5f73 796d6d76 5f616c6c _eigen_symmv_all
+  0x000007f0 6f630067 736c5f65 6967656e 5f73796d oc.gsl_eigen_sym
+  0x00000800 6d760067 736c5f65 6967656e 5f73796d mv.gsl_eigen_sym
+  0x00000810 6d765f66 72656500 67736c5f 65696765 mv_free.gsl_eige
+  0x00000820 6e5f7379 6d6d765f 736f7274 0067736c n_symmv_sort.gsl
+  0x00000830 5f6d6174 7269785f 636f6c75 6d6e0067 _matrix_column.g
+  0x00000840 736c5f76 6563746f 725f6765 74006773 sl_vector_get.gs
+  0x00000850 6c5f7665 63746f72 5f667265 65006773 l_vector_free.gs
+  0x00000860 6c5f6d61 74726978 5f667265 65005f5f l_matrix_free.__
+  0x00000870 73746163 6b5f6368 6b5f6661 696c0063 stack_chk_fail.c
+  0x00000880 72656174 655f6164 6a5f6d61 74726978 reate_adj_matrix
+  0x00000890 00736570 61726174 655f6164 6a5f6d61 .separate_adj_ma
+  0x000008a0 74726978 0066696e 616c5f63 6f6d6d75 trix.final_commu
+  0x000008b0 6e697479 5f617373 69676e6d 656e7400 nity_assignment.
+  0x000008c0 64697669 64655f63 6f6d6d75 6e697479 divide_community
+  0x000008d0 00676574 5f636f6d 6d756e69 74795f61 .get_community_a
+  0x000008e0 73736967 6e6d656e 74006c69 6267736c ssignment.libgsl
+  0x000008f0 2e736f2e 3237006c 6962632e 736f2e36 .so.27.libc.so.6
+  0x00000900 00474c49 42435f32 2e340047 4c494243 .GLIBC_2.4.GLIBC
+  0x00000910 5f322e33 2e340047 4c494243 5f322e32 _2.3.4.GLIBC_2.2
+  0x00000920 2e3500                              .5.
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -322,15 +322,23 @@
 	mov    %r12,%rdi
 	call   12a0 <free@plt>
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	ret
 
-000000000000179e <getEigenVector>:
+000000000000179e <free_1d_array>:
+free_1d_array():
+	endbr64
+	sub    $0x8,%rsp
+	call   12a0 <free@plt>
+	add    $0x8,%rsp
+	ret
+
+00000000000017b0 <getEigenVector>:
 getEigenVector():
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
@@ -342,34 +350,34 @@
 	mov    %rax,0x78(%rsp)
 	xor    %eax,%eax
 	mov    %esi,%edi
 	imul   %esi,%edi
 	call   1390 <create_1d_array@plt>
 	mov    %rax,%r15
 	test   %ebp,%ebp
-	jle    191b <getEigenVector+0x17d>
+	jle    192d <getEigenVector+0x17d>
 	mov    %rbx,%rcx
 	movslq %ebp,%r12
 	lea    0x0(,%r12,8),%r9
 	mov    %rax,%rsi
 	lea    -0x1(%rbp),%eax
 	lea    0x8(%rbx,%rax,8),%r8
 	mov    %ebp,%ebx
 	lea    0x0(,%rbx,8),%rdi
 	mov    $0x0,%eax
 	mov    (%rcx),%rdx
 	movsd  (%rdx,%rax,1),%xmm0
 	movsd  %xmm0,(%rsi,%rax,1)
 	add    $0x8,%rax
 	cmp    %rax,%rdi
-	jne    1805 <getEigenVector+0x67>
+	jne    1817 <getEigenVector+0x67>
 	add    $0x8,%rcx
 	add    %r9,%rsi
 	cmp    %r8,%rcx
-	jne    1800 <getEigenVector+0x62>
+	jne    1812 <getEigenVector+0x62>
 	lea    0x40(%rsp),%rax
 	mov    %r12,%rcx
 	mov    %r12,%rdx
 	mov    %r15,%rsi
 	mov    %rax,0x8(%rsp)
 	mov    %rax,%rdi
 	call   1320 <gsl_matrix_view_array@plt>
@@ -408,24 +416,24 @@
 	pxor   %xmm1,%xmm1
 	comisd %xmm1,%xmm0
 	setae  %al
 	movzbl %al,%eax
 	mov    %eax,(%r12,%rbp,4)
 	add    $0x1,%rbp
 	cmp    %rbp,%rbx
-	jne    18b2 <getEigenVector+0x114>
+	jne    18c4 <getEigenVector+0x114>
 	mov    %r14,%rdi
 	call   1330 <gsl_vector_free@plt>
 	mov    %r13,%rdi
 	call   1310 <gsl_matrix_free@plt>
 	mov    %r15,%rdi
 	call   12a0 <free@plt>
 	mov    0x78(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    19a2 <getEigenVector+0x204>
+	jne    19b4 <getEigenVector+0x204>
 	mov    %r12,%rax
 	add    $0x88,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
@@ -462,122 +470,122 @@
 	lea    0x10(%rsp),%rdi
 	mov    $0x1,%edx
 	mov    %r13,%rsi
 	call   1360 <gsl_matrix_column@plt>
 	mov    %ebp,%edi
 	call   1270 <create_1d_array_int@plt>
 	mov    %rax,%r12
-	jmp    18da <getEigenVector+0x13c>
+	jmp    18ec <getEigenVector+0x13c>
 	call   1340 <__stack_chk_fail@plt>
 
-00000000000019a7 <create_adj_matrix>:
+00000000000019b9 <create_adj_matrix>:
 create_adj_matrix():
 	endbr64
 	push   %r12
 	push   %rbp
 	push   %rbx
 	mov    %rdi,%rbp
 	mov    %esi,%ebx
 	mov    %edx,%r12d
 	mov    %edx,%esi
 	mov    %edx,%edi
 	call   1250 <create_2d_array@plt>
 	mov    %rax,%rdi
 	test   %r12d,%r12d
-	jle    19f8 <create_adj_matrix+0x51>
+	jle    1a0a <create_adj_matrix+0x51>
 	mov    %rax,%rcx
 	mov    %r12d,%esi
 	shl    $0x3,%rsi
 	lea    (%rsi,%rax,1),%r8
 	mov    $0x0,%eax
 	mov    (%rcx),%rdx
 	movq   $0x0,(%rdx,%rax,1)
 	add    $0x8,%rax
 	cmp    %rsi,%rax
-	jne    19db <create_adj_matrix+0x34>
+	jne    19ed <create_adj_matrix+0x34>
 	add    $0x8,%rcx
 	cmp    %r8,%rcx
-	jne    19d6 <create_adj_matrix+0x2f>
+	jne    19e8 <create_adj_matrix+0x2f>
 	test   %ebx,%ebx
-	jle    1a31 <create_adj_matrix+0x8a>
+	jle    1a43 <create_adj_matrix+0x8a>
 	mov    %rbp,%rax
 	lea    -0x1(%rbx),%edx
 	lea    0x8(%rbp,%rdx,8),%r8
-	movsd  0x651(%rip),%xmm0        
+	movsd  0x63f(%rip),%xmm0        
 	movslq (%rax),%rdx
 	movslq 0x4(%rax),%rcx
 	mov    (%rdi,%rdx,8),%rsi
 	movsd  %xmm0,(%rsi,%rcx,8)
 	mov    (%rdi,%rcx,8),%rcx
 	movsd  %xmm0,(%rcx,%rdx,8)
 	add    $0x8,%rax
 	cmp    %rax,%r8
-	jne    1a0f <create_adj_matrix+0x68>
+	jne    1a21 <create_adj_matrix+0x68>
 	mov    %rdi,%rax
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	ret
 
-0000000000001a39 <separate_adj_matrix>:
+0000000000001a4b <separate_adj_matrix>:
 separate_adj_matrix():
 	endbr64
 	push   %r12
 	push   %rbp
 	push   %rbx
 	mov    %rdi,%rbp
 	mov    %rsi,%rbx
 	mov    %edx,%r12d
 	mov    %edx,%esi
 	mov    %edx,%edi
 	call   1250 <create_2d_array@plt>
 	test   %r12d,%r12d
-	jle    1a9f <separate_adj_matrix+0x66>
+	jle    1ab1 <separate_adj_matrix+0x66>
 	mov    %rbx,%rdi
 	mov    %rax,%r8
 	lea    -0x1(%r12),%edx
 	lea    0x4(%rbx,%rdx,4),%r10
 	mov    %r12d,%r9d
 	mov    $0x0,%edx
 	movslq (%rdi),%rcx
 	movslq (%rbx,%rdx,4),%rsi
 	mov    0x0(%rbp,%rcx,8),%rcx
 	movsd  (%rcx,%rsi,8),%xmm0
 	mov    (%r8),%rcx
 	movsd  %xmm0,(%rcx,%rdx,8)
 	add    $0x1,%rdx
 	cmp    %rdx,%r9
-	jne    1a70 <separate_adj_matrix+0x37>
+	jne    1a82 <separate_adj_matrix+0x37>
 	add    $0x4,%rdi
 	add    $0x8,%r8
 	cmp    %r10,%rdi
-	jne    1a6b <separate_adj_matrix+0x32>
+	jne    1a7d <separate_adj_matrix+0x32>
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	ret
 
-0000000000001aa4 <final_community_assignment>:
+0000000000001ab6 <final_community_assignment>:
 final_community_assignment():
 	endbr64
 	test   %esi,%esi
-	jle    1ac8 <final_community_assignment+0x24>
+	jle    1ada <final_community_assignment+0x24>
 	mov    %rdi,%rax
 	lea    -0x1(%rsi),%esi
 	lea    0x4(%rdi,%rsi,4),%r8
 	mov    (%rcx),%edi
 	movslq (%rax),%rsi
 	mov    %edi,(%rdx,%rsi,4)
 	add    $0x4,%rax
 	cmp    %r8,%rax
-	jne    1ab7 <final_community_assignment+0x13>
+	jne    1ac9 <final_community_assignment+0x13>
 	addl   $0x1,(%rcx)
 	ret
 
-0000000000001acc <divide_community>:
+0000000000001ade <divide_community>:
 divide_community.localalias():
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
@@ -587,44 +595,44 @@
 	mov    %esi,0xc(%rsp)
 	mov    %rdx,%rbx
 	mov    %rcx,0x38(%rsp)
 	mov    %r8,0x30(%rsp)
 	mov    %r9,0x10(%rsp)
 	movsd  %xmm0,0x40(%rsp)
 	cmp    $0x2,%esi
-	jle    1b2c <divide_community+0x60>
+	jle    1b3e <divide_community+0x60>
 	mov    0xc(%rsp),%r14d
 	mov    %r14d,%esi
 	mov    (%rsp),%rdi
 	call   1230 <getEigenVector@plt>
 	mov    %rax,%rbp
 	mov    %r14d,%edx
 	lea    (%rax,%rdx,4),%rdx
 	mov    $0x0,%r12d
 	mov    $0x0,%r13d
-	jmp    1b63 <divide_community+0x97>
+	jmp    1b75 <divide_community+0x97>
 	mov    %r8,%rcx
 	mov    %r9,%rdx
 	mov    %esi,%r15d
 	mov    %rbx,%rdi
 	call   1350 <final_community_assignment@plt>
 	mov    %r15d,%esi
 	mov    (%rsp),%rdi
 	call   12f0 <free_2d_array@plt>
 	mov    %rbx,%rdi
 	call   12a0 <free@plt>
-	jmp    1cd7 <divide_community+0x20b>
+	jmp    1ce9 <divide_community+0x20b>
 	add    $0x1,%r12d
 	add    $0x4,%rax
 	cmp    %rdx,%rax
-	je     1b6e <divide_community+0xa2>
+	je     1b80 <divide_community+0xa2>
 	cmpl   $0x0,(%rax)
-	jne    1b56 <divide_community+0x8a>
+	jne    1b68 <divide_community+0x8a>
 	add    $0x1,%r13d
-	jmp    1b5a <divide_community+0x8e>
+	jmp    1b6c <divide_community+0x8e>
 	mov    %r13d,%edi
 	call   1270 <create_1d_array_int@plt>
 	mov    %rax,0x20(%rsp)
 	mov    %r13d,%edi
 	call   1270 <create_1d_array_int@plt>
 	mov    %rax,%r15
 	mov    %r12d,%edi
@@ -635,45 +643,45 @@
 	mov    %rax,%r14
 	mov    0xc(%rsp),%edi
 	mov    $0x0,%eax
 	mov    $0x0,%ecx
 	mov    $0x0,%edx
 	mov    0x20(%rsp),%r9
 	mov    0x28(%rsp),%r10
-	jmp    1bd8 <divide_community+0x10c>
+	jmp    1bea <divide_community+0x10c>
 	movslq %ecx,%rsi
 	mov    (%rbx,%rax,4),%r8d
 	mov    %r8d,(%r10,%rsi,4)
 	mov    %eax,(%r14,%rsi,4)
 	add    $0x1,%ecx
 	add    $0x1,%rax
 	cmp    %rdi,%rax
-	je     1bf3 <divide_community+0x127>
+	je     1c05 <divide_community+0x127>
 	cmpl   $0x0,0x0(%rbp,%rax,4)
-	jne    1bbd <divide_community+0xf1>
+	jne    1bcf <divide_community+0xf1>
 	movslq %edx,%rsi
 	mov    (%rbx,%rax,4),%r8d
 	mov    %r8d,(%r9,%rsi,4)
 	mov    %eax,(%r15,%rsi,4)
 	add    $0x1,%edx
-	jmp    1bcf <divide_community+0x103>
+	jmp    1be1 <divide_community+0x103>
 	mov    %rbp,%rdi
 	call   12a0 <free@plt>
 	pxor   %xmm1,%xmm1
 	movsd  %xmm1,0x18(%rsp)
 	cmp    $0x1,%r13d
-	jg     1ce6 <divide_community+0x21a>
-	mov    0x442(%rip),%rbp        
+	jg     1cf8 <divide_community+0x21a>
+	mov    0x430(%rip),%rbp        
 	cmp    $0x1,%r12d
-	jg     1d03 <divide_community+0x237>
+	jg     1d15 <divide_community+0x237>
 	movq   %rbp,%xmm0
 	addsd  0x18(%rsp),%xmm0
 	movsd  0x40(%rsp),%xmm3
 	comisd %xmm0,%xmm3
-	jae    1d1f <divide_community+0x253>
+	jae    1d31 <divide_community+0x253>
 	mov    %r13d,%edx
 	mov    %r15,%rsi
 	mov    (%rsp),%rdi
 	call   12d0 <separate_adj_matrix@plt>
 	mov    %rax,0x40(%rsp)
 	mov    %r12d,%edx
 	mov    %r14,%rsi
@@ -689,23 +697,23 @@
 	mov    0x30(%rsp),%r14
 	mov    %r14,%r8
 	mov    0x38(%rsp),%r15
 	mov    %r15,%rcx
 	mov    0x20(%rsp),%rdx
 	mov    %r13d,%esi
 	mov    0x40(%rsp),%rdi
-	call   1acc <divide_community>
+	call   1ade <divide_community>
 	movq   %rbp,%xmm0
 	mov    0x10(%rsp),%r9
 	mov    %r14,%r8
 	mov    %r15,%rcx
 	mov    0x28(%rsp),%rdx
 	mov    %r12d,%esi
 	mov    0x48(%rsp),%rdi
-	call   1acc <divide_community>
+	call   1ade <divide_community>
 	mov    0xc(%rsp),%esi
 	mov    (%rsp),%rdi
 	call   12f0 <free_2d_array@plt>
 	mov    %rbx,%rdi
 	call   12a0 <free@plt>
 	add    $0x58,%rsp
 	pop    %rbx
@@ -716,21 +724,21 @@
 	pop    %r15
 	ret
 	mov    0x20(%rsp),%rdx
 	mov    %r13d,%esi
 	mov    0x38(%rsp),%rdi
 	call   1260 <modularityScore@plt>
 	movsd  %xmm0,0x18(%rsp)
-	jmp    1c0f <divide_community+0x143>
+	jmp    1c21 <divide_community+0x143>
 	mov    0x28(%rsp),%rdx
 	mov    %r12d,%esi
 	mov    0x38(%rsp),%rdi
 	call   1260 <modularityScore@plt>
 	movq   %xmm0,%rbp
-	jmp    1c20 <divide_community+0x154>
+	jmp    1c32 <divide_community+0x154>
 	mov    0x30(%rsp),%rcx
 	mov    0x10(%rsp),%rdx
 	mov    0xc(%rsp),%ebp
 	mov    %ebp,%esi
 	mov    %rbx,%rdi
 	call   1350 <final_community_assignment@plt>
 	mov    %ebp,%esi
@@ -738,71 +746,74 @@
 	call   12f0 <free_2d_array@plt>
 	mov    %r15,%rdi
 	call   12a0 <free@plt>
 	mov    %r14,%rdi
 	call   12a0 <free@plt>
 	mov    %rbx,%rdi
 	call   12a0 <free@plt>
-	jmp    1cd7 <divide_community+0x20b>
+	jmp    1ce9 <divide_community+0x20b>
 
-0000000000001d5f <get_community>:
-get_community():
+0000000000001d71 <get_community_assignment>:
+get_community_assignment():
 	endbr64
-	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
-	sub    $0x18,%rsp
-	mov    %rdi,%r13
+	sub    $0x10,%rsp
+	mov    %rdi,%rbx
+	mov    %esi,%r12d
 	mov    %edx,%ebp
-	mov    %rcx,%r15
 	mov    %fs:0x28,%rax
 	mov    %rax,0x8(%rsp)
 	xor    %eax,%eax
+	mov    %edx,%edi
+	call   1270 <create_1d_array_int@plt>
+	mov    %rax,%r13
+	mov    %ebp,%edx
+	mov    %r12d,%esi
+	mov    %rbx,%rdi
 	call   1300 <create_adj_matrix@plt>
 	mov    %rax,%r14
 	mov    %ebp,%esi
 	mov    %rax,%rdi
 	call   1380 <getModularityMatrix@plt>
 	mov    %rax,%r12
 	mov    %ebp,%edi
 	call   1270 <create_1d_array_int@plt>
 	mov    %rax,%rbx
 	test   %ebp,%ebp
-	jle    1dbf <get_community+0x60>
-	mov    %ebp,%edx
-	mov    $0x0,%eax
-	mov    %eax,(%rbx,%rax,4)
-	add    $0x1,%rax
-	cmp    %rdx,%rax
-	jne    1db3 <get_community+0x54>
+	jle    1de1 <get_community_assignment+0x70>
+	mov    %ebp,%eax
+	mov    $0x0,%edx
+	mov    %edx,(%rbx,%rdx,4)
+	add    $0x1,%rdx
+	cmp    %rax,%rdx
+	jne    1dd5 <get_community_assignment+0x64>
 	movl   $0x0,0x4(%rsp)
 	mov    %rbx,%rdx
 	mov    %ebp,%esi
 	mov    %r12,%rdi
 	call   1260 <modularityScore@plt>
-	mov    %r15,%r9
+	mov    %r13,%r9
 	lea    0x4(%rsp),%r8
 	mov    %r12,%rcx
 	mov    %rbx,%rdx
 	mov    %ebp,%esi
 	mov    %r14,%rdi
 	call   1370 <divide_community@plt>
 	mov    %ebp,%esi
 	mov    %r12,%rdi
 	call   12f0 <free_2d_array@plt>
-	mov    %r13,%rdi
-	call   12a0 <free@plt>
 	mov    0x8(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    1e1d <get_community+0xbe>
-	add    $0x18,%rsp
+	jne    1e38 <get_community_assignment+0xc7>
+	mov    %r13,%rax
+	add    $0x10,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
-	pop    %r15
 	ret
 	call   1340 <__stack_chk_fail@plt>
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.fini {}

```diff
@@ -1,11 +1,11 @@
 
 
 
 Disassembly of section .fini:
 
-0000000000001e24 <_fini>:
+0000000000001e40 <_fini>:
 _fini():
 	endbr64
 	sub    $0x8,%rsp
 	add    $0x8,%rsp
 	ret
```

#### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -1,12 +1,13 @@
 
 Hex dump of section '.eh_frame_hdr':
-  0x00002068 011b033b 8c000000 10000000 b8efffff ...;............
-  0x00002078 a8000000 78f1ffff d0000000 88f1ffff ....x...........
-  0x00002088 e8000000 f1f3ffff 00010000 0bf5ffff ................
-  0x00002098 3c010000 4ef5ffff 50010000 87f5ffff <...N...P.......
-  0x000020a8 6c010000 26f6ffff a8010000 5ff6ffff l...&......._...
-  0x000020b8 c4010000 fef6ffff 00020000 36f7ffff ............6...
-  0x000020c8 30020000 3ff9ffff 80020000 d1f9ffff 0...?...........
-  0x000020d8 ac020000 3cfaffff d8020000 64faffff ....<.......d...
-  0x000020e8 ec020000 f7fcffff 3c030000          ........<...
+  0x00002068 011b033b 94000000 11000000 b8efffff ...;............
+  0x00002078 b0000000 78f1ffff d8000000 88f1ffff ....x...........
+  0x00002088 f0000000 f1f3ffff 08010000 0bf5ffff ................
+  0x00002098 44010000 4ef5ffff 58010000 87f5ffff D...N...X.......
+  0x000020a8 74010000 26f6ffff b0010000 5ff6ffff t...&......._...
+  0x000020b8 cc010000 fef6ffff 08020000 36f7ffff ............6...
+  0x000020c8 34020000 48f7ffff 50020000 51f9ffff 4...H...P...Q...
+  0x000020d8 a0020000 e3f9ffff cc020000 4efaffff ............N...
+  0x000020e8 f8020000 76faffff 0c030000 09fdffff ....v...........
+  0x000020f8 5c030000                            \...
```

#### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,51 +1,52 @@
 
 Hex dump of section '.eh_frame':
-  0x000020f8 14000000 00000000 017a5200 01781001 .........zR..x..
-  0x00002108 1b0c0708 90010000 24000000 1c000000 ........$.......
-  0x00002118 08efffff c0010000 000e1046 0e184a0f ...........F..J.
-  0x00002128 0b770880 003f1a3a 2a332422 00000000 .w...?.:*3$"....
-  0x00002138 14000000 44000000 a0f0ffff 10000000 ....D...........
-  0x00002148 00000000 00000000 14000000 5c000000 ............\...
-  0x00002158 98f0ffff b0010000 00000000 00000000 ................
-  0x00002168 38000000 74000000 e9f2ffff 1a010000 8...t...........
-  0x00002178 00460e10 8d02420e 188c0341 0e208604 .F....B....A. ..
-  0x00002188 410e2883 05440e30 0305010e 28410e20 A.(..D.0....(A. 
-  0x00002198 410e1842 0e10420e 08000000 10000000 A..B..B.........
-  0x000021a8 b0000000 c7f3ffff 43000000 00000000 ........C.......
-  0x000021b8 18000000 c4000000 f6f3ffff 39000000 ............9...
-  0x000021c8 00480e10 550a0e08 410b0000 38000000 .H..U...A...8...
-  0x000021d8 e0000000 13f4ffff 9f000000 00460e10 .............F..
-  0x000021e8 8d02420e 188c0341 0e208604 410e2883 ..B....A. ..A.(.
-  0x000021f8 05440e30 024f0a0e 28410e20 410e1842 .D.0.O..(A. A..B
-  0x00002208 0e10420e 08410b00 18000000 1c010000 ..B..A..........
-  0x00002218 76f4ffff 39000000 00480e10 550a0e08 v...9....H..U...
-  0x00002228 410b0000 38000000 38010000 93f4ffff A...8...8.......
-  0x00002238 9f000000 00460e10 8d02420e 188c0341 .....F....B....A
-  0x00002248 0e208604 410e2883 05440e30 024f0a0e . ..A.(..D.0.O..
-  0x00002258 28410e20 410e1842 0e10420e 08410b00 (A. A..B..B..A..
-  0x00002268 2c000000 74010000 f6f4ffff 38000000 ,...t.......8...
-  0x00002278 00460e10 8c02410e 18860341 0e208304 .F....A....A. ..
-  0x00002288 6c0e1841 0e10420e 08000000 00000000 l..A..B.........
-  0x00002298 4c000000 a4010000 fef4ffff 09020000 L...............
-  0x000022a8 00460e10 8f02420e 188e0342 0e208d04 .F....B....B. ..
-  0x000022b8 420e288c 05410e30 8606410e 38830747 B.(..A.0..A.8..G
-  0x000022c8 0ec00103 5d010a0e 38410e30 410e2842 ....]...8A.0A.(B
-  0x000022d8 0e20420e 18420e10 420e0841 0b000000 . B..B..B..A....
-  0x000022e8 28000000 f4010000 b7f6ffff 92000000 (...............
-  0x000022f8 00460e10 8c02410e 18860341 0e208304 .F....A....A. ..
-  0x00002308 02860e18 410e1042 0e080000 28000000 ....A..B....(...
-  0x00002318 20020000 1df7ffff 6b000000 00460e10  .......k....F..
-  0x00002328 8c02410e 18860341 0e208304 025f0e18 ..A....A. ..._..
-  0x00002338 410e1042 0e080000 10000000 4c020000 A..B........L...
-  0x00002348 5cf7ffff 28000000 00000000 4c000000 \...(.......L...
-  0x00002358 60020000 70f7ffff 93020000 00460e10 `...p........F..
-  0x00002368 8f02420e 188e0342 0e208d04 420e288c ..B....B. ..B.(.
-  0x00002378 05410e30 8606410e 38830744 0e900103 .A.0..A.8..D....
-  0x00002388 fd010a0e 38410e30 410e2842 0e20420e ....8A.0A.(B. B.
-  0x00002398 18420e10 420e0841 0b000000 48000000 .B..B..A....H...
-  0x000023a8 b0020000 b3f9ffff c3000000 00460e10 .............F..
-  0x000023b8 8f02420e 188e0342 0e208d04 420e288c ..B....B. ..B.(.
-  0x000023c8 05410e30 8606410e 38830744 0e5002a1 .A.0..A.8..D.P..
-  0x000023d8 0a0e3841 0e30410e 28420e20 420e1842 ..8A.0A.(B. B..B
-  0x000023e8 0e10420e 08410b00 00000000          ..B..A......
+  0x00002100 14000000 00000000 017a5200 01781001 .........zR..x..
+  0x00002110 1b0c0708 90010000 24000000 1c000000 ........$.......
+  0x00002120 00efffff c0010000 000e1046 0e184a0f ...........F..J.
+  0x00002130 0b770880 003f1a3a 2a332422 00000000 .w...?.:*3$"....
+  0x00002140 14000000 44000000 98f0ffff 10000000 ....D...........
+  0x00002150 00000000 00000000 14000000 5c000000 ............\...
+  0x00002160 90f0ffff b0010000 00000000 00000000 ................
+  0x00002170 38000000 74000000 e1f2ffff 1a010000 8...t...........
+  0x00002180 00460e10 8d02420e 188c0341 0e208604 .F....B....A. ..
+  0x00002190 410e2883 05440e30 0305010e 28410e20 A.(..D.0....(A. 
+  0x000021a0 410e1842 0e10420e 08000000 10000000 A..B..B.........
+  0x000021b0 b0000000 bff3ffff 43000000 00000000 ........C.......
+  0x000021c0 18000000 c4000000 eef3ffff 39000000 ............9...
+  0x000021d0 00480e10 550a0e08 410b0000 38000000 .H..U...A...8...
+  0x000021e0 e0000000 0bf4ffff 9f000000 00460e10 .............F..
+  0x000021f0 8d02420e 188c0341 0e208604 410e2883 ..B....A. ..A.(.
+  0x00002200 05440e30 024f0a0e 28410e20 410e1842 .D.0.O..(A. A..B
+  0x00002210 0e10420e 08410b00 18000000 1c010000 ..B..A..........
+  0x00002220 6ef4ffff 39000000 00480e10 550a0e08 n...9....H..U...
+  0x00002230 410b0000 38000000 38010000 8bf4ffff A...8...8.......
+  0x00002240 9f000000 00460e10 8d02420e 188c0341 .....F....B....A
+  0x00002250 0e208604 410e2883 05440e30 024f0a0e . ..A.(..D.0.O..
+  0x00002260 28410e20 410e1842 0e10420e 08410b00 (A. A..B..B..A..
+  0x00002270 28000000 74010000 eef4ffff 38000000 (...t.......8...
+  0x00002280 00460e10 8c02410e 18860341 0e208304 .F....A....A. ..
+  0x00002290 6c0e1841 0e10420e 08000000 18000000 l..A..B.........
+  0x000022a0 a0010000 faf4ffff 12000000 00480e10 .............H..
+  0x000022b0 490e0800 00000000 4c000000 bc010000 I.......L.......
+  0x000022c0 f0f4ffff 09020000 00460e10 8f02420e .........F....B.
+  0x000022d0 188e0342 0e208d04 420e288c 05410e30 ...B. ..B.(..A.0
+  0x000022e0 8606410e 38830747 0ec00103 5d010a0e ..A.8..G....]...
+  0x000022f0 38410e30 410e2842 0e20420e 18420e10 8A.0A.(B. B..B..
+  0x00002300 420e0841 0b000000 28000000 0c020000 B..A....(.......
+  0x00002310 a9f6ffff 92000000 00460e10 8c02410e .........F....A.
+  0x00002320 18860341 0e208304 02860e18 410e1042 ...A. ......A..B
+  0x00002330 0e080000 28000000 38020000 0ff7ffff ....(...8.......
+  0x00002340 6b000000 00460e10 8c02410e 18860341 k....F....A....A
+  0x00002350 0e208304 025f0e18 410e1042 0e080000 . ..._..A..B....
+  0x00002360 10000000 64020000 4ef7ffff 28000000 ....d...N...(...
+  0x00002370 00000000 4c000000 78020000 62f7ffff ....L...x...b...
+  0x00002380 93020000 00460e10 8f02420e 188e0342 .....F....B....B
+  0x00002390 0e208d04 420e288c 05410e30 8606410e . ..B.(..A.0..A.
+  0x000023a0 38830744 0e900103 fd010a0e 38410e30 8..D........8A.0
+  0x000023b0 410e2842 0e20420e 18420e10 420e0841 A.(B. B..B..B..A
+  0x000023c0 0b000000 40000000 c8020000 a5f9ffff ....@...........
+  0x000023d0 cc000000 00460e10 8e02420e 188d0342 .....F....B....B
+  0x000023e0 0e208c04 410e2886 05410e30 8306440e . ..A.(..A.0..D.
+  0x000023f0 4002ae0a 0e30410e 28410e20 420e1842 @....0A.(A. B..B
+  0x00002400 0e10420e 08410b00 00000000          ..B..A......
```

#### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -18,47 +18,48 @@
   0x000000f0 5f5f005f 5f474e55 5f45485f 4652414d __.__GNU_EH_FRAM
   0x00000100 455f4844 52005f66 696e6900 5f474c4f E_HDR._fini._GLO
   0x00000110 42414c5f 4f464653 45545f54 41424c45 BAL_OFFSET_TABLE
   0x00000120 5f005f5f 544d435f 454e445f 5f005f5f _.__TMC_END__.__
   0x00000130 64736f5f 68616e64 6c65005f 44594e41 dso_handle._DYNA
   0x00000140 4d494300 5f696e69 74006773 6c5f6569 MIC._init.gsl_ei
   0x00000150 67656e5f 73796d6d 765f616c 6c6f6300 gen_symmv_alloc.
-  0x00000160 6765745f 636f6d6d 756e6974 79005f5f get_community.__
-  0x00000170 676d6f6e 5f737461 72745f5f 00657869 gmon_start__.exi
-  0x00000180 7440474c 4942435f 322e322e 35005f5f t@GLIBC_2.2.5.__
-  0x00000190 7072696e 74665f63 686b4047 4c494243 printf_chk@GLIBC
-  0x000001a0 5f322e33 2e340067 736c5f6d 61747269 _2.3.4.gsl_matri
-  0x000001b0 785f616c 6c6f6300 67657445 6967656e x_alloc.getEigen
-  0x000001c0 56656374 6f72006d 616c6c6f 6340474c Vector.malloc@GL
-  0x000001d0 4942435f 322e322e 35006372 65617465 IBC_2.2.5.create
-  0x000001e0 5f32645f 61727261 79006d6f 64756c61 _2d_array.modula
-  0x000001f0 72697479 53636f72 65005f49 544d5f64 rityScore._ITM_d
-  0x00000200 65726567 69737465 72544d43 6c6f6e65 eregisterTMClone
-  0x00000210 5461626c 65006372 65617465 5f31645f Table.create_1d_
-  0x00000220 61727261 795f696e 74006773 6c5f6569 array_int.gsl_ei
-  0x00000230 67656e5f 73796d6d 765f736f 72740067 gen_symmv_sort.g
-  0x00000240 736c5f65 6967656e 5f73796d 6d760066 sl_eigen_symmv.f
-  0x00000250 72656540 474c4942 435f322e 322e3500 ree@GLIBC_2.2.5.
-  0x00000260 5f49544d 5f726567 69737465 72544d43 _ITM_registerTMC
-  0x00000270 6c6f6e65 5461626c 65006773 6c5f7665 loneTable.gsl_ve
-  0x00000280 63746f72 5f616c6c 6f63005f 5f637861 ctor_alloc.__cxa
-  0x00000290 5f66696e 616c697a 6540474c 4942435f _finalize@GLIBC_
-  0x000002a0 322e322e 35006773 6c5f7665 63746f72 2.2.5.gsl_vector
-  0x000002b0 5f676574 00736570 61726174 655f6164 _get.separate_ad
-  0x000002c0 6a5f6d61 74726978 0067736c 5f656967 j_matrix.gsl_eig
-  0x000002d0 656e5f73 796d6d76 5f667265 65006672 en_symmv_free.fr
-  0x000002e0 65655f32 645f6172 72617900 63726561 ee_2d_array.crea
-  0x000002f0 74655f32 645f6172 7261795f 696e7400 te_2d_array_int.
-  0x00000300 63726561 74655f61 646a5f6d 61747269 create_adj_matri
-  0x00000310 78006773 6c5f6d61 74726978 5f667265 x.gsl_matrix_fre
-  0x00000320 65006773 6c5f6d61 74726978 5f766965 e.gsl_matrix_vie
-  0x00000330 775f6172 72617900 67736c5f 76656374 w_array.gsl_vect
-  0x00000340 6f725f66 72656500 5f5f7374 61636b5f or_free.__stack_
-  0x00000350 63686b5f 6661696c 40474c49 42435f32 chk_fail@GLIBC_2
-  0x00000360 2e340066 696e616c 5f636f6d 6d756e69 .4.final_communi
-  0x00000370 74795f61 73736967 6e6d656e 74006773 ty_assignment.gs
-  0x00000380 6c5f6d61 74726978 5f636f6c 756d6e00 l_matrix_column.
-  0x00000390 64697669 64655f63 6f6d6d75 6e697479 divide_community
-  0x000003a0 00676574 4d6f6475 6c617269 74794d61 .getModularityMa
-  0x000003b0 74726978 00637265 6174655f 31645f61 trix.create_1d_a
-  0x000003c0 72726179 00                         rray.
+  0x00000160 5f5f676d 6f6e5f73 74617274 5f5f0065 __gmon_start__.e
+  0x00000170 78697440 474c4942 435f322e 322e3500 xit@GLIBC_2.2.5.
+  0x00000180 5f5f7072 696e7466 5f63686b 40474c49 __printf_chk@GLI
+  0x00000190 42435f32 2e332e34 0067736c 5f6d6174 BC_2.3.4.gsl_mat
+  0x000001a0 7269785f 616c6c6f 63006765 74456967 rix_alloc.getEig
+  0x000001b0 656e5665 63746f72 006d616c 6c6f6340 enVector.malloc@
+  0x000001c0 474c4942 435f322e 322e3500 63726561 GLIBC_2.2.5.crea
+  0x000001d0 74655f32 645f6172 72617900 6d6f6475 te_2d_array.modu
+  0x000001e0 6c617269 74795363 6f726500 5f49544d larityScore._ITM
+  0x000001f0 5f646572 65676973 74657254 4d436c6f _deregisterTMClo
+  0x00000200 6e655461 626c6500 63726561 74655f31 neTable.create_1
+  0x00000210 645f6172 7261795f 696e7400 67736c5f d_array_int.gsl_
+  0x00000220 65696765 6e5f7379 6d6d765f 736f7274 eigen_symmv_sort
+  0x00000230 0067736c 5f656967 656e5f73 796d6d76 .gsl_eigen_symmv
+  0x00000240 00676574 5f636f6d 6d756e69 74795f61 .get_community_a
+  0x00000250 73736967 6e6d656e 74006672 65654047 ssignment.free@G
+  0x00000260 4c494243 5f322e32 2e35005f 49544d5f LIBC_2.2.5._ITM_
+  0x00000270 72656769 73746572 544d436c 6f6e6554 registerTMCloneT
+  0x00000280 61626c65 0067736c 5f766563 746f725f able.gsl_vector_
+  0x00000290 616c6c6f 63005f5f 6378615f 66696e61 alloc.__cxa_fina
+  0x000002a0 6c697a65 40474c49 42435f32 2e322e35 lize@GLIBC_2.2.5
+  0x000002b0 0067736c 5f766563 746f725f 67657400 .gsl_vector_get.
+  0x000002c0 73657061 72617465 5f61646a 5f6d6174 separate_adj_mat
+  0x000002d0 72697800 67736c5f 65696765 6e5f7379 rix.gsl_eigen_sy
+  0x000002e0 6d6d765f 66726565 00667265 655f3264 mmv_free.free_2d
+  0x000002f0 5f617272 61790066 7265655f 31645f61 _array.free_1d_a
+  0x00000300 72726179 00637265 6174655f 32645f61 rray.create_2d_a
+  0x00000310 72726179 5f696e74 00637265 6174655f rray_int.create_
+  0x00000320 61646a5f 6d617472 69780067 736c5f6d adj_matrix.gsl_m
+  0x00000330 61747269 785f6672 65650067 736c5f6d atrix_free.gsl_m
+  0x00000340 61747269 785f7669 65775f61 72726179 atrix_view_array
+  0x00000350 0067736c 5f766563 746f725f 66726565 .gsl_vector_free
+  0x00000360 005f5f73 7461636b 5f63686b 5f666169 .__stack_chk_fai
+  0x00000370 6c40474c 4942435f 322e3400 66696e61 l@GLIBC_2.4.fina
+  0x00000380 6c5f636f 6d6d756e 6974795f 61737369 l_community_assi
+  0x00000390 676e6d65 6e740067 736c5f6d 61747269 gnment.gsl_matri
+  0x000003a0 785f636f 6c756d6e 00646976 6964655f x_column.divide_
+  0x000003b0 636f6d6d 756e6974 79006765 744d6f64 community.getMod
+  0x000003c0 756c6172 6974794d 61747269 78006372 ularityMatrix.cr
+  0x000003d0 65617465 5f31645f 61727261 7900     eate_1d_array.
```

### Comparing `apache-age-community-detection-0.1.3/age_community_detection/lib/library.so` & `apache-age-community-detection-0.1.4/age_community_detection/lib/library.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 8% similar despite different names*

#### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              DYN (Shared object file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          64 (bytes into file)
-  Start of section headers:          15192 (bytes into file)
+  Start of section headers:          15240 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           56 (bytes)
   Number of program headers:         11
   Size of section headers:           64 (bytes)
   Number of section headers:         30
   Section header string table index: 29
```

#### readelf --wide --program-header {}

```diff
@@ -1,23 +1,23 @@
 
 Elf file type is DYN (Shared object file)
 Entry point 0x0
 There are 11 program headers, starting at offset 64
 
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
-  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x000ca0 0x000ca0 R   0x1000
-  LOAD           0x001000 0x0000000000001000 0x0000000000001000 0x000e31 0x000e31 R E 0x1000
-  LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x0003f4 0x0003f4 R   0x1000
+  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x000ce0 0x000ce0 R   0x1000
+  LOAD           0x001000 0x0000000000001000 0x0000000000001000 0x000e4d 0x000e4d R E 0x1000
+  LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x00040c 0x00040c R   0x1000
   LOAD           0x002e00 0x0000000000003e00 0x0000000000003e00 0x0002f8 0x000300 RW  0x1000
   DYNAMIC        0x002e10 0x0000000000003e10 0x0000000000003e10 0x0001d0 0x0001d0 RW  0x8
   NOTE           0x0002a8 0x00000000000002a8 0x00000000000002a8 0x000020 0x000020 R   0x8
   NOTE           0x0002c8 0x00000000000002c8 0x00000000000002c8 0x000024 0x000024 R   0x4
   GNU_PROPERTY   0x0002a8 0x00000000000002a8 0x00000000000002a8 0x000020 0x000020 R   0x8
-  GNU_EH_FRAME   0x002068 0x0000000000002068 0x0000000000002068 0x00008c 0x00008c R   0x4
+  GNU_EH_FRAME   0x002068 0x0000000000002068 0x0000000000002068 0x000094 0x000094 R   0x4
   GNU_STACK      0x000000 0x0000000000000000 0x0000000000000000 0x000000 0x000000 RW  0x10
   GNU_RELRO      0x002e00 0x0000000000003e00 0x0000000000003e00 0x000200 0x000200 R   0x1
 
  Section to Segment mapping:
   Segment Sections...
    00     .note.gnu.property .note.gnu.build-id .gnu.hash .dynsym .dynstr .gnu.version .gnu.version_r .rela.dyn .rela.plt 
    01     .init .plt .plt.got .plt.sec .text .fini
```

#### readelf --wide --sections {}

```diff
@@ -1,39 +1,39 @@
-There are 30 section headers, starting at offset 0x3b58:
+There are 30 section headers, starting at offset 0x3b88:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .note.gnu.property NOTE            00000000000002a8 0002a8 000020 00   A  0   0  8
   [ 2] .note.gnu.build-id NOTE            00000000000002c8 0002c8 000024 00   A  0   0  4
-  [ 3] .gnu.hash         GNU_HASH        00000000000002f0 0002f0 000060 00   A  4   0  8
-  [ 4] .dynsym           DYNSYM          0000000000000350 000350 000330 18   A  5   1  8
-  [ 5] .dynstr           STRTAB          0000000000000680 000680 00026a 00   A  0   0  1
-  [ 6] .gnu.version      VERSYM          00000000000008ea 0008ea 000044 02   A  4   0  2
-  [ 7] .gnu.version_r    VERNEED         0000000000000930 000930 000040 00   A  5   1  8
-  [ 8] .rela.dyn         RELA            0000000000000970 000970 0000a8 18   A  4   0  8
-  [ 9] .rela.plt         RELA            0000000000000a18 000a18 000288 18  AI  4  23  8
+  [ 3] .gnu.hash         GNU_HASH        00000000000002f0 0002f0 000064 00   A  4   0  8
+  [ 4] .dynsym           DYNSYM          0000000000000358 000358 000348 18   A  5   1  8
+  [ 5] .dynstr           STRTAB          00000000000006a0 0006a0 000283 00   A  0   0  1
+  [ 6] .gnu.version      VERSYM          0000000000000924 000924 000046 02   A  4   0  2
+  [ 7] .gnu.version_r    VERNEED         0000000000000970 000970 000040 00   A  5   1  8
+  [ 8] .rela.dyn         RELA            00000000000009b0 0009b0 0000a8 18   A  4   0  8
+  [ 9] .rela.plt         RELA            0000000000000a58 000a58 000288 18  AI  4  23  8
   [10] .init             PROGBITS        0000000000001000 001000 00001b 00  AX  0   0  4
   [11] .plt              PROGBITS        0000000000001020 001020 0001c0 10  AX  0   0 16
   [12] .plt.got          PROGBITS        00000000000011e0 0011e0 000010 10  AX  0   0 16
   [13] .plt.sec          PROGBITS        00000000000011f0 0011f0 0001b0 10  AX  0   0 16
-  [14] .text             PROGBITS        00000000000013a0 0013a0 000a82 00  AX  0   0 16
-  [15] .fini             PROGBITS        0000000000001e24 001e24 00000d 00  AX  0   0  4
+  [14] .text             PROGBITS        00000000000013a0 0013a0 000a9d 00  AX  0   0 16
+  [15] .fini             PROGBITS        0000000000001e40 001e40 00000d 00  AX  0   0  4
   [16] .rodata           PROGBITS        0000000000002000 002000 000068 00   A  0   0  8
-  [17] .eh_frame_hdr     PROGBITS        0000000000002068 002068 00008c 00   A  0   0  4
-  [18] .eh_frame         PROGBITS        00000000000020f8 0020f8 0002fc 00   A  0   0  8
+  [17] .eh_frame_hdr     PROGBITS        0000000000002068 002068 000094 00   A  0   0  4
+  [18] .eh_frame         PROGBITS        0000000000002100 002100 00030c 00   A  0   0  8
   [19] .init_array       INIT_ARRAY      0000000000003e00 002e00 000008 08  WA  0   0  8
   [20] .fini_array       FINI_ARRAY      0000000000003e08 002e08 000008 08  WA  0   0  8
   [21] .dynamic          DYNAMIC         0000000000003e10 002e10 0001d0 10  WA  5   0  8
   [22] .got              PROGBITS        0000000000003fe0 002fe0 000020 08  WA  0   0  8
   [23] .got.plt          PROGBITS        0000000000004000 003000 0000f0 08  WA  0   0  8
   [24] .data             PROGBITS        00000000000040f0 0030f0 000008 00  WA  0   0  8
   [25] .bss              NOBITS          00000000000040f8 0030f8 000008 00  WA  0   0  1
   [26] .comment          PROGBITS        0000000000000000 0030f8 00002b 01  MS  0   0  1
-  [27] .symtab           SYMTAB          0000000000000000 003128 000558 18     28  24  8
-  [28] .strtab           STRTAB          0000000000000000 003680 0003c5 00      0   0  1
-  [29] .shstrtab         STRTAB          0000000000000000 003a45 00010d 00      0   0  1
+  [27] .symtab           SYMTAB          0000000000000000 003128 000570 18     28  24  8
+  [28] .strtab           STRTAB          0000000000000000 003698 0003de 00      0   0  1
+  [29] .shstrtab         STRTAB          0000000000000000 003a76 00010d 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

#### readelf --wide --symbols {}

```diff
@@ -1,9 +1,9 @@
 
-Symbol table '.dynsym' contains 34 entries:
+Symbol table '.dynsym' contains 35 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_eigen_symmv_alloc
      2: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
      3: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@GLIBC_2.2.5 (2)
      4: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __printf_chk@GLIBC_2.3.4 (3)
      5: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_alloc
@@ -19,79 +19,81 @@
     15: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_eigen_symmv_free
     16: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_free
     17: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_view_array
     18: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_vector_free
     19: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail@GLIBC_2.4 (4)
     20: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_column
     21: 00000000000015ef   159 FUNC    GLOBAL DEFAULT   14 create_2d_array
-    22: 00000000000019a7   146 FUNC    GLOBAL DEFAULT   14 create_adj_matrix
-    23: 0000000000001aa4    40 FUNC    GLOBAL DEFAULT   14 final_community_assignment
-    24: 0000000000001459   282 FUNC    GLOBAL DEFAULT   14 getModularityMatrix
-    25: 0000000000001d5f   195 FUNC    GLOBAL DEFAULT   14 get_community
+    22: 000000000000179e    18 FUNC    GLOBAL DEFAULT   14 free_1d_array
+    23: 00000000000019b9   146 FUNC    GLOBAL DEFAULT   14 create_adj_matrix
+    24: 0000000000001ab6    40 FUNC    GLOBAL DEFAULT   14 final_community_assignment
+    25: 0000000000001459   282 FUNC    GLOBAL DEFAULT   14 getModularityMatrix
     26: 000000000000168e    57 FUNC    GLOBAL DEFAULT   14 create_1d_array_int
-    27: 0000000000001acc   659 FUNC    GLOBAL DEFAULT   14 divide_community
+    27: 0000000000001ade   659 FUNC    GLOBAL DEFAULT   14 divide_community
     28: 00000000000015b6    57 FUNC    GLOBAL DEFAULT   14 create_1d_array
-    29: 000000000000179e   521 FUNC    GLOBAL DEFAULT   14 getEigenVector
+    29: 00000000000017b0   521 FUNC    GLOBAL DEFAULT   14 getEigenVector
     30: 0000000000001573    67 FUNC    GLOBAL DEFAULT   14 modularityScore
-    31: 0000000000001a39   107 FUNC    GLOBAL DEFAULT   14 separate_adj_matrix
-    32: 0000000000001766    56 FUNC    GLOBAL DEFAULT   14 free_2d_array
-    33: 00000000000016c7   159 FUNC    GLOBAL DEFAULT   14 create_2d_array_int
+    31: 0000000000001d71   204 FUNC    GLOBAL DEFAULT   14 get_community_assignment
+    32: 0000000000001a4b   107 FUNC    GLOBAL DEFAULT   14 separate_adj_matrix
+    33: 0000000000001766    56 FUNC    GLOBAL DEFAULT   14 free_2d_array
+    34: 00000000000016c7   159 FUNC    GLOBAL DEFAULT   14 create_2d_array_int
 
-Symbol table '.symtab' contains 57 entries:
+Symbol table '.symtab' contains 58 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
      2: 00000000000013a0     0 FUNC    LOCAL  DEFAULT   14 deregister_tm_clones
      3: 00000000000013d0     0 FUNC    LOCAL  DEFAULT   14 register_tm_clones
      4: 0000000000001410     0 FUNC    LOCAL  DEFAULT   14 __do_global_dtors_aux
      5: 00000000000040f8     1 OBJECT  LOCAL  DEFAULT   25 completed.0
      6: 0000000000003e08     0 OBJECT  LOCAL  DEFAULT   20 __do_global_dtors_aux_fini_array_entry
      7: 0000000000001450     0 FUNC    LOCAL  DEFAULT   14 frame_dummy
      8: 0000000000003e00     0 OBJECT  LOCAL  DEFAULT   19 __frame_dummy_init_array_entry
      9: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS modularity.c
     10: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS memory.c
     11: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS eigen.c
     12: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS community_detection.c
-    13: 0000000000001acc   659 FUNC    LOCAL  DEFAULT   14 divide_community.localalias
+    13: 0000000000001ade   659 FUNC    LOCAL  DEFAULT   14 divide_community.localalias
     14: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
-    15: 00000000000023f0     0 OBJECT  LOCAL  DEFAULT   18 __FRAME_END__
+    15: 0000000000002408     0 OBJECT  LOCAL  DEFAULT   18 __FRAME_END__
     16: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
     17: 0000000000002068     0 NOTYPE  LOCAL  DEFAULT   17 __GNU_EH_FRAME_HDR
-    18: 0000000000001e24     0 FUNC    LOCAL  DEFAULT   15 _fini
+    18: 0000000000001e40     0 FUNC    LOCAL  DEFAULT   15 _fini
     19: 0000000000004000     0 OBJECT  LOCAL  DEFAULT   23 _GLOBAL_OFFSET_TABLE_
     20: 00000000000040f8     0 OBJECT  LOCAL  DEFAULT   24 __TMC_END__
     21: 00000000000040f0     0 OBJECT  LOCAL  DEFAULT   24 __dso_handle
     22: 0000000000003e10     0 OBJECT  LOCAL  DEFAULT   21 _DYNAMIC
     23: 0000000000001000     0 FUNC    LOCAL  DEFAULT   10 _init
     24: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_eigen_symmv_alloc
-    25: 0000000000001d5f   195 FUNC    GLOBAL DEFAULT   14 get_community
-    26: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
-    27: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@GLIBC_2.2.5
-    28: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __printf_chk@GLIBC_2.3.4
-    29: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_alloc
-    30: 000000000000179e   521 FUNC    GLOBAL DEFAULT   14 getEigenVector
-    31: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@GLIBC_2.2.5
-    32: 00000000000015ef   159 FUNC    GLOBAL DEFAULT   14 create_2d_array
-    33: 0000000000001573    67 FUNC    GLOBAL DEFAULT   14 modularityScore
-    34: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
-    35: 000000000000168e    57 FUNC    GLOBAL DEFAULT   14 create_1d_array_int
-    36: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_eigen_symmv_sort
-    37: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_eigen_symmv
+    25: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
+    26: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@GLIBC_2.2.5
+    27: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __printf_chk@GLIBC_2.3.4
+    28: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_alloc
+    29: 00000000000017b0   521 FUNC    GLOBAL DEFAULT   14 getEigenVector
+    30: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@GLIBC_2.2.5
+    31: 00000000000015ef   159 FUNC    GLOBAL DEFAULT   14 create_2d_array
+    32: 0000000000001573    67 FUNC    GLOBAL DEFAULT   14 modularityScore
+    33: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
+    34: 000000000000168e    57 FUNC    GLOBAL DEFAULT   14 create_1d_array_int
+    35: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_eigen_symmv_sort
+    36: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_eigen_symmv
+    37: 0000000000001d71   204 FUNC    GLOBAL DEFAULT   14 get_community_assignment
     38: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@GLIBC_2.2.5
     39: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
     40: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_vector_alloc
     41: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5
     42: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_vector_get
-    43: 0000000000001a39   107 FUNC    GLOBAL DEFAULT   14 separate_adj_matrix
+    43: 0000000000001a4b   107 FUNC    GLOBAL DEFAULT   14 separate_adj_matrix
     44: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_eigen_symmv_free
     45: 0000000000001766    56 FUNC    GLOBAL DEFAULT   14 free_2d_array
-    46: 00000000000016c7   159 FUNC    GLOBAL DEFAULT   14 create_2d_array_int
-    47: 00000000000019a7   146 FUNC    GLOBAL DEFAULT   14 create_adj_matrix
-    48: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_free
-    49: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_view_array
-    50: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_vector_free
-    51: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail@GLIBC_2.4
-    52: 0000000000001aa4    40 FUNC    GLOBAL DEFAULT   14 final_community_assignment
-    53: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_column
-    54: 0000000000001acc   659 FUNC    GLOBAL DEFAULT   14 divide_community
-    55: 0000000000001459   282 FUNC    GLOBAL DEFAULT   14 getModularityMatrix
-    56: 00000000000015b6    57 FUNC    GLOBAL DEFAULT   14 create_1d_array
+    46: 000000000000179e    18 FUNC    GLOBAL DEFAULT   14 free_1d_array
+    47: 00000000000016c7   159 FUNC    GLOBAL DEFAULT   14 create_2d_array_int
+    48: 00000000000019b9   146 FUNC    GLOBAL DEFAULT   14 create_adj_matrix
+    49: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_free
+    50: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_view_array
+    51: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_vector_free
+    52: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail@GLIBC_2.4
+    53: 0000000000001ab6    40 FUNC    GLOBAL DEFAULT   14 final_community_assignment
+    54: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND gsl_matrix_column
+    55: 0000000000001ade   659 FUNC    GLOBAL DEFAULT   14 divide_community
+    56: 0000000000001459   282 FUNC    GLOBAL DEFAULT   14 getModularityMatrix
+    57: 00000000000015b6    57 FUNC    GLOBAL DEFAULT   14 create_1d_array
```

#### readelf --wide --relocs {}

```diff
@@ -1,40 +1,40 @@
 
-Relocation section '.rela.dyn' at offset 0x970 contains 7 entries:
+Relocation section '.rela.dyn' at offset 0x9b0 contains 7 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000003e00  0000000000000008 R_X86_64_RELATIVE                         1450
 0000000000003e08  0000000000000008 R_X86_64_RELATIVE                         1410
 00000000000040f0  0000000000000008 R_X86_64_RELATIVE                         40f0
 0000000000003fe0  0000000200000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
 0000000000003fe8  0000000700000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
 0000000000003ff0  0000000b00000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
 0000000000003ff8  0000000d00000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
 
-Relocation section '.rela.plt' at offset 0xa18 contains 27 entries:
+Relocation section '.rela.plt' at offset 0xa58 contains 27 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000004018  0000000100000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_eigen_symmv_alloc + 0
 0000000000004020  0000000300000007 R_X86_64_JUMP_SLOT     0000000000000000 exit@GLIBC_2.2.5 + 0
 0000000000004028  0000000400000007 R_X86_64_JUMP_SLOT     0000000000000000 __printf_chk@GLIBC_2.3.4 + 0
 0000000000004030  0000000500000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_matrix_alloc + 0
-0000000000004038  0000001d00000007 R_X86_64_JUMP_SLOT     000000000000179e getEigenVector + 0
+0000000000004038  0000001d00000007 R_X86_64_JUMP_SLOT     00000000000017b0 getEigenVector + 0
 0000000000004040  0000000600000007 R_X86_64_JUMP_SLOT     0000000000000000 malloc@GLIBC_2.2.5 + 0
 0000000000004048  0000001500000007 R_X86_64_JUMP_SLOT     00000000000015ef create_2d_array + 0
 0000000000004050  0000001e00000007 R_X86_64_JUMP_SLOT     0000000000001573 modularityScore + 0
 0000000000004058  0000001a00000007 R_X86_64_JUMP_SLOT     000000000000168e create_1d_array_int + 0
 0000000000004060  0000000800000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_eigen_symmv_sort + 0
 0000000000004068  0000000900000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_eigen_symmv + 0
 0000000000004070  0000000a00000007 R_X86_64_JUMP_SLOT     0000000000000000 free@GLIBC_2.2.5 + 0
 0000000000004078  0000000c00000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_vector_alloc + 0
 0000000000004080  0000000e00000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_vector_get + 0
-0000000000004088  0000001f00000007 R_X86_64_JUMP_SLOT     0000000000001a39 separate_adj_matrix + 0
+0000000000004088  0000002000000007 R_X86_64_JUMP_SLOT     0000000000001a4b separate_adj_matrix + 0
 0000000000004090  0000000f00000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_eigen_symmv_free + 0
-0000000000004098  0000002000000007 R_X86_64_JUMP_SLOT     0000000000001766 free_2d_array + 0
-00000000000040a0  0000001600000007 R_X86_64_JUMP_SLOT     00000000000019a7 create_adj_matrix + 0
+0000000000004098  0000002100000007 R_X86_64_JUMP_SLOT     0000000000001766 free_2d_array + 0
+00000000000040a0  0000001700000007 R_X86_64_JUMP_SLOT     00000000000019b9 create_adj_matrix + 0
 00000000000040a8  0000001000000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_matrix_free + 0
 00000000000040b0  0000001100000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_matrix_view_array + 0
 00000000000040b8  0000001200000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_vector_free + 0
 00000000000040c0  0000001300000007 R_X86_64_JUMP_SLOT     0000000000000000 __stack_chk_fail@GLIBC_2.4 + 0
-00000000000040c8  0000001700000007 R_X86_64_JUMP_SLOT     0000000000001aa4 final_community_assignment + 0
+00000000000040c8  0000001800000007 R_X86_64_JUMP_SLOT     0000000000001ab6 final_community_assignment + 0
 00000000000040d0  0000001400000007 R_X86_64_JUMP_SLOT     0000000000000000 gsl_matrix_column + 0
-00000000000040d8  0000001b00000007 R_X86_64_JUMP_SLOT     0000000000001acc divide_community + 0
-00000000000040e0  0000001800000007 R_X86_64_JUMP_SLOT     0000000000001459 getModularityMatrix + 0
+00000000000040d8  0000001b00000007 R_X86_64_JUMP_SLOT     0000000000001ade divide_community + 0
+00000000000040e0  0000001900000007 R_X86_64_JUMP_SLOT     0000000000001459 getModularityMatrix + 0
 00000000000040e8  0000001c00000007 R_X86_64_JUMP_SLOT     00000000000015b6 create_1d_array + 0
```

#### readelf --wide --dynamic {}

```diff
@@ -1,28 +1,28 @@
 
 Dynamic section at offset 0x2e10 contains 25 entries:
   Tag        Type                         Name/Value
  0x0000000000000001 (NEEDED)             Shared library: [libgsl.so.27]
  0x0000000000000001 (NEEDED)             Shared library: [libc.so.6]
  0x000000000000000c (INIT)               0x1000
- 0x000000000000000d (FINI)               0x1e24
+ 0x000000000000000d (FINI)               0x1e40
  0x0000000000000019 (INIT_ARRAY)         0x3e00
  0x000000000000001b (INIT_ARRAYSZ)       8 (bytes)
  0x000000000000001a (FINI_ARRAY)         0x3e08
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x2f0
- 0x0000000000000005 (STRTAB)             0x680
- 0x0000000000000006 (SYMTAB)             0x350
- 0x000000000000000a (STRSZ)              618 (bytes)
+ 0x0000000000000005 (STRTAB)             0x6a0
+ 0x0000000000000006 (SYMTAB)             0x358
+ 0x000000000000000a (STRSZ)              643 (bytes)
  0x000000000000000b (SYMENT)             24 (bytes)
  0x0000000000000003 (PLTGOT)             0x4000
  0x0000000000000002 (PLTRELSZ)           648 (bytes)
  0x0000000000000014 (PLTREL)             RELA
- 0x0000000000000017 (JMPREL)             0xa18
- 0x0000000000000007 (RELA)               0x970
+ 0x0000000000000017 (JMPREL)             0xa58
+ 0x0000000000000007 (RELA)               0x9b0
  0x0000000000000008 (RELASZ)             168 (bytes)
  0x0000000000000009 (RELAENT)            24 (bytes)
- 0x000000006ffffffe (VERNEED)            0x930
+ 0x000000006ffffffe (VERNEED)            0x970
  0x000000006fffffff (VERNEEDNUM)         1
- 0x000000006ffffff0 (VERSYM)             0x8ea
+ 0x000000006ffffff0 (VERSYM)             0x924
  0x000000006ffffff9 (RELACOUNT)          3
  0x0000000000000000 (NULL)               0x0
```

#### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 35efb6cd1413500676f713c5d7cf3a7cf99a2f6c
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: ef20d6395907f869f04d1c7ca5de280d7c0830df
```

#### readelf --wide --version-info {}

```diff
@@ -1,19 +1,19 @@
 
-Version symbols section '.gnu.version' contains 34 entries:
- Addr: 0x00000000000008ea  Offset: 0x000008ea  Link: 4 (.dynsym)
+Version symbols section '.gnu.version' contains 35 entries:
+ Addr: 0x0000000000000924  Offset: 0x00000924  Link: 4 (.dynsym)
   000:   0 (*local*)       1 (*global*)      1 (*global*)      2 (GLIBC_2.2.5)
   004:   3 (GLIBC_2.3.4)   1 (*global*)      2 (GLIBC_2.2.5)   1 (*global*)   
   008:   1 (*global*)      1 (*global*)      2 (GLIBC_2.2.5)   1 (*global*)   
   00c:   1 (*global*)      2 (GLIBC_2.2.5)   1 (*global*)      1 (*global*)   
   010:   1 (*global*)      1 (*global*)      1 (*global*)      4 (GLIBC_2.4)  
   014:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   018:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   01c:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
-  020:   1 (*global*)      1 (*global*)   
+  020:   1 (*global*)      1 (*global*)      1 (*global*)   
 
 Version needs section '.gnu.version_r' contains 1 entry:
- Addr: 0x0000000000000930  Offset: 0x00000930  Link: 5 (.dynstr)
+ Addr: 0x0000000000000970  Offset: 0x00000970  Link: 5 (.dynstr)
   000000: Version: 1  File: libc.so.6  Cnt: 3
   0x0010:   Name: GLIBC_2.4  Flags: none  Version: 4
   0x0020:   Name: GLIBC_2.3.4  Flags: none  Version: 3
   0x0030:   Name: GLIBC_2.2.5  Flags: none  Version: 2
```

#### readelf --wide --debug-dump=frames {}

```diff
@@ -154,15 +154,15 @@
   DW_CFA_def_cfa_offset: 16
   DW_CFA_advance_loc: 2 to 000000000000172a
   DW_CFA_def_cfa_offset: 8
   DW_CFA_advance_loc: 1 to 000000000000172b
   DW_CFA_restore_state
   DW_CFA_nop
 
-00000170 000000000000002c 00000174 FDE cie=00000000 pc=0000000000001766..000000000000179e
+00000170 0000000000000028 00000174 FDE cie=00000000 pc=0000000000001766..000000000000179e
   DW_CFA_advance_loc: 6 to 000000000000176c
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r12 (r12) at cfa-16
   DW_CFA_advance_loc: 1 to 000000000000176d
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r6 (rbp) at cfa-24
   DW_CFA_advance_loc: 1 to 000000000000176e
@@ -173,182 +173,184 @@
   DW_CFA_advance_loc: 1 to 000000000000179b
   DW_CFA_def_cfa_offset: 16
   DW_CFA_advance_loc: 2 to 000000000000179d
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
+
+0000019c 0000000000000018 000001a0 FDE cie=00000000 pc=000000000000179e..00000000000017b0
+  DW_CFA_advance_loc: 8 to 00000000000017a6
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 9 to 00000000000017af
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000001a0 000000000000004c 000001a4 FDE cie=00000000 pc=000000000000179e..00000000000019a7
-  DW_CFA_advance_loc: 6 to 00000000000017a4
+000001b8 000000000000004c 000001bc FDE cie=00000000 pc=00000000000017b0..00000000000019b9
+  DW_CFA_advance_loc: 6 to 00000000000017b6
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 00000000000017a6
+  DW_CFA_advance_loc: 2 to 00000000000017b8
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 00000000000017a8
+  DW_CFA_advance_loc: 2 to 00000000000017ba
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 00000000000017aa
+  DW_CFA_advance_loc: 2 to 00000000000017bc
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 00000000000017ab
+  DW_CFA_advance_loc: 1 to 00000000000017bd
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 00000000000017ac
+  DW_CFA_advance_loc: 1 to 00000000000017be
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 00000000000017b3
+  DW_CFA_advance_loc: 7 to 00000000000017c5
   DW_CFA_def_cfa_offset: 192
-  DW_CFA_advance_loc2: 349 to 0000000000001910
+  DW_CFA_advance_loc2: 349 to 0000000000001922
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000001911
+  DW_CFA_advance_loc: 1 to 0000000000001923
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000001912
+  DW_CFA_advance_loc: 1 to 0000000000001924
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000001914
+  DW_CFA_advance_loc: 2 to 0000000000001926
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000001916
+  DW_CFA_advance_loc: 2 to 0000000000001928
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000001918
+  DW_CFA_advance_loc: 2 to 000000000000192a
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000191a
+  DW_CFA_advance_loc: 2 to 000000000000192c
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000000000000191b
+  DW_CFA_advance_loc: 1 to 000000000000192d
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000001f0 0000000000000028 000001f4 FDE cie=00000000 pc=00000000000019a7..0000000000001a39
-  DW_CFA_advance_loc: 6 to 00000000000019ad
+00000208 0000000000000028 0000020c FDE cie=00000000 pc=00000000000019b9..0000000000001a4b
+  DW_CFA_advance_loc: 6 to 00000000000019bf
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r12 (r12) at cfa-16
-  DW_CFA_advance_loc: 1 to 00000000000019ae
+  DW_CFA_advance_loc: 1 to 00000000000019c0
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r6 (rbp) at cfa-24
-  DW_CFA_advance_loc: 1 to 00000000000019af
+  DW_CFA_advance_loc: 1 to 00000000000019c1
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r3 (rbx) at cfa-32
-  DW_CFA_advance_loc1: 134 to 0000000000001a35
+  DW_CFA_advance_loc1: 134 to 0000000000001a47
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 1 to 0000000000001a36
+  DW_CFA_advance_loc: 1 to 0000000000001a48
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000001a38
+  DW_CFA_advance_loc: 2 to 0000000000001a4a
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
 
-0000021c 0000000000000028 00000220 FDE cie=00000000 pc=0000000000001a39..0000000000001aa4
-  DW_CFA_advance_loc: 6 to 0000000000001a3f
+00000234 0000000000000028 00000238 FDE cie=00000000 pc=0000000000001a4b..0000000000001ab6
+  DW_CFA_advance_loc: 6 to 0000000000001a51
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r12 (r12) at cfa-16
-  DW_CFA_advance_loc: 1 to 0000000000001a40
+  DW_CFA_advance_loc: 1 to 0000000000001a52
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r6 (rbp) at cfa-24
-  DW_CFA_advance_loc: 1 to 0000000000001a41
+  DW_CFA_advance_loc: 1 to 0000000000001a53
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r3 (rbx) at cfa-32
-  DW_CFA_advance_loc1: 95 to 0000000000001aa0
+  DW_CFA_advance_loc1: 95 to 0000000000001ab2
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 1 to 0000000000001aa1
+  DW_CFA_advance_loc: 1 to 0000000000001ab3
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000001aa3
+  DW_CFA_advance_loc: 2 to 0000000000001ab5
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000248 0000000000000010 0000024c FDE cie=00000000 pc=0000000000001aa4..0000000000001acc
+00000260 0000000000000010 00000264 FDE cie=00000000 pc=0000000000001ab6..0000000000001ade
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000025c 000000000000004c 00000260 FDE cie=00000000 pc=0000000000001acc..0000000000001d5f
-  DW_CFA_advance_loc: 6 to 0000000000001ad2
+00000274 000000000000004c 00000278 FDE cie=00000000 pc=0000000000001ade..0000000000001d71
+  DW_CFA_advance_loc: 6 to 0000000000001ae4
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000001ad4
+  DW_CFA_advance_loc: 2 to 0000000000001ae6
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 0000000000001ad6
+  DW_CFA_advance_loc: 2 to 0000000000001ae8
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 0000000000001ad8
+  DW_CFA_advance_loc: 2 to 0000000000001aea
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000001ad9
+  DW_CFA_advance_loc: 1 to 0000000000001aeb
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 0000000000001ada
+  DW_CFA_advance_loc: 1 to 0000000000001aec
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 4 to 0000000000001ade
+  DW_CFA_advance_loc: 4 to 0000000000001af0
   DW_CFA_def_cfa_offset: 144
-  DW_CFA_advance_loc2: 509 to 0000000000001cdb
+  DW_CFA_advance_loc2: 509 to 0000000000001ced
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000001cdc
+  DW_CFA_advance_loc: 1 to 0000000000001cee
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000001cdd
+  DW_CFA_advance_loc: 1 to 0000000000001cef
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000001cdf
+  DW_CFA_advance_loc: 2 to 0000000000001cf1
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000001ce1
+  DW_CFA_advance_loc: 2 to 0000000000001cf3
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000001ce3
+  DW_CFA_advance_loc: 2 to 0000000000001cf5
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000001ce5
+  DW_CFA_advance_loc: 2 to 0000000000001cf7
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000001ce6
+  DW_CFA_advance_loc: 1 to 0000000000001cf8
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000002ac 0000000000000048 000002b0 FDE cie=00000000 pc=0000000000001d5f..0000000000001e22
-  DW_CFA_advance_loc: 6 to 0000000000001d65
+000002c4 0000000000000040 000002c8 FDE cie=00000000 pc=0000000000001d71..0000000000001e3d
+  DW_CFA_advance_loc: 6 to 0000000000001d77
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000001d67
+  DW_CFA_offset: r14 (r14) at cfa-16
+  DW_CFA_advance_loc: 2 to 0000000000001d79
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 0000000000001d69
+  DW_CFA_offset: r13 (r13) at cfa-24
+  DW_CFA_advance_loc: 2 to 0000000000001d7b
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 0000000000001d6b
+  DW_CFA_offset: r12 (r12) at cfa-32
+  DW_CFA_advance_loc: 1 to 0000000000001d7c
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000001d6c
+  DW_CFA_offset: r6 (rbp) at cfa-40
+  DW_CFA_advance_loc: 1 to 0000000000001d7d
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 0000000000001d6d
-  DW_CFA_def_cfa_offset: 56
-  DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 4 to 0000000000001d71
-  DW_CFA_def_cfa_offset: 80
-  DW_CFA_advance_loc1: 161 to 0000000000001e12
+  DW_CFA_offset: r3 (rbx) at cfa-48
+  DW_CFA_advance_loc: 4 to 0000000000001d81
+  DW_CFA_def_cfa_offset: 64
+  DW_CFA_advance_loc1: 174 to 0000000000001e2f
   DW_CFA_remember_state
-  DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000001e13
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000001e14
+  DW_CFA_advance_loc: 1 to 0000000000001e30
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000001e16
+  DW_CFA_advance_loc: 1 to 0000000000001e31
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000001e18
+  DW_CFA_advance_loc: 2 to 0000000000001e33
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000001e1a
+  DW_CFA_advance_loc: 2 to 0000000000001e35
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000001e1c
+  DW_CFA_advance_loc: 2 to 0000000000001e37
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000001e1d
+  DW_CFA_advance_loc: 1 to 0000000000001e38
   DW_CFA_restore_state
   DW_CFA_nop
 
-000002f8 ZERO terminator
+00000308 ZERO terminator
```

#### strings --all --bytes=8 {}

```diff
@@ -6,14 +6,15 @@
 create_1d_array
 create_2d_array
 modularityScore
 __printf_chk
 create_1d_array_int
 create_2d_array_int
 free_2d_array
+free_1d_array
 getEigenVector
 gsl_matrix_view_array
 gsl_vector_alloc
 gsl_matrix_alloc
 gsl_eigen_symmv_alloc
 gsl_eigen_symmv
 gsl_eigen_symmv_free
@@ -23,26 +24,26 @@
 gsl_vector_free
 gsl_matrix_free
 __stack_chk_fail
 create_adj_matrix
 separate_adj_matrix
 final_community_assignment
 divide_community
-get_community
+get_community_assignment
 libgsl.so.27
 libc.so.6
 GLIBC_2.4
 GLIBC_2.3.4
 GLIBC_2.2.5
 AWAVAUATUSH
 []A\A]A^A_
 AWAVAUATUSH
 X[]A\A]A^A_
-AWAVAUATUSH
-[]A\A]A^A_
+AVAUATUSH
+[]A\A]A^
 Error: Memory allocation failed.
 Error: Failed to allocate memory for 2D array.
 GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
 completed.0
@@ -56,35 +57,36 @@
 __FRAME_END__
 __GNU_EH_FRAME_HDR
 _GLOBAL_OFFSET_TABLE_
 __TMC_END__
 __dso_handle
 _DYNAMIC
 gsl_eigen_symmv_alloc
-get_community
 __gmon_start__
 exit@GLIBC_2.2.5
 __printf_chk@GLIBC_2.3.4
 gsl_matrix_alloc
 getEigenVector
 malloc@GLIBC_2.2.5
 create_2d_array
 modularityScore
 _ITM_deregisterTMCloneTable
 create_1d_array_int
 gsl_eigen_symmv_sort
 gsl_eigen_symmv
+get_community_assignment
 free@GLIBC_2.2.5
 _ITM_registerTMCloneTable
 gsl_vector_alloc
 __cxa_finalize@GLIBC_2.2.5
 gsl_vector_get
 separate_adj_matrix
 gsl_eigen_symmv_free
 free_2d_array
+free_1d_array
 create_2d_array_int
 create_adj_matrix
 gsl_matrix_free
 gsl_matrix_view_array
 gsl_vector_free
 __stack_chk_fail@GLIBC_2.4
 final_community_assignment
```

#### readelf --wide --decompress --hex-dump=.gnu.hash {}

```diff
@@ -1,9 +1,10 @@
 
 Hex dump of section '.gnu.hash':
   0x000002f0 03000000 15000000 02000000 07000000 ................
-  0x00000300 00404030 84002008 d3180254 000a5000 .@@0.. ....T..P.
-  0x00000310 15000000 19000000 1d000000 4ce3bf58 ............L..X
-  0x00000320 3a2743c6 ca687799 c500c2a5 687a26e4 :'C..hw.....hz&.
+  0x00000300 00404030 84002008 d3180254 82084202 .@@0.. ....T..B.
+  0x00000310 15000000 1a000000 1d000000 4ce3bf58 ............L..X
+  0x00000320 f8b33478 3a2743c6 ca687799 c500c2a5 ..4x:'C..hw.....
   0x00000330 34319b80 5e1bfcde 6b0e7e6c 40c0dcf3 41..^...k.~l@...
-  0x00000340 ea4303c3 9c939ad3 da887664 978e8eb1 .C........vd....
+  0x00000340 ea4303c3 e0788354 9c939ad3 da887664 .C...x.T......vd
+  0x00000350 978e8eb1                            ....
```

#### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -1,42 +1,44 @@
 
 Hex dump of section '.dynstr':
-  0x00000680 005f5f67 6d6f6e5f 73746172 745f5f00 .__gmon_start__.
-  0x00000690 5f49544d 5f646572 65676973 74657254 _ITM_deregisterT
-  0x000006a0 4d436c6f 6e655461 626c6500 5f49544d MCloneTable._ITM
-  0x000006b0 5f726567 69737465 72544d43 6c6f6e65 _registerTMClone
-  0x000006c0 5461626c 65005f5f 6378615f 66696e61 Table.__cxa_fina
-  0x000006d0 6c697a65 00676574 4d6f6475 6c617269 lize.getModulari
-  0x000006e0 74794d61 74726978 00637265 6174655f tyMatrix.create_
-  0x000006f0 31645f61 72726179 00637265 6174655f 1d_array.create_
-  0x00000700 32645f61 72726179 006d6f64 756c6172 2d_array.modular
-  0x00000710 69747953 636f7265 006d616c 6c6f6300 ityScore.malloc.
-  0x00000720 5f5f7072 696e7466 5f63686b 00657869 __printf_chk.exi
-  0x00000730 74006372 65617465 5f31645f 61727261 t.create_1d_arra
-  0x00000740 795f696e 74006372 65617465 5f32645f y_int.create_2d_
-  0x00000750 61727261 795f696e 74006672 65655f32 array_int.free_2
-  0x00000760 645f6172 72617900 67657445 6967656e d_array.getEigen
-  0x00000770 56656374 6f720067 736c5f6d 61747269 Vector.gsl_matri
-  0x00000780 785f7669 65775f61 72726179 0067736c x_view_array.gsl
-  0x00000790 5f766563 746f725f 616c6c6f 63006773 _vector_alloc.gs
-  0x000007a0 6c5f6d61 74726978 5f616c6c 6f630067 l_matrix_alloc.g
-  0x000007b0 736c5f65 6967656e 5f73796d 6d765f61 sl_eigen_symmv_a
-  0x000007c0 6c6c6f63 0067736c 5f656967 656e5f73 lloc.gsl_eigen_s
-  0x000007d0 796d6d76 0067736c 5f656967 656e5f73 ymmv.gsl_eigen_s
-  0x000007e0 796d6d76 5f667265 65006773 6c5f6569 ymmv_free.gsl_ei
-  0x000007f0 67656e5f 73796d6d 765f736f 72740067 gen_symmv_sort.g
-  0x00000800 736c5f6d 61747269 785f636f 6c756d6e sl_matrix_column
-  0x00000810 0067736c 5f766563 746f725f 67657400 .gsl_vector_get.
-  0x00000820 67736c5f 76656374 6f725f66 72656500 gsl_vector_free.
-  0x00000830 67736c5f 6d617472 69785f66 72656500 gsl_matrix_free.
-  0x00000840 5f5f7374 61636b5f 63686b5f 6661696c __stack_chk_fail
-  0x00000850 00637265 6174655f 61646a5f 6d617472 .create_adj_matr
-  0x00000860 69780073 65706172 6174655f 61646a5f ix.separate_adj_
-  0x00000870 6d617472 69780066 696e616c 5f636f6d matrix.final_com
-  0x00000880 6d756e69 74795f61 73736967 6e6d656e munity_assignmen
-  0x00000890 74006469 76696465 5f636f6d 6d756e69 t.divide_communi
-  0x000008a0 74790067 65745f63 6f6d6d75 6e697479 ty.get_community
-  0x000008b0 006c6962 67736c2e 736f2e32 37006c69 .libgsl.so.27.li
-  0x000008c0 62632e73 6f2e3600 474c4942 435f322e bc.so.6.GLIBC_2.
-  0x000008d0 3400474c 4942435f 322e332e 3400474c 4.GLIBC_2.3.4.GL
-  0x000008e0 4942435f 322e322e 3500              IBC_2.2.5.
+  0x000006a0 005f5f67 6d6f6e5f 73746172 745f5f00 .__gmon_start__.
+  0x000006b0 5f49544d 5f646572 65676973 74657254 _ITM_deregisterT
+  0x000006c0 4d436c6f 6e655461 626c6500 5f49544d MCloneTable._ITM
+  0x000006d0 5f726567 69737465 72544d43 6c6f6e65 _registerTMClone
+  0x000006e0 5461626c 65005f5f 6378615f 66696e61 Table.__cxa_fina
+  0x000006f0 6c697a65 00676574 4d6f6475 6c617269 lize.getModulari
+  0x00000700 74794d61 74726978 00637265 6174655f tyMatrix.create_
+  0x00000710 31645f61 72726179 00637265 6174655f 1d_array.create_
+  0x00000720 32645f61 72726179 006d6f64 756c6172 2d_array.modular
+  0x00000730 69747953 636f7265 006d616c 6c6f6300 ityScore.malloc.
+  0x00000740 5f5f7072 696e7466 5f63686b 00657869 __printf_chk.exi
+  0x00000750 74006372 65617465 5f31645f 61727261 t.create_1d_arra
+  0x00000760 795f696e 74006372 65617465 5f32645f y_int.create_2d_
+  0x00000770 61727261 795f696e 74006672 65655f32 array_int.free_2
+  0x00000780 645f6172 72617900 66726565 5f31645f d_array.free_1d_
+  0x00000790 61727261 79006765 74456967 656e5665 array.getEigenVe
+  0x000007a0 63746f72 0067736c 5f6d6174 7269785f ctor.gsl_matrix_
+  0x000007b0 76696577 5f617272 61790067 736c5f76 view_array.gsl_v
+  0x000007c0 6563746f 725f616c 6c6f6300 67736c5f ector_alloc.gsl_
+  0x000007d0 6d617472 69785f61 6c6c6f63 0067736c matrix_alloc.gsl
+  0x000007e0 5f656967 656e5f73 796d6d76 5f616c6c _eigen_symmv_all
+  0x000007f0 6f630067 736c5f65 6967656e 5f73796d oc.gsl_eigen_sym
+  0x00000800 6d760067 736c5f65 6967656e 5f73796d mv.gsl_eigen_sym
+  0x00000810 6d765f66 72656500 67736c5f 65696765 mv_free.gsl_eige
+  0x00000820 6e5f7379 6d6d765f 736f7274 0067736c n_symmv_sort.gsl
+  0x00000830 5f6d6174 7269785f 636f6c75 6d6e0067 _matrix_column.g
+  0x00000840 736c5f76 6563746f 725f6765 74006773 sl_vector_get.gs
+  0x00000850 6c5f7665 63746f72 5f667265 65006773 l_vector_free.gs
+  0x00000860 6c5f6d61 74726978 5f667265 65005f5f l_matrix_free.__
+  0x00000870 73746163 6b5f6368 6b5f6661 696c0063 stack_chk_fail.c
+  0x00000880 72656174 655f6164 6a5f6d61 74726978 reate_adj_matrix
+  0x00000890 00736570 61726174 655f6164 6a5f6d61 .separate_adj_ma
+  0x000008a0 74726978 0066696e 616c5f63 6f6d6d75 trix.final_commu
+  0x000008b0 6e697479 5f617373 69676e6d 656e7400 nity_assignment.
+  0x000008c0 64697669 64655f63 6f6d6d75 6e697479 divide_community
+  0x000008d0 00676574 5f636f6d 6d756e69 74795f61 .get_community_a
+  0x000008e0 73736967 6e6d656e 74006c69 6267736c ssignment.libgsl
+  0x000008f0 2e736f2e 3237006c 6962632e 736f2e36 .so.27.libc.so.6
+  0x00000900 00474c49 42435f32 2e340047 4c494243 .GLIBC_2.4.GLIBC
+  0x00000910 5f322e33 2e340047 4c494243 5f322e32 _2.3.4.GLIBC_2.2
+  0x00000920 2e3500                              .5.
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -322,15 +322,23 @@
 	mov    %r12,%rdi
 	call   12a0 <free@plt>
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	ret
 
-000000000000179e <getEigenVector>:
+000000000000179e <free_1d_array>:
+free_1d_array():
+	endbr64
+	sub    $0x8,%rsp
+	call   12a0 <free@plt>
+	add    $0x8,%rsp
+	ret
+
+00000000000017b0 <getEigenVector>:
 getEigenVector():
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
@@ -342,34 +350,34 @@
 	mov    %rax,0x78(%rsp)
 	xor    %eax,%eax
 	mov    %esi,%edi
 	imul   %esi,%edi
 	call   1390 <create_1d_array@plt>
 	mov    %rax,%r15
 	test   %ebp,%ebp
-	jle    191b <getEigenVector+0x17d>
+	jle    192d <getEigenVector+0x17d>
 	mov    %rbx,%rcx
 	movslq %ebp,%r12
 	lea    0x0(,%r12,8),%r9
 	mov    %rax,%rsi
 	lea    -0x1(%rbp),%eax
 	lea    0x8(%rbx,%rax,8),%r8
 	mov    %ebp,%ebx
 	lea    0x0(,%rbx,8),%rdi
 	mov    $0x0,%eax
 	mov    (%rcx),%rdx
 	movsd  (%rdx,%rax,1),%xmm0
 	movsd  %xmm0,(%rsi,%rax,1)
 	add    $0x8,%rax
 	cmp    %rax,%rdi
-	jne    1805 <getEigenVector+0x67>
+	jne    1817 <getEigenVector+0x67>
 	add    $0x8,%rcx
 	add    %r9,%rsi
 	cmp    %r8,%rcx
-	jne    1800 <getEigenVector+0x62>
+	jne    1812 <getEigenVector+0x62>
 	lea    0x40(%rsp),%rax
 	mov    %r12,%rcx
 	mov    %r12,%rdx
 	mov    %r15,%rsi
 	mov    %rax,0x8(%rsp)
 	mov    %rax,%rdi
 	call   1320 <gsl_matrix_view_array@plt>
@@ -408,24 +416,24 @@
 	pxor   %xmm1,%xmm1
 	comisd %xmm1,%xmm0
 	setae  %al
 	movzbl %al,%eax
 	mov    %eax,(%r12,%rbp,4)
 	add    $0x1,%rbp
 	cmp    %rbp,%rbx
-	jne    18b2 <getEigenVector+0x114>
+	jne    18c4 <getEigenVector+0x114>
 	mov    %r14,%rdi
 	call   1330 <gsl_vector_free@plt>
 	mov    %r13,%rdi
 	call   1310 <gsl_matrix_free@plt>
 	mov    %r15,%rdi
 	call   12a0 <free@plt>
 	mov    0x78(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    19a2 <getEigenVector+0x204>
+	jne    19b4 <getEigenVector+0x204>
 	mov    %r12,%rax
 	add    $0x88,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
@@ -462,122 +470,122 @@
 	lea    0x10(%rsp),%rdi
 	mov    $0x1,%edx
 	mov    %r13,%rsi
 	call   1360 <gsl_matrix_column@plt>
 	mov    %ebp,%edi
 	call   1270 <create_1d_array_int@plt>
 	mov    %rax,%r12
-	jmp    18da <getEigenVector+0x13c>
+	jmp    18ec <getEigenVector+0x13c>
 	call   1340 <__stack_chk_fail@plt>
 
-00000000000019a7 <create_adj_matrix>:
+00000000000019b9 <create_adj_matrix>:
 create_adj_matrix():
 	endbr64
 	push   %r12
 	push   %rbp
 	push   %rbx
 	mov    %rdi,%rbp
 	mov    %esi,%ebx
 	mov    %edx,%r12d
 	mov    %edx,%esi
 	mov    %edx,%edi
 	call   1250 <create_2d_array@plt>
 	mov    %rax,%rdi
 	test   %r12d,%r12d
-	jle    19f8 <create_adj_matrix+0x51>
+	jle    1a0a <create_adj_matrix+0x51>
 	mov    %rax,%rcx
 	mov    %r12d,%esi
 	shl    $0x3,%rsi
 	lea    (%rsi,%rax,1),%r8
 	mov    $0x0,%eax
 	mov    (%rcx),%rdx
 	movq   $0x0,(%rdx,%rax,1)
 	add    $0x8,%rax
 	cmp    %rsi,%rax
-	jne    19db <create_adj_matrix+0x34>
+	jne    19ed <create_adj_matrix+0x34>
 	add    $0x8,%rcx
 	cmp    %r8,%rcx
-	jne    19d6 <create_adj_matrix+0x2f>
+	jne    19e8 <create_adj_matrix+0x2f>
 	test   %ebx,%ebx
-	jle    1a31 <create_adj_matrix+0x8a>
+	jle    1a43 <create_adj_matrix+0x8a>
 	mov    %rbp,%rax
 	lea    -0x1(%rbx),%edx
 	lea    0x8(%rbp,%rdx,8),%r8
-	movsd  0x651(%rip),%xmm0        
+	movsd  0x63f(%rip),%xmm0        
 	movslq (%rax),%rdx
 	movslq 0x4(%rax),%rcx
 	mov    (%rdi,%rdx,8),%rsi
 	movsd  %xmm0,(%rsi,%rcx,8)
 	mov    (%rdi,%rcx,8),%rcx
 	movsd  %xmm0,(%rcx,%rdx,8)
 	add    $0x8,%rax
 	cmp    %rax,%r8
-	jne    1a0f <create_adj_matrix+0x68>
+	jne    1a21 <create_adj_matrix+0x68>
 	mov    %rdi,%rax
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	ret
 
-0000000000001a39 <separate_adj_matrix>:
+0000000000001a4b <separate_adj_matrix>:
 separate_adj_matrix():
 	endbr64
 	push   %r12
 	push   %rbp
 	push   %rbx
 	mov    %rdi,%rbp
 	mov    %rsi,%rbx
 	mov    %edx,%r12d
 	mov    %edx,%esi
 	mov    %edx,%edi
 	call   1250 <create_2d_array@plt>
 	test   %r12d,%r12d
-	jle    1a9f <separate_adj_matrix+0x66>
+	jle    1ab1 <separate_adj_matrix+0x66>
 	mov    %rbx,%rdi
 	mov    %rax,%r8
 	lea    -0x1(%r12),%edx
 	lea    0x4(%rbx,%rdx,4),%r10
 	mov    %r12d,%r9d
 	mov    $0x0,%edx
 	movslq (%rdi),%rcx
 	movslq (%rbx,%rdx,4),%rsi
 	mov    0x0(%rbp,%rcx,8),%rcx
 	movsd  (%rcx,%rsi,8),%xmm0
 	mov    (%r8),%rcx
 	movsd  %xmm0,(%rcx,%rdx,8)
 	add    $0x1,%rdx
 	cmp    %rdx,%r9
-	jne    1a70 <separate_adj_matrix+0x37>
+	jne    1a82 <separate_adj_matrix+0x37>
 	add    $0x4,%rdi
 	add    $0x8,%r8
 	cmp    %r10,%rdi
-	jne    1a6b <separate_adj_matrix+0x32>
+	jne    1a7d <separate_adj_matrix+0x32>
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	ret
 
-0000000000001aa4 <final_community_assignment>:
+0000000000001ab6 <final_community_assignment>:
 final_community_assignment():
 	endbr64
 	test   %esi,%esi
-	jle    1ac8 <final_community_assignment+0x24>
+	jle    1ada <final_community_assignment+0x24>
 	mov    %rdi,%rax
 	lea    -0x1(%rsi),%esi
 	lea    0x4(%rdi,%rsi,4),%r8
 	mov    (%rcx),%edi
 	movslq (%rax),%rsi
 	mov    %edi,(%rdx,%rsi,4)
 	add    $0x4,%rax
 	cmp    %r8,%rax
-	jne    1ab7 <final_community_assignment+0x13>
+	jne    1ac9 <final_community_assignment+0x13>
 	addl   $0x1,(%rcx)
 	ret
 
-0000000000001acc <divide_community>:
+0000000000001ade <divide_community>:
 divide_community.localalias():
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
@@ -587,44 +595,44 @@
 	mov    %esi,0xc(%rsp)
 	mov    %rdx,%rbx
 	mov    %rcx,0x38(%rsp)
 	mov    %r8,0x30(%rsp)
 	mov    %r9,0x10(%rsp)
 	movsd  %xmm0,0x40(%rsp)
 	cmp    $0x2,%esi
-	jle    1b2c <divide_community+0x60>
+	jle    1b3e <divide_community+0x60>
 	mov    0xc(%rsp),%r14d
 	mov    %r14d,%esi
 	mov    (%rsp),%rdi
 	call   1230 <getEigenVector@plt>
 	mov    %rax,%rbp
 	mov    %r14d,%edx
 	lea    (%rax,%rdx,4),%rdx
 	mov    $0x0,%r12d
 	mov    $0x0,%r13d
-	jmp    1b63 <divide_community+0x97>
+	jmp    1b75 <divide_community+0x97>
 	mov    %r8,%rcx
 	mov    %r9,%rdx
 	mov    %esi,%r15d
 	mov    %rbx,%rdi
 	call   1350 <final_community_assignment@plt>
 	mov    %r15d,%esi
 	mov    (%rsp),%rdi
 	call   12f0 <free_2d_array@plt>
 	mov    %rbx,%rdi
 	call   12a0 <free@plt>
-	jmp    1cd7 <divide_community+0x20b>
+	jmp    1ce9 <divide_community+0x20b>
 	add    $0x1,%r12d
 	add    $0x4,%rax
 	cmp    %rdx,%rax
-	je     1b6e <divide_community+0xa2>
+	je     1b80 <divide_community+0xa2>
 	cmpl   $0x0,(%rax)
-	jne    1b56 <divide_community+0x8a>
+	jne    1b68 <divide_community+0x8a>
 	add    $0x1,%r13d
-	jmp    1b5a <divide_community+0x8e>
+	jmp    1b6c <divide_community+0x8e>
 	mov    %r13d,%edi
 	call   1270 <create_1d_array_int@plt>
 	mov    %rax,0x20(%rsp)
 	mov    %r13d,%edi
 	call   1270 <create_1d_array_int@plt>
 	mov    %rax,%r15
 	mov    %r12d,%edi
@@ -635,45 +643,45 @@
 	mov    %rax,%r14
 	mov    0xc(%rsp),%edi
 	mov    $0x0,%eax
 	mov    $0x0,%ecx
 	mov    $0x0,%edx
 	mov    0x20(%rsp),%r9
 	mov    0x28(%rsp),%r10
-	jmp    1bd8 <divide_community+0x10c>
+	jmp    1bea <divide_community+0x10c>
 	movslq %ecx,%rsi
 	mov    (%rbx,%rax,4),%r8d
 	mov    %r8d,(%r10,%rsi,4)
 	mov    %eax,(%r14,%rsi,4)
 	add    $0x1,%ecx
 	add    $0x1,%rax
 	cmp    %rdi,%rax
-	je     1bf3 <divide_community+0x127>
+	je     1c05 <divide_community+0x127>
 	cmpl   $0x0,0x0(%rbp,%rax,4)
-	jne    1bbd <divide_community+0xf1>
+	jne    1bcf <divide_community+0xf1>
 	movslq %edx,%rsi
 	mov    (%rbx,%rax,4),%r8d
 	mov    %r8d,(%r9,%rsi,4)
 	mov    %eax,(%r15,%rsi,4)
 	add    $0x1,%edx
-	jmp    1bcf <divide_community+0x103>
+	jmp    1be1 <divide_community+0x103>
 	mov    %rbp,%rdi
 	call   12a0 <free@plt>
 	pxor   %xmm1,%xmm1
 	movsd  %xmm1,0x18(%rsp)
 	cmp    $0x1,%r13d
-	jg     1ce6 <divide_community+0x21a>
-	mov    0x442(%rip),%rbp        
+	jg     1cf8 <divide_community+0x21a>
+	mov    0x430(%rip),%rbp        
 	cmp    $0x1,%r12d
-	jg     1d03 <divide_community+0x237>
+	jg     1d15 <divide_community+0x237>
 	movq   %rbp,%xmm0
 	addsd  0x18(%rsp),%xmm0
 	movsd  0x40(%rsp),%xmm3
 	comisd %xmm0,%xmm3
-	jae    1d1f <divide_community+0x253>
+	jae    1d31 <divide_community+0x253>
 	mov    %r13d,%edx
 	mov    %r15,%rsi
 	mov    (%rsp),%rdi
 	call   12d0 <separate_adj_matrix@plt>
 	mov    %rax,0x40(%rsp)
 	mov    %r12d,%edx
 	mov    %r14,%rsi
@@ -689,23 +697,23 @@
 	mov    0x30(%rsp),%r14
 	mov    %r14,%r8
 	mov    0x38(%rsp),%r15
 	mov    %r15,%rcx
 	mov    0x20(%rsp),%rdx
 	mov    %r13d,%esi
 	mov    0x40(%rsp),%rdi
-	call   1acc <divide_community>
+	call   1ade <divide_community>
 	movq   %rbp,%xmm0
 	mov    0x10(%rsp),%r9
 	mov    %r14,%r8
 	mov    %r15,%rcx
 	mov    0x28(%rsp),%rdx
 	mov    %r12d,%esi
 	mov    0x48(%rsp),%rdi
-	call   1acc <divide_community>
+	call   1ade <divide_community>
 	mov    0xc(%rsp),%esi
 	mov    (%rsp),%rdi
 	call   12f0 <free_2d_array@plt>
 	mov    %rbx,%rdi
 	call   12a0 <free@plt>
 	add    $0x58,%rsp
 	pop    %rbx
@@ -716,21 +724,21 @@
 	pop    %r15
 	ret
 	mov    0x20(%rsp),%rdx
 	mov    %r13d,%esi
 	mov    0x38(%rsp),%rdi
 	call   1260 <modularityScore@plt>
 	movsd  %xmm0,0x18(%rsp)
-	jmp    1c0f <divide_community+0x143>
+	jmp    1c21 <divide_community+0x143>
 	mov    0x28(%rsp),%rdx
 	mov    %r12d,%esi
 	mov    0x38(%rsp),%rdi
 	call   1260 <modularityScore@plt>
 	movq   %xmm0,%rbp
-	jmp    1c20 <divide_community+0x154>
+	jmp    1c32 <divide_community+0x154>
 	mov    0x30(%rsp),%rcx
 	mov    0x10(%rsp),%rdx
 	mov    0xc(%rsp),%ebp
 	mov    %ebp,%esi
 	mov    %rbx,%rdi
 	call   1350 <final_community_assignment@plt>
 	mov    %ebp,%esi
@@ -738,71 +746,74 @@
 	call   12f0 <free_2d_array@plt>
 	mov    %r15,%rdi
 	call   12a0 <free@plt>
 	mov    %r14,%rdi
 	call   12a0 <free@plt>
 	mov    %rbx,%rdi
 	call   12a0 <free@plt>
-	jmp    1cd7 <divide_community+0x20b>
+	jmp    1ce9 <divide_community+0x20b>
 
-0000000000001d5f <get_community>:
-get_community():
+0000000000001d71 <get_community_assignment>:
+get_community_assignment():
 	endbr64
-	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
-	sub    $0x18,%rsp
-	mov    %rdi,%r13
+	sub    $0x10,%rsp
+	mov    %rdi,%rbx
+	mov    %esi,%r12d
 	mov    %edx,%ebp
-	mov    %rcx,%r15
 	mov    %fs:0x28,%rax
 	mov    %rax,0x8(%rsp)
 	xor    %eax,%eax
+	mov    %edx,%edi
+	call   1270 <create_1d_array_int@plt>
+	mov    %rax,%r13
+	mov    %ebp,%edx
+	mov    %r12d,%esi
+	mov    %rbx,%rdi
 	call   1300 <create_adj_matrix@plt>
 	mov    %rax,%r14
 	mov    %ebp,%esi
 	mov    %rax,%rdi
 	call   1380 <getModularityMatrix@plt>
 	mov    %rax,%r12
 	mov    %ebp,%edi
 	call   1270 <create_1d_array_int@plt>
 	mov    %rax,%rbx
 	test   %ebp,%ebp
-	jle    1dbf <get_community+0x60>
-	mov    %ebp,%edx
-	mov    $0x0,%eax
-	mov    %eax,(%rbx,%rax,4)
-	add    $0x1,%rax
-	cmp    %rdx,%rax
-	jne    1db3 <get_community+0x54>
+	jle    1de1 <get_community_assignment+0x70>
+	mov    %ebp,%eax
+	mov    $0x0,%edx
+	mov    %edx,(%rbx,%rdx,4)
+	add    $0x1,%rdx
+	cmp    %rax,%rdx
+	jne    1dd5 <get_community_assignment+0x64>
 	movl   $0x0,0x4(%rsp)
 	mov    %rbx,%rdx
 	mov    %ebp,%esi
 	mov    %r12,%rdi
 	call   1260 <modularityScore@plt>
-	mov    %r15,%r9
+	mov    %r13,%r9
 	lea    0x4(%rsp),%r8
 	mov    %r12,%rcx
 	mov    %rbx,%rdx
 	mov    %ebp,%esi
 	mov    %r14,%rdi
 	call   1370 <divide_community@plt>
 	mov    %ebp,%esi
 	mov    %r12,%rdi
 	call   12f0 <free_2d_array@plt>
-	mov    %r13,%rdi
-	call   12a0 <free@plt>
 	mov    0x8(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    1e1d <get_community+0xbe>
-	add    $0x18,%rsp
+	jne    1e38 <get_community_assignment+0xc7>
+	mov    %r13,%rax
+	add    $0x10,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
-	pop    %r15
 	ret
 	call   1340 <__stack_chk_fail@plt>
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.fini {}

```diff
@@ -1,11 +1,11 @@
 
 
 
 Disassembly of section .fini:
 
-0000000000001e24 <_fini>:
+0000000000001e40 <_fini>:
 _fini():
 	endbr64
 	sub    $0x8,%rsp
 	add    $0x8,%rsp
 	ret
```

#### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -1,12 +1,13 @@
 
 Hex dump of section '.eh_frame_hdr':
-  0x00002068 011b033b 8c000000 10000000 b8efffff ...;............
-  0x00002078 a8000000 78f1ffff d0000000 88f1ffff ....x...........
-  0x00002088 e8000000 f1f3ffff 00010000 0bf5ffff ................
-  0x00002098 3c010000 4ef5ffff 50010000 87f5ffff <...N...P.......
-  0x000020a8 6c010000 26f6ffff a8010000 5ff6ffff l...&......._...
-  0x000020b8 c4010000 fef6ffff 00020000 36f7ffff ............6...
-  0x000020c8 30020000 3ff9ffff 80020000 d1f9ffff 0...?...........
-  0x000020d8 ac020000 3cfaffff d8020000 64faffff ....<.......d...
-  0x000020e8 ec020000 f7fcffff 3c030000          ........<...
+  0x00002068 011b033b 94000000 11000000 b8efffff ...;............
+  0x00002078 b0000000 78f1ffff d8000000 88f1ffff ....x...........
+  0x00002088 f0000000 f1f3ffff 08010000 0bf5ffff ................
+  0x00002098 44010000 4ef5ffff 58010000 87f5ffff D...N...X.......
+  0x000020a8 74010000 26f6ffff b0010000 5ff6ffff t...&......._...
+  0x000020b8 cc010000 fef6ffff 08020000 36f7ffff ............6...
+  0x000020c8 34020000 48f7ffff 50020000 51f9ffff 4...H...P...Q...
+  0x000020d8 a0020000 e3f9ffff cc020000 4efaffff ............N...
+  0x000020e8 f8020000 76faffff 0c030000 09fdffff ....v...........
+  0x000020f8 5c030000                            \...
```

#### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,51 +1,52 @@
 
 Hex dump of section '.eh_frame':
-  0x000020f8 14000000 00000000 017a5200 01781001 .........zR..x..
-  0x00002108 1b0c0708 90010000 24000000 1c000000 ........$.......
-  0x00002118 08efffff c0010000 000e1046 0e184a0f ...........F..J.
-  0x00002128 0b770880 003f1a3a 2a332422 00000000 .w...?.:*3$"....
-  0x00002138 14000000 44000000 a0f0ffff 10000000 ....D...........
-  0x00002148 00000000 00000000 14000000 5c000000 ............\...
-  0x00002158 98f0ffff b0010000 00000000 00000000 ................
-  0x00002168 38000000 74000000 e9f2ffff 1a010000 8...t...........
-  0x00002178 00460e10 8d02420e 188c0341 0e208604 .F....B....A. ..
-  0x00002188 410e2883 05440e30 0305010e 28410e20 A.(..D.0....(A. 
-  0x00002198 410e1842 0e10420e 08000000 10000000 A..B..B.........
-  0x000021a8 b0000000 c7f3ffff 43000000 00000000 ........C.......
-  0x000021b8 18000000 c4000000 f6f3ffff 39000000 ............9...
-  0x000021c8 00480e10 550a0e08 410b0000 38000000 .H..U...A...8...
-  0x000021d8 e0000000 13f4ffff 9f000000 00460e10 .............F..
-  0x000021e8 8d02420e 188c0341 0e208604 410e2883 ..B....A. ..A.(.
-  0x000021f8 05440e30 024f0a0e 28410e20 410e1842 .D.0.O..(A. A..B
-  0x00002208 0e10420e 08410b00 18000000 1c010000 ..B..A..........
-  0x00002218 76f4ffff 39000000 00480e10 550a0e08 v...9....H..U...
-  0x00002228 410b0000 38000000 38010000 93f4ffff A...8...8.......
-  0x00002238 9f000000 00460e10 8d02420e 188c0341 .....F....B....A
-  0x00002248 0e208604 410e2883 05440e30 024f0a0e . ..A.(..D.0.O..
-  0x00002258 28410e20 410e1842 0e10420e 08410b00 (A. A..B..B..A..
-  0x00002268 2c000000 74010000 f6f4ffff 38000000 ,...t.......8...
-  0x00002278 00460e10 8c02410e 18860341 0e208304 .F....A....A. ..
-  0x00002288 6c0e1841 0e10420e 08000000 00000000 l..A..B.........
-  0x00002298 4c000000 a4010000 fef4ffff 09020000 L...............
-  0x000022a8 00460e10 8f02420e 188e0342 0e208d04 .F....B....B. ..
-  0x000022b8 420e288c 05410e30 8606410e 38830747 B.(..A.0..A.8..G
-  0x000022c8 0ec00103 5d010a0e 38410e30 410e2842 ....]...8A.0A.(B
-  0x000022d8 0e20420e 18420e10 420e0841 0b000000 . B..B..B..A....
-  0x000022e8 28000000 f4010000 b7f6ffff 92000000 (...............
-  0x000022f8 00460e10 8c02410e 18860341 0e208304 .F....A....A. ..
-  0x00002308 02860e18 410e1042 0e080000 28000000 ....A..B....(...
-  0x00002318 20020000 1df7ffff 6b000000 00460e10  .......k....F..
-  0x00002328 8c02410e 18860341 0e208304 025f0e18 ..A....A. ..._..
-  0x00002338 410e1042 0e080000 10000000 4c020000 A..B........L...
-  0x00002348 5cf7ffff 28000000 00000000 4c000000 \...(.......L...
-  0x00002358 60020000 70f7ffff 93020000 00460e10 `...p........F..
-  0x00002368 8f02420e 188e0342 0e208d04 420e288c ..B....B. ..B.(.
-  0x00002378 05410e30 8606410e 38830744 0e900103 .A.0..A.8..D....
-  0x00002388 fd010a0e 38410e30 410e2842 0e20420e ....8A.0A.(B. B.
-  0x00002398 18420e10 420e0841 0b000000 48000000 .B..B..A....H...
-  0x000023a8 b0020000 b3f9ffff c3000000 00460e10 .............F..
-  0x000023b8 8f02420e 188e0342 0e208d04 420e288c ..B....B. ..B.(.
-  0x000023c8 05410e30 8606410e 38830744 0e5002a1 .A.0..A.8..D.P..
-  0x000023d8 0a0e3841 0e30410e 28420e20 420e1842 ..8A.0A.(B. B..B
-  0x000023e8 0e10420e 08410b00 00000000          ..B..A......
+  0x00002100 14000000 00000000 017a5200 01781001 .........zR..x..
+  0x00002110 1b0c0708 90010000 24000000 1c000000 ........$.......
+  0x00002120 00efffff c0010000 000e1046 0e184a0f ...........F..J.
+  0x00002130 0b770880 003f1a3a 2a332422 00000000 .w...?.:*3$"....
+  0x00002140 14000000 44000000 98f0ffff 10000000 ....D...........
+  0x00002150 00000000 00000000 14000000 5c000000 ............\...
+  0x00002160 90f0ffff b0010000 00000000 00000000 ................
+  0x00002170 38000000 74000000 e1f2ffff 1a010000 8...t...........
+  0x00002180 00460e10 8d02420e 188c0341 0e208604 .F....B....A. ..
+  0x00002190 410e2883 05440e30 0305010e 28410e20 A.(..D.0....(A. 
+  0x000021a0 410e1842 0e10420e 08000000 10000000 A..B..B.........
+  0x000021b0 b0000000 bff3ffff 43000000 00000000 ........C.......
+  0x000021c0 18000000 c4000000 eef3ffff 39000000 ............9...
+  0x000021d0 00480e10 550a0e08 410b0000 38000000 .H..U...A...8...
+  0x000021e0 e0000000 0bf4ffff 9f000000 00460e10 .............F..
+  0x000021f0 8d02420e 188c0341 0e208604 410e2883 ..B....A. ..A.(.
+  0x00002200 05440e30 024f0a0e 28410e20 410e1842 .D.0.O..(A. A..B
+  0x00002210 0e10420e 08410b00 18000000 1c010000 ..B..A..........
+  0x00002220 6ef4ffff 39000000 00480e10 550a0e08 n...9....H..U...
+  0x00002230 410b0000 38000000 38010000 8bf4ffff A...8...8.......
+  0x00002240 9f000000 00460e10 8d02420e 188c0341 .....F....B....A
+  0x00002250 0e208604 410e2883 05440e30 024f0a0e . ..A.(..D.0.O..
+  0x00002260 28410e20 410e1842 0e10420e 08410b00 (A. A..B..B..A..
+  0x00002270 28000000 74010000 eef4ffff 38000000 (...t.......8...
+  0x00002280 00460e10 8c02410e 18860341 0e208304 .F....A....A. ..
+  0x00002290 6c0e1841 0e10420e 08000000 18000000 l..A..B.........
+  0x000022a0 a0010000 faf4ffff 12000000 00480e10 .............H..
+  0x000022b0 490e0800 00000000 4c000000 bc010000 I.......L.......
+  0x000022c0 f0f4ffff 09020000 00460e10 8f02420e .........F....B.
+  0x000022d0 188e0342 0e208d04 420e288c 05410e30 ...B. ..B.(..A.0
+  0x000022e0 8606410e 38830747 0ec00103 5d010a0e ..A.8..G....]...
+  0x000022f0 38410e30 410e2842 0e20420e 18420e10 8A.0A.(B. B..B..
+  0x00002300 420e0841 0b000000 28000000 0c020000 B..A....(.......
+  0x00002310 a9f6ffff 92000000 00460e10 8c02410e .........F....A.
+  0x00002320 18860341 0e208304 02860e18 410e1042 ...A. ......A..B
+  0x00002330 0e080000 28000000 38020000 0ff7ffff ....(...8.......
+  0x00002340 6b000000 00460e10 8c02410e 18860341 k....F....A....A
+  0x00002350 0e208304 025f0e18 410e1042 0e080000 . ..._..A..B....
+  0x00002360 10000000 64020000 4ef7ffff 28000000 ....d...N...(...
+  0x00002370 00000000 4c000000 78020000 62f7ffff ....L...x...b...
+  0x00002380 93020000 00460e10 8f02420e 188e0342 .....F....B....B
+  0x00002390 0e208d04 420e288c 05410e30 8606410e . ..B.(..A.0..A.
+  0x000023a0 38830744 0e900103 fd010a0e 38410e30 8..D........8A.0
+  0x000023b0 410e2842 0e20420e 18420e10 420e0841 A.(B. B..B..B..A
+  0x000023c0 0b000000 40000000 c8020000 a5f9ffff ....@...........
+  0x000023d0 cc000000 00460e10 8e02420e 188d0342 .....F....B....B
+  0x000023e0 0e208c04 410e2886 05410e30 8306440e . ..A.(..A.0..D.
+  0x000023f0 4002ae0a 0e30410e 28410e20 420e1842 @....0A.(A. B..B
+  0x00002400 0e10420e 08410b00 00000000          ..B..A......
```

#### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -18,47 +18,48 @@
   0x000000f0 5f5f005f 5f474e55 5f45485f 4652414d __.__GNU_EH_FRAM
   0x00000100 455f4844 52005f66 696e6900 5f474c4f E_HDR._fini._GLO
   0x00000110 42414c5f 4f464653 45545f54 41424c45 BAL_OFFSET_TABLE
   0x00000120 5f005f5f 544d435f 454e445f 5f005f5f _.__TMC_END__.__
   0x00000130 64736f5f 68616e64 6c65005f 44594e41 dso_handle._DYNA
   0x00000140 4d494300 5f696e69 74006773 6c5f6569 MIC._init.gsl_ei
   0x00000150 67656e5f 73796d6d 765f616c 6c6f6300 gen_symmv_alloc.
-  0x00000160 6765745f 636f6d6d 756e6974 79005f5f get_community.__
-  0x00000170 676d6f6e 5f737461 72745f5f 00657869 gmon_start__.exi
-  0x00000180 7440474c 4942435f 322e322e 35005f5f t@GLIBC_2.2.5.__
-  0x00000190 7072696e 74665f63 686b4047 4c494243 printf_chk@GLIBC
-  0x000001a0 5f322e33 2e340067 736c5f6d 61747269 _2.3.4.gsl_matri
-  0x000001b0 785f616c 6c6f6300 67657445 6967656e x_alloc.getEigen
-  0x000001c0 56656374 6f72006d 616c6c6f 6340474c Vector.malloc@GL
-  0x000001d0 4942435f 322e322e 35006372 65617465 IBC_2.2.5.create
-  0x000001e0 5f32645f 61727261 79006d6f 64756c61 _2d_array.modula
-  0x000001f0 72697479 53636f72 65005f49 544d5f64 rityScore._ITM_d
-  0x00000200 65726567 69737465 72544d43 6c6f6e65 eregisterTMClone
-  0x00000210 5461626c 65006372 65617465 5f31645f Table.create_1d_
-  0x00000220 61727261 795f696e 74006773 6c5f6569 array_int.gsl_ei
-  0x00000230 67656e5f 73796d6d 765f736f 72740067 gen_symmv_sort.g
-  0x00000240 736c5f65 6967656e 5f73796d 6d760066 sl_eigen_symmv.f
-  0x00000250 72656540 474c4942 435f322e 322e3500 ree@GLIBC_2.2.5.
-  0x00000260 5f49544d 5f726567 69737465 72544d43 _ITM_registerTMC
-  0x00000270 6c6f6e65 5461626c 65006773 6c5f7665 loneTable.gsl_ve
-  0x00000280 63746f72 5f616c6c 6f63005f 5f637861 ctor_alloc.__cxa
-  0x00000290 5f66696e 616c697a 6540474c 4942435f _finalize@GLIBC_
-  0x000002a0 322e322e 35006773 6c5f7665 63746f72 2.2.5.gsl_vector
-  0x000002b0 5f676574 00736570 61726174 655f6164 _get.separate_ad
-  0x000002c0 6a5f6d61 74726978 0067736c 5f656967 j_matrix.gsl_eig
-  0x000002d0 656e5f73 796d6d76 5f667265 65006672 en_symmv_free.fr
-  0x000002e0 65655f32 645f6172 72617900 63726561 ee_2d_array.crea
-  0x000002f0 74655f32 645f6172 7261795f 696e7400 te_2d_array_int.
-  0x00000300 63726561 74655f61 646a5f6d 61747269 create_adj_matri
-  0x00000310 78006773 6c5f6d61 74726978 5f667265 x.gsl_matrix_fre
-  0x00000320 65006773 6c5f6d61 74726978 5f766965 e.gsl_matrix_vie
-  0x00000330 775f6172 72617900 67736c5f 76656374 w_array.gsl_vect
-  0x00000340 6f725f66 72656500 5f5f7374 61636b5f or_free.__stack_
-  0x00000350 63686b5f 6661696c 40474c49 42435f32 chk_fail@GLIBC_2
-  0x00000360 2e340066 696e616c 5f636f6d 6d756e69 .4.final_communi
-  0x00000370 74795f61 73736967 6e6d656e 74006773 ty_assignment.gs
-  0x00000380 6c5f6d61 74726978 5f636f6c 756d6e00 l_matrix_column.
-  0x00000390 64697669 64655f63 6f6d6d75 6e697479 divide_community
-  0x000003a0 00676574 4d6f6475 6c617269 74794d61 .getModularityMa
-  0x000003b0 74726978 00637265 6174655f 31645f61 trix.create_1d_a
-  0x000003c0 72726179 00                         rray.
+  0x00000160 5f5f676d 6f6e5f73 74617274 5f5f0065 __gmon_start__.e
+  0x00000170 78697440 474c4942 435f322e 322e3500 xit@GLIBC_2.2.5.
+  0x00000180 5f5f7072 696e7466 5f63686b 40474c49 __printf_chk@GLI
+  0x00000190 42435f32 2e332e34 0067736c 5f6d6174 BC_2.3.4.gsl_mat
+  0x000001a0 7269785f 616c6c6f 63006765 74456967 rix_alloc.getEig
+  0x000001b0 656e5665 63746f72 006d616c 6c6f6340 enVector.malloc@
+  0x000001c0 474c4942 435f322e 322e3500 63726561 GLIBC_2.2.5.crea
+  0x000001d0 74655f32 645f6172 72617900 6d6f6475 te_2d_array.modu
+  0x000001e0 6c617269 74795363 6f726500 5f49544d larityScore._ITM
+  0x000001f0 5f646572 65676973 74657254 4d436c6f _deregisterTMClo
+  0x00000200 6e655461 626c6500 63726561 74655f31 neTable.create_1
+  0x00000210 645f6172 7261795f 696e7400 67736c5f d_array_int.gsl_
+  0x00000220 65696765 6e5f7379 6d6d765f 736f7274 eigen_symmv_sort
+  0x00000230 0067736c 5f656967 656e5f73 796d6d76 .gsl_eigen_symmv
+  0x00000240 00676574 5f636f6d 6d756e69 74795f61 .get_community_a
+  0x00000250 73736967 6e6d656e 74006672 65654047 ssignment.free@G
+  0x00000260 4c494243 5f322e32 2e35005f 49544d5f LIBC_2.2.5._ITM_
+  0x00000270 72656769 73746572 544d436c 6f6e6554 registerTMCloneT
+  0x00000280 61626c65 0067736c 5f766563 746f725f able.gsl_vector_
+  0x00000290 616c6c6f 63005f5f 6378615f 66696e61 alloc.__cxa_fina
+  0x000002a0 6c697a65 40474c49 42435f32 2e322e35 lize@GLIBC_2.2.5
+  0x000002b0 0067736c 5f766563 746f725f 67657400 .gsl_vector_get.
+  0x000002c0 73657061 72617465 5f61646a 5f6d6174 separate_adj_mat
+  0x000002d0 72697800 67736c5f 65696765 6e5f7379 rix.gsl_eigen_sy
+  0x000002e0 6d6d765f 66726565 00667265 655f3264 mmv_free.free_2d
+  0x000002f0 5f617272 61790066 7265655f 31645f61 _array.free_1d_a
+  0x00000300 72726179 00637265 6174655f 32645f61 rray.create_2d_a
+  0x00000310 72726179 5f696e74 00637265 6174655f rray_int.create_
+  0x00000320 61646a5f 6d617472 69780067 736c5f6d adj_matrix.gsl_m
+  0x00000330 61747269 785f6672 65650067 736c5f6d atrix_free.gsl_m
+  0x00000340 61747269 785f7669 65775f61 72726179 atrix_view_array
+  0x00000350 0067736c 5f766563 746f725f 66726565 .gsl_vector_free
+  0x00000360 005f5f73 7461636b 5f63686b 5f666169 .__stack_chk_fai
+  0x00000370 6c40474c 4942435f 322e3400 66696e61 l@GLIBC_2.4.fina
+  0x00000380 6c5f636f 6d6d756e 6974795f 61737369 l_community_assi
+  0x00000390 676e6d65 6e740067 736c5f6d 61747269 gnment.gsl_matri
+  0x000003a0 785f636f 6c756d6e 00646976 6964655f x_column.divide_
+  0x000003b0 636f6d6d 756e6974 79006765 744d6f64 community.getMod
+  0x000003c0 756c6172 6974794d 61747269 78006372 ularityMatrix.cr
+  0x000003d0 65617465 5f31645f 61727261 7900     eate_1d_array.
```

### Comparing `apache-age-community-detection-0.1.3/apache_age_community_detection.egg-info/PKG-INFO` & `apache-age-community-detection-0.1.4/apache_age_community_detection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-age-community-detection
-Version: 0.1.3
+Version: 0.1.4
 Summary: Detection of Community by maximizing modularity
 Home-page: https://github.com/Munmud/Community-Detection-Modularity
 Author: Moontasir Mahmood
 Author-email: moontasir042@gmail.com
 License: Apache2.0
 Keywords: Community-Detection,Modularity,Reichardt and Bornholdt,Newman,partition network,k means cluster
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `apache-age-community-detection-0.1.3/apache_age_community_detection.egg-info/SOURCES.txt` & `apache-age-community-detection-0.1.4/apache_age_community_detection.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,9 +8,8 @@
 age_community_detection/VERSION.py
 age_community_detection/__init__.py
 age_community_detection/lib/library.dll
 age_community_detection/lib/library.so
 apache_age_community_detection.egg-info/PKG-INFO
 apache_age_community_detection.egg-info/SOURCES.txt
 apache_age_community_detection.egg-info/dependency_links.txt
-apache_age_community_detection.egg-info/requires.txt
 apache_age_community_detection.egg-info/top_level.txt
```

### Comparing `apache-age-community-detection-0.1.3/setup.py` & `apache-age-community-detection-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     description      = 'Detection of Community by maximizing modularity',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author           = 'Moontasir Mahmood',
     author_email     = 'moontasir042@gmail.com',
     url              = 'https://github.com/Munmud/Community-Detection-Modularity',
     license          = 'Apache2.0',
-    install_requires = ['numpy'],
+    install_requires = [],
     packages         = ['age_community_detection'],
     package_data={'age_community_detection': ['lib/*.so', 'lib/*.dll']},
     keywords         = ['Community-Detection', 'Modularity', 'Reichardt and Bornholdt','Newman', 'partition network', 'k means cluster'],
     python_requires  = '>=3.9',
     classifiers      = [
         'Programming Language :: Python :: 3.9'
     ]
```

