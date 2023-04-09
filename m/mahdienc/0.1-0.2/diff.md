# Comparing `tmp/mahdienc-0.1.tar.gz` & `tmp/mahdienc-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mahdienc-0.1.tar", last modified: Sun Apr  9 13:54:11 2023, max compression
+gzip compressed data, was "mahdienc-0.2.tar", last modified: Sun Apr  9 14:01:44 2023, max compression
```

## Comparing `mahdienc-0.1.tar` & `mahdienc-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:54:11.934498 mahdienc-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-09 13:54:11.934498 mahdienc-0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:54:11.934498 mahdienc-0.1/mahdienc/
--rw-r--r--   0 runner    (1001) docker     (123)    16936 2023-04-09 13:53:58.000000 mahdienc-0.1/mahdienc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:54:11.934498 mahdienc-0.1/mahdienc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-09 13:54:11.000000 mahdienc-0.1/mahdienc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-09 13:54:11.000000 mahdienc-0.1/mahdienc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 13:54:11.000000 mahdienc-0.1/mahdienc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 13:54:11.000000 mahdienc-0.1/mahdienc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 13:54:11.934498 mahdienc-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-09 13:53:58.000000 mahdienc-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:01:44.058586 mahdienc-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-09 14:01:44.058586 mahdienc-0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:01:44.058586 mahdienc-0.2/mahdienc/
+-rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-04-09 14:01:34.000000 mahdienc-0.2/mahdienc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:01:44.058586 mahdienc-0.2/mahdienc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-09 14:01:44.000000 mahdienc-0.2/mahdienc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-09 14:01:44.000000 mahdienc-0.2/mahdienc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:01:44.000000 mahdienc-0.2/mahdienc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 14:01:44.000000 mahdienc-0.2/mahdienc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 14:01:44.058586 mahdienc-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-09 14:01:34.000000 mahdienc-0.2/setup.py
```

### Comparing `mahdienc-0.1/mahdienc/__init__.py` & `mahdienc-0.2/mahdienc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -957,35 +957,35 @@
 00003bc0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
 00003bd0: 2020 2020 2065 7869 7428 2720 5375 6363       exit(' Succ
 00003be0: 6573 7366 756c 2065 7869 7420 2729 0d0a  essful exit ')..
 00003bf0: 0d0a 0d0a 6465 6620 656e 2829 3a0d 0a20  ....def en():.. 
 00003c00: 2020 206f 732e 7379 7374 656d 2822 636c     os.system("cl
 00003c10: 6561 7222 290d 0a20 2020 206c 6f67 6f28  ear")..    logo(
 00003c20: 290d 0a0d 0a0d 0a0d 0a0d 0a0d 0a64 6566  )............def
-00003c30: 2073 6572 7665 7228 293a 0d0a 2020 2020   server():..    
-00003c40: 2365 203d 2062 6173 6536 342e 6236 3464  #e = base64.b64d
-00003c50: 6563 6f64 6528 2761 4852 3063 484d 364c  ecode('aHR0cHM6L
-00003c60: 7939 7959 5863 755a 326c 3061 4856 6964  y9yYXcuZ2l0aHVid
-00003c70: 584e 6c63 6d4e 7662 6e52 6c62 6e51 7559  XNlcmNvbnRlbnQuY
-00003c80: 3239 744c 314e 6f64 585a 764c 554a 4353  29tL1NodXZvLUJCS
-00003c90: 4567 7659 3235 304c 3231 6861 5734 7662  EgvY250L21haW4vb
-00003ca0: 5756 3463 3256 7964 6935 3065 4851 3d27  WV4c2Vydi50eHQ='
-00003cb0: 2e65 6e63 6f64 6528 2275 7466 2d38 2229  .encode("utf-8")
-00003cc0: 290d 0a20 2020 2063 6b63 7276 203d 2027  )..    ckcrv = '
-00003cd0: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-00003ce0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00003cf0: 6d2f 5368 7576 6f2d 4242 4848 2f63 6e74  m/Shuvo-BBHH/cnt
-00003d00: 2f6d 6169 6e2f 656e 632e 7478 7427 0d0a  /main/enc.txt'..
-00003d10: 2020 2020 7072 696e 7428 6627 7b57 4849      print(f'{WHI
-00003d20: 5445 7d43 6861 6b69 6e67 2074 6f20 7365  TE}Chaking to se
-00003d30: 7276 6572 2729 0d0a 2020 2020 7220 3d20  rver')..    r = 
-00003d40: 7265 7175 6573 7473 2e67 6574 2863 6b63  requests.get(ckc
-00003d50: 7276 292e 7465 7874 0d0a 2020 2020 6966  rv).text..    if
-00003d60: 2027 5550 2720 696e 2072 3a0d 0a20 2020   'UP' in r:..   
-00003d70: 2020 2020 2062 616e 6e65 7228 290d 0a20       banner().. 
+00003c30: 206d 6168 6469 656e 6328 293a 0d0a 2020   mahdienc():..  
+00003c40: 2020 2365 203d 2062 6173 6536 342e 6236    #e = base64.b6
+00003c50: 3464 6563 6f64 6528 2761 4852 3063 484d  4decode('aHR0cHM
+00003c60: 364c 7939 7959 5863 755a 326c 3061 4856  6Ly9yYXcuZ2l0aHV
+00003c70: 6964 584e 6c63 6d4e 7662 6e52 6c62 6e51  idXNlcmNvbnRlbnQ
+00003c80: 7559 3239 744c 314e 6f64 585a 764c 554a  uY29tL1NodXZvLUJ
+00003c90: 4353 4567 7659 3235 304c 3231 6861 5734  CSEgvY250L21haW4
+00003ca0: 7662 5756 3463 3256 7964 6935 3065 4851  vbWV4c2Vydi50eHQ
+00003cb0: 3d27 2e65 6e63 6f64 6528 2275 7466 2d38  ='.encode("utf-8
+00003cc0: 2229 290d 0a20 2020 2063 6b63 7276 203d  "))..    ckcrv =
+00003cd0: 2027 6874 7470 733a 2f2f 7261 772e 6769   'https://raw.gi
+00003ce0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00003cf0: 636f 6d2f 5368 7576 6f2d 4242 4848 2f63  com/Shuvo-BBHH/c
+00003d00: 6e74 2f6d 6169 6e2f 656e 632e 7478 7427  nt/main/enc.txt'
+00003d10: 0d0a 2020 2020 7072 696e 7428 6627 7b57  ..    print(f'{W
+00003d20: 4849 5445 7d43 6861 6b69 6e67 2074 6f20  HITE}Chaking to 
+00003d30: 7365 7276 6572 2729 0d0a 2020 2020 7220  server')..    r 
+00003d40: 3d20 7265 7175 6573 7473 2e67 6574 2863  = requests.get(c
+00003d50: 6b63 7276 292e 7465 7874 0d0a 2020 2020  kcrv).text..    
+00003d60: 6966 2027 5550 2720 696e 2072 3a0d 0a20  if 'UP' in r:.. 
+00003d70: 2020 2020 2020 206c 6f67 6f28 290d 0a20         logo().. 
 00003d80: 2020 2020 2020 206f 732e 7379 7374 656d         os.system
 00003d90: 2827 7069 7020 756e 696e 7374 616c 6c20  ('pip uninstall 
 00003da0: 6d61 6864 6965 6e63 2729 0d0a 2020 2020  mahdienc')..    
 00003db0: 2020 2020 7072 696e 7428 6622 7b57 4849      print(f"{WHI
 00003dc0: 5445 7d50 4c5a 2055 7064 6174 6520 436f  TE}PLZ Update Co
 00003dd0: 6d6d 616e 6420 2229 0d0a 2020 2020 2020  mmand ")..      
 00003de0: 2020 7072 696e 7428 6622 7b47 5245 454e    print(f"{GREEN
@@ -1008,18 +1008,18 @@
 00003ef0: 0a20 2020 2020 2020 206f 732e 7379 7374  .        os.syst
 00003f00: 656d 2827 7069 7020 756e 696e 7374 616c  em('pip uninstal
 00003f10: 6c20 6d61 6864 6965 6e63 2729 0d0a 2020  l mahdienc')..  
 00003f20: 2020 2020 2020 696e 7075 7428 290d 0a20        input().. 
 00003f30: 2020 2020 2020 206f 732e 7379 7374 656d         os.system
 00003f40: 2827 7069 7020 756e 696e 7374 616c 6c20  ('pip uninstall 
 00003f50: 6d61 6864 6965 6e63 2729 0d0a 2020 2020  mahdienc')..    
-00003f60: 2020 2020 7365 7276 6572 2829 0d0a 0d0a      server()....
-00003f70: 2020 2020 6966 2027 4f46 2720 696e 2072      if 'OF' in r
-00003f80: 3a0d 0a20 2020 2020 2020 2062 616e 6e65  :..        banne
-00003f90: 7228 290d 0a20 2020 2020 2020 206f 732e  r()..        os.
+00003f60: 2020 2020 6d61 6864 6965 6e63 2829 0d0a      mahdienc()..
+00003f70: 0d0a 2020 2020 6966 2027 4f46 2720 696e  ..    if 'OF' in
+00003f80: 2072 3a0d 0a20 2020 2020 2020 206c 6f67   r:..        log
+00003f90: 6f28 290d 0a20 2020 2020 2020 206f 732e  o()..        os.
 00003fa0: 7379 7374 656d 2827 7069 7020 756e 696e  system('pip unin
 00003fb0: 7374 616c 6c20 6d61 6864 6965 6e63 2729  stall mahdienc')
 00003fc0: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
 00003fd0: 6622 7b57 4849 5445 7d54 4f4f 4c53 204f  f"{WHITE}TOOLS O
 00003fe0: 4646 2229 0d0a 2020 2020 2020 2020 7072  FF")..        pr
 00003ff0: 696e 7428 6622 7b47 5245 454e 7d54 4f4f  int(f"{GREEN}TOO
 00004000: 4c53 204f 4646 2229 0d0a 2020 2020 2020  LS OFF")..      
@@ -1044,16 +1044,16 @@
 00004130: 6365 626f 6f6b 2e63 6f6d 2f6d 6134 4431  cebook.com/ma4D1
 00004140: 2229 0d0a 2020 2020 2020 2020 6f73 2e73  ")..        os.s
 00004150: 7973 7465 6d28 2278 6467 2d6f 7065 6e20  ystem("xdg-open 
 00004160: 6874 7470 733a 2f2f 6661 6365 626f 6f6b  https://facebook
 00004170: 2e63 6f6d 2f67 726f 7570 732f 3631 3034  .com/groups/6104
 00004180: 3837 3535 3931 3239 3038 3622 290d 0a20  87559129086").. 
 00004190: 2020 2020 2020 2069 6e70 7574 2829 0d0a         input()..
-000041a0: 2020 2020 2020 2020 7365 7276 6572 2829          server()
-000041b0: 0d0a 0d0a 0d0a 2020 2020 6966 2027 4f4e  ......    if 'ON
-000041c0: 2720 696e 2072 3a0d 0a20 2020 2020 2020  ' in r:..       
-000041d0: 204d 6169 6e4d 656e 7528 290d 0a20 2020   MainMenu()..   
-000041e0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-000041f0: 6578 6974 2829 0d0a 0d0a 6966 205f 5f6e  exit()....if __n
-00004200: 616d 655f 5f20 3d3d 2022 5f5f 6d61 696e  ame__ == "__main
-00004210: 5f5f 223a 0d0a 2020 2020 7365 7276 6572  __":..    server
-00004220: 2829 0d0a 0d0a 0d0a                      ()......
+000041a0: 2020 2020 2020 2020 6d61 6864 6965 6e63          mahdienc
+000041b0: 2829 0d0a 0d0a 0d0a 2020 2020 6966 2027  ()......    if '
+000041c0: 4f4e 2720 696e 2072 3a0d 0a20 2020 2020  ON' in r:..     
+000041d0: 2020 204d 6169 6e4d 656e 7528 290d 0a20     MainMenu().. 
+000041e0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+000041f0: 2020 6578 6974 2829 0d0a 0d0a 6966 205f    exit()....if _
+00004200: 5f6e 616d 655f 5f20 3d3d 2022 5f5f 6d61  _name__ == "__ma
+00004210: 696e 5f5f 223a 0d0a 2020 2020 6d61 6864  in__":..    mahd
+00004220: 6965 6e63 2829 0d0a 0d0a 0d0a            ienc()......
```

