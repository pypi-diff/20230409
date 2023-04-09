# Comparing `tmp/pygwalker-0.1.7a2.tar.gz` & `tmp/pygwalker-0.1.7a3.tar.gz`

## Comparing `pygwalker-0.1.7a2.tar` & `pygwalker-0.1.7a3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/app/.gitignore
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/app/index.html
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/app/package.json
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/app/tsconfig.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/app/vite.config.ts
--rw-r--r--   0        0        0   124304 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/app/yarn.lock
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/app/src/index.tsx
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/app/src/components/options.tsx
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/app/src/interfaces/index.ts
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pygwalker/__init__.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pygwalker/__main__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pygwalker/__version__.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pygwalker/base.py
--rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pygwalker/gwalker.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pygwalker/templates/.gitignore
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pygwalker/templates/index.html
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pygwalker/templates/walk.js
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pygwalker/templates/dist/index.d.ts
--rw-r--r--   0        0        0  1765339 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pygwalker/templates/dist/pygwalker-app.iife.js
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pygwalker/templates/dist/components/options.d.ts
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pygwalker/templates/dist/interfaces/index.d.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pygwalker/utils/__init__.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pygwalker/utils/check_update.py
--rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pygwalker/utils/config.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pygwalker/utils/defaults.json
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pygwalker/utils/fname_encodings.py
--rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pygwalker/utils/gwalker_props.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pygwalker/utils/render.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/scripts/__init__.py
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/scripts/compile.sh
--rwxr-xr-x   0        0        0      458 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/scripts/develop.sh
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/scripts/test-init.py
--rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/scripts/test-init.sh
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/.gitignore
--rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/LICENSE
--rw-r--r--   0        0        0    12861 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/README.md
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/pyproject.toml
--rw-r--r--   0        0        0    26945 2020-02-02 00:00:00.000000 pygwalker-0.1.7a2/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/app/.gitignore
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/app/index.html
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/app/package.json
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/app/tsconfig.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/app/vite.config.ts
+-rw-r--r--   0        0        0   124304 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/app/yarn.lock
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/app/src/index.tsx
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/app/src/components/options.tsx
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/app/src/interfaces/index.ts
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/__init__.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/__main__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/__version__.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/base.py
+-rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/gwalker.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/templates/.gitignore
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/templates/index.html
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/templates/walk.js
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/templates/dist/index.d.ts
+-rw-r--r--   0        0        0  1765339 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/templates/dist/pygwalker-app.iife.js
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/templates/dist/components/options.d.ts
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/templates/dist/interfaces/index.d.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/utils/__init__.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/utils/check_update.py
+-rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/utils/config.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/utils/defaults.json
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/utils/fname_encodings.py
+-rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/utils/gwalker_props.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/utils/render.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/scripts/__init__.py
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/scripts/compile.sh
+-rwxr-xr-x   0        0        0      458 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/scripts/develop.sh
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/scripts/test-init.py
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/scripts/test-init.sh
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/.gitignore
+-rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/LICENSE
+-rw-r--r--   0        0        0    12861 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/README.md
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pyproject.toml
+-rw-r--r--   0        0        0    26975 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/PKG-INFO
```

### Comparing `pygwalker-0.1.7a2/app/package.json` & `pygwalker-0.1.7a3/app/package.json`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/app/tsconfig.json` & `pygwalker-0.1.7a3/app/tsconfig.json`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/app/vite.config.ts` & `pygwalker-0.1.7a3/app/vite.config.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/app/yarn.lock` & `pygwalker-0.1.7a3/app/yarn.lock`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/app/src/index.tsx` & `pygwalker-0.1.7a3/app/src/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/app/src/components/options.tsx` & `pygwalker-0.1.7a3/app/src/components/options.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/pygwalker/__init__.py` & `pygwalker-0.1.7a3/pygwalker/__init__.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/pygwalker/__main__.py` & `pygwalker-0.1.7a3/pygwalker/__main__.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/pygwalker/base.py` & `pygwalker-0.1.7a3/pygwalker/base.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/pygwalker/gwalker.py` & `pygwalker-0.1.7a3/pygwalker/gwalker.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/pygwalker/templates/walk.js` & `pygwalker-0.1.7a3/pygwalker/templates/walk.js`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/pygwalker/templates/dist/pygwalker-app.iife.js` & `pygwalker-0.1.7a3/pygwalker/templates/dist/pygwalker-app.iife.js`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/pygwalker/utils/check_update.py` & `pygwalker-0.1.7a3/pygwalker/utils/check_update.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/pygwalker/utils/config.py` & `pygwalker-0.1.7a3/pygwalker/utils/config.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/pygwalker/utils/gwalker_props.py` & `pygwalker-0.1.7a3/pygwalker/utils/gwalker_props.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/pygwalker/utils/render.py` & `pygwalker-0.1.7a3/pygwalker/utils/render.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/scripts/test-init.py` & `pygwalker-0.1.7a3/scripts/test-init.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/scripts/test-init.sh` & `pygwalker-0.1.7a3/scripts/test-init.sh`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/.gitignore` & `pygwalker-0.1.7a3/.gitignore`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/LICENSE` & `pygwalker-0.1.7a3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/README.md` & `pygwalker-0.1.7a3/README.md`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a2/pyproject.toml` & `pygwalker-0.1.7a3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
 dependencies = [
     "jinja2",
     "ipython",
     "typing_extensions; python_version <= '3.7'",
-    "aiohttp>=3.0.0",
+    "aiohttp>=3.0.0; platform_machine != 'wasm32'",
 ]
 [project.urls]
 homepage = "https://github.com/Kanaries/pygwalker"
 repository = "https://github.com/Kanaries/pygwalker"
 # changelog, documentation
 
 [project.optional-dependencies]
```

### Comparing `pygwalker-0.1.7a2/PKG-INFO` & `pygwalker-0.1.7a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygwalker
-Version: 0.1.7a2
+Version: 0.1.7a3
 Summary: pygwalker: Combining Jupyter Notebook with a Tableau-like UI
 Project-URL: homepage, https://github.com/Kanaries/pygwalker
 Project-URL: repository, https://github.com/Kanaries/pygwalker
 Author-email: "Asm.Def" <woojson@zju.edu.cn>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
@@ -208,15 +208,15 @@
            See the License for the specific language governing permissions and
            limitations under the License.
 License-File: LICENSE
 Keywords: data-analysis,data-exploration,dataframe,jupyter,pandas,tableau,tableau-alternative,visualization
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
-Requires-Dist: aiohttp>=3.0.0
+Requires-Dist: aiohttp>=3.0.0; platform_machine != 'wasm32'
 Requires-Dist: ipython
 Requires-Dist: jinja2
 Requires-Dist: typing-extensions; python_version <= '3.7'
 Provides-Extra: all
 Requires-Dist: pygwalker[pandas,polars,streamlit]; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: build; extra == 'dev'
```

