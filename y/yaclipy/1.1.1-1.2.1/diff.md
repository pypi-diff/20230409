# Comparing `tmp/yaclipy-1.1.1.tar.gz` & `tmp/yaclipy-1.2.1.tar.gz`

## Comparing `yaclipy-1.1.1.tar` & `yaclipy-1.2.1.tar`

### file list

```diff
@@ -1,40 +1,38 @@
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 yaclipy-1.1.1/pytest.ini
--rwxr-xr-x   0        0        0      530 2020-02-02 00:00:00.000000 yaclipy-1.1.1/examples/readme.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 yaclipy-1.1.1/examples/simple/cmd1 -> files.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 yaclipy-1.1.1/examples/simple/cmd2 -> files.py
--rwxr-xr-x   0        0        0      657 2020-02-02 00:00:00.000000 yaclipy-1.1.1/examples/simple/files.py
--rwxr-xr-x   0        0        0      788 2020-02-02 00:00:00.000000 yaclipy-1.1.1/examples/simple/sub.py
--rwxr-xr-x   0        0        0     1371 2020-02-02 00:00:00.000000 yaclipy-1.1.1/examples/venv/cli.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 yaclipy-1.1.1/examples/venv/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaclipy-1.1.1/examples/venv/local/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 yaclipy-1.1.1/examples/venv/local/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaclipy-1.1.1/examples/venv/pyutil/__init__.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 yaclipy-1.1.1/examples/venv/pyutil/main.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 yaclipy-1.1.1/examples/venv/pyutil/requirements.txt
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 yaclipy-1.1.1/src/yaclipy/__about__.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 yaclipy-1.1.1/src/yaclipy/__init__.py
--rw-r--r--   0        0        0    14340 2020-02-02 00:00:00.000000 yaclipy-1.1.1/src/yaclipy/arg_spec.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 yaclipy-1.1.1/src/yaclipy/bootstrap.py
--rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 yaclipy-1.1.1/src/yaclipy/command.py
--rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 yaclipy-1.1.1/src/yaclipy/config.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 yaclipy-1.1.1/src/yaclipy/docs.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 yaclipy-1.1.1/src/yaclipy/exceptions.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 yaclipy-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 yaclipy-1.1.1/tests/arg_spec_test.py
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 yaclipy-1.1.1/tests/arg_type_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaclipy-1.1.1/tests/bind_sub_test.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 yaclipy-1.1.1/tests/bind_test.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 yaclipy-1.1.1/tests/boot_test.py
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 yaclipy-1.1.1/tests/call_test.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 yaclipy-1.1.1/tests/cmd_dfn_test.py
--rw-r--r--   0        0        0     6564 2020-02-02 00:00:00.000000 yaclipy-1.1.1/tests/config_test.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 yaclipy-1.1.1/tests/docs_test.py
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 yaclipy-1.1.1/tests/readme_test.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 yaclipy-1.1.1/tests/testutil.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaclipy-1.1.1/tests/notest/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 yaclipy-1.1.1/tests/notest/config_import_error.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 yaclipy-1.1.1/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 yaclipy-1.1.1/LICENSE.txt
--rw-r--r--   0        0        0    14876 2020-02-02 00:00:00.000000 yaclipy-1.1.1/README.rst
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 yaclipy-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    15951 2020-02-02 00:00:00.000000 yaclipy-1.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0      530 2020-02-02 00:00:00.000000 yaclipy-1.2.1/examples/readme.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 yaclipy-1.2.1/examples/simple/cmd1 -> files.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 yaclipy-1.2.1/examples/simple/cmd2 -> files.py
+-rwxr-xr-x   0        0        0      657 2020-02-02 00:00:00.000000 yaclipy-1.2.1/examples/simple/files.py
+-rwxr-xr-x   0        0        0      788 2020-02-02 00:00:00.000000 yaclipy-1.2.1/examples/simple/sub.py
+-rwxr-xr-x   0        0        0     1371 2020-02-02 00:00:00.000000 yaclipy-1.2.1/examples/venv/cli.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 yaclipy-1.2.1/examples/venv/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaclipy-1.2.1/examples/venv/local/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 yaclipy-1.2.1/examples/venv/local/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaclipy-1.2.1/examples/venv/pyutil/__init__.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 yaclipy-1.2.1/examples/venv/pyutil/main.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 yaclipy-1.2.1/examples/venv/pyutil/requirements.txt
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 yaclipy-1.2.1/src/yaclipy/__about__.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 yaclipy-1.2.1/src/yaclipy/__init__.py
+-rw-r--r--   0        0        0    14656 2020-02-02 00:00:00.000000 yaclipy-1.2.1/src/yaclipy/arg_spec.py
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 yaclipy-1.2.1/src/yaclipy/command.py
+-rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 yaclipy-1.2.1/src/yaclipy/config.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 yaclipy-1.2.1/src/yaclipy/docs.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 yaclipy-1.2.1/src/yaclipy/exceptions.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 yaclipy-1.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 yaclipy-1.2.1/tests/arg_spec_test.py
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 yaclipy-1.2.1/tests/arg_type_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaclipy-1.2.1/tests/bind_sub_test.py
+-rw-r--r--   0        0        0     5149 2020-02-02 00:00:00.000000 yaclipy-1.2.1/tests/bind_test.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 yaclipy-1.2.1/tests/boot_test.py
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 yaclipy-1.2.1/tests/call_test.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 yaclipy-1.2.1/tests/cmd_dfn_test.py
+-rw-r--r--   0        0        0     6564 2020-02-02 00:00:00.000000 yaclipy-1.2.1/tests/config_test.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 yaclipy-1.2.1/tests/docs_test.py
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 yaclipy-1.2.1/tests/readme_test.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 yaclipy-1.2.1/tests/testutil.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaclipy-1.2.1/tests/notest/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 yaclipy-1.2.1/tests/notest/config_import_error.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 yaclipy-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 yaclipy-1.2.1/LICENSE.txt
+-rw-r--r--   0        0        0    14876 2020-02-02 00:00:00.000000 yaclipy-1.2.1/README.rst
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 yaclipy-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    16254 2020-02-02 00:00:00.000000 yaclipy-1.2.1/PKG-INFO
```

### Comparing `yaclipy-1.1.1/examples/readme.py` & `yaclipy-1.2.1/examples/readme.py`

 * *Files identical despite different names*

### Comparing `yaclipy-1.1.1/examples/simple/files.py` & `yaclipy-1.2.1/examples/simple/files.py`

 * *Files identical despite different names*

### Comparing `yaclipy-1.1.1/examples/simple/sub.py` & `yaclipy-1.2.1/examples/simple/sub.py`

 * *Files identical despite different names*

### Comparing `yaclipy-1.1.1/examples/venv/cli.py` & `yaclipy-1.2.1/examples/venv/cli.py`

 * *Files identical despite different names*

### Comparing `yaclipy-1.1.1/examples/venv/pyutil/main.py` & `yaclipy-1.2.1/examples/venv/pyutil/main.py`

 * *Files identical despite different names*

### Comparing `yaclipy-1.1.1/src/yaclipy/arg_spec.py` & `yaclipy-1.2.1/src/yaclipy/arg_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 import inspect, os, copy, json, re
 from inspect import Parameter
 from print_ext import Table, pretty, Line
 from print_ext.widget import INFINITY
 from .exceptions import UsageError
 
+def coerce_int(v):
+    if isinstance(v, str):
+        if v.lower().startswith('0x'): return int(v, 16)
+        if v.lower().startswith('0b'): return int(v, 2)
+        if len(v)>1 and v.startswith('0') and v[1] in '123456789': return int(v, 8)
+    return int(v)
+
 
 def sig_kinds(fn):
     kinds = set()
     for k in ['module', 'function', 'generatorfunction', 'generator', 'coroutinefunction', 'asyncgenfunction', 'asyncgen', 'coroutine', 'awaitable', 'class' , 'method',  'traceback', 'frame', 'code', 'builtin', 'methodwrapper', 'routine', 'abstract', 'methoddescriptor', 'datadescriptor', 'getsetdescriptor', 'memberdescriptor']:
         try:
             if getattr(inspect, 'is'+k)(fn): kinds.add(k)
         except:
@@ -41,14 +48,15 @@
         self.repeated = False
         if isinstance(val, list):
             self.repeated = True
             val = val[0] if val else ''
         if not callable(val):
             val = type(val)
         self.coerce = str if val==type(None) or val==Parameter.empty else val
+        if self.coerce == int: self.coerce = coerce_int
         self.is_flag = self.coerce == bool
         if self.coerce == dict: self.coerce = json.loads
         if self.repeated and self.is_flag: raise ValueError("We can't handle repeated bool arguments")
 
 
     def __repr__(self):
         return f'[{self.coerce.__name__}]' if self.repeated else self.coerce.__name__
@@ -92,15 +100,15 @@
 
     
     def set(self, val, index):
         try:
             self['value'] = self.type.merge(val, self.value)
         except ValueError as e:
             if isinstance(index, int):
-                self.spec.error('TYPE_MISMATCH', f"Type mismatch on \b1 {ordinal(index)}\b  parameter.  {e}")
+                self.spec.error('TYPE_MISMATCH', f"Type mismatch on \b1 {self.ordinal}\b  parameter.  {e}")
             else:
                 self.spec.error('TYPE_MISMATCH', f"Parameter '\b1 {index}\b ' type mismatch.  {e}")
 
 
     @property
     def ordinal(self):
         n = self.index
```

### Comparing `yaclipy-1.1.1/src/yaclipy/command.py` & `yaclipy-1.2.1/src/yaclipy/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,16 +116,20 @@
         return await self.next_cmd._run(val)
 
 
     def run(self, input=None):
         try:
             loop = asyncio.get_running_loop()
         except RuntimeError:
+            loop = None
+        if loop:
+            return loop.create_task(self._run(input), name=self.name)
+        else:
             return asyncio.run(self._run(input))
-        task = loop.create_task(self._run(input), name=self.name)
+        
 
 
     def doc(self, check=False):
         if not hasattr(self, '_doc'):
             self._doc = CmdDoc(inspect.getdoc(self.fn) or '')
         return self._doc
```

### Comparing `yaclipy-1.1.1/src/yaclipy/config.py` & `yaclipy-1.2.1/src/yaclipy/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,19 +100,19 @@
         self.name = ''
         self.set_name(name or fn.__name__)
 
 
     def set_name(self, name):
         self.hide()
         self.name = name.replace('_','-')
-        get_config().set_configuration(self)
+        get_config().add_configure(self)
 
 
     def hide(self):
-        get_config().set_configuration(self, unset=True)
+        get_config().add_configure(self, unset=True)
 
 
     def __hash__(self):
         return hash(self.name.lower())
 
 
     def __eq__(self, other):
@@ -130,17 +130,17 @@
     def __lt__(self, other):
         return self.name.lower() < str(other).lower()
 
 
 
 class Config():
 
-    def __init__(self, name='', *, parent=None):
+    def __init__(self, *, parent=None):
         self.parent = parent
-        self.name = name
+        self.name = ''
         self.vars = set(parent.vars) if parent else set()
         self.configurations = set(parent.configurations) if parent else set()
         self._values = {}
         self._cache = {}
 
 
     def __repr__(self):
@@ -152,15 +152,15 @@
     def create_var(self, **kwargs):
         var = ConfigVar(**kwargs)
         self.vars.add(var)
         return var
 
 
     def __getitem__(self, var):
-        if isinstance(var, str): return self.get_configuration(var)
+        if isinstance(var, str): return self.get_configure(var)
         if var not in self.vars:
             tb = traceback.extract_stack(limit=3)[0]
             raise ConfigVarNotFound(tb=tb, var=var, cfg=self)
          # First check our cache.  Then get our value (or our parent's).  Maybe cache the result in our object.
         try:
             return self._cache[var]
         except KeyError:
@@ -188,30 +188,35 @@
             raise ConfigVarNotFound(tb=tb, var=var, cfg=self)
         self._values[var] = val
         try: del self._cache[var]
         except: pass
         var.dfns.append((os.path.relpath(tb.filename), tb.lineno))
 
 
-    def get_configuration(self, name, stack_offset=0):
+    def get_configure(self, name, stack_offset=0):
         name = name.replace('_','-')
         for cfg in self.configurations:
             if cfg == name: return cfg
         else:
             tb = traceback.extract_stack(limit=3+stack_offset)[0]
             raise InvalidConfiguration(name=name, cfg=self, tb=tb)
 
 
-    def set_configuration(self, cfg, unset=False):
+    def add_configure(self, cfg, unset=False):
         if unset:
             self.configurations.discard(cfg)
         else:
             self.configurations.add(cfg)
 
 
+    def set_configure(self, name, stack_offset=1):
+        self.name = name
+        self.get_configure(name, stack_offset=stack_offset).fn()         
+
+
     def __str__(self):
         return self.name or '<default>'
 
 
     def __pretty__(self, print, **kwargs):
         hide_all = set(name.lower() for name in kwargs.get('hide',[]))
         hide_prefix = set(n[:-1] for n in hide_all if n[-1] == '*')
@@ -231,35 +236,40 @@
                 val = var()
             except ConfigVarUnset:
                 val = Line(style='err').insert(0, 'UNSET')
             tbl(var.name,'\t', pretty(val, **kwargs),'\t',var.doc,'\t')
         print(tbl)
         if n_hidden: print(f'\bwarn {n_hidden} hidden')
         if self.configurations:
-            print.card('Configurations\t','\b1$', '    '.join(map(str, sorted(self.configurations))))
+            cfgs = [f'\b{2 if c==self.name else 3} {c}    ' for c in map(str, sorted(self.configurations))]
+            print.card('Configurations\t',*cfgs)
 
 
 # The configuration is accessed through a ContextVar
 config_contextvar = contextvars.ContextVar('Config', default=Config())
 
 def get_config():
     return config_contextvar.get()
 
 
-def copy_config(configuration='', *, context=None):
-    ''' Create a new Config() that is in the given `configuration`.
+def set_config(name='', context=None):
+    cfg = Config(parent=get_config())
+    def in_ctx():
+        config_contextvar.set(cfg)
+        if name: cfg.set_configure(name, 2)
+    context.run(in_ctx) if context else in_ctx()
+    return cfg
+
+
+def copy_config(name='', *, context=None):
+    ''' Create a new Config() that is in the given `name`.
     The new Config() is set in a copy of the given `context` and the new context is returned.
     '''
     ctx = context.copy() if context else contextvars.copy_context()
-    cfg = Config(configuration, parent=get_config())
-    def in_ctx():
-        config_contextvar.set(cfg)
-        if configuration:
-            cfg.get_configuration(configuration,stack_offset=1).fn()
-    ctx.run(in_ctx)
+    set_config(name, ctx)
     return ctx
 
 
 def config_var(doc='', default=UNSET, coerce=lambda x:x, **kwargs):
     ''' Create a new ConfigVar in the current context.
     '''
     return get_config().create_var(default=default, doc=doc, coerce=coerce, **kwargs)
```

### Comparing `yaclipy-1.1.1/src/yaclipy/docs.py` & `yaclipy-1.2.1/src/yaclipy/docs.py`

 * *Files identical despite different names*

### Comparing `yaclipy-1.1.1/src/yaclipy/exceptions.py` & `yaclipy-1.2.1/src/yaclipy/exceptions.py`

 * *Files identical despite different names*

### Comparing `yaclipy-1.1.1/tests/arg_spec_test.py` & `yaclipy-1.2.1/tests/arg_spec_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,7 +34,17 @@
     def g(bob__self): pass
     with pytest.raises(UsageError):
         spec = ArgSpec(g)
 
     def h(x__self): pass
     with pytest.raises(UsageError):
         spec = ArgSpec(h)
+
+
+def test_type_mismatch():
+    def f(a:int, b:int, * c:int): pass
+    s = ArgSpec(f)(['1','b','-c','9'])
+    errs = set([e[0] for e in s.errors])
+    assert(errs == {'NO_VALUE', 'TYPE_MISMATCH', 'UNK_PARAM'})
+    estr = [e[1] for e in s.errors if e[0] == 'NO_VALUE'][0]
+    assert('2nd' in str(estr))
+
```

### Comparing `yaclipy-1.1.1/tests/arg_type_test.py` & `yaclipy-1.2.1/tests/arg_type_test.py`

 * *Files identical despite different names*

### Comparing `yaclipy-1.1.1/tests/bind_test.py` & `yaclipy-1.2.1/tests/bind_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,24 @@
     errors = [e for e in s.errors[:-1] if not _match(e)]
     for e in errors:
         Printer(e)
     assert(matched == errs)
 
 
 
+def test_bind_int():
+    def f(a:int): return a
+    assert(bind(f, '0xff') == ([255], []))
+    assert(bind(f, '0Xff') == ([255], []))
+    assert(bind(f, '0b101') == ([5], []))
+    assert(bind(f, '077') == ([63], []))
+    assert(bind(f, '0') == ([0], []))
+    assert(bind(f, '0004') == ([4], []))
+ 
+  
 def test_bind_positional():
     def f(a, b, /): pass
     assert(bind(f, '\\ -33') == (['','-33'], []))
     assert(bind(f, '-.1 -0') == (['-.1','-0'], []))
```

### Comparing `yaclipy-1.1.1/tests/call_test.py` & `yaclipy-1.2.1/tests/call_test.py`

 * *Files identical despite different names*

### Comparing `yaclipy-1.1.1/tests/cmd_dfn_test.py` & `yaclipy-1.2.1/tests/cmd_dfn_test.py`

 * *Files identical despite different names*

### Comparing `yaclipy-1.1.1/tests/config_test.py` & `yaclipy-1.2.1/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `yaclipy-1.1.1/tests/docs_test.py` & `yaclipy-1.2.1/tests/docs_test.py`

 * *Files identical despite different names*

### Comparing `yaclipy-1.1.1/tests/readme_test.py` & `yaclipy-1.2.1/tests/readme_test.py`

 * *Files identical despite different names*

### Comparing `yaclipy-1.1.1/tests/testutil.py` & `yaclipy-1.2.1/tests/testutil.py`

 * *Files identical despite different names*

### Comparing `yaclipy-1.1.1/LICENSE.txt` & `yaclipy-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yaclipy-1.1.1/README.rst` & `yaclipy-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `yaclipy-1.1.1/pyproject.toml` & `yaclipy-1.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,21 @@
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
+  "Environment :: Console",
+  "Framework :: AsyncIO",
+  "Intended Audience :: Developers",
+  "Topic :: Software Development :: Build Tools",
+  "Topic :: Software Development",
+  "Topic :: Software Development :: User Interfaces",
+  "Topic :: Terminals",
 ]
 dependencies = ['print-ext>=2.1.1', 'docstring_parser']
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/aaron-fl/yaclipy#readme"
 Issues = "https://github.com/aaron-fl/yaclipy/issues"
@@ -65,7 +72,12 @@
 exclude = [
   "/.github",
   "/docs",
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/yaclipy"]
+
+
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+addopts = '--doctest-modules --ignore=local --ignore=tests/notest --ignore=examples --doctest-glob="*.rst"'
```

### Comparing `yaclipy-1.1.1/PKG-INFO` & `yaclipy-1.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 Metadata-Version: 2.1
 Name: yaclipy
-Version: 1.1.1
+Version: 1.2.1
 Summary: Yet another python command-line interface that has a consistent way to call any kind of function/method from the command line.
 Project-URL: Documentation, https://github.com/aaron-fl/yaclipy#readme
 Project-URL: Issues, https://github.com/aaron-fl/yaclipy/issues
 Project-URL: Source, https://github.com/aaron-fl/yaclipy
 Author-email: Aaron <aaron@framelunch.jp>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: User Interfaces
+Classifier: Topic :: Terminals
 Requires-Python: >=3.7
 Requires-Dist: docstring-parser
 Requires-Dist: print-ext>=2.1.1
 Description-Content-Type: text/x-rst
 
 yaclipy
 =======
```

