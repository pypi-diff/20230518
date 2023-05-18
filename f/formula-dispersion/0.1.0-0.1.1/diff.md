# Comparing `tmp/formula_dispersion-0.1.0.tar.gz` & `tmp/formula_dispersion-0.1.1.tar.gz`

## Comparing `formula_dispersion-0.1.0.tar` & `formula_dispersion-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      447 1970-01-01 00:00:00.000000 formula_dispersion-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123     2809 2023-05-17 15:30:13.000000 formula_dispersion-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-05-17 15:30:13.000000 formula_dispersion-0.1.0/.gitignore
--rw-r--r--   0     1001      123       52 2023-05-17 15:30:13.000000 formula_dispersion-0.1.0/.pylintrc
--rw-r--r--   0     1001      123    32472 2023-05-17 15:30:13.000000 formula_dispersion-0.1.0/LICENSE.txt
--rw-r--r--   0     1001      123       93 2023-05-17 15:30:13.000000 formula_dispersion-0.1.0/README.md
--rw-r--r--   0     1001      123       75 2023-05-17 15:30:13.000000 formula_dispersion-0.1.0/build.rs
--rw-r--r--   0     1001      123      380 2023-05-17 15:30:13.000000 formula_dispersion-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123    14451 2023-05-17 15:30:13.000000 formula_dispersion-0.1.0/src/ast.rs
--rw-r--r--   0     1001      123     2001 2023-05-17 15:30:13.000000 formula_dispersion-0.1.0/src/formula_parser.lalrpop
--rw-r--r--   0     1001      123     5383 2023-05-17 15:30:13.000000 formula_dispersion-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123     2013 2023-05-17 15:30:13.000000 formula_dispersion-0.1.0/tests/test_array.py
--rw-r--r--   0     1001      123    24620 2023-05-17 15:30:13.000000 formula_dispersion-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 formula_dispersion-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      465 1970-01-01 00:00:00.000000 formula_dispersion-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      123     2809 2023-05-18 08:09:03.000000 formula_dispersion-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-05-18 08:09:03.000000 formula_dispersion-0.1.1/.gitignore
+-rw-r--r--   0     1001      123       52 2023-05-18 08:09:03.000000 formula_dispersion-0.1.1/.pylintrc
+-rw-r--r--   0     1001      123    32472 2023-05-18 08:09:03.000000 formula_dispersion-0.1.1/LICENSE.txt
+-rw-r--r--   0     1001      123       93 2023-05-18 08:09:03.000000 formula_dispersion-0.1.1/README.md
+-rw-r--r--   0     1001      123       75 2023-05-18 08:09:03.000000 formula_dispersion-0.1.1/build.rs
+-rw-r--r--   0     1001      123      380 2023-05-18 08:09:03.000000 formula_dispersion-0.1.1/pyproject.toml
+-rw-r--r--   0     1001      123    14451 2023-05-18 08:09:03.000000 formula_dispersion-0.1.1/src/ast.rs
+-rw-r--r--   0     1001      123     2001 2023-05-18 08:09:03.000000 formula_dispersion-0.1.1/src/formula_parser.lalrpop
+-rw-r--r--   0     1001      123     5532 2023-05-18 08:09:03.000000 formula_dispersion-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      123     2013 2023-05-18 08:09:03.000000 formula_dispersion-0.1.1/tests/test_array.py
+-rw-r--r--   0     1001      123    30555 2023-05-18 08:09:03.000000 formula_dispersion-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 formula_dispersion-0.1.1/PKG-INFO
```

### Comparing `formula_dispersion-0.1.0/.github/workflows/CI.yml` & `formula_dispersion-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `formula_dispersion-0.1.0/.gitignore` & `formula_dispersion-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `formula_dispersion-0.1.0/LICENSE.txt` & `formula_dispersion-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `formula_dispersion-0.1.0/src/ast.rs` & `formula_dispersion-0.1.1/src/ast.rs`

 * *Files identical despite different names*

### Comparing `formula_dispersion-0.1.0/src/formula_parser.lalrpop` & `formula_dispersion-0.1.1/src/formula_parser.lalrpop`

 * *Files identical despite different names*

### Comparing `formula_dispersion-0.1.0/src/lib.rs` & `formula_dispersion-0.1.1/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use crate::ast::Expr;
 use crate::ast::ExprParams;
 use ast::EvaluateResult;
+use cached::proc_macro::cached;
 use lalrpop_util::lexer::Token;
 use lalrpop_util::ParseError;
 use num_complex::Complex64;
 use numpy::ndarray::Array1;
 use numpy::ndarray::ArrayView1;
 use numpy::PyReadonlyArray1;
 use numpy::{IntoPyArray, PyArray1};
@@ -79,26 +80,29 @@
         .is_err());
     assert!(formula_parser::FormulaParser::new()
         .parse("something = ((22)")
         .is_err());
     assert!(formula_parser::FormulaParser::new().parse("(22)").is_err());
 }
 
-fn parse_ast<'a>(formula: &'a str) -> Result<Box<Expr>, ParseError<usize, Token<'a>, &'a str>> {
+#[cached]
+fn parse_ast(
+    formula: &'static str,
+) -> Result<Box<Expr<'static>>, ParseError<usize, Token<'static>, &'static str>> {
     formula_parser::FormulaParser::new().parse(formula)
 }
 
 fn parse<'a>(
     formula: &'a str,
     x_axis_name: &'a str,
     x_axis_values: &'a ArrayView1<'a, f64>,
     single_params: &'a HashMap<&str, f64>,
     rep_params: &'a HashMap<&str, Vec<f64>>,
 ) -> Result<Array1<Complex64>, Box<dyn error::Error + 'a>> {
-    let ast = parse_ast(formula)?;
+    let ast = parse_ast(Box::leak(formula.to_string().into_boxed_str()))?;
     match ast.evaluate(&mut ExprParams {
         x_axis_name: &x_axis_name,
         x_axis_values: &x_axis_values,
         single_params,
         rep_params,
         sum_params: None,
     })? {
@@ -110,15 +114,15 @@
 }
 
 #[pymodule]
 fn formula_dispersion(_py: Python, m: &PyModule) -> PyResult<()> {
     #[pyfn(m)]
     #[pyo3(name = "get_representation")]
     fn get_representation_py<'py>(formula: &str) -> PyResult<&'py str> {
-        let ast = match parse_ast(formula) {
+        let ast = match parse_ast(Box::leak(formula.to_string().into_boxed_str())) {
             Ok(ast) => ast,
             Err(err) => return Err(PyErr::new::<PyTypeError, _>(err.to_string())),
         };
 
         match ast.get_representation() {
             Ok(repr) => Ok(repr),
             Err(err) => Err(PyErr::new::<PyTypeError, _>(err.to_string())),
```

### Comparing `formula_dispersion-0.1.0/tests/test_array.py` & `formula_dispersion-0.1.1/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `formula_dispersion-0.1.0/Cargo.lock` & `formula_dispersion-0.1.1/Cargo.lock`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,31 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8824ecca2e851cec16968d54a01dd372ef8f95b244fb84b84e70128be347c3c6"
 dependencies = [
  "term",
 ]
 
 [[package]]
+name = "async-trait"
+version = "0.1.68"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.15",
+]
+
+[[package]]
+name = "async_once"
+version = "0.2.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2ce4f10ea3abcd6617873bae9f91d1c5332b4a778bd9ce34d0cd517474c1de82"
+
+[[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "bit-set"
@@ -44,14 +61,52 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "cached"
+version = "0.43.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bc2fafddf188d13788e7099295a59b99e99b2148ab2195cae454e754cc099925"
+dependencies = [
+ "async-trait",
+ "async_once",
+ "cached_proc_macro",
+ "cached_proc_macro_types",
+ "futures",
+ "hashbrown 0.13.2",
+ "instant",
+ "lazy_static",
+ "once_cell",
+ "thiserror",
+ "tokio",
+]
+
+[[package]]
+name = "cached_proc_macro"
+version = "0.16.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e10ca87c81aaa3a949dbbe2b5e6c2c45dbc94ba4897e45ea31ff9ec5087be3dc"
+dependencies = [
+ "cached_proc_macro_types",
+ "darling",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "cached_proc_macro_types"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3a4f925191b4367301851c6d99b09890311d74b0d43f274c0b34c86d308a3663"
+
+[[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cfg-if"
@@ -62,14 +117,49 @@
 [[package]]
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
 [[package]]
+name = "darling"
+version = "0.14.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b750cb3417fd1b327431a470f388520309479ab0bf5e323505daf0290cd3850"
+dependencies = [
+ "darling_core",
+ "darling_macro",
+]
+
+[[package]]
+name = "darling_core"
+version = "0.14.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "109c1ca6e6b7f82cc233a97004ea8ed7ca123a9af07a8230878fcfda9b158bf0"
+dependencies = [
+ "fnv",
+ "ident_case",
+ "proc-macro2",
+ "quote",
+ "strsim",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "darling_macro"
+version = "0.14.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a4aab4dbc9f7611d8b55048a3a16d2d010c2c8334e46304b40ac1cc14bf3b48e"
+dependencies = [
+ "darling_core",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "diff"
 version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56254986775e3233ffa9c4d7d3faaf6d36a2c09d30b20687e9f88bc8bafc16c8"
 
 [[package]]
 name = "dirs-next"
@@ -141,28 +231,96 @@
 [[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
+name = "fnv"
+version = "1.0.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
+
+[[package]]
 name = "formula-dispersion"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
+ "cached",
  "errorfunctions",
  "lalrpop",
  "lalrpop-util",
  "num-complex",
  "numpy",
  "physical_constants",
  "pyo3",
  "regex",
 ]
 
 [[package]]
+name = "futures"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
+dependencies = [
+ "futures-channel",
+ "futures-core",
+ "futures-io",
+ "futures-sink",
+ "futures-task",
+ "futures-util",
+]
+
+[[package]]
+name = "futures-channel"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
+dependencies = [
+ "futures-core",
+ "futures-sink",
+]
+
+[[package]]
+name = "futures-core"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
+
+[[package]]
+name = "futures-io"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
+
+[[package]]
+name = "futures-sink"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
+
+[[package]]
+name = "futures-task"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
+
+[[package]]
+name = "futures-util"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
+dependencies = [
+ "futures-core",
+ "futures-sink",
+ "futures-task",
+ "pin-project-lite",
+ "pin-utils",
+]
+
+[[package]]
 name = "getrandom"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
@@ -172,36 +330,57 @@
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
+name = "hashbrown"
+version = "0.13.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43a3c133739dddd0d2990f9a4bdf8eb4b21ef50e4851ca85ab661199821d510e"
+
+[[package]]
 name = "hermit-abi"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
+name = "ident_case"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
+
+[[package]]
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
- "hashbrown",
+ "hashbrown 0.12.3",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
+name = "instant"
+version = "0.1.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
+dependencies = [
+ "cfg-if",
+]
+
+[[package]]
 name = "io-lifetimes"
 version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
 dependencies = [
  "hermit-abi",
  "libc",
@@ -258,14 +437,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5c1f7869c94d214466c5fd432dfed12c379fd87786768d36455892d46b18edd"
 dependencies = [
  "regex",
 ]
 
 [[package]]
+name = "lazy_static"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
+
+[[package]]
 name = "libc"
 version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "linux-raw-sys"
@@ -486,14 +671,26 @@
 [[package]]
 name = "pico-args"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "db8bcd96cb740d03149cbad5518db9fd87126a10ab519c011893b1754134c468"
 
 [[package]]
+name = "pin-project-lite"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+
+[[package]]
+name = "pin-utils"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
+
+[[package]]
 name = "precomputed-hash"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "925383efa346730478fb4838dbe9137d2a47675ad789c546d150a6e1dd4ab31c"
 
 [[package]]
 name = "proc-macro2"
@@ -676,14 +873,20 @@
  "once_cell",
  "parking_lot",
  "phf_shared",
  "precomputed-hash",
 ]
 
 [[package]]
+name = "strsim"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
+
+[[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
@@ -744,14 +947,37 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
 dependencies = [
  "crunchy",
 ]
 
 [[package]]
+name = "tokio"
+version = "1.28.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0aa32867d44e6f2ce3385e89dceb990188b8bb0fb25b0cf576647a6f98ac5105"
+dependencies = [
+ "autocfg",
+ "pin-project-lite",
+ "tokio-macros",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "tokio-macros"
+version = "2.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.15",
+]
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unicode-xid"
```

### Comparing `formula_dispersion-0.1.0/PKG-INFO` & `formula_dispersion-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formula-dispersion
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.txt
 Author: Florian Dobener <florian.dobener@schroedingerscat.org>
 Author-email: Florian Dobener <florian.dobener@schroedingerscat.org>
 Requires-Python: >=3.7
```

