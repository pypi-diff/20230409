# Comparing `tmp/tensorscout-2.0.0.tar.gz` & `tmp/tensorscout-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorscout-2.0.0.tar", max compression
+gzip compressed data, was "tensorscout-2.1.0.tar", max compression
```

## Comparing `tensorscout-2.0.0.tar` & `tensorscout-2.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1077 2022-05-25 22:13:34.760586 tensorscout-2.0.0/LICENSE
--rw-r--r--   0        0        0      970 2023-04-02 06:33:41.034133 tensorscout-2.0.0/README.md
--rw-r--r--   0        0        0      460 2023-04-02 03:35:10.045058 tensorscout-2.0.0/pyproject.toml
--rw-r--r--   0        0        0       30 2023-04-02 04:18:08.970296 tensorscout-2.0.0/tensorscout/__init__.py
--rwxr-xr-x   0        0        0     3438 2023-04-02 06:30:52.975777 tensorscout-2.0.0/tensorscout/main.py
--rw-r--r--   0        0        0     1767 1970-01-01 00:00:00.000000 tensorscout-2.0.0/setup.py
--rw-r--r--   0        0        0     1747 1970-01-01 00:00:00.000000 tensorscout-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2022-05-25 22:13:34.760586 tensorscout-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1019 2023-04-03 22:00:18.346311 tensorscout-2.1.0/README.md
+-rw-r--r--   0        0        0      460 2023-04-09 00:10:26.242626 tensorscout-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-04-02 04:18:08.970296 tensorscout-2.1.0/tensorscout/__init__.py
+-rwxr-xr-x   0        0        0     5046 2023-04-08 23:46:24.549862 tensorscout-2.1.0/tensorscout/main.py
+-rw-r--r--   0        0        0     1816 1970-01-01 00:00:00.000000 tensorscout-2.1.0/setup.py
+-rw-r--r--   0        0        0     1796 1970-01-01 00:00:00.000000 tensorscout-2.1.0/PKG-INFO
```

### Comparing `tensorscout-2.0.0/LICENSE` & `tensorscout-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorscout-2.0.0/README.md` & `tensorscout-2.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,44 +18,47 @@
 00000110: 7273 636f 7574 2e72 6561 6474 6865 646f  rscout.readthedo
 00000120: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
 00000130: 3f62 6164 6765 3d6c 6174 6573 7429 0a0a  ?badge=latest)..
 00000140: 4120 5079 7468 6f6e 206c 6962 7261 7279  A Python library
 00000150: 2066 6f72 2074 656e 736f 7220 6f70 6572   for tensor oper
 00000160: 6174 696f 6e73 2070 6f77 6572 6564 2062  ations powered b
 00000170: 7920 7061 7261 6c6c 656c 2070 726f 6365  y parallel proce
-00000180: 7373 696e 672e 0a0a 3c69 6d67 2073 7263  ssing...<img src
-00000190: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-000001a0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-000001b0: 636f 6d2f 616e 6472 6577 7267 6172 6369  com/andrewrgarci
-000001c0: 612f 7465 6e73 6f72 7363 6f75 742f 6d61  a/tensorscout/ma
-000001d0: 696e 2f69 636f 6e5f 7363 6f75 742e 7376  in/icon_scout.sv
-000001e0: 6722 2077 6964 7468 3d22 3430 3022 3e0a  g" width="400">.
-000001f0: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
-00000200: 6e0a 0a60 6060 7275 6279 0a70 6970 2069  n..```ruby.pip i
-00000210: 6e73 7461 6c6c 2074 656e 736f 7273 636f  nstall tensorsco
-00000220: 7574 0a60 6060 0a0a 4974 2069 7320 7265  ut.```..It is re
-00000230: 636f 6d6d 656e 6465 6420 796f 7520 7275  commended you ru
-00000240: 6e20 766f 7865 6c6d 6170 2075 7369 6e67  n voxelmap using
-00000250: 2061 2060 7669 7274 7561 6c65 6e76 6020   a `virtualenv` 
-00000260: 7669 7274 7561 6c20 656e 7669 726f 6e6d  virtual environm
-00000270: 656e 742e 2054 6f20 646f 2073 6f2c 2066  ent. To do so, f
-00000280: 6f6c 6c6f 7720 7468 6520 6265 6c6f 7720  ollow the below 
-00000290: 7369 6d70 6c65 2070 726f 746f 636f 6c20  simple protocol 
-000002a0: 746f 2063 7265 6174 6520 7468 6520 7669  to create the vi
-000002b0: 7274 7561 6c20 656e 7669 726f 6e6d 656e  rtual environmen
-000002c0: 742c 2072 756e 2069 742c 2061 6e64 2069  t, run it, and i
-000002d0: 6e73 7461 6c6c 2074 6865 2070 6163 6b61  nstall the packa
-000002e0: 6765 2074 6865 7265 3a0a 0a60 6060 7275  ge there:..```ru
-000002f0: 6279 200a 7669 7274 7561 6c65 6e76 2076  by .virtualenv v
-00000300: 656e 760a 736f 7572 6365 2076 656e 762f  env.source venv/
-00000310: 6269 6e2f 6163 7469 7661 7465 0a70 6970  bin/activate.pip
-00000320: 2069 6e73 7461 6c6c 2074 656e 736f 7273   install tensors
-00000330: 636f 7574 0a60 6060 0a54 6f20 6578 6974  cout.```.To exit
-00000340: 2074 6865 2076 6972 7475 616c 2065 6e76   the virtual env
-00000350: 6972 6f6e 6d65 6e74 2c20 7369 6d70 6c79  ironment, simply
-00000360: 2074 7970 6520 6064 6561 6374 6976 6174   type `deactivat
-00000370: 6560 2e20 546f 2061 6363 6573 7320 6974  e`. To access it
-00000380: 2061 7420 616e 7920 6f74 6865 7220 7469   at any other ti
-00000390: 6d65 2061 6761 696e 2c20 656e 7465 7220  me again, enter 
-000003a0: 7769 7468 2074 6865 2061 626f 7665 2060  with the above `
-000003b0: 736f 7572 6365 2076 656e 762e 2e2e 6020  source venv...` 
-000003c0: 636f 6d6d 616e 642e 200a                 command. .
+00000180: 7373 696e 672e 0a0a 3c61 2068 7265 663d  ssing...<a href=
+00000190: 2268 7474 7073 3a2f 2f74 656e 736f 7273  "https://tensors
+000001a0: 636f 7574 2e72 6561 6474 6865 646f 6373  cout.readthedocs
+000001b0: 2e69 6f22 3e3c 696d 6720 7372 633d 2268  .io"><img src="h
+000001c0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+000001d0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+000001e0: 2f61 6e64 7265 7772 6761 7263 6961 2f74  /andrewrgarcia/t
+000001f0: 656e 736f 7273 636f 7574 2f6d 6169 6e2f  ensorscout/main/
+00000200: 6963 6f6e 5f73 636f 7574 2e70 6e67 2220  icon_scout.png" 
+00000210: 7769 6474 683d 2234 3030 223e 3c2f 613e  width="400"></a>
+00000220: 0a0a 0a23 2320 496e 7374 616c 6c61 7469  ...## Installati
+00000230: 6f6e 0a0a 6060 6072 7562 790a 7069 7020  on..```ruby.pip 
+00000240: 696e 7374 616c 6c20 7465 6e73 6f72 7363  install tensorsc
+00000250: 6f75 740a 6060 600a 0a49 7420 6973 2072  out.```..It is r
+00000260: 6563 6f6d 6d65 6e64 6564 2079 6f75 2072  ecommended you r
+00000270: 756e 2076 6f78 656c 6d61 7020 7573 696e  un voxelmap usin
+00000280: 6720 6120 6076 6972 7475 616c 656e 7660  g a `virtualenv`
+00000290: 2076 6972 7475 616c 2065 6e76 6972 6f6e   virtual environ
+000002a0: 6d65 6e74 2e20 546f 2064 6f20 736f 2c20  ment. To do so, 
+000002b0: 666f 6c6c 6f77 2074 6865 2062 656c 6f77  follow the below
+000002c0: 2073 696d 706c 6520 7072 6f74 6f63 6f6c   simple protocol
+000002d0: 2074 6f20 6372 6561 7465 2074 6865 2076   to create the v
+000002e0: 6972 7475 616c 2065 6e76 6972 6f6e 6d65  irtual environme
+000002f0: 6e74 2c20 7275 6e20 6974 2c20 616e 6420  nt, run it, and 
+00000300: 696e 7374 616c 6c20 7468 6520 7061 636b  install the pack
+00000310: 6167 6520 7468 6572 653a 0a0a 6060 6072  age there:..```r
+00000320: 7562 7920 0a76 6972 7475 616c 656e 7620  uby .virtualenv 
+00000330: 7665 6e76 0a73 6f75 7263 6520 7665 6e76  venv.source venv
+00000340: 2f62 696e 2f61 6374 6976 6174 650a 7069  /bin/activate.pi
+00000350: 7020 696e 7374 616c 6c20 7465 6e73 6f72  p install tensor
+00000360: 7363 6f75 740a 6060 600a 546f 2065 7869  scout.```.To exi
+00000370: 7420 7468 6520 7669 7274 7561 6c20 656e  t the virtual en
+00000380: 7669 726f 6e6d 656e 742c 2073 696d 706c  vironment, simpl
+00000390: 7920 7479 7065 2060 6465 6163 7469 7661  y type `deactiva
+000003a0: 7465 602e 2054 6f20 6163 6365 7373 2069  te`. To access i
+000003b0: 7420 6174 2061 6e79 206f 7468 6572 2074  t at any other t
+000003c0: 696d 6520 6167 6169 6e2c 2065 6e74 6572  ime again, enter
+000003d0: 2077 6974 6820 7468 6520 6162 6f76 6520   with the above 
+000003e0: 6073 6f75 7263 6520 7665 6e76 2e2e 2e60  `source venv...`
+000003f0: 2063 6f6d 6d61 6e64 2e20 0a               command. .
```

### Comparing `tensorscout-2.0.0/tensorscout/main.py` & `tensorscout-2.1.0/tensorscout/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -35,14 +35,51 @@
             results = pool.map(partial_simulate_data, range(num_cores))
             flattened_results = [item for sublist in results for item in sublist]
             return flattened_results
         return wrapper_monte_carlo
     return decorator_monte_carlo
 
 
+def campfire(num_iters, num_cores):
+    '''
+    Much like a campfire which brings people together and allow for sharing stories and experiences, 
+    this decorator brings together the results of simulations across ``num_cores`` multiple processors and regroups them in a dictionary by key.
+    
+    Parameters
+    ------------
+    num_cores: int
+        Number of processors to use 
+    num_iters : int
+        The number of iterations to perform for a specific model / Monte Carlo simulation. 
+    '''
+    def decorator_monte_carlo(monte_carlo_func):
+        @wraps(monte_carlo_func)
+        def wrapper_monte_carlo(data, *args, **kwargs):
+            def simulate_data(data, num_iters):
+                results = {}
+                for key in data.keys():
+                    results[key] = []
+                    for i in range(num_iters):
+                        simulated_data = monte_carlo_func(data[key], *args, **kwargs)
+                        results[key].append(simulated_data)
+                return results
+            
+            pool = pathosmp.ProcessingPool(num_cores)
+            iterations_per_process = num_iters // num_cores
+            partial_simulate_data = lambda i: simulate_data(data, iterations_per_process)
+            results = pool.map(partial_simulate_data, range(num_cores))
+            regrouped_results = {}
+            for key in results[0].keys():
+                regrouped_results[key] = [item for sublist in [res[key] for res in results] for item in sublist]
+            return regrouped_results
+        return wrapper_monte_carlo
+    return decorator_monte_carlo
+
+
+
 def cakerun(num_cores, L_sectors):
     '''
     This decorator partitions an array into sectors and applies a given function to each sector in parallel. The result of each computation is merged into a final output array.
 
     Parameters
     ------------
     num_cores: int
```

### Comparing `tensorscout-2.0.0/setup.py` & `tensorscout-2.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 000000d0: 342e 3027 2c0a 2027 7363 6970 793e 3d31  4.0',. 'scipy>=1
 000000e0: 2e31 302e 312c 3c32 2e30 2e30 272c 0a20  .10.1,<2.0.0',. 
 000000f0: 2774 696d 6574 6869 733e 3d30 2e31 2e31  'timethis>=0.1.1
 00000100: 2c3c 302e 322e 3027 5d0a 0a73 6574 7570  ,<0.2.0']..setup
 00000110: 5f6b 7761 7267 7320 3d20 7b0a 2020 2020  _kwargs = {.    
 00000120: 276e 616d 6527 3a20 2774 656e 736f 7273  'name': 'tensors
 00000130: 636f 7574 272c 0a20 2020 2027 7665 7273  cout',.    'vers
-00000140: 696f 6e27 3a20 2732 2e30 2e30 272c 0a20  ion': '2.0.0',. 
+00000140: 696f 6e27 3a20 2732 2e31 2e30 272c 0a20  ion': '2.1.0',. 
 00000150: 2020 2027 6465 7363 7269 7074 696f 6e27     'description'
 00000160: 3a20 2741 2050 7974 686f 6e20 6c69 6272  : 'A Python libr
 00000170: 6172 7920 666f 7220 7465 6e73 6f72 206f  ary for tensor o
 00000180: 7065 7261 7469 6f6e 7320 706f 7765 7265  perations powere
 00000190: 6420 6279 2070 6172 616c 6c65 6c20 7072  d by parallel pr
 000001a0: 6f63 6573 7369 6e67 272c 0a20 2020 2027  ocessing',.    '
 000001b0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
@@ -47,65 +47,68 @@
 000002e0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
 000002f0: 6c61 7465 7374 2f3f 6261 6467 653d 6c61  latest/?badge=la
 00000300: 7465 7374 295c 6e5c 6e41 2050 7974 686f  test)\n\nA Pytho
 00000310: 6e20 6c69 6272 6172 7920 666f 7220 7465  n library for te
 00000320: 6e73 6f72 206f 7065 7261 7469 6f6e 7320  nsor operations 
 00000330: 706f 7765 7265 6420 6279 2070 6172 616c  powered by paral
 00000340: 6c65 6c20 7072 6f63 6573 7369 6e67 2e5c  lel processing.\
-00000350: 6e5c 6e3c 696d 6720 7372 633d 2268 7474  n\n<img src="htt
-00000360: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
-00000370: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f61  sercontent.com/a
-00000380: 6e64 7265 7772 6761 7263 6961 2f74 656e  ndrewrgarcia/ten
-00000390: 736f 7273 636f 7574 2f6d 6169 6e2f 6963  sorscout/main/ic
-000003a0: 6f6e 5f73 636f 7574 2e73 7667 2220 7769  on_scout.svg" wi
-000003b0: 6474 683d 2234 3030 223e 5c6e 5c6e 5c6e  dth="400">\n\n\n
-000003c0: 2323 2049 6e73 7461 6c6c 6174 696f 6e5c  ## Installation\
-000003d0: 6e5c 6e60 6060 7275 6279 5c6e 7069 7020  n\n```ruby\npip 
-000003e0: 696e 7374 616c 6c20 7465 6e73 6f72 7363  install tensorsc
-000003f0: 6f75 745c 6e60 6060 5c6e 5c6e 4974 2069  out\n```\n\nIt i
-00000400: 7320 7265 636f 6d6d 656e 6465 6420 796f  s recommended yo
-00000410: 7520 7275 6e20 766f 7865 6c6d 6170 2075  u run voxelmap u
-00000420: 7369 6e67 2061 2060 7669 7274 7561 6c65  sing a `virtuale
-00000430: 6e76 6020 7669 7274 7561 6c20 656e 7669  nv` virtual envi
-00000440: 726f 6e6d 656e 742e 2054 6f20 646f 2073  ronment. To do s
-00000450: 6f2c 2066 6f6c 6c6f 7720 7468 6520 6265  o, follow the be
-00000460: 6c6f 7720 7369 6d70 6c65 2070 726f 746f  low simple proto
-00000470: 636f 6c20 746f 2063 7265 6174 6520 7468  col to create th
-00000480: 6520 7669 7274 7561 6c20 656e 7669 726f  e virtual enviro
-00000490: 6e6d 656e 742c 2072 756e 2069 742c 2061  nment, run it, a
-000004a0: 6e64 2069 6e73 7461 6c6c 2074 6865 2070  nd install the p
-000004b0: 6163 6b61 6765 2074 6865 7265 3a5c 6e5c  ackage there:\n\
-000004c0: 6e60 6060 7275 6279 205c 6e76 6972 7475  n```ruby \nvirtu
-000004d0: 616c 656e 7620 7665 6e76 5c6e 736f 7572  alenv venv\nsour
-000004e0: 6365 2076 656e 762f 6269 6e2f 6163 7469  ce venv/bin/acti
-000004f0: 7661 7465 5c6e 7069 7020 696e 7374 616c  vate\npip instal
-00000500: 6c20 7465 6e73 6f72 7363 6f75 745c 6e60  l tensorscout\n`
-00000510: 6060 5c6e 546f 2065 7869 7420 7468 6520  ``\nTo exit the 
-00000520: 7669 7274 7561 6c20 656e 7669 726f 6e6d  virtual environm
-00000530: 656e 742c 2073 696d 706c 7920 7479 7065  ent, simply type
-00000540: 2060 6465 6163 7469 7661 7465 602e 2054   `deactivate`. T
-00000550: 6f20 6163 6365 7373 2069 7420 6174 2061  o access it at a
-00000560: 6e79 206f 7468 6572 2074 696d 6520 6167  ny other time ag
-00000570: 6169 6e2c 2065 6e74 6572 2077 6974 6820  ain, enter with 
-00000580: 7468 6520 6162 6f76 6520 6073 6f75 7263  the above `sourc
-00000590: 6520 7665 6e76 2e2e 2e60 2063 6f6d 6d61  e venv...` comma
-000005a0: 6e64 2e20 5c6e 272c 0a20 2020 2027 6175  nd. \n',.    'au
-000005b0: 7468 6f72 273a 2027 616e 6472 6577 7267  thor': 'andrewrg
-000005c0: 6172 6369 6127 2c0a 2020 2020 2761 7574  arcia',.    'aut
-000005d0: 686f 725f 656d 6169 6c27 3a20 2767 6172  hor_email': 'gar
-000005e0: 6369 612e 6774 7240 676d 6169 6c2e 636f  cia.gtr@gmail.co
-000005f0: 6d27 2c0a 2020 2020 276d 6169 6e74 6169  m',.    'maintai
-00000600: 6e65 7227 3a20 274e 6f6e 6527 2c0a 2020  ner': 'None',.  
-00000610: 2020 276d 6169 6e74 6169 6e65 725f 656d    'maintainer_em
-00000620: 6169 6c27 3a20 274e 6f6e 6527 2c0a 2020  ail': 'None',.  
-00000630: 2020 2775 726c 273a 2027 4e6f 6e65 272c    'url': 'None',
-00000640: 0a20 2020 2027 7061 636b 6167 6573 273a  .    'packages':
-00000650: 2070 6163 6b61 6765 732c 0a20 2020 2027   packages,.    '
-00000660: 7061 636b 6167 655f 6461 7461 273a 2070  package_data': p
-00000670: 6163 6b61 6765 5f64 6174 612c 0a20 2020  ackage_data,.   
-00000680: 2027 696e 7374 616c 6c5f 7265 7175 6972   'install_requir
-00000690: 6573 273a 2069 6e73 7461 6c6c 5f72 6571  es': install_req
-000006a0: 7569 7265 732c 0a20 2020 2027 7079 7468  uires,.    'pyth
-000006b0: 6f6e 5f72 6571 7569 7265 7327 3a20 273e  on_requires': '>
-000006c0: 3d33 2e38 2c3c 332e 3132 272c 0a7d 0a0a  =3.8,<3.12',.}..
-000006d0: 0a73 6574 7570 282a 2a73 6574 7570 5f6b  .setup(**setup_k
-000006e0: 7761 7267 7329 0a                        wargs).
+00000350: 6e5c 6e3c 6120 6872 6566 3d22 6874 7470  n\n<a href="http
+00000360: 733a 2f2f 7465 6e73 6f72 7363 6f75 742e  s://tensorscout.
+00000370: 7265 6164 7468 6564 6f63 732e 696f 223e  readthedocs.io">
+00000380: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000390: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+000003a0: 636f 6e74 656e 742e 636f 6d2f 616e 6472  content.com/andr
+000003b0: 6577 7267 6172 6369 612f 7465 6e73 6f72  ewrgarcia/tensor
+000003c0: 7363 6f75 742f 6d61 696e 2f69 636f 6e5f  scout/main/icon_
+000003d0: 7363 6f75 742e 706e 6722 2077 6964 7468  scout.png" width
+000003e0: 3d22 3430 3022 3e3c 2f61 3e5c 6e5c 6e5c  ="400"></a>\n\n\
+000003f0: 6e23 2320 496e 7374 616c 6c61 7469 6f6e  n## Installation
+00000400: 5c6e 5c6e 6060 6072 7562 795c 6e70 6970  \n\n```ruby\npip
+00000410: 2069 6e73 7461 6c6c 2074 656e 736f 7273   install tensors
+00000420: 636f 7574 5c6e 6060 605c 6e5c 6e49 7420  cout\n```\n\nIt 
+00000430: 6973 2072 6563 6f6d 6d65 6e64 6564 2079  is recommended y
+00000440: 6f75 2072 756e 2076 6f78 656c 6d61 7020  ou run voxelmap 
+00000450: 7573 696e 6720 6120 6076 6972 7475 616c  using a `virtual
+00000460: 656e 7660 2076 6972 7475 616c 2065 6e76  env` virtual env
+00000470: 6972 6f6e 6d65 6e74 2e20 546f 2064 6f20  ironment. To do 
+00000480: 736f 2c20 666f 6c6c 6f77 2074 6865 2062  so, follow the b
+00000490: 656c 6f77 2073 696d 706c 6520 7072 6f74  elow simple prot
+000004a0: 6f63 6f6c 2074 6f20 6372 6561 7465 2074  ocol to create t
+000004b0: 6865 2076 6972 7475 616c 2065 6e76 6972  he virtual envir
+000004c0: 6f6e 6d65 6e74 2c20 7275 6e20 6974 2c20  onment, run it, 
+000004d0: 616e 6420 696e 7374 616c 6c20 7468 6520  and install the 
+000004e0: 7061 636b 6167 6520 7468 6572 653a 5c6e  package there:\n
+000004f0: 5c6e 6060 6072 7562 7920 5c6e 7669 7274  \n```ruby \nvirt
+00000500: 7561 6c65 6e76 2076 656e 765c 6e73 6f75  ualenv venv\nsou
+00000510: 7263 6520 7665 6e76 2f62 696e 2f61 6374  rce venv/bin/act
+00000520: 6976 6174 655c 6e70 6970 2069 6e73 7461  ivate\npip insta
+00000530: 6c6c 2074 656e 736f 7273 636f 7574 5c6e  ll tensorscout\n
+00000540: 6060 605c 6e54 6f20 6578 6974 2074 6865  ```\nTo exit the
+00000550: 2076 6972 7475 616c 2065 6e76 6972 6f6e   virtual environ
+00000560: 6d65 6e74 2c20 7369 6d70 6c79 2074 7970  ment, simply typ
+00000570: 6520 6064 6561 6374 6976 6174 6560 2e20  e `deactivate`. 
+00000580: 546f 2061 6363 6573 7320 6974 2061 7420  To access it at 
+00000590: 616e 7920 6f74 6865 7220 7469 6d65 2061  any other time a
+000005a0: 6761 696e 2c20 656e 7465 7220 7769 7468  gain, enter with
+000005b0: 2074 6865 2061 626f 7665 2060 736f 7572   the above `sour
+000005c0: 6365 2076 656e 762e 2e2e 6020 636f 6d6d  ce venv...` comm
+000005d0: 616e 642e 205c 6e27 2c0a 2020 2020 2761  and. \n',.    'a
+000005e0: 7574 686f 7227 3a20 2761 6e64 7265 7772  uthor': 'andrewr
+000005f0: 6761 7263 6961 272c 0a20 2020 2027 6175  garcia',.    'au
+00000600: 7468 6f72 5f65 6d61 696c 273a 2027 6761  thor_email': 'ga
+00000610: 7263 6961 2e67 7472 4067 6d61 696c 2e63  rcia.gtr@gmail.c
+00000620: 6f6d 272c 0a20 2020 2027 6d61 696e 7461  om',.    'mainta
+00000630: 696e 6572 273a 2027 4e6f 6e65 272c 0a20  iner': 'None',. 
+00000640: 2020 2027 6d61 696e 7461 696e 6572 5f65     'maintainer_e
+00000650: 6d61 696c 273a 2027 4e6f 6e65 272c 0a20  mail': 'None',. 
+00000660: 2020 2027 7572 6c27 3a20 274e 6f6e 6527     'url': 'None'
+00000670: 2c0a 2020 2020 2770 6163 6b61 6765 7327  ,.    'packages'
+00000680: 3a20 7061 636b 6167 6573 2c0a 2020 2020  : packages,.    
+00000690: 2770 6163 6b61 6765 5f64 6174 6127 3a20  'package_data': 
+000006a0: 7061 636b 6167 655f 6461 7461 2c0a 2020  package_data,.  
+000006b0: 2020 2769 6e73 7461 6c6c 5f72 6571 7569    'install_requi
+000006c0: 7265 7327 3a20 696e 7374 616c 6c5f 7265  res': install_re
+000006d0: 7175 6972 6573 2c0a 2020 2020 2770 7974  quires,.    'pyt
+000006e0: 686f 6e5f 7265 7175 6972 6573 273a 2027  hon_requires': '
+000006f0: 3e3d 332e 382c 3c33 2e31 3227 2c0a 7d0a  >=3.8,<3.12',.}.
+00000700: 0a0a 7365 7475 7028 2a2a 7365 7475 705f  ..setup(**setup_
+00000710: 6b77 6172 6773 290a                      kwargs).
```

### Comparing `tensorscout-2.0.0/PKG-INFO` & `tensorscout-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7465 6e73  : 2.1.Name: tens
 00000020: 6f72 7363 6f75 740a 5665 7273 696f 6e3a  orscout.Version:
-00000030: 2032 2e30 2e30 0a53 756d 6d61 7279 3a20   2.0.0.Summary: 
+00000030: 2032 2e31 2e30 0a53 756d 6d61 7279 3a20   2.1.0.Summary: 
 00000040: 4120 5079 7468 6f6e 206c 6962 7261 7279  A Python library
 00000050: 2066 6f72 2074 656e 736f 7220 6f70 6572   for tensor oper
 00000060: 6174 696f 6e73 2070 6f77 6572 6564 2062  ations powered b
 00000070: 7920 7061 7261 6c6c 656c 2070 726f 6365  y parallel proce
 00000080: 7373 696e 670a 4c69 6365 6e73 653a 204d  ssing.License: M
 00000090: 4954 0a41 7574 686f 723a 2061 6e64 7265  IT.Author: andre
 000000a0: 7772 6761 7263 6961 0a41 7574 686f 722d  wrgarcia.Author-
@@ -67,44 +67,47 @@
 00000420: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
 00000430: 2f6c 6174 6573 742f 3f62 6164 6765 3d6c  /latest/?badge=l
 00000440: 6174 6573 7429 0a0a 4120 5079 7468 6f6e  atest)..A Python
 00000450: 206c 6962 7261 7279 2066 6f72 2074 656e   library for ten
 00000460: 736f 7220 6f70 6572 6174 696f 6e73 2070  sor operations p
 00000470: 6f77 6572 6564 2062 7920 7061 7261 6c6c  owered by parall
 00000480: 656c 2070 726f 6365 7373 696e 672e 0a0a  el processing...
-00000490: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-000004a0: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-000004b0: 636f 6e74 656e 742e 636f 6d2f 616e 6472  content.com/andr
-000004c0: 6577 7267 6172 6369 612f 7465 6e73 6f72  ewrgarcia/tensor
-000004d0: 7363 6f75 742f 6d61 696e 2f69 636f 6e5f  scout/main/icon_
-000004e0: 7363 6f75 742e 7376 6722 2077 6964 7468  scout.svg" width
-000004f0: 3d22 3430 3022 3e0a 0a0a 2323 2049 6e73  ="400">...## Ins
-00000500: 7461 6c6c 6174 696f 6e0a 0a60 6060 7275  tallation..```ru
-00000510: 6279 0a70 6970 2069 6e73 7461 6c6c 2074  by.pip install t
-00000520: 656e 736f 7273 636f 7574 0a60 6060 0a0a  ensorscout.```..
-00000530: 4974 2069 7320 7265 636f 6d6d 656e 6465  It is recommende
-00000540: 6420 796f 7520 7275 6e20 766f 7865 6c6d  d you run voxelm
-00000550: 6170 2075 7369 6e67 2061 2060 7669 7274  ap using a `virt
-00000560: 7561 6c65 6e76 6020 7669 7274 7561 6c20  ualenv` virtual 
-00000570: 656e 7669 726f 6e6d 656e 742e 2054 6f20  environment. To 
-00000580: 646f 2073 6f2c 2066 6f6c 6c6f 7720 7468  do so, follow th
-00000590: 6520 6265 6c6f 7720 7369 6d70 6c65 2070  e below simple p
-000005a0: 726f 746f 636f 6c20 746f 2063 7265 6174  rotocol to creat
-000005b0: 6520 7468 6520 7669 7274 7561 6c20 656e  e the virtual en
-000005c0: 7669 726f 6e6d 656e 742c 2072 756e 2069  vironment, run i
-000005d0: 742c 2061 6e64 2069 6e73 7461 6c6c 2074  t, and install t
-000005e0: 6865 2070 6163 6b61 6765 2074 6865 7265  he package there
-000005f0: 3a0a 0a60 6060 7275 6279 200a 7669 7274  :..```ruby .virt
-00000600: 7561 6c65 6e76 2076 656e 760a 736f 7572  ualenv venv.sour
-00000610: 6365 2076 656e 762f 6269 6e2f 6163 7469  ce venv/bin/acti
-00000620: 7661 7465 0a70 6970 2069 6e73 7461 6c6c  vate.pip install
-00000630: 2074 656e 736f 7273 636f 7574 0a60 6060   tensorscout.```
-00000640: 0a54 6f20 6578 6974 2074 6865 2076 6972  .To exit the vir
-00000650: 7475 616c 2065 6e76 6972 6f6e 6d65 6e74  tual environment
-00000660: 2c20 7369 6d70 6c79 2074 7970 6520 6064  , simply type `d
-00000670: 6561 6374 6976 6174 6560 2e20 546f 2061  eactivate`. To a
-00000680: 6363 6573 7320 6974 2061 7420 616e 7920  ccess it at any 
-00000690: 6f74 6865 7220 7469 6d65 2061 6761 696e  other time again
-000006a0: 2c20 656e 7465 7220 7769 7468 2074 6865  , enter with the
-000006b0: 2061 626f 7665 2060 736f 7572 6365 2076   above `source v
-000006c0: 656e 762e 2e2e 6020 636f 6d6d 616e 642e  env...` command.
-000006d0: 200a 0a                                   ..
+00000490: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000004a0: 2f74 656e 736f 7273 636f 7574 2e72 6561  /tensorscout.rea
+000004b0: 6474 6865 646f 6373 2e69 6f22 3e3c 696d  dthedocs.io"><im
+000004c0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+000004d0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+000004e0: 7465 6e74 2e63 6f6d 2f61 6e64 7265 7772  tent.com/andrewr
+000004f0: 6761 7263 6961 2f74 656e 736f 7273 636f  garcia/tensorsco
+00000500: 7574 2f6d 6169 6e2f 6963 6f6e 5f73 636f  ut/main/icon_sco
+00000510: 7574 2e70 6e67 2220 7769 6474 683d 2234  ut.png" width="4
+00000520: 3030 223e 3c2f 613e 0a0a 0a23 2320 496e  00"></a>...## In
+00000530: 7374 616c 6c61 7469 6f6e 0a0a 6060 6072  stallation..```r
+00000540: 7562 790a 7069 7020 696e 7374 616c 6c20  uby.pip install 
+00000550: 7465 6e73 6f72 7363 6f75 740a 6060 600a  tensorscout.```.
+00000560: 0a49 7420 6973 2072 6563 6f6d 6d65 6e64  .It is recommend
+00000570: 6564 2079 6f75 2072 756e 2076 6f78 656c  ed you run voxel
+00000580: 6d61 7020 7573 696e 6720 6120 6076 6972  map using a `vir
+00000590: 7475 616c 656e 7660 2076 6972 7475 616c  tualenv` virtual
+000005a0: 2065 6e76 6972 6f6e 6d65 6e74 2e20 546f   environment. To
+000005b0: 2064 6f20 736f 2c20 666f 6c6c 6f77 2074   do so, follow t
+000005c0: 6865 2062 656c 6f77 2073 696d 706c 6520  he below simple 
+000005d0: 7072 6f74 6f63 6f6c 2074 6f20 6372 6561  protocol to crea
+000005e0: 7465 2074 6865 2076 6972 7475 616c 2065  te the virtual e
+000005f0: 6e76 6972 6f6e 6d65 6e74 2c20 7275 6e20  nvironment, run 
+00000600: 6974 2c20 616e 6420 696e 7374 616c 6c20  it, and install 
+00000610: 7468 6520 7061 636b 6167 6520 7468 6572  the package ther
+00000620: 653a 0a0a 6060 6072 7562 7920 0a76 6972  e:..```ruby .vir
+00000630: 7475 616c 656e 7620 7665 6e76 0a73 6f75  tualenv venv.sou
+00000640: 7263 6520 7665 6e76 2f62 696e 2f61 6374  rce venv/bin/act
+00000650: 6976 6174 650a 7069 7020 696e 7374 616c  ivate.pip instal
+00000660: 6c20 7465 6e73 6f72 7363 6f75 740a 6060  l tensorscout.``
+00000670: 600a 546f 2065 7869 7420 7468 6520 7669  `.To exit the vi
+00000680: 7274 7561 6c20 656e 7669 726f 6e6d 656e  rtual environmen
+00000690: 742c 2073 696d 706c 7920 7479 7065 2060  t, simply type `
+000006a0: 6465 6163 7469 7661 7465 602e 2054 6f20  deactivate`. To 
+000006b0: 6163 6365 7373 2069 7420 6174 2061 6e79  access it at any
+000006c0: 206f 7468 6572 2074 696d 6520 6167 6169   other time agai
+000006d0: 6e2c 2065 6e74 6572 2077 6974 6820 7468  n, enter with th
+000006e0: 6520 6162 6f76 6520 6073 6f75 7263 6520  e above `source 
+000006f0: 7665 6e76 2e2e 2e60 2063 6f6d 6d61 6e64  venv...` command
+00000700: 2e20 0a0a                                . ..
```

