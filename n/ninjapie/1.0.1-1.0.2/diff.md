# Comparing `tmp/ninjapie-1.0.1.tar.gz` & `tmp/ninjapie-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninjapie-1.0.1.tar", last modified: Sun Apr  9 11:31:07 2023, max compression
+gzip compressed data, was "ninjapie-1.0.2.tar", last modified: Sun Apr  9 17:47:34 2023, max compression
```

## Comparing `ninjapie-1.0.1.tar` & `ninjapie-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-09 11:31:07.520022 ninjapie-1.0.1/
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    17987 2023-03-26 07:31:08.000000 ninjapie-1.0.1/LICENSE
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27518 2023-04-09 11:31:07.520022 ninjapie-1.0.1/PKG-INFO
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     6139 2023-04-09 11:30:25.000000 ninjapie-1.0.1/README.md
-drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-09 11:31:07.520022 ninjapie-1.0.1/ninjapie/
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)      158 2023-04-09 11:30:28.000000 ninjapie-1.0.1/ninjapie/__init__.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     4283 2023-04-09 11:30:25.000000 ninjapie-1.0.1/ninjapie/__main__.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27403 2023-04-09 11:30:25.000000 ninjapie-1.0.1/ninjapie/env.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    18899 2023-04-09 11:30:25.000000 ninjapie-1.0.1/ninjapie/generator.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     3899 2023-04-09 11:30:25.000000 ninjapie-1.0.1/ninjapie/path.py
-drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-09 11:31:07.520022 ninjapie-1.0.1/ninjapie.egg-info/
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27518 2023-04-09 11:31:07.000000 ninjapie-1.0.1/ninjapie.egg-info/PKG-INFO
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)      292 2023-04-09 11:31:07.000000 ninjapie-1.0.1/ninjapie.egg-info/SOURCES.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)        1 2023-04-09 11:31:07.000000 ninjapie-1.0.1/ninjapie.egg-info/dependency_links.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       52 2023-04-09 11:31:07.000000 ninjapie-1.0.1/ninjapie.egg-info/entry_points.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       14 2023-04-09 11:31:07.000000 ninjapie-1.0.1/ninjapie.egg-info/top_level.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     1339 2023-04-09 11:30:28.000000 ninjapie-1.0.1/pyproject.toml
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       38 2023-04-09 11:31:07.520022 ninjapie-1.0.1/setup.cfg
+drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-09 17:47:34.859796 ninjapie-1.0.2/
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    17987 2023-03-26 07:31:08.000000 ninjapie-1.0.2/LICENSE
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27518 2023-04-09 17:47:34.859796 ninjapie-1.0.2/PKG-INFO
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     6139 2023-04-09 11:30:25.000000 ninjapie-1.0.2/README.md
+drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-09 17:47:34.856462 ninjapie-1.0.2/ninjapie/
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)      158 2023-04-09 16:37:33.000000 ninjapie-1.0.2/ninjapie/__init__.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     4644 2023-04-09 15:55:05.000000 ninjapie-1.0.2/ninjapie/__main__.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27728 2023-04-09 16:36:42.000000 ninjapie-1.0.2/ninjapie/env.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    19340 2023-04-09 15:57:25.000000 ninjapie-1.0.2/ninjapie/generator.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     3894 2023-04-09 16:06:55.000000 ninjapie-1.0.2/ninjapie/path.py
+drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-09 17:47:34.859796 ninjapie-1.0.2/ninjapie.egg-info/
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27518 2023-04-09 17:47:34.000000 ninjapie-1.0.2/ninjapie.egg-info/PKG-INFO
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)      292 2023-04-09 17:47:34.000000 ninjapie-1.0.2/ninjapie.egg-info/SOURCES.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)        1 2023-04-09 17:47:34.000000 ninjapie-1.0.2/ninjapie.egg-info/dependency_links.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       52 2023-04-09 17:47:34.000000 ninjapie-1.0.2/ninjapie.egg-info/entry_points.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       14 2023-04-09 17:47:34.000000 ninjapie-1.0.2/ninjapie.egg-info/top_level.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     1339 2023-04-09 16:37:33.000000 ninjapie-1.0.2/pyproject.toml
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       38 2023-04-09 17:47:34.859796 ninjapie-1.0.2/setup.cfg
```

### Comparing `ninjapie-1.0.1/LICENSE` & `ninjapie-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ninjapie-1.0.1/PKG-INFO` & `ninjapie-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjapie
-Version: 1.0.1
+Version: 1.0.2
 Summary: Ninja-based build system with a Python API
 Author-email: Nils Asmussen <nils.asmussen@barkhauseninstitut.org>
 License: 		    GNU GENERAL PUBLIC LICENSE
         		       Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `ninjapie-1.0.1/README.md` & `ninjapie-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ninjapie-1.0.1/ninjapie/__main__.py` & `ninjapie-1.0.2/ninjapie/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,88 +3,95 @@
 import os
 import subprocess
 import sys
 
 
 def all_files(build_dir):
     """Collects a string with all files found by the patters in the globs file"""
+
     files = ''
     try:
-        with open(build_dir + '/.build.globs', 'r') as file:
+        with open(build_dir + '/.build.globs', 'r', encoding='utf-8') as file:
             for line in file.readlines():
                 files += '\n'.join(glob(line.strip(), recursive=True))
                 files += '\n'
     except FileNotFoundError:
         pass
     return files
 
 
-def clean(build_dir, args, ninja_args):
+def clean(build_dir, _args, _ninja_args):
+    """Implements the clean command"""
+
     def remove_dir(path):
         """Removes the given directory recursively"""
-        for d in os.listdir(path):
+        for entry in os.listdir(path):
             try:
-                remove_dir(path + '/' + d)
+                remove_dir(path + '/' + entry)
             except OSError:
-                os.remove(path + '/' + d)
+                os.remove(path + '/' + entry)
         os.rmdir(path)
 
     remove_dir(build_dir)
     return 0
 
 
 def build(build_dir, args, ninja_args):
+    """Implements the build command"""
+
     reconf = args.force_regen
     root_dir = os.path.dirname(os.path.dirname(os.path.realpath(__file__)))
     all_files_path = build_dir + '/.build.files'
     build_file = build_dir + '/build.ninja'
 
     # export PYTHONPATH to find the ninjapie modules
     python_path = os.environ.setdefault('PYTHONPATH', '')
     os.environ['PYTHONPATH'] = root_dir + ': ' + python_path
 
     # check if we need to reconfigure
     if not reconf:
         try:
             # check whether files have been added or removed
-            old_files = open(all_files_path, 'r').read()
+            with open(all_files_path, 'r', encoding='utf-8') as file:
+                old_files = file.read()
             new_files = all_files(build_dir)
             # if the list of files changed, we need to reconfigure
             reconf = old_files != new_files
         except FileNotFoundError:
             reconf = True
-            pass
 
     # run configure if not done before or it's required
     if reconf or not os.path.isfile(build_file):
         try:
             # run build.py, but don't write *.pyc files
             subprocess.check_call(['python3', '-B', 'build.py'])
-        except:
+        except Exception:  # pylint: disable=W0718
             return 1
 
         # store new list of files from globs
         new_files = all_files(build_dir)
-        with open(all_files_path, 'w') as file:
+        with open(all_files_path, 'w', encoding='utf-8') as file:
             file.write(new_files)
 
     # now build everything with ninja
     try:
         subprocess.check_call(['ninja', '-f', build_file] + ninja_args, stdout=sys.stderr.buffer)
-    except:
+    except Exception:  # pylint: disable=W0718
         # ensure that we regenerate the build.ninja next time. Since ninja does not accept the
         # build.ninja, it will also not detect changes our build files in order to regenerate it.
         # Therefore, force a regenerate next time by removing the file.
         os.remove(all_files_path)
         return 1
 
     return 0
 
 
 def main(argv=None):
+    """Main entry point"""
+
     if argv is None:
         argv = sys.argv[1:]
 
     # determine and create build dir
     build_dir = os.environ.setdefault('NPBUILD', 'build')
     if not os.path.isdir(build_dir):
         os.makedirs(build_dir)
@@ -110,23 +117,24 @@
     parser_build.set_defaults(func=build)
 
     # we pass everything after "--" directly to ninja
     try:
         ninja_start = argv.index('--')
         ninja_args = argv[ninja_start + 1:]
         our_args = argv[0:ninja_start]
-    except:
+    except ValueError:
         ninja_args = []
         our_args = argv
 
     # parse arguments and run command
     args = parser.parse_args(our_args)
     try:
         res = args.func(build_dir, args, ninja_args)
-    except:
+    except AttributeError:
+        # if func attribute is not found, fall back to default: build
         args.force_regen = False
         res = build(build_dir, args, ninja_args)
     return res
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `ninjapie-1.0.1/ninjapie/env.py` & `ninjapie-1.0.2/ninjapie/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,18 +211,18 @@
 
         Parameters
         ----------
         :param var: the variable name
         :param flags: the flags to remove
         """
 
-        for f in flags:
+        for flag in flags:
             assert isinstance(self._vars[var], list)
-            if f in self._vars[var]:
-                self._vars[var].remove(f)
+            if flag in self._vars[var]:
+                self._vars[var].remove(flag)
 
     def sub_build(self, gen: Generator, dir: str):
         """
         Calls the build.py in the given subdirectory
 
         In a project with multiple files to build (libraries, executables, etc.), it makes sense to
         organize them into multiple directories. This method is used to run the `build.py` in a
@@ -248,16 +248,16 @@
 
         old_cwd = self.cur_dir
         self._cwd.path += '/' + dir
 
         gen._add_build_file(self.cur_dir + '/build.py')
 
         mod_path = self.cur_dir[2:].replace('/', '.')
-        b = importlib.import_module(mod_path + '.build')
-        b.build(gen, self)
+        sub = importlib.import_module(mod_path + '.build')
+        sub.build(gen, self)
 
         self._cwd.path = old_cwd
 
     def glob(self, gen: Generator, pattern: str) -> list[SourcePath]:
         """
         Produces a list of files that match the given pattern
 
@@ -421,15 +421,15 @@
         A `BuildPath` to the output file
         """
 
         flags = ' '.join(self['ASFLAGS'] + self['CPPFLAGS'])
         flags += ' ' + ' '.join(['-I' + i for i in self['CPPPATH']])
         return self._cc(gen, out, ins, flags)
 
-    def cc(self, gen: Generator, out: str, ins: list[str]) -> BuildPath:
+    def cc(self, gen: Generator, out: str, ins: list[str]) -> BuildPath:  # pylint: disable=C0103
         """
         Runs the C compiler on the given input files
 
         Parameters
         ----------
         :param gen: the generator
         :param out: the output file
@@ -607,15 +607,15 @@
                 'shlinkflags': flags
             }
         )
         gen.add_build(edge)
         return lib
 
     def c_exe(self, gen: Generator, out: str, ins: list[str],
-              libs: list[str] = [], deps: list[str] = []) -> BuildPath:
+              libs: list[str] = None, deps: list[str] = None) -> BuildPath:
         """
         Produces a C executable from given input files
 
         The input files can be all file types that `Env.objs` supports.
 
         Parameters
         ----------
@@ -632,18 +632,20 @@
         :param `LIBPATH`: the paths to search libraries in (e.g., ['lib'])
 
         Returns
         -------
         The `BuildPath` to the produced executable
         """
 
+        libs = [] if libs is None else libs
+        deps = [] if deps is None else deps
         return self._c_cxx_exe(gen, out, ins, libs, deps, self['CC'])
 
     def cxx_exe(self, gen: Generator, out: str, ins: list[str],
-                libs: list[str] = [], deps: list[str] = []) -> BuildPath:
+                libs: list[str] = None, deps: list[str] = None) -> BuildPath:
         """
         Produces a C++ executable from given input files
 
         The input files can be all file types that `Env.objs` supports.
 
         Parameters
         ----------
@@ -660,14 +662,16 @@
         :param `LIBPATH`: the paths to search libraries in (e.g., ['lib'])
 
         Returns
         -------
         The `BuildPath` to the produced executable
         """
 
+        libs = [] if libs is None else libs
+        deps = [] if deps is None else deps
         return self._c_cxx_exe(gen, out, ins, libs, deps, self['CXX'])
 
     def _c_cxx_exe(self, gen: Generator, out: str, ins: list[str],
                    libs: list[str], deps: list[str], linker: str) -> BuildPath:
         flags = ''
         if len(libs) > 0:
             flags += ' '.join(self['LINKFLAGS'])
@@ -688,15 +692,15 @@
                 'link': linker,
                 'linkflags': flags
             }
         )
         gen.add_build(edge)
         return bin
 
-    def rust_lib(self, gen: Generator, out: str, deps: list[str] = []) -> BuildPath:
+    def rust_lib(self, gen: Generator, out: str, deps: list[str] = None) -> BuildPath:
         """
         Produces a Rust library
 
         This method runs `cargo` in the current directory and therefore expects a `Cargo.toml` that
         produces a static Rust library. The `--target-dir` argument will be pass to cargo according
         to `Env.build_dir` and `RUSTBINS`. The location of the produced file will be determined by
         the `--target` and `--release` arguments in `CRGFLAGS`, if present. You can also use
@@ -718,17 +722,18 @@
         :param `CRGENV`: additional environment variables
 
         Returns
         -------
         The `BuildPath` to the produced static library
         """
 
+        deps = [] if deps is None else deps
         return self.rust(gen, ['lib' + out + '.a'], deps)[0]
 
-    def rust_exe(self, gen: Generator, out: str, deps: list[str] = []) -> BuildPath:
+    def rust_exe(self, gen: Generator, out: str, deps: list[str] = None) -> BuildPath:
         """
         Produces a Rust executable
 
         This method runs `cargo` in the current directory and therefore expects a `Cargo.toml` that
         produces a binary. The `--target-dir` argument will be pass to cargo according to
         `Env.build_dir` and `RUSTBINS`. The location of the produced file will be determined by the
         `--target` and `--release` arguments in `CRGFLAGS`, if present. You can also use `CRGENV` to
@@ -750,14 +755,15 @@
         :param `CRGENV`: additional environment variables
 
         Returns
         -------
         The `BuildPath` to the produced executable
         """
 
+        deps = [] if deps is None else deps
         return self.rust(gen, [out], deps)[0]
 
     def rust(self, gen: Generator, outs: list[str], deps: list[str]) -> [BuildPath]:
         """
         Produces multiple Rust libraries or executables
 
         This method runs `cargo` in the current directory and therefore expects a `Cargo.toml`. The
@@ -787,15 +793,15 @@
         """
 
         # determine whether cargo puts the output in a target-specific directory
         target_dir = ''
         try:
             idx = self['CRGFLAGS'].index('--target')
             target_dir = self['CRGFLAGS'][idx + 1] + '/'
-        except:
+        except ValueError:
             pass
 
         # determine destination directory
         btype = 'release' if '--release' in self['CRGFLAGS'] else 'debug'
         dest_dir = BuildPath(self.build_dir + '/' + self['RUSTBINS'] + '/' + target_dir + btype)
         out_paths = [BuildPath(dest_dir + '/' + o) for o in outs]
```

### Comparing `ninjapie-1.0.1/ninjapie/generator.py` & `ninjapie-1.0.2/ninjapie/generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,16 +80,16 @@
 
     A build edge therefore references a specific rule and assigns values to the variables defined
     for the rule. Most importantly, a rule has one or more output files and one or more input files.
     Whenever one of the input files changes, the command of the rule will be invoked to reproduce
     the output files. Additional dependencies can be specified to also trigger a rebuild.
     """
 
-    def __init__(self, rule: str, outs: list[str], ins: list[str], deps: list[str] = [],
-                 vars: dict[str, str] = {}, libs: list[str] = [], lib_path: list[str] = []):
+    def __init__(self, rule: str, outs: list[str], ins: list[str], deps: list[str] = None,
+                 vars: dict[str, str] = None, libs: list[str] = None, lib_path: list[str] = None):
         """
         Creates a new build edge.
 
         Parameters
         ----------
         :param rule: the name of the rule (needs to exist in the `Generator`)
         :param outs: a list of paths that are produced as outputs when executing the command
@@ -98,14 +98,19 @@
         :param vars: an optional list with values for additional variables used in the rule
         :param libs: when producing executables, a list of library names that is linked against
         :param lib_path: when producing executables, a list of paths to search the libraries in
         """
 
         assert len(outs) > 0, "The list of output files cannot be empty"
 
+        deps = [] if deps is None else deps
+        vars = {} if vars is None else vars
+        libs = [] if libs is None else libs
+        lib_path = [] if lib_path is None else lib_path
+
         self.calltrace = None
         self.rule = rule
         self.outs = outs
         self.ins = ins
         # copy the dependencies, because we want to alter them for this specific BuildEdge later
         self.deps = deps.copy()
         # without inputs and dependencies, we always want to rebuild it
@@ -127,17 +132,17 @@
         """
 
         file.write('build %s: %s %s' %
                    (' '.join(self.outs), self.rule, ' '.join(self.ins)))
         if len(self.deps) > 0:
             file.write(' | %s' % (' '.join(self.deps)))
         file.write('\n')
-        for k, v in self.vars.items():
-            if k not in defaults or defaults[k] != v:
-                file.write('  %s = %s\n' % (k, v))
+        for key, val in self.vars.items():
+            if key not in defaults or defaults[key] != val:
+                file.write('  %s = %s\n' % (key, val))
 
 
 class Generator:
     """
     The `Generator` collects rules and build edges and finally writes a Ninja build file.
 
     The rules describe how specific file types are built (e.g., shared libraries), while a build
@@ -249,19 +254,19 @@
         :param name: The name of the rule
         :param rule: The `Rule` object to add
         """
 
         assert edge.rule in self._rules
 
         if self._debug:
-            for b in self._build_edges:
-                for o in edge.outs:
-                    assert o not in b.outs, \
+            for ex_edge in self._build_edges:
+                for out in ex_edge.outs:
+                    assert out not in ex_edge.outs, \
                         "Output '{}' is already produced by the build edge added here:\n{}".format(
-                            o, ''.join(traceback.format_list(b.calltrace)))
+                            out, ''.join(traceback.format_list(ex_edge.calltrace)))
             edge.calltrace = traceback.extract_stack()
 
         self._rules[edge.rule].refs += 1
         self._build_edges.append(edge)
 
     def _add_glob(self, pattern):
         """
@@ -326,72 +331,72 @@
         ))
 
         self._finalize_deps()
         if defaults is None:
             defaults = self._determine_defaults()
 
         # generate build.ninja
-        with open(build_file, 'w') as file:
+        with open(build_file, 'w', encoding='utf-8') as file:
             file.write('# This file has been generated by the ninjapie build system.\n')
             file.write('\n')
 
-            for k, v in defaults.items():
-                file.write('%s = %s\n' % (k, v))
+            for key, val in defaults.items():
+                file.write('%s = %s\n' % (key, val))
             file.write('\n')
 
-            for n, r in self._rules.items():
-                if r.refs > 0:
-                    r._write_to_file(n, file)
+            for name, rule in self._rules.items():
+                if rule.refs > 0:
+                    rule._write_to_file(name, file)
             file.write('\n')
 
             # separate pool for the build.ninja regeneration to run that alone
             file.write('pool build_pool\n')
             file.write('  depth = 1\n')
             file.write('\n')
 
-            for b in self._build_edges:
-                b._write_to_file(defaults, file)
+            for edge in self._build_edges:
+                edge._write_to_file(defaults, file)
 
         # generate deps of build.ninja
         build_files = ['build.py'] + self._build_files
-        with open(dep_file, 'w') as file:
+        with open(dep_file, 'w', encoding='utf-8') as file:
             file.write(build_file + ': ' + ' '.join(build_files))
 
         # generate files with all globs
-        with open(glob_file, 'w') as file:
-            for g in self._globs:
-                file.write(g + '\n')
+        with open(glob_file, 'w', encoding='utf-8') as file:
+            for glb in self._globs:
+                file.write(glb + '\n')
 
     def write_compile_cmds(self):
         """
         Writes a `compiler_commands.json` file for `clangd`.
 
         This file is leveraged by the language server `clangd` to know how your source files are
         build. The file is written to `$NPBUILD/compile_commands.json` and will be overwritten, if
         existing. Note that only the rules `cxx` and `cc` are considered.
         """
 
         outdir = self._build_dir
 
         # generate compile_commands.json for clangd
-        with open(outdir + '/compile_commands.json', 'w') as cmds:
+        with open(outdir + '/compile_commands.json', 'w', encoding='utf-8') as cmds:
             cmds.write('[\n')
             base_dir = os.getcwd()
-            c = 0
-            for b in self._build_edges:
-                if b.rule == 'cxx' or b.rule == 'cc':
-                    assert len(b.ins) == 1
-                    if c > 0:
+            count = 0
+            for edge in self._build_edges:
+                if edge.rule in ('cxx', 'cc'):
+                    assert len(edge.ins) == 1
+                    if count > 0:
                         cmds.write(',\n')
                     cmds.write('  {\n')
                     cmds.write('    "directory": "{}",\n'.format(base_dir))
-                    cmds.write('    "file": "{}",\n'.format(b.ins[0]))
-                    cmds.write('    "command": "{}"\n'.format(self._get_clang_flags(b)))
+                    cmds.write('    "file": "{}",\n'.format(edge.ins[0]))
+                    cmds.write('    "command": "{}"\n'.format(self._get_clang_flags(edge)))
                     cmds.write('  }')
-                    c += 1
+                    count += 1
             cmds.write('\n]\n')
 
     def _get_clang_flags(self, bedge: BuildEdge) -> str:
         """
         Determines the flags for clang or clang++ for the given build edge.
 
         Parameters
@@ -421,22 +426,22 @@
         Returns
         -------
         A dictionary with the variable names and values
         """
 
         # first count the number of times for each value and each variable
         vars = {}
-        for b in self._build_edges:
-            for k, v in b.vars.items():
-                if k not in vars:
-                    vars[k] = {}
-                if v in vars[k]:
-                    vars[k][v] += 1
+        for edge in self._build_edges:
+            for key, val in edge.vars.items():
+                if key not in vars:
+                    vars[key] = {}
+                if val in vars[key]:
+                    vars[key][val] += 1
                 else:
-                    vars[k][v] = 1
+                    vars[key][val] = 1
 
         # now use the most-used value for each variable as the default
         defaults = {}
         for name, vals in vars.items():
             max_count = 0
             max_key = None
             for key, count in vals.items():
@@ -455,34 +460,34 @@
         libraries that we build ourself are known, we complete the dependencies of the build edges
         based on these `libs`. That is, whenever we build the library ourself, we add the path to
         the built library to the dependency. Otherwise, we assume that the library exists in some
         system directory and will not change (we do not add it to the dependencies).
         """
 
         libs = self._collect_libs()
-        for b in self._build_edges:
-            for d in b.libs:
-                stname = 'lib' + d + '.a'
-                shname = 'lib' + d + '.so'
-                for p in b.lib_path:
-                    if p in libs:
-                        if shname in libs[p]:
-                            b.deps.append(libs[p][shname])
+        for edge in self._build_edges:
+            for lib in edge.libs:
+                stname = 'lib' + lib + '.a'
+                shname = 'lib' + lib + '.so'
+                for path in edge.lib_path:
+                    if path in libs:
+                        if shname in libs[path]:
+                            edge.deps.append(libs[path][shname])
                             break
-                        elif stname in libs[p]:
-                            b.deps.append(libs[p][stname])
+                        if stname in libs[path]:
+                            edge.deps.append(libs[path][stname])
                             break
 
     def _collect_libs(self) -> dict[str, dict[str, str]]:
         """
         Collects the libraries that we build ourself.
         """
 
         libs = {}
-        for b in self._build_edges:
-            for o in b.outs:
-                if o.endswith('.a') or o.endswith('.so'):
-                    dir = os.path.dirname(o)
+        for edge in self._build_edges:
+            for out in edge.outs:
+                if out.endswith('.a') or out.endswith('.so'):
+                    dir = os.path.dirname(out)
                     if dir not in libs:
                         libs[dir] = {}
-                    libs[dir][os.path.basename(o)] = o
+                    libs[dir][os.path.basename(out)] = out
         return libs
```

### Comparing `ninjapie-1.0.1/ninjapie/path.py` & `ninjapie-1.0.2/ninjapie/path.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         Parameters
         ----------
         :param path: the path
         """
 
         self._path = path
 
+    @staticmethod
     def new(env, path):
         """
         Creates a new `SourcePath` from given path object
 
         The path object can be a `SourcePath`, `BuildPath` or `str`. The former two just create a
         `SourcePath` with the path within the existing object, whereas `str` is interpreted relative
         to `Env.cur_dir`.
@@ -39,18 +40,17 @@
         Returns
         -------
         A `SourcePath` object
         """
 
         if isinstance(path, SourcePath):
             return SourcePath(path._path)
-        elif isinstance(path, BuildPath):
+        if isinstance(path, BuildPath):
             return SourcePath(path._path)
-        else:
-            return SourcePath(env.cur_dir + '/' + path)
+        return SourcePath(env.cur_dir + '/' + path)
 
     def __str__(self) -> str:
         return self._path
 
     def __repr__(self) -> str:
         return repr(self._path)
 
@@ -74,14 +74,15 @@
         Parameters
         ----------
         :param path: the path
         """
 
         self._path = path
 
+    @staticmethod
     def new(env, path):
         """
         Creates a new `BuildPath` from given path object
 
         The path object can be a `SourcePath`, `BuildPath` or `str`. If it's build path, it simply
         creates a copy. If it's a source path, it produces a `BuildPath` consisting of
         `Env.build_dir` and the path. If it's a string, it produces a `BuildPath` consisting of
@@ -95,19 +96,19 @@
         Returns
         -------
         A `BuildPath` object
         """
 
         if isinstance(path, BuildPath):
             return BuildPath(path._path)
-        elif isinstance(path, SourcePath):
+        if isinstance(path, SourcePath):
             return BuildPath(env.build_dir + '/' + path._path)
-        else:
-            return BuildPath(env.build_dir + '/' + env.cur_dir + '/' + path)
+        return BuildPath(env.build_dir + '/' + env.cur_dir + '/' + path)
 
+    @staticmethod
     def with_file_ext(env, path, ext: str):
         """
         Creates a new `BuildPath` from given path object and file extension
 
         This method is the same as `BuildPath.new`, but replaces the file extension of the given
         path with `ext`.
 
@@ -118,20 +119,19 @@
         :param ext: the new file extension
 
         Returns
         -------
         A `BuildPath` object
         """
 
-        (root, cur_ext) = os.path.splitext(path)
+        (root, _cur_ext) = os.path.splitext(path)
         if isinstance(path, BuildPath):
             return BuildPath(root + '.' + ext)
-        elif isinstance(path, SourcePath):
+        if isinstance(path, SourcePath):
             return BuildPath.new(env, SourcePath(root + '.' + ext))
-        else:
-            return BuildPath.new(env, root + '.' + ext)
+        return BuildPath.new(env, root + '.' + ext)
 
     def __str__(self) -> str:
         return self._path
 
     def __repr__(self) -> str:
         return repr(self._path)
```

### Comparing `ninjapie-1.0.1/ninjapie.egg-info/PKG-INFO` & `ninjapie-1.0.2/ninjapie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjapie
-Version: 1.0.1
+Version: 1.0.2
 Summary: Ninja-based build system with a Python API
 Author-email: Nils Asmussen <nils.asmussen@barkhauseninstitut.org>
 License: 		    GNU GENERAL PUBLIC LICENSE
         		       Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `ninjapie-1.0.1/pyproject.toml` & `ninjapie-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ninjapie"
-version = "1.0.1"
+version = "1.0.2"
 description = "Ninja-based build system with a Python API"
 readme = "README.md"
 authors = [{ name = "Nils Asmussen", email = "nils.asmussen@barkhauseninstitut.org" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -30,15 +30,15 @@
 [tool.setuptools]
 include-package-data = false
 
 [tool.setuptools.packages.find]
 exclude = ["coverage*", "tests*"]
 
 [tool.bumpver]
-current_version = "1.0.1"
+current_version = "1.0.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}."
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

