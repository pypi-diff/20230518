# Comparing `tmp/merkleasy-0.0.3.tar.gz` & `tmp/merkleasy-0.0.3.1.tar.gz`

## Comparing `merkleasy-0.0.3.tar` & `merkleasy-0.0.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 merkleasy-0.0.3/merkleasy/__init__.py
--rw-r--r--   0        0        0    10851 2020-02-02 00:00:00.000000 merkleasy-0.0.3/merkleasy/classes.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 merkleasy-0.0.3/merkleasy/errors.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 merkleasy-0.0.3/tests/context.py
--rw-r--r--   0        0        0    12206 2020-02-02 00:00:00.000000 merkleasy-0.0.3/tests/test_classes.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 merkleasy-0.0.3/tests/test_specification.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 merkleasy-0.0.3/.gitignore
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 merkleasy-0.0.3/license
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 merkleasy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 merkleasy-0.0.3/readme.md
--rw-r--r--   0        0        0    10984 2020-02-02 00:00:00.000000 merkleasy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 merkleasy-0.0.3.1/merkleasy/__init__.py
+-rw-r--r--   0        0        0    10851 2020-02-02 00:00:00.000000 merkleasy-0.0.3.1/merkleasy/classes.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 merkleasy-0.0.3.1/merkleasy/errors.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 merkleasy-0.0.3.1/tests/context.py
+-rw-r--r--   0        0        0    12206 2020-02-02 00:00:00.000000 merkleasy-0.0.3.1/tests/test_classes.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 merkleasy-0.0.3.1/tests/test_specification.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 merkleasy-0.0.3.1/.gitignore
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 merkleasy-0.0.3.1/license
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 merkleasy-0.0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    11713 2020-02-02 00:00:00.000000 merkleasy-0.0.3.1/readme.md
+-rw-r--r--   0        0        0    11902 2020-02-02 00:00:00.000000 merkleasy-0.0.3.1/PKG-INFO
```

### Comparing `merkleasy-0.0.3/merkleasy/classes.py` & `merkleasy-0.0.3.1/merkleasy/classes.py`

 * *Files identical despite different names*

### Comparing `merkleasy-0.0.3/merkleasy/errors.py` & `merkleasy-0.0.3.1/merkleasy/errors.py`

 * *Files identical despite different names*

### Comparing `merkleasy-0.0.3/tests/test_classes.py` & `merkleasy-0.0.3.1/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `merkleasy-0.0.3/license` & `merkleasy-0.0.3.1/license`

 * *Files identical despite different names*

### Comparing `merkleasy-0.0.3/pyproject.toml` & `merkleasy-0.0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "merkleasy"
-version = "0.0.3"
+version = "0.0.3.1"
 authors = [
   { name="k98kurz", email="k98kurz@gmail.com" },
 ]
 description = "Simple, easy-to-use merkle tree library"
 readme = "readme.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `merkleasy-0.0.3/readme.md` & `merkleasy-0.0.3.1/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -86,30 +86,30 @@
 - `prove(self, leaf: bytes, verbose: bool = False) -> list[bytes]`
 - `@staticmethod verify(root: bytes, leaf: bytes, proof: list[bytes]) -> None`
 
 # Usage
 
 Usage examples are shown below.
 
-## Tree.from_leaves
+## `Tree.from_leaves`
 
 The easiest way to use this to create a Merkle Tree is with `from_leaves`:
 
 ```py
 from merkleasy import Tree
 
 leaves = [b'leaf1', b'leaf2', b'leaf3', b'leaf4', b'etc']
 tree = Tree.from_leaves(leaves)
 ```
 
 Note that all leaves are hashed by the `from_leaves` method.
 
 Raises `UsagePreconditionError` upon invalid input.
 
-## Tree.__init__
+## `Tree.__init__`
 
 To make custom Merklized data structures, use the `__init__` method:
 
 ```py
 from hashlib import sha256
 from merkleasy import Tree
 
@@ -130,32 +130,33 @@
     ),
     another_whole_tree
 )
 ```
 
 Raises `UsagePreconditionError` upon invalid input.
 
-## Tree.to_dict and Tree.from_dict
+## `Tree.to_dict` and `Tree.from_dict`
 
 A Tree structure can be converted to a dict and back.
 
 ```py
 from merkleasy import Tree
 
 tree = Tree.from_leaves([b'leaf1', b'leaf2', b'leaf3'])
-converted = tree.to_dict()
-deconverted = Tree.from_dict(converted)
+serialized = tree.to_dict()
+deserialized = Tree.from_dict(serialized)
+assert deserialized == tree
 ```
 
 `Tree.from_dict` raises any of the following upon invalid input:
 - `UsagePreconditionError`
 - `ValueError`
 - `SecurityError`
 
-## Tree.to_json and Tree.from_json
+## `Tree.to_json` and `Tree.from_json`
 
 Serialization and deserialization of a structure uses `to_json` and `from_json`:
 
 ```py
 from merkleasy import Tree
 
 tree = Tree.from_leaves([b'leaf1', b'leaf2', b'leaf3'])
@@ -167,15 +168,15 @@
 
 `Tree.from_json` raises any of the following upon invalid input:
 - `json.decoder.JSONDecodeError`
 - `UsagePreconditionError`
 - `ValueError`
 - `SecurityError`
 
-## Tree.prove
+## `Tree.prove`
 
 Inclusion proofs can be generated using the `prove` method:
 
 ```py
 from merkleasy import Tree
 
 tree = Tree.from_leaves([b'leaf1', b'leaf2', b'leaf3'])
@@ -191,97 +192,118 @@
 for manual inspection by including intermediate, calculated values. However, the
 functionality exists as a side-effect of preventing malicious proofs from
 tricking the validator -- `test_Tree_verify_does_not_validate_malicious_proof`
 contains an example attack.
 
 Raises `UsagePreconditionError` upon invalid input.
 
-## Tree.verify
+## `Tree.verify`
 
 Inclusion proofs can be verified using `Tree.verify`:
 
 ```py
-from merkleasy import Tree
+from merkleasy import Tree, UsagePreconditionError, SecurityError
 
 tree = Tree.from_leaves([b'leaf1', b'leaf2', b'leaf3'])
 leaf = b'leaf1'
 proof1 = tree.prove(leaf)
 proof2 = tree.prove(b'leaf2')
 
 try:
     Tree.verify(tree.root, leaf, proof1)
     # expected result
     print(f'verified proof {[p.hex() for p in proof1]} for {leaf=}')
+except UsagePreconditionError as e:
+    print(f'invalid use of library: {e}')
+except ValueError as e:
+    print(f'invalid proof supplied: {e}')
+except SecurityError as e:
+    print(f'error encountered: {e}')
+
+try:
+    Tree.verify('some string', leaf, proof1)
+    print(f'verified proof {[p.hex() for p in proof1]} for {leaf=}')
+except UsagePreconditionError as e:
+    # expected result
+    print(f'invalid use of library: {e}')
 except ValueError as e:
-    print('invalid proof supplied')
-except AssertionError as e:
+    print(f'invalid proof supplied: {e}')
+except SecurityError as e:
     print(f'error encountered: {e}')
 
 try:
     Tree.verify(tree.root, leaf, [b'\x99', *proof2])
     print(f'verified proof {[p.hex() for p in proof2]} for {leaf=}')
+except UsagePreconditionError as e:
+    print(f'invalid use of library: {e}')
 except ValueError as e:
     # expected result
-    print('invalid proof supplied')
-except AssertionError as e:
+    print(f'invalid proof supplied: {e}')
+except SecurityError as e:
     print(f'error encountered: {e}')
 
 try:
     Tree.verify(tree.root, leaf, proof2)
     print(f'verified proof {[p.hex() for p in proof2]} for {leaf=}')
+except UsagePreconditionError as e:
+    print(f'invalid use of library: {e}')
 except ValueError as e:
-    print('invalid proof supplied')
-except AssertionError as e:
+    print(f'invalid proof supplied: {e}')
+except SecurityError as e:
     # expected result
     print(f'error encountered: {e}')
 ```
 
 This static method parses the proof, interpreting the first byte in each proof
 step as a code from `interfaces.ProofOp`. It ensures that the proof starts with
 the leaf and ends with the root, and then it follows the proof operations.
 
-Raises `UsagePreconditionError` when provided invalid parameters. Raises
-`SecurityError` when provided an invalid proof. If all checks pass, it executes
-without error and returns `None`.
+Raises `UsagePreconditionError` or `ValueError` when provided invalid parameters.
+Raises `SecurityError` when provided an invalid proof. If all checks pass, it
+executes without error and returns `None`.
 
-## get_hash_function
+## `get_hash_function`
 
 To access the currently-set hash function, use the following:
 
-```python
+```py
 from merkleasy import get_hash_function
 
 hash_function = get_hash_function()
+print(hash_function(b'abc').hex())
+# ba7816bf8f01cfea414140de5dae2223b00361a396177a9cb410ff61f20015ad
 ```
 
-## set_hash_function
+## `set_hash_function`
 
 The package uses sha256 by default, but it can be used with any hash function.
 This is accomplished by passing a Callable that takes a bytes parameter, applies
 a hash algorithm, and returns a bytes value. For example, to use sha3_256:
 
-```python
+```py
 from hashlib import sha3_256
-from merkleasy import set_hash_function
+from merkleasy import set_hash_function, get_hash_function
 
 set_hash_function(lambda preimage: sha3_256(preimage).digest())
+print(get_hash_function()(b'abc'))
+# 3a985da74fe225b2045c172d6bd390bd855f086e3e9d525b46bfe24511431532
 ```
 
 Raises `ImplementationError` if the Callable parameter passed in does not meet
 the requirements.
 
 Note that calling `set_hash_function` will have no effect on any `Tree`s created
 prior. However, it _will_ affect any calls to `Tree.verify` with proofs from
 those `Tree`s. If you plan to use the library with a custom hash function, then
 `set_hash_function` should be called during a setup routine.
 
 If you want to handle multiple `Tree`s created with different hash algorithms,
 then a context handler like the below might be useful:
 
-```python
+```py
 from hashlib import sha3_256
 from merkleasy import set_hash_function, get_hash_function, Tree
 
 
 class HashAlgoSwitch:
     """Context manager for switching out algorithms for Tree use."""
     def __init__(self, new_hash_function) -> None:
```

### Comparing `merkleasy-0.0.3/PKG-INFO` & `merkleasy-0.0.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merkleasy
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: Simple, easy-to-use merkle tree library
 Project-URL: Homepage, https://github.com/k98kurz/merkle
 Project-URL: Bug Tracker, https://github.com/k98kurz/merkle/issues
 Author-email: k98kurz <k98kurz@gmail.com>
 License-File: license
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
@@ -101,30 +101,30 @@
 - `prove(self, leaf: bytes, verbose: bool = False) -> list[bytes]`
 - `@staticmethod verify(root: bytes, leaf: bytes, proof: list[bytes]) -> None`
 
 # Usage
 
 Usage examples are shown below.
 
-## Tree.from_leaves
+## `Tree.from_leaves`
 
 The easiest way to use this to create a Merkle Tree is with `from_leaves`:
 
 ```py
 from merkleasy import Tree
 
 leaves = [b'leaf1', b'leaf2', b'leaf3', b'leaf4', b'etc']
 tree = Tree.from_leaves(leaves)
 ```
 
 Note that all leaves are hashed by the `from_leaves` method.
 
 Raises `UsagePreconditionError` upon invalid input.
 
-## Tree.__init__
+## `Tree.__init__`
 
 To make custom Merklized data structures, use the `__init__` method:
 
 ```py
 from hashlib import sha256
 from merkleasy import Tree
 
@@ -145,32 +145,33 @@
     ),
     another_whole_tree
 )
 ```
 
 Raises `UsagePreconditionError` upon invalid input.
 
-## Tree.to_dict and Tree.from_dict
+## `Tree.to_dict` and `Tree.from_dict`
 
 A Tree structure can be converted to a dict and back.
 
 ```py
 from merkleasy import Tree
 
 tree = Tree.from_leaves([b'leaf1', b'leaf2', b'leaf3'])
-converted = tree.to_dict()
-deconverted = Tree.from_dict(converted)
+serialized = tree.to_dict()
+deserialized = Tree.from_dict(serialized)
+assert deserialized == tree
 ```
 
 `Tree.from_dict` raises any of the following upon invalid input:
 - `UsagePreconditionError`
 - `ValueError`
 - `SecurityError`
 
-## Tree.to_json and Tree.from_json
+## `Tree.to_json` and `Tree.from_json`
 
 Serialization and deserialization of a structure uses `to_json` and `from_json`:
 
 ```py
 from merkleasy import Tree
 
 tree = Tree.from_leaves([b'leaf1', b'leaf2', b'leaf3'])
@@ -182,15 +183,15 @@
 
 `Tree.from_json` raises any of the following upon invalid input:
 - `json.decoder.JSONDecodeError`
 - `UsagePreconditionError`
 - `ValueError`
 - `SecurityError`
 
-## Tree.prove
+## `Tree.prove`
 
 Inclusion proofs can be generated using the `prove` method:
 
 ```py
 from merkleasy import Tree
 
 tree = Tree.from_leaves([b'leaf1', b'leaf2', b'leaf3'])
@@ -206,97 +207,118 @@
 for manual inspection by including intermediate, calculated values. However, the
 functionality exists as a side-effect of preventing malicious proofs from
 tricking the validator -- `test_Tree_verify_does_not_validate_malicious_proof`
 contains an example attack.
 
 Raises `UsagePreconditionError` upon invalid input.
 
-## Tree.verify
+## `Tree.verify`
 
 Inclusion proofs can be verified using `Tree.verify`:
 
 ```py
-from merkleasy import Tree
+from merkleasy import Tree, UsagePreconditionError, SecurityError
 
 tree = Tree.from_leaves([b'leaf1', b'leaf2', b'leaf3'])
 leaf = b'leaf1'
 proof1 = tree.prove(leaf)
 proof2 = tree.prove(b'leaf2')
 
 try:
     Tree.verify(tree.root, leaf, proof1)
     # expected result
     print(f'verified proof {[p.hex() for p in proof1]} for {leaf=}')
+except UsagePreconditionError as e:
+    print(f'invalid use of library: {e}')
+except ValueError as e:
+    print(f'invalid proof supplied: {e}')
+except SecurityError as e:
+    print(f'error encountered: {e}')
+
+try:
+    Tree.verify('some string', leaf, proof1)
+    print(f'verified proof {[p.hex() for p in proof1]} for {leaf=}')
+except UsagePreconditionError as e:
+    # expected result
+    print(f'invalid use of library: {e}')
 except ValueError as e:
-    print('invalid proof supplied')
-except AssertionError as e:
+    print(f'invalid proof supplied: {e}')
+except SecurityError as e:
     print(f'error encountered: {e}')
 
 try:
     Tree.verify(tree.root, leaf, [b'\x99', *proof2])
     print(f'verified proof {[p.hex() for p in proof2]} for {leaf=}')
+except UsagePreconditionError as e:
+    print(f'invalid use of library: {e}')
 except ValueError as e:
     # expected result
-    print('invalid proof supplied')
-except AssertionError as e:
+    print(f'invalid proof supplied: {e}')
+except SecurityError as e:
     print(f'error encountered: {e}')
 
 try:
     Tree.verify(tree.root, leaf, proof2)
     print(f'verified proof {[p.hex() for p in proof2]} for {leaf=}')
+except UsagePreconditionError as e:
+    print(f'invalid use of library: {e}')
 except ValueError as e:
-    print('invalid proof supplied')
-except AssertionError as e:
+    print(f'invalid proof supplied: {e}')
+except SecurityError as e:
     # expected result
     print(f'error encountered: {e}')
 ```
 
 This static method parses the proof, interpreting the first byte in each proof
 step as a code from `interfaces.ProofOp`. It ensures that the proof starts with
 the leaf and ends with the root, and then it follows the proof operations.
 
-Raises `UsagePreconditionError` when provided invalid parameters. Raises
-`SecurityError` when provided an invalid proof. If all checks pass, it executes
-without error and returns `None`.
+Raises `UsagePreconditionError` or `ValueError` when provided invalid parameters.
+Raises `SecurityError` when provided an invalid proof. If all checks pass, it
+executes without error and returns `None`.
 
-## get_hash_function
+## `get_hash_function`
 
 To access the currently-set hash function, use the following:
 
-```python
+```py
 from merkleasy import get_hash_function
 
 hash_function = get_hash_function()
+print(hash_function(b'abc').hex())
+# ba7816bf8f01cfea414140de5dae2223b00361a396177a9cb410ff61f20015ad
 ```
 
-## set_hash_function
+## `set_hash_function`
 
 The package uses sha256 by default, but it can be used with any hash function.
 This is accomplished by passing a Callable that takes a bytes parameter, applies
 a hash algorithm, and returns a bytes value. For example, to use sha3_256:
 
-```python
+```py
 from hashlib import sha3_256
-from merkleasy import set_hash_function
+from merkleasy import set_hash_function, get_hash_function
 
 set_hash_function(lambda preimage: sha3_256(preimage).digest())
+print(get_hash_function()(b'abc'))
+# 3a985da74fe225b2045c172d6bd390bd855f086e3e9d525b46bfe24511431532
 ```
 
 Raises `ImplementationError` if the Callable parameter passed in does not meet
 the requirements.
 
 Note that calling `set_hash_function` will have no effect on any `Tree`s created
 prior. However, it _will_ affect any calls to `Tree.verify` with proofs from
 those `Tree`s. If you plan to use the library with a custom hash function, then
 `set_hash_function` should be called during a setup routine.
 
 If you want to handle multiple `Tree`s created with different hash algorithms,
 then a context handler like the below might be useful:
 
-```python
+```py
 from hashlib import sha3_256
 from merkleasy import set_hash_function, get_hash_function, Tree
 
 
 class HashAlgoSwitch:
     """Context manager for switching out algorithms for Tree use."""
     def __init__(self, new_hash_function) -> None:
```

