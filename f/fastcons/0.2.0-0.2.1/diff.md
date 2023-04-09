# Comparing `tmp/fastcons-0.2.0-cp311-cp311-musllinux_1_1_x86_64.whl.zip` & `tmp/fastcons-0.2.1-cp311-cp311-musllinux_1_1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 29762 bytes, number of entries: 8
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 17:00 fastcons.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 17:00 fastcons-0.2.0.dist-info/
--rwxr-xr-x  2.0 unx    71016 b- defN 23-Apr-07 17:00 fastcons.cpython-311-x86_64-linux-musl.so
--rw-r--r--  2.0 unx      113 b- defN 23-Apr-07 17:00 fastcons-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Apr-07 17:00 fastcons-0.2.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx     1069 b- defN 23-Apr-07 17:00 fastcons-0.2.0.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      501 b- defN 23-Apr-07 17:00 fastcons-0.2.0.dist-info/RECORD
--rw-r--r--  2.0 unx     2619 b- defN 23-Apr-07 17:00 fastcons-0.2.0.dist-info/METADATA
-8 files, 75338 bytes uncompressed, 28636 bytes compressed:  62.0%
+Zip file size: 30016 bytes, number of entries: 8
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 14:03 fastcons-0.2.1.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 14:03 fastcons.libs/
+-rwxr-xr-x  2.0 unx    72024 b- defN 23-Apr-09 14:03 fastcons.cpython-311-x86_64-linux-musl.so
+-rw-r--r--  2.0 unx      113 b- defN 23-Apr-09 14:03 fastcons-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Apr-09 14:03 fastcons-0.2.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     1069 b- defN 23-Apr-09 14:03 fastcons-0.2.1.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      501 b- defN 23-Apr-09 14:03 fastcons-0.2.1.dist-info/RECORD
+-rw-r--r--  2.0 unx     2619 b- defN 23-Apr-09 14:03 fastcons-0.2.1.dist-info/METADATA
+8 files, 76346 bytes uncompressed, 28890 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: fastcons.libs/
+Filename: fastcons-0.2.1.dist-info/
 Comment: 
 
-Filename: fastcons-0.2.0.dist-info/
+Filename: fastcons.libs/
 Comment: 
 
 Filename: fastcons.cpython-311-x86_64-linux-musl.so
 Comment: 
 
-Filename: fastcons-0.2.0.dist-info/WHEEL
+Filename: fastcons-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: fastcons-0.2.0.dist-info/top_level.txt
+Filename: fastcons-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: fastcons-0.2.0.dist-info/LICENSE.txt
+Filename: fastcons-0.2.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: fastcons-0.2.0.dist-info/RECORD
+Filename: fastcons-0.2.1.dist-info/RECORD
 Comment: 
 
-Filename: fastcons-0.2.0.dist-info/METADATA
+Filename: fastcons-0.2.1.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## fastcons.cpython-311-x86_64-linux-musl.so

### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              DYN (Shared object file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x22b0
   Start of program headers:          64 (bytes into file)
-  Start of section headers:          69032 (bytes into file)
+  Start of section headers:          70040 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           56 (bytes)
   Number of program headers:         8
   Size of section headers:           64 (bytes)
   Number of section headers:         31
   Section header string table index: 30
```

### readelf --wide --program-header {}

```diff
@@ -2,16 +2,16 @@
 Elf file type is DYN (Shared object file)
 Entry point 0x22b0
 There are 8 program headers, starting at offset 64
 
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
   LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x0014a0 0x0014a0 R   0x1000
-  LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x000eb6 0x000eb6 R E 0x1000
-  LOAD           0x003000 0x0000000000003000 0x0000000000003000 0x000640 0x000640 R   0x1000
+  LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x000ec6 0x000ec6 R E 0x1000
+  LOAD           0x003000 0x0000000000003000 0x0000000000003000 0x000644 0x000644 R   0x1000
   LOAD           0x003cc0 0x0000000000004cc0 0x0000000000004cc0 0x000640 0x000690 RW  0x1000
   DYNAMIC        0x003ce0 0x0000000000004ce0 0x0000000000004ce0 0x000170 0x000170 RW  0x8
   GNU_EH_FRAME   0x0031d0 0x00000000000031d0 0x00000000000031d0 0x0000a4 0x0000a4 R   0x4
   GNU_STACK      0x000000 0x0000000000000000 0x0000000000000000 0x000000 0x000000 RW  0x10
   GNU_RELRO      0x003cc0 0x0000000000004cc0 0x0000000000004cc0 0x000340 0x000340 R   0x1
 
  Section to Segment mapping:
```

### readelf --wide --sections {}

```diff
@@ -1,40 +1,40 @@
-There are 31 section headers, starting at offset 0x10da8:
+There are 31 section headers, starting at offset 0x11198:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .gnu.hash         GNU_HASH        0000000000000200 000200 00005c 00   A  2   0  8
   [ 2] .dynsym           DYNSYM          0000000000000260 000260 0005b8 18   A  3   1  8
   [ 3] .dynstr           STRTAB          0000000000000818 000818 000443 00   A  0   0  1
   [ 4] .rela.dyn         RELA            0000000000000c60 000c60 000498 18   A  2   0  8
   [ 5] .rela.plt         RELA            00000000000010f8 0010f8 0003a8 18  AI  2  17  8
   [ 6] .init             PROGBITS        0000000000002000 002000 00000d 00  AX  0   0  1
   [ 7] .plt              PROGBITS        0000000000002010 002010 000280 10  AX  0   0 16
   [ 8] .plt.got          PROGBITS        0000000000002290 002290 000018 08  AX  0   0  8
-  [ 9] .text             PROGBITS        00000000000022b0 0022b0 000bfe 00  AX  0   0 16
-  [10] .fini             PROGBITS        0000000000002eae 002eae 000008 00  AX  0   0  1
+  [ 9] .text             PROGBITS        00000000000022b0 0022b0 000c0e 00  AX  0   0 16
+  [10] .fini             PROGBITS        0000000000002ebe 002ebe 000008 00  AX  0   0  1
   [11] .rodata           PROGBITS        0000000000003000 003000 0001cd 00   A  0   0 32
   [12] .eh_frame_hdr     PROGBITS        00000000000031d0 0031d0 0000a4 00   A  0   0  4
-  [13] .eh_frame         PROGBITS        0000000000003278 003278 0003c8 00   A  0   0  8
+  [13] .eh_frame         PROGBITS        0000000000003278 003278 0003cc 00   A  0   0  8
   [14] .ctors            PROGBITS        0000000000004cc0 003cc0 000010 00  WA  0   0  8
   [15] .dtors            PROGBITS        0000000000004cd0 003cd0 000010 00  WA  0   0  8
   [16] .dynamic          DYNAMIC         0000000000004ce0 003ce0 000170 10  WA  3   0  8
   [17] .got              PROGBITS        0000000000004e50 003e50 0001b0 08  WA  0   0  8
   [18] .data             PROGBITS        0000000000005000 004000 000300 00  WA  0   0 32
   [19] .bss              NOBITS          0000000000005300 004300 000050 00  WA  0   0 32
   [20] .comment          PROGBITS        0000000000000000 004300 00001a 01  MS  0   0  1
   [21] .debug_aranges    PROGBITS        0000000000000000 004320 0000b0 00      0   0 16
-  [22] .debug_info       PROGBITS        0000000000000000 0043d0 00451c 00      0   0  1
-  [23] .debug_abbrev     PROGBITS        0000000000000000 0088ec 00065b 00      0   0  1
-  [24] .debug_line       PROGBITS        0000000000000000 008f47 001414 00      0   0  1
-  [25] .debug_str        PROGBITS        0000000000000000 00a35b 0024f2 01  MS  0   0  1
-  [26] .debug_loc        PROGBITS        0000000000000000 00c84d 002a30 00      0   0  1
-  [27] .debug_ranges     PROGBITS        0000000000000000 00f280 000770 00      0   0 16
-  [28] .symtab           SYMTAB          0000000000000000 00f9f0 000c48 18     29  71  8
-  [29] .strtab           STRTAB          0000000000000000 010638 000666 00      0   0  1
-  [30] .shstrtab         STRTAB          0000000000000000 010c9e 000108 00      0   0  1
+  [22] .debug_info       PROGBITS        0000000000000000 0043d0 0045f9 00      0   0  1
+  [23] .debug_abbrev     PROGBITS        0000000000000000 0089c9 00065b 00      0   0  1
+  [24] .debug_line       PROGBITS        0000000000000000 009024 001475 00      0   0  1
+  [25] .debug_str        PROGBITS        0000000000000000 00a499 0024f2 01  MS  0   0  1
+  [26] .debug_loc        PROGBITS        0000000000000000 00c98b 002c66 00      0   0  1
+  [27] .debug_ranges     PROGBITS        0000000000000000 00f600 0007e0 00      0   0 16
+  [28] .symtab           SYMTAB          0000000000000000 00fde0 000c48 18     29  71  8
+  [29] .strtab           STRTAB          0000000000000000 010a28 000666 00      0   0  1
+  [30] .shstrtab         STRTAB          0000000000000000 01108e 000108 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

### readelf --wide --symbols {}

```diff
@@ -48,38 +48,38 @@
     44: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_New
     45: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyUnicodeWriter_Finish
     46: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __register_frame_info
     47: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyType_GetModuleState
     48: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyType_FromModuleAndSpec
     49: 00000000000023f0    12 FUNC    GLOBAL DEFAULT    9 Nil_repr
     50: 0000000000002710   516 FUNC    GLOBAL DEFAULT    9 Cons_repr
-    51: 0000000000002e80    12 FUNC    GLOBAL DEFAULT    9 PyInit_fastcons
+    51: 0000000000002e90    12 FUNC    GLOBAL DEFAULT    9 PyInit_fastcons
     52: 0000000000002530    87 FUNC    GLOBAL DEFAULT    9 Cons_clear
     53: 0000000000002590   152 FUNC    GLOBAL DEFAULT    9 Cons_dealloc
     54: 0000000000002000     1 FUNC    GLOBAL DEFAULT    6 _init
-    55: 0000000000002ca0   161 FUNC    GLOBAL DEFAULT    9 Cons_from_fast
+    55: 0000000000002ca0   183 FUNC    GLOBAL DEFAULT    9 Cons_from_fast
     56: 0000000000002ba0   138 FUNC    GLOBAL DEFAULT    9 Cons_to_list
-    57: 0000000000002d50   292 FUNC    GLOBAL DEFAULT    9 Cons_from_xs
+    57: 0000000000002d60   292 FUNC    GLOBAL DEFAULT    9 Cons_from_xs
     58: 0000000000002400   295 FUNC    GLOBAL DEFAULT    9 Cons_new
-    59: 0000000000002eae     1 FUNC    GLOBAL DEFAULT   10 _fini
+    59: 0000000000002ebe     1 FUNC    GLOBAL DEFAULT   10 _fini
     60: 0000000000002a40   254 FUNC    GLOBAL DEFAULT    9 Cons_richcompare
 
 Symbol table '.symtab' contains 131 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000200     0 SECTION LOCAL  DEFAULT    1 .gnu.hash
      2: 0000000000000260     0 SECTION LOCAL  DEFAULT    2 .dynsym
      3: 0000000000000818     0 SECTION LOCAL  DEFAULT    3 .dynstr
      4: 0000000000000c60     0 SECTION LOCAL  DEFAULT    4 .rela.dyn
      5: 00000000000010f8     0 SECTION LOCAL  DEFAULT    5 .rela.plt
      6: 0000000000002000     0 SECTION LOCAL  DEFAULT    6 .init
      7: 0000000000002010     0 SECTION LOCAL  DEFAULT    7 .plt
      8: 0000000000002290     0 SECTION LOCAL  DEFAULT    8 .plt.got
      9: 00000000000022b0     0 SECTION LOCAL  DEFAULT    9 .text
-    10: 0000000000002eae     0 SECTION LOCAL  DEFAULT   10 .fini
+    10: 0000000000002ebe     0 SECTION LOCAL  DEFAULT   10 .fini
     11: 0000000000003000     0 SECTION LOCAL  DEFAULT   11 .rodata
     12: 00000000000031d0     0 SECTION LOCAL  DEFAULT   12 .eh_frame_hdr
     13: 0000000000003278     0 SECTION LOCAL  DEFAULT   13 .eh_frame
     14: 0000000000004cc0     0 SECTION LOCAL  DEFAULT   14 .ctors
     15: 0000000000004cd0     0 SECTION LOCAL  DEFAULT   15 .dtors
     16: 0000000000004ce0     0 SECTION LOCAL  DEFAULT   16 .dynamic
     17: 0000000000004e50     0 SECTION LOCAL  DEFAULT   17 .got
@@ -102,16 +102,16 @@
     34: 000000000000230b     0 FUNC    LOCAL  DEFAULT    9 __do_global_dtors_aux
     35: 0000000000005300     1 OBJECT  LOCAL  DEFAULT   19 completed.6214
     36: 0000000000005308     8 OBJECT  LOCAL  DEFAULT   19 dtor_idx.6216
     37: 0000000000002390     0 FUNC    LOCAL  DEFAULT    9 frame_dummy
     38: 0000000000005320    48 OBJECT  LOCAL  DEFAULT   19 object.6226
     39: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
     40: 0000000000004cc8     0 OBJECT  LOCAL  DEFAULT   14 __CTOR_END__
-    41: 000000000000363c     0 OBJECT  LOCAL  DEFAULT   13 __FRAME_END__
-    42: 0000000000002e8c     0 FUNC    LOCAL  DEFAULT    9 __do_global_ctors_aux
+    41: 0000000000003640     0 OBJECT  LOCAL  DEFAULT   13 __FRAME_END__
+    42: 0000000000002e9c     0 FUNC    LOCAL  DEFAULT    9 __do_global_ctors_aux
     43: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS consmodule.c
     44: 00000000000023c0    27 FUNC    LOCAL  DEFAULT    9 Nil_traverse
     45: 00000000000023e0     3 FUNC    LOCAL  DEFAULT    9 Nil_bool
     46: 0000000000005020    24 OBJECT  LOCAL  DEFAULT   18 kwlist.10017
     47: 0000000000002630   119 FUNC    LOCAL  DEFAULT    9 consmodule_clear
     48: 00000000000026b0    85 FUNC    LOCAL  DEFAULT    9 consmodule_traverse
     49: 0000000000005120   104 OBJECT  LOCAL  DEFAULT   18 consmodule
@@ -150,49 +150,49 @@
     82: 0000000000002590   152 FUNC    GLOBAL DEFAULT    9 Cons_dealloc
     83: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyModuleDef_Init
     84: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PySequence_Tuple
     85: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThreadState_Get
     86: 0000000000002710   516 FUNC    GLOBAL DEFAULT    9 Cons_repr
     87: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND Py_ReprLeave
     88: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail
-    89: 0000000000002e80    12 FUNC    GLOBAL DEFAULT    9 PyInit_fastcons
+    89: 0000000000002e90    12 FUNC    GLOBAL DEFAULT    9 PyInit_fastcons
     90: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_NotImplementedStruct
     91: 0000000000002000     1 FUNC    GLOBAL DEFAULT    6 _init
     92: 0000000000002530    87 FUNC    GLOBAL DEFAULT    9 Cons_clear
     93: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyTrash_cond
     94: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyModule_AddType
     95: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_CallFunctionObjArgs
     96: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyModule_GetState
     97: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_Size
     98: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __deregister_frame_info
     99: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
-   100: 0000000000002ca0   161 FUNC    GLOBAL DEFAULT    9 Cons_from_fast
+   100: 0000000000002ca0   183 FUNC    GLOBAL DEFAULT    9 Cons_from_fast
    101: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_GC_UnTrack
    102: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_ValueError
    103: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND Py_ReprEnter
    104: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyTrash_begin
    105: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_TypeError
    106: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_FalseStruct
    107: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyList_New
    108: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
    109: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_Repr
    110: 0000000000002400   295 FUNC    GLOBAL DEFAULT    9 Cons_new
    111: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_Dealloc
    112: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_RichCompare
    113: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_Size
    114: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyUnicodeWriter_WriteStr
-   115: 0000000000002eae     1 FUNC    GLOBAL DEFAULT   10 _fini
+   115: 0000000000002ebe     1 FUNC    GLOBAL DEFAULT   10 _fini
    116: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyType_IsSubtype
    117: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyTrash_end
    118: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyGen_Type
    119: 0000000000002ba0   138 FUNC    GLOBAL DEFAULT    9 Cons_to_list
    120: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyUnicodeWriter_Init
    121: 0000000000002a40   254 FUNC    GLOBAL DEFAULT    9 Cons_richcompare
    122: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyArg_ParseTupleAndKeywords_SizeT
    123: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_RichCompareBool
-   124: 0000000000002d50   292 FUNC    GLOBAL DEFAULT    9 Cons_from_xs
+   124: 0000000000002d60   292 FUNC    GLOBAL DEFAULT    9 Cons_from_xs
    125: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyUnicodeWriter_WriteASCIIString
    126: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_New
    127: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyUnicodeWriter_Finish
    128: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __register_frame_info
    129: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyType_GetModuleState
    130: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyType_FromModuleAndSpec
```

### readelf --wide --relocs {}

```diff
@@ -43,15 +43,15 @@
 0000000000004fe8  0000001f00000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
 0000000000004ff0  0000002700000006 R_X86_64_GLOB_DAT      0000000000000000 PyGen_Type + 0
 0000000000004ff8  0000002e00000006 R_X86_64_GLOB_DAT      0000000000000000 __register_frame_info + 0
 00000000000051c8  0000003a00000001 R_X86_64_64            0000000000002400 Cons_new + 0
 00000000000051f8  0000003400000001 R_X86_64_64            0000000000002530 Cons_clear + 0
 0000000000005208  0000003200000001 R_X86_64_64            0000000000002710 Cons_repr + 0
 0000000000005228  0000003c00000001 R_X86_64_64            0000000000002a40 Cons_richcompare + 0
-0000000000005248  0000003900000001 R_X86_64_64            0000000000002d50 Cons_from_xs + 0
+0000000000005248  0000003900000001 R_X86_64_64            0000000000002d60 Cons_from_xs + 0
 0000000000005268  0000003800000001 R_X86_64_64            0000000000002ba0 Cons_to_list + 0
 00000000000052c8  0000003100000001 R_X86_64_64            00000000000023f0 Nil_repr + 0
 
 Relocation section '.rela.plt' at offset 0x10f8 contains 39 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000004e68  0000000100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyType_GetModuleByDef + 0
 0000000000004e70  0000000300000007 R_X86_64_JUMP_SLOT     0000000000000000 _PyUnicodeWriter_Dealloc + 0
```

### readelf --wide --dynamic {}

```diff
@@ -1,13 +1,13 @@
 
 Dynamic section at offset 0x3ce0 contains 19 entries:
   Tag        Type                         Name/Value
  0x0000000000000001 (NEEDED)             Shared library: [libc.musl-x86_64.so.1]
  0x000000000000000c (INIT)               0x2000
- 0x000000000000000d (FINI)               0x2eae
+ 0x000000000000000d (FINI)               0x2ebe
  0x000000006ffffef5 (GNU_HASH)           0x200
  0x0000000000000005 (STRTAB)             0x818
  0x0000000000000006 (SYMTAB)             0x260
  0x000000000000000a (STRSZ)              1091 (bytes)
  0x000000000000000b (SYMENT)             24 (bytes)
  0x0000000000000003 (PLTGOT)             0x4e50
  0x0000000000000002 (PLTRELSZ)           936 (bytes)
```

### readelf --wide --debug-dump=rawline {}

```diff
@@ -34,23 +34,23 @@
  Line Number Statements:
   [0x00000032]  Extended opcode 2: set Address to 0x2000
   [0x0000003d]  Special opcode 7: advance Address by 0 to 0x2000 and Line by 2 to 3
   [0x0000003e]  Special opcode 6: advance Address by 0 to 0x2000 and Line by 1 to 4 (view 1)
   [0x0000003f]  Advance PC by 1 to 0x2001
   [0x00000041]  Extended opcode 1: End of Sequence
 
-  [0x00000044]  Extended opcode 2: set Address to 0x2eae
-  [0x0000004f]  Special opcode 12: advance Address by 0 to 0x2eae and Line by 7 to 8
-  [0x00000050]  Special opcode 6: advance Address by 0 to 0x2eae and Line by 1 to 9 (view 1)
-  [0x00000051]  Advance PC by 1 to 0x2eaf
+  [0x00000044]  Extended opcode 2: set Address to 0x2ebe
+  [0x0000004f]  Special opcode 12: advance Address by 0 to 0x2ebe and Line by 7 to 8
+  [0x00000050]  Special opcode 6: advance Address by 0 to 0x2ebe and Line by 1 to 9 (view 1)
+  [0x00000051]  Advance PC by 1 to 0x2ebf
   [0x00000053]  Extended opcode 1: End of Sequence
 
 
   Offset:                      0x56
-  Length:                      4964
+  Length:                      5061
   DWARF Version:               3
   Prologue Length:             1273
   Minimum Instruction Length:  1
   Initial value of 'is_stmt':  1
   Line Base:                   -5
   Line Range:                  14
   Opcode Base:                 13
@@ -590,435 +590,435 @@
   [0x00000843]  Extended opcode 4: set Discriminator to 1
   [0x00000847]  Special opcode 187: advance Address by 13 to 0x2620 and Line by 0 to 162
   [0x00000848]  Set column to 1
   [0x0000084a]  Special opcode 6: advance Address by 0 to 0x2620 and Line by 1 to 163 (view 1)
   [0x0000084b]  Special opcode 75: advance Address by 5 to 0x2625 and Line by 0 to 163
   [0x0000084c]  Special opcode 33: advance Address by 2 to 0x2627 and Line by 0 to 163
   [0x0000084d]  Set is_stmt to 1
-  [0x0000084e]  Advance Line by 279 to 442
-  [0x00000851]  Special opcode 131: advance Address by 9 to 0x2630 and Line by 0 to 442
+  [0x0000084e]  Advance Line by 292 to 455
+  [0x00000851]  Special opcode 131: advance Address by 9 to 0x2630 and Line by 0 to 455
   [0x00000852]  Set column to 5
-  [0x00000854]  Special opcode 6: advance Address by 0 to 0x2630 and Line by 1 to 443 (view 1)
+  [0x00000854]  Special opcode 6: advance Address by 0 to 0x2630 and Line by 1 to 456 (view 1)
   [0x00000855]  Set column to 1
   [0x00000857]  Set is_stmt to 0
-  [0x00000858]  Special opcode 4: advance Address by 0 to 0x2630 and Line by -1 to 442 (view 2)
+  [0x00000858]  Special opcode 4: advance Address by 0 to 0x2630 and Line by -1 to 455 (view 2)
   [0x00000859]  Set column to 31
-  [0x0000085b]  Special opcode 20: advance Address by 1 to 0x2631 and Line by 1 to 443
+  [0x0000085b]  Special opcode 20: advance Address by 1 to 0x2631 and Line by 1 to 456
   [0x0000085c]  Set column to 5
-  [0x0000085e]  Special opcode 76: advance Address by 5 to 0x2636 and Line by 1 to 444
+  [0x0000085e]  Special opcode 76: advance Address by 5 to 0x2636 and Line by 1 to 457
   [0x0000085f]  Set column to 31
-  [0x00000861]  Special opcode 60: advance Address by 4 to 0x263a and Line by -1 to 443
+  [0x00000861]  Special opcode 60: advance Address by 4 to 0x263a and Line by -1 to 456
   [0x00000862]  Set column to 5
   [0x00000864]  Set is_stmt to 1
-  [0x00000865]  Special opcode 48: advance Address by 3 to 0x263d and Line by 1 to 444
+  [0x00000865]  Special opcode 48: advance Address by 3 to 0x263d and Line by 1 to 457
   [0x00000866]  Copy (view 1)
   [0x00000867]  Copy (view 2)
   [0x00000868]  Extended opcode 4: set Discriminator to 1
-  [0x0000086c]  Special opcode 75: advance Address by 5 to 0x2642 and Line by 0 to 444
+  [0x0000086c]  Special opcode 75: advance Address by 5 to 0x2642 and Line by 0 to 457
   [0x0000086d]  Extended opcode 4: set Discriminator to 1
-  [0x00000871]  Special opcode 117: advance Address by 8 to 0x264a and Line by 0 to 444
+  [0x00000871]  Special opcode 117: advance Address by 8 to 0x264a and Line by 0 to 457
   [0x00000872]  Set File Name to entry 2 in the File Name Table
   [0x00000874]  Set column to 20
   [0x00000876]  Extended opcode 4: set Discriminator to 1
-  [0x0000087a]  Advance Line by 89 to 533
+  [0x0000087a]  Advance Line by 76 to 533
   [0x0000087d]  Copy (view 1)
   [0x0000087e]  Set column to 5
   [0x00000880]  Extended opcode 4: set Discriminator to 1
   [0x00000884]  Special opcode 9: advance Address by 0 to 0x264a and Line by 4 to 537 (view 2)
   [0x00000885]  Set column to 8
   [0x00000887]  Extended opcode 4: set Discriminator to 1
   [0x0000088b]  Set is_stmt to 0
   [0x0000088c]  Copy (view 3)
   [0x0000088d]  Extended opcode 4: set Discriminator to 1
   [0x00000891]  Special opcode 89: advance Address by 6 to 0x2650 and Line by 0 to 537
   [0x00000892]  Set File Name to entry 1 in the File Name Table
   [0x00000894]  Set column to 5
   [0x00000896]  Extended opcode 4: set Discriminator to 3
   [0x0000089a]  Set is_stmt to 1
-  [0x0000089b]  Advance Line by -93 to 444
+  [0x0000089b]  Advance Line by -80 to 457
   [0x0000089e]  Copy (view 1)
   [0x0000089f]  Extended opcode 4: set Discriminator to 3
-  [0x000008a3]  Special opcode 6: advance Address by 0 to 0x2650 and Line by 1 to 445 (view 2)
+  [0x000008a3]  Special opcode 6: advance Address by 0 to 0x2650 and Line by 1 to 458 (view 2)
   [0x000008a4]  Extended opcode 4: set Discriminator to 3
   [0x000008a8]  Copy (view 3)
   [0x000008a9]  Extended opcode 4: set Discriminator to 3
-  [0x000008ad]  Special opcode 47: advance Address by 3 to 0x2653 and Line by 0 to 445
+  [0x000008ad]  Special opcode 47: advance Address by 3 to 0x2653 and Line by 0 to 458
   [0x000008ae]  Extended opcode 4: set Discriminator to 1
-  [0x000008b2]  Special opcode 75: advance Address by 5 to 0x2658 and Line by 0 to 445
+  [0x000008b2]  Special opcode 75: advance Address by 5 to 0x2658 and Line by 0 to 458
   [0x000008b3]  Extended opcode 4: set Discriminator to 1
-  [0x000008b7]  Special opcode 103: advance Address by 7 to 0x265f and Line by 0 to 445
+  [0x000008b7]  Special opcode 103: advance Address by 7 to 0x265f and Line by 0 to 458
   [0x000008b8]  Set File Name to entry 2 in the File Name Table
   [0x000008ba]  Set column to 20
   [0x000008bc]  Extended opcode 4: set Discriminator to 1
-  [0x000008c0]  Advance Line by 88 to 533
+  [0x000008c0]  Advance Line by 75 to 533
   [0x000008c3]  Copy (view 1)
   [0x000008c4]  Set column to 5
   [0x000008c6]  Extended opcode 4: set Discriminator to 1
   [0x000008ca]  Special opcode 9: advance Address by 0 to 0x265f and Line by 4 to 537 (view 2)
   [0x000008cb]  Set column to 8
   [0x000008cd]  Extended opcode 4: set Discriminator to 1
   [0x000008d1]  Set is_stmt to 0
   [0x000008d2]  Copy (view 3)
   [0x000008d3]  Extended opcode 4: set Discriminator to 1
   [0x000008d7]  Special opcode 89: advance Address by 6 to 0x2665 and Line by 0 to 537
   [0x000008d8]  Set File Name to entry 1 in the File Name Table
   [0x000008da]  Set column to 5
   [0x000008dc]  Extended opcode 4: set Discriminator to 3
   [0x000008e0]  Set is_stmt to 1
-  [0x000008e1]  Advance Line by -92 to 445
+  [0x000008e1]  Advance Line by -79 to 458
   [0x000008e4]  Copy (view 1)
   [0x000008e5]  Extended opcode 4: set Discriminator to 3
-  [0x000008e9]  Special opcode 6: advance Address by 0 to 0x2665 and Line by 1 to 446 (view 2)
+  [0x000008e9]  Special opcode 6: advance Address by 0 to 0x2665 and Line by 1 to 459 (view 2)
   [0x000008ea]  Extended opcode 4: set Discriminator to 3
   [0x000008ee]  Copy (view 3)
   [0x000008ef]  Extended opcode 4: set Discriminator to 3
-  [0x000008f3]  Special opcode 61: advance Address by 4 to 0x2669 and Line by 0 to 446
+  [0x000008f3]  Special opcode 61: advance Address by 4 to 0x2669 and Line by 0 to 459
   [0x000008f4]  Extended opcode 4: set Discriminator to 1
-  [0x000008f8]  Special opcode 75: advance Address by 5 to 0x266e and Line by 0 to 446
+  [0x000008f8]  Special opcode 75: advance Address by 5 to 0x266e and Line by 0 to 459
   [0x000008f9]  Extended opcode 4: set Discriminator to 1
-  [0x000008fd]  Special opcode 117: advance Address by 8 to 0x2676 and Line by 0 to 446
+  [0x000008fd]  Special opcode 117: advance Address by 8 to 0x2676 and Line by 0 to 459
   [0x000008fe]  Set File Name to entry 2 in the File Name Table
   [0x00000900]  Set column to 20
   [0x00000902]  Extended opcode 4: set Discriminator to 1
-  [0x00000906]  Advance Line by 87 to 533
+  [0x00000906]  Advance Line by 74 to 533
   [0x00000909]  Copy (view 1)
   [0x0000090a]  Set column to 5
   [0x0000090c]  Extended opcode 4: set Discriminator to 1
   [0x00000910]  Special opcode 9: advance Address by 0 to 0x2676 and Line by 4 to 537 (view 2)
   [0x00000911]  Set column to 8
   [0x00000913]  Extended opcode 4: set Discriminator to 1
   [0x00000917]  Set is_stmt to 0
   [0x00000918]  Copy (view 3)
   [0x00000919]  Extended opcode 4: set Discriminator to 1
   [0x0000091d]  Special opcode 89: advance Address by 6 to 0x267c and Line by 0 to 537
   [0x0000091e]  Set File Name to entry 1 in the File Name Table
   [0x00000920]  Set column to 5
   [0x00000922]  Extended opcode 4: set Discriminator to 3
   [0x00000926]  Set is_stmt to 1
-  [0x00000927]  Advance Line by -91 to 446
+  [0x00000927]  Advance Line by -78 to 459
   [0x0000092a]  Copy (view 1)
   [0x0000092b]  Extended opcode 4: set Discriminator to 3
-  [0x0000092f]  Special opcode 6: advance Address by 0 to 0x267c and Line by 1 to 447 (view 2)
+  [0x0000092f]  Special opcode 6: advance Address by 0 to 0x267c and Line by 1 to 460 (view 2)
   [0x00000930]  Set column to 1
   [0x00000932]  Extended opcode 4: set Discriminator to 3
   [0x00000936]  Set is_stmt to 0
-  [0x00000937]  Special opcode 6: advance Address by 0 to 0x267c and Line by 1 to 448 (view 3)
+  [0x00000937]  Special opcode 6: advance Address by 0 to 0x267c and Line by 1 to 461 (view 3)
   [0x00000938]  Extended opcode 4: set Discriminator to 3
-  [0x0000093c]  Special opcode 47: advance Address by 3 to 0x267f and Line by 0 to 448
+  [0x0000093c]  Special opcode 47: advance Address by 3 to 0x267f and Line by 0 to 461
   [0x0000093d]  Set File Name to entry 2 in the File Name Table
   [0x0000093f]  Set column to 9
   [0x00000941]  Set is_stmt to 1
-  [0x00000942]  Advance Line by 90 to 538
+  [0x00000942]  Advance Line by 77 to 538
   [0x00000945]  Special opcode 19: advance Address by 1 to 0x2680 and Line by 0 to 538
   [0x00000946]  Set is_stmt to 0
   [0x00000947]  Special opcode 75: advance Address by 5 to 0x2685 and Line by 0 to 538
   [0x00000948]  Set File Name to entry 1 in the File Name Table
   [0x0000094a]  Set column to 5
   [0x0000094c]  Set is_stmt to 1
-  [0x0000094d]  Advance Line by -92 to 446
+  [0x0000094d]  Advance Line by -79 to 459
   [0x00000950]  Copy (view 1)
-  [0x00000951]  Special opcode 6: advance Address by 0 to 0x2685 and Line by 1 to 447 (view 2)
+  [0x00000951]  Special opcode 6: advance Address by 0 to 0x2685 and Line by 1 to 460 (view 2)
   [0x00000952]  Set column to 1
   [0x00000954]  Set is_stmt to 0
-  [0x00000955]  Special opcode 6: advance Address by 0 to 0x2685 and Line by 1 to 448 (view 3)
-  [0x00000956]  Special opcode 47: advance Address by 3 to 0x2688 and Line by 0 to 448
+  [0x00000955]  Special opcode 6: advance Address by 0 to 0x2685 and Line by 1 to 461 (view 3)
+  [0x00000956]  Special opcode 47: advance Address by 3 to 0x2688 and Line by 0 to 461
   [0x00000957]  Set File Name to entry 2 in the File Name Table
   [0x00000959]  Set column to 9
   [0x0000095b]  Set is_stmt to 1
-  [0x0000095c]  Advance Line by 90 to 538
+  [0x0000095c]  Advance Line by 77 to 538
   [0x0000095f]  Special opcode 117: advance Address by 8 to 0x2690 and Line by 0 to 538
   [0x00000960]  Set is_stmt to 0
   [0x00000961]  Special opcode 75: advance Address by 5 to 0x2695 and Line by 0 to 538
   [0x00000962]  Special opcode 159: advance Address by 11 to 0x26a0 and Line by 0 to 538
   [0x00000963]  Set is_stmt to 1
   [0x00000964]  Copy (view 1)
   [0x00000965]  Set is_stmt to 0
   [0x00000966]  Special opcode 75: advance Address by 5 to 0x26a5 and Line by 0 to 538
   [0x00000967]  Set File Name to entry 1 in the File Name Table
   [0x00000969]  Set column to 1
   [0x0000096b]  Set is_stmt to 1
-  [0x0000096c]  Advance Line by -106 to 432
-  [0x0000096f]  Special opcode 159: advance Address by 11 to 0x26b0 and Line by 0 to 432
+  [0x0000096c]  Advance Line by -93 to 445
+  [0x0000096f]  Special opcode 159: advance Address by 11 to 0x26b0 and Line by 0 to 445
   [0x00000970]  Set column to 5
-  [0x00000972]  Special opcode 6: advance Address by 0 to 0x26b0 and Line by 1 to 433 (view 1)
+  [0x00000972]  Special opcode 6: advance Address by 0 to 0x26b0 and Line by 1 to 446 (view 1)
   [0x00000973]  Set column to 1
   [0x00000975]  Set is_stmt to 0
-  [0x00000976]  Special opcode 4: advance Address by 0 to 0x26b0 and Line by -1 to 432 (view 2)
+  [0x00000976]  Special opcode 4: advance Address by 0 to 0x26b0 and Line by -1 to 445 (view 2)
   [0x00000977]  Set column to 31
-  [0x00000979]  Special opcode 146: advance Address by 10 to 0x26ba and Line by 1 to 433
+  [0x00000979]  Special opcode 146: advance Address by 10 to 0x26ba and Line by 1 to 446
   [0x0000097a]  Set column to 5
-  [0x0000097c]  Special opcode 76: advance Address by 5 to 0x26bf and Line by 1 to 434
+  [0x0000097c]  Special opcode 76: advance Address by 5 to 0x26bf and Line by 1 to 447
   [0x0000097d]  Set column to 31
-  [0x0000097f]  Special opcode 60: advance Address by 4 to 0x26c3 and Line by -1 to 433
+  [0x0000097f]  Special opcode 60: advance Address by 4 to 0x26c3 and Line by -1 to 446
   [0x00000980]  Set column to 5
   [0x00000982]  Set is_stmt to 1
-  [0x00000983]  Special opcode 48: advance Address by 3 to 0x26c6 and Line by 1 to 434
+  [0x00000983]  Special opcode 48: advance Address by 3 to 0x26c6 and Line by 1 to 447
   [0x00000984]  Copy (view 1)
   [0x00000985]  Extended opcode 4: set Discriminator to 1
-  [0x00000989]  Special opcode 75: advance Address by 5 to 0x26cb and Line by 0 to 434
+  [0x00000989]  Special opcode 75: advance Address by 5 to 0x26cb and Line by 0 to 447
   [0x0000098a]  Extended opcode 4: set Discriminator to 1
-  [0x0000098e]  Special opcode 75: advance Address by 5 to 0x26d0 and Line by 0 to 434
+  [0x0000098e]  Special opcode 75: advance Address by 5 to 0x26d0 and Line by 0 to 447
   [0x0000098f]  Extended opcode 4: set Discriminator to 1
   [0x00000993]  Set is_stmt to 0
-  [0x00000994]  Special opcode 61: advance Address by 4 to 0x26d4 and Line by 0 to 434
+  [0x00000994]  Special opcode 61: advance Address by 4 to 0x26d4 and Line by 0 to 447
   [0x00000995]  Set is_stmt to 1
   [0x00000996]  Copy (view 1)
-  [0x00000997]  Special opcode 6: advance Address by 0 to 0x26d4 and Line by 1 to 435 (view 2)
+  [0x00000997]  Special opcode 6: advance Address by 0 to 0x26d4 and Line by 1 to 448 (view 2)
   [0x00000998]  Copy (view 3)
   [0x00000999]  Extended opcode 4: set Discriminator to 1
-  [0x0000099d]  Special opcode 117: advance Address by 8 to 0x26dc and Line by 0 to 435
+  [0x0000099d]  Special opcode 117: advance Address by 8 to 0x26dc and Line by 0 to 448
   [0x0000099e]  Extended opcode 4: set Discriminator to 1
-  [0x000009a2]  Special opcode 75: advance Address by 5 to 0x26e1 and Line by 0 to 435
+  [0x000009a2]  Special opcode 75: advance Address by 5 to 0x26e1 and Line by 0 to 448
   [0x000009a3]  Extended opcode 4: set Discriminator to 1
   [0x000009a7]  Set is_stmt to 0
-  [0x000009a8]  Special opcode 61: advance Address by 4 to 0x26e5 and Line by 0 to 435
+  [0x000009a8]  Special opcode 61: advance Address by 4 to 0x26e5 and Line by 0 to 448
   [0x000009a9]  Set is_stmt to 1
   [0x000009aa]  Copy (view 1)
-  [0x000009ab]  Special opcode 6: advance Address by 0 to 0x26e5 and Line by 1 to 436 (view 2)
+  [0x000009ab]  Special opcode 6: advance Address by 0 to 0x26e5 and Line by 1 to 449 (view 2)
   [0x000009ac]  Copy (view 3)
   [0x000009ad]  Set column to 12
   [0x000009af]  Set is_stmt to 0
-  [0x000009b0]  Special opcode 62: advance Address by 4 to 0x26e9 and Line by 1 to 437
+  [0x000009b0]  Special opcode 62: advance Address by 4 to 0x26e9 and Line by 1 to 450
   [0x000009b1]  Set column to 5
-  [0x000009b3]  Special opcode 32: advance Address by 2 to 0x26eb and Line by -1 to 436
+  [0x000009b3]  Special opcode 32: advance Address by 2 to 0x26eb and Line by -1 to 449
   [0x000009b4]  Extended opcode 4: set Discriminator to 1
   [0x000009b8]  Set is_stmt to 1
-  [0x000009b9]  Special opcode 75: advance Address by 5 to 0x26f0 and Line by 0 to 436
+  [0x000009b9]  Special opcode 75: advance Address by 5 to 0x26f0 and Line by 0 to 449
   [0x000009ba]  Set column to 1
   [0x000009bc]  Extended opcode 4: set Discriminator to 1
   [0x000009c0]  Set is_stmt to 0
-  [0x000009c1]  Special opcode 7: advance Address by 0 to 0x26f0 and Line by 2 to 438 (view 1)
+  [0x000009c1]  Special opcode 7: advance Address by 0 to 0x26f0 and Line by 2 to 451 (view 1)
   [0x000009c2]  Set column to 5
   [0x000009c4]  Extended opcode 4: set Discriminator to 1
-  [0x000009c8]  Special opcode 17: advance Address by 1 to 0x26f1 and Line by -2 to 436
+  [0x000009c8]  Special opcode 17: advance Address by 1 to 0x26f1 and Line by -2 to 449
   [0x000009c9]  Set column to 1
   [0x000009cb]  Extended opcode 4: set Discriminator to 1
-  [0x000009cf]  Special opcode 91: advance Address by 6 to 0x26f7 and Line by 2 to 438
+  [0x000009cf]  Special opcode 91: advance Address by 6 to 0x26f7 and Line by 2 to 451
   [0x000009d0]  Extended opcode 4: set Discriminator to 1
-  [0x000009d4]  Special opcode 19: advance Address by 1 to 0x26f8 and Line by 0 to 438
+  [0x000009d4]  Special opcode 19: advance Address by 1 to 0x26f8 and Line by 0 to 451
   [0x000009d5]  Set column to 5
   [0x000009d7]  Extended opcode 4: set Discriminator to 1
-  [0x000009db]  Special opcode 31: advance Address by 2 to 0x26fa and Line by -2 to 436
+  [0x000009db]  Special opcode 31: advance Address by 2 to 0x26fa and Line by -2 to 449
   [0x000009dc]  Extended opcode 4: set Discriminator to 1
-  [0x000009e0]  Special opcode 89: advance Address by 6 to 0x2700 and Line by 0 to 436
+  [0x000009e0]  Special opcode 89: advance Address by 6 to 0x2700 and Line by 0 to 449
   [0x000009e1]  Set column to 1
-  [0x000009e3]  Special opcode 7: advance Address by 0 to 0x2700 and Line by 2 to 438 (view 1)
-  [0x000009e4]  Special opcode 19: advance Address by 1 to 0x2701 and Line by 0 to 438
-  [0x000009e5]  Special opcode 19: advance Address by 1 to 0x2702 and Line by 0 to 438
-  [0x000009e6]  Special opcode 33: advance Address by 2 to 0x2704 and Line by 0 to 438
+  [0x000009e3]  Special opcode 7: advance Address by 0 to 0x2700 and Line by 2 to 451 (view 1)
+  [0x000009e4]  Special opcode 19: advance Address by 1 to 0x2701 and Line by 0 to 451
+  [0x000009e5]  Special opcode 19: advance Address by 1 to 0x2702 and Line by 0 to 451
+  [0x000009e6]  Special opcode 33: advance Address by 2 to 0x2704 and Line by 0 to 451
   [0x000009e7]  Set is_stmt to 1
-  [0x000009e8]  Advance Line by -195 to 243
-  [0x000009eb]  Special opcode 173: advance Address by 12 to 0x2710 and Line by 0 to 243
+  [0x000009e8]  Advance Line by -195 to 256
+  [0x000009eb]  Special opcode 173: advance Address by 12 to 0x2710 and Line by 0 to 256
   [0x000009ec]  Set is_stmt to 0
   [0x000009ed]  Copy (view 1)
   [0x000009ee]  Set column to 19
-  [0x000009f0]  Special opcode 37: advance Address by 2 to 0x2712 and Line by 4 to 247
+  [0x000009f0]  Special opcode 37: advance Address by 2 to 0x2712 and Line by 4 to 260
   [0x000009f1]  Set column to 1
-  [0x000009f3]  Special opcode 99: advance Address by 7 to 0x2719 and Line by -4 to 243
+  [0x000009f3]  Special opcode 99: advance Address by 7 to 0x2719 and Line by -4 to 256
   [0x000009f4]  Set column to 19
-  [0x000009f6]  Special opcode 219: advance Address by 15 to 0x2728 and Line by 4 to 247
+  [0x000009f6]  Special opcode 219: advance Address by 15 to 0x2728 and Line by 4 to 260
   [0x000009f7]  Set column to 1
-  [0x000009f9]  Special opcode 57: advance Address by 4 to 0x272c and Line by -4 to 243
+  [0x000009f9]  Special opcode 57: advance Address by 4 to 0x272c and Line by -4 to 256
   [0x000009fa]  Set column to 5
   [0x000009fc]  Set is_stmt to 1
-  [0x000009fd]  Special opcode 230: advance Address by 16 to 0x273c and Line by 1 to 244
-  [0x000009fe]  Special opcode 6: advance Address by 0 to 0x273c and Line by 1 to 245 (view 1)
-  [0x000009ff]  Special opcode 6: advance Address by 0 to 0x273c and Line by 1 to 246 (view 2)
-  [0x00000a00]  Special opcode 6: advance Address by 0 to 0x273c and Line by 1 to 247 (view 3)
+  [0x000009fd]  Special opcode 230: advance Address by 16 to 0x273c and Line by 1 to 257
+  [0x000009fe]  Special opcode 6: advance Address by 0 to 0x273c and Line by 1 to 258 (view 1)
+  [0x000009ff]  Special opcode 6: advance Address by 0 to 0x273c and Line by 1 to 259 (view 2)
+  [0x00000a00]  Special opcode 6: advance Address by 0 to 0x273c and Line by 1 to 260 (view 3)
   [0x00000a01]  Set File Name to entry 2 in the File Name Table
-  [0x00000a03]  Advance Line by -114 to 133
+  [0x00000a03]  Advance Line by -127 to 133
   [0x00000a06]  Copy (view 4)
   [0x00000a07]  Set File Name to entry 1 in the File Name Table
   [0x00000a09]  Set column to 19
   [0x00000a0b]  Set is_stmt to 0
-  [0x00000a0c]  Advance Line by 114 to 247
+  [0x00000a0c]  Advance Line by 127 to 260
   [0x00000a0f]  Copy (view 5)
   [0x00000a10]  Set column to 5
   [0x00000a12]  Set is_stmt to 1
-  [0x00000a13]  Special opcode 76: advance Address by 5 to 0x2741 and Line by 1 to 248
+  [0x00000a13]  Special opcode 76: advance Address by 5 to 0x2741 and Line by 1 to 261
   [0x00000a14]  Set column to 8
   [0x00000a16]  Set is_stmt to 0
   [0x00000a17]  Copy (view 1)
   [0x00000a18]  Set column to 5
   [0x00000a1a]  Set is_stmt to 1
-  [0x00000a1b]  Special opcode 120: advance Address by 8 to 0x2749 and Line by 3 to 251
+  [0x00000a1b]  Special opcode 120: advance Address by 8 to 0x2749 and Line by 3 to 264
   [0x00000a1c]  Set column to 31
   [0x00000a1e]  Set is_stmt to 0
   [0x00000a1f]  Copy (view 1)
-  [0x00000a20]  Special opcode 75: advance Address by 5 to 0x274e and Line by 0 to 251
+  [0x00000a20]  Special opcode 75: advance Address by 5 to 0x274e and Line by 0 to 264
   [0x00000a21]  Set column to 5
   [0x00000a23]  Set is_stmt to 1
-  [0x00000a24]  Special opcode 48: advance Address by 3 to 0x2751 and Line by 1 to 252
+  [0x00000a24]  Special opcode 48: advance Address by 3 to 0x2751 and Line by 1 to 265
   [0x00000a25]  Set column to 8
   [0x00000a27]  Set is_stmt to 0
   [0x00000a28]  Copy (view 1)
   [0x00000a29]  Set column to 5
   [0x00000a2b]  Set is_stmt to 1
-  [0x00000a2c]  Special opcode 78: advance Address by 5 to 0x2756 and Line by 3 to 255
+  [0x00000a2c]  Special opcode 78: advance Address by 5 to 0x2756 and Line by 3 to 268
   [0x00000a2d]  Set column to 9
   [0x00000a2f]  Set is_stmt to 0
-  [0x00000a30]  Special opcode 7: advance Address by 0 to 0x2756 and Line by 2 to 257 (view 1)
+  [0x00000a30]  Special opcode 7: advance Address by 0 to 0x2756 and Line by 2 to 270 (view 1)
   [0x00000a31]  Set column to 19
-  [0x00000a33]  Special opcode 45: advance Address by 3 to 0x2759 and Line by -2 to 255
+  [0x00000a33]  Special opcode 45: advance Address by 3 to 0x2759 and Line by -2 to 268
   [0x00000a34]  Set column to 5
   [0x00000a36]  Set is_stmt to 1
-  [0x00000a37]  Special opcode 63: advance Address by 4 to 0x275d and Line by 2 to 257
+  [0x00000a37]  Special opcode 63: advance Address by 4 to 0x275d and Line by 2 to 270
   [0x00000a38]  Set column to 9
   [0x00000a3a]  Set is_stmt to 0
   [0x00000a3b]  Copy (view 1)
   [0x00000a3c]  Set column to 7
-  [0x00000a3e]  Special opcode 75: advance Address by 5 to 0x2762 and Line by 0 to 257
+  [0x00000a3e]  Special opcode 75: advance Address by 5 to 0x2762 and Line by 0 to 270
   [0x00000a3f]  Set column to 5
   [0x00000a41]  Set is_stmt to 1
-  [0x00000a42]  Special opcode 34: advance Address by 2 to 0x2764 and Line by 1 to 258
+  [0x00000a42]  Special opcode 34: advance Address by 2 to 0x2764 and Line by 1 to 271
   [0x00000a43]  Set column to 8
   [0x00000a45]  Set is_stmt to 0
   [0x00000a46]  Copy (view 1)
   [0x00000a47]  Set column to 9
   [0x00000a49]  Set is_stmt to 1
-  [0x00000a4a]  Special opcode 76: advance Address by 5 to 0x2769 and Line by 1 to 259
+  [0x00000a4a]  Special opcode 76: advance Address by 5 to 0x2769 and Line by 1 to 272
   [0x00000a4b]  Set column to 52
   [0x00000a4d]  Set is_stmt to 0
   [0x00000a4e]  Copy (view 1)
   [0x00000a4f]  Set column to 5
   [0x00000a51]  Set is_stmt to 1
-  [0x00000a52]  Advance Line by 50 to 309
-  [0x00000a54]  Special opcode 89: advance Address by 6 to 0x276f and Line by 0 to 309
+  [0x00000a52]  Advance Line by 50 to 322
+  [0x00000a54]  Special opcode 89: advance Address by 6 to 0x276f and Line by 0 to 322
   [0x00000a55]  Set column to 12
   [0x00000a57]  Set is_stmt to 0
   [0x00000a58]  Copy (view 1)
   [0x00000a59]  Set column to 1
-  [0x00000a5b]  Special opcode 34: advance Address by 2 to 0x2771 and Line by 1 to 310
+  [0x00000a5b]  Special opcode 34: advance Address by 2 to 0x2771 and Line by 1 to 323
   [0x00000a5c]  Advance PC by constant 17 to 0x2782
-  [0x00000a5d]  Special opcode 215: advance Address by 15 to 0x2791 and Line by 0 to 310
+  [0x00000a5d]  Special opcode 215: advance Address by 15 to 0x2791 and Line by 0 to 323
   [0x00000a5e]  Set column to 5
   [0x00000a60]  Set is_stmt to 1
-  [0x00000a61]  Advance Line by -49 to 261
-  [0x00000a63]  Special opcode 103: advance Address by 7 to 0x2798 and Line by 0 to 261
-  [0x00000a64]  Special opcode 160: advance Address by 11 to 0x27a3 and Line by 1 to 262
+  [0x00000a61]  Advance Line by -49 to 274
+  [0x00000a63]  Special opcode 103: advance Address by 7 to 0x2798 and Line by 0 to 274
+  [0x00000a64]  Special opcode 160: advance Address by 11 to 0x27a3 and Line by 1 to 275
   [0x00000a65]  Set column to 9
   [0x00000a67]  Set is_stmt to 0
-  [0x00000a68]  Special opcode 7: advance Address by 0 to 0x27a3 and Line by 2 to 264 (view 1)
+  [0x00000a68]  Special opcode 7: advance Address by 0 to 0x27a3 and Line by 2 to 277 (view 1)
   [0x00000a69]  Set column to 25
-  [0x00000a6b]  Special opcode 115: advance Address by 8 to 0x27ab and Line by -2 to 262
+  [0x00000a6b]  Special opcode 115: advance Address by 8 to 0x27ab and Line by -2 to 275
   [0x00000a6c]  Set column to 5
   [0x00000a6e]  Set is_stmt to 1
-  [0x00000a6f]  Special opcode 76: advance Address by 5 to 0x27b0 and Line by 1 to 263
+  [0x00000a6f]  Special opcode 76: advance Address by 5 to 0x27b0 and Line by 1 to 276
   [0x00000a70]  Set column to 23
   [0x00000a72]  Set is_stmt to 0
   [0x00000a73]  Copy (view 1)
   [0x00000a74]  Set column to 5
   [0x00000a76]  Set is_stmt to 1
-  [0x00000a77]  Special opcode 132: advance Address by 9 to 0x27b9 and Line by 1 to 264
+  [0x00000a77]  Special opcode 132: advance Address by 9 to 0x27b9 and Line by 1 to 277
   [0x00000a78]  Set column to 9
   [0x00000a7a]  Set is_stmt to 0
   [0x00000a7b]  Copy (view 1)
   [0x00000a7c]  Set column to 8
-  [0x00000a7e]  Special opcode 75: advance Address by 5 to 0x27be and Line by 0 to 264
+  [0x00000a7e]  Special opcode 75: advance Address by 5 to 0x27be and Line by 0 to 277
   [0x00000a7f]  Set column to 9
   [0x00000a81]  Set is_stmt to 1
-  [0x00000a82]  Advance Line by 13 to 277
+  [0x00000a82]  Advance Line by 13 to 290
   [0x00000a84]  Advance PC by constant 17 to 0x27cf
-  [0x00000a85]  Special opcode 19: advance Address by 1 to 0x27d0 and Line by 0 to 277
+  [0x00000a85]  Special opcode 19: advance Address by 1 to 0x27d0 and Line by 0 to 290
   [0x00000a86]  Copy (view 1)
-  [0x00000a87]  Special opcode 7: advance Address by 0 to 0x27d0 and Line by 2 to 279 (view 2)
+  [0x00000a87]  Special opcode 7: advance Address by 0 to 0x27d0 and Line by 2 to 292 (view 2)
   [0x00000a88]  Set column to 14
   [0x00000a8a]  Set is_stmt to 0
   [0x00000a8b]  Copy (view 3)
   [0x00000a8c]  Set column to 9
   [0x00000a8e]  Set is_stmt to 1
-  [0x00000a8f]  Special opcode 62: advance Address by 4 to 0x27d4 and Line by 1 to 280
+  [0x00000a8f]  Special opcode 62: advance Address by 4 to 0x27d4 and Line by 1 to 293
   [0x00000a90]  Set column to 12
   [0x00000a92]  Set is_stmt to 0
   [0x00000a93]  Copy (view 1)
   [0x00000a94]  Set column to 14
   [0x00000a96]  Set is_stmt to 1
-  [0x00000a97]  Special opcode 147: advance Address by 10 to 0x27de and Line by 2 to 282
+  [0x00000a97]  Special opcode 147: advance Address by 10 to 0x27de and Line by 2 to 295
   [0x00000a98]  Set File Name to entry 2 in the File Name Table
   [0x00000a9a]  Set column to 19
-  [0x00000a9c]  Advance Line by -133 to 149
+  [0x00000a9c]  Advance Line by -146 to 149
   [0x00000a9f]  Copy (view 1)
   [0x00000aa0]  Set column to 5
   [0x00000aa2]  Special opcode 6: advance Address by 0 to 0x27de and Line by 1 to 150 (view 2)
   [0x00000aa3]  Set is_stmt to 0
   [0x00000aa4]  Copy (view 3)
   [0x00000aa5]  Set is_stmt to 1
   [0x00000aa6]  Advance Line by -17 to 133
   [0x00000aa8]  Copy (view 4)
   [0x00000aa9]  Set File Name to entry 1 in the File Name Table
   [0x00000aab]  Set column to 17
   [0x00000aad]  Set is_stmt to 0
-  [0x00000aae]  Advance Line by 149 to 282
+  [0x00000aae]  Advance Line by 162 to 295
   [0x00000ab1]  Copy (view 5)
   [0x00000ab2]  Set column to 9
   [0x00000ab4]  Set is_stmt to 1
-  [0x00000ab5]  Advance Line by 13 to 295
-  [0x00000ab7]  Special opcode 145: advance Address by 10 to 0x27e8 and Line by 0 to 295
+  [0x00000ab5]  Advance Line by 13 to 308
+  [0x00000ab7]  Special opcode 145: advance Address by 10 to 0x27e8 and Line by 0 to 308
   [0x00000ab8]  Set column to 13
   [0x00000aba]  Set is_stmt to 0
   [0x00000abb]  Copy (view 1)
   [0x00000abc]  Set column to 12
-  [0x00000abe]  Special opcode 187: advance Address by 13 to 0x27f5 and Line by 0 to 295
+  [0x00000abe]  Special opcode 187: advance Address by 13 to 0x27f5 and Line by 0 to 308
   [0x00000abf]  Set column to 11
   [0x00000ac1]  Set is_stmt to 1
-  [0x00000ac2]  Advance Line by -27 to 268
-  [0x00000ac4]  Special opcode 61: advance Address by 4 to 0x27f9 and Line by 0 to 268
+  [0x00000ac2]  Advance Line by -27 to 281
+  [0x00000ac4]  Special opcode 61: advance Address by 4 to 0x27f9 and Line by 0 to 281
   [0x00000ac5]  Set File Name to entry 2 in the File Name Table
   [0x00000ac7]  Set column to 19
-  [0x00000ac9]  Advance Line by -119 to 149
+  [0x00000ac9]  Advance Line by -132 to 149
   [0x00000acc]  Copy (view 1)
   [0x00000acd]  Set column to 5
   [0x00000acf]  Special opcode 6: advance Address by 0 to 0x27f9 and Line by 1 to 150 (view 2)
   [0x00000ad0]  Set is_stmt to 0
   [0x00000ad1]  Copy (view 3)
   [0x00000ad2]  Set is_stmt to 1
   [0x00000ad3]  Advance Line by -17 to 133
   [0x00000ad5]  Copy (view 4)
   [0x00000ad6]  Set File Name to entry 1 in the File Name Table
   [0x00000ad8]  Set column to 11
   [0x00000ada]  Set is_stmt to 0
-  [0x00000adb]  Advance Line by 135 to 268
+  [0x00000adb]  Advance Line by 148 to 281
   [0x00000ade]  Copy (view 5)
   [0x00000adf]  Set column to 9
   [0x00000ae1]  Set is_stmt to 1
-  [0x00000ae2]  Special opcode 146: advance Address by 10 to 0x2803 and Line by 1 to 269
-  [0x00000ae3]  Special opcode 6: advance Address by 0 to 0x2803 and Line by 1 to 270 (view 1)
+  [0x00000ae2]  Special opcode 146: advance Address by 10 to 0x2803 and Line by 1 to 282
+  [0x00000ae3]  Special opcode 6: advance Address by 0 to 0x2803 and Line by 1 to 283 (view 1)
   [0x00000ae4]  Set column to 16
   [0x00000ae6]  Set is_stmt to 0
   [0x00000ae7]  Copy (view 2)
-  [0x00000ae8]  Special opcode 131: advance Address by 9 to 0x280c and Line by 0 to 270
+  [0x00000ae8]  Special opcode 131: advance Address by 9 to 0x280c and Line by 0 to 283
   [0x00000ae9]  Set column to 9
   [0x00000aeb]  Set is_stmt to 1
-  [0x00000aec]  Special opcode 48: advance Address by 3 to 0x280f and Line by 1 to 271
+  [0x00000aec]  Special opcode 48: advance Address by 3 to 0x280f and Line by 1 to 284
   [0x00000aed]  Set column to 12
   [0x00000aef]  Set is_stmt to 0
   [0x00000af0]  Copy (view 1)
   [0x00000af1]  Set column to 9
   [0x00000af3]  Set is_stmt to 1
-  [0x00000af4]  Special opcode 77: advance Address by 5 to 0x2814 and Line by 2 to 273
+  [0x00000af4]  Special opcode 77: advance Address by 5 to 0x2814 and Line by 2 to 286
   [0x00000af5]  Set column to 13
   [0x00000af7]  Set is_stmt to 0
   [0x00000af8]  Copy (view 1)
   [0x00000af9]  Set column to 12
-  [0x00000afb]  Special opcode 159: advance Address by 11 to 0x281f and Line by 0 to 273
+  [0x00000afb]  Special opcode 159: advance Address by 11 to 0x281f and Line by 0 to 286
   [0x00000afc]  Set File Name to entry 2 in the File Name Table
   [0x00000afe]  Set column to 9
-  [0x00000b00]  Advance Line by 264 to 537
+  [0x00000b00]  Advance Line by 251 to 537
   [0x00000b03]  Special opcode 33: advance Address by 2 to 0x2821 and Line by 0 to 537
   [0x00000b04]  Set File Name to entry 1 in the File Name Table
   [0x00000b06]  Set column to 12
-  [0x00000b08]  Advance Line by -264 to 273
-  [0x00000b0b]  Special opcode 61: advance Address by 4 to 0x2825 and Line by 0 to 273
+  [0x00000b08]  Advance Line by -251 to 286
+  [0x00000b0b]  Special opcode 61: advance Address by 4 to 0x2825 and Line by 0 to 286
   [0x00000b0c]  Set column to 9
   [0x00000b0e]  Set is_stmt to 1
-  [0x00000b0f]  Special opcode 37: advance Address by 2 to 0x2827 and Line by 4 to 277
+  [0x00000b0f]  Special opcode 37: advance Address by 2 to 0x2827 and Line by 4 to 290
   [0x00000b10]  Copy (view 1)
   [0x00000b11]  Set File Name to entry 2 in the File Name Table
   [0x00000b13]  Set column to 20
-  [0x00000b15]  Advance Line by 256 to 533
+  [0x00000b15]  Advance Line by 243 to 533
   [0x00000b18]  Copy (view 2)
   [0x00000b19]  Set column to 5
   [0x00000b1b]  Special opcode 9: advance Address by 0 to 0x2827 and Line by 4 to 537 (view 3)
   [0x00000b1c]  Set column to 9
   [0x00000b1e]  Set is_stmt to 0
   [0x00000b1f]  Copy (view 4)
   [0x00000b20]  Set column to 8
@@ -1027,20 +1027,20 @@
   [0x00000b25]  Set is_stmt to 1
   [0x00000b26]  Special opcode 90: advance Address by 6 to 0x2831 and Line by 1 to 538
   [0x00000b27]  Set is_stmt to 0
   [0x00000b28]  Special opcode 215: advance Address by 15 to 0x2840 and Line by 0 to 538
   [0x00000b29]  Set File Name to entry 1 in the File Name Table
   [0x00000b2b]  Set column to 17
   [0x00000b2d]  Set is_stmt to 1
-  [0x00000b2e]  Advance Line by -249 to 289
+  [0x00000b2e]  Advance Line by -236 to 302
   [0x00000b31]  Copy (view 1)
   [0x00000b32]  Copy (view 2)
   [0x00000b33]  Set File Name to entry 2 in the File Name Table
   [0x00000b35]  Set column to 20
-  [0x00000b37]  Advance Line by 244 to 533
+  [0x00000b37]  Advance Line by 231 to 533
   [0x00000b3a]  Copy (view 3)
   [0x00000b3b]  Set column to 5
   [0x00000b3d]  Special opcode 9: advance Address by 0 to 0x2840 and Line by 4 to 537 (view 4)
   [0x00000b3e]  Set column to 9
   [0x00000b40]  Set is_stmt to 0
   [0x00000b41]  Copy (view 5)
   [0x00000b42]  Set column to 8
@@ -1049,69 +1049,69 @@
   [0x00000b47]  Set is_stmt to 1
   [0x00000b48]  Special opcode 90: advance Address by 6 to 0x284a and Line by 1 to 538
   [0x00000b49]  Set is_stmt to 0
   [0x00000b4a]  Special opcode 201: advance Address by 14 to 0x2858 and Line by 0 to 538
   [0x00000b4b]  Set File Name to entry 1 in the File Name Table
   [0x00000b4d]  Set column to 5
   [0x00000b4f]  Set is_stmt to 1
-  [0x00000b50]  Advance Line by -231 to 307
+  [0x00000b50]  Advance Line by -218 to 320
   [0x00000b53]  Copy (view 1)
-  [0x00000b54]  Special opcode 118: advance Address by 8 to 0x2860 and Line by 1 to 308
+  [0x00000b54]  Special opcode 118: advance Address by 8 to 0x2860 and Line by 1 to 321
   [0x00000b55]  Set column to 24
   [0x00000b57]  Extended opcode 4: set Discriminator to 1
   [0x00000b5b]  Set is_stmt to 0
-  [0x00000b5c]  Advance Line by -49 to 259
-  [0x00000b5e]  Special opcode 229: advance Address by 16 to 0x2870 and Line by 0 to 259
+  [0x00000b5c]  Advance Line by -49 to 272
+  [0x00000b5e]  Special opcode 229: advance Address by 16 to 0x2870 and Line by 0 to 272
   [0x00000b5f]  Extended opcode 4: set Discriminator to 1
-  [0x00000b63]  Special opcode 131: advance Address by 9 to 0x2879 and Line by 0 to 259
+  [0x00000b63]  Special opcode 131: advance Address by 9 to 0x2879 and Line by 0 to 272
   [0x00000b64]  Set column to 13
   [0x00000b66]  Set is_stmt to 1
-  [0x00000b67]  Advance Line by 24 to 283
-  [0x00000b69]  Special opcode 215: advance Address by 15 to 0x2888 and Line by 0 to 283
+  [0x00000b67]  Advance Line by 24 to 296
+  [0x00000b69]  Special opcode 215: advance Address by 15 to 0x2888 and Line by 0 to 296
   [0x00000b6a]  Set column to 17
   [0x00000b6c]  Set is_stmt to 0
   [0x00000b6d]  Copy (view 1)
   [0x00000b6e]  Set column to 16
   [0x00000b70]  Advance PC by constant 17 to 0x2899
-  [0x00000b71]  Special opcode 47: advance Address by 3 to 0x289c and Line by 0 to 283
+  [0x00000b71]  Special opcode 47: advance Address by 3 to 0x289c and Line by 0 to 296
   [0x00000b72]  Set column to 13
   [0x00000b74]  Set is_stmt to 1
-  [0x00000b75]  Special opcode 63: advance Address by 4 to 0x28a0 and Line by 2 to 285
+  [0x00000b75]  Special opcode 63: advance Address by 4 to 0x28a0 and Line by 2 to 298
   [0x00000b76]  Set column to 20
   [0x00000b78]  Set is_stmt to 0
   [0x00000b79]  Copy (view 1)
   [0x00000b7a]  Set column to 13
   [0x00000b7c]  Set is_stmt to 1
-  [0x00000b7d]  Special opcode 160: advance Address by 11 to 0x28ab and Line by 1 to 286
+  [0x00000b7d]  Special opcode 160: advance Address by 11 to 0x28ab and Line by 1 to 299
   [0x00000b7e]  Set column to 16
   [0x00000b80]  Set is_stmt to 0
   [0x00000b81]  Copy (view 1)
   [0x00000b82]  Set column to 13
   [0x00000b84]  Set is_stmt to 1
-  [0x00000b85]  Special opcode 77: advance Address by 5 to 0x28b0 and Line by 2 to 288
+  [0x00000b85]  Special opcode 77: advance Address by 5 to 0x28b0 and Line by 2 to 301
   [0x00000b86]  Set column to 17
   [0x00000b88]  Set is_stmt to 0
   [0x00000b89]  Copy (view 1)
   [0x00000b8a]  Set column to 16
-  [0x00000b8c]  Special opcode 159: advance Address by 11 to 0x28bb and Line by 0 to 288
+  [0x00000b8c]  Special opcode 159: advance Address by 11 to 0x28bb and Line by 0 to 301
   [0x00000b8d]  Set File Name to entry 2 in the File Name Table
   [0x00000b8f]  Set column to 9
-  [0x00000b91]  Advance Line by 249 to 537
+  [0x00000b91]  Advance Line by 236 to 537
   [0x00000b94]  Special opcode 33: advance Address by 2 to 0x28bd and Line by 0 to 537
   [0x00000b95]  Set File Name to entry 1 in the File Name Table
   [0x00000b97]  Set column to 16
-  [0x00000b99]  Advance Line by -249 to 288
-  [0x00000b9c]  Special opcode 61: advance Address by 4 to 0x28c1 and Line by 0 to 288
+  [0x00000b99]  Advance Line by -236 to 301
+  [0x00000b9c]  Special opcode 61: advance Address by 4 to 0x28c1 and Line by 0 to 301
   [0x00000b9d]  Set column to 13
   [0x00000b9f]  Set is_stmt to 1
-  [0x00000ba0]  Special opcode 93: advance Address by 6 to 0x28c7 and Line by 4 to 292
+  [0x00000ba0]  Special opcode 93: advance Address by 6 to 0x28c7 and Line by 4 to 305
   [0x00000ba1]  Copy (view 1)
   [0x00000ba2]  Set File Name to entry 2 in the File Name Table
   [0x00000ba4]  Set column to 20
-  [0x00000ba6]  Advance Line by 241 to 533
+  [0x00000ba6]  Advance Line by 228 to 533
   [0x00000ba9]  Copy (view 2)
   [0x00000baa]  Set column to 5
   [0x00000bac]  Special opcode 9: advance Address by 0 to 0x28c7 and Line by 4 to 537 (view 3)
   [0x00000bad]  Set column to 9
   [0x00000baf]  Set is_stmt to 0
   [0x00000bb0]  Copy (view 4)
   [0x00000bb1]  Set column to 8
@@ -1120,235 +1120,235 @@
   [0x00000bb6]  Set is_stmt to 1
   [0x00000bb7]  Special opcode 90: advance Address by 6 to 0x28d1 and Line by 1 to 538
   [0x00000bb8]  Set is_stmt to 0
   [0x00000bb9]  Special opcode 215: advance Address by 15 to 0x28e0 and Line by 0 to 538
   [0x00000bba]  Set File Name to entry 1 in the File Name Table
   [0x00000bbc]  Set column to 5
   [0x00000bbe]  Set is_stmt to 1
-  [0x00000bbf]  Advance Line by -238 to 300
+  [0x00000bbf]  Advance Line by -225 to 313
   [0x00000bc2]  Copy (view 1)
   [0x00000bc3]  Set column to 9
   [0x00000bc5]  Set is_stmt to 0
-  [0x00000bc6]  Special opcode 6: advance Address by 0 to 0x28e0 and Line by 1 to 301 (view 2)
+  [0x00000bc6]  Special opcode 6: advance Address by 0 to 0x28e0 and Line by 1 to 314 (view 2)
   [0x00000bc7]  Set column to 25
-  [0x00000bc9]  Special opcode 116: advance Address by 8 to 0x28e8 and Line by -1 to 300
+  [0x00000bc9]  Special opcode 116: advance Address by 8 to 0x28e8 and Line by -1 to 313
   [0x00000bca]  Set column to 5
   [0x00000bcc]  Set is_stmt to 1
-  [0x00000bcd]  Special opcode 76: advance Address by 5 to 0x28ed and Line by 1 to 301
+  [0x00000bcd]  Special opcode 76: advance Address by 5 to 0x28ed and Line by 1 to 314
   [0x00000bce]  Set column to 9
   [0x00000bd0]  Set is_stmt to 0
   [0x00000bd1]  Copy (view 1)
   [0x00000bd2]  Set column to 8
-  [0x00000bd4]  Special opcode 75: advance Address by 5 to 0x28f2 and Line by 0 to 301
+  [0x00000bd4]  Special opcode 75: advance Address by 5 to 0x28f2 and Line by 0 to 314
   [0x00000bd5]  Set column to 5
   [0x00000bd7]  Set is_stmt to 1
-  [0x00000bd8]  Special opcode 119: advance Address by 8 to 0x28fa and Line by 2 to 303
-  [0x00000bd9]  Special opcode 118: advance Address by 8 to 0x2902 and Line by 1 to 304
+  [0x00000bd8]  Special opcode 119: advance Address by 8 to 0x28fa and Line by 2 to 316
+  [0x00000bd9]  Special opcode 118: advance Address by 8 to 0x2902 and Line by 1 to 317
   [0x00000bda]  Set column to 12
   [0x00000bdc]  Set is_stmt to 0
   [0x00000bdd]  Copy (view 1)
   [0x00000bde]  Set column to 1
-  [0x00000be0]  Special opcode 193: advance Address by 13 to 0x290f and Line by 6 to 310
+  [0x00000be0]  Special opcode 193: advance Address by 13 to 0x290f and Line by 6 to 323
   [0x00000be1]  Set is_stmt to 1
-  [0x00000be2]  Advance Line by 81 to 391
+  [0x00000be2]  Advance Line by 81 to 404
   [0x00000be5]  Advance PC by constant 17 to 0x2920
-  [0x00000be6]  Special opcode 5: advance Address by 0 to 0x2920 and Line by 0 to 391
+  [0x00000be6]  Special opcode 5: advance Address by 0 to 0x2920 and Line by 0 to 404
   [0x00000be7]  Set column to 5
-  [0x00000be9]  Special opcode 6: advance Address by 0 to 0x2920 and Line by 1 to 392 (view 1)
+  [0x00000be9]  Special opcode 6: advance Address by 0 to 0x2920 and Line by 1 to 405 (view 1)
   [0x00000bea]  Set column to 1
   [0x00000bec]  Set is_stmt to 0
-  [0x00000bed]  Special opcode 4: advance Address by 0 to 0x2920 and Line by -1 to 391 (view 2)
+  [0x00000bed]  Special opcode 4: advance Address by 0 to 0x2920 and Line by -1 to 404 (view 2)
   [0x00000bee]  Set column to 31
-  [0x00000bf0]  Special opcode 104: advance Address by 7 to 0x2927 and Line by 1 to 392
+  [0x00000bf0]  Special opcode 104: advance Address by 7 to 0x2927 and Line by 1 to 405
   [0x00000bf1]  Set column to 5
   [0x00000bf3]  Set is_stmt to 1
-  [0x00000bf4]  Special opcode 76: advance Address by 5 to 0x292c and Line by 1 to 393
+  [0x00000bf4]  Special opcode 76: advance Address by 5 to 0x292c and Line by 1 to 406
   [0x00000bf5]  Set column to 8
   [0x00000bf7]  Set is_stmt to 0
   [0x00000bf8]  Copy (view 1)
   [0x00000bf9]  Set column to 23
-  [0x00000bfb]  Special opcode 134: advance Address by 9 to 0x2935 and Line by 3 to 396
+  [0x00000bfb]  Special opcode 134: advance Address by 9 to 0x2935 and Line by 3 to 409
   [0x00000bfc]  Set column to 5
   [0x00000bfe]  Set is_stmt to 1
-  [0x00000bff]  Special opcode 215: advance Address by 15 to 0x2944 and Line by 0 to 396
+  [0x00000bff]  Special opcode 215: advance Address by 15 to 0x2944 and Line by 0 to 409
   [0x00000c00]  Set column to 23
   [0x00000c02]  Set is_stmt to 0
   [0x00000c03]  Copy (view 1)
   [0x00000c04]  Set column to 21
-  [0x00000c06]  Special opcode 75: advance Address by 5 to 0x2949 and Line by 0 to 396
+  [0x00000c06]  Special opcode 75: advance Address by 5 to 0x2949 and Line by 0 to 409
   [0x00000c07]  Set column to 5
   [0x00000c09]  Set is_stmt to 1
-  [0x00000c0a]  Special opcode 62: advance Address by 4 to 0x294d and Line by 1 to 397
+  [0x00000c0a]  Special opcode 62: advance Address by 4 to 0x294d and Line by 1 to 410
   [0x00000c0b]  Set column to 23
   [0x00000c0d]  Set is_stmt to 0
-  [0x00000c0e]  Special opcode 4: advance Address by 0 to 0x294d and Line by -1 to 396 (view 1)
+  [0x00000c0e]  Special opcode 4: advance Address by 0 to 0x294d and Line by -1 to 409 (view 1)
   [0x00000c0f]  Set column to 8
-  [0x00000c11]  Special opcode 48: advance Address by 3 to 0x2950 and Line by 1 to 397
+  [0x00000c11]  Special opcode 48: advance Address by 3 to 0x2950 and Line by 1 to 410
   [0x00000c12]  Set column to 5
   [0x00000c14]  Set is_stmt to 1
-  [0x00000c15]  Special opcode 133: advance Address by 9 to 0x2959 and Line by 2 to 399
+  [0x00000c15]  Special opcode 133: advance Address by 9 to 0x2959 and Line by 2 to 412
   [0x00000c16]  Set column to 9
   [0x00000c18]  Set is_stmt to 0
   [0x00000c19]  Copy (view 1)
   [0x00000c1a]  Set column to 8
-  [0x00000c1c]  Special opcode 117: advance Address by 8 to 0x2961 and Line by 0 to 399
+  [0x00000c1c]  Special opcode 117: advance Address by 8 to 0x2961 and Line by 0 to 412
   [0x00000c1d]  Set column to 5
   [0x00000c1f]  Set is_stmt to 1
-  [0x00000c20]  Special opcode 119: advance Address by 8 to 0x2969 and Line by 2 to 401
+  [0x00000c20]  Special opcode 119: advance Address by 8 to 0x2969 and Line by 2 to 414
   [0x00000c21]  Set column to 28
   [0x00000c23]  Set is_stmt to 0
   [0x00000c24]  Copy (view 1)
   [0x00000c25]  Set column to 5
   [0x00000c27]  Set is_stmt to 1
-  [0x00000c28]  Special opcode 188: advance Address by 13 to 0x2976 and Line by 1 to 402
+  [0x00000c28]  Special opcode 188: advance Address by 13 to 0x2976 and Line by 1 to 415
   [0x00000c29]  Set column to 8
   [0x00000c2b]  Set is_stmt to 0
   [0x00000c2c]  Copy (view 1)
   [0x00000c2d]  Set column to 5
   [0x00000c2f]  Set is_stmt to 1
-  [0x00000c30]  Special opcode 133: advance Address by 9 to 0x297f and Line by 2 to 404
+  [0x00000c30]  Special opcode 133: advance Address by 9 to 0x297f and Line by 2 to 417
   [0x00000c31]  Set File Name to entry 3 in the File Name Table
   [0x00000c33]  Set column to 1
-  [0x00000c35]  Advance Line by -370 to 34
+  [0x00000c35]  Advance Line by -383 to 34
   [0x00000c38]  Special opcode 173: advance Address by 12 to 0x298b and Line by 0 to 34
   [0x00000c39]  Set column to 5
   [0x00000c3b]  Special opcode 6: advance Address by 0 to 0x298b and Line by 1 to 35 (view 1)
   [0x00000c3c]  Special opcode 6: advance Address by 0 to 0x298b and Line by 1 to 36 (view 2)
   [0x00000c3d]  Set File Name to entry 1 in the File Name Table
   [0x00000c3f]  Set is_stmt to 0
-  [0x00000c40]  Advance Line by 369 to 405
+  [0x00000c40]  Advance Line by 382 to 418
   [0x00000c43]  Copy (view 3)
   [0x00000c44]  Set File Name to entry 3 in the File Name Table
   [0x00000c46]  Set column to 27
-  [0x00000c48]  Advance Line by -369 to 36
+  [0x00000c48]  Advance Line by -382 to 36
   [0x00000c4b]  Special opcode 103: advance Address by 7 to 0x2992 and Line by 0 to 36
   [0x00000c4c]  Special opcode 61: advance Address by 4 to 0x2996 and Line by 0 to 36
   [0x00000c4d]  Set File Name to entry 1 in the File Name Table
   [0x00000c4f]  Set column to 5
   [0x00000c51]  Set is_stmt to 1
-  [0x00000c52]  Advance Line by 369 to 405
+  [0x00000c52]  Advance Line by 382 to 418
   [0x00000c55]  Copy (view 1)
   [0x00000c56]  Set File Name to entry 3 in the File Name Table
   [0x00000c58]  Set column to 1
-  [0x00000c5a]  Advance Line by -371 to 34
+  [0x00000c5a]  Advance Line by -384 to 34
   [0x00000c5d]  Special opcode 75: advance Address by 5 to 0x299b and Line by 0 to 34
   [0x00000c5e]  Set column to 5
   [0x00000c60]  Special opcode 6: advance Address by 0 to 0x299b and Line by 1 to 35 (view 1)
   [0x00000c61]  Special opcode 6: advance Address by 0 to 0x299b and Line by 1 to 36 (view 2)
   [0x00000c62]  Set File Name to entry 1 in the File Name Table
   [0x00000c64]  Set column to 9
   [0x00000c66]  Set is_stmt to 0
-  [0x00000c67]  Advance Line by 370 to 406
+  [0x00000c67]  Advance Line by 383 to 419
   [0x00000c6a]  Copy (view 3)
   [0x00000c6b]  Set File Name to entry 3 in the File Name Table
   [0x00000c6d]  Set column to 27
-  [0x00000c6f]  Advance Line by -370 to 36
+  [0x00000c6f]  Advance Line by -383 to 36
   [0x00000c72]  Special opcode 145: advance Address by 10 to 0x29a5 and Line by 0 to 36
   [0x00000c73]  Special opcode 61: advance Address by 4 to 0x29a9 and Line by 0 to 36
   [0x00000c74]  Set File Name to entry 1 in the File Name Table
   [0x00000c76]  Set column to 5
   [0x00000c78]  Set is_stmt to 1
-  [0x00000c79]  Advance Line by 370 to 406
+  [0x00000c79]  Advance Line by 383 to 419
   [0x00000c7c]  Copy (view 1)
   [0x00000c7d]  Set column to 9
   [0x00000c7f]  Set is_stmt to 0
   [0x00000c80]  Copy (view 2)
   [0x00000c81]  Set column to 8
-  [0x00000c83]  Special opcode 229: advance Address by 16 to 0x29b9 and Line by 0 to 406
+  [0x00000c83]  Special opcode 229: advance Address by 16 to 0x29b9 and Line by 0 to 419
   [0x00000c84]  Set File Name to entry 2 in the File Name Table
   [0x00000c86]  Set column to 9
-  [0x00000c88]  Advance Line by 131 to 537
+  [0x00000c88]  Advance Line by 118 to 537
   [0x00000c8b]  Special opcode 33: advance Address by 2 to 0x29bb and Line by 0 to 537
   [0x00000c8c]  Set File Name to entry 1 in the File Name Table
   [0x00000c8e]  Set column to 8
-  [0x00000c90]  Advance Line by -131 to 406
-  [0x00000c93]  Special opcode 61: advance Address by 4 to 0x29bf and Line by 0 to 406
+  [0x00000c90]  Advance Line by -118 to 419
+  [0x00000c93]  Special opcode 61: advance Address by 4 to 0x29bf and Line by 0 to 419
   [0x00000c94]  Set column to 5
   [0x00000c96]  Set is_stmt to 1
-  [0x00000c97]  Special opcode 38: advance Address by 2 to 0x29c1 and Line by 5 to 411
+  [0x00000c97]  Special opcode 38: advance Address by 2 to 0x29c1 and Line by 5 to 424
   [0x00000c98]  Copy (view 1)
   [0x00000c99]  Set File Name to entry 2 in the File Name Table
   [0x00000c9b]  Set column to 20
-  [0x00000c9d]  Advance Line by 122 to 533
+  [0x00000c9d]  Advance Line by 109 to 533
   [0x00000ca0]  Copy (view 2)
   [0x00000ca1]  Set column to 5
   [0x00000ca3]  Special opcode 9: advance Address by 0 to 0x29c1 and Line by 4 to 537 (view 3)
   [0x00000ca4]  Set column to 9
   [0x00000ca6]  Set is_stmt to 0
   [0x00000ca7]  Copy (view 4)
   [0x00000ca8]  Set column to 8
   [0x00000caa]  Special opcode 61: advance Address by 4 to 0x29c5 and Line by 0 to 537
   [0x00000cab]  Special opcode 89: advance Address by 6 to 0x29cb and Line by 0 to 537
   [0x00000cac]  Set File Name to entry 1 in the File Name Table
   [0x00000cae]  Set column to 5
   [0x00000cb0]  Set is_stmt to 1
-  [0x00000cb1]  Advance Line by -126 to 411
+  [0x00000cb1]  Advance Line by -113 to 424
   [0x00000cb4]  Copy (view 1)
   [0x00000cb5]  Copy (view 2)
-  [0x00000cb6]  Special opcode 7: advance Address by 0 to 0x29cb and Line by 2 to 413 (view 3)
+  [0x00000cb6]  Special opcode 7: advance Address by 0 to 0x29cb and Line by 2 to 426 (view 3)
   [0x00000cb7]  Set column to 22
   [0x00000cb9]  Set is_stmt to 0
   [0x00000cba]  Copy (view 4)
   [0x00000cbb]  Set column to 20
   [0x00000cbd]  Advance PC by constant 17 to 0x29dc
-  [0x00000cbe]  Special opcode 5: advance Address by 0 to 0x29dc and Line by 0 to 413
+  [0x00000cbe]  Special opcode 5: advance Address by 0 to 0x29dc and Line by 0 to 426
   [0x00000cbf]  Set column to 5
   [0x00000cc1]  Set is_stmt to 1
-  [0x00000cc2]  Special opcode 48: advance Address by 3 to 0x29df and Line by 1 to 414
+  [0x00000cc2]  Special opcode 48: advance Address by 3 to 0x29df and Line by 1 to 427
   [0x00000cc3]  Set column to 22
   [0x00000cc5]  Set is_stmt to 0
-  [0x00000cc6]  Special opcode 4: advance Address by 0 to 0x29df and Line by -1 to 413 (view 1)
+  [0x00000cc6]  Special opcode 4: advance Address by 0 to 0x29df and Line by -1 to 426 (view 1)
   [0x00000cc7]  Set column to 8
-  [0x00000cc9]  Special opcode 48: advance Address by 3 to 0x29e2 and Line by 1 to 414
+  [0x00000cc9]  Special opcode 48: advance Address by 3 to 0x29e2 and Line by 1 to 427
   [0x00000cca]  Set column to 5
   [0x00000ccc]  Set is_stmt to 1
-  [0x00000ccd]  Special opcode 77: advance Address by 5 to 0x29e7 and Line by 2 to 416
+  [0x00000ccd]  Special opcode 77: advance Address by 5 to 0x29e7 and Line by 2 to 429
   [0x00000cce]  Set column to 9
   [0x00000cd0]  Set is_stmt to 0
   [0x00000cd1]  Copy (view 1)
   [0x00000cd2]  Set column to 8
-  [0x00000cd4]  Special opcode 117: advance Address by 8 to 0x29ef and Line by 0 to 416
+  [0x00000cd4]  Special opcode 117: advance Address by 8 to 0x29ef and Line by 0 to 429
   [0x00000cd5]  Set column to 5
   [0x00000cd7]  Set is_stmt to 1
-  [0x00000cd8]  Special opcode 64: advance Address by 4 to 0x29f3 and Line by 3 to 419
+  [0x00000cd8]  Special opcode 64: advance Address by 4 to 0x29f3 and Line by 3 to 432
   [0x00000cd9]  Set column to 31
   [0x00000cdb]  Set is_stmt to 0
-  [0x00000cdc]  Special opcode 6: advance Address by 0 to 0x29f3 and Line by 1 to 420 (view 1)
+  [0x00000cdc]  Special opcode 6: advance Address by 0 to 0x29f3 and Line by 1 to 433 (view 1)
   [0x00000cdd]  Set column to 10
-  [0x00000cdf]  Special opcode 47: advance Address by 3 to 0x29f6 and Line by 0 to 420
+  [0x00000cdf]  Special opcode 47: advance Address by 3 to 0x29f6 and Line by 0 to 433
   [0x00000ce0]  Set column to 5
   [0x00000ce2]  Set is_stmt to 1
-  [0x00000ce3]  Special opcode 160: advance Address by 11 to 0x2a01 and Line by 1 to 421
+  [0x00000ce3]  Special opcode 160: advance Address by 11 to 0x2a01 and Line by 1 to 434
   [0x00000ce4]  Set column to 16
   [0x00000ce6]  Set is_stmt to 0
   [0x00000ce7]  Copy (view 1)
   [0x00000ce8]  Set column to 5
   [0x00000cea]  Set is_stmt to 1
-  [0x00000ceb]  Special opcode 62: advance Address by 4 to 0x2a05 and Line by 1 to 422
+  [0x00000ceb]  Special opcode 62: advance Address by 4 to 0x2a05 and Line by 1 to 435
   [0x00000cec]  Set column to 12
   [0x00000cee]  Set is_stmt to 0
   [0x00000cef]  Copy (view 1)
   [0x00000cf0]  Set column to 1
-  [0x00000cf2]  Special opcode 34: advance Address by 2 to 0x2a07 and Line by 1 to 423
-  [0x00000cf3]  Special opcode 61: advance Address by 4 to 0x2a0b and Line by 0 to 423
+  [0x00000cf2]  Special opcode 34: advance Address by 2 to 0x2a07 and Line by 1 to 436
+  [0x00000cf3]  Special opcode 61: advance Address by 4 to 0x2a0b and Line by 0 to 436
   [0x00000cf4]  Set File Name to entry 2 in the File Name Table
   [0x00000cf6]  Set column to 9
   [0x00000cf8]  Set is_stmt to 1
-  [0x00000cf9]  Advance Line by 115 to 538
+  [0x00000cf9]  Advance Line by 102 to 538
   [0x00000cfc]  Special opcode 75: advance Address by 5 to 0x2a10 and Line by 0 to 538
   [0x00000cfd]  Set is_stmt to 0
   [0x00000cfe]  Special opcode 145: advance Address by 10 to 0x2a1a and Line by 0 to 538
   [0x00000cff]  Set File Name to entry 1 in the File Name Table
   [0x00000d01]  Set is_stmt to 1
-  [0x00000d02]  Advance Line by -130 to 408
+  [0x00000d02]  Advance Line by -117 to 421
   [0x00000d05]  Copy (view 1)
   [0x00000d06]  Copy (view 2)
   [0x00000d07]  Set File Name to entry 2 in the File Name Table
   [0x00000d09]  Set column to 20
-  [0x00000d0b]  Advance Line by 125 to 533
+  [0x00000d0b]  Advance Line by 112 to 533
   [0x00000d0e]  Copy (view 3)
   [0x00000d0f]  Set column to 5
   [0x00000d11]  Special opcode 9: advance Address by 0 to 0x2a1a and Line by 4 to 537 (view 4)
   [0x00000d12]  Set column to 9
   [0x00000d14]  Set is_stmt to 0
   [0x00000d15]  Copy (view 5)
   [0x00000d16]  Set column to 8
@@ -1356,72 +1356,72 @@
   [0x00000d19]  Set column to 9
   [0x00000d1b]  Set is_stmt to 1
   [0x00000d1c]  Special opcode 90: advance Address by 6 to 0x2a24 and Line by 1 to 538
   [0x00000d1d]  Set is_stmt to 0
   [0x00000d1e]  Special opcode 173: advance Address by 12 to 0x2a30 and Line by 0 to 538
   [0x00000d1f]  Set File Name to entry 1 in the File Name Table
   [0x00000d21]  Set column to 16
-  [0x00000d23]  Advance Line by -129 to 409
+  [0x00000d23]  Advance Line by -116 to 422
   [0x00000d26]  Copy (view 1)
   [0x00000d27]  Set column to 1
   [0x00000d29]  Set is_stmt to 1
-  [0x00000d2a]  Advance Line by -95 to 314
-  [0x00000d2d]  Special opcode 229: advance Address by 16 to 0x2a40 and Line by 0 to 314
+  [0x00000d2a]  Advance Line by -95 to 327
+  [0x00000d2d]  Special opcode 229: advance Address by 16 to 0x2a40 and Line by 0 to 327
   [0x00000d2e]  Set column to 5
-  [0x00000d30]  Special opcode 6: advance Address by 0 to 0x2a40 and Line by 1 to 315 (view 1)
+  [0x00000d30]  Special opcode 6: advance Address by 0 to 0x2a40 and Line by 1 to 328 (view 1)
   [0x00000d31]  Set File Name to entry 2 in the File Name Table
-  [0x00000d33]  Advance Line by -182 to 133
+  [0x00000d33]  Advance Line by -195 to 133
   [0x00000d36]  Copy (view 2)
   [0x00000d37]  Set File Name to entry 1 in the File Name Table
   [0x00000d39]  Set column to 1
   [0x00000d3b]  Set is_stmt to 0
-  [0x00000d3c]  Advance Line by 181 to 314
+  [0x00000d3c]  Advance Line by 194 to 327
   [0x00000d3f]  Copy (view 3)
   [0x00000d40]  Set column to 31
   [0x00000d42]  Advance PC by constant 17 to 0x2a51
-  [0x00000d43]  Special opcode 6: advance Address by 0 to 0x2a51 and Line by 1 to 315
-  [0x00000d44]  Special opcode 61: advance Address by 4 to 0x2a55 and Line by 0 to 315
+  [0x00000d43]  Special opcode 6: advance Address by 0 to 0x2a51 and Line by 1 to 328
+  [0x00000d44]  Special opcode 61: advance Address by 4 to 0x2a55 and Line by 0 to 328
   [0x00000d45]  Set column to 5
   [0x00000d47]  Set is_stmt to 1
-  [0x00000d48]  Special opcode 76: advance Address by 5 to 0x2a5a and Line by 1 to 316
+  [0x00000d48]  Special opcode 76: advance Address by 5 to 0x2a5a and Line by 1 to 329
   [0x00000d49]  Set column to 8
   [0x00000d4b]  Set is_stmt to 0
   [0x00000d4c]  Copy (view 1)
   [0x00000d4d]  Set column to 5
   [0x00000d4f]  Set is_stmt to 1
-  [0x00000d50]  Special opcode 134: advance Address by 9 to 0x2a63 and Line by 3 to 319
-  [0x00000d51]  Special opcode 6: advance Address by 0 to 0x2a63 and Line by 1 to 320 (view 1)
+  [0x00000d50]  Special opcode 134: advance Address by 9 to 0x2a63 and Line by 3 to 332
+  [0x00000d51]  Special opcode 6: advance Address by 0 to 0x2a63 and Line by 1 to 333 (view 1)
   [0x00000d52]  Set column to 19
   [0x00000d54]  Set is_stmt to 0
   [0x00000d55]  Copy (view 2)
   [0x00000d56]  Set column to 5
   [0x00000d58]  Set is_stmt to 1
-  [0x00000d59]  Special opcode 62: advance Address by 4 to 0x2a67 and Line by 1 to 321
+  [0x00000d59]  Special opcode 62: advance Address by 4 to 0x2a67 and Line by 1 to 334
   [0x00000d5a]  Set File Name to entry 2 in the File Name Table
   [0x00000d5c]  Set column to 19
-  [0x00000d5e]  Advance Line by -172 to 149
+  [0x00000d5e]  Advance Line by -185 to 149
   [0x00000d61]  Copy (view 1)
   [0x00000d62]  Set column to 5
   [0x00000d64]  Special opcode 6: advance Address by 0 to 0x2a67 and Line by 1 to 150 (view 2)
   [0x00000d65]  Set is_stmt to 0
   [0x00000d66]  Copy (view 3)
   [0x00000d67]  Set is_stmt to 1
   [0x00000d68]  Advance Line by -17 to 133
   [0x00000d6a]  Copy (view 4)
   [0x00000d6b]  Set File Name to entry 1 in the File Name Table
   [0x00000d6d]  Set column to 8
   [0x00000d6f]  Set is_stmt to 0
-  [0x00000d70]  Advance Line by 188 to 321
+  [0x00000d70]  Advance Line by 201 to 334
   [0x00000d73]  Copy (view 5)
   [0x00000d74]  Set column to 9
   [0x00000d76]  Set is_stmt to 1
-  [0x00000d77]  Special opcode 104: advance Address by 7 to 0x2a6e and Line by 1 to 322
+  [0x00000d77]  Special opcode 104: advance Address by 7 to 0x2a6e and Line by 1 to 335
   [0x00000d78]  Set File Name to entry 2 in the File Name Table
   [0x00000d7a]  Set column to 25
-  [0x00000d7c]  Advance Line by 294 to 616
+  [0x00000d7c]  Advance Line by 281 to 616
   [0x00000d7f]  Copy (view 1)
   [0x00000d80]  Set column to 5
   [0x00000d82]  Special opcode 7: advance Address by 0 to 0x2a6e and Line by 2 to 618 (view 2)
   [0x00000d83]  Set column to 20
   [0x00000d85]  Advance Line by -127 to 491
   [0x00000d88]  Copy (view 3)
   [0x00000d89]  Set column to 5
@@ -1434,137 +1434,137 @@
   [0x00000d93]  Set column to 5
   [0x00000d95]  Set is_stmt to 1
   [0x00000d96]  Advance Line by 117 to 619
   [0x00000d99]  Special opcode 61: advance Address by 4 to 0x2a79 and Line by 0 to 619
   [0x00000d9a]  Set File Name to entry 1 in the File Name Table
   [0x00000d9c]  Set column to 1
   [0x00000d9e]  Set is_stmt to 0
-  [0x00000d9f]  Advance Line by -271 to 348
+  [0x00000d9f]  Advance Line by -258 to 361
   [0x00000da2]  Copy (view 1)
-  [0x00000da3]  Special opcode 33: advance Address by 2 to 0x2a7b and Line by 0 to 348
-  [0x00000da4]  Special opcode 33: advance Address by 2 to 0x2a7d and Line by 0 to 348
-  [0x00000da5]  Special opcode 33: advance Address by 2 to 0x2a7f and Line by 0 to 348
-  [0x00000da6]  Special opcode 33: advance Address by 2 to 0x2a81 and Line by 0 to 348
+  [0x00000da3]  Special opcode 33: advance Address by 2 to 0x2a7b and Line by 0 to 361
+  [0x00000da4]  Special opcode 33: advance Address by 2 to 0x2a7d and Line by 0 to 361
+  [0x00000da5]  Special opcode 33: advance Address by 2 to 0x2a7f and Line by 0 to 361
+  [0x00000da6]  Special opcode 33: advance Address by 2 to 0x2a81 and Line by 0 to 361
   [0x00000da7]  Set column to 15
-  [0x00000da9]  Advance Line by -29 to 319
-  [0x00000dab]  Special opcode 103: advance Address by 7 to 0x2a88 and Line by 0 to 319
+  [0x00000da9]  Advance Line by -29 to 332
+  [0x00000dab]  Special opcode 103: advance Address by 7 to 0x2a88 and Line by 0 to 332
   [0x00000dac]  Set column to 11
   [0x00000dae]  Set is_stmt to 1
-  [0x00000daf]  Special opcode 68: advance Address by 4 to 0x2a8c and Line by 7 to 326
+  [0x00000daf]  Special opcode 68: advance Address by 4 to 0x2a8c and Line by 7 to 339
   [0x00000db0]  Set File Name to entry 2 in the File Name Table
   [0x00000db2]  Set column to 19
-  [0x00000db4]  Advance Line by -177 to 149
+  [0x00000db4]  Advance Line by -190 to 149
   [0x00000db7]  Copy (view 1)
   [0x00000db8]  Set column to 5
   [0x00000dba]  Special opcode 6: advance Address by 0 to 0x2a8c and Line by 1 to 150 (view 2)
   [0x00000dbb]  Set is_stmt to 0
   [0x00000dbc]  Copy (view 3)
   [0x00000dbd]  Set is_stmt to 1
   [0x00000dbe]  Advance Line by -17 to 133
   [0x00000dc0]  Copy (view 4)
   [0x00000dc1]  Set File Name to entry 1 in the File Name Table
   [0x00000dc3]  Set column to 11
   [0x00000dc5]  Set is_stmt to 0
-  [0x00000dc6]  Advance Line by 193 to 326
+  [0x00000dc6]  Advance Line by 206 to 339
   [0x00000dc9]  Copy (view 5)
   [0x00000dca]  Set column to 9
   [0x00000dcc]  Set is_stmt to 1
-  [0x00000dcd]  Special opcode 174: advance Address by 12 to 0x2a98 and Line by 1 to 327
+  [0x00000dcd]  Special opcode 174: advance Address by 12 to 0x2a98 and Line by 1 to 340
   [0x00000dce]  Set column to 19
   [0x00000dd0]  Set is_stmt to 0
   [0x00000dd1]  Copy (view 1)
   [0x00000dd2]  Set column to 9
   [0x00000dd4]  Set is_stmt to 1
   [0x00000dd5]  Advance PC by constant 17 to 0x2aa9
-  [0x00000dd6]  Special opcode 6: advance Address by 0 to 0x2aa9 and Line by 1 to 328
+  [0x00000dd6]  Special opcode 6: advance Address by 0 to 0x2aa9 and Line by 1 to 341
   [0x00000dd7]  Set column to 12
   [0x00000dd9]  Set is_stmt to 0
   [0x00000dda]  Copy (view 1)
   [0x00000ddb]  Set column to 14
   [0x00000ddd]  Set is_stmt to 1
-  [0x00000dde]  Special opcode 63: advance Address by 4 to 0x2aad and Line by 2 to 330
+  [0x00000dde]  Special opcode 63: advance Address by 4 to 0x2aad and Line by 2 to 343
   [0x00000ddf]  Set column to 17
   [0x00000de1]  Set is_stmt to 0
   [0x00000de2]  Copy (view 1)
   [0x00000de3]  Set column to 14
   [0x00000de5]  Set is_stmt to 1
-  [0x00000de6]  Special opcode 119: advance Address by 8 to 0x2ab5 and Line by 2 to 332
+  [0x00000de6]  Special opcode 119: advance Address by 8 to 0x2ab5 and Line by 2 to 345
   [0x00000de7]  Set column to 17
   [0x00000de9]  Set is_stmt to 0
   [0x00000dea]  Copy (view 1)
   [0x00000deb]  Set column to 13
   [0x00000ded]  Set is_stmt to 1
-  [0x00000dee]  Special opcode 148: advance Address by 10 to 0x2abf and Line by 3 to 335
+  [0x00000dee]  Special opcode 148: advance Address by 10 to 0x2abf and Line by 3 to 348
   [0x00000def]  Set column to 18
   [0x00000df1]  Set is_stmt to 0
   [0x00000df2]  Copy (view 1)
   [0x00000df3]  Set column to 13
   [0x00000df5]  Set is_stmt to 1
-  [0x00000df6]  Special opcode 62: advance Address by 4 to 0x2ac3 and Line by 1 to 336
+  [0x00000df6]  Special opcode 62: advance Address by 4 to 0x2ac3 and Line by 1 to 349
   [0x00000df7]  Set column to 18
   [0x00000df9]  Set is_stmt to 0
   [0x00000dfa]  Copy (view 1)
-  [0x00000dfb]  Special opcode 75: advance Address by 5 to 0x2ac8 and Line by 0 to 336
+  [0x00000dfb]  Special opcode 75: advance Address by 5 to 0x2ac8 and Line by 0 to 349
   [0x00000dfc]  Set column to 11
   [0x00000dfe]  Set is_stmt to 1
-  [0x00000dff]  Advance Line by -10 to 326
+  [0x00000dff]  Advance Line by -10 to 339
   [0x00000e01]  Copy (view 1)
   [0x00000e02]  Set File Name to entry 2 in the File Name Table
   [0x00000e04]  Set column to 19
-  [0x00000e06]  Advance Line by -177 to 149
+  [0x00000e06]  Advance Line by -190 to 149
   [0x00000e09]  Copy (view 2)
   [0x00000e0a]  Set column to 5
   [0x00000e0c]  Special opcode 6: advance Address by 0 to 0x2ac8 and Line by 1 to 150 (view 3)
   [0x00000e0d]  Set is_stmt to 0
   [0x00000e0e]  Copy (view 4)
   [0x00000e0f]  Set is_stmt to 1
   [0x00000e10]  Advance Line by -17 to 133
   [0x00000e12]  Copy (view 5)
   [0x00000e13]  Set File Name to entry 1 in the File Name Table
   [0x00000e15]  Set column to 11
   [0x00000e17]  Set is_stmt to 0
-  [0x00000e18]  Advance Line by 193 to 326
+  [0x00000e18]  Advance Line by 206 to 339
   [0x00000e1b]  Copy (view 6)
   [0x00000e1c]  Set File Name to entry 2 in the File Name Table
   [0x00000e1e]  Set column to 19
   [0x00000e20]  Set is_stmt to 1
-  [0x00000e21]  Advance Line by -177 to 149
+  [0x00000e21]  Advance Line by -190 to 149
   [0x00000e24]  Special opcode 89: advance Address by 6 to 0x2ace and Line by 0 to 149
   [0x00000e25]  Set column to 5
   [0x00000e27]  Special opcode 6: advance Address by 0 to 0x2ace and Line by 1 to 150 (view 1)
   [0x00000e28]  Set is_stmt to 0
   [0x00000e29]  Copy (view 2)
   [0x00000e2a]  Set is_stmt to 1
   [0x00000e2b]  Advance Line by -17 to 133
   [0x00000e2d]  Copy (view 3)
   [0x00000e2e]  Set File Name to entry 1 in the File Name Table
   [0x00000e30]  Set column to 35
   [0x00000e32]  Set is_stmt to 0
-  [0x00000e33]  Advance Line by 193 to 326
+  [0x00000e33]  Advance Line by 206 to 339
   [0x00000e36]  Copy (view 4)
   [0x00000e37]  Set column to 5
   [0x00000e39]  Set is_stmt to 1
-  [0x00000e3a]  Advance Line by 14 to 340
-  [0x00000e3c]  Special opcode 103: advance Address by 7 to 0x2ad5 and Line by 0 to 340
+  [0x00000e3a]  Advance Line by 14 to 353
+  [0x00000e3c]  Special opcode 103: advance Address by 7 to 0x2ad5 and Line by 0 to 353
   [0x00000e3d]  Set column to 8
   [0x00000e3f]  Set is_stmt to 0
   [0x00000e40]  Copy (view 1)
-  [0x00000e41]  Special opcode 75: advance Address by 5 to 0x2ada and Line by 0 to 340
+  [0x00000e41]  Special opcode 75: advance Address by 5 to 0x2ada and Line by 0 to 353
   [0x00000e42]  Set column to 9
   [0x00000e44]  Set is_stmt to 1
-  [0x00000e45]  Special opcode 77: advance Address by 5 to 0x2adf and Line by 2 to 342
+  [0x00000e45]  Special opcode 77: advance Address by 5 to 0x2adf and Line by 2 to 355
   [0x00000e46]  Set column to 12
   [0x00000e48]  Set is_stmt to 0
   [0x00000e49]  Copy (view 1)
   [0x00000e4a]  Set column to 13
   [0x00000e4c]  Set is_stmt to 1
-  [0x00000e4d]  Special opcode 92: advance Address by 6 to 0x2ae5 and Line by 3 to 345
+  [0x00000e4d]  Special opcode 92: advance Address by 6 to 0x2ae5 and Line by 3 to 358
   [0x00000e4e]  Set File Name to entry 2 in the File Name Table
   [0x00000e50]  Set column to 25
-  [0x00000e52]  Advance Line by 271 to 616
+  [0x00000e52]  Advance Line by 258 to 616
   [0x00000e55]  Copy (view 1)
   [0x00000e56]  Set column to 5
   [0x00000e58]  Special opcode 7: advance Address by 0 to 0x2ae5 and Line by 2 to 618 (view 2)
   [0x00000e59]  Set column to 20
   [0x00000e5b]  Advance Line by -127 to 491
   [0x00000e5e]  Copy (view 3)
   [0x00000e5f]  Set column to 5
@@ -1576,34 +1576,34 @@
   [0x00000e68]  Set column to 5
   [0x00000e6a]  Set is_stmt to 1
   [0x00000e6b]  Advance Line by 117 to 619
   [0x00000e6e]  Special opcode 159: advance Address by 11 to 0x2af0 and Line by 0 to 619
   [0x00000e6f]  Set File Name to entry 1 in the File Name Table
   [0x00000e71]  Set column to 1
   [0x00000e73]  Set is_stmt to 0
-  [0x00000e74]  Advance Line by -271 to 348
+  [0x00000e74]  Advance Line by -258 to 361
   [0x00000e77]  Copy (view 1)
-  [0x00000e78]  Special opcode 33: advance Address by 2 to 0x2af2 and Line by 0 to 348
-  [0x00000e79]  Special opcode 33: advance Address by 2 to 0x2af4 and Line by 0 to 348
-  [0x00000e7a]  Special opcode 33: advance Address by 2 to 0x2af6 and Line by 0 to 348
-  [0x00000e7b]  Special opcode 33: advance Address by 2 to 0x2af8 and Line by 0 to 348
-  [0x00000e7c]  Special opcode 117: advance Address by 8 to 0x2b00 and Line by 0 to 348
+  [0x00000e78]  Special opcode 33: advance Address by 2 to 0x2af2 and Line by 0 to 361
+  [0x00000e79]  Special opcode 33: advance Address by 2 to 0x2af4 and Line by 0 to 361
+  [0x00000e7a]  Special opcode 33: advance Address by 2 to 0x2af6 and Line by 0 to 361
+  [0x00000e7b]  Special opcode 33: advance Address by 2 to 0x2af8 and Line by 0 to 361
+  [0x00000e7c]  Special opcode 117: advance Address by 8 to 0x2b00 and Line by 0 to 361
   [0x00000e7d]  Set column to 16
-  [0x00000e7f]  Advance Line by -31 to 317
-  [0x00000e81]  Special opcode 19: advance Address by 1 to 0x2b01 and Line by 0 to 317
+  [0x00000e7f]  Advance Line by -31 to 330
+  [0x00000e81]  Special opcode 19: advance Address by 1 to 0x2b01 and Line by 0 to 330
   [0x00000e82]  Set column to 1
-  [0x00000e84]  Advance Line by 31 to 348
-  [0x00000e86]  Special opcode 33: advance Address by 2 to 0x2b03 and Line by 0 to 348
-  [0x00000e87]  Special opcode 75: advance Address by 5 to 0x2b08 and Line by 0 to 348
+  [0x00000e84]  Advance Line by 31 to 361
+  [0x00000e86]  Special opcode 33: advance Address by 2 to 0x2b03 and Line by 0 to 361
+  [0x00000e87]  Special opcode 75: advance Address by 5 to 0x2b08 and Line by 0 to 361
   [0x00000e88]  Set column to 13
   [0x00000e8a]  Set is_stmt to 1
-  [0x00000e8b]  Special opcode 112: advance Address by 8 to 0x2b10 and Line by -5 to 343
+  [0x00000e8b]  Special opcode 112: advance Address by 8 to 0x2b10 and Line by -5 to 356
   [0x00000e8c]  Set File Name to entry 2 in the File Name Table
   [0x00000e8e]  Set column to 25
-  [0x00000e90]  Advance Line by 273 to 616
+  [0x00000e90]  Advance Line by 260 to 616
   [0x00000e93]  Copy (view 1)
   [0x00000e94]  Set column to 5
   [0x00000e96]  Special opcode 7: advance Address by 0 to 0x2b10 and Line by 2 to 618 (view 2)
   [0x00000e97]  Set column to 20
   [0x00000e99]  Advance Line by -127 to 491
   [0x00000e9c]  Copy (view 3)
   [0x00000e9d]  Set column to 5
@@ -1615,40 +1615,40 @@
   [0x00000ea6]  Set column to 5
   [0x00000ea8]  Set is_stmt to 1
   [0x00000ea9]  Advance Line by 117 to 619
   [0x00000eac]  Special opcode 159: advance Address by 11 to 0x2b1b and Line by 0 to 619
   [0x00000ead]  Set File Name to entry 1 in the File Name Table
   [0x00000eaf]  Set column to 1
   [0x00000eb1]  Set is_stmt to 0
-  [0x00000eb2]  Advance Line by -271 to 348
+  [0x00000eb2]  Advance Line by -258 to 361
   [0x00000eb5]  Copy (view 1)
-  [0x00000eb6]  Special opcode 33: advance Address by 2 to 0x2b1d and Line by 0 to 348
-  [0x00000eb7]  Special opcode 33: advance Address by 2 to 0x2b1f and Line by 0 to 348
-  [0x00000eb8]  Special opcode 33: advance Address by 2 to 0x2b21 and Line by 0 to 348
-  [0x00000eb9]  Special opcode 33: advance Address by 2 to 0x2b23 and Line by 0 to 348
+  [0x00000eb6]  Special opcode 33: advance Address by 2 to 0x2b1d and Line by 0 to 361
+  [0x00000eb7]  Special opcode 33: advance Address by 2 to 0x2b1f and Line by 0 to 361
+  [0x00000eb8]  Special opcode 33: advance Address by 2 to 0x2b21 and Line by 0 to 361
+  [0x00000eb9]  Special opcode 33: advance Address by 2 to 0x2b23 and Line by 0 to 361
   [0x00000eba]  Set column to 5
   [0x00000ebc]  Set is_stmt to 1
-  [0x00000ebd]  Special opcode 74: advance Address by 5 to 0x2b28 and Line by -1 to 347
+  [0x00000ebd]  Special opcode 74: advance Address by 5 to 0x2b28 and Line by -1 to 360
   [0x00000ebe]  Set column to 1
   [0x00000ec0]  Set is_stmt to 0
-  [0x00000ec1]  Special opcode 6: advance Address by 0 to 0x2b28 and Line by 1 to 348 (view 1)
+  [0x00000ec1]  Special opcode 6: advance Address by 0 to 0x2b28 and Line by 1 to 361 (view 1)
   [0x00000ec2]  Set column to 12
-  [0x00000ec4]  Special opcode 18: advance Address by 1 to 0x2b29 and Line by -1 to 347
+  [0x00000ec4]  Special opcode 18: advance Address by 1 to 0x2b29 and Line by -1 to 360
   [0x00000ec5]  Set column to 1
-  [0x00000ec7]  Special opcode 132: advance Address by 9 to 0x2b32 and Line by 1 to 348
-  [0x00000ec8]  Special opcode 19: advance Address by 1 to 0x2b33 and Line by 0 to 348
-  [0x00000ec9]  Special opcode 33: advance Address by 2 to 0x2b35 and Line by 0 to 348
-  [0x00000eca]  Special opcode 33: advance Address by 2 to 0x2b37 and Line by 0 to 348
+  [0x00000ec7]  Special opcode 132: advance Address by 9 to 0x2b32 and Line by 1 to 361
+  [0x00000ec8]  Special opcode 19: advance Address by 1 to 0x2b33 and Line by 0 to 361
+  [0x00000ec9]  Special opcode 33: advance Address by 2 to 0x2b35 and Line by 0 to 361
+  [0x00000eca]  Special opcode 33: advance Address by 2 to 0x2b37 and Line by 0 to 361
   [0x00000ecb]  Set column to 12
-  [0x00000ecd]  Special opcode 32: advance Address by 2 to 0x2b39 and Line by -1 to 347
-  [0x00000ece]  Special opcode 75: advance Address by 5 to 0x2b3e and Line by 0 to 347
+  [0x00000ecd]  Special opcode 32: advance Address by 2 to 0x2b39 and Line by -1 to 360
+  [0x00000ece]  Special opcode 75: advance Address by 5 to 0x2b3e and Line by 0 to 360
   [0x00000ecf]  Set column to 1
   [0x00000ed1]  Set is_stmt to 1
   [0x00000ed2]  Extended opcode 2: set Address to 0x2b40
-  [0x00000edd]  Advance Line by -207 to 140
+  [0x00000edd]  Advance Line by -220 to 140
   [0x00000ee0]  Copy
   [0x00000ee1]  Set column to 5
   [0x00000ee3]  Special opcode 6: advance Address by 0 to 0x2b40 and Line by 1 to 141 (view 1)
   [0x00000ee4]  Copy (view 2)
   [0x00000ee5]  Set column to 1
   [0x00000ee7]  Set is_stmt to 0
   [0x00000ee8]  Special opcode 4: advance Address by 0 to 0x2b40 and Line by -1 to 140 (view 3)
@@ -1723,86 +1723,86 @@
   [0x00000f5a]  Special opcode 145: advance Address by 10 to 0x2b90 and Line by 0 to 143
   [0x00000f5b]  Set column to 1
   [0x00000f5d]  Special opcode 7: advance Address by 0 to 0x2b90 and Line by 2 to 145 (view 1)
   [0x00000f5e]  Special opcode 19: advance Address by 1 to 0x2b91 and Line by 0 to 145
   [0x00000f5f]  Special opcode 19: advance Address by 1 to 0x2b92 and Line by 0 to 145
   [0x00000f60]  Special opcode 33: advance Address by 2 to 0x2b94 and Line by 0 to 145
   [0x00000f61]  Set is_stmt to 1
-  [0x00000f62]  Advance Line by 76 to 221
-  [0x00000f65]  Special opcode 173: advance Address by 12 to 0x2ba0 and Line by 0 to 221
+  [0x00000f62]  Advance Line by 89 to 234
+  [0x00000f65]  Special opcode 173: advance Address by 12 to 0x2ba0 and Line by 0 to 234
   [0x00000f66]  Set column to 5
-  [0x00000f68]  Special opcode 6: advance Address by 0 to 0x2ba0 and Line by 1 to 222 (view 1)
+  [0x00000f68]  Special opcode 6: advance Address by 0 to 0x2ba0 and Line by 1 to 235 (view 1)
   [0x00000f69]  Set column to 1
   [0x00000f6b]  Set is_stmt to 0
-  [0x00000f6c]  Special opcode 4: advance Address by 0 to 0x2ba0 and Line by -1 to 221 (view 2)
+  [0x00000f6c]  Special opcode 4: advance Address by 0 to 0x2ba0 and Line by -1 to 234 (view 2)
   [0x00000f6d]  Set column to 8
-  [0x00000f6f]  Special opcode 20: advance Address by 1 to 0x2ba1 and Line by 1 to 222
+  [0x00000f6f]  Special opcode 20: advance Address by 1 to 0x2ba1 and Line by 1 to 235
   [0x00000f70]  Set column to 10
   [0x00000f72]  Set is_stmt to 1
-  [0x00000f73]  Special opcode 121: advance Address by 8 to 0x2ba9 and Line by 4 to 226
+  [0x00000f73]  Special opcode 121: advance Address by 8 to 0x2ba9 and Line by 4 to 239
   [0x00000f74]  Set column to 15
   [0x00000f76]  Set is_stmt to 0
   [0x00000f77]  Copy (view 1)
   [0x00000f78]  Set column to 13
-  [0x00000f7a]  Special opcode 61: advance Address by 4 to 0x2bad and Line by 0 to 226
+  [0x00000f7a]  Special opcode 61: advance Address by 4 to 0x2bad and Line by 0 to 239
   [0x00000f7b]  Set column to 5
   [0x00000f7d]  Set is_stmt to 1
-  [0x00000f7e]  Special opcode 66: advance Address by 4 to 0x2bb1 and Line by 5 to 231
+  [0x00000f7e]  Special opcode 66: advance Address by 4 to 0x2bb1 and Line by 5 to 244
   [0x00000f7f]  Set column to 22
   [0x00000f81]  Set is_stmt to 0
   [0x00000f82]  Copy (view 1)
   [0x00000f83]  Set column to 5
   [0x00000f85]  Set is_stmt to 1
-  [0x00000f86]  Special opcode 76: advance Address by 5 to 0x2bb6 and Line by 1 to 232
-  [0x00000f87]  Special opcode 6: advance Address by 0 to 0x2bb6 and Line by 1 to 233 (view 1)
+  [0x00000f86]  Special opcode 76: advance Address by 5 to 0x2bb6 and Line by 1 to 245
+  [0x00000f87]  Special opcode 6: advance Address by 0 to 0x2bb6 and Line by 1 to 246 (view 1)
   [0x00000f88]  Set column to 10
   [0x00000f8a]  Copy (view 2)
   [0x00000f8b]  Set column to 28
   [0x00000f8d]  Copy (view 3)
   [0x00000f8e]  Set column to 32
   [0x00000f90]  Set is_stmt to 0
   [0x00000f91]  Copy (view 4)
   [0x00000f92]  Set column to 5
-  [0x00000f94]  Special opcode 61: advance Address by 4 to 0x2bba and Line by 0 to 233
+  [0x00000f94]  Special opcode 61: advance Address by 4 to 0x2bba and Line by 0 to 246
   [0x00000f95]  Set column to 9
   [0x00000f97]  Extended opcode 4: set Discriminator to 3
   [0x00000f9b]  Set is_stmt to 1
   [0x00000f9c]  Advance PC by constant 17 to 0x2bcb
-  [0x00000f9d]  Special opcode 76: advance Address by 5 to 0x2bd0 and Line by 1 to 234
+  [0x00000f9d]  Special opcode 76: advance Address by 5 to 0x2bd0 and Line by 1 to 247
   [0x00000f9e]  Set column to 14
   [0x00000fa0]  Extended opcode 4: set Discriminator to 3
   [0x00000fa4]  Set is_stmt to 0
   [0x00000fa5]  Copy (view 1)
   [0x00000fa6]  Set column to 9
   [0x00000fa8]  Extended opcode 4: set Discriminator to 3
   [0x00000fac]  Set is_stmt to 1
-  [0x00000fad]  Special opcode 62: advance Address by 4 to 0x2bd4 and Line by 1 to 235
+  [0x00000fad]  Special opcode 62: advance Address by 4 to 0x2bd4 and Line by 1 to 248
   [0x00000fae]  Set File Name to entry 2 in the File Name Table
   [0x00000fb0]  Set column to 20
   [0x00000fb2]  Extended opcode 4: set Discriminator to 3
-  [0x00000fb6]  Advance Line by 256 to 491
+  [0x00000fb6]  Advance Line by 243 to 491
   [0x00000fb9]  Copy (view 1)
   [0x00000fba]  Set column to 5
   [0x00000fbc]  Extended opcode 4: set Discriminator to 3
   [0x00000fc0]  Advance Line by 11 to 502
   [0x00000fc2]  Copy (view 2)
   [0x00000fc3]  Set column to 18
   [0x00000fc5]  Extended opcode 4: set Discriminator to 3
   [0x00000fc9]  Set is_stmt to 0
   [0x00000fca]  Special opcode 61: advance Address by 4 to 0x2bd8 and Line by 0 to 502
   [0x00000fcb]  Set File Name to entry 1 in the File Name Table
   [0x00000fcd]  Set column to 9
   [0x00000fcf]  Extended opcode 4: set Discriminator to 3
   [0x00000fd3]  Set is_stmt to 1
-  [0x00000fd4]  Advance Line by -266 to 236
-  [0x00000fd7]  Special opcode 61: advance Address by 4 to 0x2bdc and Line by 0 to 236
+  [0x00000fd4]  Advance Line by -253 to 249
+  [0x00000fd7]  Special opcode 61: advance Address by 4 to 0x2bdc and Line by 0 to 249
   [0x00000fd8]  Set File Name to entry 4 in the File Name Table
   [0x00000fda]  Set column to 1
   [0x00000fdc]  Extended opcode 4: set Discriminator to 3
-  [0x00000fe0]  Advance Line by -192 to 44
+  [0x00000fe0]  Advance Line by -205 to 44
   [0x00000fe3]  Copy (view 1)
   [0x00000fe4]  Set column to 5
   [0x00000fe6]  Extended opcode 4: set Discriminator to 3
   [0x00000fea]  Special opcode 6: advance Address by 0 to 0x2bdc and Line by 1 to 45 (view 2)
   [0x00000feb]  Extended opcode 4: set Discriminator to 3
   [0x00000fef]  Special opcode 6: advance Address by 0 to 0x2bdc and Line by 1 to 46 (view 3)
   [0x00000ff0]  Set column to 26
@@ -1811,65 +1811,65 @@
   [0x00000ff7]  Copy (view 4)
   [0x00000ff8]  Extended opcode 4: set Discriminator to 3
   [0x00000ffc]  Special opcode 61: advance Address by 4 to 0x2be0 and Line by 0 to 46
   [0x00000ffd]  Set File Name to entry 1 in the File Name Table
   [0x00000fff]  Set column to 48
   [0x00001001]  Extended opcode 4: set Discriminator to 3
   [0x00001005]  Set is_stmt to 1
-  [0x00001006]  Advance Line by 187 to 233
+  [0x00001006]  Advance Line by 200 to 246
   [0x00001009]  Copy (view 1)
   [0x0000100a]  Set column to 58
   [0x0000100c]  Extended opcode 4: set Discriminator to 3
   [0x00001010]  Set is_stmt to 0
   [0x00001011]  Copy (view 2)
   [0x00001012]  Set column to 28
   [0x00001014]  Extended opcode 4: set Discriminator to 3
   [0x00001018]  Set is_stmt to 1
-  [0x00001019]  Special opcode 61: advance Address by 4 to 0x2be4 and Line by 0 to 233
+  [0x00001019]  Special opcode 61: advance Address by 4 to 0x2be4 and Line by 0 to 246
   [0x0000101a]  Set column to 5
   [0x0000101c]  Extended opcode 4: set Discriminator to 3
   [0x00001020]  Set is_stmt to 0
   [0x00001021]  Copy (view 1)
   [0x00001022]  Extended opcode 4: set Discriminator to 3
-  [0x00001026]  Special opcode 75: advance Address by 5 to 0x2be9 and Line by 0 to 233
+  [0x00001026]  Special opcode 75: advance Address by 5 to 0x2be9 and Line by 0 to 246
   [0x00001027]  Set column to 1
-  [0x00001029]  Special opcode 11: advance Address by 0 to 0x2be9 and Line by 6 to 239 (view 1)
-  [0x0000102a]  Special opcode 19: advance Address by 1 to 0x2bea and Line by 0 to 239
+  [0x00001029]  Special opcode 11: advance Address by 0 to 0x2be9 and Line by 6 to 252 (view 1)
+  [0x0000102a]  Special opcode 19: advance Address by 1 to 0x2bea and Line by 0 to 252
   [0x0000102b]  Set column to 9
   [0x0000102d]  Set is_stmt to 1
-  [0x0000102e]  Advance Line by -12 to 227
-  [0x00001030]  Special opcode 89: advance Address by 6 to 0x2bf0 and Line by 0 to 227
+  [0x0000102e]  Advance Line by -12 to 240
+  [0x00001030]  Special opcode 89: advance Address by 6 to 0x2bf0 and Line by 0 to 240
   [0x00001031]  Set is_stmt to 0
-  [0x00001032]  Special opcode 201: advance Address by 14 to 0x2bfe and Line by 0 to 227
+  [0x00001032]  Special opcode 201: advance Address by 14 to 0x2bfe and Line by 0 to 240
   [0x00001033]  Set is_stmt to 1
-  [0x00001034]  Special opcode 118: advance Address by 8 to 0x2c06 and Line by 1 to 228
+  [0x00001034]  Special opcode 118: advance Address by 8 to 0x2c06 and Line by 1 to 241
   [0x00001035]  Set column to 16
   [0x00001037]  Set is_stmt to 0
   [0x00001038]  Copy (view 1)
   [0x00001039]  Set column to 1
-  [0x0000103b]  Advance Line by 11 to 239
-  [0x0000103d]  Special opcode 33: advance Address by 2 to 0x2c08 and Line by 0 to 239
-  [0x0000103e]  Special opcode 19: advance Address by 1 to 0x2c09 and Line by 0 to 239
+  [0x0000103b]  Advance Line by 11 to 252
+  [0x0000103d]  Special opcode 33: advance Address by 2 to 0x2c08 and Line by 0 to 252
+  [0x0000103e]  Special opcode 19: advance Address by 1 to 0x2c09 and Line by 0 to 252
   [0x0000103f]  Set is_stmt to 1
-  [0x00001040]  Advance Line by -20 to 219
-  [0x00001042]  Special opcode 103: advance Address by 7 to 0x2c10 and Line by 0 to 219
+  [0x00001040]  Advance Line by -20 to 232
+  [0x00001042]  Special opcode 103: advance Address by 7 to 0x2c10 and Line by 0 to 232
   [0x00001043]  Set column to 9
-  [0x00001045]  Special opcode 9: advance Address by 0 to 0x2c10 and Line by 4 to 223 (view 1)
+  [0x00001045]  Special opcode 9: advance Address by 0 to 0x2c10 and Line by 4 to 236 (view 1)
   [0x00001046]  Set is_stmt to 0
-  [0x00001047]  Special opcode 201: advance Address by 14 to 0x2c1e and Line by 0 to 223
-  [0x00001048]  Special opcode 47: advance Address by 3 to 0x2c21 and Line by 0 to 223
+  [0x00001047]  Special opcode 201: advance Address by 14 to 0x2c1e and Line by 0 to 236
+  [0x00001048]  Special opcode 47: advance Address by 3 to 0x2c21 and Line by 0 to 236
   [0x00001049]  Set is_stmt to 1
-  [0x0000104a]  Special opcode 76: advance Address by 5 to 0x2c26 and Line by 1 to 224
+  [0x0000104a]  Special opcode 76: advance Address by 5 to 0x2c26 and Line by 1 to 237
   [0x0000104b]  Set is_stmt to 0
-  [0x0000104c]  Special opcode 4: advance Address by 0 to 0x2c26 and Line by -1 to 223 (view 1)
+  [0x0000104c]  Special opcode 4: advance Address by 0 to 0x2c26 and Line by -1 to 236 (view 1)
   [0x0000104d]  Set column to 1
-  [0x0000104f]  Advance Line by 16 to 239
-  [0x00001051]  Special opcode 33: advance Address by 2 to 0x2c28 and Line by 0 to 239
+  [0x0000104f]  Advance Line by 16 to 252
+  [0x00001051]  Special opcode 33: advance Address by 2 to 0x2c28 and Line by 0 to 252
   [0x00001052]  Set is_stmt to 1
-  [0x00001053]  Advance Line by -177 to 62
+  [0x00001053]  Advance Line by -190 to 62
   [0x00001056]  Special opcode 117: advance Address by 8 to 0x2c30 and Line by 0 to 62
   [0x00001057]  Set is_stmt to 0
   [0x00001058]  Copy (view 1)
   [0x00001059]  Set column to 5
   [0x0000105b]  Set is_stmt to 1
   [0x0000105c]  Special opcode 118: advance Address by 8 to 0x2c38 and Line by 1 to 63
   [0x0000105d]  Set column to 1
@@ -1953,453 +1953,514 @@
   [0x000010d5]  Advance Line by 93 to 167
   [0x000010d8]  Special opcode 19: advance Address by 1 to 0x2ca0 and Line by 0 to 167
   [0x000010d9]  Set column to 5
   [0x000010db]  Special opcode 6: advance Address by 0 to 0x2ca0 and Line by 1 to 168 (view 1)
   [0x000010dc]  Set column to 1
   [0x000010de]  Set is_stmt to 0
   [0x000010df]  Special opcode 4: advance Address by 0 to 0x2ca0 and Line by -1 to 167 (view 2)
-  [0x000010e0]  Set column to 22
-  [0x000010e2]  Special opcode 121: advance Address by 8 to 0x2ca8 and Line by 4 to 171
+  [0x000010e0]  Set column to 15
+  [0x000010e2]  Special opcode 118: advance Address by 8 to 0x2ca8 and Line by 1 to 168
   [0x000010e3]  Set column to 5
-  [0x000010e5]  Special opcode 63: advance Address by 4 to 0x2cac and Line by 2 to 173
-  [0x000010e6]  Set column to 15
-  [0x000010e8]  Special opcode 56: advance Address by 4 to 0x2cb0 and Line by -5 to 168
-  [0x000010e9]  Set column to 5
-  [0x000010eb]  Set is_stmt to 1
-  [0x000010ec]  Special opcode 62: advance Address by 4 to 0x2cb4 and Line by 1 to 169
-  [0x000010ed]  Set column to 15
-  [0x000010ef]  Set is_stmt to 0
-  [0x000010f0]  Copy (view 1)
-  [0x000010f1]  Set column to 5
-  [0x000010f3]  Set is_stmt to 1
-  [0x000010f4]  Special opcode 63: advance Address by 4 to 0x2cb8 and Line by 2 to 171
-  [0x000010f5]  Set File Name to entry 2 in the File Name Table
-  [0x000010f7]  Advance Line by -38 to 133
-  [0x000010f9]  Copy (view 1)
-  [0x000010fa]  Set File Name to entry 1 in the File Name Table
-  [0x000010fc]  Set column to 22
-  [0x000010fe]  Set is_stmt to 0
-  [0x000010ff]  Advance Line by 38 to 171
-  [0x00001101]  Copy (view 2)
-  [0x00001102]  Set File Name to entry 2 in the File Name Table
-  [0x00001104]  Set column to 5
-  [0x00001106]  Set is_stmt to 1
-  [0x00001107]  Advance Line by 594 to 765
-  [0x0000110a]  Special opcode 103: advance Address by 7 to 0x2cbf and Line by 0 to 765
-  [0x0000110b]  Special opcode 10: advance Address by 0 to 0x2cbf and Line by 5 to 770 (view 1)
-  [0x0000110c]  Special opcode 7: advance Address by 0 to 0x2cbf and Line by 2 to 772 (view 2)
-  [0x0000110d]  Set File Name to entry 1 in the File Name Table
-  [0x0000110f]  Advance Line by -600 to 172
-  [0x00001112]  Copy (view 3)
-  [0x00001113]  Special opcode 6: advance Address by 0 to 0x2cbf and Line by 1 to 173 (view 4)
-  [0x00001114]  Set column to 10
-  [0x00001116]  Copy (view 5)
-  [0x00001117]  Set column to 34
-  [0x00001119]  Copy (view 6)
-  [0x0000111a]  Set column to 5
-  [0x0000111c]  Set is_stmt to 0
-  [0x0000111d]  Copy (view 7)
-  [0x0000111e]  Set column to 16
-  [0x00001120]  Extended opcode 4: set Discriminator to 1
-  [0x00001124]  Advance PC by constant 17 to 0x2cd0
-  [0x00001125]  Special opcode 6: advance Address by 0 to 0x2cd0 and Line by 1 to 174
-  [0x00001126]  Set column to 9
-  [0x00001128]  Extended opcode 4: set Discriminator to 4
-  [0x0000112c]  Set is_stmt to 1
-  [0x0000112d]  Special opcode 118: advance Address by 8 to 0x2cd8 and Line by 1 to 175
-  [0x0000112e]  Set File Name to entry 2 in the File Name Table
-  [0x00001130]  Set column to 20
-  [0x00001132]  Extended opcode 4: set Discriminator to 4
-  [0x00001136]  Advance Line by 316 to 491
-  [0x00001139]  Copy (view 1)
-  [0x0000113a]  Set column to 5
-  [0x0000113c]  Extended opcode 4: set Discriminator to 4
-  [0x00001140]  Advance Line by 11 to 502
-  [0x00001142]  Copy (view 2)
-  [0x00001143]  Set column to 18
-  [0x00001145]  Extended opcode 4: set Discriminator to 4
-  [0x00001149]  Set is_stmt to 0
-  [0x0000114a]  Copy (view 3)
-  [0x0000114b]  Set File Name to entry 1 in the File Name Table
-  [0x0000114d]  Set column to 9
-  [0x0000114f]  Extended opcode 4: set Discriminator to 4
-  [0x00001153]  Set is_stmt to 1
-  [0x00001154]  Advance Line by -326 to 176
-  [0x00001157]  Special opcode 75: advance Address by 5 to 0x2cdd and Line by 0 to 176
-  [0x00001158]  Set column to 18
-  [0x0000115a]  Extended opcode 4: set Discriminator to 4
-  [0x0000115e]  Set is_stmt to 0
-  [0x0000115f]  Copy (view 1)
-  [0x00001160]  Set File Name to entry 2 in the File Name Table
-  [0x00001162]  Set column to 8
-  [0x00001164]  Extended opcode 4: set Discriminator to 4
-  [0x00001168]  Advance Line by 361 to 537
-  [0x0000116b]  Advance PC by constant 17 to 0x2cee
-  [0x0000116c]  Special opcode 19: advance Address by 1 to 0x2cef and Line by 0 to 537
-  [0x0000116d]  Set File Name to entry 1 in the File Name Table
-  [0x0000116f]  Set column to 18
-  [0x00001171]  Extended opcode 4: set Discriminator to 4
-  [0x00001175]  Advance Line by -361 to 176
-  [0x00001178]  Special opcode 75: advance Address by 5 to 0x2cf4 and Line by 0 to 176
-  [0x00001179]  Set column to 9
-  [0x0000117b]  Extended opcode 4: set Discriminator to 4
-  [0x0000117f]  Set is_stmt to 1
-  [0x00001180]  Special opcode 48: advance Address by 3 to 0x2cf7 and Line by 1 to 177
-  [0x00001181]  Extended opcode 4: set Discriminator to 4
-  [0x00001185]  Copy (view 1)
-  [0x00001186]  Set File Name to entry 2 in the File Name Table
-  [0x00001188]  Set column to 20
-  [0x0000118a]  Extended opcode 4: set Discriminator to 4
-  [0x0000118e]  Advance Line by 356 to 533
-  [0x00001191]  Copy (view 2)
-  [0x00001192]  Set column to 5
-  [0x00001194]  Extended opcode 4: set Discriminator to 4
-  [0x00001198]  Special opcode 9: advance Address by 0 to 0x2cf7 and Line by 4 to 537 (view 3)
-  [0x00001199]  Set column to 8
-  [0x0000119b]  Extended opcode 4: set Discriminator to 4
-  [0x0000119f]  Set is_stmt to 0
-  [0x000011a0]  Copy (view 4)
-  [0x000011a1]  Extended opcode 4: set Discriminator to 4
-  [0x000011a5]  Special opcode 33: advance Address by 2 to 0x2cf9 and Line by 0 to 537
-  [0x000011a6]  Set File Name to entry 1 in the File Name Table
-  [0x000011a8]  Set column to 9
-  [0x000011aa]  Set is_stmt to 1
-  [0x000011ab]  Advance Line by -360 to 177
-  [0x000011ae]  Copy (view 1)
-  [0x000011af]  Copy (view 2)
-  [0x000011b0]  Special opcode 6: advance Address by 0 to 0x2cf9 and Line by 1 to 178 (view 3)
-  [0x000011b1]  Set column to 12
-  [0x000011b3]  Set is_stmt to 0
-  [0x000011b4]  Copy (view 4)
-  [0x000011b5]  Set column to 42
-  [0x000011b7]  Extended opcode 4: set Discriminator to 2
-  [0x000011bb]  Set is_stmt to 1
-  [0x000011bc]  Special opcode 70: advance Address by 5 to 0x2cfe and Line by -5 to 173
-  [0x000011bd]  Set column to 43
-  [0x000011bf]  Extended opcode 4: set Discriminator to 2
-  [0x000011c3]  Set is_stmt to 0
-  [0x000011c4]  Copy (view 1)
-  [0x000011c5]  Set column to 34
-  [0x000011c7]  Extended opcode 4: set Discriminator to 2
-  [0x000011cb]  Set is_stmt to 1
-  [0x000011cc]  Special opcode 61: advance Address by 4 to 0x2d02 and Line by 0 to 173
-  [0x000011cd]  Set column to 5
-  [0x000011cf]  Extended opcode 4: set Discriminator to 2
-  [0x000011d3]  Set is_stmt to 0
-  [0x000011d4]  Copy (view 1)
-  [0x000011d5]  Set column to 9
-  [0x000011d7]  Set is_stmt to 1
-  [0x000011d8]  Advance PC by constant 17 to 0x2d13
-  [0x000011d9]  Special opcode 6: advance Address by 0 to 0x2d13 and Line by 1 to 174
-  [0x000011da]  Set is_stmt to 0
-  [0x000011db]  Copy (view 1)
-  [0x000011dc]  Set File Name to entry 2 in the File Name Table
-  [0x000011de]  Set column to 5
-  [0x000011e0]  Set is_stmt to 1
-  [0x000011e1]  Advance Line by -41 to 133
-  [0x000011e3]  Copy (view 2)
-  [0x000011e4]  Set column to 1
-  [0x000011e6]  Advance Line by 630 to 763
-  [0x000011e9]  Copy (view 3)
-  [0x000011ea]  Set column to 5
-  [0x000011ec]  Special opcode 7: advance Address by 0 to 0x2d13 and Line by 2 to 765 (view 4)
-  [0x000011ed]  Special opcode 10: advance Address by 0 to 0x2d13 and Line by 5 to 770 (view 5)
-  [0x000011ee]  Special opcode 7: advance Address by 0 to 0x2d13 and Line by 2 to 772 (view 6)
-  [0x000011ef]  Set is_stmt to 0
-  [0x000011f0]  Copy (view 7)
-  [0x000011f1]  Set File Name to entry 1 in the File Name Table
-  [0x000011f3]  Set column to 16
-  [0x000011f5]  Advance Line by -598 to 174
-  [0x000011f8]  Copy (view 8)
-  [0x000011f9]  Extended opcode 4: set Discriminator to 2
-  [0x000011fd]  Special opcode 103: advance Address by 7 to 0x2d1a and Line by 0 to 174
-  [0x000011fe]  Set File Name to entry 2 in the File Name Table
-  [0x00001200]  Set column to 9
-  [0x00001202]  Set is_stmt to 1
-  [0x00001203]  Advance Line by 364 to 538
-  [0x00001206]  Special opcode 201: advance Address by 14 to 0x2d28 and Line by 0 to 538
-  [0x00001207]  Set is_stmt to 0
-  [0x00001208]  Special opcode 117: advance Address by 8 to 0x2d30 and Line by 0 to 538
-  [0x00001209]  Set File Name to entry 1 in the File Name Table
-  [0x0000120b]  Set is_stmt to 1
-  [0x0000120c]  Advance Line by -361 to 177
-  [0x0000120f]  Copy (view 1)
-  [0x00001210]  Copy (view 2)
-  [0x00001211]  Special opcode 6: advance Address by 0 to 0x2d30 and Line by 1 to 178 (view 3)
-  [0x00001212]  Set column to 12
-  [0x00001214]  Set is_stmt to 0
-  [0x00001215]  Copy (view 4)
-  [0x00001216]  Special opcode 75: advance Address by 5 to 0x2d35 and Line by 0 to 178
-  [0x00001217]  Set column to 1
-  [0x00001219]  Special opcode 10: advance Address by 0 to 0x2d35 and Line by 5 to 183 (view 1)
-  [0x0000121a]  Special opcode 103: advance Address by 7 to 0x2d3c and Line by 0 to 183
-  [0x0000121b]  Special opcode 33: advance Address by 2 to 0x2d3e and Line by 0 to 183
-  [0x0000121c]  Set is_stmt to 1
-  [0x0000121d]  Advance PC by constant 17 to 0x2d4f
-  [0x0000121e]  Special opcode 24: advance Address by 1 to 0x2d50 and Line by 5 to 188
+  [0x000010e5]  Set is_stmt to 1
+  [0x000010e6]  Special opcode 62: advance Address by 4 to 0x2cac and Line by 1 to 169
+  [0x000010e7]  Set File Name to entry 2 in the File Name Table
+  [0x000010e9]  Set column to 20
+  [0x000010eb]  Advance Line by 322 to 491
+  [0x000010ee]  Copy (view 1)
+  [0x000010ef]  Set column to 5
+  [0x000010f1]  Advance Line by 11 to 502
+  [0x000010f3]  Copy (view 2)
+  [0x000010f4]  Set File Name to entry 1 in the File Name Table
+  [0x000010f6]  Set column to 22
+  [0x000010f8]  Set is_stmt to 0
+  [0x000010f9]  Advance Line by -330 to 172
+  [0x000010fc]  Copy (view 3)
+  [0x000010fd]  Set column to 15
+  [0x000010ff]  Special opcode 59: advance Address by 4 to 0x2cb0 and Line by -2 to 170
+  [0x00001100]  Set File Name to entry 2 in the File Name Table
+  [0x00001102]  Set column to 18
+  [0x00001104]  Advance Line by 332 to 502
+  [0x00001107]  Special opcode 61: advance Address by 4 to 0x2cb4 and Line by 0 to 502
+  [0x00001108]  Set File Name to entry 1 in the File Name Table
+  [0x0000110a]  Set column to 5
+  [0x0000110c]  Set is_stmt to 1
+  [0x0000110d]  Advance Line by -332 to 170
+  [0x00001110]  Special opcode 75: advance Address by 5 to 0x2cb9 and Line by 0 to 170
+  [0x00001111]  Special opcode 7: advance Address by 0 to 0x2cb9 and Line by 2 to 172 (view 1)
+  [0x00001112]  Set File Name to entry 2 in the File Name Table
+  [0x00001114]  Advance Line by -39 to 133
+  [0x00001116]  Copy (view 2)
+  [0x00001117]  Set File Name to entry 1 in the File Name Table
+  [0x00001119]  Set is_stmt to 0
+  [0x0000111a]  Advance Line by 41 to 174
+  [0x0000111c]  Copy (view 3)
+  [0x0000111d]  Set column to 22
+  [0x0000111f]  Special opcode 59: advance Address by 4 to 0x2cbd and Line by -2 to 172
+  [0x00001120]  Set File Name to entry 2 in the File Name Table
+  [0x00001122]  Set column to 5
+  [0x00001124]  Set is_stmt to 1
+  [0x00001125]  Advance Line by 593 to 765
+  [0x00001128]  Special opcode 103: advance Address by 7 to 0x2cc4 and Line by 0 to 765
+  [0x00001129]  Special opcode 10: advance Address by 0 to 0x2cc4 and Line by 5 to 770 (view 1)
+  [0x0000112a]  Special opcode 7: advance Address by 0 to 0x2cc4 and Line by 2 to 772 (view 2)
+  [0x0000112b]  Set File Name to entry 4 in the File Name Table
+  [0x0000112d]  Set column to 26
+  [0x0000112f]  Advance Line by -739 to 33
+  [0x00001132]  Copy (view 3)
+  [0x00001133]  Set column to 5
+  [0x00001135]  Special opcode 6: advance Address by 0 to 0x2cc4 and Line by 1 to 34 (view 4)
+  [0x00001136]  Special opcode 6: advance Address by 0 to 0x2cc4 and Line by 1 to 35 (view 5)
+  [0x00001137]  Set File Name to entry 2 in the File Name Table
+  [0x00001139]  Set column to 26
+  [0x0000113b]  Advance Line by 105 to 140
+  [0x0000113e]  Copy (view 6)
+  [0x0000113f]  Set column to 5
+  [0x00001141]  Special opcode 6: advance Address by 0 to 0x2cc4 and Line by 1 to 141 (view 7)
+  [0x00001142]  Special opcode 6: advance Address by 0 to 0x2cc4 and Line by 1 to 142 (view 8)
+  [0x00001143]  Set is_stmt to 0
+  [0x00001144]  Copy (view 9)
+  [0x00001145]  Set File Name to entry 1 in the File Name Table
+  [0x00001147]  Set is_stmt to 1
+  [0x00001148]  Advance Line by 31 to 173
+  [0x0000114a]  Copy (view 10)
+  [0x0000114b]  Special opcode 6: advance Address by 0 to 0x2cc4 and Line by 1 to 174 (view 11)
+  [0x0000114c]  Set column to 10
+  [0x0000114e]  Copy (view 12)
+  [0x0000114f]  Set column to 34
+  [0x00001151]  Copy (view 13)
+  [0x00001152]  Set column to 5
+  [0x00001154]  Set is_stmt to 0
+  [0x00001155]  Copy (view 14)
+  [0x00001156]  Set column to 16
+  [0x00001158]  Extended opcode 4: set Discriminator to 1
+  [0x0000115c]  Special opcode 174: advance Address by 12 to 0x2cd0 and Line by 1 to 175
+  [0x0000115d]  Set column to 9
+  [0x0000115f]  Extended opcode 4: set Discriminator to 4
+  [0x00001163]  Set is_stmt to 1
+  [0x00001164]  Special opcode 118: advance Address by 8 to 0x2cd8 and Line by 1 to 176
+  [0x00001165]  Set File Name to entry 2 in the File Name Table
+  [0x00001167]  Set column to 20
+  [0x00001169]  Extended opcode 4: set Discriminator to 4
+  [0x0000116d]  Advance Line by 315 to 491
+  [0x00001170]  Copy (view 1)
+  [0x00001171]  Set column to 5
+  [0x00001173]  Extended opcode 4: set Discriminator to 4
+  [0x00001177]  Advance Line by 11 to 502
+  [0x00001179]  Copy (view 2)
+  [0x0000117a]  Set column to 18
+  [0x0000117c]  Extended opcode 4: set Discriminator to 4
+  [0x00001180]  Set is_stmt to 0
+  [0x00001181]  Copy (view 3)
+  [0x00001182]  Set File Name to entry 1 in the File Name Table
+  [0x00001184]  Set column to 9
+  [0x00001186]  Extended opcode 4: set Discriminator to 4
+  [0x0000118a]  Set is_stmt to 1
+  [0x0000118b]  Advance Line by -325 to 177
+  [0x0000118e]  Special opcode 75: advance Address by 5 to 0x2cdd and Line by 0 to 177
+  [0x0000118f]  Set column to 18
+  [0x00001191]  Extended opcode 4: set Discriminator to 4
+  [0x00001195]  Set is_stmt to 0
+  [0x00001196]  Copy (view 1)
+  [0x00001197]  Set column to 9
+  [0x00001199]  Extended opcode 4: set Discriminator to 4
+  [0x0000119d]  Advance Line by 12 to 189
+  [0x0000119f]  Advance PC by constant 17 to 0x2cee
+  [0x000011a0]  Special opcode 19: advance Address by 1 to 0x2cef and Line by 0 to 189
+  [0x000011a1]  Set column to 18
+  [0x000011a3]  Extended opcode 4: set Discriminator to 4
+  [0x000011a7]  Advance Line by -12 to 177
+  [0x000011a9]  Special opcode 61: advance Address by 4 to 0x2cf3 and Line by 0 to 177
+  [0x000011aa]  Set column to 9
+  [0x000011ac]  Extended opcode 4: set Discriminator to 4
+  [0x000011b0]  Set is_stmt to 1
+  [0x000011b1]  Advance Line by 12 to 189
+  [0x000011b3]  Special opcode 47: advance Address by 3 to 0x2cf6 and Line by 0 to 189
+  [0x000011b4]  Set File Name to entry 2 in the File Name Table
+  [0x000011b6]  Set column to 20
+  [0x000011b8]  Extended opcode 4: set Discriminator to 4
+  [0x000011bc]  Advance Line by 344 to 533
+  [0x000011bf]  Copy (view 1)
+  [0x000011c0]  Set column to 5
+  [0x000011c2]  Extended opcode 4: set Discriminator to 4
+  [0x000011c6]  Special opcode 9: advance Address by 0 to 0x2cf6 and Line by 4 to 537 (view 2)
+  [0x000011c7]  Set column to 8
+  [0x000011c9]  Extended opcode 4: set Discriminator to 4
+  [0x000011cd]  Set is_stmt to 0
+  [0x000011ce]  Copy (view 3)
+  [0x000011cf]  Extended opcode 4: set Discriminator to 4
+  [0x000011d3]  Special opcode 89: advance Address by 6 to 0x2cfc and Line by 0 to 537
+  [0x000011d4]  Set File Name to entry 1 in the File Name Table
+  [0x000011d6]  Set column to 9
+  [0x000011d8]  Set is_stmt to 1
+  [0x000011d9]  Advance Line by -347 to 190
+  [0x000011dc]  Copy (view 1)
+  [0x000011dd]  Copy (view 2)
+  [0x000011de]  Set File Name to entry 2 in the File Name Table
+  [0x000011e0]  Set column to 20
+  [0x000011e2]  Advance Line by 343 to 533
+  [0x000011e5]  Copy (view 3)
+  [0x000011e6]  Set column to 5
+  [0x000011e8]  Special opcode 9: advance Address by 0 to 0x2cfc and Line by 4 to 537 (view 4)
+  [0x000011e9]  Set column to 8
+  [0x000011eb]  Set is_stmt to 0
+  [0x000011ec]  Copy (view 5)
+  [0x000011ed]  Special opcode 103: advance Address by 7 to 0x2d03 and Line by 0 to 537
+  [0x000011ee]  Set File Name to entry 1 in the File Name Table
+  [0x000011f0]  Set column to 9
+  [0x000011f2]  Set is_stmt to 1
+  [0x000011f3]  Advance Line by -347 to 190
+  [0x000011f6]  Copy (view 1)
+  [0x000011f7]  Copy (view 2)
+  [0x000011f8]  Special opcode 6: advance Address by 0 to 0x2d03 and Line by 1 to 191 (view 3)
+  [0x000011f9]  Set column to 42
+  [0x000011fb]  Advance Line by -17 to 174
+  [0x000011fd]  Copy (view 4)
+  [0x000011fe]  Set column to 43
+  [0x00001200]  Set is_stmt to 0
+  [0x00001201]  Copy (view 5)
+  [0x00001202]  Set column to 34
+  [0x00001204]  Set is_stmt to 1
+  [0x00001205]  Special opcode 61: advance Address by 4 to 0x2d07 and Line by 0 to 174
+  [0x00001206]  Set column to 5
+  [0x00001208]  Set is_stmt to 0
+  [0x00001209]  Copy (view 1)
+  [0x0000120a]  Special opcode 89: advance Address by 6 to 0x2d0d and Line by 0 to 174
+  [0x0000120b]  Set column to 9
+  [0x0000120d]  Set is_stmt to 1
+  [0x0000120e]  Special opcode 160: advance Address by 11 to 0x2d18 and Line by 1 to 175
+  [0x0000120f]  Set is_stmt to 0
+  [0x00001210]  Copy (view 1)
+  [0x00001211]  Set File Name to entry 2 in the File Name Table
+  [0x00001213]  Set column to 5
+  [0x00001215]  Set is_stmt to 1
+  [0x00001216]  Advance Line by -42 to 133
+  [0x00001218]  Copy (view 2)
+  [0x00001219]  Set column to 1
+  [0x0000121b]  Advance Line by 630 to 763
+  [0x0000121e]  Copy (view 3)
   [0x0000121f]  Set column to 5
-  [0x00001221]  Special opcode 6: advance Address by 0 to 0x2d50 and Line by 1 to 189 (view 1)
-  [0x00001222]  Set column to 1
+  [0x00001221]  Special opcode 7: advance Address by 0 to 0x2d18 and Line by 2 to 765 (view 4)
+  [0x00001222]  Special opcode 10: advance Address by 0 to 0x2d18 and Line by 5 to 770 (view 5)
+  [0x00001223]  Special opcode 7: advance Address by 0 to 0x2d18 and Line by 2 to 772 (view 6)
   [0x00001224]  Set is_stmt to 0
-  [0x00001225]  Special opcode 4: advance Address by 0 to 0x2d50 and Line by -1 to 188 (view 2)
-  [0x00001226]  Set column to 8
-  [0x00001228]  Special opcode 76: advance Address by 5 to 0x2d55 and Line by 1 to 189
-  [0x00001229]  Special opcode 187: advance Address by 13 to 0x2d62 and Line by 0 to 189
-  [0x0000122a]  Set column to 5
-  [0x0000122c]  Set is_stmt to 1
-  [0x0000122d]  Special opcode 52: advance Address by 3 to 0x2d65 and Line by 5 to 194
-  [0x0000122e]  Set column to 31
-  [0x00001230]  Set is_stmt to 0
-  [0x00001231]  Copy (view 1)
-  [0x00001232]  Special opcode 75: advance Address by 5 to 0x2d6a and Line by 0 to 194
-  [0x00001233]  Set column to 5
-  [0x00001235]  Set is_stmt to 1
-  [0x00001236]  Special opcode 48: advance Address by 3 to 0x2d6d and Line by 1 to 195
-  [0x00001237]  Set column to 8
-  [0x00001239]  Set is_stmt to 0
-  [0x0000123a]  Copy (view 1)
-  [0x0000123b]  Set column to 5
-  [0x0000123d]  Set is_stmt to 1
-  [0x0000123e]  Special opcode 134: advance Address by 9 to 0x2d76 and Line by 3 to 198
-  [0x0000123f]  Set column to 15
+  [0x00001225]  Copy (view 7)
+  [0x00001226]  Set File Name to entry 1 in the File Name Table
+  [0x00001228]  Set column to 16
+  [0x0000122a]  Advance Line by -597 to 175
+  [0x0000122d]  Copy (view 8)
+  [0x0000122e]  Extended opcode 4: set Discriminator to 2
+  [0x00001232]  Special opcode 103: advance Address by 7 to 0x2d1f and Line by 0 to 175
+  [0x00001233]  Set File Name to entry 2 in the File Name Table
+  [0x00001235]  Set column to 9
+  [0x00001237]  Set is_stmt to 1
+  [0x00001238]  Advance Line by 363 to 538
+  [0x0000123b]  Advance PC by constant 17 to 0x2d30
+  [0x0000123c]  Special opcode 5: advance Address by 0 to 0x2d30 and Line by 0 to 538
+  [0x0000123d]  Set File Name to entry 1 in the File Name Table
+  [0x0000123f]  Set column to 43
   [0x00001241]  Set is_stmt to 0
-  [0x00001242]  Copy (view 1)
-  [0x00001243]  Set column to 5
-  [0x00001245]  Set is_stmt to 1
-  [0x00001246]  Special opcode 63: advance Address by 4 to 0x2d7a and Line by 2 to 200
-  [0x00001247]  Set File Name to entry 2 in the File Name Table
-  [0x00001249]  Set column to 19
-  [0x0000124b]  Advance Line by 62 to 262
-  [0x0000124d]  Copy (view 1)
-  [0x0000124e]  Set column to 5
-  [0x00001250]  Special opcode 6: advance Address by 0 to 0x2d7a and Line by 1 to 263 (view 2)
-  [0x00001251]  Set column to 19
-  [0x00001253]  Advance Line by -114 to 149
-  [0x00001256]  Copy (view 3)
-  [0x00001257]  Set column to 5
-  [0x00001259]  Special opcode 6: advance Address by 0 to 0x2d7a and Line by 1 to 150 (view 4)
-  [0x0000125a]  Set column to 33
-  [0x0000125c]  Set is_stmt to 0
-  [0x0000125d]  Advance Line by 113 to 263
-  [0x00001260]  Copy (view 5)
-  [0x00001261]  Set column to 12
-  [0x00001263]  Advance Line by -113 to 150
-  [0x00001266]  Special opcode 103: advance Address by 7 to 0x2d81 and Line by 0 to 150
-  [0x00001267]  Special opcode 61: advance Address by 4 to 0x2d85 and Line by 0 to 150
-  [0x00001268]  Set column to 5
-  [0x0000126a]  Set is_stmt to 1
-  [0x0000126b]  Advance Line by -17 to 133
-  [0x0000126d]  Copy (view 1)
-  [0x0000126e]  Set column to 33
-  [0x00001270]  Set is_stmt to 0
-  [0x00001271]  Advance Line by 130 to 263
-  [0x00001274]  Copy (view 2)
-  [0x00001275]  Special opcode 75: advance Address by 5 to 0x2d8a and Line by 0 to 263
-  [0x00001276]  Set column to 5
-  [0x00001278]  Set is_stmt to 1
-  [0x00001279]  Advance Line by -130 to 133
-  [0x0000127c]  Copy (view 1)
-  [0x0000127d]  Set column to 36
-  [0x0000127f]  Set is_stmt to 0
-  [0x00001280]  Advance Line by 130 to 263
-  [0x00001283]  Copy (view 2)
-  [0x00001284]  Set column to 33
-  [0x00001286]  Special opcode 75: advance Address by 5 to 0x2d8f and Line by 0 to 263
-  [0x00001287]  Special opcode 61: advance Address by 4 to 0x2d93 and Line by 0 to 263
-  [0x00001288]  Set File Name to entry 1 in the File Name Table
-  [0x0000128a]  Set column to 9
-  [0x0000128c]  Set is_stmt to 1
-  [0x0000128d]  Advance Line by -58 to 205
-  [0x0000128f]  Copy (view 1)
-  [0x00001290]  Set column to 14
-  [0x00001292]  Set is_stmt to 0
-  [0x00001293]  Copy (view 2)
-  [0x00001294]  Set column to 15
-  [0x00001296]  Special opcode 121: advance Address by 8 to 0x2d9b and Line by 4 to 209
-  [0x00001297]  Set column to 14
-  [0x00001299]  Special opcode 141: advance Address by 10 to 0x2da5 and Line by -4 to 205
-  [0x0000129a]  Set column to 9
-  [0x0000129c]  Set is_stmt to 1
-  [0x0000129d]  Special opcode 48: advance Address by 3 to 0x2da8 and Line by 1 to 206
-  [0x0000129e]  Set column to 5
-  [0x000012a0]  Special opcode 8: advance Address by 0 to 0x2da8 and Line by 3 to 209 (view 1)
-  [0x000012a1]  Set column to 15
-  [0x000012a3]  Set is_stmt to 0
-  [0x000012a4]  Copy (view 2)
-  [0x000012a5]  Special opcode 75: advance Address by 5 to 0x2dad and Line by 0 to 209
-  [0x000012a6]  Set column to 8
-  [0x000012a8]  Special opcode 47: advance Address by 3 to 0x2db0 and Line by 0 to 209
-  [0x000012a9]  Set column to 9
-  [0x000012ab]  Set is_stmt to 1
-  [0x000012ac]  Special opcode 76: advance Address by 5 to 0x2db5 and Line by 1 to 210
-  [0x000012ad]  Set column to 18
-  [0x000012af]  Set is_stmt to 0
-  [0x000012b0]  Copy (view 1)
-  [0x000012b1]  Set File Name to entry 2 in the File Name Table
-  [0x000012b3]  Set column to 8
-  [0x000012b5]  Advance Line by 327 to 537
-  [0x000012b8]  Special opcode 159: advance Address by 11 to 0x2dc0 and Line by 0 to 537
-  [0x000012b9]  Set File Name to entry 1 in the File Name Table
-  [0x000012bb]  Set column to 18
-  [0x000012bd]  Advance Line by -327 to 210
-  [0x000012c0]  Special opcode 75: advance Address by 5 to 0x2dc5 and Line by 0 to 210
-  [0x000012c1]  Set column to 9
-  [0x000012c3]  Set is_stmt to 1
-  [0x000012c4]  Special opcode 48: advance Address by 3 to 0x2dc8 and Line by 1 to 211
-  [0x000012c5]  Copy (view 1)
-  [0x000012c6]  Set File Name to entry 2 in the File Name Table
-  [0x000012c8]  Set column to 20
-  [0x000012ca]  Advance Line by 322 to 533
-  [0x000012cd]  Copy (view 2)
-  [0x000012ce]  Set column to 5
-  [0x000012d0]  Special opcode 9: advance Address by 0 to 0x2dc8 and Line by 4 to 537 (view 3)
-  [0x000012d1]  Set column to 8
-  [0x000012d3]  Set is_stmt to 0
-  [0x000012d4]  Copy (view 4)
-  [0x000012d5]  Set File Name to entry 1 in the File Name Table
-  [0x000012d7]  Set column to 18
-  [0x000012d9]  Advance Line by -327 to 210
-  [0x000012dc]  Special opcode 33: advance Address by 2 to 0x2dca and Line by 0 to 210
-  [0x000012dd]  Set column to 9
-  [0x000012df]  Extended opcode 4: set Discriminator to 1
-  [0x000012e3]  Set is_stmt to 1
-  [0x000012e4]  Special opcode 48: advance Address by 3 to 0x2dcd and Line by 1 to 211
-  [0x000012e5]  Set column to 5
-  [0x000012e7]  Extended opcode 4: set Discriminator to 1
-  [0x000012eb]  Special opcode 8: advance Address by 0 to 0x2dcd and Line by 3 to 214 (view 1)
-  [0x000012ec]  Extended opcode 4: set Discriminator to 1
-  [0x000012f0]  Copy (view 2)
-  [0x000012f1]  Set File Name to entry 2 in the File Name Table
-  [0x000012f3]  Set column to 20
-  [0x000012f5]  Extended opcode 4: set Discriminator to 1
-  [0x000012f9]  Advance Line by 385 to 599
-  [0x000012fc]  Copy (view 3)
-  [0x000012fd]  Set column to 5
-  [0x000012ff]  Extended opcode 4: set Discriminator to 1
-  [0x00001303]  Special opcode 7: advance Address by 0 to 0x2dcd and Line by 2 to 601 (view 4)
-  [0x00001304]  Set column to 8
-  [0x00001306]  Extended opcode 4: set Discriminator to 1
-  [0x0000130a]  Set is_stmt to 0
-  [0x0000130b]  Copy (view 5)
-  [0x0000130c]  Extended opcode 4: set Discriminator to 1
-  [0x00001310]  Special opcode 75: advance Address by 5 to 0x2dd2 and Line by 0 to 601
-  [0x00001311]  Set File Name to entry 1 in the File Name Table
-  [0x00001313]  Set column to 9
-  [0x00001315]  Set is_stmt to 1
-  [0x00001316]  Advance Line by -390 to 211
-  [0x00001319]  Copy (view 1)
-  [0x0000131a]  Copy (view 2)
-  [0x0000131b]  Set File Name to entry 2 in the File Name Table
-  [0x0000131d]  Set column to 20
-  [0x0000131f]  Advance Line by 322 to 533
-  [0x00001322]  Copy (view 3)
-  [0x00001323]  Set column to 5
-  [0x00001325]  Special opcode 9: advance Address by 0 to 0x2dd2 and Line by 4 to 537 (view 4)
-  [0x00001326]  Set column to 8
-  [0x00001328]  Set is_stmt to 0
-  [0x00001329]  Copy (view 5)
-  [0x0000132a]  Special opcode 103: advance Address by 7 to 0x2dd9 and Line by 0 to 537
-  [0x0000132b]  Set File Name to entry 1 in the File Name Table
-  [0x0000132d]  Set column to 1
-  [0x0000132f]  Advance Line by -321 to 216
-  [0x00001332]  Copy (view 1)
-  [0x00001333]  Special opcode 89: advance Address by 6 to 0x2ddf and Line by 0 to 216
-  [0x00001334]  Set column to 9
-  [0x00001336]  Set is_stmt to 1
-  [0x00001337]  Advance Line by -26 to 190
-  [0x00001339]  Special opcode 131: advance Address by 9 to 0x2de8 and Line by 0 to 190
-  [0x0000133a]  Set column to 16
-  [0x0000133c]  Set is_stmt to 0
-  [0x0000133d]  Special opcode 104: advance Address by 7 to 0x2def and Line by 1 to 191
+  [0x00001242]  Advance Line by -364 to 174
+  [0x00001245]  Special opcode 47: advance Address by 3 to 0x2d33 and Line by 0 to 174
+  [0x00001246]  Set File Name to entry 2 in the File Name Table
+  [0x00001248]  Set column to 9
+  [0x0000124a]  Advance Line by 364 to 538
+  [0x0000124d]  Special opcode 61: advance Address by 4 to 0x2d37 and Line by 0 to 538
+  [0x0000124e]  Special opcode 75: advance Address by 5 to 0x2d3c and Line by 0 to 538
+  [0x0000124f]  Set File Name to entry 1 in the File Name Table
+  [0x00001251]  Set is_stmt to 1
+  [0x00001252]  Advance Line by -348 to 190
+  [0x00001255]  Copy (view 1)
+  [0x00001256]  Copy (view 2)
+  [0x00001257]  Special opcode 6: advance Address by 0 to 0x2d3c and Line by 1 to 191 (view 3)
+  [0x00001258]  Set column to 42
+  [0x0000125a]  Advance Line by -17 to 174
+  [0x0000125c]  Copy (view 4)
+  [0x0000125d]  Set column to 34
+  [0x0000125f]  Copy (view 5)
+  [0x00001260]  Set column to 5
+  [0x00001262]  Set is_stmt to 0
+  [0x00001263]  Copy (view 6)
+  [0x00001264]  Special opcode 89: advance Address by 6 to 0x2d42 and Line by 0 to 174
+  [0x00001265]  Set column to 1
+  [0x00001267]  Advance Line by 22 to 196
+  [0x00001269]  Copy (view 1)
+  [0x0000126a]  Special opcode 19: advance Address by 1 to 0x2d43 and Line by 0 to 196
+  [0x0000126b]  Special opcode 89: advance Address by 6 to 0x2d49 and Line by 0 to 196
+  [0x0000126c]  Set File Name to entry 2 in the File Name Table
+  [0x0000126e]  Set column to 9
+  [0x00001270]  Set is_stmt to 1
+  [0x00001271]  Advance Line by 342 to 538
+  [0x00001274]  Special opcode 103: advance Address by 7 to 0x2d50 and Line by 0 to 538
+  [0x00001275]  Set is_stmt to 0
+  [0x00001276]  Special opcode 75: advance Address by 5 to 0x2d55 and Line by 0 to 538
+  [0x00001277]  Set File Name to entry 1 in the File Name Table
+  [0x00001279]  Set column to 1
+  [0x0000127b]  Set is_stmt to 1
+  [0x0000127c]  Advance Line by -337 to 201
+  [0x0000127f]  Special opcode 159: advance Address by 11 to 0x2d60 and Line by 0 to 201
+  [0x00001280]  Set column to 5
+  [0x00001282]  Special opcode 6: advance Address by 0 to 0x2d60 and Line by 1 to 202 (view 1)
+  [0x00001283]  Set column to 1
+  [0x00001285]  Set is_stmt to 0
+  [0x00001286]  Special opcode 4: advance Address by 0 to 0x2d60 and Line by -1 to 201 (view 2)
+  [0x00001287]  Set column to 8
+  [0x00001289]  Special opcode 76: advance Address by 5 to 0x2d65 and Line by 1 to 202
+  [0x0000128a]  Special opcode 187: advance Address by 13 to 0x2d72 and Line by 0 to 202
+  [0x0000128b]  Set column to 5
+  [0x0000128d]  Set is_stmt to 1
+  [0x0000128e]  Special opcode 52: advance Address by 3 to 0x2d75 and Line by 5 to 207
+  [0x0000128f]  Set column to 31
+  [0x00001291]  Set is_stmt to 0
+  [0x00001292]  Copy (view 1)
+  [0x00001293]  Special opcode 75: advance Address by 5 to 0x2d7a and Line by 0 to 207
+  [0x00001294]  Set column to 5
+  [0x00001296]  Set is_stmt to 1
+  [0x00001297]  Special opcode 48: advance Address by 3 to 0x2d7d and Line by 1 to 208
+  [0x00001298]  Set column to 8
+  [0x0000129a]  Set is_stmt to 0
+  [0x0000129b]  Copy (view 1)
+  [0x0000129c]  Set column to 5
+  [0x0000129e]  Set is_stmt to 1
+  [0x0000129f]  Special opcode 134: advance Address by 9 to 0x2d86 and Line by 3 to 211
+  [0x000012a0]  Set column to 15
+  [0x000012a2]  Set is_stmt to 0
+  [0x000012a3]  Copy (view 1)
+  [0x000012a4]  Set column to 5
+  [0x000012a6]  Set is_stmt to 1
+  [0x000012a7]  Special opcode 63: advance Address by 4 to 0x2d8a and Line by 2 to 213
+  [0x000012a8]  Set File Name to entry 2 in the File Name Table
+  [0x000012aa]  Set column to 19
+  [0x000012ac]  Advance Line by 49 to 262
+  [0x000012ae]  Copy (view 1)
+  [0x000012af]  Set column to 5
+  [0x000012b1]  Special opcode 6: advance Address by 0 to 0x2d8a and Line by 1 to 263 (view 2)
+  [0x000012b2]  Set column to 19
+  [0x000012b4]  Advance Line by -114 to 149
+  [0x000012b7]  Copy (view 3)
+  [0x000012b8]  Set column to 5
+  [0x000012ba]  Special opcode 6: advance Address by 0 to 0x2d8a and Line by 1 to 150 (view 4)
+  [0x000012bb]  Set column to 33
+  [0x000012bd]  Set is_stmt to 0
+  [0x000012be]  Advance Line by 113 to 263
+  [0x000012c1]  Copy (view 5)
+  [0x000012c2]  Set column to 12
+  [0x000012c4]  Advance Line by -113 to 150
+  [0x000012c7]  Special opcode 103: advance Address by 7 to 0x2d91 and Line by 0 to 150
+  [0x000012c8]  Special opcode 61: advance Address by 4 to 0x2d95 and Line by 0 to 150
+  [0x000012c9]  Set column to 5
+  [0x000012cb]  Set is_stmt to 1
+  [0x000012cc]  Advance Line by -17 to 133
+  [0x000012ce]  Copy (view 1)
+  [0x000012cf]  Set column to 33
+  [0x000012d1]  Set is_stmt to 0
+  [0x000012d2]  Advance Line by 130 to 263
+  [0x000012d5]  Copy (view 2)
+  [0x000012d6]  Special opcode 75: advance Address by 5 to 0x2d9a and Line by 0 to 263
+  [0x000012d7]  Set column to 5
+  [0x000012d9]  Set is_stmt to 1
+  [0x000012da]  Advance Line by -130 to 133
+  [0x000012dd]  Copy (view 1)
+  [0x000012de]  Set column to 36
+  [0x000012e0]  Set is_stmt to 0
+  [0x000012e1]  Advance Line by 130 to 263
+  [0x000012e4]  Copy (view 2)
+  [0x000012e5]  Set column to 33
+  [0x000012e7]  Special opcode 75: advance Address by 5 to 0x2d9f and Line by 0 to 263
+  [0x000012e8]  Special opcode 61: advance Address by 4 to 0x2da3 and Line by 0 to 263
+  [0x000012e9]  Set File Name to entry 1 in the File Name Table
+  [0x000012eb]  Set column to 9
+  [0x000012ed]  Set is_stmt to 1
+  [0x000012ee]  Advance Line by -45 to 218
+  [0x000012f0]  Copy (view 1)
+  [0x000012f1]  Set column to 14
+  [0x000012f3]  Set is_stmt to 0
+  [0x000012f4]  Copy (view 2)
+  [0x000012f5]  Set column to 15
+  [0x000012f7]  Special opcode 121: advance Address by 8 to 0x2dab and Line by 4 to 222
+  [0x000012f8]  Set column to 14
+  [0x000012fa]  Special opcode 141: advance Address by 10 to 0x2db5 and Line by -4 to 218
+  [0x000012fb]  Set column to 9
+  [0x000012fd]  Set is_stmt to 1
+  [0x000012fe]  Special opcode 48: advance Address by 3 to 0x2db8 and Line by 1 to 219
+  [0x000012ff]  Set column to 5
+  [0x00001301]  Special opcode 8: advance Address by 0 to 0x2db8 and Line by 3 to 222 (view 1)
+  [0x00001302]  Set column to 15
+  [0x00001304]  Set is_stmt to 0
+  [0x00001305]  Copy (view 2)
+  [0x00001306]  Special opcode 75: advance Address by 5 to 0x2dbd and Line by 0 to 222
+  [0x00001307]  Set column to 8
+  [0x00001309]  Special opcode 47: advance Address by 3 to 0x2dc0 and Line by 0 to 222
+  [0x0000130a]  Set column to 9
+  [0x0000130c]  Set is_stmt to 1
+  [0x0000130d]  Special opcode 76: advance Address by 5 to 0x2dc5 and Line by 1 to 223
+  [0x0000130e]  Set column to 18
+  [0x00001310]  Set is_stmt to 0
+  [0x00001311]  Copy (view 1)
+  [0x00001312]  Set File Name to entry 2 in the File Name Table
+  [0x00001314]  Set column to 8
+  [0x00001316]  Advance Line by 314 to 537
+  [0x00001319]  Special opcode 159: advance Address by 11 to 0x2dd0 and Line by 0 to 537
+  [0x0000131a]  Set File Name to entry 1 in the File Name Table
+  [0x0000131c]  Set column to 18
+  [0x0000131e]  Advance Line by -314 to 223
+  [0x00001321]  Special opcode 75: advance Address by 5 to 0x2dd5 and Line by 0 to 223
+  [0x00001322]  Set column to 9
+  [0x00001324]  Set is_stmt to 1
+  [0x00001325]  Special opcode 48: advance Address by 3 to 0x2dd8 and Line by 1 to 224
+  [0x00001326]  Copy (view 1)
+  [0x00001327]  Set File Name to entry 2 in the File Name Table
+  [0x00001329]  Set column to 20
+  [0x0000132b]  Advance Line by 309 to 533
+  [0x0000132e]  Copy (view 2)
+  [0x0000132f]  Set column to 5
+  [0x00001331]  Special opcode 9: advance Address by 0 to 0x2dd8 and Line by 4 to 537 (view 3)
+  [0x00001332]  Set column to 8
+  [0x00001334]  Set is_stmt to 0
+  [0x00001335]  Copy (view 4)
+  [0x00001336]  Set File Name to entry 1 in the File Name Table
+  [0x00001338]  Set column to 18
+  [0x0000133a]  Advance Line by -314 to 223
+  [0x0000133d]  Special opcode 33: advance Address by 2 to 0x2dda and Line by 0 to 223
   [0x0000133e]  Set column to 9
-  [0x00001340]  Special opcode 46: advance Address by 3 to 0x2df2 and Line by -1 to 190
-  [0x00001341]  Special opcode 103: advance Address by 7 to 0x2df9 and Line by 0 to 190
-  [0x00001342]  Special opcode 47: advance Address by 3 to 0x2dfc and Line by 0 to 190
-  [0x00001343]  Set is_stmt to 1
-  [0x00001344]  Special opcode 76: advance Address by 5 to 0x2e01 and Line by 1 to 191
-  [0x00001345]  Set column to 1
-  [0x00001347]  Set is_stmt to 0
-  [0x00001348]  Advance Line by 25 to 216
-  [0x0000134a]  Copy (view 1)
-  [0x0000134b]  Set column to 5
-  [0x0000134d]  Set is_stmt to 1
-  [0x0000134e]  Advance Line by -7 to 209
-  [0x00001350]  Special opcode 215: advance Address by 15 to 0x2e10 and Line by 0 to 209
-  [0x00001351]  Set column to 15
-  [0x00001353]  Set is_stmt to 0
-  [0x00001354]  Copy (view 1)
-  [0x00001355]  Set column to 8
-  [0x00001357]  Advance PC by constant 17 to 0x2e21
-  [0x00001358]  Special opcode 19: advance Address by 1 to 0x2e22 and Line by 0 to 209
-  [0x00001359]  Set column to 9
-  [0x0000135b]  Set is_stmt to 1
-  [0x0000135c]  Special opcode 76: advance Address by 5 to 0x2e27 and Line by 1 to 210
-  [0x0000135d]  Set column to 18
-  [0x0000135f]  Set is_stmt to 0
-  [0x00001360]  Copy (view 1)
-  [0x00001361]  Special opcode 159: advance Address by 11 to 0x2e32 and Line by 0 to 210
-  [0x00001362]  Special opcode 47: advance Address by 3 to 0x2e35 and Line by 0 to 210
-  [0x00001363]  Set File Name to entry 2 in the File Name Table
-  [0x00001365]  Set column to 9
-  [0x00001367]  Set is_stmt to 1
-  [0x00001368]  Advance Line by 328 to 538
-  [0x0000136b]  Special opcode 159: advance Address by 11 to 0x2e40 and Line by 0 to 538
-  [0x0000136c]  Set File Name to entry 1 in the File Name Table
-  [0x0000136e]  Set column to 18
-  [0x00001370]  Set is_stmt to 0
-  [0x00001371]  Advance Line by -328 to 210
-  [0x00001374]  Special opcode 47: advance Address by 3 to 0x2e43 and Line by 0 to 210
-  [0x00001375]  Set File Name to entry 2 in the File Name Table
-  [0x00001377]  Set column to 9
-  [0x00001379]  Advance Line by 328 to 538
-  [0x0000137c]  Special opcode 47: advance Address by 3 to 0x2e46 and Line by 0 to 538
-  [0x0000137d]  Special opcode 75: advance Address by 5 to 0x2e4b and Line by 0 to 538
-  [0x0000137e]  Set is_stmt to 1
-  [0x0000137f]  Special opcode 75: advance Address by 5 to 0x2e50 and Line by 0 to 538
-  [0x00001380]  Set is_stmt to 0
-  [0x00001381]  Special opcode 117: advance Address by 8 to 0x2e58 and Line by 0 to 538
-  [0x00001382]  Set File Name to entry 1 in the File Name Table
-  [0x00001384]  Set is_stmt to 1
-  [0x00001385]  Advance Line by -327 to 211
-  [0x00001388]  Copy (view 1)
-  [0x00001389]  Set column to 5
-  [0x0000138b]  Special opcode 8: advance Address by 0 to 0x2e58 and Line by 3 to 214 (view 2)
-  [0x0000138c]  Copy (view 3)
-  [0x0000138d]  Set File Name to entry 2 in the File Name Table
-  [0x0000138f]  Set column to 20
-  [0x00001391]  Advance Line by 385 to 599
-  [0x00001394]  Copy (view 4)
-  [0x00001395]  Set column to 5
-  [0x00001397]  Special opcode 7: advance Address by 0 to 0x2e58 and Line by 2 to 601 (view 5)
-  [0x00001398]  Set File Name to entry 1 in the File Name Table
-  [0x0000139a]  Set column to 1
-  [0x0000139c]  Set is_stmt to 0
-  [0x0000139d]  Advance Line by -385 to 216
-  [0x000013a0]  Copy (view 6)
-  [0x000013a1]  Special opcode 89: advance Address by 6 to 0x2e5e and Line by 0 to 216
-  [0x000013a2]  Set column to 16
-  [0x000013a4]  Advance Line by -20 to 196
-  [0x000013a6]  Special opcode 145: advance Address by 10 to 0x2e68 and Line by 0 to 196
-  [0x000013a7]  Set column to 1
-  [0x000013a9]  Advance Line by 20 to 216
-  [0x000013ab]  Special opcode 47: advance Address by 3 to 0x2e6b and Line by 0 to 216
-  [0x000013ac]  Special opcode 117: advance Address by 8 to 0x2e73 and Line by 0 to 216
-  [0x000013ad]  Set is_stmt to 1
-  [0x000013ae]  Advance Line by 247 to 463
-  [0x000013b1]  Special opcode 187: advance Address by 13 to 0x2e80 and Line by 0 to 463
-  [0x000013b2]  Set column to 5
-  [0x000013b4]  Special opcode 6: advance Address by 0 to 0x2e80 and Line by 1 to 464 (view 1)
-  [0x000013b5]  Set column to 12
-  [0x000013b7]  Set is_stmt to 0
-  [0x000013b8]  Copy (view 2)
-  [0x000013b9]  Advance PC by 12 to 0x2e8c
-  [0x000013bb]  Extended opcode 1: End of Sequence
+  [0x00001340]  Extended opcode 4: set Discriminator to 1
+  [0x00001344]  Set is_stmt to 1
+  [0x00001345]  Special opcode 48: advance Address by 3 to 0x2ddd and Line by 1 to 224
+  [0x00001346]  Set column to 5
+  [0x00001348]  Extended opcode 4: set Discriminator to 1
+  [0x0000134c]  Special opcode 8: advance Address by 0 to 0x2ddd and Line by 3 to 227 (view 1)
+  [0x0000134d]  Extended opcode 4: set Discriminator to 1
+  [0x00001351]  Copy (view 2)
+  [0x00001352]  Set File Name to entry 2 in the File Name Table
+  [0x00001354]  Set column to 20
+  [0x00001356]  Extended opcode 4: set Discriminator to 1
+  [0x0000135a]  Advance Line by 372 to 599
+  [0x0000135d]  Copy (view 3)
+  [0x0000135e]  Set column to 5
+  [0x00001360]  Extended opcode 4: set Discriminator to 1
+  [0x00001364]  Special opcode 7: advance Address by 0 to 0x2ddd and Line by 2 to 601 (view 4)
+  [0x00001365]  Set column to 8
+  [0x00001367]  Extended opcode 4: set Discriminator to 1
+  [0x0000136b]  Set is_stmt to 0
+  [0x0000136c]  Copy (view 5)
+  [0x0000136d]  Extended opcode 4: set Discriminator to 1
+  [0x00001371]  Special opcode 75: advance Address by 5 to 0x2de2 and Line by 0 to 601
+  [0x00001372]  Set File Name to entry 1 in the File Name Table
+  [0x00001374]  Set column to 9
+  [0x00001376]  Set is_stmt to 1
+  [0x00001377]  Advance Line by -377 to 224
+  [0x0000137a]  Copy (view 1)
+  [0x0000137b]  Copy (view 2)
+  [0x0000137c]  Set File Name to entry 2 in the File Name Table
+  [0x0000137e]  Set column to 20
+  [0x00001380]  Advance Line by 309 to 533
+  [0x00001383]  Copy (view 3)
+  [0x00001384]  Set column to 5
+  [0x00001386]  Special opcode 9: advance Address by 0 to 0x2de2 and Line by 4 to 537 (view 4)
+  [0x00001387]  Set column to 8
+  [0x00001389]  Set is_stmt to 0
+  [0x0000138a]  Copy (view 5)
+  [0x0000138b]  Special opcode 103: advance Address by 7 to 0x2de9 and Line by 0 to 537
+  [0x0000138c]  Set File Name to entry 1 in the File Name Table
+  [0x0000138e]  Set column to 1
+  [0x00001390]  Advance Line by -308 to 229
+  [0x00001393]  Copy (view 1)
+  [0x00001394]  Special opcode 89: advance Address by 6 to 0x2def and Line by 0 to 229
+  [0x00001395]  Set column to 9
+  [0x00001397]  Set is_stmt to 1
+  [0x00001398]  Advance Line by -26 to 203
+  [0x0000139a]  Special opcode 131: advance Address by 9 to 0x2df8 and Line by 0 to 203
+  [0x0000139b]  Set column to 16
+  [0x0000139d]  Set is_stmt to 0
+  [0x0000139e]  Special opcode 104: advance Address by 7 to 0x2dff and Line by 1 to 204
+  [0x0000139f]  Set column to 9
+  [0x000013a1]  Special opcode 46: advance Address by 3 to 0x2e02 and Line by -1 to 203
+  [0x000013a2]  Special opcode 103: advance Address by 7 to 0x2e09 and Line by 0 to 203
+  [0x000013a3]  Special opcode 47: advance Address by 3 to 0x2e0c and Line by 0 to 203
+  [0x000013a4]  Set is_stmt to 1
+  [0x000013a5]  Special opcode 76: advance Address by 5 to 0x2e11 and Line by 1 to 204
+  [0x000013a6]  Set column to 1
+  [0x000013a8]  Set is_stmt to 0
+  [0x000013a9]  Advance Line by 25 to 229
+  [0x000013ab]  Copy (view 1)
+  [0x000013ac]  Set column to 5
+  [0x000013ae]  Set is_stmt to 1
+  [0x000013af]  Advance Line by -7 to 222
+  [0x000013b1]  Special opcode 215: advance Address by 15 to 0x2e20 and Line by 0 to 222
+  [0x000013b2]  Set column to 15
+  [0x000013b4]  Set is_stmt to 0
+  [0x000013b5]  Copy (view 1)
+  [0x000013b6]  Set column to 8
+  [0x000013b8]  Advance PC by constant 17 to 0x2e31
+  [0x000013b9]  Special opcode 19: advance Address by 1 to 0x2e32 and Line by 0 to 222
+  [0x000013ba]  Set column to 9
+  [0x000013bc]  Set is_stmt to 1
+  [0x000013bd]  Special opcode 76: advance Address by 5 to 0x2e37 and Line by 1 to 223
+  [0x000013be]  Set column to 18
+  [0x000013c0]  Set is_stmt to 0
+  [0x000013c1]  Copy (view 1)
+  [0x000013c2]  Special opcode 159: advance Address by 11 to 0x2e42 and Line by 0 to 223
+  [0x000013c3]  Special opcode 47: advance Address by 3 to 0x2e45 and Line by 0 to 223
+  [0x000013c4]  Set File Name to entry 2 in the File Name Table
+  [0x000013c6]  Set column to 9
+  [0x000013c8]  Set is_stmt to 1
+  [0x000013c9]  Advance Line by 315 to 538
+  [0x000013cc]  Special opcode 159: advance Address by 11 to 0x2e50 and Line by 0 to 538
+  [0x000013cd]  Set File Name to entry 1 in the File Name Table
+  [0x000013cf]  Set column to 18
+  [0x000013d1]  Set is_stmt to 0
+  [0x000013d2]  Advance Line by -315 to 223
+  [0x000013d5]  Special opcode 47: advance Address by 3 to 0x2e53 and Line by 0 to 223
+  [0x000013d6]  Set File Name to entry 2 in the File Name Table
+  [0x000013d8]  Set column to 9
+  [0x000013da]  Advance Line by 315 to 538
+  [0x000013dd]  Special opcode 47: advance Address by 3 to 0x2e56 and Line by 0 to 538
+  [0x000013de]  Special opcode 75: advance Address by 5 to 0x2e5b and Line by 0 to 538
+  [0x000013df]  Set is_stmt to 1
+  [0x000013e0]  Special opcode 75: advance Address by 5 to 0x2e60 and Line by 0 to 538
+  [0x000013e1]  Set is_stmt to 0
+  [0x000013e2]  Special opcode 117: advance Address by 8 to 0x2e68 and Line by 0 to 538
+  [0x000013e3]  Set File Name to entry 1 in the File Name Table
+  [0x000013e5]  Set is_stmt to 1
+  [0x000013e6]  Advance Line by -314 to 224
+  [0x000013e9]  Copy (view 1)
+  [0x000013ea]  Set column to 5
+  [0x000013ec]  Special opcode 8: advance Address by 0 to 0x2e68 and Line by 3 to 227 (view 2)
+  [0x000013ed]  Copy (view 3)
+  [0x000013ee]  Set File Name to entry 2 in the File Name Table
+  [0x000013f0]  Set column to 20
+  [0x000013f2]  Advance Line by 372 to 599
+  [0x000013f5]  Copy (view 4)
+  [0x000013f6]  Set column to 5
+  [0x000013f8]  Special opcode 7: advance Address by 0 to 0x2e68 and Line by 2 to 601 (view 5)
+  [0x000013f9]  Set File Name to entry 1 in the File Name Table
+  [0x000013fb]  Set column to 1
+  [0x000013fd]  Set is_stmt to 0
+  [0x000013fe]  Advance Line by -372 to 229
+  [0x00001401]  Copy (view 6)
+  [0x00001402]  Special opcode 89: advance Address by 6 to 0x2e6e and Line by 0 to 229
+  [0x00001403]  Set column to 16
+  [0x00001405]  Advance Line by -20 to 209
+  [0x00001407]  Special opcode 145: advance Address by 10 to 0x2e78 and Line by 0 to 209
+  [0x00001408]  Set column to 1
+  [0x0000140a]  Advance Line by 20 to 229
+  [0x0000140c]  Special opcode 47: advance Address by 3 to 0x2e7b and Line by 0 to 229
+  [0x0000140d]  Special opcode 117: advance Address by 8 to 0x2e83 and Line by 0 to 229
+  [0x0000140e]  Set is_stmt to 1
+  [0x0000140f]  Advance Line by 247 to 476
+  [0x00001412]  Special opcode 187: advance Address by 13 to 0x2e90 and Line by 0 to 476
+  [0x00001413]  Set column to 5
+  [0x00001415]  Special opcode 6: advance Address by 0 to 0x2e90 and Line by 1 to 477 (view 1)
+  [0x00001416]  Set column to 12
+  [0x00001418]  Set is_stmt to 0
+  [0x00001419]  Copy (view 2)
+  [0x0000141a]  Advance PC by 12 to 0x2e9c
+  [0x0000141c]  Extended opcode 1: End of Sequence
 
 
-  Offset:                      0x13be
+  Offset:                      0x141f
   Length:                      82
   DWARF Version:               3
   Prologue Length:             40
   Minimum Instruction Length:  1
   Initial value of 'is_stmt':  1
   Line Base:                   -5
   Line Range:                  14
@@ -2415,28 +2476,28 @@
   Opcode 7 has 0 args
   Opcode 8 has 0 args
   Opcode 9 has 1 arg
   Opcode 10 has 0 args
   Opcode 11 has 0 args
   Opcode 12 has 1 arg
 
- The Directory Table (offset 0x13d9):
+ The Directory Table (offset 0x143a):
   1	crt/x86_64
 
- The File Name Table (offset 0x13e5):
+ The File Name Table (offset 0x1446):
   Entry	Dir	Time	Size	Name
   1	1	0	0	crtn.s
 
  Line Number Statements:
-  [0x000013f0]  Extended opcode 2: set Address to 0x200b
-  [0x000013fb]  Special opcode 6: advance Address by 0 to 0x200b and Line by 1 to 2
-  [0x000013fc]  Special opcode 20: advance Address by 1 to 0x200c and Line by 1 to 3
-  [0x000013fd]  Advance PC by 1 to 0x200d
-  [0x000013ff]  Extended opcode 1: End of Sequence
+  [0x00001451]  Extended opcode 2: set Address to 0x200b
+  [0x0000145c]  Special opcode 6: advance Address by 0 to 0x200b and Line by 1 to 2
+  [0x0000145d]  Special opcode 20: advance Address by 1 to 0x200c and Line by 1 to 3
+  [0x0000145e]  Advance PC by 1 to 0x200d
+  [0x00001460]  Extended opcode 1: End of Sequence
 
-  [0x00001402]  Extended opcode 2: set Address to 0x2eb4
-  [0x0000140d]  Special opcode 10: advance Address by 0 to 0x2eb4 and Line by 5 to 6
-  [0x0000140e]  Special opcode 20: advance Address by 1 to 0x2eb5 and Line by 1 to 7
-  [0x0000140f]  Advance PC by 1 to 0x2eb6
-  [0x00001411]  Extended opcode 1: End of Sequence
+  [0x00001463]  Extended opcode 2: set Address to 0x2ec4
+  [0x0000146e]  Special opcode 10: advance Address by 0 to 0x2ec4 and Line by 5 to 6
+  [0x0000146f]  Special opcode 20: advance Address by 1 to 0x2ec5 and Line by 1 to 7
+  [0x00001470]  Advance PC by 1 to 0x2ec6
+  [0x00001472]  Extended opcode 1: End of Sequence
```

### readelf --wide --debug-dump=info {}

```diff
@@ -9,25 +9,25 @@
     <c>   DW_AT_stmt_list   : (data4) 0
     <10>   DW_AT_ranges      : (data4) 0
     <14>   DW_AT_name        : (strp) (offset: 0): crt/x86_64/crti.s
     <18>   DW_AT_comp_dir    : (strp) (offset: 0x12): /home/buildozer/aports/main/musl/src/musl-1.1.24
     <1c>   DW_AT_producer    : (strp) (offset: 0x43): GNU AS 2.34
     <20>   DW_AT_language    : (data2) 32769	(MIPS assembler)
   Compilation Unit @ offset 0x22:
-   Length:        0x44d4 (32-bit)
+   Length:        0x45b1 (32-bit)
    Version:       4
    Abbrev Offset: 0x12
    Pointer Size:  8
  <0><2d>: Abbrev Number: 1 (DW_TAG_compile_unit)
     <2e>   DW_AT_producer    : (strp) (offset: 0xbdd): GNU C17 9.3.0 -mtune=generic -march=x86-64 -g -O3 -fwrapv -fPIC
     <32>   DW_AT_language    : (data1) 12	(ANSI C99)
     <33>   DW_AT_name        : (strp) (offset: 0x15d9): consmodule.c
     <37>   DW_AT_comp_dir    : (strp) (offset: 0x2061): /project
     <3b>   DW_AT_low_pc      : (addr) 0x23c0
-    <43>   DW_AT_high_pc     : (data8) 0xacc
+    <43>   DW_AT_high_pc     : (data8) 0xadc
     <4b>   DW_AT_stmt_list   : (sec_offset) 0x56
  <1><4f>: Abbrev Number: 2 (DW_TAG_base_type)
     <50>   DW_AT_byte_size   : (data1) 4
     <51>   DW_AT_encoding    : (data1) 5	(signed)
     <52>   DW_AT_name        : (string) int
  <1><56>: Abbrev Number: 3 (DW_TAG_typedef)
     <57>   DW_AT_name        : (strp) (offset: 0x19a1): size_t
@@ -5221,15 +5221,15 @@
  <2><248f>: Abbrev Number: 13 (DW_TAG_subrange_type)
     <2490>   DW_AT_type        : (ref4) <0x62>, long unsigned int
     <2494>   DW_AT_upper_bound : (data1) 2
  <2><2495>: Abbrev Number: 0
  <1><2496>: Abbrev Number: 39 (DW_TAG_variable)
     <2497>   DW_AT_name        : (strp) (offset: 0x122c): Cons_members
     <249b>   DW_AT_decl_file   : (data1) 1
-    <249c>   DW_AT_decl_line   : (data2) 350
+    <249c>   DW_AT_decl_line   : (data2) 363
     <249e>   DW_AT_decl_column : (data1) 20
     <249f>   DW_AT_type        : (ref4) <0x2486>, PyMemberDef, PyMemberDef
     <24a3>   DW_AT_location    : (exprloc) 9 byte block: 3 80 50 0 0 0 0 0 0 	(DW_OP_addr: 5080)
  <1><24ad>: Abbrev Number: 12 (DW_TAG_array_type)
     <24ae>   DW_AT_type        : (ref4) <0xaf>, char
     <24b2>   DW_AT_sibling     : (ref4) <0x24bd>
  <2><24b6>: Abbrev Number: 13 (DW_TAG_subrange_type)
@@ -5237,15 +5237,15 @@
     <24bb>   DW_AT_upper_bound : (data1) 46
  <2><24bc>: Abbrev Number: 0
  <1><24bd>: Abbrev Number: 5 (DW_TAG_const_type)
     <24be>   DW_AT_type        : (ref4) <0x24ad>, char
  <1><24c2>: Abbrev Number: 39 (DW_TAG_variable)
     <24c3>   DW_AT_name        : (strp) (offset: 0xeb1): from_xs_doc
     <24c7>   DW_AT_decl_file   : (data1) 1
-    <24c8>   DW_AT_decl_line   : (data2) 356
+    <24c8>   DW_AT_decl_line   : (data2) 369
     <24ca>   DW_AT_decl_column : (data1) 1
     <24cb>   DW_AT_type        : (ref4) <0x24bd>, char
     <24cf>   DW_AT_location    : (exprloc) 9 byte block: 3 80 31 0 0 0 0 0 0 	(DW_OP_addr: 3180)
  <1><24d9>: Abbrev Number: 12 (DW_TAG_array_type)
     <24da>   DW_AT_type        : (ref4) <0xaf>, char
     <24de>   DW_AT_sibling     : (ref4) <0x24e9>
  <2><24e2>: Abbrev Number: 13 (DW_TAG_subrange_type)
@@ -5253,29 +5253,29 @@
     <24e7>   DW_AT_upper_bound : (data1) 44
  <2><24e8>: Abbrev Number: 0
  <1><24e9>: Abbrev Number: 5 (DW_TAG_const_type)
     <24ea>   DW_AT_type        : (ref4) <0x24d9>, char
  <1><24ee>: Abbrev Number: 39 (DW_TAG_variable)
     <24ef>   DW_AT_name        : (strp) (offset: 0x1a61): to_list_doc
     <24f3>   DW_AT_decl_file   : (data1) 1
-    <24f4>   DW_AT_decl_line   : (data2) 357
+    <24f4>   DW_AT_decl_line   : (data2) 370
     <24f6>   DW_AT_decl_column : (data1) 1
     <24f7>   DW_AT_type        : (ref4) <0x24e9>, char
     <24fb>   DW_AT_location    : (exprloc) 9 byte block: 3 40 31 0 0 0 0 0 0 	(DW_OP_addr: 3140)
  <1><2505>: Abbrev Number: 12 (DW_TAG_array_type)
     <2506>   DW_AT_type        : (ref4) <0x2ce>, PyMethodDef, PyMethodDef
     <250a>   DW_AT_sibling     : (ref4) <0x2515>
  <2><250e>: Abbrev Number: 13 (DW_TAG_subrange_type)
     <250f>   DW_AT_type        : (ref4) <0x62>, long unsigned int
     <2513>   DW_AT_upper_bound : (data1) 2
  <2><2514>: Abbrev Number: 0
  <1><2515>: Abbrev Number: 39 (DW_TAG_variable)
     <2516>   DW_AT_name        : (strp) (offset: 0xa57): Cons_methods
     <251a>   DW_AT_decl_file   : (data1) 1
-    <251b>   DW_AT_decl_line   : (data2) 359
+    <251b>   DW_AT_decl_line   : (data2) 372
     <251d>   DW_AT_decl_column : (data1) 20
     <251e>   DW_AT_type        : (ref4) <0x2505>, PyMethodDef, PyMethodDef
     <2522>   DW_AT_location    : (exprloc) 9 byte block: 3 40 52 0 0 0 0 0 0 	(DW_OP_addr: 5240)
  <1><252c>: Abbrev Number: 12 (DW_TAG_array_type)
     <252d>   DW_AT_type        : (ref4) <0xaf>, char
     <2531>   DW_AT_sibling     : (ref4) <0x253c>
  <2><2535>: Abbrev Number: 13 (DW_TAG_subrange_type)
@@ -5283,250 +5283,250 @@
     <253a>   DW_AT_upper_bound : (data1) 30
  <2><253b>: Abbrev Number: 0
  <1><253c>: Abbrev Number: 5 (DW_TAG_const_type)
     <253d>   DW_AT_type        : (ref4) <0x252c>, char
  <1><2541>: Abbrev Number: 39 (DW_TAG_variable)
     <2542>   DW_AT_name        : (strp) (offset: 0x2e4): cons_doc
     <2546>   DW_AT_decl_file   : (data1) 1
-    <2547>   DW_AT_decl_line   : (data2) 367
+    <2547>   DW_AT_decl_line   : (data2) 380
     <2549>   DW_AT_decl_column : (data1) 1
     <254a>   DW_AT_type        : (ref4) <0x253c>, char
     <254e>   DW_AT_location    : (exprloc) 9 byte block: 3 20 31 0 0 0 0 0 0 	(DW_OP_addr: 3120)
  <1><2558>: Abbrev Number: 12 (DW_TAG_array_type)
     <2559>   DW_AT_type        : (ref4) <0xf00>, PyType_Slot
     <255d>   DW_AT_sibling     : (ref4) <0x2568>
  <2><2561>: Abbrev Number: 13 (DW_TAG_subrange_type)
     <2562>   DW_AT_type        : (ref4) <0x62>, long unsigned int
     <2566>   DW_AT_upper_bound : (data1) 9
  <2><2567>: Abbrev Number: 0
  <1><2568>: Abbrev Number: 39 (DW_TAG_variable)
     <2569>   DW_AT_name        : (strp) (offset: 0x116): Cons_Type_Slots
     <256d>   DW_AT_decl_file   : (data1) 1
-    <256e>   DW_AT_decl_line   : (data2) 369
+    <256e>   DW_AT_decl_line   : (data2) 382
     <2570>   DW_AT_decl_column : (data1) 20
     <2571>   DW_AT_type        : (ref4) <0x2558>, PyType_Slot
     <2575>   DW_AT_location    : (exprloc) 9 byte block: 3 a0 51 0 0 0 0 0 0 	(DW_OP_addr: 51a0)
  <1><257f>: Abbrev Number: 39 (DW_TAG_variable)
     <2580>   DW_AT_name        : (strp) (offset: 0xf7f): Cons_Type_Spec
     <2584>   DW_AT_decl_file   : (data1) 1
-    <2585>   DW_AT_decl_line   : (data2) 382
+    <2585>   DW_AT_decl_line   : (data2) 395
     <2587>   DW_AT_decl_column : (data1) 20
     <2588>   DW_AT_type        : (ref4) <0xf5d>, PyType_Spec
     <258c>   DW_AT_location    : (exprloc) 9 byte block: 3 60 50 0 0 0 0 0 0 	(DW_OP_addr: 5060)
  <1><2596>: Abbrev Number: 12 (DW_TAG_array_type)
     <2597>   DW_AT_type        : (ref4) <0x29a>, PyModuleDef_Slot, PyModuleDef_Slot
     <259b>   DW_AT_sibling     : (ref4) <0x25a6>
  <2><259f>: Abbrev Number: 13 (DW_TAG_subrange_type)
     <25a0>   DW_AT_type        : (ref4) <0x62>, long unsigned int
     <25a4>   DW_AT_upper_bound : (data1) 1
  <2><25a5>: Abbrev Number: 0
  <1><25a6>: Abbrev Number: 39 (DW_TAG_variable)
     <25a7>   DW_AT_name        : (strp) (offset: 0x2132): consmodule_slots
     <25ab>   DW_AT_decl_file   : (data1) 1
-    <25ac>   DW_AT_decl_line   : (data2) 425
+    <25ac>   DW_AT_decl_line   : (data2) 438
     <25ae>   DW_AT_decl_column : (data1) 25
     <25af>   DW_AT_type        : (ref4) <0x2596>, PyModuleDef_Slot, PyModuleDef_Slot
     <25b3>   DW_AT_location    : (exprloc) 9 byte block: 3 40 50 0 0 0 0 0 0 	(DW_OP_addr: 5040)
  <1><25bd>: Abbrev Number: 40 (DW_TAG_subprogram)
     <25be>   DW_AT_external    : (flag_present) 1
     <25be>   DW_AT_name        : (strp) (offset: 0x231c): PyInit_fastcons
     <25c2>   DW_AT_decl_file   : (data1) 1
-    <25c3>   DW_AT_decl_line   : (data2) 462
+    <25c3>   DW_AT_decl_line   : (data2) 475
     <25c5>   DW_AT_decl_column : (data1) 1
     <25c6>   DW_AT_prototyped  : (flag_present) 1
     <25c6>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <25ca>   DW_AT_low_pc      : (addr) 0x2e80
+    <25ca>   DW_AT_low_pc      : (addr) 0x2e90
     <25d2>   DW_AT_high_pc     : (data8) 0xc
     <25da>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
     <25dc>   DW_AT_GNU_all_call_sites: (flag_present) 1
     <25dc>   DW_AT_sibling     : (ref4) <0x25fc>
  <2><25e0>: Abbrev Number: 41 (DW_TAG_GNU_call_site)
-    <25e1>   DW_AT_low_pc      : (addr) 0x2e8c
+    <25e1>   DW_AT_low_pc      : (addr) 0x2e9c
     <25e9>   DW_AT_GNU_tail_call: (flag_present) 1
-    <25e9>   DW_AT_abstract_origin: (ref4) <0x432c>
+    <25e9>   DW_AT_abstract_origin: (ref4) <0x4409>
  <3><25ed>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <25ee>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
     <25f0>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 20 51 0 0 0 0 0 0 	(DW_OP_addr: 5120)
  <3><25fa>: Abbrev Number: 0
  <2><25fb>: Abbrev Number: 0
  <1><25fc>: Abbrev Number: 43 (DW_TAG_subprogram)
     <25fd>   DW_AT_name        : (strp) (offset: 0x1ad6): consmodule_clear
     <2601>   DW_AT_decl_file   : (data1) 1
-    <2602>   DW_AT_decl_line   : (data2) 441
+    <2602>   DW_AT_decl_line   : (data2) 454
     <2604>   DW_AT_decl_column : (data1) 1
     <2605>   DW_AT_prototyped  : (flag_present) 1
     <2605>   DW_AT_type        : (ref4) <0x4f>, int
     <2609>   DW_AT_low_pc      : (addr) 0x2630
     <2611>   DW_AT_high_pc     : (data8) 0x77
     <2619>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
     <261b>   DW_AT_GNU_all_call_sites: (flag_present) 1
     <261b>   DW_AT_sibling     : (ref4) <0x274d>
  <2><261f>: Abbrev Number: 44 (DW_TAG_formal_parameter)
     <2620>   DW_AT_name        : (string) m
     <2622>   DW_AT_decl_file   : (data1) 1
-    <2623>   DW_AT_decl_line   : (data2) 441
+    <2623>   DW_AT_decl_line   : (data2) 454
     <2625>   DW_AT_decl_column : (data1) 28
     <2626>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
     <262a>   DW_AT_location    : (sec_offset) 0x4 (location list)
     <262e>   DW_AT_GNU_locviews: (sec_offset) 0
  <2><2632>: Abbrev Number: 45 (DW_TAG_variable)
     <2633>   DW_AT_name        : (strp) (offset: 0x58c): state
     <2637>   DW_AT_decl_file   : (data1) 1
-    <2638>   DW_AT_decl_line   : (data2) 443
+    <2638>   DW_AT_decl_line   : (data2) 456
     <263a>   DW_AT_decl_column : (data1) 23
     <263b>   DW_AT_type        : (ref4) <0x274d>, consmodule_state
     <263f>   DW_AT_location    : (sec_offset) 0x49 (location list)
     <2643>   DW_AT_GNU_locviews: (sec_offset) 0x3d
  <2><2647>: Abbrev Number: 46 (DW_TAG_lexical_block)
     <2648>   DW_AT_ranges      : (sec_offset) 0x1b0
     <264c>   DW_AT_sibling     : (ref4) <0x2697>
  <3><2650>: Abbrev Number: 45 (DW_TAG_variable)
     <2651>   DW_AT_name        : (strp) (offset: 0x19b9): _py_tmp
     <2655>   DW_AT_decl_file   : (data1) 1
-    <2656>   DW_AT_decl_line   : (data2) 444
+    <2656>   DW_AT_decl_line   : (data2) 457
     <2658>   DW_AT_decl_column : (data1) 5
     <2659>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
     <265d>   DW_AT_location    : (sec_offset) 0xcf (location list)
     <2661>   DW_AT_GNU_locviews: (sec_offset) 0xcb
  <3><2665>: Abbrev Number: 47 (DW_TAG_inlined_subroutine)
-    <2666>   DW_AT_abstract_origin: (ref4) <0x3e47>
+    <2666>   DW_AT_abstract_origin: (ref4) <0x3f24>
     <266a>   DW_AT_entry_pc    : (addr) 0x264a
     <2672>   DW_AT_GNU_entry_view: (data1) 1
     <2673>   DW_AT_ranges      : (sec_offset) 0x1f0
     <2677>   DW_AT_call_file   : (data1) 1
-    <2678>   DW_AT_call_line   : (data2) 444
+    <2678>   DW_AT_call_line   : (data2) 457
     <267a>   DW_AT_call_column : (data1) 5
  <4><267b>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <267c>   DW_AT_abstract_origin: (ref4) <0x3e55>
+    <267c>   DW_AT_abstract_origin: (ref4) <0x3f32>
     <2680>   DW_AT_location    : (sec_offset) 0x109 (location list)
     <2684>   DW_AT_GNU_locviews: (sec_offset) 0x105
  <4><2688>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
     <2689>   DW_AT_low_pc      : (addr) 0x26a5
-    <2691>   DW_AT_abstract_origin: (ref4) <0x4338>
+    <2691>   DW_AT_abstract_origin: (ref4) <0x4415>
  <4><2695>: Abbrev Number: 0
  <3><2696>: Abbrev Number: 0
  <2><2697>: Abbrev Number: 46 (DW_TAG_lexical_block)
     <2698>   DW_AT_ranges      : (sec_offset) 0x220
     <269c>   DW_AT_sibling     : (ref4) <0x26e7>
  <3><26a0>: Abbrev Number: 45 (DW_TAG_variable)
     <26a1>   DW_AT_name        : (strp) (offset: 0x19b9): _py_tmp
     <26a5>   DW_AT_decl_file   : (data1) 1
-    <26a6>   DW_AT_decl_line   : (data2) 445
+    <26a6>   DW_AT_decl_line   : (data2) 458
     <26a8>   DW_AT_decl_column : (data1) 5
     <26a9>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
     <26ad>   DW_AT_location    : (sec_offset) 0x143 (location list)
     <26b1>   DW_AT_GNU_locviews: (sec_offset) 0x13f
  <3><26b5>: Abbrev Number: 47 (DW_TAG_inlined_subroutine)
-    <26b6>   DW_AT_abstract_origin: (ref4) <0x3e47>
+    <26b6>   DW_AT_abstract_origin: (ref4) <0x3f24>
     <26ba>   DW_AT_entry_pc    : (addr) 0x265f
     <26c2>   DW_AT_GNU_entry_view: (data1) 1
     <26c3>   DW_AT_ranges      : (sec_offset) 0x250
     <26c7>   DW_AT_call_file   : (data1) 1
-    <26c8>   DW_AT_call_line   : (data2) 445
+    <26c8>   DW_AT_call_line   : (data2) 458
     <26ca>   DW_AT_call_column : (data1) 5
  <4><26cb>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <26cc>   DW_AT_abstract_origin: (ref4) <0x3e55>
+    <26cc>   DW_AT_abstract_origin: (ref4) <0x3f32>
     <26d0>   DW_AT_location    : (sec_offset) 0x17d (location list)
     <26d4>   DW_AT_GNU_locviews: (sec_offset) 0x179
  <4><26d8>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
     <26d9>   DW_AT_low_pc      : (addr) 0x2695
-    <26e1>   DW_AT_abstract_origin: (ref4) <0x4338>
+    <26e1>   DW_AT_abstract_origin: (ref4) <0x4415>
  <4><26e5>: Abbrev Number: 0
  <3><26e6>: Abbrev Number: 0
  <2><26e7>: Abbrev Number: 46 (DW_TAG_lexical_block)
     <26e8>   DW_AT_ranges      : (sec_offset) 0x280
     <26ec>   DW_AT_sibling     : (ref4) <0x2737>
  <3><26f0>: Abbrev Number: 45 (DW_TAG_variable)
     <26f1>   DW_AT_name        : (strp) (offset: 0x19b9): _py_tmp
     <26f5>   DW_AT_decl_file   : (data1) 1
-    <26f6>   DW_AT_decl_line   : (data2) 446
+    <26f6>   DW_AT_decl_line   : (data2) 459
     <26f8>   DW_AT_decl_column : (data1) 5
     <26f9>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
     <26fd>   DW_AT_location    : (sec_offset) 0x1b5 (location list)
     <2701>   DW_AT_GNU_locviews: (sec_offset) 0x1b3
  <3><2705>: Abbrev Number: 47 (DW_TAG_inlined_subroutine)
-    <2706>   DW_AT_abstract_origin: (ref4) <0x3e47>
+    <2706>   DW_AT_abstract_origin: (ref4) <0x3f24>
     <270a>   DW_AT_entry_pc    : (addr) 0x2676
     <2712>   DW_AT_GNU_entry_view: (data1) 1
     <2713>   DW_AT_ranges      : (sec_offset) 0x2b0
     <2717>   DW_AT_call_file   : (data1) 1
-    <2718>   DW_AT_call_line   : (data2) 446
+    <2718>   DW_AT_call_line   : (data2) 459
     <271a>   DW_AT_call_column : (data1) 5
  <4><271b>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <271c>   DW_AT_abstract_origin: (ref4) <0x3e55>
+    <271c>   DW_AT_abstract_origin: (ref4) <0x3f32>
     <2720>   DW_AT_location    : (sec_offset) 0x1dc (location list)
     <2724>   DW_AT_GNU_locviews: (sec_offset) 0x1d8
  <4><2728>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
     <2729>   DW_AT_low_pc      : (addr) 0x2685
-    <2731>   DW_AT_abstract_origin: (ref4) <0x4338>
+    <2731>   DW_AT_abstract_origin: (ref4) <0x4415>
  <4><2735>: Abbrev Number: 0
  <3><2736>: Abbrev Number: 0
  <2><2737>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
     <2738>   DW_AT_low_pc      : (addr) 0x2636
-    <2740>   DW_AT_abstract_origin: (ref4) <0x4345>
+    <2740>   DW_AT_abstract_origin: (ref4) <0x4422>
  <3><2744>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <2745>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
     <2747>   DW_AT_GNU_call_site_value: (exprloc) 3 byte block: f3 1 55 	(DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)))
  <3><274b>: Abbrev Number: 0
  <2><274c>: Abbrev Number: 0
  <1><274d>: Abbrev Number: 10 (DW_TAG_pointer_type)
     <274e>   DW_AT_byte_size   : (data1) 8
     <274f>   DW_AT_type        : (ref4) <0x23a6>, consmodule_state
  <1><2753>: Abbrev Number: 43 (DW_TAG_subprogram)
     <2754>   DW_AT_name        : (strp) (offset: 0x17a): consmodule_traverse
     <2758>   DW_AT_decl_file   : (data1) 1
-    <2759>   DW_AT_decl_line   : (data2) 431
+    <2759>   DW_AT_decl_line   : (data2) 444
     <275b>   DW_AT_decl_column : (data1) 1
     <275c>   DW_AT_prototyped  : (flag_present) 1
     <275c>   DW_AT_type        : (ref4) <0x4f>, int
     <2760>   DW_AT_low_pc      : (addr) 0x26b0
     <2768>   DW_AT_high_pc     : (data8) 0x55
     <2770>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
     <2772>   DW_AT_GNU_all_call_sites: (flag_present) 1
     <2772>   DW_AT_sibling     : (ref4) <0x2885>
  <2><2776>: Abbrev Number: 44 (DW_TAG_formal_parameter)
     <2777>   DW_AT_name        : (string) m
     <2779>   DW_AT_decl_file   : (data1) 1
-    <277a>   DW_AT_decl_line   : (data2) 431
+    <277a>   DW_AT_decl_line   : (data2) 444
     <277c>   DW_AT_decl_column : (data1) 31
     <277d>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
     <2781>   DW_AT_location    : (sec_offset) 0x216 (location list)
     <2785>   DW_AT_GNU_locviews: (sec_offset) 0x212
  <2><2789>: Abbrev Number: 51 (DW_TAG_formal_parameter)
     <278a>   DW_AT_name        : (strp) (offset: 0xb21): visit
     <278e>   DW_AT_decl_file   : (data1) 1
-    <278f>   DW_AT_decl_line   : (data2) 431
+    <278f>   DW_AT_decl_line   : (data2) 444
     <2791>   DW_AT_decl_column : (data1) 44
     <2792>   DW_AT_type        : (ref4) <0xd03>, visitproc, int
     <2796>   DW_AT_location    : (sec_offset) 0x25b (location list)
     <279a>   DW_AT_GNU_locviews: (sec_offset) 0x24f
  <2><279e>: Abbrev Number: 44 (DW_TAG_formal_parameter)
     <279f>   DW_AT_name        : (string) arg
     <27a3>   DW_AT_decl_file   : (data1) 1
-    <27a4>   DW_AT_decl_line   : (data2) 431
+    <27a4>   DW_AT_decl_line   : (data2) 444
     <27a6>   DW_AT_decl_column : (data1) 57
     <27a7>   DW_AT_type        : (ref4) <0x88>
     <27ab>   DW_AT_location    : (sec_offset) 0x2ef (location list)
     <27af>   DW_AT_GNU_locviews: (sec_offset) 0x2e3
  <2><27b3>: Abbrev Number: 45 (DW_TAG_variable)
     <27b4>   DW_AT_name        : (strp) (offset: 0x58c): state
     <27b8>   DW_AT_decl_file   : (data1) 1
-    <27b9>   DW_AT_decl_line   : (data2) 433
+    <27b9>   DW_AT_decl_line   : (data2) 446
     <27bb>   DW_AT_decl_column : (data1) 23
     <27bc>   DW_AT_type        : (ref4) <0x274d>, consmodule_state
     <27c0>   DW_AT_location    : (sec_offset) 0x37d (location list)
     <27c4>   DW_AT_GNU_locviews: (sec_offset) 0x377
  <2><27c8>: Abbrev Number: 52 (DW_TAG_lexical_block)
     <27c9>   DW_AT_low_pc      : (addr) 0x26cb
     <27d1>   DW_AT_high_pc     : (data8) 0x9
     <27d9>   DW_AT_sibling     : (ref4) <0x2806>
  <3><27dd>: Abbrev Number: 45 (DW_TAG_variable)
     <27de>   DW_AT_name        : (strp) (offset: 0xb88): vret
     <27e2>   DW_AT_decl_file   : (data1) 1
-    <27e3>   DW_AT_decl_line   : (data2) 434
+    <27e3>   DW_AT_decl_line   : (data2) 447
     <27e5>   DW_AT_decl_column : (data1) 5
     <27e6>   DW_AT_type        : (ref4) <0x4f>, int
     <27ea>   DW_AT_location    : (sec_offset) 0x3c8 (location list)
     <27ee>   DW_AT_GNU_locviews: (sec_offset) 0x3c6
  <3><27f2>: Abbrev Number: 53 (DW_TAG_GNU_call_site)
     <27f3>   DW_AT_low_pc      : (addr) 0x26d0
     <27fb>   DW_AT_GNU_call_site_target: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
@@ -5538,15 +5538,15 @@
  <2><2806>: Abbrev Number: 52 (DW_TAG_lexical_block)
     <2807>   DW_AT_low_pc      : (addr) 0x26dc
     <280f>   DW_AT_high_pc     : (data8) 0x9
     <2817>   DW_AT_sibling     : (ref4) <0x2841>
  <3><281b>: Abbrev Number: 45 (DW_TAG_variable)
     <281c>   DW_AT_name        : (strp) (offset: 0xb88): vret
     <2820>   DW_AT_decl_file   : (data1) 1
-    <2821>   DW_AT_decl_line   : (data2) 435
+    <2821>   DW_AT_decl_line   : (data2) 448
     <2823>   DW_AT_decl_column : (data1) 5
     <2824>   DW_AT_type        : (ref4) <0x4f>, int
     <2828>   DW_AT_location    : (sec_offset) 0x3ed (location list)
     <282c>   DW_AT_GNU_locviews: (sec_offset) 0x3eb
  <3><2830>: Abbrev Number: 54 (DW_TAG_GNU_call_site)
     <2831>   DW_AT_low_pc      : (addr) 0x26e1
  <4><2839>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
@@ -5556,261 +5556,261 @@
  <3><2840>: Abbrev Number: 0
  <2><2841>: Abbrev Number: 46 (DW_TAG_lexical_block)
     <2842>   DW_AT_ranges      : (sec_offset) 0x2e0
     <2846>   DW_AT_sibling     : (ref4) <0x286f>
  <3><284a>: Abbrev Number: 39 (DW_TAG_variable)
     <284b>   DW_AT_name        : (strp) (offset: 0xb88): vret
     <284f>   DW_AT_decl_file   : (data1) 1
-    <2850>   DW_AT_decl_line   : (data2) 436
+    <2850>   DW_AT_decl_line   : (data2) 449
     <2852>   DW_AT_decl_column : (data1) 5
     <2853>   DW_AT_type        : (ref4) <0x4f>, int
     <2857>   DW_AT_location    : (exprloc) 1 byte block: 50 	(DW_OP_reg0 (rax))
  <3><2859>: Abbrev Number: 55 (DW_TAG_GNU_call_site)
     <285a>   DW_AT_low_pc      : (addr) 0x26fc
     <2862>   DW_AT_GNU_tail_call: (flag_present) 1
     <2862>   DW_AT_GNU_call_site_target: (exprloc) 3 byte block: f3 1 54 	(DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)))
  <4><2866>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <2867>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
     <2869>   DW_AT_GNU_call_site_value: (exprloc) 3 byte block: f3 1 51 	(DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)))
  <4><286d>: Abbrev Number: 0
  <3><286e>: Abbrev Number: 0
  <2><286f>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
     <2870>   DW_AT_low_pc      : (addr) 0x26bf
-    <2878>   DW_AT_abstract_origin: (ref4) <0x4345>
+    <2878>   DW_AT_abstract_origin: (ref4) <0x4422>
  <3><287c>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <287d>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
     <287f>   DW_AT_GNU_call_site_value: (exprloc) 3 byte block: f3 1 55 	(DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)))
  <3><2883>: Abbrev Number: 0
  <2><2884>: Abbrev Number: 0
  <1><2885>: Abbrev Number: 43 (DW_TAG_subprogram)
     <2886>   DW_AT_name        : (strp) (offset: 0x1b7c): consmodule_exec
     <288a>   DW_AT_decl_file   : (data1) 1
-    <288b>   DW_AT_decl_line   : (data2) 390
+    <288b>   DW_AT_decl_line   : (data2) 403
     <288d>   DW_AT_decl_column : (data1) 1
     <288e>   DW_AT_prototyped  : (flag_present) 1
     <288e>   DW_AT_type        : (ref4) <0x4f>, int
     <2892>   DW_AT_low_pc      : (addr) 0x2920
     <289a>   DW_AT_high_pc     : (data8) 0x117
     <28a2>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
     <28a4>   DW_AT_GNU_all_call_sites: (flag_present) 1
     <28a4>   DW_AT_sibling     : (ref4) <0x2b42>
  <2><28a8>: Abbrev Number: 44 (DW_TAG_formal_parameter)
     <28a9>   DW_AT_name        : (string) m
     <28ab>   DW_AT_decl_file   : (data1) 1
-    <28ac>   DW_AT_decl_line   : (data2) 390
+    <28ac>   DW_AT_decl_line   : (data2) 403
     <28ae>   DW_AT_decl_column : (data1) 27
     <28af>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
     <28b3>   DW_AT_location    : (sec_offset) 0x418 (location list)
     <28b7>   DW_AT_GNU_locviews: (sec_offset) 0x410
  <2><28bb>: Abbrev Number: 45 (DW_TAG_variable)
     <28bc>   DW_AT_name        : (strp) (offset: 0x58c): state
     <28c0>   DW_AT_decl_file   : (data1) 1
-    <28c1>   DW_AT_decl_line   : (data2) 392
+    <28c1>   DW_AT_decl_line   : (data2) 405
     <28c3>   DW_AT_decl_column : (data1) 23
     <28c4>   DW_AT_type        : (ref4) <0x274d>, consmodule_state
     <28c8>   DW_AT_location    : (sec_offset) 0x47d (location list)
     <28cc>   DW_AT_GNU_locviews: (sec_offset) 0x477
  <2><28d0>: Abbrev Number: 45 (DW_TAG_variable)
     <28d1>   DW_AT_name        : (strp) (offset: 0x53d): match_args
     <28d5>   DW_AT_decl_file   : (data1) 1
-    <28d6>   DW_AT_decl_line   : (data2) 401
+    <28d6>   DW_AT_decl_line   : (data2) 414
     <28d8>   DW_AT_decl_column : (data1) 15
     <28d9>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
     <28dd>   DW_AT_location    : (sec_offset) 0x4ce (location list)
     <28e1>   DW_AT_GNU_locviews: (sec_offset) 0x4c6
  <2><28e5>: Abbrev Number: 56 (DW_TAG_variable)
     <28e6>   DW_AT_name        : (string) nil
     <28ea>   DW_AT_decl_file   : (data1) 1
-    <28eb>   DW_AT_decl_line   : (data2) 419
+    <28eb>   DW_AT_decl_line   : (data2) 432
     <28ed>   DW_AT_decl_column : (data1) 15
     <28ee>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
     <28f2>   DW_AT_location    : (sec_offset) 0x52d (location list)
     <28f6>   DW_AT_GNU_locviews: (sec_offset) 0x52b
  <2><28fa>: Abbrev Number: 57 (DW_TAG_inlined_subroutine)
-    <28fb>   DW_AT_abstract_origin: (ref4) <0x3d66>
+    <28fb>   DW_AT_abstract_origin: (ref4) <0x3e43>
     <28ff>   DW_AT_entry_pc    : (addr) 0x298b
     <2907>   DW_AT_GNU_entry_view: (data1) 0
     <2908>   DW_AT_ranges      : (sec_offset) 0x350
     <290c>   DW_AT_call_file   : (data1) 1
-    <290d>   DW_AT_call_line   : (data2) 404
+    <290d>   DW_AT_call_line   : (data2) 417
     <290f>   DW_AT_call_column : (data1) 5
     <2910>   DW_AT_sibling     : (ref4) <0x294f>
  <3><2914>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <2915>   DW_AT_abstract_origin: (ref4) <0x3d8a>
+    <2915>   DW_AT_abstract_origin: (ref4) <0x3e67>
     <2919>   DW_AT_location    : (sec_offset) 0x552 (location list)
     <291d>   DW_AT_GNU_locviews: (sec_offset) 0x550
  <3><2921>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <2922>   DW_AT_abstract_origin: (ref4) <0x3d7e>
+    <2922>   DW_AT_abstract_origin: (ref4) <0x3e5b>
     <2926>   DW_AT_location    : (sec_offset) 0x577 (location list)
     <292a>   DW_AT_GNU_locviews: (sec_offset) 0x575
  <3><292e>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <292f>   DW_AT_abstract_origin: (ref4) <0x3d73>
+    <292f>   DW_AT_abstract_origin: (ref4) <0x3e50>
     <2933>   DW_AT_location    : (sec_offset) 0x59d (location list)
     <2937>   DW_AT_GNU_locviews: (sec_offset) 0x59b
  <3><293b>: Abbrev Number: 58 (DW_TAG_lexical_block)
     <293c>   DW_AT_ranges      : (sec_offset) 0x350
  <4><2940>: Abbrev Number: 59 (DW_TAG_variable)
-    <2941>   DW_AT_abstract_origin: (ref4) <0x3d96>
+    <2941>   DW_AT_abstract_origin: (ref4) <0x3e73>
     <2945>   DW_AT_location    : (sec_offset) 0x5c4 (location list)
     <2949>   DW_AT_GNU_locviews: (sec_offset) 0x5c0
  <4><294d>: Abbrev Number: 0
  <3><294e>: Abbrev Number: 0
  <2><294f>: Abbrev Number: 57 (DW_TAG_inlined_subroutine)
-    <2950>   DW_AT_abstract_origin: (ref4) <0x3d66>
+    <2950>   DW_AT_abstract_origin: (ref4) <0x3e43>
     <2954>   DW_AT_entry_pc    : (addr) 0x299b
     <295c>   DW_AT_GNU_entry_view: (data1) 0
     <295d>   DW_AT_ranges      : (sec_offset) 0x380
     <2961>   DW_AT_call_file   : (data1) 1
-    <2962>   DW_AT_call_line   : (data2) 405
+    <2962>   DW_AT_call_line   : (data2) 418
     <2964>   DW_AT_call_column : (data1) 5
     <2965>   DW_AT_sibling     : (ref4) <0x29a4>
  <3><2969>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <296a>   DW_AT_abstract_origin: (ref4) <0x3d8a>
+    <296a>   DW_AT_abstract_origin: (ref4) <0x3e67>
     <296e>   DW_AT_location    : (sec_offset) 0x5fc (location list)
     <2972>   DW_AT_GNU_locviews: (sec_offset) 0x5fa
  <3><2976>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <2977>   DW_AT_abstract_origin: (ref4) <0x3d7e>
+    <2977>   DW_AT_abstract_origin: (ref4) <0x3e5b>
     <297b>   DW_AT_location    : (sec_offset) 0x621 (location list)
     <297f>   DW_AT_GNU_locviews: (sec_offset) 0x61f
  <3><2983>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <2984>   DW_AT_abstract_origin: (ref4) <0x3d73>
+    <2984>   DW_AT_abstract_origin: (ref4) <0x3e50>
     <2988>   DW_AT_location    : (sec_offset) 0x647 (location list)
     <298c>   DW_AT_GNU_locviews: (sec_offset) 0x645
  <3><2990>: Abbrev Number: 58 (DW_TAG_lexical_block)
     <2991>   DW_AT_ranges      : (sec_offset) 0x380
  <4><2995>: Abbrev Number: 59 (DW_TAG_variable)
-    <2996>   DW_AT_abstract_origin: (ref4) <0x3d96>
+    <2996>   DW_AT_abstract_origin: (ref4) <0x3e73>
     <299a>   DW_AT_location    : (sec_offset) 0x66e (location list)
     <299e>   DW_AT_GNU_locviews: (sec_offset) 0x66a
  <4><29a2>: Abbrev Number: 0
  <3><29a3>: Abbrev Number: 0
  <2><29a4>: Abbrev Number: 57 (DW_TAG_inlined_subroutine)
-    <29a5>   DW_AT_abstract_origin: (ref4) <0x3e47>
+    <29a5>   DW_AT_abstract_origin: (ref4) <0x3f24>
     <29a9>   DW_AT_entry_pc    : (addr) 0x2a1a
     <29b1>   DW_AT_GNU_entry_view: (data1) 3
     <29b2>   DW_AT_ranges      : (sec_offset) 0x3b0
     <29b6>   DW_AT_call_file   : (data1) 1
-    <29b7>   DW_AT_call_line   : (data2) 408
+    <29b7>   DW_AT_call_line   : (data2) 421
     <29b9>   DW_AT_call_column : (data1) 9
     <29ba>   DW_AT_sibling     : (ref4) <0x29e0>
  <3><29be>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <29bf>   DW_AT_abstract_origin: (ref4) <0x3e55>
+    <29bf>   DW_AT_abstract_origin: (ref4) <0x3f32>
     <29c3>   DW_AT_location    : (sec_offset) 0x6a6 (location list)
     <29c7>   DW_AT_GNU_locviews: (sec_offset) 0x6a4
  <3><29cb>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
     <29cc>   DW_AT_low_pc      : (addr) 0x2a2c
-    <29d4>   DW_AT_abstract_origin: (ref4) <0x4338>
+    <29d4>   DW_AT_abstract_origin: (ref4) <0x4415>
  <4><29d8>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <29d9>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
     <29db>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
  <4><29de>: Abbrev Number: 0
  <3><29df>: Abbrev Number: 0
  <2><29e0>: Abbrev Number: 57 (DW_TAG_inlined_subroutine)
-    <29e1>   DW_AT_abstract_origin: (ref4) <0x3e47>
+    <29e1>   DW_AT_abstract_origin: (ref4) <0x3f24>
     <29e5>   DW_AT_entry_pc    : (addr) 0x29c1
     <29ed>   DW_AT_GNU_entry_view: (data1) 2
     <29ee>   DW_AT_ranges      : (sec_offset) 0x3e0
     <29f2>   DW_AT_call_file   : (data1) 1
-    <29f3>   DW_AT_call_line   : (data2) 411
+    <29f3>   DW_AT_call_line   : (data2) 424
     <29f5>   DW_AT_call_column : (data1) 5
     <29f6>   DW_AT_sibling     : (ref4) <0x2a1c>
  <3><29fa>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <29fb>   DW_AT_abstract_origin: (ref4) <0x3e55>
+    <29fb>   DW_AT_abstract_origin: (ref4) <0x3f32>
     <29ff>   DW_AT_location    : (sec_offset) 0x6cd (location list)
     <2a03>   DW_AT_GNU_locviews: (sec_offset) 0x6c9
  <3><2a07>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
     <2a08>   DW_AT_low_pc      : (addr) 0x2a18
-    <2a10>   DW_AT_abstract_origin: (ref4) <0x4338>
+    <2a10>   DW_AT_abstract_origin: (ref4) <0x4415>
  <4><2a14>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <2a15>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
     <2a17>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
  <4><2a1a>: Abbrev Number: 0
  <3><2a1b>: Abbrev Number: 0
  <2><2a1c>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
     <2a1d>   DW_AT_low_pc      : (addr) 0x292c
-    <2a25>   DW_AT_abstract_origin: (ref4) <0x4345>
+    <2a25>   DW_AT_abstract_origin: (ref4) <0x4422>
     <2a29>   DW_AT_sibling     : (ref4) <0x2a34>
  <3><2a2d>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <2a2e>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
     <2a30>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7c 0 	(DW_OP_breg12 (r12): 0)
  <3><2a33>: Abbrev Number: 0
  <2><2a34>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
     <2a35>   DW_AT_low_pc      : (addr) 0x2949
-    <2a3d>   DW_AT_abstract_origin: (ref4) <0x4351>
+    <2a3d>   DW_AT_abstract_origin: (ref4) <0x442e>
     <2a41>   DW_AT_sibling     : (ref4) <0x2a5e>
  <3><2a45>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <2a46>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
     <2a48>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7c 0 	(DW_OP_breg12 (r12): 0)
  <3><2a4b>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <2a4c>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
     <2a4e>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 60 50 0 0 0 0 0 0 	(DW_OP_addr: 5060)
  <3><2a58>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <2a59>   DW_AT_location    : (exprloc) 1 byte block: 51 	(DW_OP_reg1 (rdx))
     <2a5b>   DW_AT_GNU_call_site_value: (exprloc) 1 byte block: 30 	(DW_OP_lit0)
  <3><2a5d>: Abbrev Number: 0
  <2><2a5e>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
     <2a5f>   DW_AT_low_pc      : (addr) 0x2961
-    <2a67>   DW_AT_abstract_origin: (ref4) <0x435d>
+    <2a67>   DW_AT_abstract_origin: (ref4) <0x443a>
     <2a6b>   DW_AT_sibling     : (ref4) <0x2a76>
  <3><2a6f>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <2a70>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
     <2a72>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7c 0 	(DW_OP_breg12 (r12): 0)
  <3><2a75>: Abbrev Number: 0
  <2><2a76>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
     <2a77>   DW_AT_low_pc      : (addr) 0x2973
-    <2a7f>   DW_AT_abstract_origin: (ref4) <0x4369>
+    <2a7f>   DW_AT_abstract_origin: (ref4) <0x4446>
     <2a83>   DW_AT_sibling     : (ref4) <0x2a8d>
  <3><2a87>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <2a88>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
     <2a8a>   DW_AT_GNU_call_site_value: (exprloc) 1 byte block: 32 	(DW_OP_lit2)
  <3><2a8c>: Abbrev Number: 0
  <2><2a8d>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
     <2a8e>   DW_AT_low_pc      : (addr) 0x298b
-    <2a96>   DW_AT_abstract_origin: (ref4) <0x4375>
+    <2a96>   DW_AT_abstract_origin: (ref4) <0x4452>
     <2a9a>   DW_AT_sibling     : (ref4) <0x2aac>
  <3><2a9e>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <2a9f>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
     <2aa1>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 8e 30 0 0 0 0 0 0 	(DW_OP_addr: 308e)
  <3><2aab>: Abbrev Number: 0
  <2><2aac>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
     <2aad>   DW_AT_low_pc      : (addr) 0x299b
-    <2ab5>   DW_AT_abstract_origin: (ref4) <0x4375>
+    <2ab5>   DW_AT_abstract_origin: (ref4) <0x4452>
     <2ab9>   DW_AT_sibling     : (ref4) <0x2acb>
  <3><2abd>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <2abe>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
     <2ac0>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 98 30 0 0 0 0 0 0 	(DW_OP_addr: 3098)
  <3><2aca>: Abbrev Number: 0
  <2><2acb>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
     <2acc>   DW_AT_low_pc      : (addr) 0x29b9
-    <2ad4>   DW_AT_abstract_origin: (ref4) <0x4381>
+    <2ad4>   DW_AT_abstract_origin: (ref4) <0x445e>
     <2ad8>   DW_AT_sibling     : (ref4) <0x2af0>
  <3><2adc>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <2add>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
     <2adf>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 11 30 0 0 0 0 0 0 	(DW_OP_addr: 3011)
  <3><2ae9>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <2aea>   DW_AT_location    : (exprloc) 1 byte block: 51 	(DW_OP_reg1 (rdx))
     <2aec>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
  <3><2aef>: Abbrev Number: 0
  <2><2af0>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
     <2af1>   DW_AT_low_pc      : (addr) 0x29dc
-    <2af9>   DW_AT_abstract_origin: (ref4) <0x4351>
+    <2af9>   DW_AT_abstract_origin: (ref4) <0x442e>
     <2afd>   DW_AT_sibling     : (ref4) <0x2b1a>
  <3><2b01>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <2b02>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
     <2b04>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7c 0 	(DW_OP_breg12 (r12): 0)
  <3><2b07>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <2b08>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
     <2b0a>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 0 51 0 0 0 0 0 0 	(DW_OP_addr: 5100)
  <3><2b14>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <2b15>   DW_AT_location    : (exprloc) 1 byte block: 51 	(DW_OP_reg1 (rdx))
     <2b17>   DW_AT_GNU_call_site_value: (exprloc) 1 byte block: 30 	(DW_OP_lit0)
  <3><2b19>: Abbrev Number: 0
  <2><2b1a>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
     <2b1b>   DW_AT_low_pc      : (addr) 0x29ef
-    <2b23>   DW_AT_abstract_origin: (ref4) <0x435d>
+    <2b23>   DW_AT_abstract_origin: (ref4) <0x443a>
     <2b27>   DW_AT_sibling     : (ref4) <0x2b32>
  <3><2b2b>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <2b2c>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
     <2b2e>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7c 0 	(DW_OP_breg12 (r12): 0)
  <3><2b31>: Abbrev Number: 0
  <2><2b32>: Abbrev Number: 54 (DW_TAG_GNU_call_site)
     <2b33>   DW_AT_low_pc      : (addr) 0x2a01
@@ -5819,2568 +5819,2636 @@
     <2b3e>   DW_AT_GNU_call_site_value: (exprloc) 1 byte block: 30 	(DW_OP_lit0)
  <3><2b40>: Abbrev Number: 0
  <2><2b41>: Abbrev Number: 0
  <1><2b42>: Abbrev Number: 40 (DW_TAG_subprogram)
     <2b43>   DW_AT_external    : (flag_present) 1
     <2b43>   DW_AT_name        : (strp) (offset: 0xedd): Cons_richcompare
     <2b47>   DW_AT_decl_file   : (data1) 1
-    <2b48>   DW_AT_decl_line   : (data2) 313
+    <2b48>   DW_AT_decl_line   : (data2) 326
     <2b4a>   DW_AT_decl_column : (data1) 1
     <2b4b>   DW_AT_prototyped  : (flag_present) 1
     <2b4b>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
     <2b4f>   DW_AT_low_pc      : (addr) 0x2a40
     <2b57>   DW_AT_high_pc     : (data8) 0xfe
     <2b5f>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
     <2b61>   DW_AT_GNU_all_call_sites: (flag_present) 1
     <2b61>   DW_AT_sibling     : (ref4) <0x2dfd>
  <2><2b65>: Abbrev Number: 51 (DW_TAG_formal_parameter)
     <2b66>   DW_AT_name        : (strp) (offset: 0xf72): self
     <2b6a>   DW_AT_decl_file   : (data1) 1
-    <2b6b>   DW_AT_decl_line   : (data2) 313
+    <2b6b>   DW_AT_decl_line   : (data2) 326
     <2b6d>   DW_AT_decl_column : (data1) 28
     <2b6e>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
     <2b72>   DW_AT_location    : (sec_offset) 0x70d (location list)
     <2b76>   DW_AT_GNU_locviews: (sec_offset) 0x703
  <2><2b7a>: Abbrev Number: 51 (DW_TAG_formal_parameter)
     <2b7b>   DW_AT_name        : (strp) (offset: 0xa32): other
     <2b7f>   DW_AT_decl_file   : (data1) 1
-    <2b80>   DW_AT_decl_line   : (data2) 313
+    <2b80>   DW_AT_decl_line   : (data2) 326
     <2b82>   DW_AT_decl_column : (data1) 44
     <2b83>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
     <2b87>   DW_AT_location    : (sec_offset) 0x78c (location list)
     <2b8b>   DW_AT_GNU_locviews: (sec_offset) 0x782
  <2><2b8f>: Abbrev Number: 44 (DW_TAG_formal_parameter)
     <2b90>   DW_AT_name        : (string) op
     <2b93>   DW_AT_decl_file   : (data1) 1
-    <2b94>   DW_AT_decl_line   : (data2) 313
+    <2b94>   DW_AT_decl_line   : (data2) 326
     <2b96>   DW_AT_decl_column : (data1) 55
     <2b97>   DW_AT_type        : (ref4) <0x4f>, int
     <2b9b>   DW_AT_location    : (sec_offset) 0x819 (location list)
     <2b9f>   DW_AT_GNU_locviews: (sec_offset) 0x801
  <2><2ba3>: Abbrev Number: 45 (DW_TAG_variable)
     <2ba4>   DW_AT_name        : (strp) (offset: 0x58c): state
     <2ba8>   DW_AT_decl_file   : (data1) 1
-    <2ba9>   DW_AT_decl_line   : (data2) 315
+    <2ba9>   DW_AT_decl_line   : (data2) 328
     <2bab>   DW_AT_decl_column : (data1) 23
     <2bac>   DW_AT_type        : (ref4) <0x274d>, consmodule_state
     <2bb0>   DW_AT_location    : (sec_offset) 0x920 (location list)
     <2bb4>   DW_AT_GNU_locviews: (sec_offset) 0x91c
  <2><2bb8>: Abbrev Number: 56 (DW_TAG_variable)
     <2bb9>   DW_AT_name        : (string) nil
     <2bbd>   DW_AT_decl_file   : (data1) 1
-    <2bbe>   DW_AT_decl_line   : (data2) 319
+    <2bbe>   DW_AT_decl_line   : (data2) 332
     <2bc0>   DW_AT_decl_column : (data1) 15
     <2bc1>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
     <2bc5>   DW_AT_location    : (sec_offset) 0x95a (location list)
     <2bc9>   DW_AT_GNU_locviews: (sec_offset) 0x956
  <2><2bcd>: Abbrev Number: 45 (DW_TAG_variable)
     <2bce>   DW_AT_name        : (strp) (offset: 0x2327): cons
     <2bd2>   DW_AT_decl_file   : (data1) 1
-    <2bd3>   DW_AT_decl_line   : (data2) 320
+    <2bd3>   DW_AT_decl_line   : (data2) 333
     <2bd5>   DW_AT_decl_column : (data1) 19
     <2bd6>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
     <2bda>   DW_AT_location    : (sec_offset) 0x99a (location list)
     <2bde>   DW_AT_GNU_locviews: (sec_offset) 0x992
  <2><2be2>: Abbrev Number: 45 (DW_TAG_variable)
     <2be3>   DW_AT_name        : (strp) (offset: 0x1043): this
     <2be7>   DW_AT_decl_file   : (data1) 1
-    <2be8>   DW_AT_decl_line   : (data2) 324
+    <2be8>   DW_AT_decl_line   : (data2) 337
     <2bea>   DW_AT_decl_column : (data1) 15
     <2beb>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
     <2bef>   DW_AT_location    : (sec_offset) 0x9fe (location list)
     <2bf3>   DW_AT_GNU_locviews: (sec_offset) 0x9f6
  <2><2bf7>: Abbrev Number: 45 (DW_TAG_variable)
     <2bf8>   DW_AT_name        : (strp) (offset: 0x506): that
     <2bfc>   DW_AT_decl_file   : (data1) 1
-    <2bfd>   DW_AT_decl_line   : (data2) 324
+    <2bfd>   DW_AT_decl_line   : (data2) 337
     <2bff>   DW_AT_decl_column : (data1) 29
     <2c00>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
     <2c04>   DW_AT_location    : (sec_offset) 0xa62 (location list)
     <2c08>   DW_AT_GNU_locviews: (sec_offset) 0xa5a
  <2><2c0c>: Abbrev Number: 52 (DW_TAG_lexical_block)
     <2c0d>   DW_AT_low_pc      : (addr) 0x2a98
     <2c15>   DW_AT_high_pc     : (data8) 0x30
     <2c1d>   DW_AT_sibling     : (ref4) <0x2c4b>
  <3><2c21>: Abbrev Number: 56 (DW_TAG_variable)
     <2c22>   DW_AT_name        : (string) cmp
     <2c26>   DW_AT_decl_file   : (data1) 1
-    <2c27>   DW_AT_decl_line   : (data2) 327
+    <2c27>   DW_AT_decl_line   : (data2) 340
     <2c29>   DW_AT_decl_column : (data1) 13
     <2c2a>   DW_AT_type        : (ref4) <0x4f>, int
     <2c2e>   DW_AT_location    : (sec_offset) 0xac0 (location list)
     <2c32>   DW_AT_GNU_locviews: (sec_offset) 0xabe
  <3><2c36>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
     <2c37>   DW_AT_low_pc      : (addr) 0x2aa9
-    <2c3f>   DW_AT_abstract_origin: (ref4) <0x438d>
+    <2c3f>   DW_AT_abstract_origin: (ref4) <0x446a>
  <4><2c43>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <2c44>   DW_AT_location    : (exprloc) 1 byte block: 51 	(DW_OP_reg1 (rdx))
     <2c46>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7d 0 	(DW_OP_breg13 (r13): 0)
  <4><2c49>: Abbrev Number: 0
  <3><2c4a>: Abbrev Number: 0
  <2><2c4b>: Abbrev Number: 61 (DW_TAG_inlined_subroutine)
-    <2c4c>   DW_AT_abstract_origin: (ref4) <0x3ea9>
+    <2c4c>   DW_AT_abstract_origin: (ref4) <0x3f86>
     <2c50>   DW_AT_entry_pc    : (addr) 0x2a67
     <2c58>   DW_AT_GNU_entry_view: (data1) 1
     <2c59>   DW_AT_low_pc      : (addr) 0x2a67
     <2c61>   DW_AT_high_pc     : (data8) 0
     <2c69>   DW_AT_call_file   : (data1) 1
-    <2c6a>   DW_AT_call_line   : (data2) 321
+    <2c6a>   DW_AT_call_line   : (data2) 334
     <2c6c>   DW_AT_call_column : (data1) 10
     <2c6d>   DW_AT_sibling     : (ref4) <0x2c8c>
  <3><2c71>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <2c72>   DW_AT_abstract_origin: (ref4) <0x3ec5>
+    <2c72>   DW_AT_abstract_origin: (ref4) <0x3fa2>
     <2c76>   DW_AT_location    : (sec_offset) 0xae5 (location list)
     <2c7a>   DW_AT_GNU_locviews: (sec_offset) 0xae3
  <3><2c7e>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <2c7f>   DW_AT_abstract_origin: (ref4) <0x3eba>
+    <2c7f>   DW_AT_abstract_origin: (ref4) <0x3f97>
     <2c83>   DW_AT_location    : (sec_offset) 0xb0a (location list)
     <2c87>   DW_AT_GNU_locviews: (sec_offset) 0xb08
  <3><2c8b>: Abbrev Number: 0
  <2><2c8c>: Abbrev Number: 57 (DW_TAG_inlined_subroutine)
-    <2c8d>   DW_AT_abstract_origin: (ref4) <0x3e0c>
+    <2c8d>   DW_AT_abstract_origin: (ref4) <0x3ee9>
     <2c91>   DW_AT_entry_pc    : (addr) 0x2a6e
     <2c99>   DW_AT_GNU_entry_view: (data1) 1
     <2c9a>   DW_AT_ranges      : (sec_offset) 0x410
     <2c9e>   DW_AT_call_file   : (data1) 1
-    <2c9f>   DW_AT_call_line   : (data2) 322
+    <2c9f>   DW_AT_call_line   : (data2) 335
     <2ca1>   DW_AT_call_column : (data1) 9
     <2ca2>   DW_AT_sibling     : (ref4) <0x2cd4>
  <3><2ca6>: Abbrev Number: 62 (DW_TAG_formal_parameter)
-    <2ca7>   DW_AT_abstract_origin: (ref4) <0x3e1e>
+    <2ca7>   DW_AT_abstract_origin: (ref4) <0x3efb>
  <3><2cab>: Abbrev Number: 63 (DW_TAG_inlined_subroutine)
-    <2cac>   DW_AT_abstract_origin: (ref4) <0x3e62>
+    <2cac>   DW_AT_abstract_origin: (ref4) <0x3f3f>
     <2cb0>   DW_AT_entry_pc    : (addr) 0x2a6e
     <2cb8>   DW_AT_GNU_entry_view: (data1) 3
     <2cb9>   DW_AT_low_pc      : (addr) 0x2a6e
     <2cc1>   DW_AT_high_pc     : (data8) 0xb
     <2cc9>   DW_AT_call_file   : (data1) 2
     <2cca>   DW_AT_call_line   : (data2) 618
     <2ccc>   DW_AT_call_column : (data1) 5
  <4><2ccd>: Abbrev Number: 62 (DW_TAG_formal_parameter)
-    <2cce>   DW_AT_abstract_origin: (ref4) <0x3e70>
+    <2cce>   DW_AT_abstract_origin: (ref4) <0x3f4d>
  <4><2cd2>: Abbrev Number: 0
  <3><2cd3>: Abbrev Number: 0
  <2><2cd4>: Abbrev Number: 57 (DW_TAG_inlined_subroutine)
-    <2cd5>   DW_AT_abstract_origin: (ref4) <0x3ea9>
+    <2cd5>   DW_AT_abstract_origin: (ref4) <0x3f86>
     <2cd9>   DW_AT_entry_pc    : (addr) 0x2a8c
     <2ce1>   DW_AT_GNU_entry_view: (data1) 1
     <2ce2>   DW_AT_ranges      : (sec_offset) 0x440
     <2ce6>   DW_AT_call_file   : (data1) 1
-    <2ce7>   DW_AT_call_line   : (data2) 326
+    <2ce7>   DW_AT_call_line   : (data2) 339
     <2ce9>   DW_AT_call_column : (data1) 12
     <2cea>   DW_AT_sibling     : (ref4) <0x2d09>
  <3><2cee>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <2cef>   DW_AT_abstract_origin: (ref4) <0x3ec5>
+    <2cef>   DW_AT_abstract_origin: (ref4) <0x3fa2>
     <2cf3>   DW_AT_location    : (sec_offset) 0xb31 (location list)
     <2cf7>   DW_AT_GNU_locviews: (sec_offset) 0xb2d
  <3><2cfb>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <2cfc>   DW_AT_abstract_origin: (ref4) <0x3eba>
+    <2cfc>   DW_AT_abstract_origin: (ref4) <0x3f97>
     <2d00>   DW_AT_location    : (sec_offset) 0xb6b (location list)
     <2d04>   DW_AT_GNU_locviews: (sec_offset) 0xb67
  <3><2d08>: Abbrev Number: 0
  <2><2d09>: Abbrev Number: 61 (DW_TAG_inlined_subroutine)
-    <2d0a>   DW_AT_abstract_origin: (ref4) <0x3ea9>
+    <2d0a>   DW_AT_abstract_origin: (ref4) <0x3f86>
     <2d0e>   DW_AT_entry_pc    : (addr) 0x2ace
     <2d16>   DW_AT_GNU_entry_view: (data1) 0
     <2d17>   DW_AT_low_pc      : (addr) 0x2ace
     <2d1f>   DW_AT_high_pc     : (data8) 0
     <2d27>   DW_AT_call_file   : (data1) 1
-    <2d28>   DW_AT_call_line   : (data2) 326
+    <2d28>   DW_AT_call_line   : (data2) 339
     <2d2a>   DW_AT_call_column : (data1) 38
     <2d2b>   DW_AT_sibling     : (ref4) <0x2d4a>
  <3><2d2f>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <2d30>   DW_AT_abstract_origin: (ref4) <0x3ec5>
+    <2d30>   DW_AT_abstract_origin: (ref4) <0x3fa2>
     <2d34>   DW_AT_location    : (sec_offset) 0xba3 (location list)
     <2d38>   DW_AT_GNU_locviews: (sec_offset) 0xba1
  <3><2d3c>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <2d3d>   DW_AT_abstract_origin: (ref4) <0x3eba>
+    <2d3d>   DW_AT_abstract_origin: (ref4) <0x3f97>
     <2d41>   DW_AT_location    : (sec_offset) 0xbc8 (location list)
     <2d45>   DW_AT_GNU_locviews: (sec_offset) 0xbc6
  <3><2d49>: Abbrev Number: 0
  <2><2d4a>: Abbrev Number: 57 (DW_TAG_inlined_subroutine)
-    <2d4b>   DW_AT_abstract_origin: (ref4) <0x3e0c>
+    <2d4b>   DW_AT_abstract_origin: (ref4) <0x3ee9>
     <2d4f>   DW_AT_entry_pc    : (addr) 0x2ae5
     <2d57>   DW_AT_GNU_entry_view: (data1) 1
     <2d58>   DW_AT_ranges      : (sec_offset) 0x470
     <2d5c>   DW_AT_call_file   : (data1) 1
-    <2d5d>   DW_AT_call_line   : (data2) 345
+    <2d5d>   DW_AT_call_line   : (data2) 358
     <2d5f>   DW_AT_call_column : (data1) 13
     <2d60>   DW_AT_sibling     : (ref4) <0x2d92>
  <3><2d64>: Abbrev Number: 62 (DW_TAG_formal_parameter)
-    <2d65>   DW_AT_abstract_origin: (ref4) <0x3e1e>
+    <2d65>   DW_AT_abstract_origin: (ref4) <0x3efb>
  <3><2d69>: Abbrev Number: 63 (DW_TAG_inlined_subroutine)
-    <2d6a>   DW_AT_abstract_origin: (ref4) <0x3e62>
+    <2d6a>   DW_AT_abstract_origin: (ref4) <0x3f3f>
     <2d6e>   DW_AT_entry_pc    : (addr) 0x2ae5
     <2d76>   DW_AT_GNU_entry_view: (data1) 3
     <2d77>   DW_AT_low_pc      : (addr) 0x2ae5
     <2d7f>   DW_AT_high_pc     : (data8) 0xb
     <2d87>   DW_AT_call_file   : (data1) 2
     <2d88>   DW_AT_call_line   : (data2) 618
     <2d8a>   DW_AT_call_column : (data1) 5
  <4><2d8b>: Abbrev Number: 62 (DW_TAG_formal_parameter)
-    <2d8c>   DW_AT_abstract_origin: (ref4) <0x3e70>
+    <2d8c>   DW_AT_abstract_origin: (ref4) <0x3f4d>
  <4><2d90>: Abbrev Number: 0
  <3><2d91>: Abbrev Number: 0
  <2><2d92>: Abbrev Number: 57 (DW_TAG_inlined_subroutine)
-    <2d93>   DW_AT_abstract_origin: (ref4) <0x3e0c>
+    <2d93>   DW_AT_abstract_origin: (ref4) <0x3ee9>
     <2d97>   DW_AT_entry_pc    : (addr) 0x2b10
     <2d9f>   DW_AT_GNU_entry_view: (data1) 1
     <2da0>   DW_AT_ranges      : (sec_offset) 0x4a0
     <2da4>   DW_AT_call_file   : (data1) 1
-    <2da5>   DW_AT_call_line   : (data2) 343
+    <2da5>   DW_AT_call_line   : (data2) 356
     <2da7>   DW_AT_call_column : (data1) 13
     <2da8>   DW_AT_sibling     : (ref4) <0x2dda>
  <3><2dac>: Abbrev Number: 62 (DW_TAG_formal_parameter)
-    <2dad>   DW_AT_abstract_origin: (ref4) <0x3e1e>
+    <2dad>   DW_AT_abstract_origin: (ref4) <0x3efb>
  <3><2db1>: Abbrev Number: 63 (DW_TAG_inlined_subroutine)
-    <2db2>   DW_AT_abstract_origin: (ref4) <0x3e62>
+    <2db2>   DW_AT_abstract_origin: (ref4) <0x3f3f>
     <2db6>   DW_AT_entry_pc    : (addr) 0x2b10
     <2dbe>   DW_AT_GNU_entry_view: (data1) 3
     <2dbf>   DW_AT_low_pc      : (addr) 0x2b10
     <2dc7>   DW_AT_high_pc     : (data8) 0xb
     <2dcf>   DW_AT_call_file   : (data1) 2
     <2dd0>   DW_AT_call_line   : (data2) 618
     <2dd2>   DW_AT_call_column : (data1) 5
  <4><2dd3>: Abbrev Number: 62 (DW_TAG_formal_parameter)
-    <2dd4>   DW_AT_abstract_origin: (ref4) <0x3e70>
+    <2dd4>   DW_AT_abstract_origin: (ref4) <0x3f4d>
  <4><2dd8>: Abbrev Number: 0
  <3><2dd9>: Abbrev Number: 0
  <2><2dda>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
     <2ddb>   DW_AT_low_pc      : (addr) 0x2a5a
-    <2de3>   DW_AT_abstract_origin: (ref4) <0x439a>
+    <2de3>   DW_AT_abstract_origin: (ref4) <0x4477>
  <2><2de7>: Abbrev Number: 41 (DW_TAG_GNU_call_site)
     <2de8>   DW_AT_low_pc      : (addr) 0x2b3e
     <2df0>   DW_AT_GNU_tail_call: (flag_present) 1
-    <2df0>   DW_AT_abstract_origin: (ref4) <0x43a6>
+    <2df0>   DW_AT_abstract_origin: (ref4) <0x4483>
  <3><2df4>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
     <2df5>   DW_AT_location    : (exprloc) 1 byte block: 51 	(DW_OP_reg1 (rdx))
     <2df7>   DW_AT_GNU_call_site_value: (exprloc) 3 byte block: f3 1 51 	(DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)))
  <3><2dfb>: Abbrev Number: 0
  <2><2dfc>: Abbrev Number: 0
  <1><2dfd>: Abbrev Number: 64 (DW_TAG_subprogram)
     <2dfe>   DW_AT_external    : (flag_present) 1
     <2dfe>   DW_AT_name        : (strp) (offset: 0x11bc): Cons_repr
     <2e02>   DW_AT_decl_file   : (data1) 1
-    <2e03>   DW_AT_decl_line   : (data1) 242
+    <2e03>   DW_AT_decl_line   : (data1) 255
     <2e04>   DW_AT_decl_column : (data1) 1
     <2e05>   DW_AT_prototyped  : (flag_present) 1
     <2e05>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
     <2e09>   DW_AT_low_pc      : (addr) 0x2710
     <2e11>   DW_AT_high_pc     : (data8) 0x204
     <2e19>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
     <2e1b>   DW_AT_GNU_all_call_sites: (flag_present) 1
-    <2e1b>   DW_AT_sibling     : (ref4) <0x3232>
+    <2e1b>   DW_AT_sibling     : (ref4) <0x3238>
  <2><2e1f>: Abbrev Number: 65 (DW_TAG_formal_parameter)
     <2e20>   DW_AT_name        : (strp) (offset: 0xf72): self
     <2e24>   DW_AT_decl_file   : (data1) 1
-    <2e25>   DW_AT_decl_line   : (data1) 242
+    <2e25>   DW_AT_decl_line   : (data1) 255
     <2e26>   DW_AT_decl_column : (data1) 21
     <2e27>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
     <2e2b>   DW_AT_location    : (sec_offset) 0xbf3 (location list)
     <2e2f>   DW_AT_GNU_locviews: (sec_offset) 0xbeb
- <2><2e33>: Abbrev Number: 38 (DW_TAG_variable)
+ <2><2e33>: Abbrev Number: 39 (DW_TAG_variable)
     <2e34>   DW_AT_name        : (strp) (offset: 0xe32): writer
     <2e38>   DW_AT_decl_file   : (data1) 1
-    <2e39>   DW_AT_decl_line   : (data1) 244
-    <2e3a>   DW_AT_decl_column : (data1) 22
-    <2e3b>   DW_AT_type        : (ref4) <0x1730>, _PyUnicodeWriter
-    <2e3f>   DW_AT_location    : (exprloc) 3 byte block: 91 80 7f 	(DW_OP_fbreg: -128)
- <2><2e43>: Abbrev Number: 66 (DW_TAG_variable)
-    <2e44>   DW_AT_name        : (string) i
-    <2e46>   DW_AT_decl_file   : (data1) 1
-    <2e47>   DW_AT_decl_line   : (data1) 245
-    <2e48>   DW_AT_decl_column : (data1) 16
-    <2e49>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
-    <2e4d>   DW_AT_location    : (sec_offset) 0xc58 (location list)
-    <2e51>   DW_AT_GNU_locviews: (sec_offset) 0xc52
- <2><2e55>: Abbrev Number: 67 (DW_TAG_variable)
-    <2e56>   DW_AT_name        : (strp) (offset: 0x23a9): next
-    <2e5a>   DW_AT_decl_file   : (data1) 1
-    <2e5b>   DW_AT_decl_line   : (data1) 246
-    <2e5c>   DW_AT_decl_column : (data1) 15
-    <2e5d>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <2e61>   DW_AT_location    : (sec_offset) 0xca5 (location list)
-    <2e65>   DW_AT_GNU_locviews: (sec_offset) 0xca1
- <2><2e69>: Abbrev Number: 66 (DW_TAG_variable)
-    <2e6a>   DW_AT_name        : (string) m
-    <2e6c>   DW_AT_decl_file   : (data1) 1
-    <2e6d>   DW_AT_decl_line   : (data1) 247
-    <2e6e>   DW_AT_decl_column : (data1) 15
-    <2e6f>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <2e73>   DW_AT_location    : (sec_offset) 0xcdd (location list)
-    <2e77>   DW_AT_GNU_locviews: (sec_offset) 0xcdb
- <2><2e7b>: Abbrev Number: 67 (DW_TAG_variable)
-    <2e7c>   DW_AT_name        : (strp) (offset: 0x58c): state
-    <2e80>   DW_AT_decl_file   : (data1) 1
-    <2e81>   DW_AT_decl_line   : (data1) 251
-    <2e82>   DW_AT_decl_column : (data1) 23
-    <2e83>   DW_AT_type        : (ref4) <0x274d>, consmodule_state
-    <2e87>   DW_AT_location    : (sec_offset) 0xd06 (location list)
-    <2e8b>   DW_AT_GNU_locviews: (sec_offset) 0xd00
- <2><2e8f>: Abbrev Number: 67 (DW_TAG_variable)
-    <2e90>   DW_AT_name        : (strp) (offset: 0x2327): cons
-    <2e94>   DW_AT_decl_file   : (data1) 1
-    <2e95>   DW_AT_decl_line   : (data1) 255
-    <2e96>   DW_AT_decl_column : (data1) 19
-    <2e97>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
-    <2e9b>   DW_AT_location    : (sec_offset) 0xd53 (location list)
-    <2e9f>   DW_AT_GNU_locviews: (sec_offset) 0xd4f
- <2><2ea3>: Abbrev Number: 68 (DW_TAG_label)
-    <2ea4>   DW_AT_name        : (strp) (offset: 0x64c): error
-    <2ea8>   DW_AT_decl_file   : (data1) 1
-    <2ea9>   DW_AT_decl_line   : (data2) 306
-    <2eab>   DW_AT_decl_column : (data1) 1
-    <2eac>   DW_AT_low_pc      : (addr) 0x2858
- <2><2eb4>: Abbrev Number: 45 (DW_TAG_variable)
-    <2eb5>   DW_AT_name        : (strp) (offset: 0x652): head
-    <2eb9>   DW_AT_decl_file   : (data1) 1
-    <2eba>   DW_AT_decl_line   : (data2) 267
-    <2ebc>   DW_AT_decl_column : (data1) 15
-    <2ebd>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <2ec1>   DW_AT_location    : (sec_offset) 0xd8b (location list)
-    <2ec5>   DW_AT_GNU_locviews: (sec_offset) 0xd89
- <2><2ec9>: Abbrev Number: 45 (DW_TAG_variable)
-    <2eca>   DW_AT_name        : (strp) (offset: 0x1e98): repr
-    <2ece>   DW_AT_decl_file   : (data1) 1
-    <2ecf>   DW_AT_decl_line   : (data2) 267
-    <2ed1>   DW_AT_decl_column : (data1) 29
-    <2ed2>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <2ed6>   DW_AT_location    : (sec_offset) 0xdbd (location list)
-    <2eda>   DW_AT_GNU_locviews: (sec_offset) 0xdaf
- <2><2ede>: Abbrev Number: 45 (DW_TAG_variable)
-    <2edf>   DW_AT_name        : (strp) (offset: 0x203b): tail
-    <2ee3>   DW_AT_decl_file   : (data1) 1
-    <2ee4>   DW_AT_decl_line   : (data2) 267
-    <2ee6>   DW_AT_decl_column : (data1) 43
-    <2ee7>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <2eeb>   DW_AT_location    : (sec_offset) 0xe58 (location list)
-    <2eef>   DW_AT_GNU_locviews: (sec_offset) 0xe54
- <2><2ef3>: Abbrev Number: 61 (DW_TAG_inlined_subroutine)
-    <2ef4>   DW_AT_abstract_origin: (ref4) <0x3ea9>
-    <2ef8>   DW_AT_entry_pc    : (addr) 0x27de
-    <2f00>   DW_AT_GNU_entry_view: (data1) 1
-    <2f01>   DW_AT_low_pc      : (addr) 0x27de
-    <2f09>   DW_AT_high_pc     : (data8) 0
-    <2f11>   DW_AT_call_file   : (data1) 1
-    <2f12>   DW_AT_call_line   : (data2) 282
-    <2f14>   DW_AT_call_column : (data1) 19
-    <2f15>   DW_AT_sibling     : (ref4) <0x2f34>
- <3><2f19>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <2f1a>   DW_AT_abstract_origin: (ref4) <0x3ec5>
-    <2f1e>   DW_AT_location    : (sec_offset) 0xe90 (location list)
-    <2f22>   DW_AT_GNU_locviews: (sec_offset) 0xe8e
- <3><2f26>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <2f27>   DW_AT_abstract_origin: (ref4) <0x3eba>
-    <2f2b>   DW_AT_location    : (sec_offset) 0xeb5 (location list)
-    <2f2f>   DW_AT_GNU_locviews: (sec_offset) 0xeb3
- <3><2f33>: Abbrev Number: 0
- <2><2f34>: Abbrev Number: 61 (DW_TAG_inlined_subroutine)
-    <2f35>   DW_AT_abstract_origin: (ref4) <0x3ea9>
-    <2f39>   DW_AT_entry_pc    : (addr) 0x27f9
-    <2f41>   DW_AT_GNU_entry_view: (data1) 1
-    <2f42>   DW_AT_low_pc      : (addr) 0x27f9
-    <2f4a>   DW_AT_high_pc     : (data8) 0
-    <2f52>   DW_AT_call_file   : (data1) 1
-    <2f53>   DW_AT_call_line   : (data2) 268
-    <2f55>   DW_AT_call_column : (data1) 12
-    <2f56>   DW_AT_sibling     : (ref4) <0x2f75>
- <3><2f5a>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <2f5b>   DW_AT_abstract_origin: (ref4) <0x3ec5>
-    <2f5f>   DW_AT_location    : (sec_offset) 0xeda (location list)
-    <2f63>   DW_AT_GNU_locviews: (sec_offset) 0xed8
- <3><2f67>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <2f68>   DW_AT_abstract_origin: (ref4) <0x3eba>
-    <2f6c>   DW_AT_location    : (sec_offset) 0xeff (location list)
-    <2f70>   DW_AT_GNU_locviews: (sec_offset) 0xefd
- <3><2f74>: Abbrev Number: 0
- <2><2f75>: Abbrev Number: 69 (DW_TAG_inlined_subroutine)
-    <2f76>   DW_AT_abstract_origin: (ref4) <0x3e47>
-    <2f7a>   DW_AT_low_pc      : (addr) 0x2821
-    <2f82>   DW_AT_high_pc     : (data8) 0x4
-    <2f8a>   DW_AT_call_file   : (data1) 1
-    <2f8b>   DW_AT_call_line   : (data2) 274
-    <2f8d>   DW_AT_call_column : (data1) 13
-    <2f8e>   DW_AT_sibling     : (ref4) <0x2f98>
- <3><2f92>: Abbrev Number: 62 (DW_TAG_formal_parameter)
-    <2f93>   DW_AT_abstract_origin: (ref4) <0x3e55>
- <3><2f97>: Abbrev Number: 0
- <2><2f98>: Abbrev Number: 61 (DW_TAG_inlined_subroutine)
-    <2f99>   DW_AT_abstract_origin: (ref4) <0x3e47>
-    <2f9d>   DW_AT_entry_pc    : (addr) 0x2827
-    <2fa5>   DW_AT_GNU_entry_view: (data1) 2
-    <2fa6>   DW_AT_low_pc      : (addr) 0x2827
-    <2fae>   DW_AT_high_pc     : (data8) 0x19
-    <2fb6>   DW_AT_call_file   : (data1) 1
-    <2fb7>   DW_AT_call_line   : (data2) 277
-    <2fb9>   DW_AT_call_column : (data1) 9
-    <2fba>   DW_AT_sibling     : (ref4) <0x2fe0>
- <3><2fbe>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <2fbf>   DW_AT_abstract_origin: (ref4) <0x3e55>
-    <2fc3>   DW_AT_location    : (sec_offset) 0xf24 (location list)
-    <2fc7>   DW_AT_GNU_locviews: (sec_offset) 0xf22
- <3><2fcb>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
-    <2fcc>   DW_AT_low_pc      : (addr) 0x2839
-    <2fd4>   DW_AT_abstract_origin: (ref4) <0x4338>
- <4><2fd8>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <2fd9>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <2fdb>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
- <4><2fde>: Abbrev Number: 0
- <3><2fdf>: Abbrev Number: 0
- <2><2fe0>: Abbrev Number: 57 (DW_TAG_inlined_subroutine)
-    <2fe1>   DW_AT_abstract_origin: (ref4) <0x3e47>
-    <2fe5>   DW_AT_entry_pc    : (addr) 0x2840
-    <2fed>   DW_AT_GNU_entry_view: (data1) 3
-    <2fee>   DW_AT_ranges      : (sec_offset) 0x320
-    <2ff2>   DW_AT_call_file   : (data1) 1
-    <2ff3>   DW_AT_call_line   : (data2) 289
-    <2ff5>   DW_AT_call_column : (data1) 17
-    <2ff6>   DW_AT_sibling     : (ref4) <0x301c>
- <3><2ffa>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <2ffb>   DW_AT_abstract_origin: (ref4) <0x3e55>
-    <2fff>   DW_AT_location    : (sec_offset) 0xf49 (location list)
-    <3003>   DW_AT_GNU_locviews: (sec_offset) 0xf47
- <3><3007>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
-    <3008>   DW_AT_low_pc      : (addr) 0x2852
-    <3010>   DW_AT_abstract_origin: (ref4) <0x4338>
- <4><3014>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3015>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <3017>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
- <4><301a>: Abbrev Number: 0
- <3><301b>: Abbrev Number: 0
- <2><301c>: Abbrev Number: 61 (DW_TAG_inlined_subroutine)
-    <301d>   DW_AT_abstract_origin: (ref4) <0x3e47>
-    <3021>   DW_AT_entry_pc    : (addr) 0x28c7
-    <3029>   DW_AT_GNU_entry_view: (data1) 2
-    <302a>   DW_AT_low_pc      : (addr) 0x28c7
-    <3032>   DW_AT_high_pc     : (data8) 0x19
-    <303a>   DW_AT_call_file   : (data1) 1
-    <303b>   DW_AT_call_line   : (data2) 292
-    <303d>   DW_AT_call_column : (data1) 13
-    <303e>   DW_AT_sibling     : (ref4) <0x3064>
- <3><3042>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <3043>   DW_AT_abstract_origin: (ref4) <0x3e55>
-    <3047>   DW_AT_location    : (sec_offset) 0xf6e (location list)
-    <304b>   DW_AT_GNU_locviews: (sec_offset) 0xf6c
- <3><304f>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
-    <3050>   DW_AT_low_pc      : (addr) 0x28d9
-    <3058>   DW_AT_abstract_origin: (ref4) <0x4338>
- <4><305c>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <305d>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <305f>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
- <4><3062>: Abbrev Number: 0
- <3><3063>: Abbrev Number: 0
- <2><3064>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <3065>   DW_AT_low_pc      : (addr) 0x2741
-    <306d>   DW_AT_abstract_origin: (ref4) <0x43b3>
-    <3071>   DW_AT_sibling     : (ref4) <0x3083>
- <3><3075>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3076>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <3078>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 20 51 0 0 0 0 0 0 	(DW_OP_addr: 5120)
- <3><3082>: Abbrev Number: 0
- <2><3083>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
-    <3084>   DW_AT_low_pc      : (addr) 0x274e
-    <308c>   DW_AT_abstract_origin: (ref4) <0x4345>
- <2><3090>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <3091>   DW_AT_low_pc      : (addr) 0x2762
-    <3099>   DW_AT_abstract_origin: (ref4) <0x43c0>
-    <309d>   DW_AT_sibling     : (ref4) <0x30a8>
- <3><30a1>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <30a2>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <30a4>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7e 0 	(DW_OP_breg14 (r14): 0)
- <3><30a7>: Abbrev Number: 0
- <2><30a8>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <30a9>   DW_AT_low_pc      : (addr) 0x27a3
-    <30b1>   DW_AT_abstract_origin: (ref4) <0x43cd>
-    <30b5>   DW_AT_sibling     : (ref4) <0x30c0>
- <3><30b9>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <30ba>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <30bc>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 77 0 	(DW_OP_breg7 (rsp): 0)
- <3><30bf>: Abbrev Number: 0
- <2><30c0>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <30c1>   DW_AT_low_pc      : (addr) 0x27be
-    <30c9>   DW_AT_abstract_origin: (ref4) <0x43da>
-    <30cd>   DW_AT_sibling     : (ref4) <0x30de>
- <3><30d1>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <30d2>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <30d4>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 77 0 	(DW_OP_breg7 (rsp): 0)
+    <2e39>   DW_AT_decl_line   : (data2) 257
+    <2e3b>   DW_AT_decl_column : (data1) 22
+    <2e3c>   DW_AT_type        : (ref4) <0x1730>, _PyUnicodeWriter
+    <2e40>   DW_AT_location    : (exprloc) 3 byte block: 91 80 7f 	(DW_OP_fbreg: -128)
+ <2><2e44>: Abbrev Number: 56 (DW_TAG_variable)
+    <2e45>   DW_AT_name        : (string) i
+    <2e47>   DW_AT_decl_file   : (data1) 1
+    <2e48>   DW_AT_decl_line   : (data2) 258
+    <2e4a>   DW_AT_decl_column : (data1) 16
+    <2e4b>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
+    <2e4f>   DW_AT_location    : (sec_offset) 0xc58 (location list)
+    <2e53>   DW_AT_GNU_locviews: (sec_offset) 0xc52
+ <2><2e57>: Abbrev Number: 45 (DW_TAG_variable)
+    <2e58>   DW_AT_name        : (strp) (offset: 0x23a9): next
+    <2e5c>   DW_AT_decl_file   : (data1) 1
+    <2e5d>   DW_AT_decl_line   : (data2) 259
+    <2e5f>   DW_AT_decl_column : (data1) 15
+    <2e60>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <2e64>   DW_AT_location    : (sec_offset) 0xca5 (location list)
+    <2e68>   DW_AT_GNU_locviews: (sec_offset) 0xca1
+ <2><2e6c>: Abbrev Number: 56 (DW_TAG_variable)
+    <2e6d>   DW_AT_name        : (string) m
+    <2e6f>   DW_AT_decl_file   : (data1) 1
+    <2e70>   DW_AT_decl_line   : (data2) 260
+    <2e72>   DW_AT_decl_column : (data1) 15
+    <2e73>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <2e77>   DW_AT_location    : (sec_offset) 0xcdd (location list)
+    <2e7b>   DW_AT_GNU_locviews: (sec_offset) 0xcdb
+ <2><2e7f>: Abbrev Number: 45 (DW_TAG_variable)
+    <2e80>   DW_AT_name        : (strp) (offset: 0x58c): state
+    <2e84>   DW_AT_decl_file   : (data1) 1
+    <2e85>   DW_AT_decl_line   : (data2) 264
+    <2e87>   DW_AT_decl_column : (data1) 23
+    <2e88>   DW_AT_type        : (ref4) <0x274d>, consmodule_state
+    <2e8c>   DW_AT_location    : (sec_offset) 0xd06 (location list)
+    <2e90>   DW_AT_GNU_locviews: (sec_offset) 0xd00
+ <2><2e94>: Abbrev Number: 45 (DW_TAG_variable)
+    <2e95>   DW_AT_name        : (strp) (offset: 0x2327): cons
+    <2e99>   DW_AT_decl_file   : (data1) 1
+    <2e9a>   DW_AT_decl_line   : (data2) 268
+    <2e9c>   DW_AT_decl_column : (data1) 19
+    <2e9d>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
+    <2ea1>   DW_AT_location    : (sec_offset) 0xd53 (location list)
+    <2ea5>   DW_AT_GNU_locviews: (sec_offset) 0xd4f
+ <2><2ea9>: Abbrev Number: 66 (DW_TAG_label)
+    <2eaa>   DW_AT_name        : (strp) (offset: 0x64c): error
+    <2eae>   DW_AT_decl_file   : (data1) 1
+    <2eaf>   DW_AT_decl_line   : (data2) 319
+    <2eb1>   DW_AT_decl_column : (data1) 1
+    <2eb2>   DW_AT_low_pc      : (addr) 0x2858
+ <2><2eba>: Abbrev Number: 45 (DW_TAG_variable)
+    <2ebb>   DW_AT_name        : (strp) (offset: 0x652): head
+    <2ebf>   DW_AT_decl_file   : (data1) 1
+    <2ec0>   DW_AT_decl_line   : (data2) 280
+    <2ec2>   DW_AT_decl_column : (data1) 15
+    <2ec3>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <2ec7>   DW_AT_location    : (sec_offset) 0xd8b (location list)
+    <2ecb>   DW_AT_GNU_locviews: (sec_offset) 0xd89
+ <2><2ecf>: Abbrev Number: 45 (DW_TAG_variable)
+    <2ed0>   DW_AT_name        : (strp) (offset: 0x1e98): repr
+    <2ed4>   DW_AT_decl_file   : (data1) 1
+    <2ed5>   DW_AT_decl_line   : (data2) 280
+    <2ed7>   DW_AT_decl_column : (data1) 29
+    <2ed8>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <2edc>   DW_AT_location    : (sec_offset) 0xdbd (location list)
+    <2ee0>   DW_AT_GNU_locviews: (sec_offset) 0xdaf
+ <2><2ee4>: Abbrev Number: 45 (DW_TAG_variable)
+    <2ee5>   DW_AT_name        : (strp) (offset: 0x203b): tail
+    <2ee9>   DW_AT_decl_file   : (data1) 1
+    <2eea>   DW_AT_decl_line   : (data2) 280
+    <2eec>   DW_AT_decl_column : (data1) 43
+    <2eed>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <2ef1>   DW_AT_location    : (sec_offset) 0xe58 (location list)
+    <2ef5>   DW_AT_GNU_locviews: (sec_offset) 0xe54
+ <2><2ef9>: Abbrev Number: 61 (DW_TAG_inlined_subroutine)
+    <2efa>   DW_AT_abstract_origin: (ref4) <0x3f86>
+    <2efe>   DW_AT_entry_pc    : (addr) 0x27de
+    <2f06>   DW_AT_GNU_entry_view: (data1) 1
+    <2f07>   DW_AT_low_pc      : (addr) 0x27de
+    <2f0f>   DW_AT_high_pc     : (data8) 0
+    <2f17>   DW_AT_call_file   : (data1) 1
+    <2f18>   DW_AT_call_line   : (data2) 295
+    <2f1a>   DW_AT_call_column : (data1) 19
+    <2f1b>   DW_AT_sibling     : (ref4) <0x2f3a>
+ <3><2f1f>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <2f20>   DW_AT_abstract_origin: (ref4) <0x3fa2>
+    <2f24>   DW_AT_location    : (sec_offset) 0xe90 (location list)
+    <2f28>   DW_AT_GNU_locviews: (sec_offset) 0xe8e
+ <3><2f2c>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <2f2d>   DW_AT_abstract_origin: (ref4) <0x3f97>
+    <2f31>   DW_AT_location    : (sec_offset) 0xeb5 (location list)
+    <2f35>   DW_AT_GNU_locviews: (sec_offset) 0xeb3
+ <3><2f39>: Abbrev Number: 0
+ <2><2f3a>: Abbrev Number: 61 (DW_TAG_inlined_subroutine)
+    <2f3b>   DW_AT_abstract_origin: (ref4) <0x3f86>
+    <2f3f>   DW_AT_entry_pc    : (addr) 0x27f9
+    <2f47>   DW_AT_GNU_entry_view: (data1) 1
+    <2f48>   DW_AT_low_pc      : (addr) 0x27f9
+    <2f50>   DW_AT_high_pc     : (data8) 0
+    <2f58>   DW_AT_call_file   : (data1) 1
+    <2f59>   DW_AT_call_line   : (data2) 281
+    <2f5b>   DW_AT_call_column : (data1) 12
+    <2f5c>   DW_AT_sibling     : (ref4) <0x2f7b>
+ <3><2f60>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <2f61>   DW_AT_abstract_origin: (ref4) <0x3fa2>
+    <2f65>   DW_AT_location    : (sec_offset) 0xeda (location list)
+    <2f69>   DW_AT_GNU_locviews: (sec_offset) 0xed8
+ <3><2f6d>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <2f6e>   DW_AT_abstract_origin: (ref4) <0x3f97>
+    <2f72>   DW_AT_location    : (sec_offset) 0xeff (location list)
+    <2f76>   DW_AT_GNU_locviews: (sec_offset) 0xefd
+ <3><2f7a>: Abbrev Number: 0
+ <2><2f7b>: Abbrev Number: 67 (DW_TAG_inlined_subroutine)
+    <2f7c>   DW_AT_abstract_origin: (ref4) <0x3f24>
+    <2f80>   DW_AT_low_pc      : (addr) 0x2821
+    <2f88>   DW_AT_high_pc     : (data8) 0x4
+    <2f90>   DW_AT_call_file   : (data1) 1
+    <2f91>   DW_AT_call_line   : (data2) 287
+    <2f93>   DW_AT_call_column : (data1) 13
+    <2f94>   DW_AT_sibling     : (ref4) <0x2f9e>
+ <3><2f98>: Abbrev Number: 62 (DW_TAG_formal_parameter)
+    <2f99>   DW_AT_abstract_origin: (ref4) <0x3f32>
+ <3><2f9d>: Abbrev Number: 0
+ <2><2f9e>: Abbrev Number: 61 (DW_TAG_inlined_subroutine)
+    <2f9f>   DW_AT_abstract_origin: (ref4) <0x3f24>
+    <2fa3>   DW_AT_entry_pc    : (addr) 0x2827
+    <2fab>   DW_AT_GNU_entry_view: (data1) 2
+    <2fac>   DW_AT_low_pc      : (addr) 0x2827
+    <2fb4>   DW_AT_high_pc     : (data8) 0x19
+    <2fbc>   DW_AT_call_file   : (data1) 1
+    <2fbd>   DW_AT_call_line   : (data2) 290
+    <2fbf>   DW_AT_call_column : (data1) 9
+    <2fc0>   DW_AT_sibling     : (ref4) <0x2fe6>
+ <3><2fc4>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <2fc5>   DW_AT_abstract_origin: (ref4) <0x3f32>
+    <2fc9>   DW_AT_location    : (sec_offset) 0xf24 (location list)
+    <2fcd>   DW_AT_GNU_locviews: (sec_offset) 0xf22
+ <3><2fd1>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
+    <2fd2>   DW_AT_low_pc      : (addr) 0x2839
+    <2fda>   DW_AT_abstract_origin: (ref4) <0x4415>
+ <4><2fde>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <2fdf>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <2fe1>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <4><2fe4>: Abbrev Number: 0
+ <3><2fe5>: Abbrev Number: 0
+ <2><2fe6>: Abbrev Number: 57 (DW_TAG_inlined_subroutine)
+    <2fe7>   DW_AT_abstract_origin: (ref4) <0x3f24>
+    <2feb>   DW_AT_entry_pc    : (addr) 0x2840
+    <2ff3>   DW_AT_GNU_entry_view: (data1) 3
+    <2ff4>   DW_AT_ranges      : (sec_offset) 0x320
+    <2ff8>   DW_AT_call_file   : (data1) 1
+    <2ff9>   DW_AT_call_line   : (data2) 302
+    <2ffb>   DW_AT_call_column : (data1) 17
+    <2ffc>   DW_AT_sibling     : (ref4) <0x3022>
+ <3><3000>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <3001>   DW_AT_abstract_origin: (ref4) <0x3f32>
+    <3005>   DW_AT_location    : (sec_offset) 0xf49 (location list)
+    <3009>   DW_AT_GNU_locviews: (sec_offset) 0xf47
+ <3><300d>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
+    <300e>   DW_AT_low_pc      : (addr) 0x2852
+    <3016>   DW_AT_abstract_origin: (ref4) <0x4415>
+ <4><301a>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <301b>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <301d>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <4><3020>: Abbrev Number: 0
+ <3><3021>: Abbrev Number: 0
+ <2><3022>: Abbrev Number: 61 (DW_TAG_inlined_subroutine)
+    <3023>   DW_AT_abstract_origin: (ref4) <0x3f24>
+    <3027>   DW_AT_entry_pc    : (addr) 0x28c7
+    <302f>   DW_AT_GNU_entry_view: (data1) 2
+    <3030>   DW_AT_low_pc      : (addr) 0x28c7
+    <3038>   DW_AT_high_pc     : (data8) 0x19
+    <3040>   DW_AT_call_file   : (data1) 1
+    <3041>   DW_AT_call_line   : (data2) 305
+    <3043>   DW_AT_call_column : (data1) 13
+    <3044>   DW_AT_sibling     : (ref4) <0x306a>
+ <3><3048>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <3049>   DW_AT_abstract_origin: (ref4) <0x3f32>
+    <304d>   DW_AT_location    : (sec_offset) 0xf6e (location list)
+    <3051>   DW_AT_GNU_locviews: (sec_offset) 0xf6c
+ <3><3055>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
+    <3056>   DW_AT_low_pc      : (addr) 0x28d9
+    <305e>   DW_AT_abstract_origin: (ref4) <0x4415>
+ <4><3062>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3063>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3065>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <4><3068>: Abbrev Number: 0
+ <3><3069>: Abbrev Number: 0
+ <2><306a>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <306b>   DW_AT_low_pc      : (addr) 0x2741
+    <3073>   DW_AT_abstract_origin: (ref4) <0x4490>
+    <3077>   DW_AT_sibling     : (ref4) <0x3089>
+ <3><307b>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <307c>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <307e>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 20 51 0 0 0 0 0 0 	(DW_OP_addr: 5120)
+ <3><3088>: Abbrev Number: 0
+ <2><3089>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
+    <308a>   DW_AT_low_pc      : (addr) 0x274e
+    <3092>   DW_AT_abstract_origin: (ref4) <0x4422>
+ <2><3096>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <3097>   DW_AT_low_pc      : (addr) 0x2762
+    <309f>   DW_AT_abstract_origin: (ref4) <0x449d>
+    <30a3>   DW_AT_sibling     : (ref4) <0x30ae>
+ <3><30a7>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <30a8>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <30aa>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7e 0 	(DW_OP_breg14 (r14): 0)
+ <3><30ad>: Abbrev Number: 0
+ <2><30ae>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <30af>   DW_AT_low_pc      : (addr) 0x27a3
+    <30b7>   DW_AT_abstract_origin: (ref4) <0x44aa>
+    <30bb>   DW_AT_sibling     : (ref4) <0x30c6>
+ <3><30bf>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <30c0>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <30c2>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 77 0 	(DW_OP_breg7 (rsp): 0)
+ <3><30c5>: Abbrev Number: 0
+ <2><30c6>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <30c7>   DW_AT_low_pc      : (addr) 0x27be
+    <30cf>   DW_AT_abstract_origin: (ref4) <0x44b7>
+    <30d3>   DW_AT_sibling     : (ref4) <0x30e4>
  <3><30d7>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <30d8>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <30da>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 8 28 	(DW_OP_const1u: 40)
- <3><30dd>: Abbrev Number: 0
- <2><30de>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <30df>   DW_AT_low_pc      : (addr) 0x27f5
-    <30e7>   DW_AT_abstract_origin: (ref4) <0x43da>
-    <30eb>   DW_AT_sibling     : (ref4) <0x30fc>
- <3><30ef>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <30f0>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <30f2>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 77 0 	(DW_OP_breg7 (rsp): 0)
+    <30d8>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <30da>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 77 0 	(DW_OP_breg7 (rsp): 0)
+ <3><30dd>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <30de>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <30e0>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 8 28 	(DW_OP_const1u: 40)
+ <3><30e3>: Abbrev Number: 0
+ <2><30e4>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <30e5>   DW_AT_low_pc      : (addr) 0x27f5
+    <30ed>   DW_AT_abstract_origin: (ref4) <0x44b7>
+    <30f1>   DW_AT_sibling     : (ref4) <0x3102>
  <3><30f5>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <30f6>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <30f8>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 8 20 	(DW_OP_const1u: 32)
- <3><30fb>: Abbrev Number: 0
- <2><30fc>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
-    <30fd>   DW_AT_low_pc      : (addr) 0x280c
-    <3105>   DW_AT_abstract_origin: (ref4) <0x43e7>
- <2><3109>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <310a>   DW_AT_low_pc      : (addr) 0x281f
-    <3112>   DW_AT_abstract_origin: (ref4) <0x43f4>
-    <3116>   DW_AT_sibling     : (ref4) <0x3127>
- <3><311a>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <311b>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <311d>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 77 0 	(DW_OP_breg7 (rsp): 0)
+    <30f6>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <30f8>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 77 0 	(DW_OP_breg7 (rsp): 0)
+ <3><30fb>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <30fc>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <30fe>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 8 20 	(DW_OP_const1u: 32)
+ <3><3101>: Abbrev Number: 0
+ <2><3102>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
+    <3103>   DW_AT_low_pc      : (addr) 0x280c
+    <310b>   DW_AT_abstract_origin: (ref4) <0x44c4>
+ <2><310f>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <3110>   DW_AT_low_pc      : (addr) 0x281f
+    <3118>   DW_AT_abstract_origin: (ref4) <0x44d1>
+    <311c>   DW_AT_sibling     : (ref4) <0x312d>
  <3><3120>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3121>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <3123>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
- <3><3126>: Abbrev Number: 0
- <2><3127>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <3128>   DW_AT_low_pc      : (addr) 0x2860
-    <3130>   DW_AT_abstract_origin: (ref4) <0x4401>
-    <3134>   DW_AT_sibling     : (ref4) <0x313f>
- <3><3138>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3139>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <313b>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 77 0 	(DW_OP_breg7 (rsp): 0)
- <3><313e>: Abbrev Number: 0
- <2><313f>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <3140>   DW_AT_low_pc      : (addr) 0x2868
-    <3148>   DW_AT_abstract_origin: (ref4) <0x440e>
-    <314c>   DW_AT_sibling     : (ref4) <0x3157>
- <3><3150>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3151>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <3153>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7e 0 	(DW_OP_breg14 (r14): 0)
- <3><3156>: Abbrev Number: 0
- <2><3157>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <3158>   DW_AT_low_pc      : (addr) 0x287e
-    <3160>   DW_AT_abstract_origin: (ref4) <0x441b>
-    <3164>   DW_AT_sibling     : (ref4) <0x3176>
- <3><3168>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3169>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <316b>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 9 30 0 0 0 0 0 0 	(DW_OP_addr: 3009)
- <3><3175>: Abbrev Number: 0
- <2><3176>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <3177>   DW_AT_low_pc      : (addr) 0x289c
-    <317f>   DW_AT_abstract_origin: (ref4) <0x4428>
-    <3183>   DW_AT_sibling     : (ref4) <0x31a0>
- <3><3187>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3188>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <318a>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 77 0 	(DW_OP_breg7 (rsp): 0)
+    <3121>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3123>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 77 0 	(DW_OP_breg7 (rsp): 0)
+ <3><3126>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3127>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <3129>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <3><312c>: Abbrev Number: 0
+ <2><312d>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <312e>   DW_AT_low_pc      : (addr) 0x2860
+    <3136>   DW_AT_abstract_origin: (ref4) <0x44de>
+    <313a>   DW_AT_sibling     : (ref4) <0x3145>
+ <3><313e>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <313f>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3141>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 77 0 	(DW_OP_breg7 (rsp): 0)
+ <3><3144>: Abbrev Number: 0
+ <2><3145>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <3146>   DW_AT_low_pc      : (addr) 0x2868
+    <314e>   DW_AT_abstract_origin: (ref4) <0x44eb>
+    <3152>   DW_AT_sibling     : (ref4) <0x315d>
+ <3><3156>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3157>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3159>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7e 0 	(DW_OP_breg14 (r14): 0)
+ <3><315c>: Abbrev Number: 0
+ <2><315d>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <315e>   DW_AT_low_pc      : (addr) 0x287e
+    <3166>   DW_AT_abstract_origin: (ref4) <0x44f8>
+    <316a>   DW_AT_sibling     : (ref4) <0x317c>
+ <3><316e>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <316f>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3171>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 9 30 0 0 0 0 0 0 	(DW_OP_addr: 3009)
+ <3><317b>: Abbrev Number: 0
+ <2><317c>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <317d>   DW_AT_low_pc      : (addr) 0x289c
+    <3185>   DW_AT_abstract_origin: (ref4) <0x4505>
+    <3189>   DW_AT_sibling     : (ref4) <0x31a6>
  <3><318d>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <318e>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <3190>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 d 30 0 0 0 0 0 0 	(DW_OP_addr: 300d)
- <3><319a>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <319b>   DW_AT_location    : (exprloc) 1 byte block: 51 	(DW_OP_reg1 (rdx))
-    <319d>   DW_AT_GNU_call_site_value: (exprloc) 1 byte block: 33 	(DW_OP_lit3)
- <3><319f>: Abbrev Number: 0
- <2><31a0>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <31a1>   DW_AT_low_pc      : (addr) 0x28a8
-    <31a9>   DW_AT_abstract_origin: (ref4) <0x43e7>
-    <31ad>   DW_AT_sibling     : (ref4) <0x31b8>
- <3><31b1>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <31b2>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <31b4>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7f 0 	(DW_OP_breg15 (r15): 0)
- <3><31b7>: Abbrev Number: 0
- <2><31b8>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <31b9>   DW_AT_low_pc      : (addr) 0x28bb
-    <31c1>   DW_AT_abstract_origin: (ref4) <0x43f4>
-    <31c5>   DW_AT_sibling     : (ref4) <0x31d6>
- <3><31c9>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <31ca>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <31cc>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 77 0 	(DW_OP_breg7 (rsp): 0)
+    <318e>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3190>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 77 0 	(DW_OP_breg7 (rsp): 0)
+ <3><3193>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3194>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <3196>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 d 30 0 0 0 0 0 0 	(DW_OP_addr: 300d)
+ <3><31a0>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <31a1>   DW_AT_location    : (exprloc) 1 byte block: 51 	(DW_OP_reg1 (rdx))
+    <31a3>   DW_AT_GNU_call_site_value: (exprloc) 1 byte block: 33 	(DW_OP_lit3)
+ <3><31a5>: Abbrev Number: 0
+ <2><31a6>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <31a7>   DW_AT_low_pc      : (addr) 0x28a8
+    <31af>   DW_AT_abstract_origin: (ref4) <0x44c4>
+    <31b3>   DW_AT_sibling     : (ref4) <0x31be>
+ <3><31b7>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <31b8>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <31ba>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7f 0 	(DW_OP_breg15 (r15): 0)
+ <3><31bd>: Abbrev Number: 0
+ <2><31be>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <31bf>   DW_AT_low_pc      : (addr) 0x28bb
+    <31c7>   DW_AT_abstract_origin: (ref4) <0x44d1>
+    <31cb>   DW_AT_sibling     : (ref4) <0x31dc>
  <3><31cf>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <31d0>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <31d2>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
- <3><31d5>: Abbrev Number: 0
- <2><31d6>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <31d7>   DW_AT_low_pc      : (addr) 0x28f2
-    <31df>   DW_AT_abstract_origin: (ref4) <0x43da>
-    <31e3>   DW_AT_sibling     : (ref4) <0x31f4>
- <3><31e7>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <31e8>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <31ea>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 77 0 	(DW_OP_breg7 (rsp): 0)
+    <31d0>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <31d2>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 77 0 	(DW_OP_breg7 (rsp): 0)
+ <3><31d5>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <31d6>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <31d8>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <3><31db>: Abbrev Number: 0
+ <2><31dc>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <31dd>   DW_AT_low_pc      : (addr) 0x28f2
+    <31e5>   DW_AT_abstract_origin: (ref4) <0x44b7>
+    <31e9>   DW_AT_sibling     : (ref4) <0x31fa>
  <3><31ed>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <31ee>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <31f0>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 8 29 	(DW_OP_const1u: 41)
- <3><31f3>: Abbrev Number: 0
- <2><31f4>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <31f5>   DW_AT_low_pc      : (addr) 0x2902
-    <31fd>   DW_AT_abstract_origin: (ref4) <0x440e>
-    <3201>   DW_AT_sibling     : (ref4) <0x320c>
- <3><3205>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3206>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <3208>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7e 0 	(DW_OP_breg14 (r14): 0)
- <3><320b>: Abbrev Number: 0
- <2><320c>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <320d>   DW_AT_low_pc      : (addr) 0x290a
-    <3215>   DW_AT_abstract_origin: (ref4) <0x4435>
-    <3219>   DW_AT_sibling     : (ref4) <0x3224>
- <3><321d>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <321e>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <3220>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 77 0 	(DW_OP_breg7 (rsp): 0)
- <3><3223>: Abbrev Number: 0
- <2><3224>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
-    <3225>   DW_AT_low_pc      : (addr) 0x2914
-    <322d>   DW_AT_abstract_origin: (ref4) <0x4442>
- <2><3231>: Abbrev Number: 0
- <1><3232>: Abbrev Number: 70 (DW_TAG_subprogram)
-    <3233>   DW_AT_external    : (flag_present) 1
-    <3233>   DW_AT_name        : (strp) (offset: 0x995): Cons_to_list
-    <3237>   DW_AT_decl_file   : (data1) 1
-    <3238>   DW_AT_decl_line   : (data1) 219
-    <3239>   DW_AT_decl_column : (data1) 1
-    <323a>   DW_AT_prototyped  : (flag_present) 1
-    <323a>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <323e>   DW_AT_inline      : (data1) 1	(inlined)
-    <323f>   DW_AT_sibling     : (ref4) <0x32b0>
- <2><3243>: Abbrev Number: 71 (DW_TAG_formal_parameter)
-    <3244>   DW_AT_name        : (strp) (offset: 0xf72): self
-    <3248>   DW_AT_decl_file   : (data1) 1
-    <3249>   DW_AT_decl_line   : (data1) 219
-    <324a>   DW_AT_decl_column : (data1) 24
-    <324b>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><324f>: Abbrev Number: 71 (DW_TAG_formal_parameter)
-    <3250>   DW_AT_name        : (strp) (offset: 0x755): defining_class
-    <3254>   DW_AT_decl_file   : (data1) 1
-    <3255>   DW_AT_decl_line   : (data1) 219
-    <3256>   DW_AT_decl_column : (data1) 44
-    <3257>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
- <2><325b>: Abbrev Number: 71 (DW_TAG_formal_parameter)
-    <325c>   DW_AT_name        : (strp) (offset: 0x543): args
-    <3260>   DW_AT_decl_file   : (data1) 1
-    <3261>   DW_AT_decl_line   : (data1) 219
-    <3262>   DW_AT_decl_column : (data1) 77
-    <3263>   DW_AT_type        : (ref4) <0x105c>, PyObject, _object
- <2><3267>: Abbrev Number: 71 (DW_TAG_formal_parameter)
-    <3268>   DW_AT_name        : (strp) (offset: 0x229d): nargs
-    <326c>   DW_AT_decl_file   : (data1) 1
-    <326d>   DW_AT_decl_line   : (data1) 220
-    <326e>   DW_AT_decl_column : (data1) 25
-    <326f>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
- <2><3273>: Abbrev Number: 71 (DW_TAG_formal_parameter)
-    <3274>   DW_AT_name        : (strp) (offset: 0x217b): kwnames
-    <3278>   DW_AT_decl_file   : (data1) 1
-    <3279>   DW_AT_decl_line   : (data1) 220
-    <327a>   DW_AT_decl_column : (data1) 42
-    <327b>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><327f>: Abbrev Number: 72 (DW_TAG_variable)
-    <3280>   DW_AT_name        : (strp) (offset: 0x99d): list
-    <3284>   DW_AT_decl_file   : (data1) 1
-    <3285>   DW_AT_decl_line   : (data1) 231
-    <3286>   DW_AT_decl_column : (data1) 15
-    <3287>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><328b>: Abbrev Number: 72 (DW_TAG_variable)
-    <328c>   DW_AT_name        : (strp) (offset: 0x23a9): next
-    <3290>   DW_AT_decl_file   : (data1) 1
-    <3291>   DW_AT_decl_line   : (data1) 232
-    <3292>   DW_AT_decl_column : (data1) 15
-    <3293>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><3297>: Abbrev Number: 72 (DW_TAG_variable)
-    <3298>   DW_AT_name        : (strp) (offset: 0x652): head
-    <329c>   DW_AT_decl_file   : (data1) 1
-    <329d>   DW_AT_decl_line   : (data1) 232
-    <329e>   DW_AT_decl_column : (data1) 29
-    <329f>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><32a3>: Abbrev Number: 73 (DW_TAG_lexical_block)
- <3><32a4>: Abbrev Number: 74 (DW_TAG_variable)
-    <32a5>   DW_AT_name        : (string) i
-    <32a7>   DW_AT_decl_file   : (data1) 1
-    <32a8>   DW_AT_decl_line   : (data1) 233
-    <32a9>   DW_AT_decl_column : (data1) 21
-    <32aa>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
- <3><32ae>: Abbrev Number: 0
- <2><32af>: Abbrev Number: 0
- <1><32b0>: Abbrev Number: 64 (DW_TAG_subprogram)
-    <32b1>   DW_AT_external    : (flag_present) 1
-    <32b1>   DW_AT_name        : (strp) (offset: 0x1bb3): Cons_from_xs
-    <32b5>   DW_AT_decl_file   : (data1) 1
-    <32b6>   DW_AT_decl_line   : (data1) 186
-    <32b7>   DW_AT_decl_column : (data1) 1
-    <32b8>   DW_AT_prototyped  : (flag_present) 1
-    <32b8>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <32bc>   DW_AT_low_pc      : (addr) 0x2d50
-    <32c4>   DW_AT_high_pc     : (data8) 0x124
-    <32cc>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
-    <32ce>   DW_AT_GNU_all_call_sites: (flag_present) 1
-    <32ce>   DW_AT_sibling     : (ref4) <0x352c>
- <2><32d2>: Abbrev Number: 65 (DW_TAG_formal_parameter)
-    <32d3>   DW_AT_name        : (strp) (offset: 0xf72): self
-    <32d7>   DW_AT_decl_file   : (data1) 1
-    <32d8>   DW_AT_decl_line   : (data1) 186
-    <32d9>   DW_AT_decl_column : (data1) 24
-    <32da>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <32de>   DW_AT_location    : (sec_offset) 0xf99 (location list)
-    <32e2>   DW_AT_GNU_locviews: (sec_offset) 0xf91
- <2><32e6>: Abbrev Number: 65 (DW_TAG_formal_parameter)
-    <32e7>   DW_AT_name        : (strp) (offset: 0x755): defining_class
-    <32eb>   DW_AT_decl_file   : (data1) 1
-    <32ec>   DW_AT_decl_line   : (data1) 186
-    <32ed>   DW_AT_decl_column : (data1) 44
-    <32ee>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
-    <32f2>   DW_AT_location    : (sec_offset) 0x1003 (location list)
-    <32f6>   DW_AT_GNU_locviews: (sec_offset) 0xffb
- <2><32fa>: Abbrev Number: 65 (DW_TAG_formal_parameter)
-    <32fb>   DW_AT_name        : (strp) (offset: 0x543): args
-    <32ff>   DW_AT_decl_file   : (data1) 1
-    <3300>   DW_AT_decl_line   : (data1) 186
-    <3301>   DW_AT_decl_column : (data1) 77
-    <3302>   DW_AT_type        : (ref4) <0x105c>, PyObject, _object
-    <3306>   DW_AT_location    : (sec_offset) 0x1077 (location list)
-    <330a>   DW_AT_GNU_locviews: (sec_offset) 0x1065
- <2><330e>: Abbrev Number: 65 (DW_TAG_formal_parameter)
-    <330f>   DW_AT_name        : (strp) (offset: 0x229d): nargs
-    <3313>   DW_AT_decl_file   : (data1) 1
-    <3314>   DW_AT_decl_line   : (data1) 187
-    <3315>   DW_AT_decl_column : (data1) 25
-    <3316>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
-    <331a>   DW_AT_location    : (sec_offset) 0x1146 (location list)
-    <331e>   DW_AT_GNU_locviews: (sec_offset) 0x113e
- <2><3322>: Abbrev Number: 65 (DW_TAG_formal_parameter)
-    <3323>   DW_AT_name        : (strp) (offset: 0x217b): kwnames
-    <3327>   DW_AT_decl_file   : (data1) 1
-    <3328>   DW_AT_decl_line   : (data1) 187
-    <3329>   DW_AT_decl_column : (data1) 42
-    <332a>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <332e>   DW_AT_location    : (sec_offset) 0x11b0 (location list)
-    <3332>   DW_AT_GNU_locviews: (sec_offset) 0x11a8
- <2><3336>: Abbrev Number: 67 (DW_TAG_variable)
-    <3337>   DW_AT_name        : (strp) (offset: 0x58c): state
-    <333b>   DW_AT_decl_file   : (data1) 1
-    <333c>   DW_AT_decl_line   : (data1) 194
-    <333d>   DW_AT_decl_column : (data1) 23
-    <333e>   DW_AT_type        : (ref4) <0x274d>, consmodule_state
-    <3342>   DW_AT_location    : (sec_offset) 0x121a (location list)
-    <3346>   DW_AT_GNU_locviews: (sec_offset) 0x1212
- <2><334a>: Abbrev Number: 66 (DW_TAG_variable)
-    <334b>   DW_AT_name        : (string) xs
-    <334e>   DW_AT_decl_file   : (data1) 1
-    <334f>   DW_AT_decl_line   : (data1) 198
-    <3350>   DW_AT_decl_column : (data1) 15
-    <3351>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <3355>   DW_AT_location    : (sec_offset) 0x128a (location list)
-    <3359>   DW_AT_GNU_locviews: (sec_offset) 0x1276
- <2><335d>: Abbrev Number: 66 (DW_TAG_variable)
-    <335e>   DW_AT_name        : (string) tp
-    <3361>   DW_AT_decl_file   : (data1) 1
-    <3362>   DW_AT_decl_line   : (data1) 198
-    <3363>   DW_AT_decl_column : (data1) 30
-    <3364>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <3368>   DW_AT_location    : (sec_offset) 0x1362 (location list)
-    <336c>   DW_AT_GNU_locviews: (sec_offset) 0x1358
- <2><3370>: Abbrev Number: 67 (DW_TAG_variable)
-    <3371>   DW_AT_name        : (strp) (offset: 0x4d0): result
-    <3375>   DW_AT_decl_file   : (data1) 1
-    <3376>   DW_AT_decl_line   : (data1) 198
-    <3377>   DW_AT_decl_column : (data1) 42
-    <3378>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <337c>   DW_AT_location    : (sec_offset) 0x13e5 (location list)
-    <3380>   DW_AT_GNU_locviews: (sec_offset) 0x13d3
- <2><3384>: Abbrev Number: 75 (DW_TAG_inlined_subroutine)
-    <3385>   DW_AT_abstract_origin: (ref4) <0x3e7d>
-    <3389>   DW_AT_entry_pc    : (addr) 0x2d7a
-    <3391>   DW_AT_GNU_entry_view: (data1) 1
-    <3392>   DW_AT_ranges      : (sec_offset) 0x630
-    <3396>   DW_AT_call_file   : (data1) 1
-    <3397>   DW_AT_call_line   : (data1) 200
-    <3398>   DW_AT_call_column : (data1) 9
-    <3399>   DW_AT_sibling     : (ref4) <0x33ea>
- <3><339d>: Abbrev Number: 62 (DW_TAG_formal_parameter)
-    <339e>   DW_AT_abstract_origin: (ref4) <0x3e9b>
- <3><33a2>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <33a3>   DW_AT_abstract_origin: (ref4) <0x3e8f>
-    <33a7>   DW_AT_location    : (sec_offset) 0x14a4 (location list)
-    <33ab>   DW_AT_GNU_locviews: (sec_offset) 0x14a2
- <3><33af>: Abbrev Number: 57 (DW_TAG_inlined_subroutine)
-    <33b0>   DW_AT_abstract_origin: (ref4) <0x3ea9>
-    <33b4>   DW_AT_entry_pc    : (addr) 0x2d7a
-    <33bc>   DW_AT_GNU_entry_view: (data1) 3
-    <33bd>   DW_AT_ranges      : (sec_offset) 0x670
-    <33c1>   DW_AT_call_file   : (data1) 2
-    <33c2>   DW_AT_call_line   : (data2) 263
-    <33c4>   DW_AT_call_column : (data1) 12
-    <33c5>   DW_AT_sibling     : (ref4) <0x33dc>
- <4><33c9>: Abbrev Number: 62 (DW_TAG_formal_parameter)
-    <33ca>   DW_AT_abstract_origin: (ref4) <0x3ec5>
- <4><33ce>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <33cf>   DW_AT_abstract_origin: (ref4) <0x3eba>
-    <33d3>   DW_AT_location    : (sec_offset) 0x14c9 (location list)
-    <33d7>   DW_AT_GNU_locviews: (sec_offset) 0x14c7
- <4><33db>: Abbrev Number: 0
- <3><33dc>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
-    <33dd>   DW_AT_low_pc      : (addr) 0x2d8f
-    <33e5>   DW_AT_abstract_origin: (ref4) <0x444b>
- <3><33e9>: Abbrev Number: 0
- <2><33ea>: Abbrev Number: 75 (DW_TAG_inlined_subroutine)
-    <33eb>   DW_AT_abstract_origin: (ref4) <0x3e47>
-    <33ef>   DW_AT_entry_pc    : (addr) 0x2dc8
-    <33f7>   DW_AT_GNU_entry_view: (data1) 2
-    <33f8>   DW_AT_ranges      : (sec_offset) 0x6a0
-    <33fc>   DW_AT_call_file   : (data1) 1
-    <33fd>   DW_AT_call_line   : (data1) 211
-    <33fe>   DW_AT_call_column : (data1) 9
-    <33ff>   DW_AT_sibling     : (ref4) <0x3432>
- <3><3403>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <3404>   DW_AT_abstract_origin: (ref4) <0x3e55>
-    <3408>   DW_AT_location    : (sec_offset) 0x14f6 (location list)
-    <340c>   DW_AT_GNU_locviews: (sec_offset) 0x14ec
- <3><3410>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
-    <3411>   DW_AT_low_pc      : (addr) 0x2e4b
-    <3419>   DW_AT_abstract_origin: (ref4) <0x4338>
- <3><341d>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
-    <341e>   DW_AT_low_pc      : (addr) 0x2e58
-    <3426>   DW_AT_abstract_origin: (ref4) <0x4338>
- <4><342a>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <342b>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <342d>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
- <4><3430>: Abbrev Number: 0
- <3><3431>: Abbrev Number: 0
- <2><3432>: Abbrev Number: 75 (DW_TAG_inlined_subroutine)
-    <3433>   DW_AT_abstract_origin: (ref4) <0x3e2c>
-    <3437>   DW_AT_entry_pc    : (addr) 0x2dcd
-    <343f>   DW_AT_GNU_entry_view: (data1) 3
-    <3440>   DW_AT_ranges      : (sec_offset) 0x700
-    <3444>   DW_AT_call_file   : (data1) 1
-    <3445>   DW_AT_call_line   : (data1) 214
-    <3446>   DW_AT_call_column : (data1) 5
-    <3447>   DW_AT_sibling     : (ref4) <0x3459>
- <3><344b>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <344c>   DW_AT_abstract_origin: (ref4) <0x3e3a>
-    <3450>   DW_AT_location    : (sec_offset) 0x1569 (location list)
-    <3454>   DW_AT_GNU_locviews: (sec_offset) 0x1565
- <3><3458>: Abbrev Number: 0
- <2><3459>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <345a>   DW_AT_low_pc      : (addr) 0x2d6a
-    <3462>   DW_AT_abstract_origin: (ref4) <0x439a>
-    <3466>   DW_AT_sibling     : (ref4) <0x3472>
- <3><346a>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <346b>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <346d>   DW_AT_GNU_call_site_value: (exprloc) 3 byte block: f3 1 54 	(DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)))
- <3><3471>: Abbrev Number: 0
- <2><3472>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <3473>   DW_AT_low_pc      : (addr) 0x2d9b
-    <347b>   DW_AT_abstract_origin: (ref4) <0x4458>
-    <347f>   DW_AT_sibling     : (ref4) <0x348a>
- <3><3483>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3484>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <3486>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
- <3><3489>: Abbrev Number: 0
- <2><348a>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <348b>   DW_AT_low_pc      : (addr) 0x2dad
-    <3493>   DW_AT_abstract_origin: (ref4) <0x4465>
-    <3497>   DW_AT_sibling     : (ref4) <0x34af>
- <3><349b>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <349c>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <349e>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+    <31ee>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <31f0>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 77 0 	(DW_OP_breg7 (rsp): 0)
+ <3><31f3>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <31f4>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <31f6>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 8 29 	(DW_OP_const1u: 41)
+ <3><31f9>: Abbrev Number: 0
+ <2><31fa>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <31fb>   DW_AT_low_pc      : (addr) 0x2902
+    <3203>   DW_AT_abstract_origin: (ref4) <0x44eb>
+    <3207>   DW_AT_sibling     : (ref4) <0x3212>
+ <3><320b>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <320c>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <320e>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7e 0 	(DW_OP_breg14 (r14): 0)
+ <3><3211>: Abbrev Number: 0
+ <2><3212>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <3213>   DW_AT_low_pc      : (addr) 0x290a
+    <321b>   DW_AT_abstract_origin: (ref4) <0x4512>
+    <321f>   DW_AT_sibling     : (ref4) <0x322a>
+ <3><3223>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3224>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3226>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 77 0 	(DW_OP_breg7 (rsp): 0)
+ <3><3229>: Abbrev Number: 0
+ <2><322a>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
+    <322b>   DW_AT_low_pc      : (addr) 0x2914
+    <3233>   DW_AT_abstract_origin: (ref4) <0x451f>
+ <2><3237>: Abbrev Number: 0
+ <1><3238>: Abbrev Number: 68 (DW_TAG_subprogram)
+    <3239>   DW_AT_external    : (flag_present) 1
+    <3239>   DW_AT_name        : (strp) (offset: 0x995): Cons_to_list
+    <323d>   DW_AT_decl_file   : (data1) 1
+    <323e>   DW_AT_decl_line   : (data1) 232
+    <323f>   DW_AT_decl_column : (data1) 1
+    <3240>   DW_AT_prototyped  : (flag_present) 1
+    <3240>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <3244>   DW_AT_inline      : (data1) 1	(inlined)
+    <3245>   DW_AT_sibling     : (ref4) <0x32b6>
+ <2><3249>: Abbrev Number: 69 (DW_TAG_formal_parameter)
+    <324a>   DW_AT_name        : (strp) (offset: 0xf72): self
+    <324e>   DW_AT_decl_file   : (data1) 1
+    <324f>   DW_AT_decl_line   : (data1) 232
+    <3250>   DW_AT_decl_column : (data1) 24
+    <3251>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3255>: Abbrev Number: 69 (DW_TAG_formal_parameter)
+    <3256>   DW_AT_name        : (strp) (offset: 0x755): defining_class
+    <325a>   DW_AT_decl_file   : (data1) 1
+    <325b>   DW_AT_decl_line   : (data1) 232
+    <325c>   DW_AT_decl_column : (data1) 44
+    <325d>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
+ <2><3261>: Abbrev Number: 69 (DW_TAG_formal_parameter)
+    <3262>   DW_AT_name        : (strp) (offset: 0x543): args
+    <3266>   DW_AT_decl_file   : (data1) 1
+    <3267>   DW_AT_decl_line   : (data1) 232
+    <3268>   DW_AT_decl_column : (data1) 77
+    <3269>   DW_AT_type        : (ref4) <0x105c>, PyObject, _object
+ <2><326d>: Abbrev Number: 69 (DW_TAG_formal_parameter)
+    <326e>   DW_AT_name        : (strp) (offset: 0x229d): nargs
+    <3272>   DW_AT_decl_file   : (data1) 1
+    <3273>   DW_AT_decl_line   : (data1) 233
+    <3274>   DW_AT_decl_column : (data1) 25
+    <3275>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
+ <2><3279>: Abbrev Number: 69 (DW_TAG_formal_parameter)
+    <327a>   DW_AT_name        : (strp) (offset: 0x217b): kwnames
+    <327e>   DW_AT_decl_file   : (data1) 1
+    <327f>   DW_AT_decl_line   : (data1) 233
+    <3280>   DW_AT_decl_column : (data1) 42
+    <3281>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3285>: Abbrev Number: 70 (DW_TAG_variable)
+    <3286>   DW_AT_name        : (strp) (offset: 0x99d): list
+    <328a>   DW_AT_decl_file   : (data1) 1
+    <328b>   DW_AT_decl_line   : (data1) 244
+    <328c>   DW_AT_decl_column : (data1) 15
+    <328d>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3291>: Abbrev Number: 70 (DW_TAG_variable)
+    <3292>   DW_AT_name        : (strp) (offset: 0x23a9): next
+    <3296>   DW_AT_decl_file   : (data1) 1
+    <3297>   DW_AT_decl_line   : (data1) 245
+    <3298>   DW_AT_decl_column : (data1) 15
+    <3299>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><329d>: Abbrev Number: 70 (DW_TAG_variable)
+    <329e>   DW_AT_name        : (strp) (offset: 0x652): head
+    <32a2>   DW_AT_decl_file   : (data1) 1
+    <32a3>   DW_AT_decl_line   : (data1) 245
+    <32a4>   DW_AT_decl_column : (data1) 29
+    <32a5>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><32a9>: Abbrev Number: 71 (DW_TAG_lexical_block)
+ <3><32aa>: Abbrev Number: 72 (DW_TAG_variable)
+    <32ab>   DW_AT_name        : (string) i
+    <32ad>   DW_AT_decl_file   : (data1) 1
+    <32ae>   DW_AT_decl_line   : (data1) 246
+    <32af>   DW_AT_decl_column : (data1) 21
+    <32b0>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
+ <3><32b4>: Abbrev Number: 0
+ <2><32b5>: Abbrev Number: 0
+ <1><32b6>: Abbrev Number: 64 (DW_TAG_subprogram)
+    <32b7>   DW_AT_external    : (flag_present) 1
+    <32b7>   DW_AT_name        : (strp) (offset: 0x1bb3): Cons_from_xs
+    <32bb>   DW_AT_decl_file   : (data1) 1
+    <32bc>   DW_AT_decl_line   : (data1) 199
+    <32bd>   DW_AT_decl_column : (data1) 1
+    <32be>   DW_AT_prototyped  : (flag_present) 1
+    <32be>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <32c2>   DW_AT_low_pc      : (addr) 0x2d60
+    <32ca>   DW_AT_high_pc     : (data8) 0x124
+    <32d2>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
+    <32d4>   DW_AT_GNU_all_call_sites: (flag_present) 1
+    <32d4>   DW_AT_sibling     : (ref4) <0x3532>
+ <2><32d8>: Abbrev Number: 65 (DW_TAG_formal_parameter)
+    <32d9>   DW_AT_name        : (strp) (offset: 0xf72): self
+    <32dd>   DW_AT_decl_file   : (data1) 1
+    <32de>   DW_AT_decl_line   : (data1) 199
+    <32df>   DW_AT_decl_column : (data1) 24
+    <32e0>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <32e4>   DW_AT_location    : (sec_offset) 0xf99 (location list)
+    <32e8>   DW_AT_GNU_locviews: (sec_offset) 0xf91
+ <2><32ec>: Abbrev Number: 65 (DW_TAG_formal_parameter)
+    <32ed>   DW_AT_name        : (strp) (offset: 0x755): defining_class
+    <32f1>   DW_AT_decl_file   : (data1) 1
+    <32f2>   DW_AT_decl_line   : (data1) 199
+    <32f3>   DW_AT_decl_column : (data1) 44
+    <32f4>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
+    <32f8>   DW_AT_location    : (sec_offset) 0x1003 (location list)
+    <32fc>   DW_AT_GNU_locviews: (sec_offset) 0xffb
+ <2><3300>: Abbrev Number: 65 (DW_TAG_formal_parameter)
+    <3301>   DW_AT_name        : (strp) (offset: 0x543): args
+    <3305>   DW_AT_decl_file   : (data1) 1
+    <3306>   DW_AT_decl_line   : (data1) 199
+    <3307>   DW_AT_decl_column : (data1) 77
+    <3308>   DW_AT_type        : (ref4) <0x105c>, PyObject, _object
+    <330c>   DW_AT_location    : (sec_offset) 0x1077 (location list)
+    <3310>   DW_AT_GNU_locviews: (sec_offset) 0x1065
+ <2><3314>: Abbrev Number: 65 (DW_TAG_formal_parameter)
+    <3315>   DW_AT_name        : (strp) (offset: 0x229d): nargs
+    <3319>   DW_AT_decl_file   : (data1) 1
+    <331a>   DW_AT_decl_line   : (data1) 200
+    <331b>   DW_AT_decl_column : (data1) 25
+    <331c>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
+    <3320>   DW_AT_location    : (sec_offset) 0x1146 (location list)
+    <3324>   DW_AT_GNU_locviews: (sec_offset) 0x113e
+ <2><3328>: Abbrev Number: 65 (DW_TAG_formal_parameter)
+    <3329>   DW_AT_name        : (strp) (offset: 0x217b): kwnames
+    <332d>   DW_AT_decl_file   : (data1) 1
+    <332e>   DW_AT_decl_line   : (data1) 200
+    <332f>   DW_AT_decl_column : (data1) 42
+    <3330>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <3334>   DW_AT_location    : (sec_offset) 0x11b0 (location list)
+    <3338>   DW_AT_GNU_locviews: (sec_offset) 0x11a8
+ <2><333c>: Abbrev Number: 73 (DW_TAG_variable)
+    <333d>   DW_AT_name        : (strp) (offset: 0x58c): state
+    <3341>   DW_AT_decl_file   : (data1) 1
+    <3342>   DW_AT_decl_line   : (data1) 207
+    <3343>   DW_AT_decl_column : (data1) 23
+    <3344>   DW_AT_type        : (ref4) <0x274d>, consmodule_state
+    <3348>   DW_AT_location    : (sec_offset) 0x121a (location list)
+    <334c>   DW_AT_GNU_locviews: (sec_offset) 0x1212
+ <2><3350>: Abbrev Number: 74 (DW_TAG_variable)
+    <3351>   DW_AT_name        : (string) xs
+    <3354>   DW_AT_decl_file   : (data1) 1
+    <3355>   DW_AT_decl_line   : (data1) 211
+    <3356>   DW_AT_decl_column : (data1) 15
+    <3357>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <335b>   DW_AT_location    : (sec_offset) 0x128a (location list)
+    <335f>   DW_AT_GNU_locviews: (sec_offset) 0x1276
+ <2><3363>: Abbrev Number: 74 (DW_TAG_variable)
+    <3364>   DW_AT_name        : (string) tp
+    <3367>   DW_AT_decl_file   : (data1) 1
+    <3368>   DW_AT_decl_line   : (data1) 211
+    <3369>   DW_AT_decl_column : (data1) 30
+    <336a>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <336e>   DW_AT_location    : (sec_offset) 0x1362 (location list)
+    <3372>   DW_AT_GNU_locviews: (sec_offset) 0x1358
+ <2><3376>: Abbrev Number: 73 (DW_TAG_variable)
+    <3377>   DW_AT_name        : (strp) (offset: 0x4d0): result
+    <337b>   DW_AT_decl_file   : (data1) 1
+    <337c>   DW_AT_decl_line   : (data1) 211
+    <337d>   DW_AT_decl_column : (data1) 42
+    <337e>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <3382>   DW_AT_location    : (sec_offset) 0x13e5 (location list)
+    <3386>   DW_AT_GNU_locviews: (sec_offset) 0x13d3
+ <2><338a>: Abbrev Number: 75 (DW_TAG_inlined_subroutine)
+    <338b>   DW_AT_abstract_origin: (ref4) <0x3f5a>
+    <338f>   DW_AT_entry_pc    : (addr) 0x2d8a
+    <3397>   DW_AT_GNU_entry_view: (data1) 1
+    <3398>   DW_AT_ranges      : (sec_offset) 0x6a0
+    <339c>   DW_AT_call_file   : (data1) 1
+    <339d>   DW_AT_call_line   : (data1) 213
+    <339e>   DW_AT_call_column : (data1) 9
+    <339f>   DW_AT_sibling     : (ref4) <0x33f0>
+ <3><33a3>: Abbrev Number: 62 (DW_TAG_formal_parameter)
+    <33a4>   DW_AT_abstract_origin: (ref4) <0x3f78>
+ <3><33a8>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <33a9>   DW_AT_abstract_origin: (ref4) <0x3f6c>
+    <33ad>   DW_AT_location    : (sec_offset) 0x14a4 (location list)
+    <33b1>   DW_AT_GNU_locviews: (sec_offset) 0x14a2
+ <3><33b5>: Abbrev Number: 57 (DW_TAG_inlined_subroutine)
+    <33b6>   DW_AT_abstract_origin: (ref4) <0x3f86>
+    <33ba>   DW_AT_entry_pc    : (addr) 0x2d8a
+    <33c2>   DW_AT_GNU_entry_view: (data1) 3
+    <33c3>   DW_AT_ranges      : (sec_offset) 0x6e0
+    <33c7>   DW_AT_call_file   : (data1) 2
+    <33c8>   DW_AT_call_line   : (data2) 263
+    <33ca>   DW_AT_call_column : (data1) 12
+    <33cb>   DW_AT_sibling     : (ref4) <0x33e2>
+ <4><33cf>: Abbrev Number: 62 (DW_TAG_formal_parameter)
+    <33d0>   DW_AT_abstract_origin: (ref4) <0x3fa2>
+ <4><33d4>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <33d5>   DW_AT_abstract_origin: (ref4) <0x3f97>
+    <33d9>   DW_AT_location    : (sec_offset) 0x14c9 (location list)
+    <33dd>   DW_AT_GNU_locviews: (sec_offset) 0x14c7
+ <4><33e1>: Abbrev Number: 0
+ <3><33e2>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
+    <33e3>   DW_AT_low_pc      : (addr) 0x2d9f
+    <33eb>   DW_AT_abstract_origin: (ref4) <0x4528>
+ <3><33ef>: Abbrev Number: 0
+ <2><33f0>: Abbrev Number: 75 (DW_TAG_inlined_subroutine)
+    <33f1>   DW_AT_abstract_origin: (ref4) <0x3f24>
+    <33f5>   DW_AT_entry_pc    : (addr) 0x2dd8
+    <33fd>   DW_AT_GNU_entry_view: (data1) 2
+    <33fe>   DW_AT_ranges      : (sec_offset) 0x710
+    <3402>   DW_AT_call_file   : (data1) 1
+    <3403>   DW_AT_call_line   : (data1) 224
+    <3404>   DW_AT_call_column : (data1) 9
+    <3405>   DW_AT_sibling     : (ref4) <0x3438>
+ <3><3409>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <340a>   DW_AT_abstract_origin: (ref4) <0x3f32>
+    <340e>   DW_AT_location    : (sec_offset) 0x14f6 (location list)
+    <3412>   DW_AT_GNU_locviews: (sec_offset) 0x14ec
+ <3><3416>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
+    <3417>   DW_AT_low_pc      : (addr) 0x2e5b
+    <341f>   DW_AT_abstract_origin: (ref4) <0x4415>
+ <3><3423>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
+    <3424>   DW_AT_low_pc      : (addr) 0x2e68
+    <342c>   DW_AT_abstract_origin: (ref4) <0x4415>
+ <4><3430>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3431>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3433>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <4><3436>: Abbrev Number: 0
+ <3><3437>: Abbrev Number: 0
+ <2><3438>: Abbrev Number: 75 (DW_TAG_inlined_subroutine)
+    <3439>   DW_AT_abstract_origin: (ref4) <0x3f09>
+    <343d>   DW_AT_entry_pc    : (addr) 0x2ddd
+    <3445>   DW_AT_GNU_entry_view: (data1) 3
+    <3446>   DW_AT_ranges      : (sec_offset) 0x770
+    <344a>   DW_AT_call_file   : (data1) 1
+    <344b>   DW_AT_call_line   : (data1) 227
+    <344c>   DW_AT_call_column : (data1) 5
+    <344d>   DW_AT_sibling     : (ref4) <0x345f>
+ <3><3451>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <3452>   DW_AT_abstract_origin: (ref4) <0x3f17>
+    <3456>   DW_AT_location    : (sec_offset) 0x1569 (location list)
+    <345a>   DW_AT_GNU_locviews: (sec_offset) 0x1565
+ <3><345e>: Abbrev Number: 0
+ <2><345f>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <3460>   DW_AT_low_pc      : (addr) 0x2d7a
+    <3468>   DW_AT_abstract_origin: (ref4) <0x4477>
+    <346c>   DW_AT_sibling     : (ref4) <0x3478>
+ <3><3470>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3471>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3473>   DW_AT_GNU_call_site_value: (exprloc) 3 byte block: f3 1 54 	(DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)))
+ <3><3477>: Abbrev Number: 0
+ <2><3478>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <3479>   DW_AT_low_pc      : (addr) 0x2dab
+    <3481>   DW_AT_abstract_origin: (ref4) <0x4535>
+    <3485>   DW_AT_sibling     : (ref4) <0x3490>
+ <3><3489>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <348a>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <348c>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <3><348f>: Abbrev Number: 0
+ <2><3490>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <3491>   DW_AT_low_pc      : (addr) 0x2dbd
+    <3499>   DW_AT_abstract_origin: (ref4) <0x4542>
+    <349d>   DW_AT_sibling     : (ref4) <0x34b5>
  <3><34a1>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <34a2>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <34a4>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 f8 30 0 0 0 0 0 0 	(DW_OP_addr: 30f8)
- <3><34ae>: Abbrev Number: 0
- <2><34af>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <34b0>   DW_AT_low_pc      : (addr) 0x2dc0
-    <34b8>   DW_AT_abstract_origin: (ref4) <0x352c>
-    <34bc>   DW_AT_sibling     : (ref4) <0x34cd>
- <3><34c0>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <34c1>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <34c3>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7c 0 	(DW_OP_breg12 (r12): 0)
+    <34a2>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <34a4>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <3><34a7>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <34a8>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <34aa>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 f8 30 0 0 0 0 0 0 	(DW_OP_addr: 30f8)
+ <3><34b4>: Abbrev Number: 0
+ <2><34b5>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <34b6>   DW_AT_low_pc      : (addr) 0x2dd0
+    <34be>   DW_AT_abstract_origin: (ref4) <0x3532>
+    <34c2>   DW_AT_sibling     : (ref4) <0x34d3>
  <3><34c6>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <34c7>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <34c9>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7d 0 	(DW_OP_breg13 (r13): 0)
- <3><34cc>: Abbrev Number: 0
- <2><34cd>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <34ce>   DW_AT_low_pc      : (addr) 0x2e01
-    <34d6>   DW_AT_abstract_origin: (ref4) <0x4472>
-    <34da>   DW_AT_sibling     : (ref4) <0x34ec>
- <3><34de>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <34df>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <34e1>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 d0 30 0 0 0 0 0 0 	(DW_OP_addr: 30d0)
- <3><34eb>: Abbrev Number: 0
- <2><34ec>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <34ed>   DW_AT_low_pc      : (addr) 0x2e1f
-    <34f5>   DW_AT_abstract_origin: (ref4) <0x4465>
-    <34f9>   DW_AT_sibling     : (ref4) <0x3511>
- <3><34fd>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <34fe>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <3500>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+    <34c7>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <34c9>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7c 0 	(DW_OP_breg12 (r12): 0)
+ <3><34cc>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <34cd>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <34cf>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7d 0 	(DW_OP_breg13 (r13): 0)
+ <3><34d2>: Abbrev Number: 0
+ <2><34d3>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <34d4>   DW_AT_low_pc      : (addr) 0x2e11
+    <34dc>   DW_AT_abstract_origin: (ref4) <0x454f>
+    <34e0>   DW_AT_sibling     : (ref4) <0x34f2>
+ <3><34e4>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <34e5>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <34e7>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 d0 30 0 0 0 0 0 0 	(DW_OP_addr: 30d0)
+ <3><34f1>: Abbrev Number: 0
+ <2><34f2>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <34f3>   DW_AT_low_pc      : (addr) 0x2e2f
+    <34fb>   DW_AT_abstract_origin: (ref4) <0x4542>
+    <34ff>   DW_AT_sibling     : (ref4) <0x3517>
  <3><3503>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3504>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <3506>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 f8 30 0 0 0 0 0 0 	(DW_OP_addr: 30f8)
- <3><3510>: Abbrev Number: 0
- <2><3511>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
-    <3512>   DW_AT_low_pc      : (addr) 0x2e32
-    <351a>   DW_AT_abstract_origin: (ref4) <0x352c>
- <3><351e>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <351f>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <3521>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+    <3504>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3506>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <3><3509>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <350a>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <350c>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 f8 30 0 0 0 0 0 0 	(DW_OP_addr: 30f8)
+ <3><3516>: Abbrev Number: 0
+ <2><3517>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
+    <3518>   DW_AT_low_pc      : (addr) 0x2e42
+    <3520>   DW_AT_abstract_origin: (ref4) <0x3532>
  <3><3524>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3525>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <3527>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7d 0 	(DW_OP_breg13 (r13): 0)
- <3><352a>: Abbrev Number: 0
- <2><352b>: Abbrev Number: 0
- <1><352c>: Abbrev Number: 64 (DW_TAG_subprogram)
-    <352d>   DW_AT_external    : (flag_present) 1
-    <352d>   DW_AT_name        : (strp) (offset: 0x1395): Cons_from_fast
-    <3531>   DW_AT_decl_file   : (data1) 1
-    <3532>   DW_AT_decl_line   : (data1) 166
-    <3533>   DW_AT_decl_column : (data1) 1
-    <3534>   DW_AT_prototyped  : (flag_present) 1
-    <3534>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <3538>   DW_AT_low_pc      : (addr) 0x2ca0
-    <3540>   DW_AT_high_pc     : (data8) 0xa1
-    <3548>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
-    <354a>   DW_AT_GNU_all_call_sites: (flag_present) 1
-    <354a>   DW_AT_sibling     : (ref4) <0x36d2>
- <2><354e>: Abbrev Number: 76 (DW_TAG_formal_parameter)
-    <354f>   DW_AT_name        : (string) xs
-    <3552>   DW_AT_decl_file   : (data1) 1
-    <3553>   DW_AT_decl_line   : (data1) 166
-    <3554>   DW_AT_decl_column : (data1) 26
-    <3555>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <3559>   DW_AT_location    : (sec_offset) 0x15a6 (location list)
-    <355d>   DW_AT_GNU_locviews: (sec_offset) 0x15a0
- <2><3561>: Abbrev Number: 65 (DW_TAG_formal_parameter)
-    <3562>   DW_AT_name        : (strp) (offset: 0x58c): state
-    <3566>   DW_AT_decl_file   : (data1) 1
-    <3567>   DW_AT_decl_line   : (data1) 166
-    <3568>   DW_AT_decl_column : (data1) 48
-    <3569>   DW_AT_type        : (ref4) <0x274d>, consmodule_state
-    <356d>   DW_AT_location    : (sec_offset) 0x15f6 (location list)
-    <3571>   DW_AT_GNU_locviews: (sec_offset) 0x15f2
- <2><3575>: Abbrev Number: 66 (DW_TAG_variable)
-    <3576>   DW_AT_name        : (string) nil
-    <357a>   DW_AT_decl_file   : (data1) 1
-    <357b>   DW_AT_decl_line   : (data1) 168
-    <357c>   DW_AT_decl_column : (data1) 15
-    <357d>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <3581>   DW_AT_location    : (sec_offset) 0x1631 (location list)
-    <3585>   DW_AT_GNU_locviews: (sec_offset) 0x162f
- <2><3589>: Abbrev Number: 67 (DW_TAG_variable)
-    <358a>   DW_AT_name        : (strp) (offset: 0x2327): cons
-    <358e>   DW_AT_decl_file   : (data1) 1
-    <358f>   DW_AT_decl_line   : (data1) 169
-    <3590>   DW_AT_decl_column : (data1) 15
-    <3591>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <3595>   DW_AT_location    : (sec_offset) 0x1656 (location list)
-    <3599>   DW_AT_GNU_locviews: (sec_offset) 0x1654
- <2><359d>: Abbrev Number: 66 (DW_TAG_variable)
-    <359e>   DW_AT_name        : (string) len
-    <35a2>   DW_AT_decl_file   : (data1) 1
-    <35a3>   DW_AT_decl_line   : (data1) 171
-    <35a4>   DW_AT_decl_column : (data1) 16
-    <35a5>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
-    <35a9>   DW_AT_location    : (sec_offset) 0x167b (location list)
-    <35ad>   DW_AT_GNU_locviews: (sec_offset) 0x1679
- <2><35b1>: Abbrev Number: 67 (DW_TAG_variable)
-    <35b2>   DW_AT_name        : (strp) (offset: 0x4d0): result
-    <35b6>   DW_AT_decl_file   : (data1) 1
-    <35b7>   DW_AT_decl_line   : (data1) 172
-    <35b8>   DW_AT_decl_column : (data1) 15
-    <35b9>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <35bd>   DW_AT_location    : (sec_offset) 0x16ab (location list)
-    <35c1>   DW_AT_GNU_locviews: (sec_offset) 0x169f
- <2><35c5>: Abbrev Number: 67 (DW_TAG_variable)
-    <35c6>   DW_AT_name        : (strp) (offset: 0x1c68): item
-    <35ca>   DW_AT_decl_file   : (data1) 1
-    <35cb>   DW_AT_decl_line   : (data1) 172
-    <35cc>   DW_AT_decl_column : (data1) 30
-    <35cd>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <35d1>   DW_AT_location    : (sec_offset) 0x1735 (location list)
-    <35d5>   DW_AT_GNU_locviews: (sec_offset) 0x172d
- <2><35d9>: Abbrev Number: 58 (DW_TAG_lexical_block)
-    <35da>   DW_AT_ranges      : (sec_offset) 0x5b0
- <3><35de>: Abbrev Number: 66 (DW_TAG_variable)
-    <35df>   DW_AT_name        : (string) i
-    <35e1>   DW_AT_decl_file   : (data1) 1
-    <35e2>   DW_AT_decl_line   : (data1) 173
-    <35e3>   DW_AT_decl_column : (data1) 21
-    <35e4>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
-    <35e8>   DW_AT_location    : (sec_offset) 0x1797 (location list)
-    <35ec>   DW_AT_GNU_locviews: (sec_offset) 0x1793
- <3><35f0>: Abbrev Number: 77 (DW_TAG_inlined_subroutine)
-    <35f1>   DW_AT_abstract_origin: (ref4) <0x3e62>
-    <35f5>   DW_AT_entry_pc    : (addr) 0x2cd8
-    <35fd>   DW_AT_GNU_entry_view: (data1) 1
-    <35fe>   DW_AT_low_pc      : (addr) 0x2cd8
-    <3606>   DW_AT_high_pc     : (data8) 0x5
-    <360e>   DW_AT_call_file   : (data1) 1
-    <360f>   DW_AT_call_line   : (data1) 175
-    <3610>   DW_AT_call_column : (data1) 9
-    <3611>   DW_AT_sibling     : (ref4) <0x3623>
- <4><3615>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <3616>   DW_AT_abstract_origin: (ref4) <0x3e70>
-    <361a>   DW_AT_location    : (sec_offset) 0x17d6 (location list)
-    <361e>   DW_AT_GNU_locviews: (sec_offset) 0x17d2
- <4><3622>: Abbrev Number: 0
- <3><3623>: Abbrev Number: 75 (DW_TAG_inlined_subroutine)
-    <3624>   DW_AT_abstract_origin: (ref4) <0x3e47>
-    <3628>   DW_AT_entry_pc    : (addr) 0x2cf7
-    <3630>   DW_AT_GNU_entry_view: (data1) 2
-    <3631>   DW_AT_ranges      : (sec_offset) 0x5f0
-    <3635>   DW_AT_call_file   : (data1) 1
-    <3636>   DW_AT_call_line   : (data1) 177
-    <3637>   DW_AT_call_column : (data1) 9
-    <3638>   DW_AT_sibling     : (ref4) <0x365e>
- <4><363c>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <363d>   DW_AT_abstract_origin: (ref4) <0x3e55>
-    <3641>   DW_AT_location    : (sec_offset) 0x1810 (location list)
-    <3645>   DW_AT_GNU_locviews: (sec_offset) 0x180c
- <4><3649>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
-    <364a>   DW_AT_low_pc      : (addr) 0x2d30
-    <3652>   DW_AT_abstract_origin: (ref4) <0x4338>
- <5><3656>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3657>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <3659>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
- <5><365c>: Abbrev Number: 0
- <4><365d>: Abbrev Number: 0
- <3><365e>: Abbrev Number: 77 (DW_TAG_inlined_subroutine)
-    <365f>   DW_AT_abstract_origin: (ref4) <0x3dd2>
-    <3663>   DW_AT_entry_pc    : (addr) 0x2d13
-    <366b>   DW_AT_GNU_entry_view: (data1) 3
-    <366c>   DW_AT_low_pc      : (addr) 0x2d13
-    <3674>   DW_AT_high_pc     : (data8) 0
-    <367c>   DW_AT_call_file   : (data1) 1
-    <367d>   DW_AT_call_line   : (data1) 174
-    <367e>   DW_AT_call_column : (data1) 16
-    <367f>   DW_AT_sibling     : (ref4) <0x36ab>
- <4><3683>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <3684>   DW_AT_abstract_origin: (ref4) <0x3de4>
-    <3688>   DW_AT_location    : (sec_offset) 0x184a (location list)
-    <368c>   DW_AT_GNU_locviews: (sec_offset) 0x1846
- <4><3690>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <3691>   DW_AT_abstract_origin: (ref4) <0x3df1>
-    <3695>   DW_AT_location    : (sec_offset) 0x1884 (location list)
-    <3699>   DW_AT_GNU_locviews: (sec_offset) 0x1882
- <4><369d>: Abbrev Number: 59 (DW_TAG_variable)
-    <369e>   DW_AT_abstract_origin: (ref4) <0x3dfe>
-    <36a2>   DW_AT_location    : (sec_offset) 0x18ac (location list)
-    <36a6>   DW_AT_GNU_locviews: (sec_offset) 0x18aa
- <4><36aa>: Abbrev Number: 0
- <3><36ab>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
-    <36ac>   DW_AT_low_pc      : (addr) 0x2cef
-    <36b4>   DW_AT_abstract_origin: (ref4) <0x447e>
- <4><36b8>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <36b9>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <36bb>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7d 0 	(DW_OP_breg13 (r13): 0)
- <4><36be>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <36bf>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <36c1>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
- <4><36c4>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <36c5>   DW_AT_location    : (exprloc) 1 byte block: 51 	(DW_OP_reg1 (rdx))
-    <36c7>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7c 0 	(DW_OP_breg12 (r12): 0)
- <4><36ca>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <36cb>   DW_AT_location    : (exprloc) 1 byte block: 52 	(DW_OP_reg2 (rcx))
-    <36cd>   DW_AT_GNU_call_site_value: (exprloc) 1 byte block: 30 	(DW_OP_lit0)
- <4><36cf>: Abbrev Number: 0
- <3><36d0>: Abbrev Number: 0
- <2><36d1>: Abbrev Number: 0
- <1><36d2>: Abbrev Number: 78 (DW_TAG_subprogram)
-    <36d3>   DW_AT_external    : (flag_present) 1
-    <36d3>   DW_AT_name        : (strp) (offset: 0x2ed): Cons_dealloc
-    <36d7>   DW_AT_decl_file   : (data1) 1
-    <36d8>   DW_AT_decl_line   : (data1) 156
-    <36d9>   DW_AT_decl_column : (data1) 1
-    <36da>   DW_AT_prototyped  : (flag_present) 1
-    <36da>   DW_AT_low_pc      : (addr) 0x2590
-    <36e2>   DW_AT_high_pc     : (data8) 0x98
-    <36ea>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
-    <36ec>   DW_AT_GNU_all_call_sites: (flag_present) 1
-    <36ec>   DW_AT_sibling     : (ref4) <0x37ed>
- <2><36f0>: Abbrev Number: 65 (DW_TAG_formal_parameter)
-    <36f1>   DW_AT_name        : (strp) (offset: 0xf72): self
-    <36f5>   DW_AT_decl_file   : (data1) 1
-    <36f6>   DW_AT_decl_line   : (data1) 156
-    <36f7>   DW_AT_decl_column : (data1) 26
-    <36f8>   DW_AT_type        : (ref4) <0x37ed>, ConsObject
-    <36fc>   DW_AT_location    : (sec_offset) 0x18e4 (location list)
-    <3700>   DW_AT_GNU_locviews: (sec_offset) 0x18d4
- <2><3704>: Abbrev Number: 46 (DW_TAG_lexical_block)
-    <3705>   DW_AT_ranges      : (sec_offset) 0x140
-    <3709>   DW_AT_sibling     : (ref4) <0x37d8>
- <3><370d>: Abbrev Number: 67 (DW_TAG_variable)
-    <370e>   DW_AT_name        : (strp) (offset: 0x416): _tstate
-    <3712>   DW_AT_decl_file   : (data1) 1
-    <3713>   DW_AT_decl_line   : (data1) 159
-    <3714>   DW_AT_decl_column : (data1) 5
-    <3715>   DW_AT_type        : (ref4) <0x1d29>, PyThreadState, _ts
-    <3719>   DW_AT_location    : (sec_offset) 0x199f (location list)
-    <371d>   DW_AT_GNU_locviews: (sec_offset) 0x1995
- <3><3721>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <3722>   DW_AT_low_pc      : (addr) 0x25ae
-    <372a>   DW_AT_abstract_origin: (ref4) <0x448a>
-    <372e>   DW_AT_sibling     : (ref4) <0x3746>
- <4><3732>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3733>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <3735>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
- <4><3738>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3739>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <373b>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 90 25 0 0 0 0 0 0 	(DW_OP_addr: 2590)
- <4><3745>: Abbrev Number: 0
- <3><3746>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <3747>   DW_AT_low_pc      : (addr) 0x25ba
-    <374f>   DW_AT_abstract_origin: (ref4) <0x37f3>
-    <3753>   DW_AT_sibling     : (ref4) <0x375e>
- <4><3757>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3758>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <375a>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
- <4><375d>: Abbrev Number: 0
- <3><375e>: Abbrev Number: 79 (DW_TAG_GNU_call_site)
-    <375f>   DW_AT_low_pc      : (addr) 0x25d1
-    <3767>   DW_AT_GNU_tail_call: (flag_present) 1
-    <3767>   DW_AT_sibling     : (ref4) <0x3773>
- <4><376b>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <376c>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <376e>   DW_AT_GNU_call_site_value: (exprloc) 3 byte block: f3 1 55 	(DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)))
- <4><3772>: Abbrev Number: 0
- <3><3773>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
-    <3774>   DW_AT_low_pc      : (addr) 0x25dd
-    <377c>   DW_AT_abstract_origin: (ref4) <0x4497>
- <3><3780>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <3781>   DW_AT_low_pc      : (addr) 0x25eb
-    <3789>   DW_AT_abstract_origin: (ref4) <0x44a3>
-    <378d>   DW_AT_sibling     : (ref4) <0x379e>
- <4><3791>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3792>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <3794>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7c 0 	(DW_OP_breg12 (r12): 0)
- <4><3797>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3798>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <379a>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
- <4><379d>: Abbrev Number: 0
- <3><379e>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <379f>   DW_AT_low_pc      : (addr) 0x25f7
-    <37a7>   DW_AT_abstract_origin: (ref4) <0x37f3>
-    <37ab>   DW_AT_sibling     : (ref4) <0x37b6>
- <4><37af>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <37b0>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <37b2>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
- <4><37b5>: Abbrev Number: 0
- <3><37b6>: Abbrev Number: 80 (DW_TAG_GNU_call_site)
-    <37b7>   DW_AT_low_pc      : (addr) 0x2604
-    <37bf>   DW_AT_sibling     : (ref4) <0x37ca>
- <4><37c3>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <37c4>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <37c6>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
- <4><37c9>: Abbrev Number: 0
- <3><37ca>: Abbrev Number: 81 (DW_TAG_GNU_call_site)
-    <37cb>   DW_AT_low_pc      : (addr) 0x2618
-    <37d3>   DW_AT_GNU_tail_call: (flag_present) 1
-    <37d3>   DW_AT_abstract_origin: (ref4) <0x44b0>
- <3><37d7>: Abbrev Number: 0
- <2><37d8>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
-    <37d9>   DW_AT_low_pc      : (addr) 0x259f
-    <37e1>   DW_AT_abstract_origin: (ref4) <0x44bd>
- <3><37e5>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <37e6>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <37e8>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
- <3><37eb>: Abbrev Number: 0
- <2><37ec>: Abbrev Number: 0
- <1><37ed>: Abbrev Number: 10 (DW_TAG_pointer_type)
-    <37ee>   DW_AT_byte_size   : (data1) 8
-    <37ef>   DW_AT_type        : (ref4) <0x247a>, ConsObject
- <1><37f3>: Abbrev Number: 64 (DW_TAG_subprogram)
-    <37f4>   DW_AT_external    : (flag_present) 1
-    <37f4>   DW_AT_name        : (strp) (offset: 0x1849): Cons_clear
-    <37f8>   DW_AT_decl_file   : (data1) 1
-    <37f9>   DW_AT_decl_line   : (data1) 148
-    <37fa>   DW_AT_decl_column : (data1) 1
-    <37fb>   DW_AT_prototyped  : (flag_present) 1
-    <37fb>   DW_AT_type        : (ref4) <0x4f>, int
-    <37ff>   DW_AT_low_pc      : (addr) 0x2530
-    <3807>   DW_AT_high_pc     : (data8) 0x57
-    <380f>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
-    <3811>   DW_AT_GNU_all_call_sites: (flag_present) 1
-    <3811>   DW_AT_sibling     : (ref4) <0x38c2>
- <2><3815>: Abbrev Number: 65 (DW_TAG_formal_parameter)
-    <3816>   DW_AT_name        : (strp) (offset: 0xf72): self
-    <381a>   DW_AT_decl_file   : (data1) 1
-    <381b>   DW_AT_decl_line   : (data1) 148
-    <381c>   DW_AT_decl_column : (data1) 22
-    <381d>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <3821>   DW_AT_location    : (sec_offset) 0x1a1b (location list)
-    <3825>   DW_AT_GNU_locviews: (sec_offset) 0x1a0f
- <2><3829>: Abbrev Number: 46 (DW_TAG_lexical_block)
-    <382a>   DW_AT_ranges      : (sec_offset) 0x70
-    <382e>   DW_AT_sibling     : (ref4) <0x3877>
- <3><3832>: Abbrev Number: 67 (DW_TAG_variable)
-    <3833>   DW_AT_name        : (strp) (offset: 0x19b9): _py_tmp
-    <3837>   DW_AT_decl_file   : (data1) 1
-    <3838>   DW_AT_decl_line   : (data1) 150
-    <3839>   DW_AT_decl_column : (data1) 5
-    <383a>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <383e>   DW_AT_location    : (sec_offset) 0x1aa7 (location list)
-    <3842>   DW_AT_GNU_locviews: (sec_offset) 0x1aa3
- <3><3846>: Abbrev Number: 82 (DW_TAG_inlined_subroutine)
-    <3847>   DW_AT_abstract_origin: (ref4) <0x3e47>
-    <384b>   DW_AT_entry_pc    : (addr) 0x2545
-    <3853>   DW_AT_GNU_entry_view: (data1) 1
-    <3854>   DW_AT_ranges      : (sec_offset) 0xb0
-    <3858>   DW_AT_call_file   : (data1) 1
-    <3859>   DW_AT_call_line   : (data1) 150
-    <385a>   DW_AT_call_column : (data1) 5
- <4><385b>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <385c>   DW_AT_abstract_origin: (ref4) <0x3e55>
-    <3860>   DW_AT_location    : (sec_offset) 0x1ae1 (location list)
-    <3864>   DW_AT_GNU_locviews: (sec_offset) 0x1add
- <4><3868>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
-    <3869>   DW_AT_low_pc      : (addr) 0x2585
-    <3871>   DW_AT_abstract_origin: (ref4) <0x4338>
- <4><3875>: Abbrev Number: 0
- <3><3876>: Abbrev Number: 0
- <2><3877>: Abbrev Number: 58 (DW_TAG_lexical_block)
-    <3878>   DW_AT_ranges      : (sec_offset) 0xe0
- <3><387c>: Abbrev Number: 67 (DW_TAG_variable)
-    <387d>   DW_AT_name        : (strp) (offset: 0x19b9): _py_tmp
-    <3881>   DW_AT_decl_file   : (data1) 1
-    <3882>   DW_AT_decl_line   : (data1) 151
-    <3883>   DW_AT_decl_column : (data1) 5
-    <3884>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <3888>   DW_AT_location    : (sec_offset) 0x1b19 (location list)
-    <388c>   DW_AT_GNU_locviews: (sec_offset) 0x1b17
- <3><3890>: Abbrev Number: 82 (DW_TAG_inlined_subroutine)
-    <3891>   DW_AT_abstract_origin: (ref4) <0x3e47>
-    <3895>   DW_AT_entry_pc    : (addr) 0x255c
-    <389d>   DW_AT_GNU_entry_view: (data1) 1
-    <389e>   DW_AT_ranges      : (sec_offset) 0x110
-    <38a2>   DW_AT_call_file   : (data1) 1
-    <38a3>   DW_AT_call_line   : (data1) 151
-    <38a4>   DW_AT_call_column : (data1) 5
- <4><38a5>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <38a6>   DW_AT_abstract_origin: (ref4) <0x3e55>
-    <38aa>   DW_AT_location    : (sec_offset) 0x1b40 (location list)
-    <38ae>   DW_AT_GNU_locviews: (sec_offset) 0x1b3c
- <4><38b2>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
-    <38b3>   DW_AT_low_pc      : (addr) 0x2575
-    <38bb>   DW_AT_abstract_origin: (ref4) <0x4338>
- <4><38bf>: Abbrev Number: 0
- <3><38c0>: Abbrev Number: 0
- <2><38c1>: Abbrev Number: 0
- <1><38c2>: Abbrev Number: 83 (DW_TAG_subprogram)
-    <38c3>   DW_AT_name        : (strp) (offset: 0x1bf): Cons_traverse
-    <38c7>   DW_AT_decl_file   : (data1) 1
-    <38c8>   DW_AT_decl_line   : (data1) 139
-    <38c9>   DW_AT_decl_column : (data1) 1
-    <38ca>   DW_AT_prototyped  : (flag_present) 1
-    <38ca>   DW_AT_type        : (ref4) <0x4f>, int
-    <38ce>   DW_AT_inline      : (data1) 1	(inlined)
-    <38cf>   DW_AT_sibling     : (ref4) <0x394d>
- <2><38d3>: Abbrev Number: 71 (DW_TAG_formal_parameter)
-    <38d4>   DW_AT_name        : (strp) (offset: 0xf72): self
-    <38d8>   DW_AT_decl_file   : (data1) 1
-    <38d9>   DW_AT_decl_line   : (data1) 139
-    <38da>   DW_AT_decl_column : (data1) 27
-    <38db>   DW_AT_type        : (ref4) <0x37ed>, ConsObject
- <2><38df>: Abbrev Number: 71 (DW_TAG_formal_parameter)
-    <38e0>   DW_AT_name        : (strp) (offset: 0xb21): visit
-    <38e4>   DW_AT_decl_file   : (data1) 1
-    <38e5>   DW_AT_decl_line   : (data1) 139
-    <38e6>   DW_AT_decl_column : (data1) 43
-    <38e7>   DW_AT_type        : (ref4) <0xd03>, visitproc, int
- <2><38eb>: Abbrev Number: 84 (DW_TAG_formal_parameter)
-    <38ec>   DW_AT_name        : (string) arg
-    <38f0>   DW_AT_decl_file   : (data1) 1
-    <38f1>   DW_AT_decl_line   : (data1) 139
-    <38f2>   DW_AT_decl_column : (data1) 56
-    <38f3>   DW_AT_type        : (ref4) <0x88>
- <2><38f7>: Abbrev Number: 85 (DW_TAG_lexical_block)
-    <38f8>   DW_AT_sibling     : (ref4) <0x391c>
- <3><38fc>: Abbrev Number: 72 (DW_TAG_variable)
-    <38fd>   DW_AT_name        : (strp) (offset: 0xb88): vret
-    <3901>   DW_AT_decl_file   : (data1) 1
-    <3902>   DW_AT_decl_line   : (data1) 141
-    <3903>   DW_AT_decl_column : (data1) 5
-    <3904>   DW_AT_type        : (ref4) <0x4f>, int
- <3><3908>: Abbrev Number: 53 (DW_TAG_GNU_call_site)
-    <3909>   DW_AT_low_pc      : (addr) 0x2b5b
-    <3911>   DW_AT_GNU_call_site_target: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
- <4><3914>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3915>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <3917>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7c 0 	(DW_OP_breg12 (r12): 0)
- <4><391a>: Abbrev Number: 0
- <3><391b>: Abbrev Number: 0
- <2><391c>: Abbrev Number: 85 (DW_TAG_lexical_block)
-    <391d>   DW_AT_sibling     : (ref4) <0x393e>
- <3><3921>: Abbrev Number: 72 (DW_TAG_variable)
-    <3922>   DW_AT_name        : (strp) (offset: 0xb88): vret
-    <3926>   DW_AT_decl_file   : (data1) 1
-    <3927>   DW_AT_decl_line   : (data1) 142
-    <3928>   DW_AT_decl_column : (data1) 5
-    <3929>   DW_AT_type        : (ref4) <0x4f>, int
- <3><392d>: Abbrev Number: 54 (DW_TAG_GNU_call_site)
-    <392e>   DW_AT_low_pc      : (addr) 0x2b6d
- <4><3936>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3937>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <3939>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7c 0 	(DW_OP_breg12 (r12): 0)
- <4><393c>: Abbrev Number: 0
- <3><393d>: Abbrev Number: 0
- <2><393e>: Abbrev Number: 73 (DW_TAG_lexical_block)
- <3><393f>: Abbrev Number: 72 (DW_TAG_variable)
-    <3940>   DW_AT_name        : (strp) (offset: 0xb88): vret
-    <3944>   DW_AT_decl_file   : (data1) 1
-    <3945>   DW_AT_decl_line   : (data1) 143
-    <3946>   DW_AT_decl_column : (data1) 5
-    <3947>   DW_AT_type        : (ref4) <0x4f>, int
- <3><394b>: Abbrev Number: 0
- <2><394c>: Abbrev Number: 0
- <1><394d>: Abbrev Number: 64 (DW_TAG_subprogram)
-    <394e>   DW_AT_external    : (flag_present) 1
-    <394e>   DW_AT_name        : (strp) (offset: 0x464): Cons_new
-    <3952>   DW_AT_decl_file   : (data1) 1
-    <3953>   DW_AT_decl_line   : (data1) 105
-    <3954>   DW_AT_decl_column : (data1) 1
-    <3955>   DW_AT_prototyped  : (flag_present) 1
-    <3955>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <3959>   DW_AT_low_pc      : (addr) 0x2400
-    <3961>   DW_AT_high_pc     : (data8) 0x127
-    <3969>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
-    <396b>   DW_AT_GNU_all_call_sites: (flag_present) 1
-    <396b>   DW_AT_sibling     : (ref4) <0x3b8d>
- <2><396f>: Abbrev Number: 65 (DW_TAG_formal_parameter)
-    <3970>   DW_AT_name        : (strp) (offset: 0x2201): type
-    <3974>   DW_AT_decl_file   : (data1) 1
-    <3975>   DW_AT_decl_line   : (data1) 105
-    <3976>   DW_AT_decl_column : (data1) 24
-    <3977>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
-    <397b>   DW_AT_location    : (sec_offset) 0x1b7e (location list)
-    <397f>   DW_AT_GNU_locviews: (sec_offset) 0x1b76
- <2><3983>: Abbrev Number: 65 (DW_TAG_formal_parameter)
-    <3984>   DW_AT_name        : (strp) (offset: 0x543): args
-    <3988>   DW_AT_decl_file   : (data1) 1
-    <3989>   DW_AT_decl_line   : (data1) 105
-    <398a>   DW_AT_decl_column : (data1) 40
-    <398b>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <398f>   DW_AT_location    : (sec_offset) 0x1be5 (location list)
-    <3993>   DW_AT_GNU_locviews: (sec_offset) 0x1bdd
- <2><3997>: Abbrev Number: 65 (DW_TAG_formal_parameter)
-    <3998>   DW_AT_name        : (strp) (offset: 0x2040): kwds
-    <399c>   DW_AT_decl_file   : (data1) 1
-    <399d>   DW_AT_decl_line   : (data1) 105
-    <399e>   DW_AT_decl_column : (data1) 56
-    <399f>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <39a3>   DW_AT_location    : (sec_offset) 0x1c4c (location list)
-    <39a7>   DW_AT_GNU_locviews: (sec_offset) 0x1c44
- <2><39ab>: Abbrev Number: 67 (DW_TAG_variable)
-    <39ac>   DW_AT_name        : (strp) (offset: 0xf72): self
-    <39b0>   DW_AT_decl_file   : (data1) 1
-    <39b1>   DW_AT_decl_line   : (data1) 107
-    <39b2>   DW_AT_decl_column : (data1) 17
-    <39b3>   DW_AT_type        : (ref4) <0x37ed>, ConsObject
-    <39b7>   DW_AT_location    : (sec_offset) 0x1cb3 (location list)
-    <39bb>   DW_AT_GNU_locviews: (sec_offset) 0x1cab
- <2><39bf>: Abbrev Number: 38 (DW_TAG_variable)
-    <39c0>   DW_AT_name        : (strp) (offset: 0xc3d): kwlist
-    <39c4>   DW_AT_decl_file   : (data1) 1
-    <39c5>   DW_AT_decl_line   : (data1) 112
-    <39c6>   DW_AT_decl_column : (data1) 18
-    <39c7>   DW_AT_type        : (ref4) <0x3b8d>, char
-    <39cb>   DW_AT_location    : (exprloc) 9 byte block: 3 20 50 0 0 0 0 0 0 	(DW_OP_addr: 5020)
- <2><39d5>: Abbrev Number: 38 (DW_TAG_variable)
-    <39d6>   DW_AT_name        : (strp) (offset: 0x652): head
-    <39da>   DW_AT_decl_file   : (data1) 1
-    <39db>   DW_AT_decl_line   : (data1) 113
-    <39dc>   DW_AT_decl_column : (data1) 15
-    <39dd>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <39e1>   DW_AT_location    : (exprloc) 3 byte block: 91 b8 7f 	(DW_OP_fbreg: -72)
- <2><39e5>: Abbrev Number: 38 (DW_TAG_variable)
-    <39e6>   DW_AT_name        : (strp) (offset: 0x203b): tail
-    <39ea>   DW_AT_decl_file   : (data1) 1
-    <39eb>   DW_AT_decl_line   : (data1) 113
-    <39ec>   DW_AT_decl_column : (data1) 29
-    <39ed>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <39f1>   DW_AT_location    : (exprloc) 2 byte block: 91 40 	(DW_OP_fbreg: -64)
- <2><39f4>: Abbrev Number: 67 (DW_TAG_variable)
-    <39f5>   DW_AT_name        : (strp) (offset: 0x58c): state
-    <39f9>   DW_AT_decl_file   : (data1) 1
-    <39fa>   DW_AT_decl_line   : (data1) 119
-    <39fb>   DW_AT_decl_column : (data1) 23
-    <39fc>   DW_AT_type        : (ref4) <0x274d>, consmodule_state
-    <3a00>   DW_AT_location    : (sec_offset) 0x1d13 (location list)
-    <3a04>   DW_AT_GNU_locviews: (sec_offset) 0x1d0f
- <2><3a08>: Abbrev Number: 67 (DW_TAG_variable)
-    <3a09>   DW_AT_name        : (strp) (offset: 0x2327): cons
-    <3a0d>   DW_AT_decl_file   : (data1) 1
-    <3a0e>   DW_AT_decl_line   : (data1) 122
-    <3a0f>   DW_AT_decl_column : (data1) 19
-    <3a10>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
-    <3a14>   DW_AT_location    : (sec_offset) 0x1d4d (location list)
-    <3a18>   DW_AT_GNU_locviews: (sec_offset) 0x1d49
- <2><3a1c>: Abbrev Number: 77 (DW_TAG_inlined_subroutine)
-    <3a1d>   DW_AT_abstract_origin: (ref4) <0x3ea9>
-    <3a21>   DW_AT_entry_pc    : (addr) 0x248b
-    <3a29>   DW_AT_GNU_entry_view: (data1) 1
-    <3a2a>   DW_AT_low_pc      : (addr) 0x248b
-    <3a32>   DW_AT_high_pc     : (data8) 0
-    <3a3a>   DW_AT_call_file   : (data1) 1
-    <3a3b>   DW_AT_call_line   : (data1) 126
-    <3a3c>   DW_AT_call_column : (data1) 14
-    <3a3d>   DW_AT_sibling     : (ref4) <0x3a5c>
- <3><3a41>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <3a42>   DW_AT_abstract_origin: (ref4) <0x3ec5>
-    <3a46>   DW_AT_location    : (sec_offset) 0x1d87 (location list)
-    <3a4a>   DW_AT_GNU_locviews: (sec_offset) 0x1d85
- <3><3a4e>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <3a4f>   DW_AT_abstract_origin: (ref4) <0x3eba>
-    <3a53>   DW_AT_location    : (sec_offset) 0x1dad (location list)
-    <3a57>   DW_AT_GNU_locviews: (sec_offset) 0x1dab
- <3><3a5b>: Abbrev Number: 0
- <2><3a5c>: Abbrev Number: 77 (DW_TAG_inlined_subroutine)
-    <3a5d>   DW_AT_abstract_origin: (ref4) <0x3e62>
-    <3a61>   DW_AT_entry_pc    : (addr) 0x24a3
-    <3a69>   DW_AT_GNU_entry_view: (data1) 0
-    <3a6a>   DW_AT_low_pc      : (addr) 0x24a3
-    <3a72>   DW_AT_high_pc     : (data8) 0x4
-    <3a7a>   DW_AT_call_file   : (data1) 1
-    <3a7b>   DW_AT_call_line   : (data1) 131
-    <3a7c>   DW_AT_call_column : (data1) 5
-    <3a7d>   DW_AT_sibling     : (ref4) <0x3a8f>
- <3><3a81>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <3a82>   DW_AT_abstract_origin: (ref4) <0x3e70>
-    <3a86>   DW_AT_location    : (sec_offset) 0x1dd4 (location list)
-    <3a8a>   DW_AT_GNU_locviews: (sec_offset) 0x1dd0
- <3><3a8e>: Abbrev Number: 0
- <2><3a8f>: Abbrev Number: 77 (DW_TAG_inlined_subroutine)
-    <3a90>   DW_AT_abstract_origin: (ref4) <0x3e62>
-    <3a94>   DW_AT_entry_pc    : (addr) 0x24ac
-    <3a9c>   DW_AT_GNU_entry_view: (data1) 1
-    <3a9d>   DW_AT_low_pc      : (addr) 0x24ac
-    <3aa5>   DW_AT_high_pc     : (data8) 0x4
-    <3aad>   DW_AT_call_file   : (data1) 1
-    <3aae>   DW_AT_call_line   : (data1) 133
-    <3aaf>   DW_AT_call_column : (data1) 5
-    <3ab0>   DW_AT_sibling     : (ref4) <0x3ac2>
- <3><3ab4>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <3ab5>   DW_AT_abstract_origin: (ref4) <0x3e70>
-    <3ab9>   DW_AT_location    : (sec_offset) 0x1e0c (location list)
-    <3abd>   DW_AT_GNU_locviews: (sec_offset) 0x1e0a
- <3><3ac1>: Abbrev Number: 0
- <2><3ac2>: Abbrev Number: 77 (DW_TAG_inlined_subroutine)
-    <3ac3>   DW_AT_abstract_origin: (ref4) <0x3e47>
-    <3ac7>   DW_AT_entry_pc    : (addr) 0x24d8
-    <3acf>   DW_AT_GNU_entry_view: (data1) 2
-    <3ad0>   DW_AT_low_pc      : (addr) 0x24d8
-    <3ad8>   DW_AT_high_pc     : (data8) 0x18
-    <3ae0>   DW_AT_call_file   : (data1) 1
-    <3ae1>   DW_AT_call_line   : (data1) 115
-    <3ae2>   DW_AT_call_column : (data1) 9
-    <3ae3>   DW_AT_sibling     : (ref4) <0x3b09>
- <3><3ae7>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <3ae8>   DW_AT_abstract_origin: (ref4) <0x3e55>
-    <3aec>   DW_AT_location    : (sec_offset) 0x1e31 (location list)
-    <3af0>   DW_AT_GNU_locviews: (sec_offset) 0x1e2f
- <3><3af4>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
-    <3af5>   DW_AT_low_pc      : (addr) 0x24e7
-    <3afd>   DW_AT_abstract_origin: (ref4) <0x4338>
- <4><3b01>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3b02>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <3b04>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7c 0 	(DW_OP_breg12 (r12): 0)
- <4><3b07>: Abbrev Number: 0
- <3><3b08>: Abbrev Number: 0
- <2><3b09>: Abbrev Number: 80 (DW_TAG_GNU_call_site)
-    <3b0a>   DW_AT_low_pc      : (addr) 0x242c
-    <3b12>   DW_AT_sibling     : (ref4) <0x3b22>
- <3><3b16>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3b17>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <3b19>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
- <3><3b1c>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3b1d>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <3b1f>   DW_AT_GNU_call_site_value: (exprloc) 1 byte block: 30 	(DW_OP_lit0)
- <3><3b21>: Abbrev Number: 0
- <2><3b22>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <3b23>   DW_AT_low_pc      : (addr) 0x246f
-    <3b2b>   DW_AT_abstract_origin: (ref4) <0x44c9>
-    <3b2f>   DW_AT_sibling     : (ref4) <0x3b67>
- <3><3b33>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3b34>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <3b36>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7d 0 	(DW_OP_breg13 (r13): 0)
- <3><3b39>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3b3a>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <3b3c>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7e 0 	(DW_OP_breg14 (r14): 0)
- <3><3b3f>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3b40>   DW_AT_location    : (exprloc) 1 byte block: 51 	(DW_OP_reg1 (rdx))
-    <3b42>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 6 30 0 0 0 0 0 0 	(DW_OP_addr: 3006)
- <3><3b4c>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3b4d>   DW_AT_location    : (exprloc) 1 byte block: 52 	(DW_OP_reg2 (rcx))
-    <3b4f>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 20 50 0 0 0 0 0 0 	(DW_OP_addr: 5020)
- <3><3b59>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3b5a>   DW_AT_location    : (exprloc) 1 byte block: 58 	(DW_OP_reg8 (r8))
-    <3b5c>   DW_AT_GNU_call_site_value: (exprloc) 3 byte block: 91 b8 7f 	(DW_OP_fbreg: -72)
- <3><3b60>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3b61>   DW_AT_location    : (exprloc) 1 byte block: 59 	(DW_OP_reg9 (r9))
-    <3b63>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 91 40 	(DW_OP_fbreg: -64)
- <3><3b66>: Abbrev Number: 0
- <2><3b67>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <3b68>   DW_AT_low_pc      : (addr) 0x247b
-    <3b70>   DW_AT_abstract_origin: (ref4) <0x439a>
-    <3b74>   DW_AT_sibling     : (ref4) <0x3b7f>
- <3><3b78>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3b79>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <3b7b>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
- <3><3b7e>: Abbrev Number: 0
- <2><3b7f>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
-    <3b80>   DW_AT_low_pc      : (addr) 0x2527
-    <3b88>   DW_AT_abstract_origin: (ref4) <0x4442>
- <2><3b8c>: Abbrev Number: 0
- <1><3b8d>: Abbrev Number: 12 (DW_TAG_array_type)
-    <3b8e>   DW_AT_type        : (ref4) <0xea>, char
-    <3b92>   DW_AT_sibling     : (ref4) <0x3b9d>
- <2><3b96>: Abbrev Number: 13 (DW_TAG_subrange_type)
-    <3b97>   DW_AT_type        : (ref4) <0x62>, long unsigned int
-    <3b9b>   DW_AT_upper_bound : (data1) 2
- <2><3b9c>: Abbrev Number: 0
- <1><3b9d>: Abbrev Number: 86 (DW_TAG_subprogram)
-    <3b9e>   DW_AT_name        : (strp) (offset: 0x1ab9): Nil_bool
-    <3ba2>   DW_AT_decl_file   : (data1) 1
-    <3ba3>   DW_AT_decl_line   : (data1) 77
-    <3ba4>   DW_AT_decl_column : (data1) 1
-    <3ba5>   DW_AT_prototyped  : (flag_present) 1
-    <3ba5>   DW_AT_type        : (ref4) <0x4f>, int
-    <3ba9>   DW_AT_low_pc      : (addr) 0x23e0
-    <3bb1>   DW_AT_high_pc     : (data8) 0x3
-    <3bb9>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
-    <3bbb>   DW_AT_GNU_all_call_sites: (flag_present) 1
-    <3bbb>   DW_AT_sibling     : (ref4) <0x3bce>
- <2><3bbf>: Abbrev Number: 87 (DW_TAG_formal_parameter)
-    <3bc0>   DW_AT_name        : (strp) (offset: 0xf72): self
-    <3bc4>   DW_AT_decl_file   : (data1) 1
-    <3bc5>   DW_AT_decl_line   : (data1) 77
-    <3bc6>   DW_AT_decl_column : (data1) 20
-    <3bc7>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <3bcb>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
- <2><3bcd>: Abbrev Number: 0
- <1><3bce>: Abbrev Number: 83 (DW_TAG_subprogram)
-    <3bcf>   DW_AT_name        : (strp) (offset: 0xe7c): Nil_new
-    <3bd3>   DW_AT_decl_file   : (data1) 1
-    <3bd4>   DW_AT_decl_line   : (data1) 61
-    <3bd5>   DW_AT_decl_column : (data1) 1
-    <3bd6>   DW_AT_prototyped  : (flag_present) 1
-    <3bd6>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <3bda>   DW_AT_inline      : (data1) 1	(inlined)
-    <3bdb>   DW_AT_sibling     : (ref4) <0x3c1c>
- <2><3bdf>: Abbrev Number: 71 (DW_TAG_formal_parameter)
-    <3be0>   DW_AT_name        : (strp) (offset: 0x2201): type
-    <3be4>   DW_AT_decl_file   : (data1) 1
-    <3be5>   DW_AT_decl_line   : (data1) 61
-    <3be6>   DW_AT_decl_column : (data1) 23
-    <3be7>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
- <2><3beb>: Abbrev Number: 71 (DW_TAG_formal_parameter)
-    <3bec>   DW_AT_name        : (strp) (offset: 0x543): args
-    <3bf0>   DW_AT_decl_file   : (data1) 1
-    <3bf1>   DW_AT_decl_line   : (data1) 61
-    <3bf2>   DW_AT_decl_column : (data1) 39
-    <3bf3>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><3bf7>: Abbrev Number: 71 (DW_TAG_formal_parameter)
-    <3bf8>   DW_AT_name        : (strp) (offset: 0x2040): kwds
-    <3bfc>   DW_AT_decl_file   : (data1) 1
-    <3bfd>   DW_AT_decl_line   : (data1) 61
-    <3bfe>   DW_AT_decl_column : (data1) 55
-    <3bff>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><3c03>: Abbrev Number: 72 (DW_TAG_variable)
-    <3c04>   DW_AT_name        : (strp) (offset: 0x58c): state
-    <3c08>   DW_AT_decl_file   : (data1) 1
-    <3c09>   DW_AT_decl_line   : (data1) 68
-    <3c0a>   DW_AT_decl_column : (data1) 23
-    <3c0b>   DW_AT_type        : (ref4) <0x274d>, consmodule_state
- <2><3c0f>: Abbrev Number: 72 (DW_TAG_variable)
-    <3c10>   DW_AT_name        : (strp) (offset: 0xf72): self
-    <3c14>   DW_AT_decl_file   : (data1) 1
-    <3c15>   DW_AT_decl_line   : (data1) 71
-    <3c16>   DW_AT_decl_column : (data1) 15
-    <3c17>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><3c1b>: Abbrev Number: 0
- <1><3c1c>: Abbrev Number: 64 (DW_TAG_subprogram)
-    <3c1d>   DW_AT_external    : (flag_present) 1
-    <3c1d>   DW_AT_name        : (strp) (offset: 0x1e94): Nil_repr
-    <3c21>   DW_AT_decl_file   : (data1) 1
-    <3c22>   DW_AT_decl_line   : (data1) 55
-    <3c23>   DW_AT_decl_column : (data1) 1
-    <3c24>   DW_AT_prototyped  : (flag_present) 1
-    <3c24>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <3c28>   DW_AT_low_pc      : (addr) 0x23f0
-    <3c30>   DW_AT_high_pc     : (data8) 0xc
-    <3c38>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
-    <3c3a>   DW_AT_GNU_all_call_sites: (flag_present) 1
-    <3c3a>   DW_AT_sibling     : (ref4) <0x3c6e>
- <2><3c3e>: Abbrev Number: 65 (DW_TAG_formal_parameter)
-    <3c3f>   DW_AT_name        : (strp) (offset: 0xf72): self
-    <3c43>   DW_AT_decl_file   : (data1) 1
-    <3c44>   DW_AT_decl_line   : (data1) 55
-    <3c45>   DW_AT_decl_column : (data1) 20
-    <3c46>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <3c4a>   DW_AT_location    : (sec_offset) 0x1e58 (location list)
-    <3c4e>   DW_AT_GNU_locviews: (sec_offset) 0x1e54
- <2><3c52>: Abbrev Number: 41 (DW_TAG_GNU_call_site)
-    <3c53>   DW_AT_low_pc      : (addr) 0x23fc
-    <3c5b>   DW_AT_GNU_tail_call: (flag_present) 1
-    <3c5b>   DW_AT_abstract_origin: (ref4) <0x4375>
- <3><3c5f>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3c60>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <3c62>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 0 30 0 0 0 0 0 0 	(DW_OP_addr: 3000)
- <3><3c6c>: Abbrev Number: 0
- <2><3c6d>: Abbrev Number: 0
- <1><3c6e>: Abbrev Number: 86 (DW_TAG_subprogram)
-    <3c6f>   DW_AT_name        : (strp) (offset: 0x1287): Nil_traverse
-    <3c73>   DW_AT_decl_file   : (data1) 1
-    <3c74>   DW_AT_decl_line   : (data1) 48
-    <3c75>   DW_AT_decl_column : (data1) 1
-    <3c76>   DW_AT_prototyped  : (flag_present) 1
-    <3c76>   DW_AT_type        : (ref4) <0x4f>, int
-    <3c7a>   DW_AT_low_pc      : (addr) 0x23c0
-    <3c82>   DW_AT_high_pc     : (data8) 0x1b
-    <3c8a>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
-    <3c8c>   DW_AT_GNU_all_call_sites: (flag_present) 1
-    <3c8c>   DW_AT_sibling     : (ref4) <0x3cf4>
- <2><3c90>: Abbrev Number: 65 (DW_TAG_formal_parameter)
-    <3c91>   DW_AT_name        : (strp) (offset: 0xf72): self
-    <3c95>   DW_AT_decl_file   : (data1) 1
-    <3c96>   DW_AT_decl_line   : (data1) 48
-    <3c97>   DW_AT_decl_column : (data1) 25
-    <3c98>   DW_AT_type        : (ref4) <0x3cf4>, NilObject
-    <3c9c>   DW_AT_location    : (sec_offset) 0x1e95 (location list)
-    <3ca0>   DW_AT_GNU_locviews: (sec_offset) 0x1e91
- <2><3ca4>: Abbrev Number: 65 (DW_TAG_formal_parameter)
-    <3ca5>   DW_AT_name        : (strp) (offset: 0xb21): visit
-    <3ca9>   DW_AT_decl_file   : (data1) 1
-    <3caa>   DW_AT_decl_line   : (data1) 48
-    <3cab>   DW_AT_decl_column : (data1) 41
-    <3cac>   DW_AT_type        : (ref4) <0xd03>, visitproc, int
-    <3cb0>   DW_AT_location    : (sec_offset) 0x1ed8 (location list)
-    <3cb4>   DW_AT_GNU_locviews: (sec_offset) 0x1ece
- <2><3cb8>: Abbrev Number: 76 (DW_TAG_formal_parameter)
-    <3cb9>   DW_AT_name        : (string) arg
-    <3cbd>   DW_AT_decl_file   : (data1) 1
-    <3cbe>   DW_AT_decl_line   : (data1) 48
-    <3cbf>   DW_AT_decl_column : (data1) 54
-    <3cc0>   DW_AT_type        : (ref4) <0x88>
-    <3cc4>   DW_AT_location    : (sec_offset) 0x1f53 (location list)
-    <3cc8>   DW_AT_GNU_locviews: (sec_offset) 0x1f4d
- <2><3ccc>: Abbrev Number: 58 (DW_TAG_lexical_block)
-    <3ccd>   DW_AT_ranges      : (sec_offset) 0x40
- <3><3cd1>: Abbrev Number: 72 (DW_TAG_variable)
-    <3cd2>   DW_AT_name        : (strp) (offset: 0xb88): vret
-    <3cd6>   DW_AT_decl_file   : (data1) 1
-    <3cd7>   DW_AT_decl_line   : (data1) 50
-    <3cd8>   DW_AT_decl_column : (data1) 5
-    <3cd9>   DW_AT_type        : (ref4) <0x4f>, int
- <3><3cdd>: Abbrev Number: 55 (DW_TAG_GNU_call_site)
-    <3cde>   DW_AT_low_pc      : (addr) 0x23d1
-    <3ce6>   DW_AT_GNU_tail_call: (flag_present) 1
-    <3ce6>   DW_AT_GNU_call_site_target: (exprloc) 3 byte block: f3 1 54 	(DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)))
- <4><3cea>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3ceb>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <3ced>   DW_AT_GNU_call_site_value: (exprloc) 3 byte block: f3 1 51 	(DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)))
- <4><3cf1>: Abbrev Number: 0
- <3><3cf2>: Abbrev Number: 0
- <2><3cf3>: Abbrev Number: 0
- <1><3cf4>: Abbrev Number: 10 (DW_TAG_pointer_type)
-    <3cf5>   DW_AT_byte_size   : (data1) 8
-    <3cf6>   DW_AT_type        : (ref4) <0x23c9>, NilObject
- <1><3cfa>: Abbrev Number: 88 (DW_TAG_subprogram)
-    <3cfb>   DW_AT_name        : (strp) (offset: 0x2259): PyList_SET_ITEM
-    <3cff>   DW_AT_decl_file   : (data1) 4
-    <3d00>   DW_AT_decl_line   : (data1) 44
-    <3d01>   DW_AT_decl_column : (data1) 1
-    <3d02>   DW_AT_prototyped  : (flag_present) 1
-    <3d02>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
-    <3d03>   DW_AT_sibling     : (ref4) <0x3d37>
- <2><3d07>: Abbrev Number: 84 (DW_TAG_formal_parameter)
-    <3d08>   DW_AT_name        : (string) op
-    <3d0b>   DW_AT_decl_file   : (data1) 4
-    <3d0c>   DW_AT_decl_line   : (data1) 44
-    <3d0d>   DW_AT_decl_column : (data1) 27
-    <3d0e>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><3d12>: Abbrev Number: 71 (DW_TAG_formal_parameter)
-    <3d13>   DW_AT_name        : (strp) (offset: 0x1a08): index
-    <3d17>   DW_AT_decl_file   : (data1) 4
-    <3d18>   DW_AT_decl_line   : (data1) 44
-    <3d19>   DW_AT_decl_column : (data1) 42
-    <3d1a>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
- <2><3d1e>: Abbrev Number: 71 (DW_TAG_formal_parameter)
-    <3d1f>   DW_AT_name        : (strp) (offset: 0xb09): value
-    <3d23>   DW_AT_decl_file   : (data1) 4
-    <3d24>   DW_AT_decl_line   : (data1) 44
-    <3d25>   DW_AT_decl_column : (data1) 59
-    <3d26>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><3d2a>: Abbrev Number: 72 (DW_TAG_variable)
-    <3d2b>   DW_AT_name        : (strp) (offset: 0x99d): list
-    <3d2f>   DW_AT_decl_file   : (data1) 4
-    <3d30>   DW_AT_decl_line   : (data1) 45
-    <3d31>   DW_AT_decl_column : (data1) 19
-    <3d32>   DW_AT_type        : (ref4) <0x3d37>, PyListObject
- <2><3d36>: Abbrev Number: 0
- <1><3d37>: Abbrev Number: 10 (DW_TAG_pointer_type)
-    <3d38>   DW_AT_byte_size   : (data1) 8
-    <3d39>   DW_AT_type        : (ref4) <0x18a7>, PyListObject
- <1><3d3d>: Abbrev Number: 83 (DW_TAG_subprogram)
-    <3d3e>   DW_AT_name        : (strp) (offset: 0x7c5): PyList_GET_SIZE
-    <3d42>   DW_AT_decl_file   : (data1) 4
-    <3d43>   DW_AT_decl_line   : (data1) 33
-    <3d44>   DW_AT_decl_column : (data1) 26
-    <3d45>   DW_AT_prototyped  : (flag_present) 1
-    <3d45>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
-    <3d49>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
-    <3d4a>   DW_AT_sibling     : (ref4) <0x3d66>
- <2><3d4e>: Abbrev Number: 84 (DW_TAG_formal_parameter)
-    <3d4f>   DW_AT_name        : (string) op
-    <3d52>   DW_AT_decl_file   : (data1) 4
-    <3d53>   DW_AT_decl_line   : (data1) 33
-    <3d54>   DW_AT_decl_column : (data1) 52
-    <3d55>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><3d59>: Abbrev Number: 72 (DW_TAG_variable)
-    <3d5a>   DW_AT_name        : (strp) (offset: 0x99d): list
-    <3d5e>   DW_AT_decl_file   : (data1) 4
-    <3d5f>   DW_AT_decl_line   : (data1) 34
-    <3d60>   DW_AT_decl_column : (data1) 19
-    <3d61>   DW_AT_type        : (ref4) <0x3d37>, PyListObject
- <2><3d65>: Abbrev Number: 0
- <1><3d66>: Abbrev Number: 88 (DW_TAG_subprogram)
-    <3d67>   DW_AT_name        : (strp) (offset: 0x2c5): PyTuple_SET_ITEM
-    <3d6b>   DW_AT_decl_file   : (data1) 3
-    <3d6c>   DW_AT_decl_line   : (data1) 34
-    <3d6d>   DW_AT_decl_column : (data1) 1
-    <3d6e>   DW_AT_prototyped  : (flag_present) 1
-    <3d6e>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
-    <3d6f>   DW_AT_sibling     : (ref4) <0x3da3>
- <2><3d73>: Abbrev Number: 84 (DW_TAG_formal_parameter)
-    <3d74>   DW_AT_name        : (string) op
-    <3d77>   DW_AT_decl_file   : (data1) 3
-    <3d78>   DW_AT_decl_line   : (data1) 34
-    <3d79>   DW_AT_decl_column : (data1) 28
-    <3d7a>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><3d7e>: Abbrev Number: 71 (DW_TAG_formal_parameter)
-    <3d7f>   DW_AT_name        : (strp) (offset: 0x1a08): index
-    <3d83>   DW_AT_decl_file   : (data1) 3
-    <3d84>   DW_AT_decl_line   : (data1) 34
-    <3d85>   DW_AT_decl_column : (data1) 43
-    <3d86>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
- <2><3d8a>: Abbrev Number: 71 (DW_TAG_formal_parameter)
-    <3d8b>   DW_AT_name        : (strp) (offset: 0xb09): value
-    <3d8f>   DW_AT_decl_file   : (data1) 3
-    <3d90>   DW_AT_decl_line   : (data1) 34
-    <3d91>   DW_AT_decl_column : (data1) 60
-    <3d92>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><3d96>: Abbrev Number: 72 (DW_TAG_variable)
-    <3d97>   DW_AT_name        : (strp) (offset: 0x677): tuple
-    <3d9b>   DW_AT_decl_file   : (data1) 3
-    <3d9c>   DW_AT_decl_line   : (data1) 35
-    <3d9d>   DW_AT_decl_column : (data1) 20
-    <3d9e>   DW_AT_type        : (ref4) <0x3da3>, PyTupleObject
- <2><3da2>: Abbrev Number: 0
- <1><3da3>: Abbrev Number: 10 (DW_TAG_pointer_type)
-    <3da4>   DW_AT_byte_size   : (data1) 8
-    <3da5>   DW_AT_type        : (ref4) <0x1846>, PyTupleObject
- <1><3da9>: Abbrev Number: 83 (DW_TAG_subprogram)
-    <3daa>   DW_AT_name        : (strp) (offset: 0x17d7): PyTuple_GET_SIZE
-    <3dae>   DW_AT_decl_file   : (data1) 3
-    <3daf>   DW_AT_decl_line   : (data1) 22
-    <3db0>   DW_AT_decl_column : (data1) 26
-    <3db1>   DW_AT_prototyped  : (flag_present) 1
-    <3db1>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
-    <3db5>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
-    <3db6>   DW_AT_sibling     : (ref4) <0x3dd2>
- <2><3dba>: Abbrev Number: 84 (DW_TAG_formal_parameter)
-    <3dbb>   DW_AT_name        : (string) op
-    <3dbe>   DW_AT_decl_file   : (data1) 3
-    <3dbf>   DW_AT_decl_line   : (data1) 22
-    <3dc0>   DW_AT_decl_column : (data1) 53
-    <3dc1>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><3dc5>: Abbrev Number: 72 (DW_TAG_variable)
-    <3dc6>   DW_AT_name        : (strp) (offset: 0x677): tuple
-    <3dca>   DW_AT_decl_file   : (data1) 3
-    <3dcb>   DW_AT_decl_line   : (data1) 23
-    <3dcc>   DW_AT_decl_column : (data1) 20
-    <3dcd>   DW_AT_type        : (ref4) <0x3da3>, PyTupleObject
- <2><3dd1>: Abbrev Number: 0
- <1><3dd2>: Abbrev Number: 89 (DW_TAG_subprogram)
-    <3dd3>   DW_AT_name        : (strp) (offset: 0x15af): PyType_HasFeature
-    <3dd7>   DW_AT_decl_file   : (data1) 2
-    <3dd8>   DW_AT_decl_line   : (data2) 763
-    <3dda>   DW_AT_decl_column : (data1) 1
-    <3ddb>   DW_AT_prototyped  : (flag_present) 1
-    <3ddb>   DW_AT_type        : (ref4) <0x4f>, int
+    <3525>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3527>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <3><352a>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <352b>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <352d>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7d 0 	(DW_OP_breg13 (r13): 0)
+ <3><3530>: Abbrev Number: 0
+ <2><3531>: Abbrev Number: 0
+ <1><3532>: Abbrev Number: 64 (DW_TAG_subprogram)
+    <3533>   DW_AT_external    : (flag_present) 1
+    <3533>   DW_AT_name        : (strp) (offset: 0x1395): Cons_from_fast
+    <3537>   DW_AT_decl_file   : (data1) 1
+    <3538>   DW_AT_decl_line   : (data1) 166
+    <3539>   DW_AT_decl_column : (data1) 1
+    <353a>   DW_AT_prototyped  : (flag_present) 1
+    <353a>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <353e>   DW_AT_low_pc      : (addr) 0x2ca0
+    <3546>   DW_AT_high_pc     : (data8) 0xb7
+    <354e>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
+    <3550>   DW_AT_GNU_all_call_sites: (flag_present) 1
+    <3550>   DW_AT_sibling     : (ref4) <0x37af>
+ <2><3554>: Abbrev Number: 76 (DW_TAG_formal_parameter)
+    <3555>   DW_AT_name        : (string) xs
+    <3558>   DW_AT_decl_file   : (data1) 1
+    <3559>   DW_AT_decl_line   : (data1) 166
+    <355a>   DW_AT_decl_column : (data1) 26
+    <355b>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <355f>   DW_AT_location    : (sec_offset) 0x15a8 (location list)
+    <3563>   DW_AT_GNU_locviews: (sec_offset) 0x15a0
+ <2><3567>: Abbrev Number: 65 (DW_TAG_formal_parameter)
+    <3568>   DW_AT_name        : (strp) (offset: 0x58c): state
+    <356c>   DW_AT_decl_file   : (data1) 1
+    <356d>   DW_AT_decl_line   : (data1) 166
+    <356e>   DW_AT_decl_column : (data1) 48
+    <356f>   DW_AT_type        : (ref4) <0x274d>, consmodule_state
+    <3573>   DW_AT_location    : (sec_offset) 0x160b (location list)
+    <3577>   DW_AT_GNU_locviews: (sec_offset) 0x1607
+ <2><357b>: Abbrev Number: 74 (DW_TAG_variable)
+    <357c>   DW_AT_name        : (string) nil
+    <3580>   DW_AT_decl_file   : (data1) 1
+    <3581>   DW_AT_decl_line   : (data1) 168
+    <3582>   DW_AT_decl_column : (data1) 15
+    <3583>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <3587>   DW_AT_location    : (sec_offset) 0x1646 (location list)
+    <358b>   DW_AT_GNU_locviews: (sec_offset) 0x1644
+ <2><358f>: Abbrev Number: 73 (DW_TAG_variable)
+    <3590>   DW_AT_name        : (strp) (offset: 0x2327): cons
+    <3594>   DW_AT_decl_file   : (data1) 1
+    <3595>   DW_AT_decl_line   : (data1) 170
+    <3596>   DW_AT_decl_column : (data1) 15
+    <3597>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <359b>   DW_AT_location    : (sec_offset) 0x166d (location list)
+    <359f>   DW_AT_GNU_locviews: (sec_offset) 0x1669
+ <2><35a3>: Abbrev Number: 74 (DW_TAG_variable)
+    <35a4>   DW_AT_name        : (string) len
+    <35a8>   DW_AT_decl_file   : (data1) 1
+    <35a9>   DW_AT_decl_line   : (data1) 172
+    <35aa>   DW_AT_decl_column : (data1) 16
+    <35ab>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
+    <35af>   DW_AT_location    : (sec_offset) 0x16a5 (location list)
+    <35b3>   DW_AT_GNU_locviews: (sec_offset) 0x16a3
+ <2><35b7>: Abbrev Number: 73 (DW_TAG_variable)
+    <35b8>   DW_AT_name        : (strp) (offset: 0x4d0): result
+    <35bc>   DW_AT_decl_file   : (data1) 1
+    <35bd>   DW_AT_decl_line   : (data1) 173
+    <35be>   DW_AT_decl_column : (data1) 15
+    <35bf>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <35c3>   DW_AT_location    : (sec_offset) 0x16d3 (location list)
+    <35c7>   DW_AT_GNU_locviews: (sec_offset) 0x16c9
+ <2><35cb>: Abbrev Number: 73 (DW_TAG_variable)
+    <35cc>   DW_AT_name        : (strp) (offset: 0x1c68): item
+    <35d0>   DW_AT_decl_file   : (data1) 1
+    <35d1>   DW_AT_decl_line   : (data1) 173
+    <35d2>   DW_AT_decl_column : (data1) 30
+    <35d3>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <35d7>   DW_AT_location    : (sec_offset) 0x174c (location list)
+    <35db>   DW_AT_GNU_locviews: (sec_offset) 0x1742
+ <2><35df>: Abbrev Number: 46 (DW_TAG_lexical_block)
+    <35e0>   DW_AT_ranges      : (sec_offset) 0x5e0
+    <35e4>   DW_AT_sibling     : (ref4) <0x370f>
+ <3><35e8>: Abbrev Number: 74 (DW_TAG_variable)
+    <35e9>   DW_AT_name        : (string) i
+    <35eb>   DW_AT_decl_file   : (data1) 1
+    <35ec>   DW_AT_decl_line   : (data1) 174
+    <35ed>   DW_AT_decl_column : (data1) 21
+    <35ee>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
+    <35f2>   DW_AT_location    : (sec_offset) 0x17c7 (location list)
+    <35f6>   DW_AT_GNU_locviews: (sec_offset) 0x17bd
+ <3><35fa>: Abbrev Number: 77 (DW_TAG_inlined_subroutine)
+    <35fb>   DW_AT_abstract_origin: (ref4) <0x3f3f>
+    <35ff>   DW_AT_entry_pc    : (addr) 0x2cd8
+    <3607>   DW_AT_GNU_entry_view: (data1) 1
+    <3608>   DW_AT_low_pc      : (addr) 0x2cd8
+    <3610>   DW_AT_high_pc     : (data8) 0x5
+    <3618>   DW_AT_call_file   : (data1) 1
+    <3619>   DW_AT_call_line   : (data1) 176
+    <361a>   DW_AT_call_column : (data1) 9
+    <361b>   DW_AT_sibling     : (ref4) <0x362d>
+ <4><361f>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <3620>   DW_AT_abstract_origin: (ref4) <0x3f4d>
+    <3624>   DW_AT_location    : (sec_offset) 0x1843 (location list)
+    <3628>   DW_AT_GNU_locviews: (sec_offset) 0x183d
+ <4><362c>: Abbrev Number: 0
+ <3><362d>: Abbrev Number: 75 (DW_TAG_inlined_subroutine)
+    <362e>   DW_AT_abstract_origin: (ref4) <0x3f24>
+    <3632>   DW_AT_entry_pc    : (addr) 0x2cf6
+    <363a>   DW_AT_GNU_entry_view: (data1) 1
+    <363b>   DW_AT_ranges      : (sec_offset) 0x630
+    <363f>   DW_AT_call_file   : (data1) 1
+    <3640>   DW_AT_call_line   : (data1) 189
+    <3641>   DW_AT_call_column : (data1) 9
+    <3642>   DW_AT_sibling     : (ref4) <0x3661>
+ <4><3646>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <3647>   DW_AT_abstract_origin: (ref4) <0x3f32>
+    <364b>   DW_AT_location    : (sec_offset) 0x1890 (location list)
+    <364f>   DW_AT_GNU_locviews: (sec_offset) 0x188c
+ <4><3653>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
+    <3654>   DW_AT_low_pc      : (addr) 0x2d55
+    <365c>   DW_AT_abstract_origin: (ref4) <0x4415>
+ <4><3660>: Abbrev Number: 0
+ <3><3661>: Abbrev Number: 75 (DW_TAG_inlined_subroutine)
+    <3662>   DW_AT_abstract_origin: (ref4) <0x3f24>
+    <3666>   DW_AT_entry_pc    : (addr) 0x2cfc
+    <366e>   DW_AT_GNU_entry_view: (data1) 3
+    <366f>   DW_AT_ranges      : (sec_offset) 0x660
+    <3673>   DW_AT_call_file   : (data1) 1
+    <3674>   DW_AT_call_line   : (data1) 190
+    <3675>   DW_AT_call_column : (data1) 9
+    <3676>   DW_AT_sibling     : (ref4) <0x369c>
+ <4><367a>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <367b>   DW_AT_abstract_origin: (ref4) <0x3f32>
+    <367f>   DW_AT_location    : (sec_offset) 0x18ca (location list)
+    <3683>   DW_AT_GNU_locviews: (sec_offset) 0x18c6
+ <4><3687>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
+    <3688>   DW_AT_low_pc      : (addr) 0x2d3c
+    <3690>   DW_AT_abstract_origin: (ref4) <0x4415>
+ <5><3694>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3695>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3697>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <5><369a>: Abbrev Number: 0
+ <4><369b>: Abbrev Number: 0
+ <3><369c>: Abbrev Number: 77 (DW_TAG_inlined_subroutine)
+    <369d>   DW_AT_abstract_origin: (ref4) <0x3eaf>
+    <36a1>   DW_AT_entry_pc    : (addr) 0x2d18
+    <36a9>   DW_AT_GNU_entry_view: (data1) 3
+    <36aa>   DW_AT_low_pc      : (addr) 0x2d18
+    <36b2>   DW_AT_high_pc     : (data8) 0
+    <36ba>   DW_AT_call_file   : (data1) 1
+    <36bb>   DW_AT_call_line   : (data1) 175
+    <36bc>   DW_AT_call_column : (data1) 16
+    <36bd>   DW_AT_sibling     : (ref4) <0x36e9>
+ <4><36c1>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <36c2>   DW_AT_abstract_origin: (ref4) <0x3ec1>
+    <36c6>   DW_AT_location    : (sec_offset) 0x1904 (location list)
+    <36ca>   DW_AT_GNU_locviews: (sec_offset) 0x1900
+ <4><36ce>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <36cf>   DW_AT_abstract_origin: (ref4) <0x3ece>
+    <36d3>   DW_AT_location    : (sec_offset) 0x193e (location list)
+    <36d7>   DW_AT_GNU_locviews: (sec_offset) 0x193c
+ <4><36db>: Abbrev Number: 59 (DW_TAG_variable)
+    <36dc>   DW_AT_abstract_origin: (ref4) <0x3edb>
+    <36e0>   DW_AT_location    : (sec_offset) 0x1966 (location list)
+    <36e4>   DW_AT_GNU_locviews: (sec_offset) 0x1964
+ <4><36e8>: Abbrev Number: 0
+ <3><36e9>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
+    <36ea>   DW_AT_low_pc      : (addr) 0x2cef
+    <36f2>   DW_AT_abstract_origin: (ref4) <0x455b>
+ <4><36f6>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <36f7>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <36f9>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 73 0 	(DW_OP_breg3 (rbx): 0)
+ <4><36fc>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <36fd>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <36ff>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <4><3702>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3703>   DW_AT_location    : (exprloc) 1 byte block: 51 	(DW_OP_reg1 (rdx))
+    <3705>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7c 0 	(DW_OP_breg12 (r12): 0)
+ <4><3708>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3709>   DW_AT_location    : (exprloc) 1 byte block: 52 	(DW_OP_reg2 (rcx))
+    <370b>   DW_AT_GNU_call_site_value: (exprloc) 1 byte block: 30 	(DW_OP_lit0)
+ <4><370d>: Abbrev Number: 0
+ <3><370e>: Abbrev Number: 0
+ <2><370f>: Abbrev Number: 75 (DW_TAG_inlined_subroutine)
+    <3710>   DW_AT_abstract_origin: (ref4) <0x3f3f>
+    <3714>   DW_AT_entry_pc    : (addr) 0x2cac
+    <371c>   DW_AT_GNU_entry_view: (data1) 1
+    <371d>   DW_AT_ranges      : (sec_offset) 0x5b0
+    <3721>   DW_AT_call_file   : (data1) 1
+    <3722>   DW_AT_call_line   : (data1) 169
+    <3723>   DW_AT_call_column : (data1) 5
+    <3724>   DW_AT_sibling     : (ref4) <0x3736>
+ <3><3728>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <3729>   DW_AT_abstract_origin: (ref4) <0x3f4d>
+    <372d>   DW_AT_location    : (sec_offset) 0x1996 (location list)
+    <3731>   DW_AT_GNU_locviews: (sec_offset) 0x198e
+ <3><3735>: Abbrev Number: 0
+ <2><3736>: Abbrev Number: 78 (DW_TAG_inlined_subroutine)
+    <3737>   DW_AT_abstract_origin: (ref4) <0x3e1a>
+    <373b>   DW_AT_entry_pc    : (addr) 0x2cc4
+    <3743>   DW_AT_GNU_entry_view: (data1) 3
+    <3744>   DW_AT_low_pc      : (addr) 0x2cc4
+    <374c>   DW_AT_high_pc     : (data8) 0
+    <3754>   DW_AT_call_file   : (data1) 1
+    <3755>   DW_AT_call_line   : (data1) 172
+    <3756>   DW_AT_call_column : (data1) 22
+ <3><3757>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <3758>   DW_AT_abstract_origin: (ref4) <0x3e2b>
+    <375c>   DW_AT_location    : (sec_offset) 0x19f4 (location list)
+    <3760>   DW_AT_GNU_locviews: (sec_offset) 0x19f2
+ <3><3764>: Abbrev Number: 59 (DW_TAG_variable)
+    <3765>   DW_AT_abstract_origin: (ref4) <0x3e36>
+    <3769>   DW_AT_location    : (sec_offset) 0x1a1f (location list)
+    <376d>   DW_AT_GNU_locviews: (sec_offset) 0x1a17
+ <3><3771>: Abbrev Number: 78 (DW_TAG_inlined_subroutine)
+    <3772>   DW_AT_abstract_origin: (ref4) <0x3faf>
+    <3776>   DW_AT_entry_pc    : (addr) 0x2cc4
+    <377e>   DW_AT_GNU_entry_view: (data1) 6
+    <377f>   DW_AT_low_pc      : (addr) 0x2cc4
+    <3787>   DW_AT_high_pc     : (data8) 0
+    <378f>   DW_AT_call_file   : (data1) 4
+    <3790>   DW_AT_call_line   : (data1) 35
+    <3791>   DW_AT_call_column : (data1) 12
+ <4><3792>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <3793>   DW_AT_abstract_origin: (ref4) <0x3fc0>
+    <3797>   DW_AT_location    : (sec_offset) 0x1a80 (location list)
+    <379b>   DW_AT_GNU_locviews: (sec_offset) 0x1a7e
+ <4><379f>: Abbrev Number: 59 (DW_TAG_variable)
+    <37a0>   DW_AT_abstract_origin: (ref4) <0x3fcb>
+    <37a4>   DW_AT_location    : (sec_offset) 0x1aab (location list)
+    <37a8>   DW_AT_GNU_locviews: (sec_offset) 0x1aa3
+ <4><37ac>: Abbrev Number: 0
+ <3><37ad>: Abbrev Number: 0
+ <2><37ae>: Abbrev Number: 0
+ <1><37af>: Abbrev Number: 79 (DW_TAG_subprogram)
+    <37b0>   DW_AT_external    : (flag_present) 1
+    <37b0>   DW_AT_name        : (strp) (offset: 0x2ed): Cons_dealloc
+    <37b4>   DW_AT_decl_file   : (data1) 1
+    <37b5>   DW_AT_decl_line   : (data1) 156
+    <37b6>   DW_AT_decl_column : (data1) 1
+    <37b7>   DW_AT_prototyped  : (flag_present) 1
+    <37b7>   DW_AT_low_pc      : (addr) 0x2590
+    <37bf>   DW_AT_high_pc     : (data8) 0x98
+    <37c7>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
+    <37c9>   DW_AT_GNU_all_call_sites: (flag_present) 1
+    <37c9>   DW_AT_sibling     : (ref4) <0x38ca>
+ <2><37cd>: Abbrev Number: 65 (DW_TAG_formal_parameter)
+    <37ce>   DW_AT_name        : (strp) (offset: 0xf72): self
+    <37d2>   DW_AT_decl_file   : (data1) 1
+    <37d3>   DW_AT_decl_line   : (data1) 156
+    <37d4>   DW_AT_decl_column : (data1) 26
+    <37d5>   DW_AT_type        : (ref4) <0x38ca>, ConsObject
+    <37d9>   DW_AT_location    : (sec_offset) 0x1b1a (location list)
+    <37dd>   DW_AT_GNU_locviews: (sec_offset) 0x1b0a
+ <2><37e1>: Abbrev Number: 46 (DW_TAG_lexical_block)
+    <37e2>   DW_AT_ranges      : (sec_offset) 0x140
+    <37e6>   DW_AT_sibling     : (ref4) <0x38b5>
+ <3><37ea>: Abbrev Number: 73 (DW_TAG_variable)
+    <37eb>   DW_AT_name        : (strp) (offset: 0x416): _tstate
+    <37ef>   DW_AT_decl_file   : (data1) 1
+    <37f0>   DW_AT_decl_line   : (data1) 159
+    <37f1>   DW_AT_decl_column : (data1) 5
+    <37f2>   DW_AT_type        : (ref4) <0x1d29>, PyThreadState, _ts
+    <37f6>   DW_AT_location    : (sec_offset) 0x1bd5 (location list)
+    <37fa>   DW_AT_GNU_locviews: (sec_offset) 0x1bcb
+ <3><37fe>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <37ff>   DW_AT_low_pc      : (addr) 0x25ae
+    <3807>   DW_AT_abstract_origin: (ref4) <0x4567>
+    <380b>   DW_AT_sibling     : (ref4) <0x3823>
+ <4><380f>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3810>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3812>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <4><3815>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3816>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <3818>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 90 25 0 0 0 0 0 0 	(DW_OP_addr: 2590)
+ <4><3822>: Abbrev Number: 0
+ <3><3823>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <3824>   DW_AT_low_pc      : (addr) 0x25ba
+    <382c>   DW_AT_abstract_origin: (ref4) <0x38d0>
+    <3830>   DW_AT_sibling     : (ref4) <0x383b>
+ <4><3834>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3835>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3837>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <4><383a>: Abbrev Number: 0
+ <3><383b>: Abbrev Number: 80 (DW_TAG_GNU_call_site)
+    <383c>   DW_AT_low_pc      : (addr) 0x25d1
+    <3844>   DW_AT_GNU_tail_call: (flag_present) 1
+    <3844>   DW_AT_sibling     : (ref4) <0x3850>
+ <4><3848>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3849>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <384b>   DW_AT_GNU_call_site_value: (exprloc) 3 byte block: f3 1 55 	(DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)))
+ <4><384f>: Abbrev Number: 0
+ <3><3850>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
+    <3851>   DW_AT_low_pc      : (addr) 0x25dd
+    <3859>   DW_AT_abstract_origin: (ref4) <0x4574>
+ <3><385d>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <385e>   DW_AT_low_pc      : (addr) 0x25eb
+    <3866>   DW_AT_abstract_origin: (ref4) <0x4580>
+    <386a>   DW_AT_sibling     : (ref4) <0x387b>
+ <4><386e>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <386f>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3871>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7c 0 	(DW_OP_breg12 (r12): 0)
+ <4><3874>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3875>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <3877>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <4><387a>: Abbrev Number: 0
+ <3><387b>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <387c>   DW_AT_low_pc      : (addr) 0x25f7
+    <3884>   DW_AT_abstract_origin: (ref4) <0x38d0>
+    <3888>   DW_AT_sibling     : (ref4) <0x3893>
+ <4><388c>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <388d>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <388f>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <4><3892>: Abbrev Number: 0
+ <3><3893>: Abbrev Number: 81 (DW_TAG_GNU_call_site)
+    <3894>   DW_AT_low_pc      : (addr) 0x2604
+    <389c>   DW_AT_sibling     : (ref4) <0x38a7>
+ <4><38a0>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <38a1>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <38a3>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <4><38a6>: Abbrev Number: 0
+ <3><38a7>: Abbrev Number: 82 (DW_TAG_GNU_call_site)
+    <38a8>   DW_AT_low_pc      : (addr) 0x2618
+    <38b0>   DW_AT_GNU_tail_call: (flag_present) 1
+    <38b0>   DW_AT_abstract_origin: (ref4) <0x458d>
+ <3><38b4>: Abbrev Number: 0
+ <2><38b5>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
+    <38b6>   DW_AT_low_pc      : (addr) 0x259f
+    <38be>   DW_AT_abstract_origin: (ref4) <0x459a>
+ <3><38c2>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <38c3>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <38c5>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <3><38c8>: Abbrev Number: 0
+ <2><38c9>: Abbrev Number: 0
+ <1><38ca>: Abbrev Number: 10 (DW_TAG_pointer_type)
+    <38cb>   DW_AT_byte_size   : (data1) 8
+    <38cc>   DW_AT_type        : (ref4) <0x247a>, ConsObject
+ <1><38d0>: Abbrev Number: 64 (DW_TAG_subprogram)
+    <38d1>   DW_AT_external    : (flag_present) 1
+    <38d1>   DW_AT_name        : (strp) (offset: 0x1849): Cons_clear
+    <38d5>   DW_AT_decl_file   : (data1) 1
+    <38d6>   DW_AT_decl_line   : (data1) 148
+    <38d7>   DW_AT_decl_column : (data1) 1
+    <38d8>   DW_AT_prototyped  : (flag_present) 1
+    <38d8>   DW_AT_type        : (ref4) <0x4f>, int
+    <38dc>   DW_AT_low_pc      : (addr) 0x2530
+    <38e4>   DW_AT_high_pc     : (data8) 0x57
+    <38ec>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
+    <38ee>   DW_AT_GNU_all_call_sites: (flag_present) 1
+    <38ee>   DW_AT_sibling     : (ref4) <0x399f>
+ <2><38f2>: Abbrev Number: 65 (DW_TAG_formal_parameter)
+    <38f3>   DW_AT_name        : (strp) (offset: 0xf72): self
+    <38f7>   DW_AT_decl_file   : (data1) 1
+    <38f8>   DW_AT_decl_line   : (data1) 148
+    <38f9>   DW_AT_decl_column : (data1) 22
+    <38fa>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <38fe>   DW_AT_location    : (sec_offset) 0x1c51 (location list)
+    <3902>   DW_AT_GNU_locviews: (sec_offset) 0x1c45
+ <2><3906>: Abbrev Number: 46 (DW_TAG_lexical_block)
+    <3907>   DW_AT_ranges      : (sec_offset) 0x70
+    <390b>   DW_AT_sibling     : (ref4) <0x3954>
+ <3><390f>: Abbrev Number: 73 (DW_TAG_variable)
+    <3910>   DW_AT_name        : (strp) (offset: 0x19b9): _py_tmp
+    <3914>   DW_AT_decl_file   : (data1) 1
+    <3915>   DW_AT_decl_line   : (data1) 150
+    <3916>   DW_AT_decl_column : (data1) 5
+    <3917>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <391b>   DW_AT_location    : (sec_offset) 0x1cdd (location list)
+    <391f>   DW_AT_GNU_locviews: (sec_offset) 0x1cd9
+ <3><3923>: Abbrev Number: 83 (DW_TAG_inlined_subroutine)
+    <3924>   DW_AT_abstract_origin: (ref4) <0x3f24>
+    <3928>   DW_AT_entry_pc    : (addr) 0x2545
+    <3930>   DW_AT_GNU_entry_view: (data1) 1
+    <3931>   DW_AT_ranges      : (sec_offset) 0xb0
+    <3935>   DW_AT_call_file   : (data1) 1
+    <3936>   DW_AT_call_line   : (data1) 150
+    <3937>   DW_AT_call_column : (data1) 5
+ <4><3938>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <3939>   DW_AT_abstract_origin: (ref4) <0x3f32>
+    <393d>   DW_AT_location    : (sec_offset) 0x1d17 (location list)
+    <3941>   DW_AT_GNU_locviews: (sec_offset) 0x1d13
+ <4><3945>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
+    <3946>   DW_AT_low_pc      : (addr) 0x2585
+    <394e>   DW_AT_abstract_origin: (ref4) <0x4415>
+ <4><3952>: Abbrev Number: 0
+ <3><3953>: Abbrev Number: 0
+ <2><3954>: Abbrev Number: 58 (DW_TAG_lexical_block)
+    <3955>   DW_AT_ranges      : (sec_offset) 0xe0
+ <3><3959>: Abbrev Number: 73 (DW_TAG_variable)
+    <395a>   DW_AT_name        : (strp) (offset: 0x19b9): _py_tmp
+    <395e>   DW_AT_decl_file   : (data1) 1
+    <395f>   DW_AT_decl_line   : (data1) 151
+    <3960>   DW_AT_decl_column : (data1) 5
+    <3961>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <3965>   DW_AT_location    : (sec_offset) 0x1d4f (location list)
+    <3969>   DW_AT_GNU_locviews: (sec_offset) 0x1d4d
+ <3><396d>: Abbrev Number: 83 (DW_TAG_inlined_subroutine)
+    <396e>   DW_AT_abstract_origin: (ref4) <0x3f24>
+    <3972>   DW_AT_entry_pc    : (addr) 0x255c
+    <397a>   DW_AT_GNU_entry_view: (data1) 1
+    <397b>   DW_AT_ranges      : (sec_offset) 0x110
+    <397f>   DW_AT_call_file   : (data1) 1
+    <3980>   DW_AT_call_line   : (data1) 151
+    <3981>   DW_AT_call_column : (data1) 5
+ <4><3982>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <3983>   DW_AT_abstract_origin: (ref4) <0x3f32>
+    <3987>   DW_AT_location    : (sec_offset) 0x1d76 (location list)
+    <398b>   DW_AT_GNU_locviews: (sec_offset) 0x1d72
+ <4><398f>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
+    <3990>   DW_AT_low_pc      : (addr) 0x2575
+    <3998>   DW_AT_abstract_origin: (ref4) <0x4415>
+ <4><399c>: Abbrev Number: 0
+ <3><399d>: Abbrev Number: 0
+ <2><399e>: Abbrev Number: 0
+ <1><399f>: Abbrev Number: 84 (DW_TAG_subprogram)
+    <39a0>   DW_AT_name        : (strp) (offset: 0x1bf): Cons_traverse
+    <39a4>   DW_AT_decl_file   : (data1) 1
+    <39a5>   DW_AT_decl_line   : (data1) 139
+    <39a6>   DW_AT_decl_column : (data1) 1
+    <39a7>   DW_AT_prototyped  : (flag_present) 1
+    <39a7>   DW_AT_type        : (ref4) <0x4f>, int
+    <39ab>   DW_AT_inline      : (data1) 1	(inlined)
+    <39ac>   DW_AT_sibling     : (ref4) <0x3a2a>
+ <2><39b0>: Abbrev Number: 69 (DW_TAG_formal_parameter)
+    <39b1>   DW_AT_name        : (strp) (offset: 0xf72): self
+    <39b5>   DW_AT_decl_file   : (data1) 1
+    <39b6>   DW_AT_decl_line   : (data1) 139
+    <39b7>   DW_AT_decl_column : (data1) 27
+    <39b8>   DW_AT_type        : (ref4) <0x38ca>, ConsObject
+ <2><39bc>: Abbrev Number: 69 (DW_TAG_formal_parameter)
+    <39bd>   DW_AT_name        : (strp) (offset: 0xb21): visit
+    <39c1>   DW_AT_decl_file   : (data1) 1
+    <39c2>   DW_AT_decl_line   : (data1) 139
+    <39c3>   DW_AT_decl_column : (data1) 43
+    <39c4>   DW_AT_type        : (ref4) <0xd03>, visitproc, int
+ <2><39c8>: Abbrev Number: 85 (DW_TAG_formal_parameter)
+    <39c9>   DW_AT_name        : (string) arg
+    <39cd>   DW_AT_decl_file   : (data1) 1
+    <39ce>   DW_AT_decl_line   : (data1) 139
+    <39cf>   DW_AT_decl_column : (data1) 56
+    <39d0>   DW_AT_type        : (ref4) <0x88>
+ <2><39d4>: Abbrev Number: 86 (DW_TAG_lexical_block)
+    <39d5>   DW_AT_sibling     : (ref4) <0x39f9>
+ <3><39d9>: Abbrev Number: 70 (DW_TAG_variable)
+    <39da>   DW_AT_name        : (strp) (offset: 0xb88): vret
+    <39de>   DW_AT_decl_file   : (data1) 1
+    <39df>   DW_AT_decl_line   : (data1) 141
+    <39e0>   DW_AT_decl_column : (data1) 5
+    <39e1>   DW_AT_type        : (ref4) <0x4f>, int
+ <3><39e5>: Abbrev Number: 53 (DW_TAG_GNU_call_site)
+    <39e6>   DW_AT_low_pc      : (addr) 0x2b5b
+    <39ee>   DW_AT_GNU_call_site_target: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <4><39f1>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <39f2>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <39f4>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7c 0 	(DW_OP_breg12 (r12): 0)
+ <4><39f7>: Abbrev Number: 0
+ <3><39f8>: Abbrev Number: 0
+ <2><39f9>: Abbrev Number: 86 (DW_TAG_lexical_block)
+    <39fa>   DW_AT_sibling     : (ref4) <0x3a1b>
+ <3><39fe>: Abbrev Number: 70 (DW_TAG_variable)
+    <39ff>   DW_AT_name        : (strp) (offset: 0xb88): vret
+    <3a03>   DW_AT_decl_file   : (data1) 1
+    <3a04>   DW_AT_decl_line   : (data1) 142
+    <3a05>   DW_AT_decl_column : (data1) 5
+    <3a06>   DW_AT_type        : (ref4) <0x4f>, int
+ <3><3a0a>: Abbrev Number: 54 (DW_TAG_GNU_call_site)
+    <3a0b>   DW_AT_low_pc      : (addr) 0x2b6d
+ <4><3a13>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3a14>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <3a16>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7c 0 	(DW_OP_breg12 (r12): 0)
+ <4><3a19>: Abbrev Number: 0
+ <3><3a1a>: Abbrev Number: 0
+ <2><3a1b>: Abbrev Number: 71 (DW_TAG_lexical_block)
+ <3><3a1c>: Abbrev Number: 70 (DW_TAG_variable)
+    <3a1d>   DW_AT_name        : (strp) (offset: 0xb88): vret
+    <3a21>   DW_AT_decl_file   : (data1) 1
+    <3a22>   DW_AT_decl_line   : (data1) 143
+    <3a23>   DW_AT_decl_column : (data1) 5
+    <3a24>   DW_AT_type        : (ref4) <0x4f>, int
+ <3><3a28>: Abbrev Number: 0
+ <2><3a29>: Abbrev Number: 0
+ <1><3a2a>: Abbrev Number: 64 (DW_TAG_subprogram)
+    <3a2b>   DW_AT_external    : (flag_present) 1
+    <3a2b>   DW_AT_name        : (strp) (offset: 0x464): Cons_new
+    <3a2f>   DW_AT_decl_file   : (data1) 1
+    <3a30>   DW_AT_decl_line   : (data1) 105
+    <3a31>   DW_AT_decl_column : (data1) 1
+    <3a32>   DW_AT_prototyped  : (flag_present) 1
+    <3a32>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <3a36>   DW_AT_low_pc      : (addr) 0x2400
+    <3a3e>   DW_AT_high_pc     : (data8) 0x127
+    <3a46>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
+    <3a48>   DW_AT_GNU_all_call_sites: (flag_present) 1
+    <3a48>   DW_AT_sibling     : (ref4) <0x3c6a>
+ <2><3a4c>: Abbrev Number: 65 (DW_TAG_formal_parameter)
+    <3a4d>   DW_AT_name        : (strp) (offset: 0x2201): type
+    <3a51>   DW_AT_decl_file   : (data1) 1
+    <3a52>   DW_AT_decl_line   : (data1) 105
+    <3a53>   DW_AT_decl_column : (data1) 24
+    <3a54>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
+    <3a58>   DW_AT_location    : (sec_offset) 0x1db4 (location list)
+    <3a5c>   DW_AT_GNU_locviews: (sec_offset) 0x1dac
+ <2><3a60>: Abbrev Number: 65 (DW_TAG_formal_parameter)
+    <3a61>   DW_AT_name        : (strp) (offset: 0x543): args
+    <3a65>   DW_AT_decl_file   : (data1) 1
+    <3a66>   DW_AT_decl_line   : (data1) 105
+    <3a67>   DW_AT_decl_column : (data1) 40
+    <3a68>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <3a6c>   DW_AT_location    : (sec_offset) 0x1e1b (location list)
+    <3a70>   DW_AT_GNU_locviews: (sec_offset) 0x1e13
+ <2><3a74>: Abbrev Number: 65 (DW_TAG_formal_parameter)
+    <3a75>   DW_AT_name        : (strp) (offset: 0x2040): kwds
+    <3a79>   DW_AT_decl_file   : (data1) 1
+    <3a7a>   DW_AT_decl_line   : (data1) 105
+    <3a7b>   DW_AT_decl_column : (data1) 56
+    <3a7c>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <3a80>   DW_AT_location    : (sec_offset) 0x1e82 (location list)
+    <3a84>   DW_AT_GNU_locviews: (sec_offset) 0x1e7a
+ <2><3a88>: Abbrev Number: 73 (DW_TAG_variable)
+    <3a89>   DW_AT_name        : (strp) (offset: 0xf72): self
+    <3a8d>   DW_AT_decl_file   : (data1) 1
+    <3a8e>   DW_AT_decl_line   : (data1) 107
+    <3a8f>   DW_AT_decl_column : (data1) 17
+    <3a90>   DW_AT_type        : (ref4) <0x38ca>, ConsObject
+    <3a94>   DW_AT_location    : (sec_offset) 0x1ee9 (location list)
+    <3a98>   DW_AT_GNU_locviews: (sec_offset) 0x1ee1
+ <2><3a9c>: Abbrev Number: 38 (DW_TAG_variable)
+    <3a9d>   DW_AT_name        : (strp) (offset: 0xc3d): kwlist
+    <3aa1>   DW_AT_decl_file   : (data1) 1
+    <3aa2>   DW_AT_decl_line   : (data1) 112
+    <3aa3>   DW_AT_decl_column : (data1) 18
+    <3aa4>   DW_AT_type        : (ref4) <0x3c6a>, char
+    <3aa8>   DW_AT_location    : (exprloc) 9 byte block: 3 20 50 0 0 0 0 0 0 	(DW_OP_addr: 5020)
+ <2><3ab2>: Abbrev Number: 38 (DW_TAG_variable)
+    <3ab3>   DW_AT_name        : (strp) (offset: 0x652): head
+    <3ab7>   DW_AT_decl_file   : (data1) 1
+    <3ab8>   DW_AT_decl_line   : (data1) 113
+    <3ab9>   DW_AT_decl_column : (data1) 15
+    <3aba>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <3abe>   DW_AT_location    : (exprloc) 3 byte block: 91 b8 7f 	(DW_OP_fbreg: -72)
+ <2><3ac2>: Abbrev Number: 38 (DW_TAG_variable)
+    <3ac3>   DW_AT_name        : (strp) (offset: 0x203b): tail
+    <3ac7>   DW_AT_decl_file   : (data1) 1
+    <3ac8>   DW_AT_decl_line   : (data1) 113
+    <3ac9>   DW_AT_decl_column : (data1) 29
+    <3aca>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <3ace>   DW_AT_location    : (exprloc) 2 byte block: 91 40 	(DW_OP_fbreg: -64)
+ <2><3ad1>: Abbrev Number: 73 (DW_TAG_variable)
+    <3ad2>   DW_AT_name        : (strp) (offset: 0x58c): state
+    <3ad6>   DW_AT_decl_file   : (data1) 1
+    <3ad7>   DW_AT_decl_line   : (data1) 119
+    <3ad8>   DW_AT_decl_column : (data1) 23
+    <3ad9>   DW_AT_type        : (ref4) <0x274d>, consmodule_state
+    <3add>   DW_AT_location    : (sec_offset) 0x1f49 (location list)
+    <3ae1>   DW_AT_GNU_locviews: (sec_offset) 0x1f45
+ <2><3ae5>: Abbrev Number: 73 (DW_TAG_variable)
+    <3ae6>   DW_AT_name        : (strp) (offset: 0x2327): cons
+    <3aea>   DW_AT_decl_file   : (data1) 1
+    <3aeb>   DW_AT_decl_line   : (data1) 122
+    <3aec>   DW_AT_decl_column : (data1) 19
+    <3aed>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
+    <3af1>   DW_AT_location    : (sec_offset) 0x1f83 (location list)
+    <3af5>   DW_AT_GNU_locviews: (sec_offset) 0x1f7f
+ <2><3af9>: Abbrev Number: 77 (DW_TAG_inlined_subroutine)
+    <3afa>   DW_AT_abstract_origin: (ref4) <0x3f86>
+    <3afe>   DW_AT_entry_pc    : (addr) 0x248b
+    <3b06>   DW_AT_GNU_entry_view: (data1) 1
+    <3b07>   DW_AT_low_pc      : (addr) 0x248b
+    <3b0f>   DW_AT_high_pc     : (data8) 0
+    <3b17>   DW_AT_call_file   : (data1) 1
+    <3b18>   DW_AT_call_line   : (data1) 126
+    <3b19>   DW_AT_call_column : (data1) 14
+    <3b1a>   DW_AT_sibling     : (ref4) <0x3b39>
+ <3><3b1e>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <3b1f>   DW_AT_abstract_origin: (ref4) <0x3fa2>
+    <3b23>   DW_AT_location    : (sec_offset) 0x1fbd (location list)
+    <3b27>   DW_AT_GNU_locviews: (sec_offset) 0x1fbb
+ <3><3b2b>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <3b2c>   DW_AT_abstract_origin: (ref4) <0x3f97>
+    <3b30>   DW_AT_location    : (sec_offset) 0x1fe3 (location list)
+    <3b34>   DW_AT_GNU_locviews: (sec_offset) 0x1fe1
+ <3><3b38>: Abbrev Number: 0
+ <2><3b39>: Abbrev Number: 77 (DW_TAG_inlined_subroutine)
+    <3b3a>   DW_AT_abstract_origin: (ref4) <0x3f3f>
+    <3b3e>   DW_AT_entry_pc    : (addr) 0x24a3
+    <3b46>   DW_AT_GNU_entry_view: (data1) 0
+    <3b47>   DW_AT_low_pc      : (addr) 0x24a3
+    <3b4f>   DW_AT_high_pc     : (data8) 0x4
+    <3b57>   DW_AT_call_file   : (data1) 1
+    <3b58>   DW_AT_call_line   : (data1) 131
+    <3b59>   DW_AT_call_column : (data1) 5
+    <3b5a>   DW_AT_sibling     : (ref4) <0x3b6c>
+ <3><3b5e>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <3b5f>   DW_AT_abstract_origin: (ref4) <0x3f4d>
+    <3b63>   DW_AT_location    : (sec_offset) 0x200a (location list)
+    <3b67>   DW_AT_GNU_locviews: (sec_offset) 0x2006
+ <3><3b6b>: Abbrev Number: 0
+ <2><3b6c>: Abbrev Number: 77 (DW_TAG_inlined_subroutine)
+    <3b6d>   DW_AT_abstract_origin: (ref4) <0x3f3f>
+    <3b71>   DW_AT_entry_pc    : (addr) 0x24ac
+    <3b79>   DW_AT_GNU_entry_view: (data1) 1
+    <3b7a>   DW_AT_low_pc      : (addr) 0x24ac
+    <3b82>   DW_AT_high_pc     : (data8) 0x4
+    <3b8a>   DW_AT_call_file   : (data1) 1
+    <3b8b>   DW_AT_call_line   : (data1) 133
+    <3b8c>   DW_AT_call_column : (data1) 5
+    <3b8d>   DW_AT_sibling     : (ref4) <0x3b9f>
+ <3><3b91>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <3b92>   DW_AT_abstract_origin: (ref4) <0x3f4d>
+    <3b96>   DW_AT_location    : (sec_offset) 0x2042 (location list)
+    <3b9a>   DW_AT_GNU_locviews: (sec_offset) 0x2040
+ <3><3b9e>: Abbrev Number: 0
+ <2><3b9f>: Abbrev Number: 77 (DW_TAG_inlined_subroutine)
+    <3ba0>   DW_AT_abstract_origin: (ref4) <0x3f24>
+    <3ba4>   DW_AT_entry_pc    : (addr) 0x24d8
+    <3bac>   DW_AT_GNU_entry_view: (data1) 2
+    <3bad>   DW_AT_low_pc      : (addr) 0x24d8
+    <3bb5>   DW_AT_high_pc     : (data8) 0x18
+    <3bbd>   DW_AT_call_file   : (data1) 1
+    <3bbe>   DW_AT_call_line   : (data1) 115
+    <3bbf>   DW_AT_call_column : (data1) 9
+    <3bc0>   DW_AT_sibling     : (ref4) <0x3be6>
+ <3><3bc4>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <3bc5>   DW_AT_abstract_origin: (ref4) <0x3f32>
+    <3bc9>   DW_AT_location    : (sec_offset) 0x2067 (location list)
+    <3bcd>   DW_AT_GNU_locviews: (sec_offset) 0x2065
+ <3><3bd1>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
+    <3bd2>   DW_AT_low_pc      : (addr) 0x24e7
+    <3bda>   DW_AT_abstract_origin: (ref4) <0x4415>
+ <4><3bde>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3bdf>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3be1>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7c 0 	(DW_OP_breg12 (r12): 0)
+ <4><3be4>: Abbrev Number: 0
+ <3><3be5>: Abbrev Number: 0
+ <2><3be6>: Abbrev Number: 81 (DW_TAG_GNU_call_site)
+    <3be7>   DW_AT_low_pc      : (addr) 0x242c
+    <3bef>   DW_AT_sibling     : (ref4) <0x3bff>
+ <3><3bf3>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3bf4>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3bf6>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <3><3bf9>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3bfa>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <3bfc>   DW_AT_GNU_call_site_value: (exprloc) 1 byte block: 30 	(DW_OP_lit0)
+ <3><3bfe>: Abbrev Number: 0
+ <2><3bff>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <3c00>   DW_AT_low_pc      : (addr) 0x246f
+    <3c08>   DW_AT_abstract_origin: (ref4) <0x45a6>
+    <3c0c>   DW_AT_sibling     : (ref4) <0x3c44>
+ <3><3c10>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3c11>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3c13>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7d 0 	(DW_OP_breg13 (r13): 0)
+ <3><3c16>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3c17>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <3c19>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7e 0 	(DW_OP_breg14 (r14): 0)
+ <3><3c1c>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3c1d>   DW_AT_location    : (exprloc) 1 byte block: 51 	(DW_OP_reg1 (rdx))
+    <3c1f>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 6 30 0 0 0 0 0 0 	(DW_OP_addr: 3006)
+ <3><3c29>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3c2a>   DW_AT_location    : (exprloc) 1 byte block: 52 	(DW_OP_reg2 (rcx))
+    <3c2c>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 20 50 0 0 0 0 0 0 	(DW_OP_addr: 5020)
+ <3><3c36>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3c37>   DW_AT_location    : (exprloc) 1 byte block: 58 	(DW_OP_reg8 (r8))
+    <3c39>   DW_AT_GNU_call_site_value: (exprloc) 3 byte block: 91 b8 7f 	(DW_OP_fbreg: -72)
+ <3><3c3d>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3c3e>   DW_AT_location    : (exprloc) 1 byte block: 59 	(DW_OP_reg9 (r9))
+    <3c40>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 91 40 	(DW_OP_fbreg: -64)
+ <3><3c43>: Abbrev Number: 0
+ <2><3c44>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <3c45>   DW_AT_low_pc      : (addr) 0x247b
+    <3c4d>   DW_AT_abstract_origin: (ref4) <0x4477>
+    <3c51>   DW_AT_sibling     : (ref4) <0x3c5c>
+ <3><3c55>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3c56>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3c58>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <3><3c5b>: Abbrev Number: 0
+ <2><3c5c>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
+    <3c5d>   DW_AT_low_pc      : (addr) 0x2527
+    <3c65>   DW_AT_abstract_origin: (ref4) <0x451f>
+ <2><3c69>: Abbrev Number: 0
+ <1><3c6a>: Abbrev Number: 12 (DW_TAG_array_type)
+    <3c6b>   DW_AT_type        : (ref4) <0xea>, char
+    <3c6f>   DW_AT_sibling     : (ref4) <0x3c7a>
+ <2><3c73>: Abbrev Number: 13 (DW_TAG_subrange_type)
+    <3c74>   DW_AT_type        : (ref4) <0x62>, long unsigned int
+    <3c78>   DW_AT_upper_bound : (data1) 2
+ <2><3c79>: Abbrev Number: 0
+ <1><3c7a>: Abbrev Number: 87 (DW_TAG_subprogram)
+    <3c7b>   DW_AT_name        : (strp) (offset: 0x1ab9): Nil_bool
+    <3c7f>   DW_AT_decl_file   : (data1) 1
+    <3c80>   DW_AT_decl_line   : (data1) 77
+    <3c81>   DW_AT_decl_column : (data1) 1
+    <3c82>   DW_AT_prototyped  : (flag_present) 1
+    <3c82>   DW_AT_type        : (ref4) <0x4f>, int
+    <3c86>   DW_AT_low_pc      : (addr) 0x23e0
+    <3c8e>   DW_AT_high_pc     : (data8) 0x3
+    <3c96>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
+    <3c98>   DW_AT_GNU_all_call_sites: (flag_present) 1
+    <3c98>   DW_AT_sibling     : (ref4) <0x3cab>
+ <2><3c9c>: Abbrev Number: 88 (DW_TAG_formal_parameter)
+    <3c9d>   DW_AT_name        : (strp) (offset: 0xf72): self
+    <3ca1>   DW_AT_decl_file   : (data1) 1
+    <3ca2>   DW_AT_decl_line   : (data1) 77
+    <3ca3>   DW_AT_decl_column : (data1) 20
+    <3ca4>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <3ca8>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+ <2><3caa>: Abbrev Number: 0
+ <1><3cab>: Abbrev Number: 84 (DW_TAG_subprogram)
+    <3cac>   DW_AT_name        : (strp) (offset: 0xe7c): Nil_new
+    <3cb0>   DW_AT_decl_file   : (data1) 1
+    <3cb1>   DW_AT_decl_line   : (data1) 61
+    <3cb2>   DW_AT_decl_column : (data1) 1
+    <3cb3>   DW_AT_prototyped  : (flag_present) 1
+    <3cb3>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <3cb7>   DW_AT_inline      : (data1) 1	(inlined)
+    <3cb8>   DW_AT_sibling     : (ref4) <0x3cf9>
+ <2><3cbc>: Abbrev Number: 69 (DW_TAG_formal_parameter)
+    <3cbd>   DW_AT_name        : (strp) (offset: 0x2201): type
+    <3cc1>   DW_AT_decl_file   : (data1) 1
+    <3cc2>   DW_AT_decl_line   : (data1) 61
+    <3cc3>   DW_AT_decl_column : (data1) 23
+    <3cc4>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
+ <2><3cc8>: Abbrev Number: 69 (DW_TAG_formal_parameter)
+    <3cc9>   DW_AT_name        : (strp) (offset: 0x543): args
+    <3ccd>   DW_AT_decl_file   : (data1) 1
+    <3cce>   DW_AT_decl_line   : (data1) 61
+    <3ccf>   DW_AT_decl_column : (data1) 39
+    <3cd0>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3cd4>: Abbrev Number: 69 (DW_TAG_formal_parameter)
+    <3cd5>   DW_AT_name        : (strp) (offset: 0x2040): kwds
+    <3cd9>   DW_AT_decl_file   : (data1) 1
+    <3cda>   DW_AT_decl_line   : (data1) 61
+    <3cdb>   DW_AT_decl_column : (data1) 55
+    <3cdc>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3ce0>: Abbrev Number: 70 (DW_TAG_variable)
+    <3ce1>   DW_AT_name        : (strp) (offset: 0x58c): state
+    <3ce5>   DW_AT_decl_file   : (data1) 1
+    <3ce6>   DW_AT_decl_line   : (data1) 68
+    <3ce7>   DW_AT_decl_column : (data1) 23
+    <3ce8>   DW_AT_type        : (ref4) <0x274d>, consmodule_state
+ <2><3cec>: Abbrev Number: 70 (DW_TAG_variable)
+    <3ced>   DW_AT_name        : (strp) (offset: 0xf72): self
+    <3cf1>   DW_AT_decl_file   : (data1) 1
+    <3cf2>   DW_AT_decl_line   : (data1) 71
+    <3cf3>   DW_AT_decl_column : (data1) 15
+    <3cf4>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3cf8>: Abbrev Number: 0
+ <1><3cf9>: Abbrev Number: 64 (DW_TAG_subprogram)
+    <3cfa>   DW_AT_external    : (flag_present) 1
+    <3cfa>   DW_AT_name        : (strp) (offset: 0x1e94): Nil_repr
+    <3cfe>   DW_AT_decl_file   : (data1) 1
+    <3cff>   DW_AT_decl_line   : (data1) 55
+    <3d00>   DW_AT_decl_column : (data1) 1
+    <3d01>   DW_AT_prototyped  : (flag_present) 1
+    <3d01>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <3d05>   DW_AT_low_pc      : (addr) 0x23f0
+    <3d0d>   DW_AT_high_pc     : (data8) 0xc
+    <3d15>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
+    <3d17>   DW_AT_GNU_all_call_sites: (flag_present) 1
+    <3d17>   DW_AT_sibling     : (ref4) <0x3d4b>
+ <2><3d1b>: Abbrev Number: 65 (DW_TAG_formal_parameter)
+    <3d1c>   DW_AT_name        : (strp) (offset: 0xf72): self
+    <3d20>   DW_AT_decl_file   : (data1) 1
+    <3d21>   DW_AT_decl_line   : (data1) 55
+    <3d22>   DW_AT_decl_column : (data1) 20
+    <3d23>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <3d27>   DW_AT_location    : (sec_offset) 0x208e (location list)
+    <3d2b>   DW_AT_GNU_locviews: (sec_offset) 0x208a
+ <2><3d2f>: Abbrev Number: 41 (DW_TAG_GNU_call_site)
+    <3d30>   DW_AT_low_pc      : (addr) 0x23fc
+    <3d38>   DW_AT_GNU_tail_call: (flag_present) 1
+    <3d38>   DW_AT_abstract_origin: (ref4) <0x4452>
+ <3><3d3c>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3d3d>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <3d3f>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 0 30 0 0 0 0 0 0 	(DW_OP_addr: 3000)
+ <3><3d49>: Abbrev Number: 0
+ <2><3d4a>: Abbrev Number: 0
+ <1><3d4b>: Abbrev Number: 87 (DW_TAG_subprogram)
+    <3d4c>   DW_AT_name        : (strp) (offset: 0x1287): Nil_traverse
+    <3d50>   DW_AT_decl_file   : (data1) 1
+    <3d51>   DW_AT_decl_line   : (data1) 48
+    <3d52>   DW_AT_decl_column : (data1) 1
+    <3d53>   DW_AT_prototyped  : (flag_present) 1
+    <3d53>   DW_AT_type        : (ref4) <0x4f>, int
+    <3d57>   DW_AT_low_pc      : (addr) 0x23c0
+    <3d5f>   DW_AT_high_pc     : (data8) 0x1b
+    <3d67>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
+    <3d69>   DW_AT_GNU_all_call_sites: (flag_present) 1
+    <3d69>   DW_AT_sibling     : (ref4) <0x3dd1>
+ <2><3d6d>: Abbrev Number: 65 (DW_TAG_formal_parameter)
+    <3d6e>   DW_AT_name        : (strp) (offset: 0xf72): self
+    <3d72>   DW_AT_decl_file   : (data1) 1
+    <3d73>   DW_AT_decl_line   : (data1) 48
+    <3d74>   DW_AT_decl_column : (data1) 25
+    <3d75>   DW_AT_type        : (ref4) <0x3dd1>, NilObject
+    <3d79>   DW_AT_location    : (sec_offset) 0x20cb (location list)
+    <3d7d>   DW_AT_GNU_locviews: (sec_offset) 0x20c7
+ <2><3d81>: Abbrev Number: 65 (DW_TAG_formal_parameter)
+    <3d82>   DW_AT_name        : (strp) (offset: 0xb21): visit
+    <3d86>   DW_AT_decl_file   : (data1) 1
+    <3d87>   DW_AT_decl_line   : (data1) 48
+    <3d88>   DW_AT_decl_column : (data1) 41
+    <3d89>   DW_AT_type        : (ref4) <0xd03>, visitproc, int
+    <3d8d>   DW_AT_location    : (sec_offset) 0x210e (location list)
+    <3d91>   DW_AT_GNU_locviews: (sec_offset) 0x2104
+ <2><3d95>: Abbrev Number: 76 (DW_TAG_formal_parameter)
+    <3d96>   DW_AT_name        : (string) arg
+    <3d9a>   DW_AT_decl_file   : (data1) 1
+    <3d9b>   DW_AT_decl_line   : (data1) 48
+    <3d9c>   DW_AT_decl_column : (data1) 54
+    <3d9d>   DW_AT_type        : (ref4) <0x88>
+    <3da1>   DW_AT_location    : (sec_offset) 0x2189 (location list)
+    <3da5>   DW_AT_GNU_locviews: (sec_offset) 0x2183
+ <2><3da9>: Abbrev Number: 58 (DW_TAG_lexical_block)
+    <3daa>   DW_AT_ranges      : (sec_offset) 0x40
+ <3><3dae>: Abbrev Number: 70 (DW_TAG_variable)
+    <3daf>   DW_AT_name        : (strp) (offset: 0xb88): vret
+    <3db3>   DW_AT_decl_file   : (data1) 1
+    <3db4>   DW_AT_decl_line   : (data1) 50
+    <3db5>   DW_AT_decl_column : (data1) 5
+    <3db6>   DW_AT_type        : (ref4) <0x4f>, int
+ <3><3dba>: Abbrev Number: 55 (DW_TAG_GNU_call_site)
+    <3dbb>   DW_AT_low_pc      : (addr) 0x23d1
+    <3dc3>   DW_AT_GNU_tail_call: (flag_present) 1
+    <3dc3>   DW_AT_GNU_call_site_target: (exprloc) 3 byte block: f3 1 54 	(DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)))
+ <4><3dc7>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <3dc8>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <3dca>   DW_AT_GNU_call_site_value: (exprloc) 3 byte block: f3 1 51 	(DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)))
+ <4><3dce>: Abbrev Number: 0
+ <3><3dcf>: Abbrev Number: 0
+ <2><3dd0>: Abbrev Number: 0
+ <1><3dd1>: Abbrev Number: 10 (DW_TAG_pointer_type)
+    <3dd2>   DW_AT_byte_size   : (data1) 8
+    <3dd3>   DW_AT_type        : (ref4) <0x23c9>, NilObject
+ <1><3dd7>: Abbrev Number: 89 (DW_TAG_subprogram)
+    <3dd8>   DW_AT_name        : (strp) (offset: 0x2259): PyList_SET_ITEM
+    <3ddc>   DW_AT_decl_file   : (data1) 4
+    <3ddd>   DW_AT_decl_line   : (data1) 44
+    <3dde>   DW_AT_decl_column : (data1) 1
+    <3ddf>   DW_AT_prototyped  : (flag_present) 1
     <3ddf>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
-    <3de0>   DW_AT_sibling     : (ref4) <0x3e0c>
- <2><3de4>: Abbrev Number: 90 (DW_TAG_formal_parameter)
-    <3de5>   DW_AT_name        : (strp) (offset: 0x2201): type
-    <3de9>   DW_AT_decl_file   : (data1) 2
-    <3dea>   DW_AT_decl_line   : (data2) 763
-    <3dec>   DW_AT_decl_column : (data1) 33
-    <3ded>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
- <2><3df1>: Abbrev Number: 90 (DW_TAG_formal_parameter)
-    <3df2>   DW_AT_name        : (strp) (offset: 0x98d): feature
-    <3df6>   DW_AT_decl_file   : (data1) 2
-    <3df7>   DW_AT_decl_line   : (data2) 763
-    <3df9>   DW_AT_decl_column : (data1) 53
-    <3dfa>   DW_AT_type        : (ref4) <0x62>, long unsigned int
- <2><3dfe>: Abbrev Number: 91 (DW_TAG_variable)
-    <3dff>   DW_AT_name        : (strp) (offset: 0x1226): flags
-    <3e03>   DW_AT_decl_file   : (data1) 2
-    <3e04>   DW_AT_decl_line   : (data2) 765
-    <3e06>   DW_AT_decl_column : (data1) 19
-    <3e07>   DW_AT_type        : (ref4) <0x62>, long unsigned int
- <2><3e0b>: Abbrev Number: 0
- <1><3e0c>: Abbrev Number: 89 (DW_TAG_subprogram)
-    <3e0d>   DW_AT_name        : (strp) (offset: 0x1658): _Py_NewRef
-    <3e11>   DW_AT_decl_file   : (data1) 2
-    <3e12>   DW_AT_decl_line   : (data2) 616
-    <3e14>   DW_AT_decl_column : (data1) 25
-    <3e15>   DW_AT_prototyped  : (flag_present) 1
-    <3e15>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
-    <3e19>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
-    <3e1a>   DW_AT_sibling     : (ref4) <0x3e2c>
- <2><3e1e>: Abbrev Number: 92 (DW_TAG_formal_parameter)
-    <3e1f>   DW_AT_name        : (string) obj
-    <3e23>   DW_AT_decl_file   : (data1) 2
-    <3e24>   DW_AT_decl_line   : (data2) 616
-    <3e26>   DW_AT_decl_column : (data1) 46
-    <3e27>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><3e2b>: Abbrev Number: 0
- <1><3e2c>: Abbrev Number: 93 (DW_TAG_subprogram)
-    <3e2d>   DW_AT_name        : (strp) (offset: 0x5d): Py_XDECREF
-    <3e31>   DW_AT_decl_file   : (data1) 2
-    <3e32>   DW_AT_decl_line   : (data2) 599
-    <3e34>   DW_AT_decl_column : (data1) 20
-    <3e35>   DW_AT_prototyped  : (flag_present) 1
-    <3e35>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
-    <3e36>   DW_AT_sibling     : (ref4) <0x3e47>
- <2><3e3a>: Abbrev Number: 92 (DW_TAG_formal_parameter)
-    <3e3b>   DW_AT_name        : (string) op
-    <3e3e>   DW_AT_decl_file   : (data1) 2
-    <3e3f>   DW_AT_decl_line   : (data2) 599
-    <3e41>   DW_AT_decl_column : (data1) 41
-    <3e42>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><3e46>: Abbrev Number: 0
- <1><3e47>: Abbrev Number: 93 (DW_TAG_subprogram)
-    <3e48>   DW_AT_name        : (strp) (offset: 0xa64): Py_DECREF
-    <3e4c>   DW_AT_decl_file   : (data1) 2
-    <3e4d>   DW_AT_decl_line   : (data2) 533
-    <3e4f>   DW_AT_decl_column : (data1) 20
-    <3e50>   DW_AT_prototyped  : (flag_present) 1
-    <3e50>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
-    <3e51>   DW_AT_sibling     : (ref4) <0x3e62>
- <2><3e55>: Abbrev Number: 92 (DW_TAG_formal_parameter)
-    <3e56>   DW_AT_name        : (string) op
-    <3e59>   DW_AT_decl_file   : (data1) 2
-    <3e5a>   DW_AT_decl_line   : (data2) 533
-    <3e5c>   DW_AT_decl_column : (data1) 40
-    <3e5d>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><3e61>: Abbrev Number: 0
- <1><3e62>: Abbrev Number: 93 (DW_TAG_subprogram)
-    <3e63>   DW_AT_name        : (strp) (offset: 0x1419): Py_INCREF
-    <3e67>   DW_AT_decl_file   : (data1) 2
-    <3e68>   DW_AT_decl_line   : (data2) 491
-    <3e6a>   DW_AT_decl_column : (data1) 20
-    <3e6b>   DW_AT_prototyped  : (flag_present) 1
-    <3e6b>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
-    <3e6c>   DW_AT_sibling     : (ref4) <0x3e7d>
- <2><3e70>: Abbrev Number: 92 (DW_TAG_formal_parameter)
-    <3e71>   DW_AT_name        : (string) op
-    <3e74>   DW_AT_decl_file   : (data1) 2
-    <3e75>   DW_AT_decl_line   : (data2) 491
-    <3e77>   DW_AT_decl_column : (data1) 40
-    <3e78>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><3e7c>: Abbrev Number: 0
- <1><3e7d>: Abbrev Number: 89 (DW_TAG_subprogram)
-    <3e7e>   DW_AT_name        : (strp) (offset: 0x1e58): PyObject_TypeCheck
-    <3e82>   DW_AT_decl_file   : (data1) 2
-    <3e83>   DW_AT_decl_line   : (data2) 262
-    <3e85>   DW_AT_decl_column : (data1) 19
-    <3e86>   DW_AT_prototyped  : (flag_present) 1
-    <3e86>   DW_AT_type        : (ref4) <0x4f>, int
-    <3e8a>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
-    <3e8b>   DW_AT_sibling     : (ref4) <0x3ea9>
- <2><3e8f>: Abbrev Number: 92 (DW_TAG_formal_parameter)
-    <3e90>   DW_AT_name        : (string) ob
-    <3e93>   DW_AT_decl_file   : (data1) 2
-    <3e94>   DW_AT_decl_line   : (data2) 262
-    <3e96>   DW_AT_decl_column : (data1) 48
-    <3e97>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><3e9b>: Abbrev Number: 90 (DW_TAG_formal_parameter)
-    <3e9c>   DW_AT_name        : (strp) (offset: 0x2201): type
-    <3ea0>   DW_AT_decl_file   : (data1) 2
-    <3ea1>   DW_AT_decl_line   : (data2) 262
-    <3ea3>   DW_AT_decl_column : (data1) 66
-    <3ea4>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
- <2><3ea8>: Abbrev Number: 0
- <1><3ea9>: Abbrev Number: 83 (DW_TAG_subprogram)
-    <3eaa>   DW_AT_name        : (strp) (offset: 0x41e): Py_IS_TYPE
-    <3eae>   DW_AT_decl_file   : (data1) 2
-    <3eaf>   DW_AT_decl_line   : (data1) 149
-    <3eb0>   DW_AT_decl_column : (data1) 19
-    <3eb1>   DW_AT_prototyped  : (flag_present) 1
-    <3eb1>   DW_AT_type        : (ref4) <0x4f>, int
-    <3eb5>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
-    <3eb6>   DW_AT_sibling     : (ref4) <0x3ed2>
- <2><3eba>: Abbrev Number: 84 (DW_TAG_formal_parameter)
-    <3ebb>   DW_AT_name        : (string) ob
-    <3ebe>   DW_AT_decl_file   : (data1) 2
-    <3ebf>   DW_AT_decl_line   : (data1) 149
-    <3ec0>   DW_AT_decl_column : (data1) 40
-    <3ec1>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><3ec5>: Abbrev Number: 71 (DW_TAG_formal_parameter)
-    <3ec6>   DW_AT_name        : (strp) (offset: 0x2201): type
-    <3eca>   DW_AT_decl_file   : (data1) 2
-    <3ecb>   DW_AT_decl_line   : (data1) 149
-    <3ecc>   DW_AT_decl_column : (data1) 58
-    <3ecd>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
- <2><3ed1>: Abbrev Number: 0
- <1><3ed2>: Abbrev Number: 83 (DW_TAG_subprogram)
-    <3ed3>   DW_AT_name        : (strp) (offset: 0x2bd): Py_SIZE
-    <3ed7>   DW_AT_decl_file   : (data1) 2
-    <3ed8>   DW_AT_decl_line   : (data1) 140
-    <3ed9>   DW_AT_decl_column : (data1) 26
-    <3eda>   DW_AT_prototyped  : (flag_present) 1
-    <3eda>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
-    <3ede>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
-    <3edf>   DW_AT_sibling     : (ref4) <0x3efb>
- <2><3ee3>: Abbrev Number: 84 (DW_TAG_formal_parameter)
-    <3ee4>   DW_AT_name        : (string) ob
-    <3ee7>   DW_AT_decl_file   : (data1) 2
-    <3ee8>   DW_AT_decl_line   : (data1) 140
-    <3ee9>   DW_AT_decl_column : (data1) 44
-    <3eea>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><3eee>: Abbrev Number: 72 (DW_TAG_variable)
-    <3eef>   DW_AT_name        : (strp) (offset: 0x1996): var_ob
-    <3ef3>   DW_AT_decl_file   : (data1) 2
-    <3ef4>   DW_AT_decl_line   : (data1) 141
-    <3ef5>   DW_AT_decl_column : (data1) 18
-    <3ef6>   DW_AT_type        : (ref4) <0x3efb>, PyVarObject
- <2><3efa>: Abbrev Number: 0
- <1><3efb>: Abbrev Number: 10 (DW_TAG_pointer_type)
-    <3efc>   DW_AT_byte_size   : (data1) 8
-    <3efd>   DW_AT_type        : (ref4) <0xba1>, PyVarObject
- <1><3f01>: Abbrev Number: 83 (DW_TAG_subprogram)
-    <3f02>   DW_AT_name        : (strp) (offset: 0x11b4): Py_TYPE
-    <3f06>   DW_AT_decl_file   : (data1) 2
-    <3f07>   DW_AT_decl_line   : (data1) 132
-    <3f08>   DW_AT_decl_column : (data1) 29
-    <3f09>   DW_AT_prototyped  : (flag_present) 1
-    <3f09>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
-    <3f0d>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
-    <3f0e>   DW_AT_sibling     : (ref4) <0x3f1e>
- <2><3f12>: Abbrev Number: 84 (DW_TAG_formal_parameter)
-    <3f13>   DW_AT_name        : (string) ob
-    <3f16>   DW_AT_decl_file   : (data1) 2
-    <3f17>   DW_AT_decl_line   : (data1) 132
-    <3f18>   DW_AT_decl_column : (data1) 47
-    <3f19>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
- <2><3f1d>: Abbrev Number: 0
- <1><3f1e>: Abbrev Number: 94 (DW_TAG_subprogram)
-    <3f1f>   DW_AT_abstract_origin: (ref4) <0x38c2>
-    <3f23>   DW_AT_low_pc      : (addr) 0x2b40
-    <3f2b>   DW_AT_high_pc     : (data8) 0x55
-    <3f33>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
-    <3f35>   DW_AT_GNU_all_call_sites: (flag_present) 1
-    <3f35>   DW_AT_sibling     : (ref4) <0x4006>
- <2><3f39>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <3f3a>   DW_AT_abstract_origin: (ref4) <0x38d3>
-    <3f3e>   DW_AT_location    : (sec_offset) 0x1fa9 (location list)
-    <3f42>   DW_AT_GNU_locviews: (sec_offset) 0x1f9f
- <2><3f46>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <3f47>   DW_AT_abstract_origin: (ref4) <0x38df>
-    <3f4b>   DW_AT_location    : (sec_offset) 0x202a (location list)
-    <3f4f>   DW_AT_GNU_locviews: (sec_offset) 0x201e
- <2><3f53>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <3f54>   DW_AT_abstract_origin: (ref4) <0x38eb>
-    <3f58>   DW_AT_location    : (sec_offset) 0x20be (location list)
-    <3f5c>   DW_AT_GNU_locviews: (sec_offset) 0x20b2
- <2><3f60>: Abbrev Number: 95 (DW_TAG_lexical_block)
-    <3f61>   DW_AT_abstract_origin: (ref4) <0x38f7>
-    <3f65>   DW_AT_ranges      : (sec_offset) 0x4d0
-    <3f69>   DW_AT_sibling     : (ref4) <0x3f7b>
- <3><3f6d>: Abbrev Number: 59 (DW_TAG_variable)
-    <3f6e>   DW_AT_abstract_origin: (ref4) <0x38fc>
-    <3f72>   DW_AT_location    : (sec_offset) 0x2148 (location list)
-    <3f76>   DW_AT_GNU_locviews: (sec_offset) 0x2146
- <3><3f7a>: Abbrev Number: 0
- <2><3f7b>: Abbrev Number: 96 (DW_TAG_lexical_block)
-    <3f7c>   DW_AT_abstract_origin: (ref4) <0x391c>
-    <3f80>   DW_AT_low_pc      : (addr) 0x2b68
-    <3f88>   DW_AT_high_pc     : (data8) 0x9
-    <3f90>   DW_AT_sibling     : (ref4) <0x3fa2>
- <3><3f94>: Abbrev Number: 59 (DW_TAG_variable)
-    <3f95>   DW_AT_abstract_origin: (ref4) <0x3921>
-    <3f99>   DW_AT_location    : (sec_offset) 0x216d (location list)
-    <3f9d>   DW_AT_GNU_locviews: (sec_offset) 0x216b
- <3><3fa1>: Abbrev Number: 0
- <2><3fa2>: Abbrev Number: 82 (DW_TAG_inlined_subroutine)
-    <3fa3>   DW_AT_abstract_origin: (ref4) <0x38c2>
-    <3fa7>   DW_AT_entry_pc    : (addr) 0x2b71
-    <3faf>   DW_AT_GNU_entry_view: (data1) 1
-    <3fb0>   DW_AT_ranges      : (sec_offset) 0x500
-    <3fb4>   DW_AT_call_file   : (data1) 1
-    <3fb5>   DW_AT_call_line   : (data1) 139
-    <3fb6>   DW_AT_call_column : (data1) 1
- <3><3fb7>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <3fb8>   DW_AT_abstract_origin: (ref4) <0x38eb>
-    <3fbc>   DW_AT_location    : (sec_offset) 0x2196 (location list)
-    <3fc0>   DW_AT_GNU_locviews: (sec_offset) 0x2190
- <3><3fc4>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <3fc5>   DW_AT_abstract_origin: (ref4) <0x38df>
-    <3fc9>   DW_AT_location    : (sec_offset) 0x21e8 (location list)
-    <3fcd>   DW_AT_GNU_locviews: (sec_offset) 0x21e2
- <3><3fd1>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <3fd2>   DW_AT_abstract_origin: (ref4) <0x38d3>
-    <3fd6>   DW_AT_location    : (sec_offset) 0x2238 (location list)
-    <3fda>   DW_AT_GNU_locviews: (sec_offset) 0x2234
- <3><3fde>: Abbrev Number: 97 (DW_TAG_lexical_block)
-    <3fdf>   DW_AT_abstract_origin: (ref4) <0x393e>
-    <3fe3>   DW_AT_ranges      : (sec_offset) 0x540
- <4><3fe7>: Abbrev Number: 98 (DW_TAG_variable)
-    <3fe8>   DW_AT_abstract_origin: (ref4) <0x393f>
-    <3fec>   DW_AT_location    : (exprloc) 1 byte block: 50 	(DW_OP_reg0 (rax))
- <4><3fee>: Abbrev Number: 55 (DW_TAG_GNU_call_site)
-    <3fef>   DW_AT_low_pc      : (addr) 0x2b88
-    <3ff7>   DW_AT_GNU_tail_call: (flag_present) 1
-    <3ff7>   DW_AT_GNU_call_site_target: (exprloc) 3 byte block: f3 1 54 	(DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)))
- <5><3ffb>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <3ffc>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <3ffe>   DW_AT_GNU_call_site_value: (exprloc) 3 byte block: f3 1 51 	(DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)))
- <5><4002>: Abbrev Number: 0
- <4><4003>: Abbrev Number: 0
- <3><4004>: Abbrev Number: 0
- <2><4005>: Abbrev Number: 0
- <1><4006>: Abbrev Number: 94 (DW_TAG_subprogram)
-    <4007>   DW_AT_abstract_origin: (ref4) <0x3232>
-    <400b>   DW_AT_low_pc      : (addr) 0x2ba0
-    <4013>   DW_AT_high_pc     : (data8) 0x8a
-    <401b>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
-    <401d>   DW_AT_GNU_all_call_sites: (flag_present) 1
-    <401d>   DW_AT_sibling     : (ref4) <0x41eb>
- <2><4021>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <4022>   DW_AT_abstract_origin: (ref4) <0x3243>
-    <4026>   DW_AT_location    : (sec_offset) 0x227f (location list)
-    <402a>   DW_AT_GNU_locviews: (sec_offset) 0x2271
- <2><402e>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <402f>   DW_AT_abstract_origin: (ref4) <0x324f>
-    <4033>   DW_AT_location    : (sec_offset) 0x2329 (location list)
-    <4037>   DW_AT_GNU_locviews: (sec_offset) 0x231d
- <2><403b>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <403c>   DW_AT_abstract_origin: (ref4) <0x325b>
-    <4040>   DW_AT_location    : (sec_offset) 0x23c0 (location list)
-    <4044>   DW_AT_GNU_locviews: (sec_offset) 0x23b4
- <2><4048>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <4049>   DW_AT_abstract_origin: (ref4) <0x3267>
-    <404d>   DW_AT_location    : (sec_offset) 0x2457 (location list)
-    <4051>   DW_AT_GNU_locviews: (sec_offset) 0x244b
- <2><4055>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <4056>   DW_AT_abstract_origin: (ref4) <0x3273>
-    <405a>   DW_AT_location    : (sec_offset) 0x24ee (location list)
-    <405e>   DW_AT_GNU_locviews: (sec_offset) 0x24e2
- <2><4062>: Abbrev Number: 59 (DW_TAG_variable)
-    <4063>   DW_AT_abstract_origin: (ref4) <0x327f>
-    <4067>   DW_AT_location    : (sec_offset) 0x257b (location list)
-    <406b>   DW_AT_GNU_locviews: (sec_offset) 0x2579
- <2><406f>: Abbrev Number: 59 (DW_TAG_variable)
-    <4070>   DW_AT_abstract_origin: (ref4) <0x328b>
-    <4074>   DW_AT_location    : (sec_offset) 0x25a4 (location list)
-    <4078>   DW_AT_GNU_locviews: (sec_offset) 0x259e
- <2><407c>: Abbrev Number: 59 (DW_TAG_variable)
-    <407d>   DW_AT_abstract_origin: (ref4) <0x3297>
-    <4081>   DW_AT_location    : (sec_offset) 0x25f2 (location list)
-    <4085>   DW_AT_GNU_locviews: (sec_offset) 0x25ee
- <2><4089>: Abbrev Number: 96 (DW_TAG_lexical_block)
-    <408a>   DW_AT_abstract_origin: (ref4) <0x32a3>
-    <408e>   DW_AT_low_pc      : (addr) 0x2bb6
-    <4096>   DW_AT_high_pc     : (data8) 0x33
-    <409e>   DW_AT_sibling     : (ref4) <0x4131>
- <3><40a2>: Abbrev Number: 59 (DW_TAG_variable)
-    <40a3>   DW_AT_abstract_origin: (ref4) <0x32a4>
-    <40a7>   DW_AT_location    : (sec_offset) 0x262b (location list)
-    <40ab>   DW_AT_GNU_locviews: (sec_offset) 0x2629
- <3><40af>: Abbrev Number: 77 (DW_TAG_inlined_subroutine)
-    <40b0>   DW_AT_abstract_origin: (ref4) <0x3e62>
-    <40b4>   DW_AT_entry_pc    : (addr) 0x2bd4
-    <40bc>   DW_AT_GNU_entry_view: (data1) 1
-    <40bd>   DW_AT_low_pc      : (addr) 0x2bd4
-    <40c5>   DW_AT_high_pc     : (data8) 0x8
-    <40cd>   DW_AT_call_file   : (data1) 1
-    <40ce>   DW_AT_call_line   : (data1) 235
-    <40cf>   DW_AT_call_column : (data1) 9
-    <40d0>   DW_AT_sibling     : (ref4) <0x40e2>
- <4><40d4>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <40d5>   DW_AT_abstract_origin: (ref4) <0x3e70>
-    <40d9>   DW_AT_location    : (sec_offset) 0x2651 (location list)
-    <40dd>   DW_AT_GNU_locviews: (sec_offset) 0x264f
- <4><40e1>: Abbrev Number: 0
- <3><40e2>: Abbrev Number: 99 (DW_TAG_inlined_subroutine)
-    <40e3>   DW_AT_abstract_origin: (ref4) <0x3cfa>
-    <40e7>   DW_AT_entry_pc    : (addr) 0x2bdc
-    <40ef>   DW_AT_GNU_entry_view: (data1) 1
-    <40f0>   DW_AT_low_pc      : (addr) 0x2bdc
-    <40f8>   DW_AT_high_pc     : (data8) 0x4
-    <4100>   DW_AT_call_file   : (data1) 1
-    <4101>   DW_AT_call_line   : (data1) 236
-    <4102>   DW_AT_call_column : (data1) 9
- <4><4103>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <4104>   DW_AT_abstract_origin: (ref4) <0x3d1e>
-    <4108>   DW_AT_location    : (sec_offset) 0x2676 (location list)
-    <410c>   DW_AT_GNU_locviews: (sec_offset) 0x2674
- <4><4110>: Abbrev Number: 62 (DW_TAG_formal_parameter)
-    <4111>   DW_AT_abstract_origin: (ref4) <0x3d12>
- <4><4115>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <4116>   DW_AT_abstract_origin: (ref4) <0x3d07>
-    <411a>   DW_AT_location    : (sec_offset) 0x269b (location list)
-    <411e>   DW_AT_GNU_locviews: (sec_offset) 0x2699
- <4><4122>: Abbrev Number: 59 (DW_TAG_variable)
-    <4123>   DW_AT_abstract_origin: (ref4) <0x3d2a>
-    <4127>   DW_AT_location    : (sec_offset) 0x26c0 (location list)
-    <412b>   DW_AT_GNU_locviews: (sec_offset) 0x26be
- <4><412f>: Abbrev Number: 0
- <3><4130>: Abbrev Number: 0
- <2><4131>: Abbrev Number: 77 (DW_TAG_inlined_subroutine)
-    <4132>   DW_AT_abstract_origin: (ref4) <0x3232>
-    <4136>   DW_AT_entry_pc    : (addr) 0x2c10
-    <413e>   DW_AT_GNU_entry_view: (data1) 0
-    <413f>   DW_AT_low_pc      : (addr) 0x2c10
-    <4147>   DW_AT_high_pc     : (data8) 0x18
-    <414f>   DW_AT_call_file   : (data1) 1
-    <4150>   DW_AT_call_line   : (data1) 219
-    <4151>   DW_AT_call_column : (data1) 1
-    <4152>   DW_AT_sibling     : (ref4) <0x41c2>
- <3><4156>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <4157>   DW_AT_abstract_origin: (ref4) <0x3243>
-    <415b>   DW_AT_location    : (sec_offset) 0x26e7 (location list)
-    <415f>   DW_AT_GNU_locviews: (sec_offset) 0x26e3
- <3><4163>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <4164>   DW_AT_abstract_origin: (ref4) <0x324f>
-    <4168>   DW_AT_location    : (sec_offset) 0x2724 (location list)
-    <416c>   DW_AT_GNU_locviews: (sec_offset) 0x2720
- <3><4170>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <4171>   DW_AT_abstract_origin: (ref4) <0x325b>
-    <4175>   DW_AT_location    : (sec_offset) 0x2761 (location list)
-    <4179>   DW_AT_GNU_locviews: (sec_offset) 0x275d
- <3><417d>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <417e>   DW_AT_abstract_origin: (ref4) <0x3267>
-    <4182>   DW_AT_location    : (sec_offset) 0x279e (location list)
-    <4186>   DW_AT_GNU_locviews: (sec_offset) 0x279a
- <3><418a>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <418b>   DW_AT_abstract_origin: (ref4) <0x3273>
-    <418f>   DW_AT_location    : (sec_offset) 0x27db (location list)
-    <4193>   DW_AT_GNU_locviews: (sec_offset) 0x27d7
- <3><4197>: Abbrev Number: 100 (DW_TAG_variable)
-    <4198>   DW_AT_abstract_origin: (ref4) <0x327f>
- <3><419c>: Abbrev Number: 100 (DW_TAG_variable)
-    <419d>   DW_AT_abstract_origin: (ref4) <0x328b>
- <3><41a1>: Abbrev Number: 100 (DW_TAG_variable)
-    <41a2>   DW_AT_abstract_origin: (ref4) <0x3297>
- <3><41a6>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
-    <41a7>   DW_AT_low_pc      : (addr) 0x2c26
-    <41af>   DW_AT_abstract_origin: (ref4) <0x4472>
- <4><41b3>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <41b4>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <41b6>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 20 30 0 0 0 0 0 0 	(DW_OP_addr: 3020)
- <4><41c0>: Abbrev Number: 0
- <3><41c1>: Abbrev Number: 0
- <2><41c2>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
-    <41c3>   DW_AT_low_pc      : (addr) 0x2bb6
-    <41cb>   DW_AT_abstract_origin: (ref4) <0x44d5>
- <2><41cf>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
-    <41d0>   DW_AT_low_pc      : (addr) 0x2c06
-    <41d8>   DW_AT_abstract_origin: (ref4) <0x4472>
- <3><41dc>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <41dd>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <41df>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 38 30 0 0 0 0 0 0 	(DW_OP_addr: 3038)
- <3><41e9>: Abbrev Number: 0
- <2><41ea>: Abbrev Number: 0
- <1><41eb>: Abbrev Number: 94 (DW_TAG_subprogram)
-    <41ec>   DW_AT_abstract_origin: (ref4) <0x3bce>
-    <41f0>   DW_AT_low_pc      : (addr) 0x2c30
-    <41f8>   DW_AT_high_pc     : (data8) 0x70
-    <4200>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
-    <4202>   DW_AT_GNU_all_call_sites: (flag_present) 1
-    <4202>   DW_AT_sibling     : (ref4) <0x432c>
- <2><4206>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <4207>   DW_AT_abstract_origin: (ref4) <0x3bdf>
-    <420b>   DW_AT_location    : (sec_offset) 0x281e (location list)
-    <420f>   DW_AT_GNU_locviews: (sec_offset) 0x2814
- <2><4213>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <4214>   DW_AT_abstract_origin: (ref4) <0x3beb>
-    <4218>   DW_AT_location    : (sec_offset) 0x2897 (location list)
-    <421c>   DW_AT_GNU_locviews: (sec_offset) 0x2893
- <2><4220>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <4221>   DW_AT_abstract_origin: (ref4) <0x3bf7>
-    <4225>   DW_AT_location    : (sec_offset) 0x28da (location list)
-    <4229>   DW_AT_GNU_locviews: (sec_offset) 0x28d0
- <2><422d>: Abbrev Number: 59 (DW_TAG_variable)
-    <422e>   DW_AT_abstract_origin: (ref4) <0x3c03>
-    <4232>   DW_AT_location    : (sec_offset) 0x2951 (location list)
-    <4236>   DW_AT_GNU_locviews: (sec_offset) 0x294f
- <2><423a>: Abbrev Number: 59 (DW_TAG_variable)
-    <423b>   DW_AT_abstract_origin: (ref4) <0x3c0f>
-    <423f>   DW_AT_location    : (sec_offset) 0x2976 (location list)
-    <4243>   DW_AT_GNU_locviews: (sec_offset) 0x2974
- <2><4247>: Abbrev Number: 77 (DW_TAG_inlined_subroutine)
-    <4248>   DW_AT_abstract_origin: (ref4) <0x3e62>
-    <424c>   DW_AT_entry_pc    : (addr) 0x2c6d
-    <4254>   DW_AT_GNU_entry_view: (data1) 1
-    <4255>   DW_AT_low_pc      : (addr) 0x2c6d
-    <425d>   DW_AT_high_pc     : (data8) 0x4
-    <4265>   DW_AT_call_file   : (data1) 1
-    <4266>   DW_AT_call_line   : (data1) 72
-    <4267>   DW_AT_call_column : (data1) 5
-    <4268>   DW_AT_sibling     : (ref4) <0x427a>
- <3><426c>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <426d>   DW_AT_abstract_origin: (ref4) <0x3e70>
-    <4271>   DW_AT_location    : (sec_offset) 0x299b (location list)
-    <4275>   DW_AT_GNU_locviews: (sec_offset) 0x2999
- <3><4279>: Abbrev Number: 0
- <2><427a>: Abbrev Number: 75 (DW_TAG_inlined_subroutine)
-    <427b>   DW_AT_abstract_origin: (ref4) <0x3bce>
-    <427f>   DW_AT_entry_pc    : (addr) 0x2c80
-    <4287>   DW_AT_GNU_entry_view: (data1) 0
-    <4288>   DW_AT_ranges      : (sec_offset) 0x580
-    <428c>   DW_AT_call_file   : (data1) 1
-    <428d>   DW_AT_call_line   : (data1) 61
-    <428e>   DW_AT_call_column : (data1) 1
-    <428f>   DW_AT_sibling     : (ref4) <0x42e6>
- <3><4293>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <4294>   DW_AT_abstract_origin: (ref4) <0x3bdf>
-    <4298>   DW_AT_location    : (sec_offset) 0x29c0 (location list)
-    <429c>   DW_AT_GNU_locviews: (sec_offset) 0x29be
- <3><42a0>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <42a1>   DW_AT_abstract_origin: (ref4) <0x3beb>
-    <42a5>   DW_AT_location    : (sec_offset) 0x29e5 (location list)
-    <42a9>   DW_AT_GNU_locviews: (sec_offset) 0x29e3
- <3><42ad>: Abbrev Number: 48 (DW_TAG_formal_parameter)
-    <42ae>   DW_AT_abstract_origin: (ref4) <0x3bf7>
-    <42b2>   DW_AT_location    : (sec_offset) 0x2a0d (location list)
-    <42b6>   DW_AT_GNU_locviews: (sec_offset) 0x2a0b
- <3><42ba>: Abbrev Number: 58 (DW_TAG_lexical_block)
-    <42bb>   DW_AT_ranges      : (sec_offset) 0x580
- <4><42bf>: Abbrev Number: 100 (DW_TAG_variable)
-    <42c0>   DW_AT_abstract_origin: (ref4) <0x3c03>
- <4><42c4>: Abbrev Number: 100 (DW_TAG_variable)
-    <42c5>   DW_AT_abstract_origin: (ref4) <0x3c0f>
- <4><42c9>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
-    <42ca>   DW_AT_low_pc      : (addr) 0x2c96
-    <42d2>   DW_AT_abstract_origin: (ref4) <0x4472>
- <5><42d6>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <42d7>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
-    <42d9>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 52 30 0 0 0 0 0 0 	(DW_OP_addr: 3052)
- <5><42e3>: Abbrev Number: 0
- <4><42e4>: Abbrev Number: 0
- <3><42e5>: Abbrev Number: 0
- <2><42e6>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <42e7>   DW_AT_low_pc      : (addr) 0x2c45
-    <42ef>   DW_AT_abstract_origin: (ref4) <0x44e1>
-    <42f3>   DW_AT_sibling     : (ref4) <0x42ff>
- <3><42f7>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <42f8>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <42fa>   DW_AT_GNU_call_site_value: (exprloc) 3 byte block: f3 1 54 	(DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)))
- <3><42fe>: Abbrev Number: 0
- <2><42ff>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
-    <4300>   DW_AT_low_pc      : (addr) 0x2c57
-    <4308>   DW_AT_abstract_origin: (ref4) <0x44ed>
-    <430c>   DW_AT_sibling     : (ref4) <0x4317>
- <3><4310>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <4311>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <4313>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
- <3><4316>: Abbrev Number: 0
- <2><4317>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
-    <4318>   DW_AT_low_pc      : (addr) 0x2c64
-    <4320>   DW_AT_abstract_origin: (ref4) <0x439a>
- <3><4324>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
-    <4325>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
-    <4327>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7c 0 	(DW_OP_breg12 (r12): 0)
- <3><432a>: Abbrev Number: 0
- <2><432b>: Abbrev Number: 0
- <1><432c>: Abbrev Number: 101 (DW_TAG_subprogram)
-    <432d>   DW_AT_external    : (flag_present) 1
-    <432d>   DW_AT_declaration : (flag_present) 1
-    <432d>   DW_AT_linkage_name: (strp) (offset: 0x18fd): PyModuleDef_Init
-    <4331>   DW_AT_name        : (strp) (offset: 0x18fd): PyModuleDef_Init
-    <4335>   DW_AT_decl_file   : (data1) 12
-    <4336>   DW_AT_decl_line   : (data1) 40
-    <4337>   DW_AT_decl_column : (data1) 24
- <1><4338>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <4339>   DW_AT_external    : (flag_present) 1
-    <4339>   DW_AT_declaration : (flag_present) 1
-    <4339>   DW_AT_linkage_name: (strp) (offset: 0x2499): _Py_Dealloc
-    <433d>   DW_AT_name        : (strp) (offset: 0x2499): _Py_Dealloc
-    <4341>   DW_AT_decl_file   : (data1) 2
-    <4342>   DW_AT_decl_line   : (data2) 477
-    <4344>   DW_AT_decl_column : (data1) 18
- <1><4345>: Abbrev Number: 101 (DW_TAG_subprogram)
-    <4346>   DW_AT_external    : (flag_present) 1
-    <4346>   DW_AT_declaration : (flag_present) 1
-    <4346>   DW_AT_linkage_name: (strp) (offset: 0x1494): PyModule_GetState
-    <434a>   DW_AT_name        : (strp) (offset: 0x1494): PyModule_GetState
-    <434e>   DW_AT_decl_file   : (data1) 12
-    <434f>   DW_AT_decl_line   : (data1) 36
-    <4350>   DW_AT_decl_column : (data1) 19
- <1><4351>: Abbrev Number: 101 (DW_TAG_subprogram)
-    <4352>   DW_AT_external    : (flag_present) 1
-    <4352>   DW_AT_declaration : (flag_present) 1
-    <4352>   DW_AT_linkage_name: (strp) (offset: 0x11d2): PyType_FromModuleAndSpec
-    <4356>   DW_AT_name        : (strp) (offset: 0x11d2): PyType_FromModuleAndSpec
-    <435a>   DW_AT_decl_file   : (data1) 2
-    <435b>   DW_AT_decl_line   : (data1) 250
-    <435c>   DW_AT_decl_column : (data1) 23
- <1><435d>: Abbrev Number: 101 (DW_TAG_subprogram)
-    <435e>   DW_AT_external    : (flag_present) 1
-    <435e>   DW_AT_declaration : (flag_present) 1
-    <435e>   DW_AT_linkage_name: (strp) (offset: 0x1e6): PyModule_AddType
-    <4362>   DW_AT_name        : (strp) (offset: 0x1e6): PyModule_AddType
-    <4366>   DW_AT_decl_file   : (data1) 69
-    <4367>   DW_AT_decl_line   : (data1) 58
-    <4368>   DW_AT_decl_column : (data1) 17
- <1><4369>: Abbrev Number: 101 (DW_TAG_subprogram)
-    <436a>   DW_AT_external    : (flag_present) 1
-    <436a>   DW_AT_declaration : (flag_present) 1
-    <436a>   DW_AT_linkage_name: (strp) (offset: 0xea5): PyTuple_New
-    <436e>   DW_AT_name        : (strp) (offset: 0xea5): PyTuple_New
-    <4372>   DW_AT_decl_file   : (data1) 35
-    <4373>   DW_AT_decl_line   : (data1) 30
-    <4374>   DW_AT_decl_column : (data1) 24
- <1><4375>: Abbrev Number: 101 (DW_TAG_subprogram)
-    <4376>   DW_AT_external    : (flag_present) 1
-    <4376>   DW_AT_declaration : (flag_present) 1
-    <4376>   DW_AT_linkage_name: (strp) (offset: 0xb4a): PyUnicode_FromString
-    <437a>   DW_AT_name        : (strp) (offset: 0xb4a): PyUnicode_FromString
-    <437e>   DW_AT_decl_file   : (data1) 27
-    <437f>   DW_AT_decl_line   : (data1) 137
-    <4380>   DW_AT_decl_column : (data1) 23
- <1><4381>: Abbrev Number: 101 (DW_TAG_subprogram)
-    <4382>   DW_AT_external    : (flag_present) 1
-    <4382>   DW_AT_declaration : (flag_present) 1
-    <4382>   DW_AT_linkage_name: (strp) (offset: 0x22c9): PyDict_SetItemString
-    <4386>   DW_AT_name        : (strp) (offset: 0x22c9): PyDict_SetItemString
-    <438a>   DW_AT_decl_file   : (data1) 37
-    <438b>   DW_AT_decl_line   : (data1) 58
-    <438c>   DW_AT_decl_column : (data1) 17
- <1><438d>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <438e>   DW_AT_external    : (flag_present) 1
-    <438e>   DW_AT_declaration : (flag_present) 1
-    <438e>   DW_AT_linkage_name: (strp) (offset: 0x1423): PyObject_RichCompareBool
-    <4392>   DW_AT_name        : (strp) (offset: 0x1423): PyObject_RichCompareBool
-    <4396>   DW_AT_decl_file   : (data1) 2
-    <4397>   DW_AT_decl_line   : (data2) 288
-    <4399>   DW_AT_decl_column : (data1) 17
- <1><439a>: Abbrev Number: 101 (DW_TAG_subprogram)
-    <439b>   DW_AT_external    : (flag_present) 1
-    <439b>   DW_AT_declaration : (flag_present) 1
-    <439b>   DW_AT_linkage_name: (strp) (offset: 0x1cbe): PyType_GetModuleState
-    <439f>   DW_AT_name        : (strp) (offset: 0x1cbe): PyType_GetModuleState
-    <43a3>   DW_AT_decl_file   : (data1) 2
-    <43a4>   DW_AT_decl_line   : (data1) 252
-    <43a5>   DW_AT_decl_column : (data1) 20
- <1><43a6>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <43a7>   DW_AT_external    : (flag_present) 1
-    <43a7>   DW_AT_declaration : (flag_present) 1
-    <43a7>   DW_AT_linkage_name: (strp) (offset: 0x2a8): PyObject_RichCompare
-    <43ab>   DW_AT_name        : (strp) (offset: 0x2a8): PyObject_RichCompare
-    <43af>   DW_AT_decl_file   : (data1) 2
-    <43b0>   DW_AT_decl_line   : (data2) 287
-    <43b2>   DW_AT_decl_column : (data1) 24
- <1><43b3>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <43b4>   DW_AT_external    : (flag_present) 1
-    <43b4>   DW_AT_declaration : (flag_present) 1
-    <43b4>   DW_AT_linkage_name: (strp) (offset: 0x1707): PyType_GetModuleByDef
-    <43b8>   DW_AT_name        : (strp) (offset: 0x1707): PyType_GetModuleByDef
-    <43bc>   DW_AT_decl_file   : (data1) 18
-    <43bd>   DW_AT_decl_line   : (data2) 273
-    <43bf>   DW_AT_decl_column : (data1) 24
- <1><43c0>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <43c1>   DW_AT_external    : (flag_present) 1
-    <43c1>   DW_AT_declaration : (flag_present) 1
-    <43c1>   DW_AT_linkage_name: (strp) (offset: 0x916): Py_ReprEnter
-    <43c5>   DW_AT_name        : (strp) (offset: 0x916): Py_ReprEnter
-    <43c9>   DW_AT_decl_file   : (data1) 2
-    <43ca>   DW_AT_decl_line   : (data2) 322
-    <43cc>   DW_AT_decl_column : (data1) 17
- <1><43cd>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <43ce>   DW_AT_external    : (flag_present) 1
-    <43ce>   DW_AT_declaration : (flag_present) 1
-    <43ce>   DW_AT_linkage_name: (strp) (offset: 0xb1): _PyUnicodeWriter_Init
-    <43d2>   DW_AT_name        : (strp) (offset: 0xb1): _PyUnicodeWriter_Init
-    <43d6>   DW_AT_decl_file   : (data1) 28
-    <43d7>   DW_AT_decl_line   : (data2) 746
-    <43d9>   DW_AT_decl_column : (data1) 1
- <1><43da>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <43db>   DW_AT_external    : (flag_present) 1
-    <43db>   DW_AT_declaration : (flag_present) 1
-    <43db>   DW_AT_linkage_name: (strp) (offset: 0x22de): _PyUnicodeWriter_WriteChar
-    <43df>   DW_AT_name        : (strp) (offset: 0x22de): _PyUnicodeWriter_WriteChar
-    <43e3>   DW_AT_decl_file   : (data1) 28
-    <43e4>   DW_AT_decl_line   : (data2) 786
-    <43e6>   DW_AT_decl_column : (data1) 1
- <1><43e7>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <43e8>   DW_AT_external    : (flag_present) 1
-    <43e8>   DW_AT_declaration : (flag_present) 1
-    <43e8>   DW_AT_linkage_name: (strp) (offset: 0x1780): PyObject_Repr
-    <43ec>   DW_AT_name        : (strp) (offset: 0x1780): PyObject_Repr
-    <43f0>   DW_AT_decl_file   : (data1) 2
-    <43f1>   DW_AT_decl_line   : (data2) 283
-    <43f3>   DW_AT_decl_column : (data1) 24
- <1><43f4>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <43f5>   DW_AT_external    : (flag_present) 1
-    <43f5>   DW_AT_declaration : (flag_present) 1
-    <43f5>   DW_AT_linkage_name: (strp) (offset: 0x14f3): _PyUnicodeWriter_WriteStr
-    <43f9>   DW_AT_name        : (strp) (offset: 0x14f3): _PyUnicodeWriter_WriteStr
-    <43fd>   DW_AT_decl_file   : (data1) 28
-    <43fe>   DW_AT_decl_line   : (data2) 793
-    <4400>   DW_AT_decl_column : (data1) 1
- <1><4401>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <4402>   DW_AT_external    : (flag_present) 1
-    <4402>   DW_AT_declaration : (flag_present) 1
-    <4402>   DW_AT_linkage_name: (strp) (offset: 0x20c2): _PyUnicodeWriter_Dealloc
-    <4406>   DW_AT_name        : (strp) (offset: 0x20c2): _PyUnicodeWriter_Dealloc
-    <440a>   DW_AT_decl_file   : (data1) 28
-    <440b>   DW_AT_decl_line   : (data2) 830
-    <440d>   DW_AT_decl_column : (data1) 1
- <1><440e>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <440f>   DW_AT_external    : (flag_present) 1
-    <440f>   DW_AT_declaration : (flag_present) 1
-    <440f>   DW_AT_linkage_name: (strp) (offset: 0xf4c): Py_ReprLeave
-    <4413>   DW_AT_name        : (strp) (offset: 0xf4c): Py_ReprLeave
-    <4417>   DW_AT_decl_file   : (data1) 2
-    <4418>   DW_AT_decl_line   : (data2) 323
-    <441a>   DW_AT_decl_column : (data1) 18
- <1><441b>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <441c>   DW_AT_external    : (flag_present) 1
-    <441c>   DW_AT_declaration : (flag_present) 1
-    <441c>   DW_AT_linkage_name: (strp) (offset: 0x6a5): PyUnicode_FromFormat
-    <4420>   DW_AT_name        : (strp) (offset: 0x6a5): PyUnicode_FromFormat
-    <4424>   DW_AT_decl_file   : (data1) 27
-    <4425>   DW_AT_decl_line   : (data2) 258
-    <4427>   DW_AT_decl_column : (data1) 24
- <1><4428>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <4429>   DW_AT_external    : (flag_present) 1
-    <4429>   DW_AT_declaration : (flag_present) 1
-    <4429>   DW_AT_linkage_name: (strp) (offset: 0x12e2): _PyUnicodeWriter_WriteASCIIString
-    <442d>   DW_AT_name        : (strp) (offset: 0x12e2): _PyUnicodeWriter_WriteASCIIString
-    <4431>   DW_AT_decl_file   : (data1) 28
-    <4432>   DW_AT_decl_line   : (data2) 809
-    <4434>   DW_AT_decl_column : (data1) 1
- <1><4435>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <4436>   DW_AT_external    : (flag_present) 1
-    <4436>   DW_AT_declaration : (flag_present) 1
-    <4436>   DW_AT_linkage_name: (strp) (offset: 0x1d32): _PyUnicodeWriter_Finish
-    <443a>   DW_AT_name        : (strp) (offset: 0x1d32): _PyUnicodeWriter_Finish
-    <443e>   DW_AT_decl_file   : (data1) 28
-    <443f>   DW_AT_decl_line   : (data2) 826
-    <4441>   DW_AT_decl_column : (data1) 1
- <1><4442>: Abbrev Number: 103 (DW_TAG_subprogram)
-    <4443>   DW_AT_external    : (flag_present) 1
-    <4443>   DW_AT_declaration : (flag_present) 1
-    <4443>   DW_AT_linkage_name: (strp) (offset: 0x126a): __stack_chk_fail
-    <4447>   DW_AT_name        : (strp) (offset: 0x126a): __stack_chk_fail
- <1><444b>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <444c>   DW_AT_external    : (flag_present) 1
-    <444c>   DW_AT_declaration : (flag_present) 1
-    <444c>   DW_AT_linkage_name: (strp) (offset: 0x9f6): PyType_IsSubtype
-    <4450>   DW_AT_name        : (strp) (offset: 0x9f6): PyType_IsSubtype
-    <4454>   DW_AT_decl_file   : (data1) 2
-    <4455>   DW_AT_decl_line   : (data2) 260
-    <4457>   DW_AT_decl_column : (data1) 17
- <1><4458>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <4459>   DW_AT_external    : (flag_present) 1
-    <4459>   DW_AT_declaration : (flag_present) 1
-    <4459>   DW_AT_linkage_name: (strp) (offset: 0x1697): PySequence_Tuple
-    <445d>   DW_AT_name        : (strp) (offset: 0x1697): PySequence_Tuple
-    <4461>   DW_AT_decl_file   : (data1) 70
-    <4462>   DW_AT_decl_line   : (data2) 702
-    <4464>   DW_AT_decl_column : (data1) 24
- <1><4465>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <4466>   DW_AT_external    : (flag_present) 1
-    <4466>   DW_AT_declaration : (flag_present) 1
-    <4466>   DW_AT_linkage_name: (strp) (offset: 0xc95): PySequence_Fast
-    <446a>   DW_AT_name        : (strp) (offset: 0xc95): PySequence_Fast
-    <446e>   DW_AT_decl_file   : (data1) 70
-    <446f>   DW_AT_decl_line   : (data2) 715
-    <4471>   DW_AT_decl_column : (data1) 24
- <1><4472>: Abbrev Number: 101 (DW_TAG_subprogram)
-    <4473>   DW_AT_external    : (flag_present) 1
-    <4473>   DW_AT_declaration : (flag_present) 1
-    <4473>   DW_AT_linkage_name: (strp) (offset: 0x2427): PyErr_SetString
-    <4477>   DW_AT_name        : (strp) (offset: 0x2427): PyErr_SetString
-    <447b>   DW_AT_decl_file   : (data1) 60
-    <447c>   DW_AT_decl_line   : (data1) 13
-    <447d>   DW_AT_decl_column : (data1) 18
- <1><447e>: Abbrev Number: 101 (DW_TAG_subprogram)
-    <447f>   DW_AT_external    : (flag_present) 1
-    <447f>   DW_AT_declaration : (flag_present) 1
-    <447f>   DW_AT_linkage_name: (strp) (offset: 0x1009): PyObject_CallFunctionObjArgs
-    <4483>   DW_AT_name        : (strp) (offset: 0x1009): PyObject_CallFunctionObjArgs
-    <4487>   DW_AT_decl_file   : (data1) 70
-    <4488>   DW_AT_decl_line   : (data1) 215
-    <4489>   DW_AT_decl_column : (data1) 24
- <1><448a>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <448b>   DW_AT_external    : (flag_present) 1
-    <448b>   DW_AT_declaration : (flag_present) 1
-    <448b>   DW_AT_linkage_name: (strp) (offset: 0x1179): _PyTrash_cond
-    <448f>   DW_AT_name        : (strp) (offset: 0x1179): _PyTrash_cond
-    <4493>   DW_AT_decl_file   : (data1) 18
-    <4494>   DW_AT_decl_line   : (data2) 475
-    <4496>   DW_AT_decl_column : (data1) 17
- <1><4497>: Abbrev Number: 101 (DW_TAG_subprogram)
-    <4498>   DW_AT_external    : (flag_present) 1
-    <4498>   DW_AT_declaration : (flag_present) 1
-    <4498>   DW_AT_linkage_name: (strp) (offset: 0x1a4f): PyThreadState_Get
-    <449c>   DW_AT_name        : (strp) (offset: 0x1a4f): PyThreadState_Get
-    <44a0>   DW_AT_decl_file   : (data1) 71
-    <44a1>   DW_AT_decl_line   : (data1) 60
-    <44a2>   DW_AT_decl_column : (data1) 29
- <1><44a3>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <44a4>   DW_AT_external    : (flag_present) 1
-    <44a4>   DW_AT_declaration : (flag_present) 1
-    <44a4>   DW_AT_linkage_name: (strp) (offset: 0x23bd): _PyTrash_begin
-    <44a8>   DW_AT_name        : (strp) (offset: 0x23bd): _PyTrash_begin
-    <44ac>   DW_AT_decl_file   : (data1) 18
-    <44ad>   DW_AT_decl_line   : (data2) 472
-    <44af>   DW_AT_decl_column : (data1) 17
- <1><44b0>: Abbrev Number: 102 (DW_TAG_subprogram)
-    <44b1>   DW_AT_external    : (flag_present) 1
-    <44b1>   DW_AT_declaration : (flag_present) 1
-    <44b1>   DW_AT_linkage_name: (strp) (offset: 0xa38): _PyTrash_end
-    <44b5>   DW_AT_name        : (strp) (offset: 0xa38): _PyTrash_end
-    <44b9>   DW_AT_decl_file   : (data1) 18
-    <44ba>   DW_AT_decl_line   : (data2) 473
-    <44bc>   DW_AT_decl_column : (data1) 18
- <1><44bd>: Abbrev Number: 101 (DW_TAG_subprogram)
-    <44be>   DW_AT_external    : (flag_present) 1
-    <44be>   DW_AT_declaration : (flag_present) 1
-    <44be>   DW_AT_linkage_name: (strp) (offset: 0x804): PyObject_GC_UnTrack
-    <44c2>   DW_AT_name        : (strp) (offset: 0x804): PyObject_GC_UnTrack
-    <44c6>   DW_AT_decl_file   : (data1) 72
-    <44c7>   DW_AT_decl_line   : (data1) 180
-    <44c8>   DW_AT_decl_column : (data1) 18
- <1><44c9>: Abbrev Number: 101 (DW_TAG_subprogram)
-    <44ca>   DW_AT_external    : (flag_present) 1
-    <44ca>   DW_AT_declaration : (flag_present) 1
-    <44ca>   DW_AT_linkage_name: (strp) (offset: 0x1afe): _PyArg_ParseTupleAndKeywords_SizeT
-    <44ce>   DW_AT_name        : (strp) (offset: 0x1afe): _PyArg_ParseTupleAndKeywords_SizeT
-    <44d2>   DW_AT_decl_file   : (data1) 69
-    <44d3>   DW_AT_decl_line   : (data1) 28
-    <44d4>   DW_AT_decl_column : (data1) 17
- <1><44d5>: Abbrev Number: 101 (DW_TAG_subprogram)
-    <44d6>   DW_AT_external    : (flag_present) 1
-    <44d6>   DW_AT_declaration : (flag_present) 1
-    <44d6>   DW_AT_linkage_name: (strp) (offset: 0xc8a): PyList_New
-    <44da>   DW_AT_name        : (strp) (offset: 0xc8a): PyList_New
-    <44de>   DW_AT_decl_file   : (data1) 36
-    <44df>   DW_AT_decl_line   : (data1) 28
-    <44e0>   DW_AT_decl_column : (data1) 24
- <1><44e1>: Abbrev Number: 101 (DW_TAG_subprogram)
-    <44e2>   DW_AT_external    : (flag_present) 1
-    <44e2>   DW_AT_declaration : (flag_present) 1
-    <44e2>   DW_AT_linkage_name: (strp) (offset: 0x24b3): PyTuple_Size
-    <44e6>   DW_AT_name        : (strp) (offset: 0x24b3): PyTuple_Size
-    <44ea>   DW_AT_decl_file   : (data1) 35
-    <44eb>   DW_AT_decl_line   : (data1) 31
-    <44ec>   DW_AT_decl_column : (data1) 24
- <1><44ed>: Abbrev Number: 101 (DW_TAG_subprogram)
-    <44ee>   DW_AT_external    : (flag_present) 1
-    <44ee>   DW_AT_declaration : (flag_present) 1
-    <44ee>   DW_AT_linkage_name: (strp) (offset: 0x1c2e): PyDict_Size
-    <44f2>   DW_AT_name        : (strp) (offset: 0x1c2e): PyDict_Size
-    <44f6>   DW_AT_decl_file   : (data1) 37
-    <44f7>   DW_AT_decl_line   : (data1) 32
-    <44f8>   DW_AT_decl_column : (data1) 24
- <1><44f9>: Abbrev Number: 0
-  Compilation Unit @ offset 0x44fa:
+    <3de0>   DW_AT_sibling     : (ref4) <0x3e14>
+ <2><3de4>: Abbrev Number: 85 (DW_TAG_formal_parameter)
+    <3de5>   DW_AT_name        : (string) op
+    <3de8>   DW_AT_decl_file   : (data1) 4
+    <3de9>   DW_AT_decl_line   : (data1) 44
+    <3dea>   DW_AT_decl_column : (data1) 27
+    <3deb>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3def>: Abbrev Number: 69 (DW_TAG_formal_parameter)
+    <3df0>   DW_AT_name        : (strp) (offset: 0x1a08): index
+    <3df4>   DW_AT_decl_file   : (data1) 4
+    <3df5>   DW_AT_decl_line   : (data1) 44
+    <3df6>   DW_AT_decl_column : (data1) 42
+    <3df7>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
+ <2><3dfb>: Abbrev Number: 69 (DW_TAG_formal_parameter)
+    <3dfc>   DW_AT_name        : (strp) (offset: 0xb09): value
+    <3e00>   DW_AT_decl_file   : (data1) 4
+    <3e01>   DW_AT_decl_line   : (data1) 44
+    <3e02>   DW_AT_decl_column : (data1) 59
+    <3e03>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3e07>: Abbrev Number: 70 (DW_TAG_variable)
+    <3e08>   DW_AT_name        : (strp) (offset: 0x99d): list
+    <3e0c>   DW_AT_decl_file   : (data1) 4
+    <3e0d>   DW_AT_decl_line   : (data1) 45
+    <3e0e>   DW_AT_decl_column : (data1) 19
+    <3e0f>   DW_AT_type        : (ref4) <0x3e14>, PyListObject
+ <2><3e13>: Abbrev Number: 0
+ <1><3e14>: Abbrev Number: 10 (DW_TAG_pointer_type)
+    <3e15>   DW_AT_byte_size   : (data1) 8
+    <3e16>   DW_AT_type        : (ref4) <0x18a7>, PyListObject
+ <1><3e1a>: Abbrev Number: 84 (DW_TAG_subprogram)
+    <3e1b>   DW_AT_name        : (strp) (offset: 0x7c5): PyList_GET_SIZE
+    <3e1f>   DW_AT_decl_file   : (data1) 4
+    <3e20>   DW_AT_decl_line   : (data1) 33
+    <3e21>   DW_AT_decl_column : (data1) 26
+    <3e22>   DW_AT_prototyped  : (flag_present) 1
+    <3e22>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
+    <3e26>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
+    <3e27>   DW_AT_sibling     : (ref4) <0x3e43>
+ <2><3e2b>: Abbrev Number: 85 (DW_TAG_formal_parameter)
+    <3e2c>   DW_AT_name        : (string) op
+    <3e2f>   DW_AT_decl_file   : (data1) 4
+    <3e30>   DW_AT_decl_line   : (data1) 33
+    <3e31>   DW_AT_decl_column : (data1) 52
+    <3e32>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3e36>: Abbrev Number: 70 (DW_TAG_variable)
+    <3e37>   DW_AT_name        : (strp) (offset: 0x99d): list
+    <3e3b>   DW_AT_decl_file   : (data1) 4
+    <3e3c>   DW_AT_decl_line   : (data1) 34
+    <3e3d>   DW_AT_decl_column : (data1) 19
+    <3e3e>   DW_AT_type        : (ref4) <0x3e14>, PyListObject
+ <2><3e42>: Abbrev Number: 0
+ <1><3e43>: Abbrev Number: 89 (DW_TAG_subprogram)
+    <3e44>   DW_AT_name        : (strp) (offset: 0x2c5): PyTuple_SET_ITEM
+    <3e48>   DW_AT_decl_file   : (data1) 3
+    <3e49>   DW_AT_decl_line   : (data1) 34
+    <3e4a>   DW_AT_decl_column : (data1) 1
+    <3e4b>   DW_AT_prototyped  : (flag_present) 1
+    <3e4b>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
+    <3e4c>   DW_AT_sibling     : (ref4) <0x3e80>
+ <2><3e50>: Abbrev Number: 85 (DW_TAG_formal_parameter)
+    <3e51>   DW_AT_name        : (string) op
+    <3e54>   DW_AT_decl_file   : (data1) 3
+    <3e55>   DW_AT_decl_line   : (data1) 34
+    <3e56>   DW_AT_decl_column : (data1) 28
+    <3e57>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3e5b>: Abbrev Number: 69 (DW_TAG_formal_parameter)
+    <3e5c>   DW_AT_name        : (strp) (offset: 0x1a08): index
+    <3e60>   DW_AT_decl_file   : (data1) 3
+    <3e61>   DW_AT_decl_line   : (data1) 34
+    <3e62>   DW_AT_decl_column : (data1) 43
+    <3e63>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
+ <2><3e67>: Abbrev Number: 69 (DW_TAG_formal_parameter)
+    <3e68>   DW_AT_name        : (strp) (offset: 0xb09): value
+    <3e6c>   DW_AT_decl_file   : (data1) 3
+    <3e6d>   DW_AT_decl_line   : (data1) 34
+    <3e6e>   DW_AT_decl_column : (data1) 60
+    <3e6f>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3e73>: Abbrev Number: 70 (DW_TAG_variable)
+    <3e74>   DW_AT_name        : (strp) (offset: 0x677): tuple
+    <3e78>   DW_AT_decl_file   : (data1) 3
+    <3e79>   DW_AT_decl_line   : (data1) 35
+    <3e7a>   DW_AT_decl_column : (data1) 20
+    <3e7b>   DW_AT_type        : (ref4) <0x3e80>, PyTupleObject
+ <2><3e7f>: Abbrev Number: 0
+ <1><3e80>: Abbrev Number: 10 (DW_TAG_pointer_type)
+    <3e81>   DW_AT_byte_size   : (data1) 8
+    <3e82>   DW_AT_type        : (ref4) <0x1846>, PyTupleObject
+ <1><3e86>: Abbrev Number: 84 (DW_TAG_subprogram)
+    <3e87>   DW_AT_name        : (strp) (offset: 0x17d7): PyTuple_GET_SIZE
+    <3e8b>   DW_AT_decl_file   : (data1) 3
+    <3e8c>   DW_AT_decl_line   : (data1) 22
+    <3e8d>   DW_AT_decl_column : (data1) 26
+    <3e8e>   DW_AT_prototyped  : (flag_present) 1
+    <3e8e>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
+    <3e92>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
+    <3e93>   DW_AT_sibling     : (ref4) <0x3eaf>
+ <2><3e97>: Abbrev Number: 85 (DW_TAG_formal_parameter)
+    <3e98>   DW_AT_name        : (string) op
+    <3e9b>   DW_AT_decl_file   : (data1) 3
+    <3e9c>   DW_AT_decl_line   : (data1) 22
+    <3e9d>   DW_AT_decl_column : (data1) 53
+    <3e9e>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3ea2>: Abbrev Number: 70 (DW_TAG_variable)
+    <3ea3>   DW_AT_name        : (strp) (offset: 0x677): tuple
+    <3ea7>   DW_AT_decl_file   : (data1) 3
+    <3ea8>   DW_AT_decl_line   : (data1) 23
+    <3ea9>   DW_AT_decl_column : (data1) 20
+    <3eaa>   DW_AT_type        : (ref4) <0x3e80>, PyTupleObject
+ <2><3eae>: Abbrev Number: 0
+ <1><3eaf>: Abbrev Number: 90 (DW_TAG_subprogram)
+    <3eb0>   DW_AT_name        : (strp) (offset: 0x15af): PyType_HasFeature
+    <3eb4>   DW_AT_decl_file   : (data1) 2
+    <3eb5>   DW_AT_decl_line   : (data2) 763
+    <3eb7>   DW_AT_decl_column : (data1) 1
+    <3eb8>   DW_AT_prototyped  : (flag_present) 1
+    <3eb8>   DW_AT_type        : (ref4) <0x4f>, int
+    <3ebc>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
+    <3ebd>   DW_AT_sibling     : (ref4) <0x3ee9>
+ <2><3ec1>: Abbrev Number: 91 (DW_TAG_formal_parameter)
+    <3ec2>   DW_AT_name        : (strp) (offset: 0x2201): type
+    <3ec6>   DW_AT_decl_file   : (data1) 2
+    <3ec7>   DW_AT_decl_line   : (data2) 763
+    <3ec9>   DW_AT_decl_column : (data1) 33
+    <3eca>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
+ <2><3ece>: Abbrev Number: 91 (DW_TAG_formal_parameter)
+    <3ecf>   DW_AT_name        : (strp) (offset: 0x98d): feature
+    <3ed3>   DW_AT_decl_file   : (data1) 2
+    <3ed4>   DW_AT_decl_line   : (data2) 763
+    <3ed6>   DW_AT_decl_column : (data1) 53
+    <3ed7>   DW_AT_type        : (ref4) <0x62>, long unsigned int
+ <2><3edb>: Abbrev Number: 92 (DW_TAG_variable)
+    <3edc>   DW_AT_name        : (strp) (offset: 0x1226): flags
+    <3ee0>   DW_AT_decl_file   : (data1) 2
+    <3ee1>   DW_AT_decl_line   : (data2) 765
+    <3ee3>   DW_AT_decl_column : (data1) 19
+    <3ee4>   DW_AT_type        : (ref4) <0x62>, long unsigned int
+ <2><3ee8>: Abbrev Number: 0
+ <1><3ee9>: Abbrev Number: 90 (DW_TAG_subprogram)
+    <3eea>   DW_AT_name        : (strp) (offset: 0x1658): _Py_NewRef
+    <3eee>   DW_AT_decl_file   : (data1) 2
+    <3eef>   DW_AT_decl_line   : (data2) 616
+    <3ef1>   DW_AT_decl_column : (data1) 25
+    <3ef2>   DW_AT_prototyped  : (flag_present) 1
+    <3ef2>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+    <3ef6>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
+    <3ef7>   DW_AT_sibling     : (ref4) <0x3f09>
+ <2><3efb>: Abbrev Number: 93 (DW_TAG_formal_parameter)
+    <3efc>   DW_AT_name        : (string) obj
+    <3f00>   DW_AT_decl_file   : (data1) 2
+    <3f01>   DW_AT_decl_line   : (data2) 616
+    <3f03>   DW_AT_decl_column : (data1) 46
+    <3f04>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3f08>: Abbrev Number: 0
+ <1><3f09>: Abbrev Number: 94 (DW_TAG_subprogram)
+    <3f0a>   DW_AT_name        : (strp) (offset: 0x5d): Py_XDECREF
+    <3f0e>   DW_AT_decl_file   : (data1) 2
+    <3f0f>   DW_AT_decl_line   : (data2) 599
+    <3f11>   DW_AT_decl_column : (data1) 20
+    <3f12>   DW_AT_prototyped  : (flag_present) 1
+    <3f12>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
+    <3f13>   DW_AT_sibling     : (ref4) <0x3f24>
+ <2><3f17>: Abbrev Number: 93 (DW_TAG_formal_parameter)
+    <3f18>   DW_AT_name        : (string) op
+    <3f1b>   DW_AT_decl_file   : (data1) 2
+    <3f1c>   DW_AT_decl_line   : (data2) 599
+    <3f1e>   DW_AT_decl_column : (data1) 41
+    <3f1f>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3f23>: Abbrev Number: 0
+ <1><3f24>: Abbrev Number: 94 (DW_TAG_subprogram)
+    <3f25>   DW_AT_name        : (strp) (offset: 0xa64): Py_DECREF
+    <3f29>   DW_AT_decl_file   : (data1) 2
+    <3f2a>   DW_AT_decl_line   : (data2) 533
+    <3f2c>   DW_AT_decl_column : (data1) 20
+    <3f2d>   DW_AT_prototyped  : (flag_present) 1
+    <3f2d>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
+    <3f2e>   DW_AT_sibling     : (ref4) <0x3f3f>
+ <2><3f32>: Abbrev Number: 93 (DW_TAG_formal_parameter)
+    <3f33>   DW_AT_name        : (string) op
+    <3f36>   DW_AT_decl_file   : (data1) 2
+    <3f37>   DW_AT_decl_line   : (data2) 533
+    <3f39>   DW_AT_decl_column : (data1) 40
+    <3f3a>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3f3e>: Abbrev Number: 0
+ <1><3f3f>: Abbrev Number: 94 (DW_TAG_subprogram)
+    <3f40>   DW_AT_name        : (strp) (offset: 0x1419): Py_INCREF
+    <3f44>   DW_AT_decl_file   : (data1) 2
+    <3f45>   DW_AT_decl_line   : (data2) 491
+    <3f47>   DW_AT_decl_column : (data1) 20
+    <3f48>   DW_AT_prototyped  : (flag_present) 1
+    <3f48>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
+    <3f49>   DW_AT_sibling     : (ref4) <0x3f5a>
+ <2><3f4d>: Abbrev Number: 93 (DW_TAG_formal_parameter)
+    <3f4e>   DW_AT_name        : (string) op
+    <3f51>   DW_AT_decl_file   : (data1) 2
+    <3f52>   DW_AT_decl_line   : (data2) 491
+    <3f54>   DW_AT_decl_column : (data1) 40
+    <3f55>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3f59>: Abbrev Number: 0
+ <1><3f5a>: Abbrev Number: 90 (DW_TAG_subprogram)
+    <3f5b>   DW_AT_name        : (strp) (offset: 0x1e58): PyObject_TypeCheck
+    <3f5f>   DW_AT_decl_file   : (data1) 2
+    <3f60>   DW_AT_decl_line   : (data2) 262
+    <3f62>   DW_AT_decl_column : (data1) 19
+    <3f63>   DW_AT_prototyped  : (flag_present) 1
+    <3f63>   DW_AT_type        : (ref4) <0x4f>, int
+    <3f67>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
+    <3f68>   DW_AT_sibling     : (ref4) <0x3f86>
+ <2><3f6c>: Abbrev Number: 93 (DW_TAG_formal_parameter)
+    <3f6d>   DW_AT_name        : (string) ob
+    <3f70>   DW_AT_decl_file   : (data1) 2
+    <3f71>   DW_AT_decl_line   : (data2) 262
+    <3f73>   DW_AT_decl_column : (data1) 48
+    <3f74>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3f78>: Abbrev Number: 91 (DW_TAG_formal_parameter)
+    <3f79>   DW_AT_name        : (strp) (offset: 0x2201): type
+    <3f7d>   DW_AT_decl_file   : (data1) 2
+    <3f7e>   DW_AT_decl_line   : (data2) 262
+    <3f80>   DW_AT_decl_column : (data1) 66
+    <3f81>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
+ <2><3f85>: Abbrev Number: 0
+ <1><3f86>: Abbrev Number: 84 (DW_TAG_subprogram)
+    <3f87>   DW_AT_name        : (strp) (offset: 0x41e): Py_IS_TYPE
+    <3f8b>   DW_AT_decl_file   : (data1) 2
+    <3f8c>   DW_AT_decl_line   : (data1) 149
+    <3f8d>   DW_AT_decl_column : (data1) 19
+    <3f8e>   DW_AT_prototyped  : (flag_present) 1
+    <3f8e>   DW_AT_type        : (ref4) <0x4f>, int
+    <3f92>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
+    <3f93>   DW_AT_sibling     : (ref4) <0x3faf>
+ <2><3f97>: Abbrev Number: 85 (DW_TAG_formal_parameter)
+    <3f98>   DW_AT_name        : (string) ob
+    <3f9b>   DW_AT_decl_file   : (data1) 2
+    <3f9c>   DW_AT_decl_line   : (data1) 149
+    <3f9d>   DW_AT_decl_column : (data1) 40
+    <3f9e>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3fa2>: Abbrev Number: 69 (DW_TAG_formal_parameter)
+    <3fa3>   DW_AT_name        : (strp) (offset: 0x2201): type
+    <3fa7>   DW_AT_decl_file   : (data1) 2
+    <3fa8>   DW_AT_decl_line   : (data1) 149
+    <3fa9>   DW_AT_decl_column : (data1) 58
+    <3faa>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
+ <2><3fae>: Abbrev Number: 0
+ <1><3faf>: Abbrev Number: 84 (DW_TAG_subprogram)
+    <3fb0>   DW_AT_name        : (strp) (offset: 0x2bd): Py_SIZE
+    <3fb4>   DW_AT_decl_file   : (data1) 2
+    <3fb5>   DW_AT_decl_line   : (data1) 140
+    <3fb6>   DW_AT_decl_column : (data1) 26
+    <3fb7>   DW_AT_prototyped  : (flag_present) 1
+    <3fb7>   DW_AT_type        : (ref4) <0x1ab>, Py_ssize_t, ssize_t, long int
+    <3fbb>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
+    <3fbc>   DW_AT_sibling     : (ref4) <0x3fd8>
+ <2><3fc0>: Abbrev Number: 85 (DW_TAG_formal_parameter)
+    <3fc1>   DW_AT_name        : (string) ob
+    <3fc4>   DW_AT_decl_file   : (data1) 2
+    <3fc5>   DW_AT_decl_line   : (data1) 140
+    <3fc6>   DW_AT_decl_column : (data1) 44
+    <3fc7>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3fcb>: Abbrev Number: 70 (DW_TAG_variable)
+    <3fcc>   DW_AT_name        : (strp) (offset: 0x1996): var_ob
+    <3fd0>   DW_AT_decl_file   : (data1) 2
+    <3fd1>   DW_AT_decl_line   : (data1) 141
+    <3fd2>   DW_AT_decl_column : (data1) 18
+    <3fd3>   DW_AT_type        : (ref4) <0x3fd8>, PyVarObject
+ <2><3fd7>: Abbrev Number: 0
+ <1><3fd8>: Abbrev Number: 10 (DW_TAG_pointer_type)
+    <3fd9>   DW_AT_byte_size   : (data1) 8
+    <3fda>   DW_AT_type        : (ref4) <0xba1>, PyVarObject
+ <1><3fde>: Abbrev Number: 84 (DW_TAG_subprogram)
+    <3fdf>   DW_AT_name        : (strp) (offset: 0x11b4): Py_TYPE
+    <3fe3>   DW_AT_decl_file   : (data1) 2
+    <3fe4>   DW_AT_decl_line   : (data1) 132
+    <3fe5>   DW_AT_decl_column : (data1) 29
+    <3fe6>   DW_AT_prototyped  : (flag_present) 1
+    <3fe6>   DW_AT_type        : (ref4) <0xb77>, PyTypeObject, _typeobject
+    <3fea>   DW_AT_inline      : (data1) 3	(declared as inline and inlined)
+    <3feb>   DW_AT_sibling     : (ref4) <0x3ffb>
+ <2><3fef>: Abbrev Number: 85 (DW_TAG_formal_parameter)
+    <3ff0>   DW_AT_name        : (string) ob
+    <3ff3>   DW_AT_decl_file   : (data1) 2
+    <3ff4>   DW_AT_decl_line   : (data1) 132
+    <3ff5>   DW_AT_decl_column : (data1) 47
+    <3ff6>   DW_AT_type        : (ref4) <0xb5a>, PyObject, _object
+ <2><3ffa>: Abbrev Number: 0
+ <1><3ffb>: Abbrev Number: 95 (DW_TAG_subprogram)
+    <3ffc>   DW_AT_abstract_origin: (ref4) <0x399f>
+    <4000>   DW_AT_low_pc      : (addr) 0x2b40
+    <4008>   DW_AT_high_pc     : (data8) 0x55
+    <4010>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
+    <4012>   DW_AT_GNU_all_call_sites: (flag_present) 1
+    <4012>   DW_AT_sibling     : (ref4) <0x40e3>
+ <2><4016>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <4017>   DW_AT_abstract_origin: (ref4) <0x39b0>
+    <401b>   DW_AT_location    : (sec_offset) 0x21df (location list)
+    <401f>   DW_AT_GNU_locviews: (sec_offset) 0x21d5
+ <2><4023>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <4024>   DW_AT_abstract_origin: (ref4) <0x39bc>
+    <4028>   DW_AT_location    : (sec_offset) 0x2260 (location list)
+    <402c>   DW_AT_GNU_locviews: (sec_offset) 0x2254
+ <2><4030>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <4031>   DW_AT_abstract_origin: (ref4) <0x39c8>
+    <4035>   DW_AT_location    : (sec_offset) 0x22f4 (location list)
+    <4039>   DW_AT_GNU_locviews: (sec_offset) 0x22e8
+ <2><403d>: Abbrev Number: 96 (DW_TAG_lexical_block)
+    <403e>   DW_AT_abstract_origin: (ref4) <0x39d4>
+    <4042>   DW_AT_ranges      : (sec_offset) 0x4d0
+    <4046>   DW_AT_sibling     : (ref4) <0x4058>
+ <3><404a>: Abbrev Number: 59 (DW_TAG_variable)
+    <404b>   DW_AT_abstract_origin: (ref4) <0x39d9>
+    <404f>   DW_AT_location    : (sec_offset) 0x237e (location list)
+    <4053>   DW_AT_GNU_locviews: (sec_offset) 0x237c
+ <3><4057>: Abbrev Number: 0
+ <2><4058>: Abbrev Number: 97 (DW_TAG_lexical_block)
+    <4059>   DW_AT_abstract_origin: (ref4) <0x39f9>
+    <405d>   DW_AT_low_pc      : (addr) 0x2b68
+    <4065>   DW_AT_high_pc     : (data8) 0x9
+    <406d>   DW_AT_sibling     : (ref4) <0x407f>
+ <3><4071>: Abbrev Number: 59 (DW_TAG_variable)
+    <4072>   DW_AT_abstract_origin: (ref4) <0x39fe>
+    <4076>   DW_AT_location    : (sec_offset) 0x23a3 (location list)
+    <407a>   DW_AT_GNU_locviews: (sec_offset) 0x23a1
+ <3><407e>: Abbrev Number: 0
+ <2><407f>: Abbrev Number: 83 (DW_TAG_inlined_subroutine)
+    <4080>   DW_AT_abstract_origin: (ref4) <0x399f>
+    <4084>   DW_AT_entry_pc    : (addr) 0x2b71
+    <408c>   DW_AT_GNU_entry_view: (data1) 1
+    <408d>   DW_AT_ranges      : (sec_offset) 0x500
+    <4091>   DW_AT_call_file   : (data1) 1
+    <4092>   DW_AT_call_line   : (data1) 139
+    <4093>   DW_AT_call_column : (data1) 1
+ <3><4094>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <4095>   DW_AT_abstract_origin: (ref4) <0x39c8>
+    <4099>   DW_AT_location    : (sec_offset) 0x23cc (location list)
+    <409d>   DW_AT_GNU_locviews: (sec_offset) 0x23c6
+ <3><40a1>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <40a2>   DW_AT_abstract_origin: (ref4) <0x39bc>
+    <40a6>   DW_AT_location    : (sec_offset) 0x241e (location list)
+    <40aa>   DW_AT_GNU_locviews: (sec_offset) 0x2418
+ <3><40ae>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <40af>   DW_AT_abstract_origin: (ref4) <0x39b0>
+    <40b3>   DW_AT_location    : (sec_offset) 0x246e (location list)
+    <40b7>   DW_AT_GNU_locviews: (sec_offset) 0x246a
+ <3><40bb>: Abbrev Number: 98 (DW_TAG_lexical_block)
+    <40bc>   DW_AT_abstract_origin: (ref4) <0x3a1b>
+    <40c0>   DW_AT_ranges      : (sec_offset) 0x540
+ <4><40c4>: Abbrev Number: 99 (DW_TAG_variable)
+    <40c5>   DW_AT_abstract_origin: (ref4) <0x3a1c>
+    <40c9>   DW_AT_location    : (exprloc) 1 byte block: 50 	(DW_OP_reg0 (rax))
+ <4><40cb>: Abbrev Number: 55 (DW_TAG_GNU_call_site)
+    <40cc>   DW_AT_low_pc      : (addr) 0x2b88
+    <40d4>   DW_AT_GNU_tail_call: (flag_present) 1
+    <40d4>   DW_AT_GNU_call_site_target: (exprloc) 3 byte block: f3 1 54 	(DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)))
+ <5><40d8>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <40d9>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <40db>   DW_AT_GNU_call_site_value: (exprloc) 3 byte block: f3 1 51 	(DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)))
+ <5><40df>: Abbrev Number: 0
+ <4><40e0>: Abbrev Number: 0
+ <3><40e1>: Abbrev Number: 0
+ <2><40e2>: Abbrev Number: 0
+ <1><40e3>: Abbrev Number: 95 (DW_TAG_subprogram)
+    <40e4>   DW_AT_abstract_origin: (ref4) <0x3238>
+    <40e8>   DW_AT_low_pc      : (addr) 0x2ba0
+    <40f0>   DW_AT_high_pc     : (data8) 0x8a
+    <40f8>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
+    <40fa>   DW_AT_GNU_all_call_sites: (flag_present) 1
+    <40fa>   DW_AT_sibling     : (ref4) <0x42c8>
+ <2><40fe>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <40ff>   DW_AT_abstract_origin: (ref4) <0x3249>
+    <4103>   DW_AT_location    : (sec_offset) 0x24b5 (location list)
+    <4107>   DW_AT_GNU_locviews: (sec_offset) 0x24a7
+ <2><410b>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <410c>   DW_AT_abstract_origin: (ref4) <0x3255>
+    <4110>   DW_AT_location    : (sec_offset) 0x255f (location list)
+    <4114>   DW_AT_GNU_locviews: (sec_offset) 0x2553
+ <2><4118>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <4119>   DW_AT_abstract_origin: (ref4) <0x3261>
+    <411d>   DW_AT_location    : (sec_offset) 0x25f6 (location list)
+    <4121>   DW_AT_GNU_locviews: (sec_offset) 0x25ea
+ <2><4125>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <4126>   DW_AT_abstract_origin: (ref4) <0x326d>
+    <412a>   DW_AT_location    : (sec_offset) 0x268d (location list)
+    <412e>   DW_AT_GNU_locviews: (sec_offset) 0x2681
+ <2><4132>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <4133>   DW_AT_abstract_origin: (ref4) <0x3279>
+    <4137>   DW_AT_location    : (sec_offset) 0x2724 (location list)
+    <413b>   DW_AT_GNU_locviews: (sec_offset) 0x2718
+ <2><413f>: Abbrev Number: 59 (DW_TAG_variable)
+    <4140>   DW_AT_abstract_origin: (ref4) <0x3285>
+    <4144>   DW_AT_location    : (sec_offset) 0x27b1 (location list)
+    <4148>   DW_AT_GNU_locviews: (sec_offset) 0x27af
+ <2><414c>: Abbrev Number: 59 (DW_TAG_variable)
+    <414d>   DW_AT_abstract_origin: (ref4) <0x3291>
+    <4151>   DW_AT_location    : (sec_offset) 0x27da (location list)
+    <4155>   DW_AT_GNU_locviews: (sec_offset) 0x27d4
+ <2><4159>: Abbrev Number: 59 (DW_TAG_variable)
+    <415a>   DW_AT_abstract_origin: (ref4) <0x329d>
+    <415e>   DW_AT_location    : (sec_offset) 0x2828 (location list)
+    <4162>   DW_AT_GNU_locviews: (sec_offset) 0x2824
+ <2><4166>: Abbrev Number: 97 (DW_TAG_lexical_block)
+    <4167>   DW_AT_abstract_origin: (ref4) <0x32a9>
+    <416b>   DW_AT_low_pc      : (addr) 0x2bb6
+    <4173>   DW_AT_high_pc     : (data8) 0x33
+    <417b>   DW_AT_sibling     : (ref4) <0x420e>
+ <3><417f>: Abbrev Number: 59 (DW_TAG_variable)
+    <4180>   DW_AT_abstract_origin: (ref4) <0x32aa>
+    <4184>   DW_AT_location    : (sec_offset) 0x2861 (location list)
+    <4188>   DW_AT_GNU_locviews: (sec_offset) 0x285f
+ <3><418c>: Abbrev Number: 77 (DW_TAG_inlined_subroutine)
+    <418d>   DW_AT_abstract_origin: (ref4) <0x3f3f>
+    <4191>   DW_AT_entry_pc    : (addr) 0x2bd4
+    <4199>   DW_AT_GNU_entry_view: (data1) 1
+    <419a>   DW_AT_low_pc      : (addr) 0x2bd4
+    <41a2>   DW_AT_high_pc     : (data8) 0x8
+    <41aa>   DW_AT_call_file   : (data1) 1
+    <41ab>   DW_AT_call_line   : (data1) 248
+    <41ac>   DW_AT_call_column : (data1) 9
+    <41ad>   DW_AT_sibling     : (ref4) <0x41bf>
+ <4><41b1>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <41b2>   DW_AT_abstract_origin: (ref4) <0x3f4d>
+    <41b6>   DW_AT_location    : (sec_offset) 0x2887 (location list)
+    <41ba>   DW_AT_GNU_locviews: (sec_offset) 0x2885
+ <4><41be>: Abbrev Number: 0
+ <3><41bf>: Abbrev Number: 78 (DW_TAG_inlined_subroutine)
+    <41c0>   DW_AT_abstract_origin: (ref4) <0x3dd7>
+    <41c4>   DW_AT_entry_pc    : (addr) 0x2bdc
+    <41cc>   DW_AT_GNU_entry_view: (data1) 1
+    <41cd>   DW_AT_low_pc      : (addr) 0x2bdc
+    <41d5>   DW_AT_high_pc     : (data8) 0x4
+    <41dd>   DW_AT_call_file   : (data1) 1
+    <41de>   DW_AT_call_line   : (data1) 249
+    <41df>   DW_AT_call_column : (data1) 9
+ <4><41e0>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <41e1>   DW_AT_abstract_origin: (ref4) <0x3dfb>
+    <41e5>   DW_AT_location    : (sec_offset) 0x28ac (location list)
+    <41e9>   DW_AT_GNU_locviews: (sec_offset) 0x28aa
+ <4><41ed>: Abbrev Number: 62 (DW_TAG_formal_parameter)
+    <41ee>   DW_AT_abstract_origin: (ref4) <0x3def>
+ <4><41f2>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <41f3>   DW_AT_abstract_origin: (ref4) <0x3de4>
+    <41f7>   DW_AT_location    : (sec_offset) 0x28d1 (location list)
+    <41fb>   DW_AT_GNU_locviews: (sec_offset) 0x28cf
+ <4><41ff>: Abbrev Number: 59 (DW_TAG_variable)
+    <4200>   DW_AT_abstract_origin: (ref4) <0x3e07>
+    <4204>   DW_AT_location    : (sec_offset) 0x28f6 (location list)
+    <4208>   DW_AT_GNU_locviews: (sec_offset) 0x28f4
+ <4><420c>: Abbrev Number: 0
+ <3><420d>: Abbrev Number: 0
+ <2><420e>: Abbrev Number: 77 (DW_TAG_inlined_subroutine)
+    <420f>   DW_AT_abstract_origin: (ref4) <0x3238>
+    <4213>   DW_AT_entry_pc    : (addr) 0x2c10
+    <421b>   DW_AT_GNU_entry_view: (data1) 0
+    <421c>   DW_AT_low_pc      : (addr) 0x2c10
+    <4224>   DW_AT_high_pc     : (data8) 0x18
+    <422c>   DW_AT_call_file   : (data1) 1
+    <422d>   DW_AT_call_line   : (data1) 232
+    <422e>   DW_AT_call_column : (data1) 1
+    <422f>   DW_AT_sibling     : (ref4) <0x429f>
+ <3><4233>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <4234>   DW_AT_abstract_origin: (ref4) <0x3249>
+    <4238>   DW_AT_location    : (sec_offset) 0x291d (location list)
+    <423c>   DW_AT_GNU_locviews: (sec_offset) 0x2919
+ <3><4240>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <4241>   DW_AT_abstract_origin: (ref4) <0x3255>
+    <4245>   DW_AT_location    : (sec_offset) 0x295a (location list)
+    <4249>   DW_AT_GNU_locviews: (sec_offset) 0x2956
+ <3><424d>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <424e>   DW_AT_abstract_origin: (ref4) <0x3261>
+    <4252>   DW_AT_location    : (sec_offset) 0x2997 (location list)
+    <4256>   DW_AT_GNU_locviews: (sec_offset) 0x2993
+ <3><425a>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <425b>   DW_AT_abstract_origin: (ref4) <0x326d>
+    <425f>   DW_AT_location    : (sec_offset) 0x29d4 (location list)
+    <4263>   DW_AT_GNU_locviews: (sec_offset) 0x29d0
+ <3><4267>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <4268>   DW_AT_abstract_origin: (ref4) <0x3279>
+    <426c>   DW_AT_location    : (sec_offset) 0x2a11 (location list)
+    <4270>   DW_AT_GNU_locviews: (sec_offset) 0x2a0d
+ <3><4274>: Abbrev Number: 100 (DW_TAG_variable)
+    <4275>   DW_AT_abstract_origin: (ref4) <0x3285>
+ <3><4279>: Abbrev Number: 100 (DW_TAG_variable)
+    <427a>   DW_AT_abstract_origin: (ref4) <0x3291>
+ <3><427e>: Abbrev Number: 100 (DW_TAG_variable)
+    <427f>   DW_AT_abstract_origin: (ref4) <0x329d>
+ <3><4283>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
+    <4284>   DW_AT_low_pc      : (addr) 0x2c26
+    <428c>   DW_AT_abstract_origin: (ref4) <0x454f>
+ <4><4290>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <4291>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <4293>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 20 30 0 0 0 0 0 0 	(DW_OP_addr: 3020)
+ <4><429d>: Abbrev Number: 0
+ <3><429e>: Abbrev Number: 0
+ <2><429f>: Abbrev Number: 49 (DW_TAG_GNU_call_site)
+    <42a0>   DW_AT_low_pc      : (addr) 0x2bb6
+    <42a8>   DW_AT_abstract_origin: (ref4) <0x45b2>
+ <2><42ac>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
+    <42ad>   DW_AT_low_pc      : (addr) 0x2c06
+    <42b5>   DW_AT_abstract_origin: (ref4) <0x454f>
+ <3><42b9>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <42ba>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <42bc>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 38 30 0 0 0 0 0 0 	(DW_OP_addr: 3038)
+ <3><42c6>: Abbrev Number: 0
+ <2><42c7>: Abbrev Number: 0
+ <1><42c8>: Abbrev Number: 95 (DW_TAG_subprogram)
+    <42c9>   DW_AT_abstract_origin: (ref4) <0x3cab>
+    <42cd>   DW_AT_low_pc      : (addr) 0x2c30
+    <42d5>   DW_AT_high_pc     : (data8) 0x70
+    <42dd>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
+    <42df>   DW_AT_GNU_all_call_sites: (flag_present) 1
+    <42df>   DW_AT_sibling     : (ref4) <0x4409>
+ <2><42e3>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <42e4>   DW_AT_abstract_origin: (ref4) <0x3cbc>
+    <42e8>   DW_AT_location    : (sec_offset) 0x2a54 (location list)
+    <42ec>   DW_AT_GNU_locviews: (sec_offset) 0x2a4a
+ <2><42f0>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <42f1>   DW_AT_abstract_origin: (ref4) <0x3cc8>
+    <42f5>   DW_AT_location    : (sec_offset) 0x2acd (location list)
+    <42f9>   DW_AT_GNU_locviews: (sec_offset) 0x2ac9
+ <2><42fd>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <42fe>   DW_AT_abstract_origin: (ref4) <0x3cd4>
+    <4302>   DW_AT_location    : (sec_offset) 0x2b10 (location list)
+    <4306>   DW_AT_GNU_locviews: (sec_offset) 0x2b06
+ <2><430a>: Abbrev Number: 59 (DW_TAG_variable)
+    <430b>   DW_AT_abstract_origin: (ref4) <0x3ce0>
+    <430f>   DW_AT_location    : (sec_offset) 0x2b87 (location list)
+    <4313>   DW_AT_GNU_locviews: (sec_offset) 0x2b85
+ <2><4317>: Abbrev Number: 59 (DW_TAG_variable)
+    <4318>   DW_AT_abstract_origin: (ref4) <0x3cec>
+    <431c>   DW_AT_location    : (sec_offset) 0x2bac (location list)
+    <4320>   DW_AT_GNU_locviews: (sec_offset) 0x2baa
+ <2><4324>: Abbrev Number: 77 (DW_TAG_inlined_subroutine)
+    <4325>   DW_AT_abstract_origin: (ref4) <0x3f3f>
+    <4329>   DW_AT_entry_pc    : (addr) 0x2c6d
+    <4331>   DW_AT_GNU_entry_view: (data1) 1
+    <4332>   DW_AT_low_pc      : (addr) 0x2c6d
+    <433a>   DW_AT_high_pc     : (data8) 0x4
+    <4342>   DW_AT_call_file   : (data1) 1
+    <4343>   DW_AT_call_line   : (data1) 72
+    <4344>   DW_AT_call_column : (data1) 5
+    <4345>   DW_AT_sibling     : (ref4) <0x4357>
+ <3><4349>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <434a>   DW_AT_abstract_origin: (ref4) <0x3f4d>
+    <434e>   DW_AT_location    : (sec_offset) 0x2bd1 (location list)
+    <4352>   DW_AT_GNU_locviews: (sec_offset) 0x2bcf
+ <3><4356>: Abbrev Number: 0
+ <2><4357>: Abbrev Number: 75 (DW_TAG_inlined_subroutine)
+    <4358>   DW_AT_abstract_origin: (ref4) <0x3cab>
+    <435c>   DW_AT_entry_pc    : (addr) 0x2c80
+    <4364>   DW_AT_GNU_entry_view: (data1) 0
+    <4365>   DW_AT_ranges      : (sec_offset) 0x580
+    <4369>   DW_AT_call_file   : (data1) 1
+    <436a>   DW_AT_call_line   : (data1) 61
+    <436b>   DW_AT_call_column : (data1) 1
+    <436c>   DW_AT_sibling     : (ref4) <0x43c3>
+ <3><4370>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <4371>   DW_AT_abstract_origin: (ref4) <0x3cbc>
+    <4375>   DW_AT_location    : (sec_offset) 0x2bf6 (location list)
+    <4379>   DW_AT_GNU_locviews: (sec_offset) 0x2bf4
+ <3><437d>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <437e>   DW_AT_abstract_origin: (ref4) <0x3cc8>
+    <4382>   DW_AT_location    : (sec_offset) 0x2c1b (location list)
+    <4386>   DW_AT_GNU_locviews: (sec_offset) 0x2c19
+ <3><438a>: Abbrev Number: 48 (DW_TAG_formal_parameter)
+    <438b>   DW_AT_abstract_origin: (ref4) <0x3cd4>
+    <438f>   DW_AT_location    : (sec_offset) 0x2c43 (location list)
+    <4393>   DW_AT_GNU_locviews: (sec_offset) 0x2c41
+ <3><4397>: Abbrev Number: 58 (DW_TAG_lexical_block)
+    <4398>   DW_AT_ranges      : (sec_offset) 0x580
+ <4><439c>: Abbrev Number: 100 (DW_TAG_variable)
+    <439d>   DW_AT_abstract_origin: (ref4) <0x3ce0>
+ <4><43a1>: Abbrev Number: 100 (DW_TAG_variable)
+    <43a2>   DW_AT_abstract_origin: (ref4) <0x3cec>
+ <4><43a6>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
+    <43a7>   DW_AT_low_pc      : (addr) 0x2c96
+    <43af>   DW_AT_abstract_origin: (ref4) <0x454f>
+ <5><43b3>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <43b4>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
+    <43b6>   DW_AT_GNU_call_site_value: (exprloc) 9 byte block: 3 52 30 0 0 0 0 0 0 	(DW_OP_addr: 3052)
+ <5><43c0>: Abbrev Number: 0
+ <4><43c1>: Abbrev Number: 0
+ <3><43c2>: Abbrev Number: 0
+ <2><43c3>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <43c4>   DW_AT_low_pc      : (addr) 0x2c45
+    <43cc>   DW_AT_abstract_origin: (ref4) <0x45be>
+    <43d0>   DW_AT_sibling     : (ref4) <0x43dc>
+ <3><43d4>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <43d5>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <43d7>   DW_AT_GNU_call_site_value: (exprloc) 3 byte block: f3 1 54 	(DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)))
+ <3><43db>: Abbrev Number: 0
+ <2><43dc>: Abbrev Number: 60 (DW_TAG_GNU_call_site)
+    <43dd>   DW_AT_low_pc      : (addr) 0x2c57
+    <43e5>   DW_AT_abstract_origin: (ref4) <0x45ca>
+    <43e9>   DW_AT_sibling     : (ref4) <0x43f4>
+ <3><43ed>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <43ee>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <43f0>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 76 0 	(DW_OP_breg6 (rbp): 0)
+ <3><43f3>: Abbrev Number: 0
+ <2><43f4>: Abbrev Number: 50 (DW_TAG_GNU_call_site)
+    <43f5>   DW_AT_low_pc      : (addr) 0x2c64
+    <43fd>   DW_AT_abstract_origin: (ref4) <0x4477>
+ <3><4401>: Abbrev Number: 42 (DW_TAG_GNU_call_site_parameter)
+    <4402>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
+    <4404>   DW_AT_GNU_call_site_value: (exprloc) 2 byte block: 7c 0 	(DW_OP_breg12 (r12): 0)
+ <3><4407>: Abbrev Number: 0
+ <2><4408>: Abbrev Number: 0
+ <1><4409>: Abbrev Number: 101 (DW_TAG_subprogram)
+    <440a>   DW_AT_external    : (flag_present) 1
+    <440a>   DW_AT_declaration : (flag_present) 1
+    <440a>   DW_AT_linkage_name: (strp) (offset: 0x18fd): PyModuleDef_Init
+    <440e>   DW_AT_name        : (strp) (offset: 0x18fd): PyModuleDef_Init
+    <4412>   DW_AT_decl_file   : (data1) 12
+    <4413>   DW_AT_decl_line   : (data1) 40
+    <4414>   DW_AT_decl_column : (data1) 24
+ <1><4415>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <4416>   DW_AT_external    : (flag_present) 1
+    <4416>   DW_AT_declaration : (flag_present) 1
+    <4416>   DW_AT_linkage_name: (strp) (offset: 0x2499): _Py_Dealloc
+    <441a>   DW_AT_name        : (strp) (offset: 0x2499): _Py_Dealloc
+    <441e>   DW_AT_decl_file   : (data1) 2
+    <441f>   DW_AT_decl_line   : (data2) 477
+    <4421>   DW_AT_decl_column : (data1) 18
+ <1><4422>: Abbrev Number: 101 (DW_TAG_subprogram)
+    <4423>   DW_AT_external    : (flag_present) 1
+    <4423>   DW_AT_declaration : (flag_present) 1
+    <4423>   DW_AT_linkage_name: (strp) (offset: 0x1494): PyModule_GetState
+    <4427>   DW_AT_name        : (strp) (offset: 0x1494): PyModule_GetState
+    <442b>   DW_AT_decl_file   : (data1) 12
+    <442c>   DW_AT_decl_line   : (data1) 36
+    <442d>   DW_AT_decl_column : (data1) 19
+ <1><442e>: Abbrev Number: 101 (DW_TAG_subprogram)
+    <442f>   DW_AT_external    : (flag_present) 1
+    <442f>   DW_AT_declaration : (flag_present) 1
+    <442f>   DW_AT_linkage_name: (strp) (offset: 0x11d2): PyType_FromModuleAndSpec
+    <4433>   DW_AT_name        : (strp) (offset: 0x11d2): PyType_FromModuleAndSpec
+    <4437>   DW_AT_decl_file   : (data1) 2
+    <4438>   DW_AT_decl_line   : (data1) 250
+    <4439>   DW_AT_decl_column : (data1) 23
+ <1><443a>: Abbrev Number: 101 (DW_TAG_subprogram)
+    <443b>   DW_AT_external    : (flag_present) 1
+    <443b>   DW_AT_declaration : (flag_present) 1
+    <443b>   DW_AT_linkage_name: (strp) (offset: 0x1e6): PyModule_AddType
+    <443f>   DW_AT_name        : (strp) (offset: 0x1e6): PyModule_AddType
+    <4443>   DW_AT_decl_file   : (data1) 69
+    <4444>   DW_AT_decl_line   : (data1) 58
+    <4445>   DW_AT_decl_column : (data1) 17
+ <1><4446>: Abbrev Number: 101 (DW_TAG_subprogram)
+    <4447>   DW_AT_external    : (flag_present) 1
+    <4447>   DW_AT_declaration : (flag_present) 1
+    <4447>   DW_AT_linkage_name: (strp) (offset: 0xea5): PyTuple_New
+    <444b>   DW_AT_name        : (strp) (offset: 0xea5): PyTuple_New
+    <444f>   DW_AT_decl_file   : (data1) 35
+    <4450>   DW_AT_decl_line   : (data1) 30
+    <4451>   DW_AT_decl_column : (data1) 24
+ <1><4452>: Abbrev Number: 101 (DW_TAG_subprogram)
+    <4453>   DW_AT_external    : (flag_present) 1
+    <4453>   DW_AT_declaration : (flag_present) 1
+    <4453>   DW_AT_linkage_name: (strp) (offset: 0xb4a): PyUnicode_FromString
+    <4457>   DW_AT_name        : (strp) (offset: 0xb4a): PyUnicode_FromString
+    <445b>   DW_AT_decl_file   : (data1) 27
+    <445c>   DW_AT_decl_line   : (data1) 137
+    <445d>   DW_AT_decl_column : (data1) 23
+ <1><445e>: Abbrev Number: 101 (DW_TAG_subprogram)
+    <445f>   DW_AT_external    : (flag_present) 1
+    <445f>   DW_AT_declaration : (flag_present) 1
+    <445f>   DW_AT_linkage_name: (strp) (offset: 0x22c9): PyDict_SetItemString
+    <4463>   DW_AT_name        : (strp) (offset: 0x22c9): PyDict_SetItemString
+    <4467>   DW_AT_decl_file   : (data1) 37
+    <4468>   DW_AT_decl_line   : (data1) 58
+    <4469>   DW_AT_decl_column : (data1) 17
+ <1><446a>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <446b>   DW_AT_external    : (flag_present) 1
+    <446b>   DW_AT_declaration : (flag_present) 1
+    <446b>   DW_AT_linkage_name: (strp) (offset: 0x1423): PyObject_RichCompareBool
+    <446f>   DW_AT_name        : (strp) (offset: 0x1423): PyObject_RichCompareBool
+    <4473>   DW_AT_decl_file   : (data1) 2
+    <4474>   DW_AT_decl_line   : (data2) 288
+    <4476>   DW_AT_decl_column : (data1) 17
+ <1><4477>: Abbrev Number: 101 (DW_TAG_subprogram)
+    <4478>   DW_AT_external    : (flag_present) 1
+    <4478>   DW_AT_declaration : (flag_present) 1
+    <4478>   DW_AT_linkage_name: (strp) (offset: 0x1cbe): PyType_GetModuleState
+    <447c>   DW_AT_name        : (strp) (offset: 0x1cbe): PyType_GetModuleState
+    <4480>   DW_AT_decl_file   : (data1) 2
+    <4481>   DW_AT_decl_line   : (data1) 252
+    <4482>   DW_AT_decl_column : (data1) 20
+ <1><4483>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <4484>   DW_AT_external    : (flag_present) 1
+    <4484>   DW_AT_declaration : (flag_present) 1
+    <4484>   DW_AT_linkage_name: (strp) (offset: 0x2a8): PyObject_RichCompare
+    <4488>   DW_AT_name        : (strp) (offset: 0x2a8): PyObject_RichCompare
+    <448c>   DW_AT_decl_file   : (data1) 2
+    <448d>   DW_AT_decl_line   : (data2) 287
+    <448f>   DW_AT_decl_column : (data1) 24
+ <1><4490>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <4491>   DW_AT_external    : (flag_present) 1
+    <4491>   DW_AT_declaration : (flag_present) 1
+    <4491>   DW_AT_linkage_name: (strp) (offset: 0x1707): PyType_GetModuleByDef
+    <4495>   DW_AT_name        : (strp) (offset: 0x1707): PyType_GetModuleByDef
+    <4499>   DW_AT_decl_file   : (data1) 18
+    <449a>   DW_AT_decl_line   : (data2) 273
+    <449c>   DW_AT_decl_column : (data1) 24
+ <1><449d>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <449e>   DW_AT_external    : (flag_present) 1
+    <449e>   DW_AT_declaration : (flag_present) 1
+    <449e>   DW_AT_linkage_name: (strp) (offset: 0x916): Py_ReprEnter
+    <44a2>   DW_AT_name        : (strp) (offset: 0x916): Py_ReprEnter
+    <44a6>   DW_AT_decl_file   : (data1) 2
+    <44a7>   DW_AT_decl_line   : (data2) 322
+    <44a9>   DW_AT_decl_column : (data1) 17
+ <1><44aa>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <44ab>   DW_AT_external    : (flag_present) 1
+    <44ab>   DW_AT_declaration : (flag_present) 1
+    <44ab>   DW_AT_linkage_name: (strp) (offset: 0xb1): _PyUnicodeWriter_Init
+    <44af>   DW_AT_name        : (strp) (offset: 0xb1): _PyUnicodeWriter_Init
+    <44b3>   DW_AT_decl_file   : (data1) 28
+    <44b4>   DW_AT_decl_line   : (data2) 746
+    <44b6>   DW_AT_decl_column : (data1) 1
+ <1><44b7>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <44b8>   DW_AT_external    : (flag_present) 1
+    <44b8>   DW_AT_declaration : (flag_present) 1
+    <44b8>   DW_AT_linkage_name: (strp) (offset: 0x22de): _PyUnicodeWriter_WriteChar
+    <44bc>   DW_AT_name        : (strp) (offset: 0x22de): _PyUnicodeWriter_WriteChar
+    <44c0>   DW_AT_decl_file   : (data1) 28
+    <44c1>   DW_AT_decl_line   : (data2) 786
+    <44c3>   DW_AT_decl_column : (data1) 1
+ <1><44c4>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <44c5>   DW_AT_external    : (flag_present) 1
+    <44c5>   DW_AT_declaration : (flag_present) 1
+    <44c5>   DW_AT_linkage_name: (strp) (offset: 0x1780): PyObject_Repr
+    <44c9>   DW_AT_name        : (strp) (offset: 0x1780): PyObject_Repr
+    <44cd>   DW_AT_decl_file   : (data1) 2
+    <44ce>   DW_AT_decl_line   : (data2) 283
+    <44d0>   DW_AT_decl_column : (data1) 24
+ <1><44d1>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <44d2>   DW_AT_external    : (flag_present) 1
+    <44d2>   DW_AT_declaration : (flag_present) 1
+    <44d2>   DW_AT_linkage_name: (strp) (offset: 0x14f3): _PyUnicodeWriter_WriteStr
+    <44d6>   DW_AT_name        : (strp) (offset: 0x14f3): _PyUnicodeWriter_WriteStr
+    <44da>   DW_AT_decl_file   : (data1) 28
+    <44db>   DW_AT_decl_line   : (data2) 793
+    <44dd>   DW_AT_decl_column : (data1) 1
+ <1><44de>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <44df>   DW_AT_external    : (flag_present) 1
+    <44df>   DW_AT_declaration : (flag_present) 1
+    <44df>   DW_AT_linkage_name: (strp) (offset: 0x20c2): _PyUnicodeWriter_Dealloc
+    <44e3>   DW_AT_name        : (strp) (offset: 0x20c2): _PyUnicodeWriter_Dealloc
+    <44e7>   DW_AT_decl_file   : (data1) 28
+    <44e8>   DW_AT_decl_line   : (data2) 830
+    <44ea>   DW_AT_decl_column : (data1) 1
+ <1><44eb>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <44ec>   DW_AT_external    : (flag_present) 1
+    <44ec>   DW_AT_declaration : (flag_present) 1
+    <44ec>   DW_AT_linkage_name: (strp) (offset: 0xf4c): Py_ReprLeave
+    <44f0>   DW_AT_name        : (strp) (offset: 0xf4c): Py_ReprLeave
+    <44f4>   DW_AT_decl_file   : (data1) 2
+    <44f5>   DW_AT_decl_line   : (data2) 323
+    <44f7>   DW_AT_decl_column : (data1) 18
+ <1><44f8>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <44f9>   DW_AT_external    : (flag_present) 1
+    <44f9>   DW_AT_declaration : (flag_present) 1
+    <44f9>   DW_AT_linkage_name: (strp) (offset: 0x6a5): PyUnicode_FromFormat
+    <44fd>   DW_AT_name        : (strp) (offset: 0x6a5): PyUnicode_FromFormat
+    <4501>   DW_AT_decl_file   : (data1) 27
+    <4502>   DW_AT_decl_line   : (data2) 258
+    <4504>   DW_AT_decl_column : (data1) 24
+ <1><4505>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <4506>   DW_AT_external    : (flag_present) 1
+    <4506>   DW_AT_declaration : (flag_present) 1
+    <4506>   DW_AT_linkage_name: (strp) (offset: 0x12e2): _PyUnicodeWriter_WriteASCIIString
+    <450a>   DW_AT_name        : (strp) (offset: 0x12e2): _PyUnicodeWriter_WriteASCIIString
+    <450e>   DW_AT_decl_file   : (data1) 28
+    <450f>   DW_AT_decl_line   : (data2) 809
+    <4511>   DW_AT_decl_column : (data1) 1
+ <1><4512>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <4513>   DW_AT_external    : (flag_present) 1
+    <4513>   DW_AT_declaration : (flag_present) 1
+    <4513>   DW_AT_linkage_name: (strp) (offset: 0x1d32): _PyUnicodeWriter_Finish
+    <4517>   DW_AT_name        : (strp) (offset: 0x1d32): _PyUnicodeWriter_Finish
+    <451b>   DW_AT_decl_file   : (data1) 28
+    <451c>   DW_AT_decl_line   : (data2) 826
+    <451e>   DW_AT_decl_column : (data1) 1
+ <1><451f>: Abbrev Number: 103 (DW_TAG_subprogram)
+    <4520>   DW_AT_external    : (flag_present) 1
+    <4520>   DW_AT_declaration : (flag_present) 1
+    <4520>   DW_AT_linkage_name: (strp) (offset: 0x126a): __stack_chk_fail
+    <4524>   DW_AT_name        : (strp) (offset: 0x126a): __stack_chk_fail
+ <1><4528>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <4529>   DW_AT_external    : (flag_present) 1
+    <4529>   DW_AT_declaration : (flag_present) 1
+    <4529>   DW_AT_linkage_name: (strp) (offset: 0x9f6): PyType_IsSubtype
+    <452d>   DW_AT_name        : (strp) (offset: 0x9f6): PyType_IsSubtype
+    <4531>   DW_AT_decl_file   : (data1) 2
+    <4532>   DW_AT_decl_line   : (data2) 260
+    <4534>   DW_AT_decl_column : (data1) 17
+ <1><4535>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <4536>   DW_AT_external    : (flag_present) 1
+    <4536>   DW_AT_declaration : (flag_present) 1
+    <4536>   DW_AT_linkage_name: (strp) (offset: 0x1697): PySequence_Tuple
+    <453a>   DW_AT_name        : (strp) (offset: 0x1697): PySequence_Tuple
+    <453e>   DW_AT_decl_file   : (data1) 70
+    <453f>   DW_AT_decl_line   : (data2) 702
+    <4541>   DW_AT_decl_column : (data1) 24
+ <1><4542>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <4543>   DW_AT_external    : (flag_present) 1
+    <4543>   DW_AT_declaration : (flag_present) 1
+    <4543>   DW_AT_linkage_name: (strp) (offset: 0xc95): PySequence_Fast
+    <4547>   DW_AT_name        : (strp) (offset: 0xc95): PySequence_Fast
+    <454b>   DW_AT_decl_file   : (data1) 70
+    <454c>   DW_AT_decl_line   : (data2) 715
+    <454e>   DW_AT_decl_column : (data1) 24
+ <1><454f>: Abbrev Number: 101 (DW_TAG_subprogram)
+    <4550>   DW_AT_external    : (flag_present) 1
+    <4550>   DW_AT_declaration : (flag_present) 1
+    <4550>   DW_AT_linkage_name: (strp) (offset: 0x2427): PyErr_SetString
+    <4554>   DW_AT_name        : (strp) (offset: 0x2427): PyErr_SetString
+    <4558>   DW_AT_decl_file   : (data1) 60
+    <4559>   DW_AT_decl_line   : (data1) 13
+    <455a>   DW_AT_decl_column : (data1) 18
+ <1><455b>: Abbrev Number: 101 (DW_TAG_subprogram)
+    <455c>   DW_AT_external    : (flag_present) 1
+    <455c>   DW_AT_declaration : (flag_present) 1
+    <455c>   DW_AT_linkage_name: (strp) (offset: 0x1009): PyObject_CallFunctionObjArgs
+    <4560>   DW_AT_name        : (strp) (offset: 0x1009): PyObject_CallFunctionObjArgs
+    <4564>   DW_AT_decl_file   : (data1) 70
+    <4565>   DW_AT_decl_line   : (data1) 215
+    <4566>   DW_AT_decl_column : (data1) 24
+ <1><4567>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <4568>   DW_AT_external    : (flag_present) 1
+    <4568>   DW_AT_declaration : (flag_present) 1
+    <4568>   DW_AT_linkage_name: (strp) (offset: 0x1179): _PyTrash_cond
+    <456c>   DW_AT_name        : (strp) (offset: 0x1179): _PyTrash_cond
+    <4570>   DW_AT_decl_file   : (data1) 18
+    <4571>   DW_AT_decl_line   : (data2) 475
+    <4573>   DW_AT_decl_column : (data1) 17
+ <1><4574>: Abbrev Number: 101 (DW_TAG_subprogram)
+    <4575>   DW_AT_external    : (flag_present) 1
+    <4575>   DW_AT_declaration : (flag_present) 1
+    <4575>   DW_AT_linkage_name: (strp) (offset: 0x1a4f): PyThreadState_Get
+    <4579>   DW_AT_name        : (strp) (offset: 0x1a4f): PyThreadState_Get
+    <457d>   DW_AT_decl_file   : (data1) 71
+    <457e>   DW_AT_decl_line   : (data1) 60
+    <457f>   DW_AT_decl_column : (data1) 29
+ <1><4580>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <4581>   DW_AT_external    : (flag_present) 1
+    <4581>   DW_AT_declaration : (flag_present) 1
+    <4581>   DW_AT_linkage_name: (strp) (offset: 0x23bd): _PyTrash_begin
+    <4585>   DW_AT_name        : (strp) (offset: 0x23bd): _PyTrash_begin
+    <4589>   DW_AT_decl_file   : (data1) 18
+    <458a>   DW_AT_decl_line   : (data2) 472
+    <458c>   DW_AT_decl_column : (data1) 17
+ <1><458d>: Abbrev Number: 102 (DW_TAG_subprogram)
+    <458e>   DW_AT_external    : (flag_present) 1
+    <458e>   DW_AT_declaration : (flag_present) 1
+    <458e>   DW_AT_linkage_name: (strp) (offset: 0xa38): _PyTrash_end
+    <4592>   DW_AT_name        : (strp) (offset: 0xa38): _PyTrash_end
+    <4596>   DW_AT_decl_file   : (data1) 18
+    <4597>   DW_AT_decl_line   : (data2) 473
+    <4599>   DW_AT_decl_column : (data1) 18
+ <1><459a>: Abbrev Number: 101 (DW_TAG_subprogram)
+    <459b>   DW_AT_external    : (flag_present) 1
+    <459b>   DW_AT_declaration : (flag_present) 1
+    <459b>   DW_AT_linkage_name: (strp) (offset: 0x804): PyObject_GC_UnTrack
+    <459f>   DW_AT_name        : (strp) (offset: 0x804): PyObject_GC_UnTrack
+    <45a3>   DW_AT_decl_file   : (data1) 72
+    <45a4>   DW_AT_decl_line   : (data1) 180
+    <45a5>   DW_AT_decl_column : (data1) 18
+ <1><45a6>: Abbrev Number: 101 (DW_TAG_subprogram)
+    <45a7>   DW_AT_external    : (flag_present) 1
+    <45a7>   DW_AT_declaration : (flag_present) 1
+    <45a7>   DW_AT_linkage_name: (strp) (offset: 0x1afe): _PyArg_ParseTupleAndKeywords_SizeT
+    <45ab>   DW_AT_name        : (strp) (offset: 0x1afe): _PyArg_ParseTupleAndKeywords_SizeT
+    <45af>   DW_AT_decl_file   : (data1) 69
+    <45b0>   DW_AT_decl_line   : (data1) 28
+    <45b1>   DW_AT_decl_column : (data1) 17
+ <1><45b2>: Abbrev Number: 101 (DW_TAG_subprogram)
+    <45b3>   DW_AT_external    : (flag_present) 1
+    <45b3>   DW_AT_declaration : (flag_present) 1
+    <45b3>   DW_AT_linkage_name: (strp) (offset: 0xc8a): PyList_New
+    <45b7>   DW_AT_name        : (strp) (offset: 0xc8a): PyList_New
+    <45bb>   DW_AT_decl_file   : (data1) 36
+    <45bc>   DW_AT_decl_line   : (data1) 28
+    <45bd>   DW_AT_decl_column : (data1) 24
+ <1><45be>: Abbrev Number: 101 (DW_TAG_subprogram)
+    <45bf>   DW_AT_external    : (flag_present) 1
+    <45bf>   DW_AT_declaration : (flag_present) 1
+    <45bf>   DW_AT_linkage_name: (strp) (offset: 0x24b3): PyTuple_Size
+    <45c3>   DW_AT_name        : (strp) (offset: 0x24b3): PyTuple_Size
+    <45c7>   DW_AT_decl_file   : (data1) 35
+    <45c8>   DW_AT_decl_line   : (data1) 31
+    <45c9>   DW_AT_decl_column : (data1) 24
+ <1><45ca>: Abbrev Number: 101 (DW_TAG_subprogram)
+    <45cb>   DW_AT_external    : (flag_present) 1
+    <45cb>   DW_AT_declaration : (flag_present) 1
+    <45cb>   DW_AT_linkage_name: (strp) (offset: 0x1c2e): PyDict_Size
+    <45cf>   DW_AT_name        : (strp) (offset: 0x1c2e): PyDict_Size
+    <45d3>   DW_AT_decl_file   : (data1) 37
+    <45d4>   DW_AT_decl_line   : (data1) 32
+    <45d5>   DW_AT_decl_column : (data1) 24
+ <1><45d6>: Abbrev Number: 0
+  Compilation Unit @ offset 0x45d7:
    Length:        0x1e (32-bit)
    Version:       2
    Abbrev Offset: 0x649
    Pointer Size:  8
- <0><4505>: Abbrev Number: 1 (DW_TAG_compile_unit)
-    <4506>   DW_AT_stmt_list   : (data4) 0x13be
-    <450a>   DW_AT_ranges      : (data4) 0x730
-    <450e>   DW_AT_name        : (strp) (offset: 0x24e0): crt/x86_64/crtn.s
-    <4512>   DW_AT_comp_dir    : (strp) (offset: 0x12): /home/buildozer/aports/main/musl/src/musl-1.1.24
-    <4516>   DW_AT_producer    : (strp) (offset: 0x43): GNU AS 2.34
-    <451a>   DW_AT_language    : (data2) 32769	(MIPS assembler)
+ <0><45e2>: Abbrev Number: 1 (DW_TAG_compile_unit)
+    <45e3>   DW_AT_stmt_list   : (data4) 0x141f
+    <45e7>   DW_AT_ranges      : (data4) 0x7a0
+    <45eb>   DW_AT_name        : (strp) (offset: 0x24e0): crt/x86_64/crtn.s
+    <45ef>   DW_AT_comp_dir    : (strp) (offset: 0x12): /home/buildozer/aports/main/musl/src/musl-1.1.24
+    <45f3>   DW_AT_producer    : (strp) (offset: 0x43): GNU AS 2.34
+    <45f7>   DW_AT_language    : (data2) 32769	(MIPS assembler)
```

### readelf --wide --debug-dump=abbrev {}

```diff
@@ -435,81 +435,81 @@
     DW_AT_decl_file    DW_FORM_data1
     DW_AT_decl_line    DW_FORM_data1
     DW_AT_decl_column  DW_FORM_data1
     DW_AT_type         DW_FORM_ref4
     DW_AT_location     DW_FORM_sec_offset
     DW_AT_GNU_locviews DW_FORM_sec_offset
     DW_AT value: 0     DW_FORM value: 0
-   66      DW_TAG_variable    [no children]
-    DW_AT_name         DW_FORM_string
-    DW_AT_decl_file    DW_FORM_data1
-    DW_AT_decl_line    DW_FORM_data1
-    DW_AT_decl_column  DW_FORM_data1
-    DW_AT_type         DW_FORM_ref4
-    DW_AT_location     DW_FORM_sec_offset
-    DW_AT_GNU_locviews DW_FORM_sec_offset
-    DW_AT value: 0     DW_FORM value: 0
-   67      DW_TAG_variable    [no children]
-    DW_AT_name         DW_FORM_strp
-    DW_AT_decl_file    DW_FORM_data1
-    DW_AT_decl_line    DW_FORM_data1
-    DW_AT_decl_column  DW_FORM_data1
-    DW_AT_type         DW_FORM_ref4
-    DW_AT_location     DW_FORM_sec_offset
-    DW_AT_GNU_locviews DW_FORM_sec_offset
-    DW_AT value: 0     DW_FORM value: 0
-   68      DW_TAG_label    [no children]
+   66      DW_TAG_label    [no children]
     DW_AT_name         DW_FORM_strp
     DW_AT_decl_file    DW_FORM_data1
     DW_AT_decl_line    DW_FORM_data2
     DW_AT_decl_column  DW_FORM_data1
     DW_AT_low_pc       DW_FORM_addr
     DW_AT value: 0     DW_FORM value: 0
-   69      DW_TAG_inlined_subroutine    [has children]
+   67      DW_TAG_inlined_subroutine    [has children]
     DW_AT_abstract_origin DW_FORM_ref4
     DW_AT_low_pc       DW_FORM_addr
     DW_AT_high_pc      DW_FORM_data8
     DW_AT_call_file    DW_FORM_data1
     DW_AT_call_line    DW_FORM_data2
     DW_AT_call_column  DW_FORM_data1
     DW_AT_sibling      DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   70      DW_TAG_subprogram    [has children]
+   68      DW_TAG_subprogram    [has children]
     DW_AT_external     DW_FORM_flag_present
     DW_AT_name         DW_FORM_strp
     DW_AT_decl_file    DW_FORM_data1
     DW_AT_decl_line    DW_FORM_data1
     DW_AT_decl_column  DW_FORM_data1
     DW_AT_prototyped   DW_FORM_flag_present
     DW_AT_type         DW_FORM_ref4
     DW_AT_inline       DW_FORM_data1
     DW_AT_sibling      DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   71      DW_TAG_formal_parameter    [no children]
+   69      DW_TAG_formal_parameter    [no children]
     DW_AT_name         DW_FORM_strp
     DW_AT_decl_file    DW_FORM_data1
     DW_AT_decl_line    DW_FORM_data1
     DW_AT_decl_column  DW_FORM_data1
     DW_AT_type         DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   72      DW_TAG_variable    [no children]
+   70      DW_TAG_variable    [no children]
     DW_AT_name         DW_FORM_strp
     DW_AT_decl_file    DW_FORM_data1
     DW_AT_decl_line    DW_FORM_data1
     DW_AT_decl_column  DW_FORM_data1
     DW_AT_type         DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   73      DW_TAG_lexical_block    [has children]
+   71      DW_TAG_lexical_block    [has children]
+    DW_AT value: 0     DW_FORM value: 0
+   72      DW_TAG_variable    [no children]
+    DW_AT_name         DW_FORM_string
+    DW_AT_decl_file    DW_FORM_data1
+    DW_AT_decl_line    DW_FORM_data1
+    DW_AT_decl_column  DW_FORM_data1
+    DW_AT_type         DW_FORM_ref4
+    DW_AT value: 0     DW_FORM value: 0
+   73      DW_TAG_variable    [no children]
+    DW_AT_name         DW_FORM_strp
+    DW_AT_decl_file    DW_FORM_data1
+    DW_AT_decl_line    DW_FORM_data1
+    DW_AT_decl_column  DW_FORM_data1
+    DW_AT_type         DW_FORM_ref4
+    DW_AT_location     DW_FORM_sec_offset
+    DW_AT_GNU_locviews DW_FORM_sec_offset
     DW_AT value: 0     DW_FORM value: 0
    74      DW_TAG_variable    [no children]
     DW_AT_name         DW_FORM_string
     DW_AT_decl_file    DW_FORM_data1
     DW_AT_decl_line    DW_FORM_data1
     DW_AT_decl_column  DW_FORM_data1
     DW_AT_type         DW_FORM_ref4
+    DW_AT_location     DW_FORM_sec_offset
+    DW_AT_GNU_locviews DW_FORM_sec_offset
     DW_AT value: 0     DW_FORM value: 0
    75      DW_TAG_inlined_subroutine    [has children]
     DW_AT_abstract_origin DW_FORM_ref4
     DW_AT_entry_pc     DW_FORM_addr
     DW_AT_GNU_entry_view DW_FORM_data1
     DW_AT_ranges       DW_FORM_sec_offset
     DW_AT_call_file    DW_FORM_data1
@@ -533,177 +533,177 @@
     DW_AT_low_pc       DW_FORM_addr
     DW_AT_high_pc      DW_FORM_data8
     DW_AT_call_file    DW_FORM_data1
     DW_AT_call_line    DW_FORM_data1
     DW_AT_call_column  DW_FORM_data1
     DW_AT_sibling      DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   78      DW_TAG_subprogram    [has children]
+   78      DW_TAG_inlined_subroutine    [has children]
+    DW_AT_abstract_origin DW_FORM_ref4
+    DW_AT_entry_pc     DW_FORM_addr
+    DW_AT_GNU_entry_view DW_FORM_data1
+    DW_AT_low_pc       DW_FORM_addr
+    DW_AT_high_pc      DW_FORM_data8
+    DW_AT_call_file    DW_FORM_data1
+    DW_AT_call_line    DW_FORM_data1
+    DW_AT_call_column  DW_FORM_data1
+    DW_AT value: 0     DW_FORM value: 0
+   79      DW_TAG_subprogram    [has children]
     DW_AT_external     DW_FORM_flag_present
     DW_AT_name         DW_FORM_strp
     DW_AT_decl_file    DW_FORM_data1
     DW_AT_decl_line    DW_FORM_data1
     DW_AT_decl_column  DW_FORM_data1
     DW_AT_prototyped   DW_FORM_flag_present
     DW_AT_low_pc       DW_FORM_addr
     DW_AT_high_pc      DW_FORM_data8
     DW_AT_frame_base   DW_FORM_exprloc
     DW_AT_GNU_all_call_sites DW_FORM_flag_present
     DW_AT_sibling      DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   79      DW_TAG_GNU_call_site    [has children]
+   80      DW_TAG_GNU_call_site    [has children]
     DW_AT_low_pc       DW_FORM_addr
     DW_AT_GNU_tail_call DW_FORM_flag_present
     DW_AT_sibling      DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   80      DW_TAG_GNU_call_site    [has children]
+   81      DW_TAG_GNU_call_site    [has children]
     DW_AT_low_pc       DW_FORM_addr
     DW_AT_sibling      DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   81      DW_TAG_GNU_call_site    [no children]
+   82      DW_TAG_GNU_call_site    [no children]
     DW_AT_low_pc       DW_FORM_addr
     DW_AT_GNU_tail_call DW_FORM_flag_present
     DW_AT_abstract_origin DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   82      DW_TAG_inlined_subroutine    [has children]
+   83      DW_TAG_inlined_subroutine    [has children]
     DW_AT_abstract_origin DW_FORM_ref4
     DW_AT_entry_pc     DW_FORM_addr
     DW_AT_GNU_entry_view DW_FORM_data1
     DW_AT_ranges       DW_FORM_sec_offset
     DW_AT_call_file    DW_FORM_data1
     DW_AT_call_line    DW_FORM_data1
     DW_AT_call_column  DW_FORM_data1
     DW_AT value: 0     DW_FORM value: 0
-   83      DW_TAG_subprogram    [has children]
+   84      DW_TAG_subprogram    [has children]
     DW_AT_name         DW_FORM_strp
     DW_AT_decl_file    DW_FORM_data1
     DW_AT_decl_line    DW_FORM_data1
     DW_AT_decl_column  DW_FORM_data1
     DW_AT_prototyped   DW_FORM_flag_present
     DW_AT_type         DW_FORM_ref4
     DW_AT_inline       DW_FORM_data1
     DW_AT_sibling      DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   84      DW_TAG_formal_parameter    [no children]
+   85      DW_TAG_formal_parameter    [no children]
     DW_AT_name         DW_FORM_string
     DW_AT_decl_file    DW_FORM_data1
     DW_AT_decl_line    DW_FORM_data1
     DW_AT_decl_column  DW_FORM_data1
     DW_AT_type         DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   85      DW_TAG_lexical_block    [has children]
+   86      DW_TAG_lexical_block    [has children]
     DW_AT_sibling      DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   86      DW_TAG_subprogram    [has children]
+   87      DW_TAG_subprogram    [has children]
     DW_AT_name         DW_FORM_strp
     DW_AT_decl_file    DW_FORM_data1
     DW_AT_decl_line    DW_FORM_data1
     DW_AT_decl_column  DW_FORM_data1
     DW_AT_prototyped   DW_FORM_flag_present
     DW_AT_type         DW_FORM_ref4
     DW_AT_low_pc       DW_FORM_addr
     DW_AT_high_pc      DW_FORM_data8
     DW_AT_frame_base   DW_FORM_exprloc
     DW_AT_GNU_all_call_sites DW_FORM_flag_present
     DW_AT_sibling      DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   87      DW_TAG_formal_parameter    [no children]
+   88      DW_TAG_formal_parameter    [no children]
     DW_AT_name         DW_FORM_strp
     DW_AT_decl_file    DW_FORM_data1
     DW_AT_decl_line    DW_FORM_data1
     DW_AT_decl_column  DW_FORM_data1
     DW_AT_type         DW_FORM_ref4
     DW_AT_location     DW_FORM_exprloc
     DW_AT value: 0     DW_FORM value: 0
-   88      DW_TAG_subprogram    [has children]
+   89      DW_TAG_subprogram    [has children]
     DW_AT_name         DW_FORM_strp
     DW_AT_decl_file    DW_FORM_data1
     DW_AT_decl_line    DW_FORM_data1
     DW_AT_decl_column  DW_FORM_data1
     DW_AT_prototyped   DW_FORM_flag_present
     DW_AT_inline       DW_FORM_data1
     DW_AT_sibling      DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   89      DW_TAG_subprogram    [has children]
+   90      DW_TAG_subprogram    [has children]
     DW_AT_name         DW_FORM_strp
     DW_AT_decl_file    DW_FORM_data1
     DW_AT_decl_line    DW_FORM_data2
     DW_AT_decl_column  DW_FORM_data1
     DW_AT_prototyped   DW_FORM_flag_present
     DW_AT_type         DW_FORM_ref4
     DW_AT_inline       DW_FORM_data1
     DW_AT_sibling      DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   90      DW_TAG_formal_parameter    [no children]
+   91      DW_TAG_formal_parameter    [no children]
     DW_AT_name         DW_FORM_strp
     DW_AT_decl_file    DW_FORM_data1
     DW_AT_decl_line    DW_FORM_data2
     DW_AT_decl_column  DW_FORM_data1
     DW_AT_type         DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   91      DW_TAG_variable    [no children]
+   92      DW_TAG_variable    [no children]
     DW_AT_name         DW_FORM_strp
     DW_AT_decl_file    DW_FORM_data1
     DW_AT_decl_line    DW_FORM_data2
     DW_AT_decl_column  DW_FORM_data1
     DW_AT_type         DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   92      DW_TAG_formal_parameter    [no children]
+   93      DW_TAG_formal_parameter    [no children]
     DW_AT_name         DW_FORM_string
     DW_AT_decl_file    DW_FORM_data1
     DW_AT_decl_line    DW_FORM_data2
     DW_AT_decl_column  DW_FORM_data1
     DW_AT_type         DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   93      DW_TAG_subprogram    [has children]
+   94      DW_TAG_subprogram    [has children]
     DW_AT_name         DW_FORM_strp
     DW_AT_decl_file    DW_FORM_data1
     DW_AT_decl_line    DW_FORM_data2
     DW_AT_decl_column  DW_FORM_data1
     DW_AT_prototyped   DW_FORM_flag_present
     DW_AT_inline       DW_FORM_data1
     DW_AT_sibling      DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   94      DW_TAG_subprogram    [has children]
+   95      DW_TAG_subprogram    [has children]
     DW_AT_abstract_origin DW_FORM_ref4
     DW_AT_low_pc       DW_FORM_addr
     DW_AT_high_pc      DW_FORM_data8
     DW_AT_frame_base   DW_FORM_exprloc
     DW_AT_GNU_all_call_sites DW_FORM_flag_present
     DW_AT_sibling      DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   95      DW_TAG_lexical_block    [has children]
+   96      DW_TAG_lexical_block    [has children]
     DW_AT_abstract_origin DW_FORM_ref4
     DW_AT_ranges       DW_FORM_sec_offset
     DW_AT_sibling      DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   96      DW_TAG_lexical_block    [has children]
+   97      DW_TAG_lexical_block    [has children]
     DW_AT_abstract_origin DW_FORM_ref4
     DW_AT_low_pc       DW_FORM_addr
     DW_AT_high_pc      DW_FORM_data8
     DW_AT_sibling      DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
-   97      DW_TAG_lexical_block    [has children]
+   98      DW_TAG_lexical_block    [has children]
     DW_AT_abstract_origin DW_FORM_ref4
     DW_AT_ranges       DW_FORM_sec_offset
     DW_AT value: 0     DW_FORM value: 0
-   98      DW_TAG_variable    [no children]
+   99      DW_TAG_variable    [no children]
     DW_AT_abstract_origin DW_FORM_ref4
     DW_AT_location     DW_FORM_exprloc
     DW_AT value: 0     DW_FORM value: 0
-   99      DW_TAG_inlined_subroutine    [has children]
-    DW_AT_abstract_origin DW_FORM_ref4
-    DW_AT_entry_pc     DW_FORM_addr
-    DW_AT_GNU_entry_view DW_FORM_data1
-    DW_AT_low_pc       DW_FORM_addr
-    DW_AT_high_pc      DW_FORM_data8
-    DW_AT_call_file    DW_FORM_data1
-    DW_AT_call_line    DW_FORM_data1
-    DW_AT_call_column  DW_FORM_data1
-    DW_AT value: 0     DW_FORM value: 0
    100      DW_TAG_variable    [no children]
     DW_AT_abstract_origin DW_FORM_ref4
     DW_AT value: 0     DW_FORM value: 0
    101      DW_TAG_subprogram    [no children]
     DW_AT_external     DW_FORM_flag_present
     DW_AT_declaration  DW_FORM_flag_present
     DW_AT_linkage_name DW_FORM_strp
```

### readelf --wide --debug-dump=aranges {}

```diff
@@ -4,29 +4,29 @@
   Version:                  2
   Offset into .debug_info:  0
   Pointer Size:             8
   Segment Size:             0
 
     Address            Length
     0000000000002000 0000000000000001
-    0000000000002eae 0000000000000001
+    0000000000002ebe 0000000000000001
     0000000000000000 0000000000000000
   Length:                   44
   Version:                  2
   Offset into .debug_info:  0x22
   Pointer Size:             8
   Segment Size:             0
 
     Address            Length
-    00000000000023c0 0000000000000acc
+    00000000000023c0 0000000000000adc
     0000000000000000 0000000000000000
   Length:                   60
   Version:                  2
-  Offset into .debug_info:  0x44fa
+  Offset into .debug_info:  0x45d7
   Pointer Size:             8
   Segment Size:             0
 
     Address            Length
     000000000000200b 0000000000000002
-    0000000000002eb4 0000000000000002
+    0000000000002ec4 0000000000000002
     0000000000000000 0000000000000000
```

### readelf --wide --debug-dump=frames {}

```diff
@@ -388,15 +388,15 @@
   DW_CFA_def_cfa_offset: 24
   DW_CFA_advance_loc: 3 to 0000000000002c9d
   DW_CFA_def_cfa_offset: 16
   DW_CFA_advance_loc: 2 to 0000000000002c9f
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
 
-00000324 0000000000000038 00000328 FDE cie=00000000 pc=0000000000002ca0..0000000000002d41
+00000324 000000000000003c 00000328 FDE cie=00000000 pc=0000000000002ca0..0000000000002d57
   DW_CFA_advance_loc: 2 to 0000000000002ca2
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r14 (r14) at cfa-16
   DW_CFA_advance_loc: 2 to 0000000000002ca4
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r13 (r13) at cfa-24
   DW_CFA_advance_loc: 2 to 0000000000002ca6
@@ -404,73 +404,77 @@
   DW_CFA_offset: r12 (r12) at cfa-32
   DW_CFA_advance_loc: 1 to 0000000000002ca7
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r6 (rbp) at cfa-40
   DW_CFA_advance_loc: 1 to 0000000000002ca8
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_advance_loc1: 142 to 0000000000002d36
+  DW_CFA_advance_loc1: 155 to 0000000000002d43
+  DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 4 to 0000000000002d3a
+  DW_CFA_advance_loc: 4 to 0000000000002d47
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000002d3c
+  DW_CFA_advance_loc: 2 to 0000000000002d49
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000002d3e
+  DW_CFA_advance_loc: 2 to 0000000000002d4b
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000002d40
+  DW_CFA_advance_loc: 2 to 0000000000002d4d
   DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 3 to 0000000000002d50
+  DW_CFA_restore_state
+  DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000360 000000000000004c 00000364 FDE cie=00000000 pc=0000000000002d50..0000000000002e74
-  DW_CFA_advance_loc: 2 to 0000000000002d52
+00000364 000000000000004c 00000368 FDE cie=00000000 pc=0000000000002d60..0000000000002e84
+  DW_CFA_advance_loc: 2 to 0000000000002d62
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r13 (r13) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000002d54
+  DW_CFA_advance_loc: 2 to 0000000000002d64
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r12 (r12) at cfa-24
-  DW_CFA_advance_loc: 1 to 0000000000002d55
+  DW_CFA_advance_loc: 1 to 0000000000002d65
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r6 (rbp) at cfa-32
-  DW_CFA_advance_loc1: 136 to 0000000000002ddd
+  DW_CFA_advance_loc1: 136 to 0000000000002ded
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000002ddf
+  DW_CFA_advance_loc: 2 to 0000000000002def
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000002de1
+  DW_CFA_advance_loc: 2 to 0000000000002df1
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 7 to 0000000000002de8
+  DW_CFA_advance_loc: 7 to 0000000000002df8
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 29 to 0000000000002e05
+  DW_CFA_advance_loc: 29 to 0000000000002e15
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000002e07
+  DW_CFA_advance_loc: 2 to 0000000000002e17
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000002e09
+  DW_CFA_advance_loc: 2 to 0000000000002e19
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 7 to 0000000000002e10
+  DW_CFA_advance_loc: 7 to 0000000000002e20
   DW_CFA_restore_state
-  DW_CFA_advance_loc1: 76 to 0000000000002e5c
+  DW_CFA_advance_loc1: 76 to 0000000000002e6c
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000002e5e
+  DW_CFA_advance_loc: 2 to 0000000000002e6e
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000002e60
+  DW_CFA_advance_loc: 2 to 0000000000002e70
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 8 to 0000000000002e68
+  DW_CFA_advance_loc: 8 to 0000000000002e78
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 4 to 0000000000002e6c
+  DW_CFA_advance_loc: 4 to 0000000000002e7c
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 5 to 0000000000002e71
+  DW_CFA_advance_loc: 5 to 0000000000002e81
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000002e73
+  DW_CFA_advance_loc: 2 to 0000000000002e83
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
 
-000003b0 0000000000000010 000003b4 FDE cie=00000000 pc=0000000000002e80..0000000000002e8c
+000003b4 0000000000000010 000003b8 FDE cie=00000000 pc=0000000000002e90..0000000000002e9c
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000003c4 ZERO terminator
+000003c8 ZERO terminator
```

### readelf --wide --debug-dump=loc {}

```diff
@@ -607,1003 +607,1087 @@
 
     00000f91 v000000000000000 v000000000000000 location view pair
     00000f93 v000000000000000 v000000000000000 location view pair
     00000f95 v000000000000000 v000000000000000 location view pair
     00000f97 v000000000000000 v000000000000000 location view pair
 
     00000f99 v000000000000000 v000000000000000 views at 00000f91 for:
-             0000000000002d50 0000000000002d62 (DW_OP_reg5 (rdi))
+             0000000000002d60 0000000000002d72 (DW_OP_reg5 (rdi))
     00000fac v000000000000000 v000000000000000 views at 00000f93 for:
-             0000000000002d62 0000000000002de2 (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
+             0000000000002d72 0000000000002df2 (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
     00000fc2 v000000000000000 v000000000000000 views at 00000f95 for:
-             0000000000002de2 0000000000002dfc (DW_OP_reg5 (rdi))
+             0000000000002df2 0000000000002e0c (DW_OP_reg5 (rdi))
     00000fd5 v000000000000000 v000000000000000 views at 00000f97 for:
-             0000000000002dfc 0000000000002e74 (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
+             0000000000002e0c 0000000000002e84 (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
     00000feb <End of list>
 
     00000ffb v000000000000000 v000000000000000 location view pair
     00000ffd v000000000000000 v000000000000000 location view pair
     00000fff v000000000000000 v000000000000000 location view pair
     00001001 v000000000000000 v000000000000000 location view pair
 
     00001003 v000000000000000 v000000000000000 views at 00000ffb for:
-             0000000000002d50 0000000000002d69 (DW_OP_reg4 (rsi))
+             0000000000002d60 0000000000002d79 (DW_OP_reg4 (rsi))
     00001016 v000000000000000 v000000000000000 views at 00000ffd for:
-             0000000000002d69 0000000000002de2 (DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)); DW_OP_stack_value)
+             0000000000002d79 0000000000002df2 (DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)); DW_OP_stack_value)
     0000102c v000000000000000 v000000000000000 views at 00000fff for:
-             0000000000002de2 0000000000002df9 (DW_OP_reg4 (rsi))
+             0000000000002df2 0000000000002e09 (DW_OP_reg4 (rsi))
     0000103f v000000000000000 v000000000000000 views at 00001001 for:
-             0000000000002df9 0000000000002e74 (DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)); DW_OP_stack_value)
+             0000000000002e09 0000000000002e84 (DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)); DW_OP_stack_value)
     00001055 <End of list>
 
     00001065 v000000000000000 v000000000000000 location view pair
     00001067 v000000000000000 v000000000000000 location view pair
     00001069 v000000000000000 v000000000000000 location view pair
     0000106b v000000000000000 v000000000000000 location view pair
     0000106d v000000000000000 v000000000000000 location view pair
     0000106f v000000000000000 v000000000000000 location view pair
     00001071 v000000000000000 v000000000000000 location view pair
     00001073 v000000000000000 v000000000000000 location view pair
     00001075 v000000000000000 v000000000000000 location view pair
 
     00001077 v000000000000000 v000000000000000 views at 00001065 for:
-             0000000000002d50 0000000000002d69 (DW_OP_reg1 (rdx))
+             0000000000002d60 0000000000002d79 (DW_OP_reg1 (rdx))
     0000108a v000000000000000 v000000000000000 views at 00001067 for:
-             0000000000002d69 0000000000002db0 (DW_OP_reg12 (r12))
+             0000000000002d79 0000000000002dc0 (DW_OP_reg12 (r12))
     0000109d v000000000000000 v000000000000000 views at 00001069 for:
-             0000000000002db0 0000000000002de2 (DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)); DW_OP_stack_value)
+             0000000000002dc0 0000000000002df2 (DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)); DW_OP_stack_value)
     000010b3 v000000000000000 v000000000000000 views at 0000106b for:
-             0000000000002de2 0000000000002e00 (DW_OP_reg1 (rdx))
+             0000000000002df2 0000000000002e10 (DW_OP_reg1 (rdx))
     000010c6 v000000000000000 v000000000000000 views at 0000106d for:
-             0000000000002e00 0000000000002e0a (DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)); DW_OP_stack_value)
+             0000000000002e10 0000000000002e1a (DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)); DW_OP_stack_value)
     000010dc v000000000000000 v000000000000000 views at 0000106f for:
-             0000000000002e0a 0000000000002e35 (DW_OP_reg12 (r12))
+             0000000000002e1a 0000000000002e45 (DW_OP_reg12 (r12))
     000010ef v000000000000000 v000000000000000 views at 00001071 for:
-             0000000000002e35 0000000000002e61 (DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)); DW_OP_stack_value)
+             0000000000002e45 0000000000002e71 (DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)); DW_OP_stack_value)
     00001105 v000000000000000 v000000000000000 views at 00001073 for:
-             0000000000002e61 0000000000002e6b (DW_OP_reg12 (r12))
+             0000000000002e71 0000000000002e7b (DW_OP_reg12 (r12))
     00001118 v000000000000000 v000000000000000 views at 00001075 for:
-             0000000000002e6b 0000000000002e74 (DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)); DW_OP_stack_value)
+             0000000000002e7b 0000000000002e84 (DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)); DW_OP_stack_value)
     0000112e <End of list>
 
     0000113e v000000000000000 v000000000000000 location view pair
     00001140 v000000000000000 v000000000000000 location view pair
     00001142 v000000000000000 v000000000000000 location view pair
     00001144 v000000000000000 v000000000000000 location view pair
 
     00001146 v000000000000000 v000000000000000 views at 0000113e for:
-             0000000000002d50 0000000000002d69 (DW_OP_reg2 (rcx))
+             0000000000002d60 0000000000002d79 (DW_OP_reg2 (rcx))
     00001159 v000000000000000 v000000000000000 views at 00001140 for:
-             0000000000002d69 0000000000002de2 (DW_OP_GNU_entry_value: (DW_OP_reg2 (rcx)); DW_OP_stack_value)
+             0000000000002d79 0000000000002df2 (DW_OP_GNU_entry_value: (DW_OP_reg2 (rcx)); DW_OP_stack_value)
     0000116f v000000000000000 v000000000000000 views at 00001142 for:
-             0000000000002de2 0000000000002e00 (DW_OP_reg2 (rcx))
+             0000000000002df2 0000000000002e10 (DW_OP_reg2 (rcx))
     00001182 v000000000000000 v000000000000000 views at 00001144 for:
-             0000000000002e00 0000000000002e74 (DW_OP_GNU_entry_value: (DW_OP_reg2 (rcx)); DW_OP_stack_value)
+             0000000000002e10 0000000000002e84 (DW_OP_GNU_entry_value: (DW_OP_reg2 (rcx)); DW_OP_stack_value)
     00001198 <End of list>
 
     000011a8 v000000000000000 v000000000000000 location view pair
     000011aa v000000000000000 v000000000000000 location view pair
     000011ac v000000000000000 v000000000000000 location view pair
     000011ae v000000000000000 v000000000000000 location view pair
 
     000011b0 v000000000000000 v000000000000000 views at 000011a8 for:
-             0000000000002d50 0000000000002d69 (DW_OP_reg8 (r8))
+             0000000000002d60 0000000000002d79 (DW_OP_reg8 (r8))
     000011c3 v000000000000000 v000000000000000 views at 000011aa for:
-             0000000000002d69 0000000000002de2 (DW_OP_GNU_entry_value: (DW_OP_reg8 (r8)); DW_OP_stack_value)
+             0000000000002d79 0000000000002df2 (DW_OP_GNU_entry_value: (DW_OP_reg8 (r8)); DW_OP_stack_value)
     000011d9 v000000000000000 v000000000000000 views at 000011ac for:
-             0000000000002de2 0000000000002e00 (DW_OP_reg8 (r8))
+             0000000000002df2 0000000000002e10 (DW_OP_reg8 (r8))
     000011ec v000000000000000 v000000000000000 views at 000011ae for:
-             0000000000002e00 0000000000002e74 (DW_OP_GNU_entry_value: (DW_OP_reg8 (r8)); DW_OP_stack_value)
+             0000000000002e10 0000000000002e84 (DW_OP_GNU_entry_value: (DW_OP_reg8 (r8)); DW_OP_stack_value)
     00001202 <End of list>
 
     00001212 v000000000000000 v000000000000000 location view pair
     00001214 v000000000000000 v000000000000000 location view pair
     00001216 v000000000000000 v000000000000000 location view pair
     00001218 v000000000000000 v000000000000000 location view pair
 
     0000121a v000000000000000 v000000000000000 views at 00001212 for:
-             0000000000002d6d 0000000000002d8e (DW_OP_reg0 (rax))
+             0000000000002d7d 0000000000002d9e (DW_OP_reg0 (rax))
     0000122d v000000000000000 v000000000000000 views at 00001214 for:
-             0000000000002d8e 0000000000002dc8 (DW_OP_reg13 (r13))
+             0000000000002d9e 0000000000002dd8 (DW_OP_reg13 (r13))
     00001240 v000000000000000 v000000000000000 views at 00001216 for:
-             0000000000002e0a 0000000000002e37 (DW_OP_reg13 (r13))
+             0000000000002e1a 0000000000002e47 (DW_OP_reg13 (r13))
     00001253 v000000000000000 v000000000000000 views at 00001218 for:
-             0000000000002e61 0000000000002e73 (DW_OP_reg13 (r13))
+             0000000000002e71 0000000000002e83 (DW_OP_reg13 (r13))
     00001266 <End of list>
 
     00001276 v000000000000000 v000000000000000 location view pair
     00001278 v000000000000001 v000000000000000 location view pair
     0000127a v000000000000000 v000000000000000 location view pair
     0000127c v000000000000000 v000000000000000 location view pair
     0000127e v000000000000000 v000000000000000 location view pair
     00001280 v000000000000000 v000000000000000 location view pair
     00001282 v000000000000000 v000000000000000 location view pair
     00001284 v000000000000000 v000000000000000 location view pair
     00001286 v000000000000000 v000000000000000 location view pair
     00001288 v000000000000000 v000000000000000 location view pair
 
     0000128a v000000000000000 v000000000000000 views at 00001276 for:
-             0000000000002d7a 0000000000002da8 (DW_OP_reg6 (rbp))
+             0000000000002d8a 0000000000002db8 (DW_OP_reg6 (rbp))
     0000129d v000000000000001 v000000000000000 views at 00001278 for:
-             0000000000002da8 0000000000002dac (DW_OP_reg0 (rax))
+             0000000000002db8 0000000000002dbc (DW_OP_reg0 (rax))
     000012b0 v000000000000000 v000000000000000 views at 0000127a for:
-             0000000000002dac 0000000000002db0 (DW_OP_reg6 (rbp))
+             0000000000002dbc 0000000000002dc0 (DW_OP_reg6 (rbp))
     000012c3 v000000000000000 v000000000000000 views at 0000127c for:
-             0000000000002db0 0000000000002dbf (DW_OP_reg0 (rax))
+             0000000000002dc0 0000000000002dcf (DW_OP_reg0 (rax))
     000012d6 v000000000000000 v000000000000000 views at 0000127e for:
-             0000000000002dbf 0000000000002dcd (DW_OP_reg12 (r12))
+             0000000000002dcf 0000000000002ddd (DW_OP_reg12 (r12))
     000012e9 v000000000000000 v000000000000000 views at 00001280 for:
-             0000000000002e0a 0000000000002e22 (DW_OP_reg6 (rbp))
+             0000000000002e1a 0000000000002e32 (DW_OP_reg6 (rbp))
     000012fc v000000000000000 v000000000000000 views at 00001282 for:
-             0000000000002e22 0000000000002e31 (DW_OP_reg0 (rax))
+             0000000000002e32 0000000000002e41 (DW_OP_reg0 (rax))
     0000130f v000000000000000 v000000000000000 views at 00001284 for:
-             0000000000002e31 0000000000002e37 (DW_OP_reg6 (rbp))
+             0000000000002e41 0000000000002e47 (DW_OP_reg6 (rbp))
     00001322 v000000000000000 v000000000000000 views at 00001286 for:
-             0000000000002e37 0000000000002e46 (DW_OP_reg12 (r12))
+             0000000000002e47 0000000000002e56 (DW_OP_reg12 (r12))
     00001335 v000000000000000 v000000000000000 views at 00001288 for:
-             0000000000002e46 0000000000002e4a (DW_OP_reg5 (rdi))
+             0000000000002e56 0000000000002e5a (DW_OP_reg5 (rdi))
     00001348 <End of list>
 
     00001358 v000000000000000 v000000000000000 location view pair
     0000135a v000000000000000 v000000000000000 location view pair
     0000135c v000000000000000 v000000000000000 location view pair
     0000135e v000000000000000 v000000000000000 location view pair
     00001360 v000000000000000 v000000000000000 location view pair
 
     00001362 v000000000000000 v000000000000000 views at 00001358 for:
-             0000000000002d7a 0000000000002da8 (DW_OP_lit0; DW_OP_stack_value)
+             0000000000002d8a 0000000000002db8 (DW_OP_lit0; DW_OP_stack_value)
     00001376 v000000000000000 v000000000000000 views at 0000135a for:
-             0000000000002da8 0000000000002dac (DW_OP_reg0 (rax))
+             0000000000002db8 0000000000002dbc (DW_OP_reg0 (rax))
     00001389 v000000000000000 v000000000000000 views at 0000135c for:
-             0000000000002dac 0000000000002dd2 (DW_OP_reg6 (rbp))
+             0000000000002dbc 0000000000002de2 (DW_OP_reg6 (rbp))
     0000139c v000000000000000 v000000000000000 views at 0000135e for:
-             0000000000002e0a 0000000000002e37 (DW_OP_lit0; DW_OP_stack_value)
+             0000000000002e1a 0000000000002e47 (DW_OP_lit0; DW_OP_stack_value)
     000013b0 v000000000000000 v000000000000000 views at 00001360 for:
-             0000000000002e37 0000000000002e4d (DW_OP_reg6 (rbp))
+             0000000000002e47 0000000000002e5d (DW_OP_reg6 (rbp))
     000013c3 <End of list>
 
     000013d3 v000000000000000 v000000000000000 location view pair
     000013d5 v000000000000000 v000000000000000 location view pair
     000013d7 v000000000000000 v000000000000000 location view pair
     000013d9 v000000000000000 v000000000000000 location view pair
     000013db v000000000000000 v000000000000000 location view pair
     000013dd v000000000000000 v000000000000000 location view pair
     000013df v000000000000000 v000000000000000 location view pair
     000013e1 v000000000000000 v000000000000000 location view pair
     000013e3 v000000000000000 v000000000000000 location view pair
 
     000013e5 v000000000000000 v000000000000000 views at 000013d3 for:
-             0000000000002d7a 0000000000002dc8 (DW_OP_lit0; DW_OP_stack_value)
+             0000000000002d8a 0000000000002dd8 (DW_OP_lit0; DW_OP_stack_value)
     000013f9 v000000000000000 v000000000000000 views at 000013d5 for:
-             0000000000002dc8 0000000000002dcd (DW_OP_reg0 (rax))
+             0000000000002dd8 0000000000002ddd (DW_OP_reg0 (rax))
     0000140c v000000000000000 v000000000000000 views at 000013d7 for:
-             0000000000002dcd 0000000000002ddf (DW_OP_reg12 (r12))
+             0000000000002ddd 0000000000002def (DW_OP_reg12 (r12))
     0000141f v000000000000000 v000000000000000 views at 000013d9 for:
-             0000000000002ddf 0000000000002de2 (DW_OP_reg0 (rax))
+             0000000000002def 0000000000002df2 (DW_OP_reg0 (rax))
     00001432 v000000000000000 v000000000000000 views at 000013db for:
-             0000000000002e0a 0000000000002e37 (DW_OP_lit0; DW_OP_stack_value)
+             0000000000002e1a 0000000000002e47 (DW_OP_lit0; DW_OP_stack_value)
     00001446 v000000000000000 v000000000000000 views at 000013dd for:
-             0000000000002e37 0000000000002e4a (DW_OP_reg0 (rax))
+             0000000000002e47 0000000000002e5a (DW_OP_reg0 (rax))
     00001459 v000000000000000 v000000000000000 views at 000013df for:
-             0000000000002e4a 0000000000002e4d (DW_OP_reg13 (r13))
+             0000000000002e5a 0000000000002e5d (DW_OP_reg13 (r13))
     0000146c v000000000000000 v000000000000000 views at 000013e1 for:
-             0000000000002e4d 0000000000002e5e (DW_OP_reg12 (r12))
+             0000000000002e5d 0000000000002e6e (DW_OP_reg12 (r12))
     0000147f v000000000000000 v000000000000000 views at 000013e3 for:
-             0000000000002e5e 0000000000002e61 (DW_OP_reg0 (rax))
+             0000000000002e6e 0000000000002e71 (DW_OP_reg0 (rax))
     00001492 <End of list>
 
     000014a2 v000000000000001 v000000000000000 location view pair
 
     000014a4 v000000000000001 v000000000000000 views at 000014a2 for:
-             0000000000002d7a 0000000000002d93 (DW_OP_reg6 (rbp))
+             0000000000002d8a 0000000000002da3 (DW_OP_reg6 (rbp))
     000014b7 <End of list>
 
     000014c7 v000000000000003 v000000000000002 location view pair
 
     000014c9 v000000000000003 v000000000000002 views at 000014c7 for:
-             0000000000002d7a 0000000000002d85 (DW_OP_reg6 (rbp))
+             0000000000002d8a 0000000000002d95 (DW_OP_reg6 (rbp))
     000014dc <End of list>
 
     000014ec v000000000000002 v000000000000000 location view pair
     000014ee v000000000000003 v000000000000000 location view pair
     000014f0 v000000000000000 v000000000000000 location view pair
     000014f2 v000000000000000 v000000000000000 location view pair
     000014f4 v000000000000000 v000000000000000 location view pair
 
     000014f6 v000000000000002 v000000000000000 views at 000014ec for:
-             0000000000002dc8 0000000000002dcd (DW_OP_reg12 (r12))
+             0000000000002dd8 0000000000002ddd (DW_OP_reg12 (r12))
     00001509 v000000000000003 v000000000000000 views at 000014ee for:
-             0000000000002dd2 0000000000002dd9 (DW_OP_reg6 (rbp))
+             0000000000002de2 0000000000002de9 (DW_OP_reg6 (rbp))
     0000151c v000000000000000 v000000000000000 views at 000014f0 for:
-             0000000000002e37 0000000000002e46 (DW_OP_reg12 (r12))
+             0000000000002e47 0000000000002e56 (DW_OP_reg12 (r12))
     0000152f v000000000000000 v000000000000000 views at 000014f2 for:
-             0000000000002e46 0000000000002e4a (DW_OP_reg5 (rdi))
+             0000000000002e56 0000000000002e5a (DW_OP_reg5 (rdi))
     00001542 v000000000000000 v000000000000000 views at 000014f4 for:
-             0000000000002e4d 0000000000002e58 (DW_OP_reg6 (rbp))
+             0000000000002e5d 0000000000002e68 (DW_OP_reg6 (rbp))
     00001555 <End of list>
 
     00001565 v000000000000003 v000000000000000 location view pair
     00001567 v000000000000004 v000000000000000 location view pair
 
     00001569 v000000000000003 v000000000000000 views at 00001565 for:
-             0000000000002dcd 0000000000002dd2 (DW_OP_reg6 (rbp))
+             0000000000002ddd 0000000000002de2 (DW_OP_reg6 (rbp))
     0000157c v000000000000004 v000000000000000 views at 00001567 for:
-             0000000000002e58 0000000000002e61 (DW_OP_lit0; DW_OP_stack_value)
+             0000000000002e68 0000000000002e71 (DW_OP_lit0; DW_OP_stack_value)
     00001590 <End of list>
 
     000015a0 v000000000000000 v000000000000000 location view pair
     000015a2 v000000000000000 v000000000000000 location view pair
     000015a4 v000000000000000 v000000000000000 location view pair
+    000015a6 v000000000000000 v000000000000000 location view pair
 
-    000015a6 v000000000000000 v000000000000000 views at 000015a0 for:
-             0000000000002ca0 0000000000002cca (DW_OP_reg5 (rdi))
-    000015b9 v000000000000000 v000000000000000 views at 000015a2 for:
-             0000000000002cca 0000000000002d35 (DW_OP_reg14 (r14))
-    000015cc v000000000000000 v000000000000000 views at 000015a4 for:
-             0000000000002d35 0000000000002d41 (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
-    000015e2 <End of list>
-
-    000015f2 v000000000000000 v000000000000000 location view pair
-    000015f4 v000000000000000 v000000000000000 location view pair
-
-    000015f6 v000000000000000 v000000000000000 views at 000015f2 for:
-             0000000000002ca0 0000000000002cca (DW_OP_reg4 (rsi))
-    00001609 v000000000000000 v000000000000000 views at 000015f4 for:
-             0000000000002cca 0000000000002d41 (DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)); DW_OP_stack_value)
-    0000161f <End of list>
-
-    0000162f v000000000000000 v000000000000000 location view pair
-
-    00001631 v000000000000000 v000000000000000 views at 0000162f for:
-             0000000000002cb4 0000000000002cca (DW_OP_reg12 (r12))
-    00001644 <End of list>
-
-    00001654 v000000000000000 v000000000000000 location view pair
-
-    00001656 v000000000000000 v000000000000000 views at 00001654 for:
-             0000000000002cb8 0000000000002d3e (DW_OP_reg13 (r13))
-    00001669 <End of list>
-
-    00001679 v000000000000003 v000000000000000 location view pair
-
-    0000167b v000000000000003 v000000000000000 views at 00001679 for:
-             0000000000002cbf 0000000000002cca (DW_OP_breg5 (rdi): 16)
-    0000168f <End of list>
-
-    0000169f v000000000000004 v000000000000000 location view pair
-    000016a1 v000000000000000 v000000000000000 location view pair
-    000016a3 v000000000000000 v000000000000000 location view pair
-    000016a5 v000000000000000 v000000000000000 location view pair
-    000016a7 v000000000000000 v000000000000000 location view pair
-    000016a9 v000000000000000 v000000000000000 location view pair
-
-    000016ab v000000000000004 v000000000000000 views at 0000169f for:
-             0000000000002cbf 0000000000002cf7 (DW_OP_reg12 (r12))
-    000016be v000000000000000 v000000000000000 views at 000016a1 for:
-             0000000000002cf7 0000000000002cfe (DW_OP_reg0 (rax))
-    000016d1 v000000000000000 v000000000000000 views at 000016a3 for:
-             0000000000002cfe 0000000000002d21 (DW_OP_reg12 (r12))
-    000016e4 v000000000000000 v000000000000000 views at 000016a5 for:
-             0000000000002d21 0000000000002d2f (DW_OP_reg0 (rax))
-    000016f7 v000000000000000 v000000000000000 views at 000016a7 for:
-             0000000000002d2f 0000000000002d3c (DW_OP_reg12 (r12))
-    0000170a v000000000000000 v000000000000000 views at 000016a9 for:
-             0000000000002d3c 0000000000002d41 (DW_OP_reg0 (rax))
-    0000171d <End of list>
-
-    0000172d v000000000000000 v000000000000002 location view pair
-    0000172f v000000000000002 v000000000000000 location view pair
-    00001731 v000000000000000 v000000000000002 location view pair
-    00001733 v000000000000002 v000000000000000 location view pair
-
-    00001735 v000000000000000 v000000000000002 views at 0000172d for:
-             0000000000002cd8 0000000000002cf9 (DW_OP_reg6 (rbp))
-    00001748 v000000000000002 v000000000000000 views at 0000172f for:
-             0000000000002cf9 0000000000002d13 (DW_OP_lit0; DW_OP_stack_value)
-    0000175c v000000000000000 v000000000000002 views at 00001731 for:
-             0000000000002d21 0000000000002d30 (DW_OP_reg6 (rbp))
-    0000176f v000000000000002 v000000000000000 views at 00001733 for:
-             0000000000002d30 0000000000002d35 (DW_OP_lit0; DW_OP_stack_value)
-    00001783 <End of list>
-
-    00001793 v000000000000006 v000000000000000 location view pair
-    00001795 v000000000000000 v000000000000000 location view pair
-
-    00001797 v000000000000006 v000000000000000 views at 00001793 for:
-             0000000000002cbf 0000000000002cca (DW_OP_breg5 (rdi): 16; DW_OP_deref; DW_OP_lit1; DW_OP_minus; DW_OP_stack_value)
-    000017af v000000000000000 v000000000000000 views at 00001795 for:
-             0000000000002cca 0000000000002d35 (DW_OP_reg3 (rbx))
-    000017c2 <End of list>
-
-    000017d2 v000000000000002 v000000000000000 location view pair
-    000017d4 v000000000000000 v000000000000000 location view pair
-
-    000017d6 v000000000000002 v000000000000000 views at 000017d2 for:
-             0000000000002cd8 0000000000002d13 (DW_OP_reg6 (rbp))
-    000017e9 v000000000000000 v000000000000000 views at 000017d4 for:
-             0000000000002d21 0000000000002d35 (DW_OP_reg6 (rbp))
-    000017fc <End of list>
-
-    0000180c v000000000000002 v000000000000000 location view pair
-    0000180e v000000000000000 v000000000000000 location view pair
-
-    00001810 v000000000000002 v000000000000000 views at 0000180c for:
-             0000000000002cf7 0000000000002cf9 (DW_OP_reg6 (rbp))
-    00001823 v000000000000000 v000000000000000 views at 0000180e for:
-             0000000000002d21 0000000000002d30 (DW_OP_reg6 (rbp))
-    00001836 <End of list>
-
-    00001846 v000000000000000 v000000000000000 location view pair
-    00001848 v000000000000004 v000000000000000 location view pair
-
-    0000184a v000000000000000 v000000000000000 views at 00001846 for:
-             0000000000002cca 0000000000002cee (DW_OP_breg14 (r14): 8)
-    0000185e v000000000000004 v000000000000000 views at 00001848 for:
-             0000000000002d13 0000000000002d21 (DW_OP_breg14 (r14): 8)
-    00001872 <End of list>
-
-    00001882 v000000000000003 v000000000000007 location view pair
-
-    00001884 v000000000000003 v000000000000007 views at 00001882 for:
-             0000000000002d13 0000000000002d13 (DW_OP_lit16; DW_OP_lit21; DW_OP_shl; DW_OP_stack_value)
-    0000189a <End of list>
-
-    000018aa v000000000000006 v000000000000007 location view pair
-
-    000018ac v000000000000006 v000000000000007 views at 000018aa for:
-             0000000000002d13 0000000000002d13 (DW_OP_breg14 (r14): 8; DW_OP_deref; DW_OP_plus_uconst: 168)
-    000018c4 <End of list>
-
-    000018d4 v000000000000000 v000000000000000 location view pair
-    000018d6 v000000000000000 v000000000000000 location view pair
-    000018d8 v000000000000000 v000000000000000 location view pair
-    000018da v000000000000000 v000000000000000 location view pair
-    000018dc v000000000000000 v000000000000000 location view pair
-    000018de v000000000000000 v000000000000000 location view pair
-    000018e0 v000000000000000 v000000000000000 location view pair
-    000018e2 v000000000000000 v000000000000000 location view pair
+    000015a8 v000000000000000 v000000000000000 views at 000015a0 for:
+             0000000000002ca0 0000000000002ccf (DW_OP_reg5 (rdi))
+    000015bb v000000000000000 v000000000000000 views at 000015a2 for:
+             0000000000002ccf 0000000000002d42 (DW_OP_reg14 (r14))
+    000015ce v000000000000000 v000000000000000 views at 000015a4 for:
+             0000000000002d42 0000000000002d4e (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
+    000015e4 v000000000000000 v000000000000000 views at 000015a6 for:
+             0000000000002d4e 0000000000002d57 (DW_OP_reg14 (r14))
+    000015f7 <End of list>
+
+    00001607 v000000000000000 v000000000000000 location view pair
+    00001609 v000000000000000 v000000000000000 location view pair
+
+    0000160b v000000000000000 v000000000000000 views at 00001607 for:
+             0000000000002ca0 0000000000002ccf (DW_OP_reg4 (rsi))
+    0000161e v000000000000000 v000000000000000 views at 00001609 for:
+             0000000000002ccf 0000000000002d57 (DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)); DW_OP_stack_value)
+    00001634 <End of list>
+
+    00001644 v000000000000000 v000000000000000 location view pair
+
+    00001646 v000000000000000 v000000000000000 views at 00001644 for:
+             0000000000002cac 0000000000002ccf (DW_OP_reg12 (r12))
+    00001659 <End of list>
+
+    00001669 v000000000000001 v000000000000000 location view pair
+    0000166b v000000000000000 v000000000000000 location view pair
+
+    0000166d v000000000000001 v000000000000000 views at 00001669 for:
+             0000000000002cb9 0000000000002d43 (DW_OP_reg3 (rbx))
+    00001680 v000000000000000 v000000000000000 views at 0000166b for:
+             0000000000002d4e 0000000000002d57 (DW_OP_reg3 (rbx))
+    00001693 <End of list>
+
+    000016a3 v000000000000009 v000000000000000 location view pair
+
+    000016a5 v000000000000009 v000000000000000 views at 000016a3 for:
+             0000000000002cc4 0000000000002ccf (DW_OP_breg5 (rdi): 16)
+    000016b9 <End of list>
+
+    000016c9 v00000000000000b v000000000000000 location view pair
+    000016cb v000000000000000 v000000000000000 location view pair
+    000016cd v000000000000000 v000000000000000 location view pair
+    000016cf v000000000000000 v000000000000000 location view pair
+    000016d1 v000000000000000 v000000000000000 location view pair
+
+    000016d3 v00000000000000b v000000000000000 views at 000016c9 for:
+             0000000000002cc4 0000000000002cf6 (DW_OP_reg12 (r12))
+    000016e6 v000000000000000 v000000000000000 views at 000016cb for:
+             0000000000002cf6 0000000000002cfc (DW_OP_reg0 (rax))
+    000016f9 v000000000000000 v000000000000000 views at 000016cd for:
+             0000000000002cfc 0000000000002d49 (DW_OP_reg12 (r12))
+    0000170c v000000000000000 v000000000000000 views at 000016cf for:
+             0000000000002d49 0000000000002d54 (DW_OP_reg0 (rax))
+    0000171f v000000000000000 v000000000000000 views at 000016d1 for:
+             0000000000002d54 0000000000002d57 (DW_OP_reg12 (r12))
+    00001732 <End of list>
+
+    00001742 v000000000000000 v000000000000002 location view pair
+    00001744 v000000000000002 v000000000000000 location view pair
+    00001746 v000000000000000 v000000000000002 location view pair
+    00001748 v000000000000002 v000000000000000 location view pair
+    0000174a v000000000000000 v000000000000000 location view pair
+
+    0000174c v000000000000000 v000000000000002 views at 00001742 for:
+             0000000000002cd8 0000000000002d03 (DW_OP_reg6 (rbp))
+    0000175f v000000000000002 v000000000000000 views at 00001744 for:
+             0000000000002d03 0000000000002d18 (DW_OP_lit0; DW_OP_stack_value)
+    00001773 v000000000000000 v000000000000002 views at 00001746 for:
+             0000000000002d26 0000000000002d3c (DW_OP_reg6 (rbp))
+    00001786 v000000000000002 v000000000000000 views at 00001748 for:
+             0000000000002d3c 0000000000002d42 (DW_OP_lit0; DW_OP_stack_value)
+    0000179a v000000000000000 v000000000000000 views at 0000174a for:
+             0000000000002d4e 0000000000002d57 (DW_OP_reg6 (rbp))
+    000017ad <End of list>
+
+    000017bd v00000000000000d v000000000000000 location view pair
+    000017bf v000000000000000 v000000000000000 location view pair
+    000017c1 v000000000000000 v000000000000005 location view pair
+    000017c3 v000000000000005 v000000000000000 location view pair
+    000017c5 v000000000000000 v000000000000000 location view pair
+
+    000017c7 v00000000000000d v000000000000000 views at 000017bd for:
+             0000000000002cc4 0000000000002ccf (DW_OP_breg5 (rdi): 16; DW_OP_deref; DW_OP_lit1; DW_OP_minus; DW_OP_stack_value)
+    000017df v000000000000000 v000000000000000 views at 000017bf for:
+             0000000000002ccf 0000000000002d37 (DW_OP_reg13 (r13))
+    000017f2 v000000000000000 v000000000000005 views at 000017c1 for:
+             0000000000002d37 0000000000002d3c (DW_OP_breg13 (r13): 1; DW_OP_stack_value)
+    00001807 v000000000000005 v000000000000000 views at 000017c3 for:
+             0000000000002d3c 0000000000002d42 (DW_OP_reg13 (r13))
+    0000181a v000000000000000 v000000000000000 views at 000017c5 for:
+             0000000000002d4e 0000000000002d57 (DW_OP_reg13 (r13))
+    0000182d <End of list>
+
+    0000183d v000000000000002 v000000000000000 location view pair
+    0000183f v000000000000000 v000000000000000 location view pair
+    00001841 v000000000000000 v000000000000000 location view pair
+
+    00001843 v000000000000002 v000000000000000 views at 0000183d for:
+             0000000000002cd8 0000000000002d18 (DW_OP_reg6 (rbp))
+    00001856 v000000000000000 v000000000000000 views at 0000183f for:
+             0000000000002d26 0000000000002d42 (DW_OP_reg6 (rbp))
+    00001869 v000000000000000 v000000000000000 views at 00001841 for:
+             0000000000002d4e 0000000000002d57 (DW_OP_reg6 (rbp))
+    0000187c <End of list>
+
+    0000188c v000000000000001 v000000000000000 location view pair
+    0000188e v000000000000000 v000000000000000 location view pair
+
+    00001890 v000000000000001 v000000000000000 views at 0000188c for:
+             0000000000002cf6 0000000000002cfc (DW_OP_reg5 (rdi))
+    000018a3 v000000000000000 v000000000000000 views at 0000188e for:
+             0000000000002d4e 0000000000002d54 (DW_OP_reg5 (rdi))
+    000018b6 <End of list>
+
+    000018c6 v000000000000003 v000000000000000 location view pair
+    000018c8 v000000000000000 v000000000000000 location view pair
+
+    000018ca v000000000000003 v000000000000000 views at 000018c6 for:
+             0000000000002cfc 0000000000002d03 (DW_OP_reg6 (rbp))
+    000018dd v000000000000000 v000000000000000 views at 000018c8 for:
+             0000000000002d26 0000000000002d3c (DW_OP_reg6 (rbp))
+    000018f0 <End of list>
+
+    00001900 v000000000000000 v000000000000000 location view pair
+    00001902 v000000000000004 v000000000000000 location view pair
+
+    00001904 v000000000000000 v000000000000000 views at 00001900 for:
+             0000000000002ccf 0000000000002cee (DW_OP_breg14 (r14): 8)
+    00001918 v000000000000004 v000000000000000 views at 00001902 for:
+             0000000000002d18 0000000000002d26 (DW_OP_breg14 (r14): 8)
+    0000192c <End of list>
+
+    0000193c v000000000000003 v000000000000007 location view pair
+
+    0000193e v000000000000003 v000000000000007 views at 0000193c for:
+             0000000000002d18 0000000000002d18 (DW_OP_lit16; DW_OP_lit21; DW_OP_shl; DW_OP_stack_value)
+    00001954 <End of list>
+
+    00001964 v000000000000006 v000000000000007 location view pair
+
+    00001966 v000000000000006 v000000000000007 views at 00001964 for:
+             0000000000002d18 0000000000002d18 (DW_OP_breg14 (r14): 8; DW_OP_deref; DW_OP_plus_uconst: 168)
+    0000197e <End of list>
+
+    0000198e v000000000000002 v000000000000000 location view pair
+    00001990 v000000000000001 v000000000000000 location view pair
+    00001992 v000000000000000 v000000000000000 location view pair
+    00001994 v000000000000000 v000000000000000 location view pair
+
+    00001996 v000000000000002 v000000000000000 views at 0000198e for:
+             0000000000002cac 0000000000002ccf (DW_OP_reg12 (r12))
+    000019a9 v000000000000001 v000000000000000 views at 00001990 for:
+             0000000000002cd8 0000000000002d18 (DW_OP_reg6 (rbp))
+    000019bc v000000000000000 v000000000000000 views at 00001992 for:
+             0000000000002d26 0000000000002d42 (DW_OP_reg6 (rbp))
+    000019cf v000000000000000 v000000000000000 views at 00001994 for:
+             0000000000002d4e 0000000000002d57 (DW_OP_reg6 (rbp))
+    000019e2 <End of list>
+
+    000019f2 v000000000000003 v000000000000009 location view pair
+
+    000019f4 v000000000000003 v000000000000009 views at 000019f2 for:
+             0000000000002cc4 0000000000002cc4 (DW_OP_reg5 (rdi))
+    00001a07 <End of list>
 
-    000018e4 v000000000000000 v000000000000000 views at 000018d4 for:
+    00001a17 v000000000000005 v000000000000000 location view pair
+    00001a19 v000000000000000 v000000000000000 location view pair
+    00001a1b v000000000000000 v000000000000000 location view pair
+    00001a1d v000000000000000 v000000000000000 location view pair
+
+    00001a1f v000000000000005 v000000000000000 views at 00001a17 for:
+             0000000000002cc4 0000000000002ccf (DW_OP_reg5 (rdi))
+    00001a32 v000000000000000 v000000000000000 views at 00001a19 for:
+             0000000000002ccf 0000000000002d42 (DW_OP_reg14 (r14))
+    00001a45 v000000000000000 v000000000000000 views at 00001a1b for:
+             0000000000002d42 0000000000002d4e (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
+    00001a5b v000000000000000 v000000000000000 views at 00001a1d for:
+             0000000000002d4e 0000000000002d57 (DW_OP_reg14 (r14))
+    00001a6e <End of list>
+
+    00001a7e v000000000000006 v000000000000009 location view pair
+
+    00001a80 v000000000000006 v000000000000009 views at 00001a7e for:
+             0000000000002cc4 0000000000002cc4 (DW_OP_reg5 (rdi))
+    00001a93 <End of list>
+
+    00001aa3 v000000000000008 v000000000000000 location view pair
+    00001aa5 v000000000000000 v000000000000000 location view pair
+    00001aa7 v000000000000000 v000000000000000 location view pair
+    00001aa9 v000000000000000 v000000000000000 location view pair
+
+    00001aab v000000000000008 v000000000000000 views at 00001aa3 for:
+             0000000000002cc4 0000000000002ccf (DW_OP_reg5 (rdi))
+    00001abe v000000000000000 v000000000000000 views at 00001aa5 for:
+             0000000000002ccf 0000000000002d42 (DW_OP_reg14 (r14))
+    00001ad1 v000000000000000 v000000000000000 views at 00001aa7 for:
+             0000000000002d42 0000000000002d4e (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
+    00001ae7 v000000000000000 v000000000000000 views at 00001aa9 for:
+             0000000000002d4e 0000000000002d57 (DW_OP_reg14 (r14))
+    00001afa <End of list>
+
+    00001b0a v000000000000000 v000000000000000 location view pair
+    00001b0c v000000000000000 v000000000000000 location view pair
+    00001b0e v000000000000000 v000000000000000 location view pair
+    00001b10 v000000000000000 v000000000000000 location view pair
+    00001b12 v000000000000000 v000000000000000 location view pair
+    00001b14 v000000000000000 v000000000000000 location view pair
+    00001b16 v000000000000000 v000000000000000 location view pair
+    00001b18 v000000000000000 v000000000000000 location view pair
+
+    00001b1a v000000000000000 v000000000000000 views at 00001b0a for:
              0000000000002590 000000000000259e (DW_OP_reg5 (rdi))
-    000018f7 v000000000000000 v000000000000000 views at 000018d6 for:
+    00001b2d v000000000000000 v000000000000000 views at 00001b0c for:
              000000000000259e 00000000000025cd (DW_OP_reg6 (rbp))
-    0000190a v000000000000000 v000000000000000 views at 000018d8 for:
+    00001b40 v000000000000000 v000000000000000 views at 00001b0e for:
              00000000000025cd 00000000000025d0 (DW_OP_reg5 (rdi))
-    0000191d v000000000000000 v000000000000000 views at 000018da for:
+    00001b53 v000000000000000 v000000000000000 views at 00001b10 for:
              00000000000025d0 00000000000025d1 (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
-    00001933 v000000000000000 v000000000000000 views at 000018dc for:
+    00001b69 v000000000000000 v000000000000000 views at 00001b12 for:
              00000000000025d1 0000000000002611 (DW_OP_reg6 (rbp))
-    00001946 v000000000000000 v000000000000000 views at 000018de for:
+    00001b7c v000000000000000 v000000000000000 views at 00001b14 for:
              0000000000002611 0000000000002618 (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
-    0000195c v000000000000000 v000000000000000 views at 000018e0 for:
+    00001b92 v000000000000000 v000000000000000 views at 00001b16 for:
              0000000000002618 0000000000002625 (DW_OP_reg6 (rbp))
-    0000196f v000000000000000 v000000000000000 views at 000018e2 for:
+    00001ba5 v000000000000000 v000000000000000 views at 00001b18 for:
              0000000000002625 0000000000002628 (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
-    00001985 <End of list>
+    00001bbb <End of list>
 
-    00001995 v000000000000002 v000000000000000 location view pair
-    00001997 v000000000000000 v000000000000000 location view pair
-    00001999 v000000000000000 v000000000000000 location view pair
-    0000199b v000000000000000 v000000000000000 location view pair
-    0000199d v000000000000000 v000000000000000 location view pair
+    00001bcb v000000000000002 v000000000000000 location view pair
+    00001bcd v000000000000000 v000000000000000 location view pair
+    00001bcf v000000000000000 v000000000000000 location view pair
+    00001bd1 v000000000000000 v000000000000000 location view pair
+    00001bd3 v000000000000000 v000000000000000 location view pair
 
-    0000199f v000000000000002 v000000000000000 views at 00001995 for:
+    00001bd5 v000000000000002 v000000000000000 views at 00001bcb for:
              000000000000259f 00000000000025e6 (DW_OP_lit0; DW_OP_stack_value)
-    000019b3 v000000000000000 v000000000000000 views at 00001997 for:
+    00001be9 v000000000000000 v000000000000000 views at 00001bcd for:
              00000000000025e6 00000000000025ea (DW_OP_reg0 (rax))
-    000019c6 v000000000000000 v000000000000000 views at 00001999 for:
+    00001bfc v000000000000000 v000000000000000 views at 00001bcf for:
              00000000000025ea 0000000000002613 (DW_OP_reg12 (r12))
-    000019d9 v000000000000000 v000000000000000 views at 0000199b for:
+    00001c0f v000000000000000 v000000000000000 views at 00001bd1 for:
              0000000000002613 0000000000002617 (DW_OP_reg5 (rdi))
-    000019ec v000000000000000 v000000000000000 views at 0000199d for:
+    00001c22 v000000000000000 v000000000000000 views at 00001bd3 for:
              0000000000002618 0000000000002627 (DW_OP_reg12 (r12))
-    000019ff <End of list>
+    00001c35 <End of list>
 
-    00001a0f v000000000000000 v000000000000000 location view pair
-    00001a11 v000000000000000 v000000000000000 location view pair
-    00001a13 v000000000000000 v000000000000000 location view pair
-    00001a15 v000000000000000 v000000000000000 location view pair
-    00001a17 v000000000000000 v000000000000000 location view pair
-    00001a19 v000000000000000 v000000000000000 location view pair
+    00001c45 v000000000000000 v000000000000000 location view pair
+    00001c47 v000000000000000 v000000000000000 location view pair
+    00001c49 v000000000000000 v000000000000000 location view pair
+    00001c4b v000000000000000 v000000000000000 location view pair
+    00001c4d v000000000000000 v000000000000000 location view pair
+    00001c4f v000000000000000 v000000000000000 location view pair
 
-    00001a1b v000000000000000 v000000000000000 views at 00001a0f for:
+    00001c51 v000000000000000 v000000000000000 views at 00001c45 for:
              0000000000002530 0000000000002538 (DW_OP_reg5 (rdi))
-    00001a2e v000000000000000 v000000000000000 views at 00001a11 for:
+    00001c64 v000000000000000 v000000000000000 views at 00001c47 for:
              0000000000002538 0000000000002565 (DW_OP_reg3 (rbx))
-    00001a41 v000000000000000 v000000000000000 views at 00001a13 for:
+    00001c77 v000000000000000 v000000000000000 views at 00001c49 for:
              0000000000002565 0000000000002566 (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
-    00001a57 v000000000000000 v000000000000000 views at 00001a15 for:
+    00001c8d v000000000000000 v000000000000000 views at 00001c4b for:
              0000000000002566 0000000000002578 (DW_OP_reg3 (rbx))
-    00001a6a v000000000000000 v000000000000000 views at 00001a17 for:
+    00001ca0 v000000000000000 v000000000000000 views at 00001c4d for:
              0000000000002578 0000000000002579 (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
-    00001a80 v000000000000000 v000000000000000 views at 00001a19 for:
+    00001cb6 v000000000000000 v000000000000000 views at 00001c4f for:
              0000000000002579 0000000000002587 (DW_OP_reg3 (rbx))
-    00001a93 <End of list>
+    00001cc9 <End of list>
 
-    00001aa3 v000000000000000 v000000000000000 location view pair
-    00001aa5 v000000000000000 v000000000000000 location view pair
+    00001cd9 v000000000000000 v000000000000000 location view pair
+    00001cdb v000000000000000 v000000000000000 location view pair
 
-    00001aa7 v000000000000000 v000000000000000 views at 00001aa3 for:
+    00001cdd v000000000000000 v000000000000000 views at 00001cd9 for:
              0000000000002538 000000000000254b (DW_OP_reg5 (rdi))
-    00001aba v000000000000000 v000000000000000 views at 00001aa5 for:
+    00001cf0 v000000000000000 v000000000000000 views at 00001cdb for:
              0000000000002579 0000000000002584 (DW_OP_reg5 (rdi))
-    00001acd <End of list>
+    00001d03 <End of list>
 
-    00001add v000000000000001 v000000000000000 location view pair
-    00001adf v000000000000000 v000000000000000 location view pair
+    00001d13 v000000000000001 v000000000000000 location view pair
+    00001d15 v000000000000000 v000000000000000 location view pair
 
-    00001ae1 v000000000000001 v000000000000000 views at 00001add for:
+    00001d17 v000000000000001 v000000000000000 views at 00001d13 for:
              0000000000002545 000000000000254b (DW_OP_reg5 (rdi))
-    00001af4 v000000000000000 v000000000000000 views at 00001adf for:
+    00001d2a v000000000000000 v000000000000000 views at 00001d15 for:
              0000000000002579 0000000000002584 (DW_OP_reg5 (rdi))
-    00001b07 <End of list>
+    00001d3d <End of list>
 
-    00001b17 v000000000000000 v000000000000000 location view pair
+    00001d4d v000000000000000 v000000000000000 location view pair
 
-    00001b19 v000000000000000 v000000000000000 views at 00001b17 for:
+    00001d4f v000000000000000 v000000000000000 views at 00001d4d for:
              000000000000254f 0000000000002574 (DW_OP_reg5 (rdi))
-    00001b2c <End of list>
+    00001d62 <End of list>
 
-    00001b3c v000000000000001 v000000000000000 location view pair
-    00001b3e v000000000000000 v000000000000000 location view pair
+    00001d72 v000000000000001 v000000000000000 location view pair
+    00001d74 v000000000000000 v000000000000000 location view pair
 
-    00001b40 v000000000000001 v000000000000000 views at 00001b3c for:
+    00001d76 v000000000000001 v000000000000000 views at 00001d72 for:
              000000000000255c 0000000000002562 (DW_OP_reg5 (rdi))
-    00001b53 v000000000000000 v000000000000000 views at 00001b3e for:
+    00001d89 v000000000000000 v000000000000000 views at 00001d74 for:
              0000000000002566 0000000000002574 (DW_OP_reg5 (rdi))
-    00001b66 <End of list>
+    00001d9c <End of list>
 
-    00001b76 v000000000000000 v000000000000000 location view pair
-    00001b78 v000000000000000 v000000000000000 location view pair
-    00001b7a v000000000000000 v000000000000000 location view pair
-    00001b7c v000000000000000 v000000000000000 location view pair
+    00001dac v000000000000000 v000000000000000 location view pair
+    00001dae v000000000000000 v000000000000000 location view pair
+    00001db0 v000000000000000 v000000000000000 location view pair
+    00001db2 v000000000000000 v000000000000000 location view pair
 
-    00001b7e v000000000000000 v000000000000000 views at 00001b76 for:
+    00001db4 v000000000000000 v000000000000000 views at 00001dac for:
              0000000000002400 000000000000242b (DW_OP_reg5 (rdi))
-    00001b91 v000000000000000 v000000000000000 views at 00001b78 for:
+    00001dc7 v000000000000000 v000000000000000 views at 00001dae for:
              000000000000242b 00000000000024cd (DW_OP_reg6 (rbp))
-    00001ba4 v000000000000000 v000000000000000 views at 00001b7a for:
+    00001dda v000000000000000 v000000000000000 views at 00001db0 for:
              00000000000024cd 00000000000024d4 (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
-    00001bba v000000000000000 v000000000000000 views at 00001b7c for:
+    00001df0 v000000000000000 v000000000000000 views at 00001db2 for:
              00000000000024d4 0000000000002527 (DW_OP_reg6 (rbp))
-    00001bcd <End of list>
+    00001e03 <End of list>
 
-    00001bdd v000000000000000 v000000000000000 location view pair
-    00001bdf v000000000000000 v000000000000000 location view pair
-    00001be1 v000000000000000 v000000000000000 location view pair
-    00001be3 v000000000000000 v000000000000000 location view pair
+    00001e13 v000000000000000 v000000000000000 location view pair
+    00001e15 v000000000000000 v000000000000000 location view pair
+    00001e17 v000000000000000 v000000000000000 location view pair
+    00001e19 v000000000000000 v000000000000000 location view pair
 
-    00001be5 v000000000000000 v000000000000000 views at 00001bdd for:
+    00001e1b v000000000000000 v000000000000000 views at 00001e13 for:
              0000000000002400 000000000000240c (DW_OP_reg4 (rsi))
-    00001bf8 v000000000000000 v000000000000000 views at 00001bdf for:
+    00001e2e v000000000000000 v000000000000000 views at 00001e15 for:
              000000000000240c 00000000000024d1 (DW_OP_reg13 (r13))
-    00001c0b v000000000000000 v000000000000000 views at 00001be1 for:
+    00001e41 v000000000000000 v000000000000000 views at 00001e17 for:
              00000000000024d1 00000000000024d4 (DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)); DW_OP_stack_value)
-    00001c21 v000000000000000 v000000000000000 views at 00001be3 for:
+    00001e57 v000000000000000 v000000000000000 views at 00001e19 for:
              00000000000024d4 0000000000002527 (DW_OP_reg13 (r13))
-    00001c34 <End of list>
+    00001e6a <End of list>
 
-    00001c44 v000000000000000 v000000000000000 location view pair
-    00001c46 v000000000000000 v000000000000000 location view pair
-    00001c48 v000000000000000 v000000000000000 location view pair
-    00001c4a v000000000000000 v000000000000000 location view pair
+    00001e7a v000000000000000 v000000000000000 location view pair
+    00001e7c v000000000000000 v000000000000000 location view pair
+    00001e7e v000000000000000 v000000000000000 location view pair
+    00001e80 v000000000000000 v000000000000000 location view pair
 
-    00001c4c v000000000000000 v000000000000000 views at 00001c44 for:
+    00001e82 v000000000000000 v000000000000000 views at 00001e7a for:
              0000000000002400 000000000000242b (DW_OP_reg1 (rdx))
-    00001c5f v000000000000000 v000000000000000 views at 00001c46 for:
+    00001e95 v000000000000000 v000000000000000 views at 00001e7c for:
              000000000000242b 00000000000024d3 (DW_OP_reg14 (r14))
-    00001c72 v000000000000000 v000000000000000 views at 00001c48 for:
+    00001ea8 v000000000000000 v000000000000000 views at 00001e7e for:
              00000000000024d3 00000000000024d4 (DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)); DW_OP_stack_value)
-    00001c88 v000000000000000 v000000000000000 views at 00001c4a for:
+    00001ebe v000000000000000 v000000000000000 views at 00001e80 for:
              00000000000024d4 0000000000002527 (DW_OP_reg14 (r14))
-    00001c9b <End of list>
+    00001ed1 <End of list>
 
-    00001cab v000000000000000 v000000000000000 location view pair
-    00001cad v000000000000000 v000000000000001 location view pair
-    00001caf v000000000000000 v000000000000000 location view pair
-    00001cb1 v000000000000000 v000000000000000 location view pair
+    00001ee1 v000000000000000 v000000000000000 location view pair
+    00001ee3 v000000000000000 v000000000000001 location view pair
+    00001ee5 v000000000000000 v000000000000000 location view pair
+    00001ee7 v000000000000000 v000000000000000 location view pair
 
-    00001cb3 v000000000000000 v000000000000000 views at 00001cab for:
+    00001ee9 v000000000000000 v000000000000000 views at 00001ee1 for:
              000000000000242c 000000000000243f (DW_OP_reg0 (rax))
-    00001cc6 v000000000000000 v000000000000001 views at 00001cad for:
+    00001efc v000000000000000 v000000000000001 views at 00001ee3 for:
              000000000000243f 00000000000024b5 (DW_OP_reg12 (r12))
-    00001cd9 v000000000000000 v000000000000000 views at 00001caf for:
+    00001f0f v000000000000000 v000000000000000 views at 00001ee5 for:
              00000000000024d4 00000000000024e7 (DW_OP_reg12 (r12))
-    00001cec v000000000000000 v000000000000000 views at 00001cb1 for:
+    00001f22 v000000000000000 v000000000000000 views at 00001ee7 for:
              00000000000024f5 0000000000002522 (DW_OP_reg12 (r12))
-    00001cff <End of list>
+    00001f35 <End of list>
 
-    00001d0f v000000000000000 v000000000000000 location view pair
-    00001d11 v000000000000000 v000000000000000 location view pair
+    00001f45 v000000000000000 v000000000000000 location view pair
+    00001f47 v000000000000000 v000000000000000 location view pair
 
-    00001d13 v000000000000000 v000000000000000 views at 00001d0f for:
+    00001f49 v000000000000000 v000000000000000 views at 00001f45 for:
              000000000000247b 000000000000249e (DW_OP_reg0 (rax))
-    00001d26 v000000000000000 v000000000000000 views at 00001d11 for:
+    00001f5c v000000000000000 v000000000000000 views at 00001f47 for:
              00000000000024f5 000000000000250e (DW_OP_reg0 (rax))
-    00001d39 <End of list>
+    00001f6f <End of list>
 
-    00001d49 v000000000000001 v000000000000000 location view pair
-    00001d4b v000000000000000 v000000000000000 location view pair
+    00001f7f v000000000000001 v000000000000000 location view pair
+    00001f81 v000000000000000 v000000000000000 location view pair
 
-    00001d4d v000000000000001 v000000000000000 views at 00001d49 for:
+    00001f83 v000000000000001 v000000000000000 views at 00001f7f for:
              0000000000002480 000000000000249e (DW_OP_breg0 (rax): 16)
-    00001d61 v000000000000000 v000000000000000 views at 00001d4b for:
+    00001f97 v000000000000000 v000000000000000 views at 00001f81 for:
              00000000000024f5 000000000000250e (DW_OP_breg0 (rax): 16)
-    00001d75 <End of list>
+    00001fab <End of list>
 
-    00001d85 v000000000000001 v000000000000005 location view pair
+    00001fbb v000000000000001 v000000000000005 location view pair
 
-    00001d87 v000000000000001 v000000000000005 views at 00001d85 for:
+    00001fbd v000000000000001 v000000000000005 views at 00001fbb for:
              000000000000248b 000000000000248b (DW_OP_breg0 (rax): 16)
-    00001d9b <End of list>
+    00001fd1 <End of list>
 
-    00001dab v000000000000001 v000000000000005 location view pair
+    00001fe1 v000000000000001 v000000000000005 location view pair
 
-    00001dad v000000000000001 v000000000000005 views at 00001dab for:
+    00001fe3 v000000000000001 v000000000000005 views at 00001fe1 for:
              000000000000248b 000000000000248b (DW_OP_reg1 (rdx))
-    00001dc0 <End of list>
+    00001ff6 <End of list>
 
-    00001dd0 v000000000000001 v000000000000001 location view pair
-    00001dd2 v000000000000001 v000000000000001 location view pair
+    00002006 v000000000000001 v000000000000001 location view pair
+    00002008 v000000000000001 v000000000000001 location view pair
 
-    00001dd4 v000000000000001 v000000000000001 views at 00001dd0 for:
+    0000200a v000000000000001 v000000000000001 views at 00002006 for:
              00000000000024a3 00000000000024ac (DW_OP_reg0 (rax))
-    00001de7 v000000000000001 v000000000000001 views at 00001dd2 for:
+    0000201d v000000000000001 v000000000000001 views at 00002008 for:
              00000000000024ac 00000000000024b5 (DW_OP_reg1 (rdx))
-    00001dfa <End of list>
+    00002030 <End of list>
 
-    00001e0a v000000000000002 v000000000000001 location view pair
+    00002040 v000000000000002 v000000000000001 location view pair
 
-    00001e0c v000000000000002 v000000000000001 views at 00001e0a for:
+    00002042 v000000000000002 v000000000000001 views at 00002040 for:
              00000000000024ac 00000000000024b5 (DW_OP_reg1 (rdx))
-    00001e1f <End of list>
+    00002055 <End of list>
 
-    00001e2f v000000000000002 v000000000000000 location view pair
+    00002065 v000000000000002 v000000000000000 location view pair
 
-    00001e31 v000000000000002 v000000000000000 views at 00001e2f for:
+    00002067 v000000000000002 v000000000000000 views at 00002065 for:
              00000000000024d4 00000000000024e7 (DW_OP_reg12 (r12))
-    00001e44 <End of list>
+    0000207a <End of list>
 
-    00001e54 v000000000000000 v000000000000000 location view pair
-    00001e56 v000000000000000 v000000000000000 location view pair
+    0000208a v000000000000000 v000000000000000 location view pair
+    0000208c v000000000000000 v000000000000000 location view pair
 
-    00001e58 v000000000000000 v000000000000000 views at 00001e54 for:
+    0000208e v000000000000000 v000000000000000 views at 0000208a for:
              00000000000023f0 00000000000023f7 (DW_OP_reg5 (rdi))
-    00001e6b v000000000000000 v000000000000000 views at 00001e56 for:
+    000020a1 v000000000000000 v000000000000000 views at 0000208c for:
              00000000000023f7 00000000000023fc (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
-    00001e81 <End of list>
+    000020b7 <End of list>
 
-    00001e91 v000000000000000 v000000000000000 location view pair
-    00001e93 v000000000000000 v000000000000000 location view pair
+    000020c7 v000000000000000 v000000000000000 location view pair
+    000020c9 v000000000000000 v000000000000000 location view pair
 
-    00001e95 v000000000000000 v000000000000000 views at 00001e91 for:
+    000020cb v000000000000000 v000000000000000 views at 000020c7 for:
              00000000000023c0 00000000000023c4 (DW_OP_reg5 (rdi))
-    00001ea8 v000000000000000 v000000000000000 views at 00001e93 for:
+    000020de v000000000000000 v000000000000000 views at 000020c9 for:
              00000000000023c4 00000000000023db (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
-    00001ebe <End of list>
+    000020f4 <End of list>
 
-    00001ece v000000000000000 v000000000000000 location view pair
-    00001ed0 v000000000000000 v000000000000000 location view pair
-    00001ed2 v000000000000000 v000000000000000 location view pair
-    00001ed4 v000000000000000 v000000000000000 location view pair
-    00001ed6 v000000000000000 v000000000000000 location view pair
+    00002104 v000000000000000 v000000000000000 location view pair
+    00002106 v000000000000000 v000000000000000 location view pair
+    00002108 v000000000000000 v000000000000000 location view pair
+    0000210a v000000000000000 v000000000000000 location view pair
+    0000210c v000000000000000 v000000000000000 location view pair
 
-    00001ed8 v000000000000000 v000000000000000 views at 00001ece for:
+    0000210e v000000000000000 v000000000000000 views at 00002104 for:
              00000000000023c0 00000000000023ca (DW_OP_reg4 (rsi))
-    00001eeb v000000000000000 v000000000000000 views at 00001ed0 for:
+    00002121 v000000000000000 v000000000000000 views at 00002106 for:
              00000000000023ca 00000000000023d0 (DW_OP_reg0 (rax))
-    00001efe v000000000000000 v000000000000000 views at 00001ed2 for:
+    00002134 v000000000000000 v000000000000000 views at 00002108 for:
              00000000000023d0 00000000000023d1 (DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)); DW_OP_stack_value)
-    00001f14 v000000000000000 v000000000000000 views at 00001ed4 for:
+    0000214a v000000000000000 v000000000000000 views at 0000210a for:
              00000000000023d1 00000000000023da (DW_OP_reg0 (rax))
-    00001f27 v000000000000000 v000000000000000 views at 00001ed6 for:
+    0000215d v000000000000000 v000000000000000 views at 0000210c for:
              00000000000023da 00000000000023db (DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)); DW_OP_stack_value)
-    00001f3d <End of list>
+    00002173 <End of list>
 
-    00001f4d v000000000000000 v000000000000000 location view pair
-    00001f4f v000000000000000 v000000000000000 location view pair
-    00001f51 v000000000000000 v000000000000000 location view pair
+    00002183 v000000000000000 v000000000000000 location view pair
+    00002185 v000000000000000 v000000000000000 location view pair
+    00002187 v000000000000000 v000000000000000 location view pair
 
-    00001f53 v000000000000000 v000000000000000 views at 00001f4d for:
+    00002189 v000000000000000 v000000000000000 views at 00002183 for:
              00000000000023c0 00000000000023d0 (DW_OP_reg1 (rdx))
-    00001f66 v000000000000000 v000000000000000 views at 00001f4f for:
+    0000219c v000000000000000 v000000000000000 views at 00002185 for:
              00000000000023d0 00000000000023d1 (DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)); DW_OP_stack_value)
-    00001f7c v000000000000000 v000000000000000 views at 00001f51 for:
+    000021b2 v000000000000000 v000000000000000 views at 00002187 for:
              00000000000023d1 00000000000023db (DW_OP_reg1 (rdx))
-    00001f8f <End of list>
+    000021c5 <End of list>
 
-    00001f9f v000000000000000 v000000000000000 location view pair
-    00001fa1 v000000000000000 v000000000000000 location view pair
-    00001fa3 v000000000000000 v000000000000000 location view pair
-    00001fa5 v000000000000000 v000000000000000 location view pair
-    00001fa7 v000000000000000 v000000000000000 location view pair
+    000021d5 v000000000000000 v000000000000000 location view pair
+    000021d7 v000000000000000 v000000000000000 location view pair
+    000021d9 v000000000000000 v000000000000000 location view pair
+    000021db v000000000000000 v000000000000000 location view pair
+    000021dd v000000000000000 v000000000000000 location view pair
 
-    00001fa9 v000000000000000 v000000000000000 views at 00001f9f for:
+    000021df v000000000000000 v000000000000000 views at 000021d5 for:
              0000000000002b40 0000000000002b51 (DW_OP_reg5 (rdi))
-    00001fbc v000000000000000 v000000000000000 views at 00001fa1 for:
+    000021f2 v000000000000000 v000000000000000 views at 000021d7 for:
              0000000000002b51 0000000000002b7d (DW_OP_reg3 (rbx))
-    00001fcf v000000000000000 v000000000000000 views at 00001fa3 for:
+    00002205 v000000000000000 v000000000000000 views at 000021d9 for:
              0000000000002b7d 0000000000002b88 (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
-    00001fe5 v000000000000000 v000000000000000 views at 00001fa5 for:
+    0000221b v000000000000000 v000000000000000 views at 000021db for:
              0000000000002b88 0000000000002b91 (DW_OP_reg3 (rbx))
-    00001ff8 v000000000000000 v000000000000000 views at 00001fa7 for:
+    0000222e v000000000000000 v000000000000000 views at 000021dd for:
              0000000000002b91 0000000000002b95 (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
-    0000200e <End of list>
+    00002244 <End of list>
 
-    0000201e v000000000000000 v000000000000000 location view pair
-    00002020 v000000000000000 v000000000000000 location view pair
-    00002022 v000000000000000 v000000000000000 location view pair
-    00002024 v000000000000000 v000000000000000 location view pair
-    00002026 v000000000000000 v000000000000000 location view pair
-    00002028 v000000000000000 v000000000000000 location view pair
+    00002254 v000000000000000 v000000000000000 location view pair
+    00002256 v000000000000000 v000000000000000 location view pair
+    00002258 v000000000000000 v000000000000000 location view pair
+    0000225a v000000000000000 v000000000000000 location view pair
+    0000225c v000000000000000 v000000000000000 location view pair
+    0000225e v000000000000000 v000000000000000 location view pair
 
-    0000202a v000000000000000 v000000000000000 views at 0000201e for:
+    00002260 v000000000000000 v000000000000000 views at 00002254 for:
              0000000000002b40 0000000000002b59 (DW_OP_reg4 (rsi))
-    0000203d v000000000000000 v000000000000000 views at 00002020 for:
+    00002273 v000000000000000 v000000000000000 views at 00002256 for:
              0000000000002b59 0000000000002b84 (DW_OP_reg6 (rbp))
-    00002050 v000000000000000 v000000000000000 views at 00002022 for:
+    00002286 v000000000000000 v000000000000000 views at 00002258 for:
              0000000000002b84 0000000000002b87 (DW_OP_reg0 (rax))
-    00002063 v000000000000000 v000000000000000 views at 00002024 for:
+    00002299 v000000000000000 v000000000000000 views at 0000225a for:
              0000000000002b87 0000000000002b88 (DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)); DW_OP_stack_value)
-    00002079 v000000000000000 v000000000000000 views at 00002026 for:
+    000022af v000000000000000 v000000000000000 views at 0000225c for:
              0000000000002b88 0000000000002b92 (DW_OP_reg6 (rbp))
-    0000208c v000000000000000 v000000000000000 views at 00002028 for:
+    000022c2 v000000000000000 v000000000000000 views at 0000225e for:
              0000000000002b92 0000000000002b95 (DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)); DW_OP_stack_value)
-    000020a2 <End of list>
+    000022d8 <End of list>
 
-    000020b2 v000000000000000 v000000000000000 location view pair
-    000020b4 v000000000000000 v000000000000000 location view pair
-    000020b6 v000000000000000 v000000000000000 location view pair
-    000020b8 v000000000000000 v000000000000000 location view pair
-    000020ba v000000000000000 v000000000000000 location view pair
-    000020bc v000000000000000 v000000000000000 location view pair
+    000022e8 v000000000000000 v000000000000000 location view pair
+    000022ea v000000000000000 v000000000000000 location view pair
+    000022ec v000000000000000 v000000000000000 location view pair
+    000022ee v000000000000000 v000000000000000 location view pair
+    000022f0 v000000000000000 v000000000000000 location view pair
+    000022f2 v000000000000000 v000000000000000 location view pair
 
-    000020be v000000000000000 v000000000000000 views at 000020b2 for:
+    000022f4 v000000000000000 v000000000000000 views at 000022e8 for:
              0000000000002b40 0000000000002b5a (DW_OP_reg1 (rdx))
-    000020d1 v000000000000000 v000000000000000 views at 000020b4 for:
+    00002307 v000000000000000 v000000000000000 views at 000022ea for:
              0000000000002b5a 0000000000002b86 (DW_OP_reg12 (r12))
-    000020e4 v000000000000000 v000000000000000 views at 000020b6 for:
+    0000231a v000000000000000 v000000000000000 views at 000022ec for:
              0000000000002b86 0000000000002b87 (DW_OP_reg4 (rsi))
-    000020f7 v000000000000000 v000000000000000 views at 000020b8 for:
+    0000232d v000000000000000 v000000000000000 views at 000022ee for:
              0000000000002b87 0000000000002b88 (DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)); DW_OP_stack_value)
-    0000210d v000000000000000 v000000000000000 views at 000020ba for:
+    00002343 v000000000000000 v000000000000000 views at 000022f0 for:
              0000000000002b88 0000000000002b94 (DW_OP_reg12 (r12))
-    00002120 v000000000000000 v000000000000000 views at 000020bc for:
+    00002356 v000000000000000 v000000000000000 views at 000022f2 for:
              0000000000002b94 0000000000002b95 (DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)); DW_OP_stack_value)
-    00002136 <End of list>
+    0000236c <End of list>
 
-    00002146 v000000000000000 v000000000000000 location view pair
+    0000237c v000000000000000 v000000000000000 location view pair
 
-    00002148 v000000000000000 v000000000000000 views at 00002146 for:
+    0000237e v000000000000000 v000000000000000 views at 0000237c for:
              0000000000002b5b 0000000000002b5f (DW_OP_reg0 (rax))
-    0000215b <End of list>
+    00002391 <End of list>
 
-    0000216b v000000000000000 v000000000000000 location view pair
+    000023a1 v000000000000000 v000000000000000 location view pair
 
-    0000216d v000000000000000 v000000000000000 views at 0000216b for:
+    000023a3 v000000000000000 v000000000000000 views at 000023a1 for:
              0000000000002b6d 0000000000002b71 (DW_OP_reg0 (rax))
-    00002180 <End of list>
+    000023b6 <End of list>
 
-    00002190 v000000000000000 v000000000000000 location view pair
-    00002192 v000000000000000 v000000000000000 location view pair
-    00002194 v000000000000000 v000000000000000 location view pair
+    000023c6 v000000000000000 v000000000000000 location view pair
+    000023c8 v000000000000000 v000000000000000 location view pair
+    000023ca v000000000000000 v000000000000000 location view pair
 
-    00002196 v000000000000000 v000000000000000 views at 00002190 for:
+    000023cc v000000000000000 v000000000000000 views at 000023c6 for:
              0000000000002b71 0000000000002b86 (DW_OP_reg12 (r12))
-    000021a9 v000000000000000 v000000000000000 views at 00002192 for:
+    000023df v000000000000000 v000000000000000 views at 000023c8 for:
              0000000000002b86 0000000000002b87 (DW_OP_reg4 (rsi))
-    000021bc v000000000000000 v000000000000000 views at 00002194 for:
+    000023f2 v000000000000000 v000000000000000 views at 000023ca for:
              0000000000002b87 0000000000002b88 (DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)); DW_OP_stack_value)
-    000021d2 <End of list>
+    00002408 <End of list>
 
-    000021e2 v000000000000000 v000000000000000 location view pair
-    000021e4 v000000000000000 v000000000000000 location view pair
-    000021e6 v000000000000000 v000000000000000 location view pair
+    00002418 v000000000000000 v000000000000000 location view pair
+    0000241a v000000000000000 v000000000000000 location view pair
+    0000241c v000000000000000 v000000000000000 location view pair
 
-    000021e8 v000000000000000 v000000000000000 views at 000021e2 for:
+    0000241e v000000000000000 v000000000000000 views at 00002418 for:
              0000000000002b71 0000000000002b84 (DW_OP_reg6 (rbp))
-    000021fb v000000000000000 v000000000000000 views at 000021e4 for:
+    00002431 v000000000000000 v000000000000000 views at 0000241a for:
              0000000000002b84 0000000000002b87 (DW_OP_reg0 (rax))
-    0000220e v000000000000000 v000000000000000 views at 000021e6 for:
+    00002444 v000000000000000 v000000000000000 views at 0000241c for:
              0000000000002b87 0000000000002b88 (DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)); DW_OP_stack_value)
-    00002224 <End of list>
+    0000245a <End of list>
 
-    00002234 v000000000000000 v000000000000000 location view pair
-    00002236 v000000000000000 v000000000000000 location view pair
+    0000246a v000000000000000 v000000000000000 location view pair
+    0000246c v000000000000000 v000000000000000 location view pair
 
-    00002238 v000000000000000 v000000000000000 views at 00002234 for:
+    0000246e v000000000000000 v000000000000000 views at 0000246a for:
              0000000000002b71 0000000000002b7d (DW_OP_reg3 (rbx))
-    0000224b v000000000000000 v000000000000000 views at 00002236 for:
+    00002481 v000000000000000 v000000000000000 views at 0000246c for:
              0000000000002b7d 0000000000002b88 (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
-    00002261 <End of list>
+    00002497 <End of list>
 
-    00002271 v000000000000000 v000000000000000 location view pair
-    00002273 v000000000000000 v000000000000000 location view pair
-    00002275 v000000000000000 v000000000000000 location view pair
-    00002277 v000000000000000 v000000000000000 location view pair
-    00002279 v000000000000000 v000000000000000 location view pair
-    0000227b v000000000000000 v000000000000000 location view pair
-    0000227d v000000000000000 v000000000000000 location view pair
+    000024a7 v000000000000000 v000000000000000 location view pair
+    000024a9 v000000000000000 v000000000000000 location view pair
+    000024ab v000000000000000 v000000000000000 location view pair
+    000024ad v000000000000000 v000000000000000 location view pair
+    000024af v000000000000000 v000000000000000 location view pair
+    000024b1 v000000000000000 v000000000000000 location view pair
+    000024b3 v000000000000000 v000000000000000 location view pair
 
-    0000227f v000000000000000 v000000000000000 views at 00002271 for:
+    000024b5 v000000000000000 v000000000000000 views at 000024a7 for:
              0000000000002ba0 0000000000002bad (DW_OP_reg5 (rdi))
-    00002292 v000000000000000 v000000000000000 views at 00002273 for:
+    000024c8 v000000000000000 v000000000000000 views at 000024a9 for:
              0000000000002bad 0000000000002bc6 (DW_OP_reg3 (rbx))
-    000022a5 v000000000000000 v000000000000000 views at 00002275 for:
+    000024db v000000000000000 v000000000000000 views at 000024ab for:
              0000000000002bc6 0000000000002beb (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
-    000022bb v000000000000000 v000000000000000 views at 00002277 for:
+    000024f1 v000000000000000 v000000000000000 views at 000024ad for:
              0000000000002beb 0000000000002c09 (DW_OP_reg3 (rbx))
-    000022ce v000000000000000 v000000000000000 views at 00002279 for:
+    00002504 v000000000000000 v000000000000000 views at 000024af for:
              0000000000002c09 0000000000002c0a (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
-    000022e4 v000000000000000 v000000000000000 views at 0000227b for:
+    0000251a v000000000000000 v000000000000000 views at 000024b1 for:
              0000000000002c0a 0000000000002c21 (DW_OP_reg5 (rdi))
-    000022f7 v000000000000000 v000000000000000 views at 0000227d for:
+    0000252d v000000000000000 v000000000000000 views at 000024b3 for:
              0000000000002c21 0000000000002c2a (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
-    0000230d <End of list>
+    00002543 <End of list>
 
-    0000231d v000000000000000 v000000000000000 location view pair
-    0000231f v000000000000000 v000000000000000 location view pair
-    00002321 v000000000000000 v000000000000000 location view pair
-    00002323 v000000000000000 v000000000000000 location view pair
-    00002325 v000000000000000 v000000000000000 location view pair
-    00002327 v000000000000000 v000000000000000 location view pair
+    00002553 v000000000000000 v000000000000000 location view pair
+    00002555 v000000000000000 v000000000000000 location view pair
+    00002557 v000000000000000 v000000000000000 location view pair
+    00002559 v000000000000000 v000000000000000 location view pair
+    0000255b v000000000000000 v000000000000000 location view pair
+    0000255d v000000000000000 v000000000000000 location view pair
 
-    00002329 v000000000000000 v000000000000000 views at 0000231d for:
+    0000255f v000000000000000 v000000000000000 views at 00002553 for:
              0000000000002ba0 0000000000002bb5 (DW_OP_reg4 (rsi))
-    0000233c v000000000000000 v000000000000000 views at 0000231f for:
+    00002572 v000000000000000 v000000000000000 views at 00002555 for:
              0000000000002bb5 0000000000002beb (DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)); DW_OP_stack_value)
-    00002352 v000000000000000 v000000000000000 views at 00002321 for:
+    00002588 v000000000000000 v000000000000000 views at 00002557 for:
              0000000000002beb 0000000000002bfe (DW_OP_reg4 (rsi))
-    00002365 v000000000000000 v000000000000000 views at 00002323 for:
+    0000259b v000000000000000 v000000000000000 views at 00002559 for:
              0000000000002bfe 0000000000002c0a (DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)); DW_OP_stack_value)
-    0000237b v000000000000000 v000000000000000 views at 00002325 for:
+    000025b1 v000000000000000 v000000000000000 views at 0000255b for:
              0000000000002c0a 0000000000002c1e (DW_OP_reg4 (rsi))
-    0000238e v000000000000000 v000000000000000 views at 00002327 for:
+    000025c4 v000000000000000 v000000000000000 views at 0000255d for:
              0000000000002c1e 0000000000002c2a (DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)); DW_OP_stack_value)
-    000023a4 <End of list>
+    000025da <End of list>
 
-    000023b4 v000000000000000 v000000000000000 location view pair
-    000023b6 v000000000000000 v000000000000000 location view pair
-    000023b8 v000000000000000 v000000000000000 location view pair
-    000023ba v000000000000000 v000000000000000 location view pair
-    000023bc v000000000000000 v000000000000000 location view pair
-    000023be v000000000000000 v000000000000000 location view pair
+    000025ea v000000000000000 v000000000000000 location view pair
+    000025ec v000000000000000 v000000000000000 location view pair
+    000025ee v000000000000000 v000000000000000 location view pair
+    000025f0 v000000000000000 v000000000000000 location view pair
+    000025f2 v000000000000000 v000000000000000 location view pair
+    000025f4 v000000000000000 v000000000000000 location view pair
 
-    000023c0 v000000000000000 v000000000000000 views at 000023b4 for:
+    000025f6 v000000000000000 v000000000000000 views at 000025ea for:
              0000000000002ba0 0000000000002bb5 (DW_OP_reg1 (rdx))
-    000023d3 v000000000000000 v000000000000000 views at 000023b6 for:
+    00002609 v000000000000000 v000000000000000 views at 000025ec for:
              0000000000002bb5 0000000000002beb (DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)); DW_OP_stack_value)
-    000023e9 v000000000000000 v000000000000000 views at 000023b8 for:
+    0000261f v000000000000000 v000000000000000 views at 000025ee for:
              0000000000002beb 0000000000002c05 (DW_OP_reg1 (rdx))
-    000023fc v000000000000000 v000000000000000 views at 000023ba for:
+    00002632 v000000000000000 v000000000000000 views at 000025f0 for:
              0000000000002c05 0000000000002c0a (DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)); DW_OP_stack_value)
-    00002412 v000000000000000 v000000000000000 views at 000023bc for:
+    00002648 v000000000000000 v000000000000000 views at 000025f2 for:
              0000000000002c0a 0000000000002c25 (DW_OP_reg1 (rdx))
-    00002425 v000000000000000 v000000000000000 views at 000023be for:
+    0000265b v000000000000000 v000000000000000 views at 000025f4 for:
              0000000000002c25 0000000000002c2a (DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)); DW_OP_stack_value)
-    0000243b <End of list>
+    00002671 <End of list>
 
-    0000244b v000000000000000 v000000000000000 location view pair
-    0000244d v000000000000000 v000000000000000 location view pair
-    0000244f v000000000000000 v000000000000000 location view pair
-    00002451 v000000000000000 v000000000000000 location view pair
-    00002453 v000000000000000 v000000000000000 location view pair
-    00002455 v000000000000000 v000000000000000 location view pair
+    00002681 v000000000000000 v000000000000000 location view pair
+    00002683 v000000000000000 v000000000000000 location view pair
+    00002685 v000000000000000 v000000000000000 location view pair
+    00002687 v000000000000000 v000000000000000 location view pair
+    00002689 v000000000000000 v000000000000000 location view pair
+    0000268b v000000000000000 v000000000000000 location view pair
 
-    00002457 v000000000000000 v000000000000000 views at 0000244b for:
+    0000268d v000000000000000 v000000000000000 views at 00002681 for:
              0000000000002ba0 0000000000002bb5 (DW_OP_reg2 (rcx))
-    0000246a v000000000000000 v000000000000000 views at 0000244d for:
+    000026a0 v000000000000000 v000000000000000 views at 00002683 for:
              0000000000002bb5 0000000000002beb (DW_OP_GNU_entry_value: (DW_OP_reg2 (rcx)); DW_OP_stack_value)
-    00002480 v000000000000000 v000000000000000 views at 0000244f for:
+    000026b6 v000000000000000 v000000000000000 views at 00002685 for:
              0000000000002beb 0000000000002c05 (DW_OP_reg2 (rcx))
-    00002493 v000000000000000 v000000000000000 views at 00002451 for:
+    000026c9 v000000000000000 v000000000000000 views at 00002687 for:
              0000000000002c05 0000000000002c0a (DW_OP_GNU_entry_value: (DW_OP_reg2 (rcx)); DW_OP_stack_value)
-    000024a9 v000000000000000 v000000000000000 views at 00002453 for:
+    000026df v000000000000000 v000000000000000 views at 00002689 for:
              0000000000002c0a 0000000000002c25 (DW_OP_reg2 (rcx))
-    000024bc v000000000000000 v000000000000000 views at 00002455 for:
+    000026f2 v000000000000000 v000000000000000 views at 0000268b for:
              0000000000002c25 0000000000002c2a (DW_OP_GNU_entry_value: (DW_OP_reg2 (rcx)); DW_OP_stack_value)
-    000024d2 <End of list>
+    00002708 <End of list>
 
-    000024e2 v000000000000000 v000000000000000 location view pair
-    000024e4 v000000000000000 v000000000000000 location view pair
-    000024e6 v000000000000000 v000000000000000 location view pair
-    000024e8 v000000000000000 v000000000000000 location view pair
-    000024ea v000000000000000 v000000000000000 location view pair
-    000024ec v000000000000000 v000000000000000 location view pair
+    00002718 v000000000000000 v000000000000000 location view pair
+    0000271a v000000000000000 v000000000000000 location view pair
+    0000271c v000000000000000 v000000000000000 location view pair
+    0000271e v000000000000000 v000000000000000 location view pair
+    00002720 v000000000000000 v000000000000000 location view pair
+    00002722 v000000000000000 v000000000000000 location view pair
 
-    000024ee v000000000000000 v000000000000000 views at 000024e2 for:
+    00002724 v000000000000000 v000000000000000 views at 00002718 for:
              0000000000002ba0 0000000000002bb5 (DW_OP_reg8 (r8))
-    00002501 v000000000000000 v000000000000000 views at 000024e4 for:
+    00002737 v000000000000000 v000000000000000 views at 0000271a for:
              0000000000002bb5 0000000000002beb (DW_OP_GNU_entry_value: (DW_OP_reg8 (r8)); DW_OP_stack_value)
-    00002517 v000000000000000 v000000000000000 views at 000024e6 for:
+    0000274d v000000000000000 v000000000000000 views at 0000271c for:
              0000000000002beb 0000000000002c05 (DW_OP_reg8 (r8))
-    0000252a v000000000000000 v000000000000000 views at 000024e8 for:
+    00002760 v000000000000000 v000000000000000 views at 0000271e for:
              0000000000002c05 0000000000002c0a (DW_OP_GNU_entry_value: (DW_OP_reg8 (r8)); DW_OP_stack_value)
-    00002540 v000000000000000 v000000000000000 views at 000024ea for:
+    00002776 v000000000000000 v000000000000000 views at 00002720 for:
              0000000000002c0a 0000000000002c25 (DW_OP_reg8 (r8))
-    00002553 v000000000000000 v000000000000000 views at 000024ec for:
+    00002789 v000000000000000 v000000000000000 views at 00002722 for:
              0000000000002c25 0000000000002c2a (DW_OP_GNU_entry_value: (DW_OP_reg8 (r8)); DW_OP_stack_value)
-    00002569 <End of list>
+    0000279f <End of list>
 
-    00002579 v000000000000000 v000000000000000 location view pair
+    000027af v000000000000000 v000000000000000 location view pair
 
-    0000257b v000000000000000 v000000000000000 views at 00002579 for:
+    000027b1 v000000000000000 v000000000000000 views at 000027af for:
              0000000000002bb6 0000000000002beb (DW_OP_reg0 (rax))
-    0000258e <End of list>
+    000027c4 <End of list>
 
-    0000259e v000000000000001 v000000000000002 location view pair
-    000025a0 v000000000000002 v000000000000000 location view pair
-    000025a2 v000000000000000 v000000000000000 location view pair
+    000027d4 v000000000000001 v000000000000002 location view pair
+    000027d6 v000000000000002 v000000000000000 location view pair
+    000027d8 v000000000000000 v000000000000000 location view pair
 
-    000025a4 v000000000000001 v000000000000002 views at 0000259e for:
+    000027da v000000000000001 v000000000000002 views at 000027d4 for:
              0000000000002bb6 0000000000002be0 (DW_OP_reg3 (rbx))
-    000025b7 v000000000000002 v000000000000000 views at 000025a0 for:
+    000027ed v000000000000002 v000000000000000 views at 000027d6 for:
              0000000000002be0 0000000000002be4 (DW_OP_breg3 (rbx): 24)
-    000025cb v000000000000000 v000000000000000 views at 000025a2 for:
+    00002801 v000000000000000 v000000000000000 views at 000027d8 for:
              0000000000002be4 0000000000002bea (DW_OP_reg3 (rbx))
-    000025de <End of list>
+    00002814 <End of list>
 
-    000025ee v000000000000001 v000000000000000 location view pair
-    000025f0 v000000000000000 v000000000000000 location view pair
+    00002824 v000000000000001 v000000000000000 location view pair
+    00002826 v000000000000000 v000000000000000 location view pair
 
-    000025f2 v000000000000001 v000000000000000 views at 000025ee for:
+    00002828 v000000000000001 v000000000000000 views at 00002824 for:
              0000000000002bb6 0000000000002bc6 (DW_OP_lit0; DW_OP_stack_value)
-    00002606 v000000000000000 v000000000000000 views at 000025f0 for:
+    0000283c v000000000000000 v000000000000000 views at 00002826 for:
              0000000000002bd4 0000000000002be9 (DW_OP_reg2 (rcx))
-    00002619 <End of list>
+    0000284f <End of list>
 
-    00002629 v000000000000003 v000000000000000 location view pair
+    0000285f v000000000000003 v000000000000000 location view pair
 
-    0000262b v000000000000003 v000000000000000 views at 00002629 for:
+    00002861 v000000000000003 v000000000000000 views at 0000285f for:
              0000000000002bb6 0000000000002bc6 (DW_OP_lit0; DW_OP_stack_value)
-    0000263f <End of list>
+    00002875 <End of list>
 
-    0000264f v000000000000002 v000000000000000 location view pair
+    00002885 v000000000000002 v000000000000000 location view pair
 
-    00002651 v000000000000002 v000000000000000 views at 0000264f for:
+    00002887 v000000000000002 v000000000000000 views at 00002885 for:
              0000000000002bd4 0000000000002be9 (DW_OP_reg2 (rcx))
-    00002664 <End of list>
+    0000289a <End of list>
 
-    00002674 v000000000000001 v000000000000000 location view pair
+    000028aa v000000000000001 v000000000000000 location view pair
 
-    00002676 v000000000000001 v000000000000000 views at 00002674 for:
+    000028ac v000000000000001 v000000000000000 views at 000028aa for:
              0000000000002bdc 0000000000002be0 (DW_OP_reg2 (rcx))
-    00002689 <End of list>
+    000028bf <End of list>
 
-    00002699 v000000000000001 v000000000000000 location view pair
+    000028cf v000000000000001 v000000000000000 location view pair
 
-    0000269b v000000000000001 v000000000000000 views at 00002699 for:
+    000028d1 v000000000000001 v000000000000000 views at 000028cf for:
              0000000000002bdc 0000000000002be0 (DW_OP_reg0 (rax))
-    000026ae <End of list>
+    000028e4 <End of list>
 
-    000026be v000000000000003 v000000000000000 location view pair
+    000028f4 v000000000000003 v000000000000000 location view pair
 
-    000026c0 v000000000000003 v000000000000000 views at 000026be for:
+    000028f6 v000000000000003 v000000000000000 views at 000028f4 for:
              0000000000002bdc 0000000000002be9 (DW_OP_reg0 (rax))
-    000026d3 <End of list>
+    00002909 <End of list>
 
-    000026e3 v000000000000001 v000000000000000 location view pair
-    000026e5 v000000000000000 v000000000000001 location view pair
+    00002919 v000000000000001 v000000000000000 location view pair
+    0000291b v000000000000000 v000000000000001 location view pair
 
-    000026e7 v000000000000001 v000000000000000 views at 000026e3 for:
+    0000291d v000000000000001 v000000000000000 views at 00002919 for:
              0000000000002c0a 0000000000002c21 (DW_OP_reg5 (rdi))
-    000026fa v000000000000000 v000000000000001 views at 000026e5 for:
+    00002930 v000000000000000 v000000000000001 views at 0000291b for:
              0000000000002c21 0000000000002c26 (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
-    00002710 <End of list>
+    00002946 <End of list>
 
-    00002720 v000000000000001 v000000000000000 location view pair
-    00002722 v000000000000000 v000000000000001 location view pair
+    00002956 v000000000000001 v000000000000000 location view pair
+    00002958 v000000000000000 v000000000000001 location view pair
 
-    00002724 v000000000000001 v000000000000000 views at 00002720 for:
+    0000295a v000000000000001 v000000000000000 views at 00002956 for:
              0000000000002c0a 0000000000002c1e (DW_OP_reg4 (rsi))
-    00002737 v000000000000000 v000000000000001 views at 00002722 for:
+    0000296d v000000000000000 v000000000000001 views at 00002958 for:
              0000000000002c1e 0000000000002c26 (DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)); DW_OP_stack_value)
-    0000274d <End of list>
+    00002983 <End of list>
 
-    0000275d v000000000000001 v000000000000000 location view pair
-    0000275f v000000000000000 v000000000000001 location view pair
+    00002993 v000000000000001 v000000000000000 location view pair
+    00002995 v000000000000000 v000000000000001 location view pair
 
-    00002761 v000000000000001 v000000000000000 views at 0000275d for:
+    00002997 v000000000000001 v000000000000000 views at 00002993 for:
              0000000000002c0a 0000000000002c25 (DW_OP_reg1 (rdx))
-    00002774 v000000000000000 v000000000000001 views at 0000275f for:
+    000029aa v000000000000000 v000000000000001 views at 00002995 for:
              0000000000002c25 0000000000002c26 (DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)); DW_OP_stack_value)
-    0000278a <End of list>
+    000029c0 <End of list>
 
-    0000279a v000000000000001 v000000000000000 location view pair
-    0000279c v000000000000000 v000000000000001 location view pair
+    000029d0 v000000000000001 v000000000000000 location view pair
+    000029d2 v000000000000000 v000000000000001 location view pair
 
-    0000279e v000000000000001 v000000000000000 views at 0000279a for:
+    000029d4 v000000000000001 v000000000000000 views at 000029d0 for:
              0000000000002c0a 0000000000002c25 (DW_OP_reg2 (rcx))
-    000027b1 v000000000000000 v000000000000001 views at 0000279c for:
+    000029e7 v000000000000000 v000000000000001 views at 000029d2 for:
              0000000000002c25 0000000000002c26 (DW_OP_GNU_entry_value: (DW_OP_reg2 (rcx)); DW_OP_stack_value)
-    000027c7 <End of list>
+    000029fd <End of list>
 
-    000027d7 v000000000000001 v000000000000000 location view pair
-    000027d9 v000000000000000 v000000000000001 location view pair
+    00002a0d v000000000000001 v000000000000000 location view pair
+    00002a0f v000000000000000 v000000000000001 location view pair
 
-    000027db v000000000000001 v000000000000000 views at 000027d7 for:
+    00002a11 v000000000000001 v000000000000000 views at 00002a0d for:
              0000000000002c0a 0000000000002c25 (DW_OP_reg8 (r8))
-    000027ee v000000000000000 v000000000000001 views at 000027d9 for:
+    00002a24 v000000000000000 v000000000000001 views at 00002a0f for:
              0000000000002c25 0000000000002c26 (DW_OP_GNU_entry_value: (DW_OP_reg8 (r8)); DW_OP_stack_value)
-    00002804 <End of list>
+    00002a3a <End of list>
 
-    00002814 v000000000000000 v000000000000000 location view pair
-    00002816 v000000000000000 v000000000000000 location view pair
-    00002818 v000000000000000 v000000000000000 location view pair
-    0000281a v000000000000000 v000000000000000 location view pair
-    0000281c v000000000000000 v000000000000000 location view pair
+    00002a4a v000000000000000 v000000000000000 location view pair
+    00002a4c v000000000000000 v000000000000000 location view pair
+    00002a4e v000000000000000 v000000000000000 location view pair
+    00002a50 v000000000000000 v000000000000000 location view pair
+    00002a52 v000000000000000 v000000000000000 location view pair
 
-    0000281e v000000000000000 v000000000000000 views at 00002814 for:
+    00002a54 v000000000000000 v000000000000000 views at 00002a4a for:
              0000000000002c30 0000000000002c38 (DW_OP_reg5 (rdi))
-    00002831 v000000000000000 v000000000000000 views at 00002816 for:
+    00002a67 v000000000000000 v000000000000000 views at 00002a4c for:
              0000000000002c38 0000000000002c78 (DW_OP_reg12 (r12))
-    00002844 v000000000000000 v000000000000000 views at 00002818 for:
+    00002a7a v000000000000000 v000000000000000 views at 00002a4e for:
              0000000000002c78 0000000000002c79 (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
-    0000285a v000000000000000 v000000000000000 views at 0000281a for:
+    00002a90 v000000000000000 v000000000000000 views at 00002a50 for:
              0000000000002c79 0000000000002c9f (DW_OP_reg12 (r12))
-    0000286d v000000000000000 v000000000000000 views at 0000281c for:
+    00002aa3 v000000000000000 v000000000000000 views at 00002a52 for:
              0000000000002c9f 0000000000002ca0 (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
-    00002883 <End of list>
+    00002ab9 <End of list>
 
-    00002893 v000000000000000 v000000000000000 location view pair
-    00002895 v000000000000000 v000000000000000 location view pair
+    00002ac9 v000000000000000 v000000000000000 location view pair
+    00002acb v000000000000000 v000000000000000 location view pair
 
-    00002897 v000000000000000 v000000000000000 views at 00002893 for:
+    00002acd v000000000000000 v000000000000000 views at 00002ac9 for:
              0000000000002c30 0000000000002c44 (DW_OP_reg4 (rsi))
-    000028aa v000000000000000 v000000000000000 views at 00002895 for:
+    00002ae0 v000000000000000 v000000000000000 views at 00002acb for:
              0000000000002c44 0000000000002ca0 (DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)); DW_OP_stack_value)
-    000028c0 <End of list>
+    00002af6 <End of list>
 
-    000028d0 v000000000000000 v000000000000000 location view pair
-    000028d2 v000000000000000 v000000000000000 location view pair
-    000028d4 v000000000000000 v000000000000000 location view pair
-    000028d6 v000000000000000 v000000000000000 location view pair
-    000028d8 v000000000000000 v000000000000000 location view pair
+    00002b06 v000000000000000 v000000000000000 location view pair
+    00002b08 v000000000000000 v000000000000000 location view pair
+    00002b0a v000000000000000 v000000000000000 location view pair
+    00002b0c v000000000000000 v000000000000000 location view pair
+    00002b0e v000000000000000 v000000000000000 location view pair
 
-    000028da v000000000000000 v000000000000000 views at 000028d0 for:
+    00002b10 v000000000000000 v000000000000000 views at 00002b06 for:
              0000000000002c30 0000000000002c44 (DW_OP_reg1 (rdx))
-    000028ed v000000000000000 v000000000000000 views at 000028d2 for:
+    00002b23 v000000000000000 v000000000000000 views at 00002b08 for:
              0000000000002c44 0000000000002c76 (DW_OP_reg6 (rbp))
-    00002900 v000000000000000 v000000000000000 views at 000028d4 for:
+    00002b36 v000000000000000 v000000000000000 views at 00002b0a for:
              0000000000002c76 0000000000002c79 (DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)); DW_OP_stack_value)
-    00002916 v000000000000000 v000000000000000 views at 000028d6 for:
+    00002b4c v000000000000000 v000000000000000 views at 00002b0c for:
              0000000000002c79 0000000000002c9d (DW_OP_reg6 (rbp))
-    00002929 v000000000000000 v000000000000000 views at 000028d8 for:
+    00002b5f v000000000000000 v000000000000000 views at 00002b0e for:
              0000000000002c9d 0000000000002ca0 (DW_OP_GNU_entry_value: (DW_OP_reg1 (rdx)); DW_OP_stack_value)
-    0000293f <End of list>
+    00002b75 <End of list>
 
-    0000294f v000000000000000 v000000000000000 location view pair
+    00002b85 v000000000000000 v000000000000000 location view pair
 
-    00002951 v000000000000000 v000000000000000 views at 0000294f for:
+    00002b87 v000000000000000 v000000000000000 views at 00002b85 for:
              0000000000002c64 0000000000002c6d (DW_OP_reg0 (rax))
-    00002964 <End of list>
+    00002b9a <End of list>
 
-    00002974 v000000000000000 v000000000000001 location view pair
+    00002baa v000000000000000 v000000000000001 location view pair
 
-    00002976 v000000000000000 v000000000000001 views at 00002974 for:
+    00002bac v000000000000000 v000000000000001 views at 00002baa for:
              0000000000002c6d 0000000000002c71 (DW_OP_reg0 (rax))
-    00002989 <End of list>
+    00002bbf <End of list>
 
-    00002999 v000000000000002 v000000000000001 location view pair
+    00002bcf v000000000000002 v000000000000001 location view pair
 
-    0000299b v000000000000002 v000000000000001 views at 00002999 for:
+    00002bd1 v000000000000002 v000000000000001 views at 00002bcf for:
              0000000000002c6d 0000000000002c71 (DW_OP_reg0 (rax))
-    000029ae <End of list>
+    00002be4 <End of list>
 
-    000029be v000000000000001 v000000000000001 location view pair
+    00002bf4 v000000000000001 v000000000000001 location view pair
 
-    000029c0 v000000000000001 v000000000000001 views at 000029be for:
+    00002bf6 v000000000000001 v000000000000001 views at 00002bf4 for:
              0000000000002c79 0000000000002c96 (DW_OP_reg12 (r12))
-    000029d3 <End of list>
+    00002c09 <End of list>
 
-    000029e3 v000000000000001 v000000000000001 location view pair
+    00002c19 v000000000000001 v000000000000001 location view pair
 
-    000029e5 v000000000000001 v000000000000001 views at 000029e3 for:
+    00002c1b v000000000000001 v000000000000001 views at 00002c19 for:
              0000000000002c79 0000000000002c96 (DW_OP_GNU_entry_value: (DW_OP_reg4 (rsi)); DW_OP_stack_value)
-    000029fb <End of list>
+    00002c31 <End of list>
 
-    00002a0b v000000000000001 v000000000000001 location view pair
+    00002c41 v000000000000001 v000000000000001 location view pair
 
-    00002a0d v000000000000001 v000000000000001 views at 00002a0b for:
+    00002c43 v000000000000001 v000000000000001 views at 00002c41 for:
              0000000000002c79 0000000000002c96 (DW_OP_reg6 (rbp))
-    00002a20 <End of list>
+    00002c56 <End of list>
```

### readelf --wide --debug-dump=ranges {}

```diff
@@ -4,29 +4,29 @@
   Version:                  2
   Offset into .debug_info:  0
   Pointer Size:             8
   Segment Size:             0
 
     Address            Length
     0000000000002000 0000000000000001
-    0000000000002eae 0000000000000001
+    0000000000002ebe 0000000000000001
     0000000000000000 0000000000000000
   Length:                   44
   Version:                  2
   Offset into .debug_info:  0x22
   Pointer Size:             8
   Segment Size:             0
 
     Address            Length
-    00000000000023c0 0000000000000acc
+    00000000000023c0 0000000000000adc
     0000000000000000 0000000000000000
   Length:                   60
   Version:                  2
-  Offset into .debug_info:  0x44fa
+  Offset into .debug_info:  0x45d7
   Pointer Size:             8
   Segment Size:             0
 
     Address            Length
     000000000000200b 0000000000000002
-    0000000000002eb4 0000000000000002
+    0000000000002ec4 0000000000000002
     0000000000000000 0000000000000000
```

### strings --all --bytes=8 {}

```diff
@@ -57,15 +57,15 @@
 PyInit_fastcons
 PyModuleDef_Init
 libc.musl-x86_64.so.1
 H[]A\A]A^A_
 []A\A]A^
 []A\A]A^
 []A\A]A^
-AVAUATUSH
+AVAUATUSL
 __match_args__
 expected zero arguments
 expected proper cons list
 nil() takes no arguments
 fastcons.cons
 cons head
 cons tail
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.init {}

```diff
@@ -4,12 +4,12 @@
 Disassembly of section .init:
 
 0000000000002000 <_init>:
 _init():
 /home/buildozer/aports/main/musl/src/musl-1.1.24/crt/x86_64/crti.s:4
 	push   %rax
 	call   2390 <frame_dummy>
-	call   2e8c <__do_global_ctors_aux>
+	call   2e9c <__do_global_ctors_aux>
 /home/buildozer/aports/main/musl/src/musl-1.1.24/crt/x86_64/crtn.s:2
 	pop    %rax
 /home/buildozer/aports/main/musl/src/musl-1.1.24/crt/x86_64/crtn.s:3
 	ret
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -337,63 +337,63 @@
 	pop    %rbp
 	pop    %r12
 	ret
 	nopl   0x0(%rax,%rax,1)
 
 0000000000002630 <consmodule_clear>:
 consmodule_clear():
-/project/consmodule.c:442
+/project/consmodule.c:455
 	push   %rbx
-/project/consmodule.c:443
+/project/consmodule.c:456
 	call   2130 <PyModule_GetState@plt>
-/project/consmodule.c:444
+/project/consmodule.c:457
 	mov    0x10(%rax),%rdi
-/project/consmodule.c:443
+/project/consmodule.c:456
 	mov    %rax,%rbx
-/project/consmodule.c:444
+/project/consmodule.c:457
 	test   %rdi,%rdi
 	je     2650 <consmodule_clear+0x20>
-/project/consmodule.c:444 (discriminator 1)
+/project/consmodule.c:457 (discriminator 1)
 	movq   $0x0,0x10(%rax)
 Py_DECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:537 (discriminator 1)
 	subq   $0x1,(%rdi)
 	je     26a0 <consmodule_clear+0x70>
 consmodule_clear():
-/project/consmodule.c:445 (discriminator 3)
+/project/consmodule.c:458 (discriminator 3)
 	mov    (%rbx),%rdi
 	test   %rdi,%rdi
 	je     2665 <consmodule_clear+0x35>
-/project/consmodule.c:445 (discriminator 1)
+/project/consmodule.c:458 (discriminator 1)
 	movq   $0x0,(%rbx)
 Py_DECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:537 (discriminator 1)
 	subq   $0x1,(%rdi)
 	je     2690 <consmodule_clear+0x60>
 consmodule_clear():
-/project/consmodule.c:446 (discriminator 3)
+/project/consmodule.c:459 (discriminator 3)
 	mov    0x8(%rbx),%rdi
 	test   %rdi,%rdi
 	je     267c <consmodule_clear+0x4c>
-/project/consmodule.c:446 (discriminator 1)
+/project/consmodule.c:459 (discriminator 1)
 	movq   $0x0,0x8(%rbx)
 Py_DECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:537 (discriminator 1)
 	subq   $0x1,(%rdi)
 	je     2680 <consmodule_clear+0x50>
 consmodule_clear():
-/project/consmodule.c:448 (discriminator 3)
+/project/consmodule.c:461 (discriminator 3)
 	xor    %eax,%eax
 	pop    %rbx
 	ret
 Py_DECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:538
 	call   21b0 <_Py_Dealloc@plt>
 consmodule_clear():
-/project/consmodule.c:448
+/project/consmodule.c:461
 	xor    %eax,%eax
 	pop    %rbx
 	ret
 	nopl   0x0(%rax)
 Py_DECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:538
 	call   21b0 <_Py_Dealloc@plt>
@@ -403,179 +403,179 @@
 	jmp    2650 <consmodule_clear+0x20>
 consmodule_clear():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:538
 	nopw   0x0(%rax,%rax,1)
 
 00000000000026b0 <consmodule_traverse>:
 consmodule_traverse():
-/project/consmodule.c:432
+/project/consmodule.c:445
 	push   %r12
 	mov    %rdx,%r12
 	push   %rbp
 	mov    %rsi,%rbp
 	push   %rbx
-/project/consmodule.c:433
+/project/consmodule.c:446
 	call   2130 <PyModule_GetState@plt>
-/project/consmodule.c:434
+/project/consmodule.c:447
 	mov    0x10(%rax),%rdi
-/project/consmodule.c:433
+/project/consmodule.c:446
 	mov    %rax,%rbx
-/project/consmodule.c:434
+/project/consmodule.c:447
 	test   %rdi,%rdi
 	je     26d4 <consmodule_traverse+0x24>
-/project/consmodule.c:434 (discriminator 1)
+/project/consmodule.c:447 (discriminator 1)
 	mov    %r12,%rsi
 	call   *%rbp
 	test   %eax,%eax
 	jne    2700 <consmodule_traverse+0x50>
-/project/consmodule.c:435
+/project/consmodule.c:448
 	mov    (%rbx),%rdi
 	test   %rdi,%rdi
 	je     26e5 <consmodule_traverse+0x35>
-/project/consmodule.c:435 (discriminator 1)
+/project/consmodule.c:448 (discriminator 1)
 	mov    %r12,%rsi
 	call   *%rbp
 	test   %eax,%eax
 	jne    2700 <consmodule_traverse+0x50>
-/project/consmodule.c:436
+/project/consmodule.c:449
 	mov    0x8(%rbx),%rdi
-/project/consmodule.c:437
+/project/consmodule.c:450
 	xor    %eax,%eax
-/project/consmodule.c:436
+/project/consmodule.c:449
 	test   %rdi,%rdi
 	je     2700 <consmodule_traverse+0x50>
-/project/consmodule.c:438 (discriminator 1)
+/project/consmodule.c:451 (discriminator 1)
 	pop    %rbx
-/project/consmodule.c:436 (discriminator 1)
+/project/consmodule.c:449 (discriminator 1)
 	mov    %r12,%rsi
 	mov    %rbp,%rax
-/project/consmodule.c:438 (discriminator 1)
+/project/consmodule.c:451 (discriminator 1)
 	pop    %rbp
 	pop    %r12
-/project/consmodule.c:436 (discriminator 1)
+/project/consmodule.c:449 (discriminator 1)
 	jmp    *%rax
 	nopl   0x0(%rax)
-/project/consmodule.c:438
+/project/consmodule.c:451
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 
 0000000000002710 <Cons_repr>:
 Cons_repr():
-/project/consmodule.c:243
+/project/consmodule.c:256
 	push   %r15
-/project/consmodule.c:247
+/project/consmodule.c:260
 	lea    0x2a07(%rip),%rsi        
-/project/consmodule.c:243
+/project/consmodule.c:256
 	push   %r14
 	mov    %rdi,%r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
 	sub    $0x48,%rsp
-/project/consmodule.c:247
+/project/consmodule.c:260
 	mov    0x8(%rdi),%rdi
-/project/consmodule.c:243
+/project/consmodule.c:256
 	mov    %fs:0x28,%rax
 	mov    %rax,0x38(%rsp)
 	xor    %eax,%eax
-/project/consmodule.c:247
+/project/consmodule.c:260
 	call   2020 <PyType_GetModuleByDef@plt>
-/project/consmodule.c:248
+/project/consmodule.c:261
 	test   %rax,%rax
 	je     276f <Cons_repr+0x5f>
 	mov    %rax,%rdi
-/project/consmodule.c:251
+/project/consmodule.c:264
 	call   2130 <PyModule_GetState@plt>
 	mov    %rax,%rbx
-/project/consmodule.c:252
+/project/consmodule.c:265
 	test   %rax,%rax
 	je     276f <Cons_repr+0x5f>
-/project/consmodule.c:257
+/project/consmodule.c:270
 	mov    %r14,%rdi
-/project/consmodule.c:255
+/project/consmodule.c:268
 	mov    0x10(%rax),%r13
-/project/consmodule.c:257
+/project/consmodule.c:270
 	call   2170 <Py_ReprEnter@plt>
 	cltq
-/project/consmodule.c:258
+/project/consmodule.c:271
 	test   %rax,%rax
 	je     2798 <Cons_repr+0x88>
-/project/consmodule.c:259
+/project/consmodule.c:272
 	jg     2870 <Cons_repr+0x160>
-/project/consmodule.c:309
+/project/consmodule.c:322
 	xor    %eax,%eax
-/project/consmodule.c:310
+/project/consmodule.c:323
 	mov    0x38(%rsp),%rcx
 	xor    %fs:0x28,%rcx
 	jne    290f <Cons_repr+0x1ff>
 	add    $0x48,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nopl   0x0(%rax)
-/project/consmodule.c:261
+/project/consmodule.c:274
 	mov    %rsp,%r12
 	mov    %r12,%rdi
 	call   2210 <_PyUnicodeWriter_Init@plt>
-/project/consmodule.c:264
+/project/consmodule.c:277
 	mov    $0x28,%esi
 	mov    %r12,%rdi
-/project/consmodule.c:262
+/project/consmodule.c:275
 	movb   $0x1,0x34(%rsp)
-/project/consmodule.c:263
+/project/consmodule.c:276
 	movq   $0x3,0x28(%rsp)
-/project/consmodule.c:264
+/project/consmodule.c:277
 	call   2070 <_PyUnicodeWriter_WriteChar@plt>
 	test   %eax,%eax
 	js     2858 <Cons_repr+0x148>
 	mov    %r14,%r15
 	jmp    27f9 <Cons_repr+0xe9>
 	nopl   0x0(%rax,%rax,1)
-/project/consmodule.c:279
+/project/consmodule.c:292
 	mov    0x18(%r15),%r15
-/project/consmodule.c:280
+/project/consmodule.c:293
 	cmp    %r15,0x8(%rbx)
 	je     28e0 <Cons_repr+0x1d0>
-/project/consmodule.c:282
+/project/consmodule.c:295
 	cmp    0x8(%r15),%r13
 	jne    2888 <Cons_repr+0x178>
-/project/consmodule.c:295
+/project/consmodule.c:308
 	mov    $0x20,%esi
 	mov    %r12,%rdi
 	call   2070 <_PyUnicodeWriter_WriteChar@plt>
 	test   %eax,%eax
 	js     2858 <Cons_repr+0x148>
-/project/consmodule.c:268
+/project/consmodule.c:281
 	cmp    0x8(%r15),%r13
 	jne    28e0 <Cons_repr+0x1d0>
-/project/consmodule.c:270
+/project/consmodule.c:283
 	mov    0x10(%r15),%rdi
 	call   21a0 <PyObject_Repr@plt>
 	mov    %rax,%rbp
-/project/consmodule.c:271
+/project/consmodule.c:284
 	test   %rax,%rax
 	je     2858 <Cons_repr+0x148>
-/project/consmodule.c:273
+/project/consmodule.c:286
 	mov    %rax,%rsi
 	mov    %r12,%rdi
 	call   21e0 <_PyUnicodeWriter_WriteStr@plt>
 	test   %eax,%eax
 Py_DECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:537
 	mov    0x0(%rbp),%rax
 Cons_repr():
-/project/consmodule.c:273
+/project/consmodule.c:286
 	js     2840 <Cons_repr+0x130>
 Py_DECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:537
 	sub    $0x1,%rax
 	mov    %rax,0x0(%rbp)
 	jne    27d0 <Cons_repr+0xc0>
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:538
@@ -588,179 +588,179 @@
 	mov    %rax,0x0(%rbp)
 	jne    2858 <Cons_repr+0x148>
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:538
 	mov    %rbp,%rdi
 	call   21b0 <_Py_Dealloc@plt>
 	nopw   0x0(%rax,%rax,1)
 Cons_repr():
-/project/consmodule.c:307
+/project/consmodule.c:320
 	mov    %r12,%rdi
 	call   2030 <_PyUnicodeWriter_Dealloc@plt>
-/project/consmodule.c:308
+/project/consmodule.c:321
 	mov    %r14,%rdi
 	call   20d0 <Py_ReprLeave@plt>
 	jmp    276f <Cons_repr+0x5f>
 	nopl   (%rax)
-/project/consmodule.c:259 (discriminator 1)
+/project/consmodule.c:272 (discriminator 1)
 	lea    0x792(%rip),%rdi        
 	xor    %eax,%eax
 	call   2040 <PyUnicode_FromFormat@plt>
 	jmp    2771 <Cons_repr+0x61>
 	nopl   0x0(%rax,%rax,1)
-/project/consmodule.c:283
+/project/consmodule.c:296
 	mov    $0x3,%edx
 	lea    0x779(%rip),%rsi        
 	mov    %r12,%rdi
 	call   2240 <_PyUnicodeWriter_WriteASCIIString@plt>
 	test   %eax,%eax
 	js     2858 <Cons_repr+0x148>
-/project/consmodule.c:285
+/project/consmodule.c:298
 	mov    %r15,%rdi
 	call   21a0 <PyObject_Repr@plt>
 	mov    %rax,%rbp
-/project/consmodule.c:286
+/project/consmodule.c:299
 	test   %rax,%rax
 	je     2858 <Cons_repr+0x148>
-/project/consmodule.c:288
+/project/consmodule.c:301
 	mov    %rax,%rsi
 	mov    %r12,%rdi
 	call   21e0 <_PyUnicodeWriter_WriteStr@plt>
 	test   %eax,%eax
 Py_DECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:537
 	mov    0x0(%rbp),%rax
 Cons_repr():
-/project/consmodule.c:288
+/project/consmodule.c:301
 	js     2840 <Cons_repr+0x130>
 Py_DECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:537
 	sub    $0x1,%rax
 	mov    %rax,0x0(%rbp)
 	jne    28e0 <Cons_repr+0x1d0>
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:538
 	mov    %rbp,%rdi
 	call   21b0 <_Py_Dealloc@plt>
 	nopl   0x0(%rax)
 Cons_repr():
-/project/consmodule.c:301
+/project/consmodule.c:314
 	mov    $0x29,%esi
 	mov    %r12,%rdi
-/project/consmodule.c:300
+/project/consmodule.c:313
 	movb   $0x0,0x34(%rsp)
-/project/consmodule.c:301
+/project/consmodule.c:314
 	call   2070 <_PyUnicodeWriter_WriteChar@plt>
 	test   %eax,%eax
 	js     2858 <Cons_repr+0x148>
-/project/consmodule.c:303
+/project/consmodule.c:316
 	mov    %r14,%rdi
 	call   20d0 <Py_ReprLeave@plt>
-/project/consmodule.c:304
+/project/consmodule.c:317
 	mov    %r12,%rdi
 	call   2260 <_PyUnicodeWriter_Finish@plt>
 	jmp    2771 <Cons_repr+0x61>
-/project/consmodule.c:310
+/project/consmodule.c:323
 	call   20e0 <__stack_chk_fail@plt>
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nop
 
 0000000000002920 <consmodule_exec>:
 consmodule_exec():
-/project/consmodule.c:391
+/project/consmodule.c:404
 	push   %r12
 	mov    %rdi,%r12
 	push   %rbp
 	push   %rbx
-/project/consmodule.c:392
+/project/consmodule.c:405
 	call   2130 <PyModule_GetState@plt>
-/project/consmodule.c:393
+/project/consmodule.c:406
 	test   %rax,%rax
 	je     2a30 <consmodule_exec+0x110>
-/project/consmodule.c:396
+/project/consmodule.c:409
 	lea    0x2724(%rip),%rsi        
 	xor    %edx,%edx
 	mov    %r12,%rdi
 	mov    %rax,%rbx
 	call   2280 <PyType_FromModuleAndSpec@plt>
 	mov    %rax,0x10(%rbx)
 	mov    %rax,%rsi
-/project/consmodule.c:397
+/project/consmodule.c:410
 	test   %rax,%rax
 	je     2a30 <consmodule_exec+0x110>
-/project/consmodule.c:399
+/project/consmodule.c:412
 	mov    %r12,%rdi
 	call   2110 <PyModule_AddType@plt>
 	test   %eax,%eax
 	js     2a30 <consmodule_exec+0x110>
-/project/consmodule.c:401
+/project/consmodule.c:414
 	mov    $0x2,%edi
 	call   2250 <PyTuple_New@plt>
 	mov    %rax,%rbp
-/project/consmodule.c:402
+/project/consmodule.c:415
 	test   %rax,%rax
 	je     2a30 <consmodule_exec+0x110>
-/project/consmodule.c:404
+/project/consmodule.c:417
 	lea    0x708(%rip),%rdi        
 	call   2090 <PyUnicode_FromString@plt>
-/project/consmodule.c:405
+/project/consmodule.c:418
 	lea    0x706(%rip),%rdi        
 PyTuple_SET_ITEM():
 /opt/_internal/cpython-3.11.2/include/python3.11/cpython/tupleobject.h:36
 	mov    %rax,0x18(%rbp)
 consmodule_exec():
-/project/consmodule.c:405
+/project/consmodule.c:418
 	call   2090 <PyUnicode_FromString@plt>
-/project/consmodule.c:406
+/project/consmodule.c:419
 	mov    %rbp,%rdx
 	lea    0x66c(%rip),%rsi        
 PyTuple_SET_ITEM():
 /opt/_internal/cpython-3.11.2/include/python3.11/cpython/tupleobject.h:36
 	mov    %rax,0x20(%rbp)
 consmodule_exec():
-/project/consmodule.c:406
+/project/consmodule.c:419
 	mov    0x10(%rbx),%rax
 	mov    0x108(%rax),%rdi
 	call   2060 <PyDict_SetItemString@plt>
 	test   %eax,%eax
 Py_DECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:537
 	mov    0x0(%rbp),%rax
 consmodule_exec():
-/project/consmodule.c:406
+/project/consmodule.c:419
 	js     2a1a <consmodule_exec+0xfa>
 Py_DECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:537
 	sub    $0x1,%rax
 	mov    %rax,0x0(%rbp)
 	je     2a10 <consmodule_exec+0xf0>
 consmodule_exec():
-/project/consmodule.c:413
+/project/consmodule.c:426
 	lea    0x272e(%rip),%rsi        
 	xor    %edx,%edx
 	mov    %r12,%rdi
 	call   2280 <PyType_FromModuleAndSpec@plt>
 	mov    %rax,(%rbx)
 	mov    %rax,%rsi
-/project/consmodule.c:414
+/project/consmodule.c:427
 	test   %rax,%rax
 	je     2a30 <consmodule_exec+0x110>
-/project/consmodule.c:416
+/project/consmodule.c:429
 	mov    %r12,%rdi
 	call   2110 <PyModule_AddType@plt>
 	test   %eax,%eax
 	js     2a30 <consmodule_exec+0x110>
-/project/consmodule.c:420
+/project/consmodule.c:433
 	mov    (%rbx),%rax
 	xor    %esi,%esi
 	mov    %rax,%rdi
 	call   *0x130(%rax)
-/project/consmodule.c:421
+/project/consmodule.c:434
 	mov    %rax,0x8(%rbx)
-/project/consmodule.c:422
+/project/consmodule.c:435
 	xor    %eax,%eax
-/project/consmodule.c:423
+/project/consmodule.c:436
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	ret
 	nopl   0x0(%rax)
 Py_DECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:538
@@ -772,141 +772,141 @@
 	mov    %rax,0x0(%rbp)
 	jne    2a30 <consmodule_exec+0x110>
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:538
 	mov    %rbp,%rdi
 	call   21b0 <_Py_Dealloc@plt>
 	nopl   0x0(%rax)
 consmodule_exec():
-/project/consmodule.c:409
+/project/consmodule.c:422
 	mov    $0xffffffff,%eax
 	jmp    2a07 <consmodule_exec+0xe7>
 	nopw   0x0(%rax,%rax,1)
 
 0000000000002a40 <Cons_richcompare>:
 Cons_richcompare():
-/project/consmodule.c:314
+/project/consmodule.c:327
 	push   %r14
 	push   %r13
 	mov    %edx,%r13d
 	push   %r12
 	mov    %rsi,%r12
 	push   %rbp
 	mov    %rdi,%rbp
 	push   %rbx
-/project/consmodule.c:315
+/project/consmodule.c:328
 	mov    0x8(%rdi),%rdi
 	call   2270 <PyType_GetModuleState@plt>
-/project/consmodule.c:316
+/project/consmodule.c:329
 	test   %rax,%rax
 	je     2b00 <Cons_richcompare+0xc0>
-/project/consmodule.c:320
+/project/consmodule.c:333
 	mov    0x10(%rax),%r14
-/project/consmodule.c:321
+/project/consmodule.c:334
 	cmp    0x8(%r12),%r14
 	je     2a88 <Cons_richcompare+0x48>
 Py_INCREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:502
 	mov    0x2543(%rip),%rax        
 	addq   $0x1,(%rax)
 Cons_richcompare():
-/project/consmodule.c:348
+/project/consmodule.c:361
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 	nopw   0x0(%rax,%rax,1)
-/project/consmodule.c:319
+/project/consmodule.c:332
 	mov    0x8(%rax),%rbx
-/project/consmodule.c:326
+/project/consmodule.c:339
 	cmp    0x8(%rbp),%r14
 	jne    2ad5 <Cons_richcompare+0x95>
 	nopw   0x0(%rax,%rax,1)
-/project/consmodule.c:327
+/project/consmodule.c:340
 	mov    0x10(%r12),%rsi
 	mov    0x10(%rbp),%rdi
 	mov    %r13d,%edx
 	call   2230 <PyObject_RichCompareBool@plt>
-/project/consmodule.c:328
+/project/consmodule.c:341
 	test   %eax,%eax
 	js     2b00 <Cons_richcompare+0xc0>
-/project/consmodule.c:330
+/project/consmodule.c:343
 	je     2ab5 <Cons_richcompare+0x75>
 	cmp    $0x3,%r13d
 	je     2ae5 <Cons_richcompare+0xa5>
-/project/consmodule.c:332
+/project/consmodule.c:345
 	test   %eax,%eax
 	jne    2abf <Cons_richcompare+0x7f>
 	cmp    $0x3,%r13d
 	jne    2b10 <Cons_richcompare+0xd0>
-/project/consmodule.c:335
+/project/consmodule.c:348
 	mov    0x18(%rbp),%rbp
-/project/consmodule.c:336
+/project/consmodule.c:349
 	mov    0x18(%r12),%r12
-/project/consmodule.c:326
+/project/consmodule.c:339
 	cmp    0x8(%rbp),%r14
 	jne    2ad5 <Cons_richcompare+0x95>
 	cmp    0x8(%r12),%r14
 	je     2a98 <Cons_richcompare+0x58>
-/project/consmodule.c:340
+/project/consmodule.c:353
 	cmp    %rbp,%rbx
 	jne    2b28 <Cons_richcompare+0xe8>
 	cmp    %r12,%rbx
 	jne    2b28 <Cons_richcompare+0xe8>
-/project/consmodule.c:342
+/project/consmodule.c:355
 	cmp    $0x3,%r13d
 	je     2b10 <Cons_richcompare+0xd0>
 Py_INCREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:502
 	mov    0x24b4(%rip),%rax        
 	addq   $0x1,(%rax)
 Cons_richcompare():
-/project/consmodule.c:348
+/project/consmodule.c:361
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 	nopl   0x0(%rax)
 	pop    %rbx
-/project/consmodule.c:317
+/project/consmodule.c:330
 	xor    %eax,%eax
-/project/consmodule.c:348
+/project/consmodule.c:361
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 	nopl   0x0(%rax,%rax,1)
 Py_INCREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:502
 	mov    0x24c9(%rip),%rax        
 	addq   $0x1,(%rax)
 Cons_richcompare():
-/project/consmodule.c:348
+/project/consmodule.c:361
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 	nopl   0x0(%rax)
 	pop    %rbx
-/project/consmodule.c:347
+/project/consmodule.c:360
 	mov    %r13d,%edx
 	mov    %r12,%rsi
 	mov    %rbp,%rdi
-/project/consmodule.c:348
+/project/consmodule.c:361
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
-/project/consmodule.c:347
+/project/consmodule.c:360
 	jmp    21c0 <PyObject_RichCompare@plt>
 	xchg   %ax,%ax
 
 0000000000002b40 <Cons_traverse>:
 Cons_traverse():
 /project/consmodule.c:140
 	push   %r12
@@ -956,69 +956,69 @@
 	pop    %rbp
 	pop    %r12
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 
 0000000000002ba0 <Cons_to_list>:
 Cons_to_list():
-/project/consmodule.c:221
+/project/consmodule.c:234
 	push   %rbx
-/project/consmodule.c:222
+/project/consmodule.c:235
 	test   %rcx,%rcx
 	jne    2c10 <Cons_to_list+0x70>
 	mov    %rdi,%rbx
-/project/consmodule.c:226
+/project/consmodule.c:239
 	movslq 0x20(%rdi),%rdi
 	test   %edi,%edi
 	jle    2bf0 <Cons_to_list+0x50>
-/project/consmodule.c:231
+/project/consmodule.c:244
 	call   2190 <PyList_New@plt>
-/project/consmodule.c:233
+/project/consmodule.c:246
 	movslq 0x20(%rbx),%rcx
 	test   %ecx,%ecx
 	jle    2be9 <Cons_to_list+0x49>
 	mov    0x18(%rax),%rdx
 	lea    (%rdx,%rcx,8),%rsi
 	cs nopw 0x0(%rax,%rax,1)
-/project/consmodule.c:234 (discriminator 3)
+/project/consmodule.c:247 (discriminator 3)
 	mov    0x10(%rbx),%rcx
 Py_INCREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:502 (discriminator 3)
 	add    $0x8,%rdx
 	addq   $0x1,(%rcx)
 PyList_SET_ITEM():
 /opt/_internal/cpython-3.11.2/include/python3.11/cpython/listobject.h:46 (discriminator 3)
 	mov    %rcx,-0x8(%rdx)
 Cons_to_list():
-/project/consmodule.c:233 (discriminator 3)
+/project/consmodule.c:246 (discriminator 3)
 	mov    0x18(%rbx),%rbx
 	cmp    %rdx,%rsi
 	jne    2bd0 <Cons_to_list+0x30>
-/project/consmodule.c:239
+/project/consmodule.c:252
 	pop    %rbx
 	ret
 	nopl   0x0(%rax,%rax,1)
-/project/consmodule.c:227
+/project/consmodule.c:240
 	mov    0x23d9(%rip),%rax        
 	lea    0x43a(%rip),%rsi        
 	mov    (%rax),%rdi
 	call   2080 <PyErr_SetString@plt>
-/project/consmodule.c:228
+/project/consmodule.c:241
 	xor    %eax,%eax
-/project/consmodule.c:239
+/project/consmodule.c:252
 	pop    %rbx
 	ret
 	nopw   0x0(%rax,%rax,1)
-/project/consmodule.c:223
+/project/consmodule.c:236
 	mov    0x23c1(%rip),%rax        
 	lea    0x402(%rip),%rsi        
 	mov    (%rax),%rdi
 	call   2080 <PyErr_SetString@plt>
 	xor    %eax,%eax
-/project/consmodule.c:239
+/project/consmodule.c:252
 	pop    %rbx
 	ret
 	nopw   0x0(%rax,%rax,1)
 
 0000000000002c30 <Nil_new>:
 Nil_new():
 /project/consmodule.c:62
@@ -1076,244 +1076,258 @@
 Cons_from_fast():
 /project/consmodule.c:167
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
-/project/consmodule.c:171
-	mov    0x8(%rdi),%rax
-/project/consmodule.c:173
-	mov    0x10(%rdi),%rbx
 /project/consmodule.c:168
 	mov    0x8(%rsi),%r12
-/project/consmodule.c:169
-	mov    0x10(%rsi),%r13
-/project/consmodule.c:171
+/project/consmodule.c:172
+	mov    0x8(%rdi),%rax
+/project/consmodule.c:170
+	mov    0x10(%rsi),%rbx
+Py_INCREF():
+/opt/_internal/cpython-3.11.2/include/python3.11/object.h:502
+	addq   $0x1,(%r12)
+Cons_from_fast():
+/project/consmodule.c:174
+	mov    0x10(%rdi),%r13
+/project/consmodule.c:172
 	mov    0xa8(%rax),%rax
-/project/consmodule.c:173
-	sub    $0x1,%rbx
-	js     2d35 <Cons_from_fast+0x95>
+/project/consmodule.c:174
+	sub    $0x1,%r13
+	js     2d42 <Cons_from_fast+0xa2>
 	mov    %rdi,%r14
-	jmp    2d13 <Cons_from_fast+0x73>
-	nopw   0x0(%rax,%rax,1)
-/project/consmodule.c:174 (discriminator 1)
+	jmp    2d18 <Cons_from_fast+0x78>
+	nop
+/project/consmodule.c:175 (discriminator 1)
 	mov    0x18(%r14),%rax
-	mov    (%rax,%rbx,8),%rbp
+	mov    (%rax,%r13,8),%rbp
 Py_INCREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:502 (discriminator 4)
 	addq   $0x1,0x0(%rbp)
 Cons_from_fast():
-/project/consmodule.c:176 (discriminator 4)
+/project/consmodule.c:177 (discriminator 4)
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
+	mov    %rbx,%rdi
 	xor    %eax,%eax
 	mov    %rbp,%rsi
-	mov    %r13,%rdi
 	call   2120 <PyObject_CallFunctionObjArgs@plt>
-Py_DECREF():
-/opt/_internal/cpython-3.11.2/include/python3.11/object.h:537 (discriminator 4)
-	subq   $0x1,0x0(%rbp)
-Cons_from_fast():
-/project/consmodule.c:176 (discriminator 4)
+/project/consmodule.c:189 (discriminator 4)
+	mov    0x18(%rax),%rdi
+/project/consmodule.c:177 (discriminator 4)
 	mov    %rax,%r12
 Py_DECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:537 (discriminator 4)
-	je     2d28 <Cons_from_fast+0x88>
+	subq   $0x1,(%rdi)
+	je     2d50 <Cons_from_fast+0xb0>
+/opt/_internal/cpython-3.11.2/include/python3.11/object.h:537
+	subq   $0x1,0x0(%rbp)
+	je     2d30 <Cons_from_fast+0x90>
 Cons_from_fast():
-/project/consmodule.c:178
-	test   %r12,%r12
-	je     2d35 <Cons_from_fast+0x95>
-/project/consmodule.c:173 (discriminator 2)
-	sub    $0x1,%rbx
-	cmp    $0xffffffffffffffff,%rbx
-	je     2d35 <Cons_from_fast+0x95>
+/project/consmodule.c:174
+	sub    $0x1,%r13
+	cmp    $0xffffffffffffffff,%r13
+	je     2d42 <Cons_from_fast+0xa2>
 	mov    0x8(%r14),%rax
 	mov    0xa8(%rax),%rax
-/project/consmodule.c:174
+/project/consmodule.c:175
 	test   $0x2000000,%eax
 	jne    2cd0 <Cons_from_fast+0x30>
-/project/consmodule.c:174 (discriminator 2)
-	mov    0x18(%r14,%rbx,8),%rbp
+/project/consmodule.c:175 (discriminator 2)
+	mov    0x18(%r14,%r13,8),%rbp
 	jmp    2cd8 <Cons_from_fast+0x38>
-	nopl   0x0(%rax)
+	cs nopw 0x0(%rax,%rax,1)
 Py_DECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:538
 	mov    %rbp,%rdi
+Cons_from_fast():
+/project/consmodule.c:174
+	sub    $0x1,%r13
+Py_DECREF():
+/opt/_internal/cpython-3.11.2/include/python3.11/object.h:538
 	call   21b0 <_Py_Dealloc@plt>
 Cons_from_fast():
-/project/consmodule.c:178
-	test   %r12,%r12
-	jne    2cfe <Cons_from_fast+0x5e>
-/project/consmodule.c:183
+/project/consmodule.c:174
+	cmp    $0xffffffffffffffff,%r13
+	jne    2d0d <Cons_from_fast+0x6d>
+/project/consmodule.c:196
 	pop    %rbx
 	mov    %r12,%rax
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
-	data16 cs nopw 0x0(%rax,%rax,1)
-	nopl   0x0(%rax)
+	xchg   %ax,%ax
+Py_DECREF():
+/opt/_internal/cpython-3.11.2/include/python3.11/object.h:538
+	call   21b0 <_Py_Dealloc@plt>
+	jmp    2cfc <Cons_from_fast+0x5c>
+Cons_from_fast():
+/opt/_internal/cpython-3.11.2/include/python3.11/object.h:538
+	nopw   0x0(%rax,%rax,1)
 
-0000000000002d50 <Cons_from_xs>:
+0000000000002d60 <Cons_from_xs>:
 Cons_from_xs():
-/project/consmodule.c:188
+/project/consmodule.c:201
 	push   %r13
 	push   %r12
 	push   %rbp
-/project/consmodule.c:189
+/project/consmodule.c:202
 	cmp    $0x1,%rcx
-	jne    2de8 <Cons_from_xs+0x98>
+	jne    2df8 <Cons_from_xs+0x98>
 	mov    %rsi,%rdi
 	mov    %rdx,%r12
-/project/consmodule.c:194
+/project/consmodule.c:207
 	call   2270 <PyType_GetModuleState@plt>
 	mov    %rax,%r13
-/project/consmodule.c:195
+/project/consmodule.c:208
 	test   %rax,%rax
-	je     2e68 <Cons_from_xs+0x118>
-/project/consmodule.c:198
+	je     2e78 <Cons_from_xs+0x118>
+/project/consmodule.c:211
 	mov    (%r12),%rbp
 PyObject_TypeCheck():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:263
-	mov    0x226f(%rip),%rsi        
+	mov    0x225f(%rip),%rsi        
 Py_IS_TYPE():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:150
 	mov    0x8(%rbp),%rdi
 PyObject_TypeCheck():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:263
 	cmp    %rsi,%rdi
-	je     2d93 <Cons_from_xs+0x43>
+	je     2da3 <Cons_from_xs+0x43>
 	call   21f0 <PyType_IsSubtype@plt>
 	test   %eax,%eax
-	je     2e10 <Cons_from_xs+0xc0>
+	je     2e20 <Cons_from_xs+0xc0>
 Cons_from_xs():
-/project/consmodule.c:205
+/project/consmodule.c:218
 	mov    %rbp,%rdi
 	call   20b0 <PySequence_Tuple@plt>
-/project/consmodule.c:209
-	lea    0x356(%rip),%rsi        
+/project/consmodule.c:222
+	lea    0x346(%rip),%rsi        
 	mov    %rax,%rdi
-/project/consmodule.c:205
+/project/consmodule.c:218
 	mov    %rax,%rbp
-/project/consmodule.c:209
+/project/consmodule.c:222
 	call   2050 <PySequence_Fast@plt>
 	mov    %rax,%r12
 	test   %rax,%rax
-	je     2dcd <Cons_from_xs+0x7d>
-/project/consmodule.c:210
+	je     2ddd <Cons_from_xs+0x7d>
+/project/consmodule.c:223
 	mov    %r13,%rsi
 	mov    %rax,%rdi
 	call   2150 <Cons_from_fast@plt>
 Py_DECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:537
 	subq   $0x1,(%r12)
 Cons_from_xs():
-/project/consmodule.c:210
+/project/consmodule.c:223
 	mov    %rax,%r13
 Py_DECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:537
-	je     2e40 <Cons_from_xs+0xf0>
+	je     2e50 <Cons_from_xs+0xf0>
 Cons_from_xs():
-/project/consmodule.c:210
+/project/consmodule.c:223
 	mov    %rax,%r12
 Py_XDECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:601 (discriminator 1)
 	test   %rbp,%rbp
-	je     2dd9 <Cons_from_xs+0x89>
+	je     2de9 <Cons_from_xs+0x89>
 Py_DECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:537
 	subq   $0x1,0x0(%rbp)
-	je     2e50 <Cons_from_xs+0x100>
+	je     2e60 <Cons_from_xs+0x100>
 Cons_from_xs():
-/project/consmodule.c:216
+/project/consmodule.c:229
 	mov    %r12,%rax
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	nopw   0x0(%rax,%rax,1)
-/project/consmodule.c:190
-	mov    0x21e9(%rip),%rax        
-/project/consmodule.c:191
+/project/consmodule.c:203
+	mov    0x21d9(%rip),%rax        
+/project/consmodule.c:204
 	xor    %r12d,%r12d
-/project/consmodule.c:190
-	lea    0x2d7(%rip),%rsi        
+/project/consmodule.c:203
+	lea    0x2c7(%rip),%rsi        
 	mov    (%rax),%rdi
 	call   2080 <PyErr_SetString@plt>
-/project/consmodule.c:216
+/project/consmodule.c:229
 	mov    %r12,%rax
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	nopw   0x0(%rax,%rax,1)
-/project/consmodule.c:209
+/project/consmodule.c:222
 	mov    %rbp,%rdi
-	lea    0x2de(%rip),%rsi        
+	lea    0x2ce(%rip),%rsi        
 	call   2050 <PySequence_Fast@plt>
 	mov    %rax,%rbp
 	test   %rax,%rax
-	je     2e68 <Cons_from_xs+0x118>
-/project/consmodule.c:210
+	je     2e78 <Cons_from_xs+0x118>
+/project/consmodule.c:223
 	mov    %r13,%rsi
 	mov    %rax,%rdi
 	call   2150 <Cons_from_fast@plt>
 	mov    %rax,%r12
-	jmp    2dd2 <Cons_from_xs+0x82>
+	jmp    2de2 <Cons_from_xs+0x82>
 	nopw   0x0(%rax,%rax,1)
 Py_DECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:538
 	mov    %r12,%rdi
 Cons_from_xs():
-/project/consmodule.c:210
+/project/consmodule.c:223
 	mov    %r13,%r12
 Py_DECREF():
 /opt/_internal/cpython-3.11.2/include/python3.11/object.h:538
 	call   21b0 <_Py_Dealloc@plt>
-	jmp    2dcd <Cons_from_xs+0x7d>
+	jmp    2ddd <Cons_from_xs+0x7d>
 	nopl   (%rax)
 	mov    %rbp,%rdi
 	call   21b0 <_Py_Dealloc@plt>
 Cons_from_xs():
-/project/consmodule.c:216
+/project/consmodule.c:229
 	mov    %r12,%rax
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	nopl   0x0(%rax)
-/project/consmodule.c:196
+/project/consmodule.c:209
 	xor    %r12d,%r12d
-/project/consmodule.c:216
+/project/consmodule.c:229
 	pop    %rbp
 	mov    %r12,%rax
 	pop    %r12
 	pop    %r13
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nop
 
-0000000000002e80 <PyInit_fastcons>:
+0000000000002e90 <PyInit_fastcons>:
 PyInit_fastcons():
-/project/consmodule.c:464
-	lea    0x2299(%rip),%rdi        
+/project/consmodule.c:477
+	lea    0x2289(%rip),%rdi        
 	jmp    20a0 <PyModuleDef_Init@plt>
 
-0000000000002e8c <__do_global_ctors_aux>:
+0000000000002e9c <__do_global_ctors_aux>:
 __do_global_ctors_aux():
 	push   %rbp
 	mov    %rsp,%rbp
 	push   %rbx
-	lea    0x1e28(%rip),%rbx        
+	lea    0x1e18(%rip),%rbx        
 	push   %rdx
 	mov    (%rbx),%rax
 	cmp    $0xffffffffffffffff,%rax
-	je     2eaa <__do_global_ctors_aux+0x1e>
+	je     2eba <__do_global_ctors_aux+0x1e>
 	call   *%rax
 	sub    $0x8,%rbx
-	jmp    2e99 <__do_global_ctors_aux+0xd>
+	jmp    2ea9 <__do_global_ctors_aux+0xd>
 	pop    %rax
 	pop    %rbx
 	pop    %rbp
 	ret
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.fini {}

```diff
@@ -1,13 +1,13 @@
 
 
 
 Disassembly of section .fini:
 
-0000000000002eae <_fini>:
+0000000000002ebe <_fini>:
 _fini():
 /home/buildozer/aports/main/musl/src/musl-1.1.24/crt/x86_64/crti.s:9
 	push   %rax
 	call   230b <__do_global_dtors_aux>
 /home/buildozer/aports/main/musl/src/musl-1.1.24/crt/x86_64/crtn.s:6
 	pop    %rax
 /home/buildozer/aports/main/musl/src/musl-1.1.24/crt/x86_64/crtn.s:7
```

### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -5,10 +5,10 @@
   0x000031f0 00010000 10f2ffff 14010000 20f2ffff ............ ...
   0x00003200 28010000 30f2ffff 3c010000 60f3ffff (...0...<...`...
   0x00003210 78010000 c0f3ffff 9c010000 60f4ffff x...........`...
   0x00003220 dc010000 e0f4ffff 00020000 40f5ffff ............@...
   0x00003230 38020000 50f7ffff 84020000 70f8ffff 8...P.......p...
   0x00003240 b4020000 70f9ffff 38030000 d0f9ffff ....p...8.......
   0x00003250 70030000 60faffff 98030000 d0faffff p...`...........
-  0x00003260 cc030000 80fbffff 08040000 b0fcffff ................
-  0x00003270 58040000                            X...
+  0x00003260 cc030000 90fbffff 0c040000 c0fcffff ................
+  0x00003270 5c040000                            \...
```

### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -46,19 +46,19 @@
   0x00003528 730a0e18 470e1042 0e084a0b 410e1841 s...G..B..J.A..A
   0x00003538 0e10420e 08000000 24000000 cc020000 ..B.....$.......
   0x00003548 58f6ffff 8a000000 00410e10 83020249 X........A.....I
   0x00003558 0a0e0846 0b590a0e 08470b59 0e080000 ...F.Y...G.Y....
   0x00003568 30000000 f4020000 c0f6ffff 70000000 0...........p...
   0x00003578 00420e10 8c02470e 18860347 0e20750a .B....G....G. u.
   0x00003588 0e18410e 10420e08 480b5a0e 18430e10 ..A..B..H.Z..C..
-  0x00003598 420e0800 38000000 28030000 fcf6ffff B...8...(.......
-  0x000035a8 a1000000 00420e10 8e02420e 188d0342 .....B....B....B
-  0x000035b8 0e208c04 410e2886 05410e30 8306028e . ..A.(..A.0....
-  0x000035c8 0e28440e 20420e18 420e1042 0e080000 .(D. B..B..B....
-  0x000035d8 4c000000 64030000 70f7ffff 24010000 L...d...p...$...
-  0x000035e8 00420e10 8d02420e 188c0341 0e208604 .B....B....A. ..
-  0x000035f8 02880a0e 18420e10 420e0847 0b5d0a0e .....B..B..G.]..
-  0x00003608 18420e10 420e0847 0b024c0a 0e18420e .B..B..G..L...B.
-  0x00003618 10420e08 480b440e 18450e10 420e0800 .B..H.D..E..B...
-  0x00003628 10000000 b4030000 50f8ffff 0c000000 ........P.......
-  0x00003638 00000000 00000000                   ........
+  0x00003598 420e0800 3c000000 28030000 fcf6ffff B...<...(.......
+  0x000035a8 b7000000 00420e10 8e02420e 188d0342 .....B....B....B
+  0x000035b8 0e208c04 410e2886 05410e30 8306029b . ..A.(..A.0....
+  0x000035c8 0a0e2844 0e20420e 18420e10 420e0843 ..(D. B..B..B..C
+  0x000035d8 0b000000 4c000000 68030000 7cf7ffff ....L...h...|...
+  0x000035e8 24010000 00420e10 8d02420e 188c0341 $....B....B....A
+  0x000035f8 0e208604 02880a0e 18420e10 420e0847 . .......B..B..G
+  0x00003608 0b5d0a0e 18420e10 420e0847 0b024c0a .]...B..B..G..L.
+  0x00003618 0e18420e 10420e08 480b440e 18450e10 ..B..B..H.D..E..
+  0x00003628 420e0800 10000000 b8030000 5cf8ffff B...........\...
+  0x00003638 0c000000 00000000 00000000          ............
```

## Comparing `fastcons-0.2.0.dist-info/LICENSE.txt` & `fastcons-0.2.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `fastcons-0.2.0.dist-info/METADATA` & `fastcons-0.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastcons
-Version: 0.2.0
+Version: 0.2.1
 Summary: An efficient implementation of cons
 Author-email: Joshua Munn <public@elysee-munn.family>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Provides-Extra: build
 Requires-Dist: build (==0.10.0) ; extra == 'build'
```

