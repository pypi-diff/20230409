# Comparing `tmp/granola_py-1.0.3.tar.gz` & `tmp/granola_py-1.0.4.tar.gz`

## Comparing `granola_py-1.0.3.tar` & `granola_py-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      302 1970-01-01 00:00:00.000000 granola_py-1.0.3/Cargo.toml
--rw-r--r--   0      501       20     6148 2023-03-22 00:08:45.000000 granola_py-1.0.3/.DS_Store
--rw-r--r--   0      501       20       24 2023-03-22 00:08:45.000000 granola_py-1.0.3/.gitignore
--rw-r--r--   0      501       20  1029970 2023-03-22 00:08:45.000000 granola_py-1.0.3/Granola_Logo.png
--rw-r--r--   0      501       20     1063 2023-03-22 00:08:45.000000 granola_py-1.0.3/LICENSE.md
--rw-r--r--   0      501       20     1061 2023-03-22 00:08:45.000000 granola_py-1.0.3/README.md
--rw-r--r--   0      501       20   132240 2023-03-22 00:08:45.000000 granola_py-1.0.3/code_snippet.png
--rw-r--r--   0      501       20      114 2023-03-22 00:08:45.000000 granola_py-1.0.3/examples/hello_world.py
--rw-r--r--   0      501       20      235 2023-03-22 00:08:45.000000 granola_py-1.0.3/main.py
--rw-r--r--   0      501       20      320 2023-03-22 00:08:45.000000 granola_py-1.0.3/pyproject.toml
--rw-r--r--   0      501       20     2275 2023-04-05 22:16:13.000000 granola_py-1.0.3/src/http.rs
--rw-r--r--   0      501       20     4454 2023-04-05 22:17:12.000000 granola_py-1.0.3/src/lib.rs
--rw-r--r--   0      501       20      942 2023-03-22 00:08:45.000000 granola_py-1.0.3/src/net/mod.rs
--rw-r--r--   0      501       20       26 2023-03-22 00:08:45.000000 granola_py-1.0.3/tests/__main__.py
--rw-r--r--   0      501       20      885 2023-03-22 00:08:45.000000 granola_py-1.0.3/user-guide.md
--rw-r--r--   0      501       20     8755 2023-04-06 00:09:23.000000 granola_py-1.0.3/Cargo.lock
--rw-r--r--   0        0        0     1415 1970-01-01 00:00:00.000000 granola_py-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      321 1970-01-01 00:00:00.000000 granola_py-1.0.4/Cargo.toml
+-rw-r--r--   0      501       20     6148 2023-04-07 17:31:37.000000 granola_py-1.0.4/.DS_Store
+-rw-r--r--   0      501       20       24 2023-04-07 17:31:37.000000 granola_py-1.0.4/.gitignore
+-rw-r--r--   0      501       20  1029970 2023-04-07 17:31:37.000000 granola_py-1.0.4/Granola_Logo.png
+-rw-r--r--   0      501       20     1063 2023-04-07 17:31:37.000000 granola_py-1.0.4/LICENSE.md
+-rw-r--r--   0      501       20     1061 2023-04-07 17:31:37.000000 granola_py-1.0.4/README.md
+-rw-r--r--   0      501       20   132240 2023-04-07 17:31:37.000000 granola_py-1.0.4/code_snippet.png
+-rw-r--r--   0      501       20      114 2023-04-07 17:31:37.000000 granola_py-1.0.4/examples/hello_world.py
+-rw-r--r--   0      501       20      235 2023-04-07 17:31:37.000000 granola_py-1.0.4/main.py
+-rw-r--r--   0      501       20      320 2023-04-07 17:31:37.000000 granola_py-1.0.4/pyproject.toml
+-rw-r--r--   0      501       20     2122 2023-04-09 00:35:32.000000 granola_py-1.0.4/src/http.rs
+-rw-r--r--   0      501       20     4618 2023-04-09 00:38:32.000000 granola_py-1.0.4/src/lib.rs
+-rw-r--r--   0      501       20      942 2023-04-07 17:31:37.000000 granola_py-1.0.4/src/net/mod.rs
+-rw-r--r--   0      501       20       26 2023-04-07 17:31:37.000000 granola_py-1.0.4/tests/__main__.py
+-rw-r--r--   0      501       20      885 2023-04-07 17:31:37.000000 granola_py-1.0.4/user-guide.md
+-rw-r--r--   0      501       20     9578 2023-04-09 00:41:43.000000 granola_py-1.0.4/Cargo.lock
+-rw-r--r--   0        0        0     1415 1970-01-01 00:00:00.000000 granola_py-1.0.4/PKG-INFO
```

### Comparing `granola_py-1.0.3/.DS_Store` & `granola_py-1.0.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.3/Granola_Logo.png` & `granola_py-1.0.4/Granola_Logo.png`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.3/LICENSE.md` & `granola_py-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.3/README.md` & `granola_py-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.3/code_snippet.png` & `granola_py-1.0.4/code_snippet.png`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.3/src/http.rs` & `granola_py-1.0.4/src/http.rs`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,16 @@
     net::TcpStream,
 };
 
 #[derive(Debug, Clone)]
 pub struct Request {
     pub method: String,
     pub host: String,
-    pub route: String,
+        pub route: String,
     pub version: f32,
-    pub body: String,
 }
 
 impl Request {
     pub fn new(mut stream: &TcpStream) -> Self {
         let buf_reader = BufReader::new(&mut stream);
         let http_request_data: Vec<_> = buf_reader
             .lines()
@@ -30,34 +29,31 @@
             .split_whitespace().collect::<Vec<_>>()[0].to_string();
         let host =  http_request_data[1]
             .split_whitespace().collect::<Vec<_>>()[1].to_string();
         let route =  http_request_data[0]
             .split_whitespace().collect::<Vec<_>>()[1].to_string();
         let version = http_request_data[0] 
             .split('/').collect::<Vec<_>>().last().expect("1.1").parse().unwrap();
-        let body = http_request_data.last().unwrap().to_string();
 
         Self {
             method,
             host,
             route,
             version,
-            body
         }
     }
 }
 
 impl IntoPy<Py<PyTuple>> for Request {
     fn into_py(self, py: Python<'_>) -> Py<PyTuple> {
         let dict = PyDict::new(py);
         dict.set_item("method" , &self.method ).unwrap();
         dict.set_item("host"   , &self.host   ).unwrap();
         dict.set_item("route"  , &self.route  ).unwrap();
         dict.set_item("version", &self.version).unwrap();
-        dict.set_item("body", &self.body).unwrap();
         PyTuple::new(py, [dict]).into_py(py)
     }
 }
 
 impl ToString for Request {
     fn to_string(&self) -> String {
         format!("{}: {} {} | {}", self.method, self.host, self.route, self.version)
```

### Comparing `granola_py-1.0.3/src/lib.rs` & `granola_py-1.0.4/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,21 @@
 }
 
 enum RouteResult<T> {
     SubRoute(T),
     Failed
 }
 
+fn extract_path_from_url(url: &str) -> &str {
+    match url.find('?') {
+        Some(index) => &url[..index],
+        None => url,
+    }
+}
+
 fn is_valid_json(json: &RouteResult<&PyAny>) -> bool {
     let final_json = match json {
         RouteResult::Failed => return false,
         RouteResult::SubRoute(resp) => {
             if resp.hasattr("__granola__").unwrap() {
                 resp.call_method0("__granola__").unwrap()
             } else {
@@ -79,15 +86,15 @@
     }
 }
 
 fn handle_connection(stream: Stream, app: &PyAny) {
     let mut request = Request::new(&stream);
     let mut response: RouteResult<&PyAny> = RouteResult::SubRoute(app);
     println!("{}", request.to_string());
-    for call in request.clone().route.split('/').skip_while(|route| route.is_empty()).take_while(|route| !route.is_empty() ) {
+    for call in extract_path_from_url(&request.clone().route).split('/').skip_while(|route| route.is_empty()).take_while(|route| !route.is_empty() ) {
         (response, request) = process_request(call.to_string(), request, response);
     };
 
     let result = if let RouteResult::SubRoute(resp) = response {
         if resp.hasattr("__granola__").unwrap() {
             resp.call_method0("__granola__").unwrap().str().unwrap().to_string()
         } else {
```

### Comparing `granola_py-1.0.3/src/net/mod.rs` & `granola_py-1.0.4/src/net/mod.rs`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.3/user-guide.md` & `granola_py-1.0.4/user-guide.md`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.3/Cargo.lock` & `granola_py-1.0.4/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -28,27 +28,34 @@
 dependencies = [
  "nix",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "granola"
-version = "1.0.3"
+version = "1.0.4"
 dependencies = [
  "ctrlc",
  "pyo3",
+ "serde_json",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da2d6f23ffea9d7e76c53eee25dfb67bcd8fde7f1198b0855350698c9f07c780"
 
 [[package]]
+name = "itoa"
+version = "1.0.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+
+[[package]]
 name = "libc"
 version = "0.2.139"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
 
 [[package]]
 name = "lock_api"
@@ -194,20 +201,43 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "ryu"
+version = "1.0.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+
+[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
+name = "serde"
+version = "1.0.158"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "771d4d9c4163ee138805e12c710dd365e4f44be8be0503cb1bb9eb989425d9c9"
+
+[[package]]
+name = "serde_json"
+version = "1.0.94"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1c533a59c9d8a93a09c6ab31f0fd5e5f4dd1b8fc9434804029839884765d04ea"
+dependencies = [
+ "itoa",
+ "ryu",
+ "serde",
+]
+
+[[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "static_assertions"
```

### Comparing `granola_py-1.0.3/PKG-INFO` & `granola_py-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granola-py
-Version: 1.0.3
+Version: 1.0.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.md
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

