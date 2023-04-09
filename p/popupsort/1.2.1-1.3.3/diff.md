# Comparing `tmp/popupsort-1.2.1.tar.gz` & `tmp/popupsort-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popupsort-1.2.1.tar", last modified: Sat Mar 25 09:39:06 2023, max compression
+gzip compressed data, was "popupsort-1.3.3.tar", last modified: Sun Apr  9 15:48:13 2023, max compression
```

## Comparing `popupsort-1.2.1.tar` & `popupsort-1.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-25 09:39:06.852923 popupsort-1.2.1/
--rw-rw-rw-   0        0        0     1093 2023-03-18 09:14:08.000000 popupsort-1.2.1/LICENSE.md
--rw-rw-rw-   0        0        0     2105 2023-03-25 09:39:06.852923 popupsort-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1410 2023-03-24 13:40:27.000000 popupsort-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-25 09:39:06.836934 popupsort-1.2.1/popupsort/
--rw-rw-rw-   0        0        0       41 2023-03-18 09:14:08.000000 popupsort-1.2.1/popupsort/__init__.py
--rw-rw-rw-   0        0        0     5061 2023-03-25 09:38:38.000000 popupsort-1.2.1/popupsort/popupsort.py
-drwxrwxrwx   0        0        0        0 2023-03-25 09:39:06.851894 popupsort-1.2.1/popupsort.egg-info/
--rw-rw-rw-   0        0        0     2105 2023-03-25 09:39:06.000000 popupsort-1.2.1/popupsort.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-03-25 09:39:06.000000 popupsort-1.2.1/popupsort.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-25 09:39:06.000000 popupsort-1.2.1/popupsort.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-18 09:46:14.000000 popupsort-1.2.1/popupsort.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-03-25 09:39:06.000000 popupsort-1.2.1/popupsort.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-25 09:39:06.854923 popupsort-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      574 2023-03-25 09:38:45.000000 popupsort-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 15:48:13.678715 popupsort-1.3.3/
+-rw-rw-rw-   0        0        0     1093 2023-03-18 09:14:08.000000 popupsort-1.3.3/LICENSE.md
+-rw-rw-rw-   0        0        0     2552 2023-04-09 15:48:13.679725 popupsort-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1785 2023-04-09 15:41:22.000000 popupsort-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 15:48:13.663776 popupsort-1.3.3/popupsort/
+-rw-rw-rw-   0        0        0       41 2023-03-18 09:14:08.000000 popupsort-1.3.3/popupsort/__init__.py
+-rw-rw-rw-   0        0        0     9991 2023-04-09 15:47:57.000000 popupsort-1.3.3/popupsort/popupsort.py
+drwxrwxrwx   0        0        0        0 2023-04-09 15:48:13.677717 popupsort-1.3.3/popupsort.egg-info/
+-rw-rw-rw-   0        0        0     2552 2023-04-09 15:48:13.000000 popupsort-1.3.3/popupsort.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-04-09 15:48:13.000000 popupsort-1.3.3/popupsort.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 15:48:13.000000 popupsort-1.3.3/popupsort.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-18 09:46:14.000000 popupsort-1.3.3/popupsort.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-04-09 15:48:13.000000 popupsort-1.3.3/popupsort.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 15:48:13.680709 popupsort-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      574 2023-04-09 15:48:06.000000 popupsort-1.3.3/setup.py
```

### Comparing `popupsort-1.2.1/LICENSE.md` & `popupsort-1.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `popupsort-1.2.1/README.md` & `popupsort-1.3.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,89 +1,112 @@
-00000000: 2320 506f 7055 7053 6f72 740d 0a57 6974  # PopUpSort..Wit
-00000010: 6820 7468 6520 6173 7369 7374 616e 6365  h the assistance
-00000020: 206f 6620 4368 6174 4750 542d 332e 352c   of ChatGPT-3.5,
-00000030: 2049 2077 6173 2061 626c 6520 746f 2063   I was able to c
-00000040: 7265 6174 6520 7468 6973 2073 6f72 7469  reate this sorti
-00000050: 6e67 2076 6973 7561 6c69 7a65 722e 200d  ng visualizer. .
-00000060: 0a0d 0a54 6865 2050 6f70 5570 536f 7274  ...The PopUpSort
-00000070: 2070 6163 6b61 6765 2069 7320 6120 5079   package is a Py
-00000080: 7468 6f6e 2070 6163 6b61 6765 2074 6861  thon package tha
-00000090: 7420 7669 7375 616c 697a 6573 2074 6865  t visualizes the
-000000a0: 2073 6f72 7469 6e67 2061 6c67 6f72 6974   sorting algorit
-000000b0: 686d 733a 2062 7562 626c 6520 736f 7274  hms: bubble sort
-000000c0: 2c20 7365 6c65 6374 696f 6e20 736f 7274  , selection sort
-000000d0: 2c20 616e 6420 696e 7365 7274 696f 6e20  , and insertion 
-000000e0: 736f 7274 2e20 5468 6520 7061 636b 6167  sort. The packag
-000000f0: 6520 7573 6573 2074 6865 2054 6b69 6e74  e uses the Tkint
-00000100: 6572 206c 6962 7261 7279 2066 6f72 2074  er library for t
-00000110: 6865 2067 7261 7068 6963 616c 2075 7365  he graphical use
-00000120: 7220 696e 7465 7266 6163 652e 0d0a 0d0a  r interface.....
-00000130: 2320 5265 7175 6972 656d 656e 7473 0d0a  # Requirements..
-00000140: 2d20 5079 7468 6f6e 2033 2e78 0d0a 2d20  - Python 3.x..- 
-00000150: 746b 696e 7465 7220 6c69 6272 6172 7920  tkinter library 
-00000160: 2869 6e63 6c75 6465 6420 696e 206d 6f73  (included in mos
-00000170: 7420 5079 7468 6f6e 2069 6e73 7461 6c6c  t Python install
-00000180: 6174 696f 6e73 290d 0a0d 0a23 2049 6e73  ations)....# Ins
-00000190: 7461 6c6c 6174 696f 6e0d 0a0d 0a23 2323  tallation....###
-000001a0: 204d 6574 686f 6420 313a 2055 7369 6e67   Method 1: Using
-000001b0: 2070 6970 0d0a 6060 6070 7974 686f 6e0d   pip..```python.
-000001c0: 0a70 6970 2069 6e73 7461 6c6c 2070 6f70  .pip install pop
-000001d0: 7570 736f 7274 0d0a 6060 600d 0a23 2323  upsort..```..###
-000001e0: 204d 6574 686f 6420 323a 2044 6f77 6e6c   Method 2: Downl
-000001f0: 6f61 6420 7468 6520 736f 7572 6365 2063  oad the source c
-00000200: 6f64 652c 2074 6865 6e20 6f70 656e 2074  ode, then open t
-00000210: 6572 6d69 6e61 6c20 696e 2074 6865 2064  erminal in the d
-00000220: 6f77 6e6c 6f61 6465 6420 666f 6c64 6572  ownloaded folder
-00000230: 2028 7768 6572 6520 7365 7475 702e 7079   (where setup.py
-00000240: 2069 7329 2061 6e64 2072 756e 0d0a 6060   is) and run..``
-00000250: 6070 7974 686f 6e0d 0a70 6970 2069 6e73  `python..pip ins
-00000260: 7461 6c6c 202e 0d0a 6060 600d 0a0d 0a23  tall ...```....#
-00000270: 2055 7361 6765 0d0a 2323 2320 4669 7273   Usage..### Firs
-00000280: 7420 696d 706f 7274 2074 6865 2070 6163  t import the pac
-00000290: 6b61 6765 0d0a 6060 6070 7974 686f 6e0d  kage..```python.
-000002a0: 0a69 6d70 6f72 7420 706f 7075 7073 6f72  .import popupsor
-000002b0: 7420 6173 2070 7573 0d0a 6060 600d 0a0d  t as pus..```...
-000002c0: 0a23 2323 2053 796e 7461 780d 0a60 6060  .### Syntax..```
-000002d0: 7079 7468 6f6e 0d0a 7075 732e 736f 7274  python..pus.sort
-000002e0: 2861 7272 6179 2c20 616c 676f 7269 7468  (array, algorith
-000002f0: 6d2c 2073 7065 6564 2920 2320 536f 7274  m, speed) # Sort
-00000300: 696e 6720 616e 2061 6c72 6561 6479 2064  ing an already d
-00000310: 6566 696e 6564 2061 7272 6179 0d0a 0d0a  efined array....
-00000320: 7075 732e 736f 7274 5f72 616e 6428 7369  pus.sort_rand(si
-00000330: 7a65 2c20 6d69 6e2c 206d 6178 2c20 616c  ze, min, max, al
-00000340: 676f 7269 7468 6d2c 2073 7065 6564 2920  gorithm, speed) 
-00000350: 2320 4175 746f 2067 656e 6572 6174 6520  # Auto generate 
-00000360: 616e 2061 7272 6179 2061 6e64 2073 6f72  an array and sor
-00000370: 7420 6974 0d0a 6060 600d 0a0d 0a23 2323  t it..```....###
-00000380: 2041 6c67 6f72 6974 686d 730d 0a0d 0a52   Algorithms....R
-00000390: 6570 6c61 6365 2027 616c 676f 7269 7468  eplace 'algorith
-000003a0: 6d27 2061 7267 756d 656e 7420 7769 7468  m' argument with
-000003b0: 2061 6e79 206f 6620 7468 6573 6520 6f70   any of these op
-000003c0: 7469 6f6e 733a 0d0a 2d20 2742 7562 626c  tions:..- 'Bubbl
-000003d0: 6520 536f 7274 2720 6f72 2027 6227 0d0a  e Sort' or 'b'..
-000003e0: 2d20 2753 656c 6563 7469 6f6e 2053 6f72  - 'Selection Sor
-000003f0: 7427 206f 7220 2773 270d 0a2d 2027 496e  t' or 's'..- 'In
-00000400: 7365 7274 696f 6e20 536f 7274 2720 6f72  sertion Sort' or
-00000410: 2027 6927 0d0a 0d0a 2323 2320 4578 616d   'i'....### Exam
-00000420: 706c 6573 0d0a 6060 6070 7974 686f 6e0d  ples..```python.
-00000430: 0a61 7272 203d 205b 3630 2c32 342c 3231  .arr = [60,24,21
-00000440: 2c36 352c 3933 2c35 362c 3335 2c31 302c  ,65,93,56,35,10,
-00000450: 3535 2c34 392c 3836 2c37 365d 2023 2044  55,49,86,76] # D
-00000460: 6566 696e 6520 616e 2061 7272 6179 0d0a  efine an array..
-00000470: 7075 732e 736f 7274 2861 7272 2c20 2762  pus.sort(arr, 'b
-00000480: 272c 2030 2e30 3229 2020 2020 2020 2020  ', 0.02)        
-00000490: 2020 2020 2020 2020 2020 2020 2320 5669              # Vi
-000004a0: 7375 616c 697a 6520 7468 6520 6275 6262  sualize the bubb
-000004b0: 6c65 2073 6f72 7420 6f66 2074 6869 7320  le sort of this 
-000004c0: 6172 7261 7920 7769 7468 2061 2073 7065  array with a spe
-000004d0: 6564 206f 6620 302e 3032 730d 0a0d 0a70  ed of 0.02s....p
-000004e0: 7573 2e73 6f72 745f 7261 6e64 2835 302c  us.sort_rand(50,
-000004f0: 2031 2c20 3130 302c 2027 6927 2920 2320   1, 100, 'i') # 
-00000500: 4765 6e65 7261 7465 2061 6e20 6172 7261  Generate an arra
-00000510: 7920 6f66 2073 697a 6520 3530 2077 6974  y of size 50 wit
-00000520: 6820 656c 656d 656e 7473 2072 616e 6769  h elements rangi
-00000530: 6e67 2066 726f 6d20 3120 746f 2031 3030  ng from 1 to 100
-00000540: 2061 6e64 2073 6f72 7420 6974 2075 7369   and sort it usi
-00000550: 6e67 2069 6e73 6572 7469 6f6e 2073 6f72  ng insertion sor
-00000560: 742c 2073 7065 6564 2069 7320 302e 3031  t, speed is 0.01
-00000570: 2062 7920 6465 6661 756c 740d 0a60 6060   by default..```
-00000580: 0d0a                                     ..
+00000000: 2320 506f 7055 7053 6f72 740d 0a0d 0a3c  # PopUpSort....<
+00000010: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+00000020: 3e0d 0a3c 6120 6872 6566 3d22 6874 7470  >..<a href="http
+00000030: 733a 2f2f 6869 7473 2e73 6565 796f 7566  s://hits.seeyouf
+00000040: 6172 6d2e 636f 6d22 3e3c 696d 6720 7372  arm.com"><img sr
+00000050: 633d 2268 7474 7073 3a2f 2f68 6974 732e  c="https://hits.
+00000060: 7365 6579 6f75 6661 726d 2e63 6f6d 2f61  seeyoufarm.com/a
+00000070: 7069 2f63 6f75 6e74 2f69 6e63 722f 6261  pi/count/incr/ba
+00000080: 6467 652e 7376 673f 7572 6c3d 6874 7470  dge.svg?url=http
+00000090: 7325 3341 2532 4625 3246 6769 7468 7562  s%3A%2F%2Fgithub
+000000a0: 2e63 6f6d 2532 465a 6f75 6865 6972 4e25  .com%2FZouheirN%
+000000b0: 3246 506f 7055 7053 6f72 7426 636f 756e  2FPopUpSort&coun
+000000c0: 745f 6267 3d25 3233 4646 4434 3342 2674  t_bg=%23FFD43B&t
+000000d0: 6974 6c65 5f62 673d 2532 3333 3036 3939  itle_bg=%2330699
+000000e0: 3826 6963 6f6e 3d26 6963 6f6e 5f63 6f6c  8&icon=&icon_col
+000000f0: 6f72 3d25 3233 4537 4537 4537 2674 6974  or=%23E7E7E7&tit
+00000100: 6c65 3d68 6974 7326 6564 6765 5f66 6c61  le=hits&edge_fla
+00000110: 743d 6661 6c73 6522 2f3e 3c2f 613e 0d0a  t=false"/></a>..
+00000120: 3c2f 703e 0d0a 0d0a 5769 7468 2074 6865  </p>....With the
+00000130: 2061 7373 6973 7461 6e63 6520 6f66 2043   assistance of C
+00000140: 6861 7447 5054 2d33 2e35 2c20 4920 7761  hatGPT-3.5, I wa
+00000150: 7320 6162 6c65 2074 6f20 6372 6561 7465  s able to create
+00000160: 2074 6869 7320 736f 7274 696e 6720 7669   this sorting vi
+00000170: 7375 616c 697a 6572 2e20 0d0a 0d0a 5468  sualizer. ....Th
+00000180: 6520 506f 7055 7053 6f72 7420 7061 636b  e PopUpSort pack
+00000190: 6167 6520 6973 2061 2050 7974 686f 6e20  age is a Python 
+000001a0: 7061 636b 6167 6520 7468 6174 2076 6973  package that vis
+000001b0: 7561 6c69 7a65 7320 7468 6520 736f 7274  ualizes the sort
+000001c0: 696e 6720 616c 676f 7269 7468 6d73 3a20  ing algorithms: 
+000001d0: 6275 6262 6c65 2073 6f72 742c 2073 656c  bubble sort, sel
+000001e0: 6563 7469 6f6e 2073 6f72 742c 2061 6e64  ection sort, and
+000001f0: 2069 6e73 6572 7469 6f6e 2073 6f72 742e   insertion sort.
+00000200: 2054 6865 2070 6163 6b61 6765 2075 7365   The package use
+00000210: 7320 7468 6520 546b 696e 7465 7220 6c69  s the Tkinter li
+00000220: 6272 6172 7920 666f 7220 7468 6520 6772  brary for the gr
+00000230: 6170 6869 6361 6c20 7573 6572 2069 6e74  aphical user int
+00000240: 6572 6661 6365 2e0d 0a0d 0a23 2052 6571  erface.....# Req
+00000250: 7569 7265 6d65 6e74 730d 0a2d 2050 7974  uirements..- Pyt
+00000260: 686f 6e20 332e 780d 0a2d 2074 6b69 6e74  hon 3.x..- tkint
+00000270: 6572 206c 6962 7261 7279 2028 696e 636c  er library (incl
+00000280: 7564 6564 2069 6e20 6d6f 7374 2050 7974  uded in most Pyt
+00000290: 686f 6e20 696e 7374 616c 6c61 7469 6f6e  hon installation
+000002a0: 7329 0d0a 0d0a 2320 496e 7374 616c 6c61  s)....# Installa
+000002b0: 7469 6f6e 0d0a 0d0a 2323 2320 4d65 7468  tion....### Meth
+000002c0: 6f64 2031 3a20 5573 696e 6720 7069 700d  od 1: Using pip.
+000002d0: 0a60 6060 7079 7468 6f6e 0d0a 7069 7020  .```python..pip 
+000002e0: 696e 7374 616c 6c20 706f 7075 7073 6f72  install popupsor
+000002f0: 740d 0a60 6060 0d0a 2323 2320 4d65 7468  t..```..### Meth
+00000300: 6f64 2032 3a20 446f 776e 6c6f 6164 2074  od 2: Download t
+00000310: 6865 2073 6f75 7263 6520 636f 6465 2c20  he source code, 
+00000320: 7468 656e 206f 7065 6e20 7465 726d 696e  then open termin
+00000330: 616c 2069 6e20 7468 6520 646f 776e 6c6f  al in the downlo
+00000340: 6164 6564 2066 6f6c 6465 7220 2877 6865  aded folder (whe
+00000350: 7265 2073 6574 7570 2e70 7920 6973 2920  re setup.py is) 
+00000360: 616e 6420 7275 6e0d 0a60 6060 7079 7468  and run..```pyth
+00000370: 6f6e 0d0a 7069 7020 696e 7374 616c 6c20  on..pip install 
+00000380: 2e0d 0a60 6060 0d0a 0d0a 2320 5573 6167  ...```....# Usag
+00000390: 650d 0a23 2323 2046 6972 7374 2069 6d70  e..### First imp
+000003a0: 6f72 7420 7468 6520 7061 636b 6167 650d  ort the package.
+000003b0: 0a60 6060 7079 7468 6f6e 0d0a 696d 706f  .```python..impo
+000003c0: 7274 2070 6f70 7570 736f 7274 2061 7320  rt popupsort as 
+000003d0: 7075 730d 0a60 6060 0d0a 0d0a 2323 2320  pus..```....### 
+000003e0: 5379 6e74 6178 0d0a 6060 6070 7974 686f  Syntax..```pytho
+000003f0: 6e0d 0a70 7573 2e73 6f72 7428 6172 7261  n..pus.sort(arra
+00000400: 792c 2061 6c67 6f72 6974 686d 2c20 7370  y, algorithm, sp
+00000410: 6565 6429 2023 2053 6f72 7469 6e67 2061  eed) # Sorting a
+00000420: 6e20 616c 7265 6164 7920 6465 6669 6e65  n already define
+00000430: 6420 6172 7261 790d 0a0d 0a70 7573 2e73  d array....pus.s
+00000440: 6f72 745f 7261 6e64 2873 697a 652c 206d  ort_rand(size, m
+00000450: 696e 2c20 6d61 782c 2061 6c67 6f72 6974  in, max, algorit
+00000460: 686d 2c20 7370 6565 6429 2023 2041 7574  hm, speed) # Aut
+00000470: 6f20 6765 6e65 7261 7465 2061 6e20 6172  o generate an ar
+00000480: 7261 7920 616e 6420 736f 7274 2069 740d  ray and sort it.
+00000490: 0a60 6060 0d0a 0d0a 2323 2320 416c 676f  .```....### Algo
+000004a0: 7269 7468 6d73 0d0a 0d0a 5265 706c 6163  rithms....Replac
+000004b0: 6520 2761 6c67 6f72 6974 686d 2720 6172  e 'algorithm' ar
+000004c0: 6775 6d65 6e74 2077 6974 6820 616e 7920  gument with any 
+000004d0: 6f66 2074 6865 7365 206f 7074 696f 6e73  of these options
+000004e0: 3a0d 0a2d 2027 4275 6262 6c65 2053 6f72  :..- 'Bubble Sor
+000004f0: 7427 206f 7220 2762 270d 0a2d 2027 5365  t' or 'b'..- 'Se
+00000500: 6c65 6374 696f 6e20 536f 7274 2720 6f72  lection Sort' or
+00000510: 2027 7327 0d0a 2d20 2749 6e73 6572 7469   's'..- 'Inserti
+00000520: 6f6e 2053 6f72 7427 206f 7220 2769 270d  on Sort' or 'i'.
+00000530: 0a2d 2027 5175 6963 6b20 536f 7274 2720  .- 'Quick Sort' 
+00000540: 6f72 2027 7127 0d0a 2d20 274d 6572 6765  or 'q'..- 'Merge
+00000550: 2053 6f72 7427 206f 7220 276d 270d 0a2d   Sort' or 'm'..-
+00000560: 2027 4865 6170 2053 6f72 7427 206f 7220   'Heap Sort' or 
+00000570: 2768 270d 0a2d 2027 5368 656c 6c20 536f  'h'..- 'Shell So
+00000580: 7274 2720 6f72 2027 7368 270d 0a0d 0a23  rt' or 'sh'....#
+00000590: 2323 2045 7861 6d70 6c65 730d 0a60 6060  ## Examples..```
+000005a0: 7079 7468 6f6e 0d0a 6172 7220 3d20 5b36  python..arr = [6
+000005b0: 302c 3234 2c32 312c 3635 2c39 332c 3536  0,24,21,65,93,56
+000005c0: 2c33 352c 3130 2c35 352c 3439 2c38 362c  ,35,10,55,49,86,
+000005d0: 3736 5d20 2320 4465 6669 6e65 2061 6e20  76] # Define an 
+000005e0: 6172 7261 790d 0a70 7573 2e73 6f72 7428  array..pus.sort(
+000005f0: 6172 722c 2027 6227 2c20 302e 3032 2920  arr, 'b', 0.02) 
+00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000610: 2020 2023 2056 6973 7561 6c69 7a65 2074     # Visualize t
+00000620: 6865 2062 7562 626c 6520 736f 7274 206f  he bubble sort o
+00000630: 6620 7468 6973 2061 7272 6179 2077 6974  f this array wit
+00000640: 6820 6120 7370 6565 6420 6f66 2030 2e30  h a speed of 0.0
+00000650: 3273 0d0a 0d0a 7075 732e 736f 7274 5f72  2s....pus.sort_r
+00000660: 616e 6428 3530 2c20 312c 2031 3030 2c20  and(50, 1, 100, 
+00000670: 2769 2729 2023 2047 656e 6572 6174 6520  'i') # Generate 
+00000680: 616e 2061 7272 6179 206f 6620 7369 7a65  an array of size
+00000690: 2035 3020 7769 7468 2065 6c65 6d65 6e74   50 with element
+000006a0: 7320 7261 6e67 696e 6720 6672 6f6d 2031  s ranging from 1
+000006b0: 2074 6f20 3130 3020 616e 6420 736f 7274   to 100 and sort
+000006c0: 2069 7420 7573 696e 6720 696e 7365 7274   it using insert
+000006d0: 696f 6e20 736f 7274 2c20 7370 6565 6420  ion sort, speed 
+000006e0: 6973 2030 2e30 3120 6279 2064 6566 6175  is 0.01 by defau
+000006f0: 6c74 0d0a 6060 600d 0a                   lt..```..
```

### Comparing `popupsort-1.2.1/setup.py` & `popupsort-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name='popupsort',
-    version='1.2.1',
+    version='1.3.3',
     description='A Python package for visualizing sorting algorithms',
     long_description = README,
     long_description_content_type="text/markdown",
     author='Zouheir Nakouzi',
     author_email='zouheir2002@gmail.com',
     url='https://github.com/ZouheirN/PopUpSort',
     packages=['popupsort'],
```

