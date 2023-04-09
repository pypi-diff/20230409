# Comparing `tmp/riscv_isac-0.8.0.tar.gz` & `tmp/riscv_isac-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/riscv_isac-0.8.0.tar", last modified: Mon Nov  1 12:12:07 2021, max compression
+gzip compressed data, was "dist/riscv_isac-0.9.0.tar", last modified: Sat Jan  8 12:40:14 2022, max compression
```

## Comparing `riscv_isac-0.8.0.tar` & `riscv_isac-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 12:12:07.000000 riscv_isac-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1532 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/LICENSE.incore
--rw-r--r--   0 runner    (1001) docker     (121)      140 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      722 2021-11-01 12:12:07.000000 riscv_isac-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      224 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 12:12:07.000000 riscv_isac-0.8.0/riscv_isac/
--rw-r--r--   0 runner    (1001) docker     (121)     3329 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/riscv_isac/InstructionObject.py
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/riscv_isac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17797 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/riscv_isac/cgf_normalize.py
--rw-r--r--   0 runner    (1001) docker     (121)     2058 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/riscv_isac/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    40514 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/riscv_isac/coverage.py
--rw-r--r--   0 runner    (1001) docker     (121)   184341 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/riscv_isac/fp_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2262 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/riscv_isac/isac.py
--rw-r--r--   0 runner    (1001) docker     (121)     3080 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/riscv_isac/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     5918 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/riscv_isac/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 12:12:07.000000 riscv_isac-0.8.0/riscv_isac/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/riscv_isac/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/riscv_isac/plugins/c_sail.py
--rw-r--r--   0 runner    (1001) docker     (121)    56720 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/riscv_isac/plugins/internaldecoder.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/riscv_isac/plugins/specification.py
--rw-r--r--   0 runner    (1001) docker     (121)     2086 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/riscv_isac/plugins/spike.py
--rw-r--r--   0 runner    (1001) docker     (121)       80 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/riscv_isac/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12601 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/riscv_isac/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 12:12:07.000000 riscv_isac-0.8.0/riscv_isac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      722 2021-11-01 12:12:07.000000 riscv_isac-0.8.0/riscv_isac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      759 2021-11-01 12:12:07.000000 riscv_isac-0.8.0/riscv_isac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-01 12:12:07.000000 riscv_isac-0.8.0/riscv_isac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-11-01 12:12:07.000000 riscv_isac-0.8.0/riscv_isac.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-01 12:12:07.000000 riscv_isac-0.8.0/riscv_isac.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       80 2021-11-01 12:12:07.000000 riscv_isac-0.8.0/riscv_isac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-11-01 12:12:07.000000 riscv_isac-0.8.0/riscv_isac.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      393 2021-11-01 12:12:07.000000 riscv_isac-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 12:12:07.000000 riscv_isac-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      449 2021-11-01 12:11:48.000000 riscv_isac-0.8.0/tests/test_riscv_isac.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-08 12:40:14.000000 riscv_isac-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/LICENSE.incore
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      722 2022-01-08 12:40:14.000000 riscv_isac-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-08 12:40:14.000000 riscv_isac-0.9.0/riscv_isac/
+-rw-r--r--   0 runner    (1001) docker     (121)     3473 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/riscv_isac/InstructionObject.py
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/riscv_isac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20373 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/riscv_isac/cgf_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2058 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/riscv_isac/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43710 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/riscv_isac/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (121)   184341 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/riscv_isac/fp_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2262 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/riscv_isac/isac.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3080 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/riscv_isac/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5918 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/riscv_isac/main.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-08 12:40:14.000000 riscv_isac-0.9.0/riscv_isac/plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/riscv_isac/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/riscv_isac/plugins/c_sail.py
+-rw-r--r--   0 runner    (1001) docker     (121)    86750 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/riscv_isac/plugins/internaldecoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/riscv_isac/plugins/specification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2086 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/riscv_isac/plugins/spike.py
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/riscv_isac/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    12601 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/riscv_isac/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-08 12:40:14.000000 riscv_isac-0.9.0/riscv_isac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      722 2022-01-08 12:40:14.000000 riscv_isac-0.9.0/riscv_isac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      759 2022-01-08 12:40:14.000000 riscv_isac-0.9.0/riscv_isac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-08 12:40:14.000000 riscv_isac-0.9.0/riscv_isac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-01-08 12:40:14.000000 riscv_isac-0.9.0/riscv_isac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-08 12:40:14.000000 riscv_isac-0.9.0/riscv_isac.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-01-08 12:40:14.000000 riscv_isac-0.9.0/riscv_isac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-01-08 12:40:14.000000 riscv_isac-0.9.0/riscv_isac.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-01-08 12:40:14.000000 riscv_isac-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-08 12:40:14.000000 riscv_isac-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      449 2022-01-08 12:39:54.000000 riscv_isac-0.9.0/tests/test_riscv_isac.py
```

### Comparing `riscv_isac-0.8.0/LICENSE.incore` & `riscv_isac-0.9.0/LICENSE.incore`

 * *Files identical despite different names*

### Comparing `riscv_isac-0.8.0/PKG-INFO` & `riscv_isac-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: riscv_isac
-Version: 0.8.0
+Version: 0.9.0
 Summary: RISC-V ISAC
 Home-page: https://github.com/riscv/riscv-isac
 Author: InCore Semiconductors Pvt. Ltd.
 Author-email: info@incoresemi.com
 License: BSD-3-Clause
 Description: #####################################
         **RISC-V ISA Coverage** : RISC-V ISAC
```

### Comparing `riscv_isac-0.8.0/riscv_isac/InstructionObject.py` & `riscv_isac-0.9.0/riscv_isac/InstructionObject.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,20 @@
         self.pred = pred
         self.rl = rl
         self.aq = aq
         self.rm = rm
         self.reg_commit = reg_commit
         self.csr_commit = csr_commit
         self.mnemonic = mnemonic
+        self.is_rvp = False
+        self.rs1_nregs = 1
+        self.rs2_nregs = 1
+        self.rs3_nregs = 1
+        self.rd_nregs = 1
+
 
     def __str__(self):
         line = 'instr: '+ str(self.instr)+ ' addr: '+ str(hex(self.instr_addr)) +' instr_name: '+ str(self.instr_name)
         if self.rd:
             line+= ' rd: '+ str(self.rd)
         if self.rs1:
             line+= ' rs1: '+ str(self.rs1)
@@ -88,8 +94,8 @@
             line+= ' rm: '+ str(self.rm)
         if self.reg_commit:
             line+= ' reg_commit: '+ str(self.reg_commit)
         if self.csr_commit:
             line+= ' csr_commit: '+ str(self.csr_commit)
         if self.mnemonic:
             line+= ' mnemonic: '+ str(self.mnemonic)
-        return line
+        return line
```

### Comparing `riscv_isac-0.8.0/riscv_isac/cgf_normalize.py` & `riscv_isac-0.9.0/riscv_isac/cgf_normalize.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,24 +23,89 @@
             val = int(val,16)
         else:
             val = int(val,2)
     if (val & (1 << (bits - 1))) != 0:
         val = val - (1 << bits)
     return val
 
+def simd_val_comb(xlen, bit_width, signed=True):
+    if type(bit_width)==tuple:
+        bit_width1, bit_width2 = bit_width
+    else:
+        bit_width1, bit_width2 = bit_width, bit_width
+
+    fmt = {8: 'b', 16: 'h', 32: 'w', 64: 'd'}
+    sz1 = fmt[bit_width1]
+    sz2 = fmt[bit_width2]
+    var_num = xlen//bit_width1
+    coverpoints = []
+    for i in range(var_num):
+        var1 = f'rs1_{sz1}{i}_val'
+        var2 = f'rs2_{sz2}{i}_val'
+        if (signed):
+            coverpoints += [(f'{var1} > 0 and {var2} > 0','simd_val_comb')]
+            coverpoints += [(f'{var1} > 0 and {var2} < 0','simd_val_comb')]
+            coverpoints += [(f'{var1} < 0 and {var2} < 0','simd_val_comb')]
+            coverpoints += [(f'{var1} < 0 and {var2} > 0','simd_val_comb')]
+            coverpoints += [(f'{var1} == {var2}','simd_val_comb')]
+            coverpoints += [(f'{var1} != {var2}','simd_val_comb')]
+        else:
+            coverpoints += [(f'{var1} == {var2} and {var1} > 0 and {var2} > 0','simd_val_comb')]
+            coverpoints += [(f'{var1} != {var2} and {var1} > 0 and {var2} > 0','simd_val_comb')]
+
+    return coverpoints
+
+def simd_base_val(rs, xlen, _bit_width, signed=True):
+    fmt = {8: 'b', 16: 'h', 32: 'w', 64: 'd'}
+
+    if type(_bit_width)==tuple:
+        if (rs=="rs1"):
+            bit_width, not_used = _bit_width
+        else:
+            not_used, bit_width = _bit_width
+    else:
+        bit_width, not_used = _bit_width, _bit_width
+
+    sz = fmt[bit_width]
+    var_num = xlen//bit_width
+    sign_val = [(-2**(bit_width-1)), -1, 0, 1, int((2**(bit_width-1)-1))]
+    usign_val = [0, 1, 2**bit_width-2, 2**bit_width-1]
+    coverpoints = []
+    for i in range(var_num):
+        var = f'{rs}_{sz}{i}_val'
+        if (signed):
+            for val in sign_val:
+                coverpoints += [(f'{var} == {val}', 'signed_min_max_middle')]
+            coverpoints += walking_ones(var, bit_width, True)
+            coverpoints += walking_zeros(var, bit_width, True)
+            coverpoints += alternate(var, bit_width, True)
+        else:
+            for val in usign_val:
+                coverpoints += [(f'{var} == {val}','unsigned_min_max_middle')]
+            coverpoints += walking_ones(var, bit_width, False)
+            coverpoints += walking_zeros(var, bit_width, False)
+            coverpoints += alternate(var, bit_width, False)
+    return coverpoints
+
+def simd_imm_val(imm, bit_width):
+    usign_val = (2**(bit_width))
+    coverpoints = []
+    for i in range(usign_val):
+        coverpoints += [(f'{imm} == {i}','simd_imm_val')]
+    return coverpoints
+
 def sp_vals(bit_width,signed):
     if signed:
         conv_func = lambda x: twos(x,bit_width)
         sqrt_min = int(-sqrt(2**(bit_width-1)))
         sqrt_max = int(sqrt((2**(bit_width-1)-1)))
     else:
         sqrt_min = 0
         sqrt_max = int(sqrt((2**bit_width)-1))
         conv_func = lambda x: (int(x,16) if '0x' in x else int(x,2)) if isinstance(x,str) else x
-
     dataset = [3, "0x"+"".join(["5"]*int(bit_width/4)), "0x"+"".join(["a"]*int(bit_width/4)), 5, "0x"+"".join(["3"]*int(bit_width/4)), "0x"+"".join(["6"]*int(bit_width/4))]
     dataset = list(map(conv_func,dataset)) + [int(sqrt(abs(conv_func("0x8"+"".join(["0"]*int((bit_width/4)-1)))))*(-1 if signed else 1))] + [sqrt_min,sqrt_max]
     return dataset + [x - 1 if x>0 else 0 for x in dataset] + [x+1 for x in dataset]
 
 def sp_dataset(bit_width,var_lst=["rs1_val","rs2_val"],signed=True):
     coverpoints = []
     datasets = []
@@ -432,14 +497,15 @@
     for labels, cats in cgf.items():
         if labels != 'datasets':
             for label,node in cats.items():
                 if isinstance(node,dict):
                     if 'abstract_comb' in node:
                         temp = node['abstract_comb']
                         del node['abstract_comb']
+
                         for coverpoints, coverage in temp.items():
                             i = 0
                             try:
                                 exp_cp = eval(coverpoints)
                             except Exception as e:
                                 pass
                             else:
```

### Comparing `riscv_isac-0.8.0/riscv_isac/constants.py` & `riscv_isac-0.9.0/riscv_isac/constants.py`

 * *Files identical despite different names*

### Comparing `riscv_isac-0.8.0/riscv_isac/coverage.py` & `riscv_isac-0.9.0/riscv_isac/coverage.py`

 * *Files 5% similar despite different names*

```diff
@@ -281,14 +281,15 @@
 
         if flen == 32:
             self.f_rf = ['00000000']*32
             self.fcsr = 0
         else:
             self.f_rf = ['0000000000000000']*32
             self.fcsr = 0
+        self.vxsat = 0
         self.pc = 0
 
 class statistics:
     '''
     Class for holding statistics used for Data propagation report
     '''
 
@@ -461,14 +462,54 @@
     return gen_report(cgf, detailed)
 
 def twos_complement(val,bits):
     if (val & (1 << (bits - 1))) != 0:
         val = val - (1 << bits)
     return val
 
+def simd_val_unpack(val_comb, op_width, op_name, val, local_dict):
+    '''
+    This function unpacks `val` into its simd elements.
+
+    :param val_comb: val_comb from the cgf dictionary
+    :param op_name: name of the operand (rs1/rs2)
+    :param val: operand value
+    :param local_dict: locals() of the calling context
+
+    '''
+    simd_size = op_width
+    simd_sgn = False
+    for coverpoints in val_comb:
+        if f"{op_name}_b0_val" in coverpoints:
+            simd_size = 8
+        if f"{op_name}_h0_val" in coverpoints:
+            simd_size = 16
+        if f"{op_name}_w0_val" in coverpoints:
+            simd_size = 32
+        if op_name in coverpoints:
+            if any([s in coverpoints for s in ["<", "== -", "== (-"]]):
+                simd_sgn = True
+
+    fmt = {8: 'b', 16: 'h', 32: 'w', 64: 'd'}
+    sz = fmt[simd_size]
+
+    if simd_size > op_width:
+        return
+
+    elm_urange = 1<<simd_size
+    elm_mask = elm_urange-1
+    elm_msb_mask = (1<<(simd_size-1))
+    for i in range(op_width//simd_size):
+        elm_val = (val >> (i*simd_size)) & elm_mask
+        if simd_sgn and (elm_val & elm_msb_mask) != 0:
+            elm_val = elm_val - elm_urange
+        local_dict[f"{op_name}_{sz}{i}_val"]=elm_val
+    if simd_size == op_width:
+        local_dict[f"{op_name}_val"]=elm_val
+
 def compute_per_line(instr, cgf, xlen, addr_pairs,  sig_addrs):
     '''
     This function checks if the current instruction under scrutiny matches a
     particular coverpoint of interest. If so, it updates the coverpoints and
     return the same.
 
     :param instr: an instructionObject of the single instruction currently parsed
@@ -480,14 +521,15 @@
     :type cgf: dict
     :type xlen: int
     :type addr_pairs: (int, int)
     '''
     global arch_state
     global csr_regfile
     global stats
+    global result_count
 
     mnemonic = instr.mnemonic
     commitvalue = instr.reg_commit
 
     # assign default values to operands
     rs1 = 0
     rs2 = 0
@@ -543,32 +585,55 @@
         imm_val = instr.imm
     if instr.shamt is not None:
         imm_val = instr.shamt
 
     # special value conversion based on signed/unsigned operations
     if instr.instr_name in unsgn_rs1:
         rs1_val = struct.unpack(unsgn_sz, bytes.fromhex(arch_state.x_rf[rs1]))[0]
+    elif instr.is_rvp:
+        rs1_val = struct.unpack(unsgn_sz, bytes.fromhex(arch_state.x_rf[rs1]))[0]
+        if instr.rs1_nregs == 2:
+            rs1_hi_val = struct.unpack(unsgn_sz, bytes.fromhex(arch_state.x_rf[rs1+1]))[0]
+            rs1_val = (rs1_hi_val << 32) | rs1_val
     elif rs1_type == 'x':
         rs1_val = struct.unpack(sgn_sz, bytes.fromhex(arch_state.x_rf[rs1]))[0]
         if instr.instr_name in ["fmv.w.x"]:
             rs1_val = '0x' + (arch_state.x_rf[rs1]).lower()
     elif rs1_type == 'f':
         rs1_val = struct.unpack(sgn_sz, bytes.fromhex(arch_state.f_rf[rs1]))[0]
         if instr.instr_name in ["fadd.s","fsub.s","fmul.s","fdiv.s","fsqrt.s","fmadd.s","fmsub.s","fnmadd.s","fnmsub.s","fmax.s","fmin.s","feq.s","flt.s","fle.s","fmv.x.w","fmv.w.x","fcvt.wu.s","fcvt.s.wu","fcvt.w.s","fcvt.s.w","fsgnj.s","fsgnjn.s","fsgnjx.s","fclass.s"]:
             rs1_val = '0x' + (arch_state.f_rf[rs1]).lower()
 
     if instr.instr_name in unsgn_rs2:
         rs2_val = struct.unpack(unsgn_sz, bytes.fromhex(arch_state.x_rf[rs2]))[0]
+    elif instr.is_rvp:
+        rs2_val = struct.unpack(unsgn_sz, bytes.fromhex(arch_state.x_rf[rs2]))[0]
+        if instr.rs2_nregs == 2:
+            rs2_hi_val = struct.unpack(unsgn_sz, bytes.fromhex(arch_state.x_rf[rs2+1]))[0]
+            rs2_val = (rs2_hi_val << 32) | rs2_val
     elif rs2_type == 'x':
         rs2_val = struct.unpack(sgn_sz, bytes.fromhex(arch_state.x_rf[rs2]))[0]
     elif rs2_type == 'f':
         rs2_val = struct.unpack(sgn_sz, bytes.fromhex(arch_state.f_rf[rs2]))[0]
         if instr.instr_name in ["fadd.s","fsub.s","fmul.s","fdiv.s","fmadd.s","fmsub.s","fnmadd.s","fnmsub.s","fmax.s","fmin.s","feq.s","flt.s","fle.s","fsgnj.s","fsgnjn.s","fsgnjx.s"]:
             rs2_val = '0x' + (arch_state.f_rf[rs2]).lower()
 
+    sig_update = False
+    if instr.instr_name in ['sh','sb','sw','sd','c.sw','c.sd','c.swsp','c.sdsp'] and sig_addrs:
+        store_address = rs1_val + imm_val
+        for start, end in sig_addrs:
+            if store_address >= start and store_address <= end:
+                sig_update = True
+                break
+
+    if sig_update: # writing result operands of last non-store instruction to the signature region
+        result_count = result_count - 1
+    else:
+        result_count = instr.rd_nregs
+
     if instr.instr_name in ["fmadd.s","fmsub.s","fnmadd.s","fnmsub.s"]:
         rs3_val = '0x' + (arch_state.f_rf[rs3]).lower()
 
     if instr.instr_name in ['csrrwi']:
         arch_state.fcsr = instr.zimm
 
     if instr.instr_name in ["fadd.s","fsub.s","fmul.s","fdiv.s","fsqrt.s","fmadd.s","fmsub.s","fnmadd.s","fnmsub.s","fmax.s","fmin.s","feq.s","flt.s","fle.s","fmv.x.w","fmv.w.x","fcvt.wu.s","fcvt.s.wu","fcvt.w.s","fcvt.s.w","fsgnj.s","fsgnjn.s","fsgnjx.s","fclass.s"]:
@@ -700,16 +765,23 @@
                                     val_key = l
                                     if(val_key[0] in cgf[cov_labels]['val_comb']):
                                         if cgf[cov_labels]['val_comb'][val_key[0]] == 0:
                                             stats.ucovpt.append(str(val_key[0]))
                                         stats.covpt.append(str(val_key[0]))
                                         cgf[cov_labels]['val_comb'][val_key[0]] += 1
                             else:
+                                lcls=locals().copy()
+                                if instr.is_rvp and "rs1" in value:
+                                    op_width = 64 if instr.rs1_nregs == 2 else xlen
+                                    simd_val_unpack(value['val_comb'], op_width, "rs1", rs1_val, lcls)
+                                if instr.is_rvp and "rs2" in value:
+                                    op_width = 64 if instr.rs2_nregs == 2 else xlen
+                                    simd_val_unpack(value['val_comb'], op_width, "rs2", rs2_val, lcls)
                                 for coverpoints in value['val_comb']:
-                                    if eval(coverpoints):
+                                    if eval(coverpoints, globals(), lcls):
                                         if cgf[cov_labels]['val_comb'][coverpoints] == 0:
                                             stats.ucovpt.append(str(coverpoints))
                                         stats.covpt.append(str(coverpoints))
                                         cgf[cov_labels]['val_comb'][coverpoints] += 1
                         if 'abstract_comb' in value \
                                 and len(value['abstract_comb']) != 0 :
                             for coverpoints in value['abstract_comb']:
@@ -749,43 +821,45 @@
         store_address = rs1_val + imm_val
         store_val = '0x'+arch_state.x_rf[rs2]
         for start, end in sig_addrs:
             if store_address >= start and store_address <= end:
                 logger.debug('Signature update : ' + str(hex(store_address)))
                 stats.stat5.append((store_address, store_val, stats.ucovpt, stats.code_seq))
                 stats.cov_pt_sig += stats.covpt
-                if stats.ucovpt:
-                    stats.stat1.append((store_address, store_val, stats.ucovpt, stats.ucode_seq))
-                    stats.last_meta = [store_address, store_val, stats.ucovpt, stats.ucode_seq]
-                    stats.ucovpt = []
-                elif stats.covpt:
-                    _log = 'Op without unique coverpoint updates Signature\n'
-                    _log += ' -- Code Sequence:\n'
-                    for op in stats.code_seq:
-                        _log += '      ' + op + '\n'
-                    _log += ' -- Signature Address: {0} Data: {1}\n'.format(
-                            str(hex(store_address)), store_val)
-                    _log += ' -- Redundant Coverpoints hit by the op\n'
-                    for c in stats.covpt:
-                        _log += '      - ' + str(c) + '\n'
-                    logger.warn(_log)
-                    stats.stat2.append(_log + '\n\n')
-                    stats.last_meta = [store_address, store_val, stats.covpt, stats.code_seq]
-                else:
-                    _log = 'Last Coverpoint : ' + str(stats.last_meta[2]) + '\n'
-                    _log += 'Last Code Sequence : \n\t-' + '\n\t-'.join(stats.last_meta[3]) + '\n'
-                    _log +='Current Store : [{0}] : {1} -- Store: [{2}]:{3}\n'.format(\
-                        str(hex(instr.instr_addr)), mnemonic,
-                        str(hex(store_address)),
-                        store_val)
-                    logger.error(_log)
-                    stats.stat4.append(_log + '\n\n')
-                stats.covpt = []
-                stats.code_seq = []
-                stats.ucode_seq = []
+                if result_count <= 0:
+                    if stats.ucovpt:
+                        stats.stat1.append((store_address, store_val, stats.ucovpt, stats.ucode_seq))
+                        stats.last_meta = [store_address, store_val, stats.ucovpt, stats.ucode_seq]
+                        stats.ucovpt = []
+                    elif stats.covpt:
+                        _log = 'Op without unique coverpoint updates Signature\n'
+                        _log += ' -- Code Sequence:\n'
+                        for op in stats.code_seq:
+                            _log += '      ' + op + '\n'
+                        _log += ' -- Signature Address: {0} Data: {1}\n'.format(
+                                str(hex(store_address)), store_val)
+                        _log += ' -- Redundant Coverpoints hit by the op\n'
+                        for c in stats.covpt:
+                            _log += '      - ' + str(c) + '\n'
+                        logger.warn(_log)
+                        stats.stat2.append(_log + '\n\n')
+                        stats.last_meta = [store_address, store_val, stats.covpt, stats.code_seq]
+                    else:
+                        _log = 'Last Coverpoint : ' + str(stats.last_meta[2]) + '\n'
+                        _log += 'Last Code Sequence : \n\t-' + '\n\t-'.join(stats.last_meta[3]) + '\n'
+                        _log +='Current Store : [{0}] : {1} -- Store: [{2}]:{3}\n'.format(\
+                            str(hex(instr.instr_addr)), mnemonic,
+                            str(hex(store_address)),
+                            store_val)
+                        logger.error(_log)
+                        stats.stat4.append(_log + '\n\n')
+
+                    stats.covpt = []
+                    stats.code_seq = []
+                    stats.ucode_seq = []
 
 
 
     if commitvalue is not None:
         if rd_type == 'x':
             arch_state.x_rf[int(commitvalue[1])] =  str(commitvalue[2][2:])
         elif rd_type == 'f':
@@ -804,14 +878,15 @@
         , dump, cov_labels, sig_addrs, window_size):
     '''Compute the Coverage'''
 
     global arch_state
     global csr_regfile
     global stats
     global cross_cover_queue
+    global result_count
 
     temp = cgf.copy()
     if cov_labels:
         for groups in cgf:
             if groups not in cov_labels:
                 del temp[groups]
         cgf = temp
@@ -822,14 +897,15 @@
         dump_f.close()
         sys.exit(0)
 
     arch_state = archState(xlen,32)
     csr_regfile = csr_registers(xlen)
     stats = statistics(xlen, 32)
     cross_cover_queue = []
+    result_count = 0
 
     ## Get coverpoints from cgf
     obj_dict = {} ## (label,coverpoint): object
     for cov_labels,value in cgf.items():
         if cov_labels != 'datasets':
             if 'cross_comb' in value and len(value['cross_comb'])!=0:
                 for coverpt in value['cross_comb'].keys():
```

### Comparing `riscv_isac-0.8.0/riscv_isac/fp_dataset.py` & `riscv_isac-0.9.0/riscv_isac/fp_dataset.py`

 * *Files identical despite different names*

### Comparing `riscv_isac-0.8.0/riscv_isac/isac.py` & `riscv_isac-0.9.0/riscv_isac/isac.py`

 * *Files identical despite different names*

### Comparing `riscv_isac-0.8.0/riscv_isac/log.py` & `riscv_isac-0.9.0/riscv_isac/log.py`

 * *Files identical despite different names*

### Comparing `riscv_isac-0.8.0/riscv_isac/main.py` & `riscv_isac-0.9.0/riscv_isac/main.py`

 * *Files identical despite different names*

### Comparing `riscv_isac-0.8.0/riscv_isac/plugins/c_sail.py` & `riscv_isac-0.9.0/riscv_isac/plugins/c_sail.py`

 * *Files identical despite different names*

### Comparing `riscv_isac-0.8.0/riscv_isac/plugins/spike.py` & `riscv_isac-0.9.0/riscv_isac/plugins/spike.py`

 * *Files identical despite different names*

### Comparing `riscv_isac-0.8.0/riscv_isac/utils.py` & `riscv_isac-0.9.0/riscv_isac/utils.py`

 * *Files identical despite different names*

### Comparing `riscv_isac-0.8.0/riscv_isac.egg-info/PKG-INFO` & `riscv_isac-0.9.0/riscv_isac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: riscv-isac
-Version: 0.8.0
+Version: 0.9.0
 Summary: RISC-V ISAC
 Home-page: https://github.com/riscv/riscv-isac
 Author: InCore Semiconductors Pvt. Ltd.
 Author-email: info@incoresemi.com
 License: BSD-3-Clause
 Description: #####################################
         **RISC-V ISA Coverage** : RISC-V ISAC
```

### Comparing `riscv_isac-0.8.0/riscv_isac.egg-info/SOURCES.txt` & `riscv_isac-0.9.0/riscv_isac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `riscv_isac-0.8.0/setup.py` & `riscv_isac-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 setup_requirements = [ ]
 
 test_requirements = [ ]
 
 setup(
     name='riscv_isac',
-    version='0.8.0',
+    version='0.9.0',
     description="RISC-V ISAC",
     long_description=readme + '\n\n',
     classifiers=[
           "Programming Language :: Python :: 3.6",
           "License :: OSI Approved :: BSD License",
           "Development Status :: 4 - Beta"
     ],
```

