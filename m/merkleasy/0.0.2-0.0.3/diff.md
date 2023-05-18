# Comparing `tmp/merkleasy-0.0.2.tar.gz` & `tmp/merkleasy-0.0.3.tar.gz`

## Comparing `merkleasy-0.0.2.tar` & `merkleasy-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 merkleasy-0.0.2/merkleasy/__init__.py
--rw-r--r--   0        0        0     9215 2020-02-02 00:00:00.000000 merkleasy-0.0.2/merkleasy/classes.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 merkleasy-0.0.2/merkleasy/interfaces.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 merkleasy-0.0.2/tests/context.py
--rw-r--r--   0        0        0    10259 2020-02-02 00:00:00.000000 merkleasy-0.0.2/tests/test_classes.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 merkleasy-0.0.2/.gitignore
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 merkleasy-0.0.2/license
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 merkleasy-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6766 2020-02-02 00:00:00.000000 merkleasy-0.0.2/readme.md
--rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 merkleasy-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 merkleasy-0.0.3/merkleasy/__init__.py
+-rw-r--r--   0        0        0    10851 2020-02-02 00:00:00.000000 merkleasy-0.0.3/merkleasy/classes.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 merkleasy-0.0.3/merkleasy/errors.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 merkleasy-0.0.3/tests/context.py
+-rw-r--r--   0        0        0    12206 2020-02-02 00:00:00.000000 merkleasy-0.0.3/tests/test_classes.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 merkleasy-0.0.3/tests/test_specification.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 merkleasy-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 merkleasy-0.0.3/license
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 merkleasy-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 merkleasy-0.0.3/readme.md
+-rw-r--r--   0        0        0    10984 2020-02-02 00:00:00.000000 merkleasy-0.0.3/PKG-INFO
```

### Comparing `merkleasy-0.0.2/merkleasy/classes.py` & `merkleasy-0.0.3/merkleasy/classes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,97 @@
 from __future__ import annotations
+from .errors import ImplementationError, tressa, eruces
+from enum import Enum
 from hashlib import sha256
-from .interfaces import ProofOp
-from typing import Optional
+from typing import Callable, Optional
 import json
 
 
+_HASH_FUNCTION = lambda input: sha256(input).digest()
+
+def set_hash_function(hash_function: Callable[[bytes], bytes]) -> None:
+    if not callable(hash_function):
+        raise ImplementationError('hash_function must be callable')
+    try:
+        output = hash_function(b'test')
+        if not type(output) is bytes:
+            raise ImplementationError('hash_function must return bytes when called')
+        global _HASH_FUNCTION
+        _HASH_FUNCTION = hash_function
+    except BaseException as e:
+        raise ImplementationError(f'hash_function execution failed with {e}')
+
+def get_hash_function() -> Callable[[bytes], bytes]:
+    return _HASH_FUNCTION
+
+
+class ProofOp(Enum):
+    load_left = b'\x00'
+    load_right = b'\x01'
+    hash_left = b'\x02'
+    hash_right = b'\x03'
+    hash_final = b'\x04'
+
+
 class Tree:
-    root: bytes
-    left: Tree | bytes
-    right: Tree | bytes
-    parent: Optional[Tree]
-    left_bytes: bytes
-    right_bytes: bytes
+    _root: bytes
+    _parent: Optional[Tree]
+    _left: Tree | bytes
+    _right: Tree | bytes
+    _left_bytes: bytes
+    _right_bytes: bytes
+
+    @property
+    def root(self) -> bytes:
+        return self._root
+
+    @property
+    def parent(self) -> Optional[Tree]:
+        return self._parent
+
+    @parent.setter
+    def parent(self, parent) -> None:
+        tressa(isinstance(parent, Tree) or parent is None, 'invalid parent')
+        self._parent = parent
+
+    @property
+    def left(self) -> Tree | bytes:
+        return self._left
+
+    @property
+    def right(self) -> Tree | bytes:
+        return self._right
+
+    @property
+    def left_bytes(self) -> Tree | bytes:
+        return self._left_bytes
+
+    @property
+    def right_bytes(self) -> Tree | bytes:
+        return self._right_bytes
 
     def __init__(self, left: Tree | bytes, right: Tree | bytes) -> None:
         """Set the left, right, and calculated root."""
-        assert type(left) in (Tree, bytes, bytearray), \
-            'left must be one of Tree, bytes, bytearray'
-        assert type(right) in (Tree, bytes, bytearray), \
-            'right must be one of Tree, bytes, bytearray'
+        tressa(type(left) in (Tree, bytes, bytearray),
+            'left must be one of Tree, bytes, bytearray')
+        tressa(type(right) in (Tree, bytes, bytearray),
+            'right must be one of Tree, bytes, bytearray')
 
-        self.left = left if type(left) in (Tree, bytes) else bytes(left)
-        self.right = right if type(right) in (Tree, bytes) else bytes(right)
+        self._left = left if type(left) in (Tree, bytes) else bytes(left)
+        self._right = right if type(right) in (Tree, bytes) else bytes(right)
         self.parent = None
 
         if type(self.left) is Tree:
             self.left.parent = self
         if type(self.right) is Tree:
             self.right.parent = self
 
-        self.left_bytes = self.left.root if isinstance(self.left, Tree) else self.left
-        self.right_bytes = self.right.root if isinstance(self.right, Tree) else self.right
-        self.root = sha256(self.left_bytes + self.right_bytes).digest()
+        self._left_bytes = self.left.root if isinstance(self.left, Tree) else self.left
+        self._right_bytes = self.right.root if isinstance(self.right, Tree) else self.right
+        self._root = get_hash_function()(self.left_bytes + self.right_bytes)
 
     def __str__(self) -> str:
         """Return the root, left, and right in hexadecimal."""
         return f'({self.root.hex()} [{self.left_bytes.hex()}, {self.right_bytes.hex()}])'
 
     def __repr__(self) -> str:
         """Return the root, left, and right in hexadecimal recursively."""
@@ -63,93 +119,63 @@
         """Serialize to json."""
         opts = {} if not pretty else {'indent': '\t'}
         return json.dumps(self.to_dict(), **opts)
 
     @classmethod
     def from_leaves(cls, leaves: list[bytes]) -> Tree:
         """Return a full Tree constructed from the leaves."""
-        assert type(leaves) in (tuple, list), 'leaves must be tuple or list of bytes'
-        assert len(leaves) >= 2, 'must have at least 2 leaves'
+        tressa(type(leaves) in (tuple, list), 'leaves must be tuple or list of bytes')
+        tressa(len(leaves) >= 2, 'must have at least 2 leaves')
 
         for leaf in leaves:
-            assert isinstance(leaf, bytes), 'leaves must be tuple or list of bytes'
+            tressa(isinstance(leaf, bytes), 'leaves must be tuple or list of bytes')
 
         # hash all leaves
-        leaves = [*leaves]
-        for i in range(len(leaves)):
-            leaves[i] = sha256(leaves[i]).digest()
-
-        def join(parts) -> list[Tree]:
-            new_parts = []
-
-            # join every two together
-            for i in range(0, len(parts), 2):
-                if i+1 < len(parts):
-                    new_parts.append(Tree(parts[i], parts[i+1]))
-                else:
-                    new_parts.append(parts[i])
-
-            return new_parts
+        parts = [get_hash_function()(leaf) for leaf in leaves]
 
         # recursively join until reaching the root
-        parts = leaves
         while len(parts) > 1:
-            parts = join(parts)
+            parts = _join(parts)
 
         return parts[0]
 
     @classmethod
     def from_dict(cls, data: dict) -> Tree:
         """Deserialize from a dict and return an instance."""
-        assert type(data) is dict, 'data must be dict type'
-        assert len(data.keys()) == 1, 'data must have one key'
+        tressa(type(data) is dict, 'data must be dict type')
+        tressa(len(data.keys()) == 1, 'data must have one key')
         root = list(data.keys())[0]
-        assert len(data[root]) == 2, 'data must have left and right branch'
+        tressa(len(data[root]) == 2, 'data[root] must have left and right branch')
         left = data[root][0]
         right = data[root][1]
 
         left = bytes.fromhex(left) if type(left) is str else cls.from_dict(left)
         right = bytes.fromhex(right) if type(right) is str else cls.from_dict(right)
-        return cls(left, right)
+        tree = cls(left, right)
+        eruces(tree.root.hex() == root, 'root mismatch')
+        return tree
 
     @classmethod
     def from_json(cls, data: str) -> Tree:
         """Deserialize from json and return an instance."""
         return cls.from_dict(json.loads(data))
 
     def prove(self, leaf: bytes, verbose: bool = False) -> list[bytes]:
         """Create an inclusion proof for a leaf. Use verbose=True to add
             hash checks at each tree level.
         """
-        assert type(leaf) is bytes, 'leaf must be bytes'
-        leaf_hash = sha256(leaf).digest()
+        tressa(type(leaf) is bytes, 'leaf must be bytes')
+        leaf_hash = get_hash_function()(leaf)
 
         # get set of nodes
-        def traverse(branch: Tree, history: tuple[int], exclude_root: bool = True) -> list:
-            """Returns form [(hash, parent, history),...]."""
-            nodes = []
-            if not exclude_root:
-                root = (branch.root, None, tuple(history))
-                nodes += [root]
-            left = (branch.left_bytes, branch, (*history, -1))
-            right = (branch.right_bytes, branch, (*history, 1))
-            nodes += [left, right]
-
-            if type(branch.left) is Tree:
-                nodes.extend(traverse(branch.left, (*history, -1)))
-            if type(branch.right) is Tree:
-                nodes.extend(traverse(branch.right, (*history, 1)))
-
-            return nodes
-
-        nodes = set(traverse(self, tuple(), False))
+        nodes = set(_traverse(self, tuple(), False))
         node_hashes = [n[0] for n in nodes]
 
-        assert leaf in node_hashes or leaf_hash in node_hashes, \
-            'the given leaf was not found in the tree'
+        tressa(leaf in node_hashes or leaf_hash in node_hashes,
+            'the given leaf was not found in the tree')
 
         # start at the leaf node
         node = [n for n in nodes if n[0] in (leaf, leaf_hash)][0]
 
         # reverse the history
         history = list(node)[2][::-1]
         proof = []
@@ -182,50 +208,87 @@
     @staticmethod
     def verify(root: bytes, leaf: bytes, proof: list[bytes]) -> None:
         """Verify an inclusion proof is valid. Raises AssertionError upon
             failure on any step. Raises AssertionError or ValueError on
             invalid input.
         """
         # preconditions
-        assert type(root) is bytes and len(root) == 32, 'root must be 32 bytes'
-        assert type(leaf) is bytes, 'leaf must be bytes'
-        assert type(proof) is list, 'proof must be list of bytes'
+        tressa(type(root) is bytes, 'root must be bytes')
+        tressa(type(leaf) is bytes, 'leaf must be bytes')
+        tressa(type(proof) is list, 'proof must be list of bytes')
 
         # parsing proof
-        leaf_hash = sha256(leaf).digest()
+        leaf_hash = get_hash_function()(leaf)
         steps = []
         for step in proof:
             # another precondition
-            assert type(step) is bytes, 'proof must be list of bytes'
+            tressa(type(step) is bytes, 'proof must be list of bytes')
             steps.append((ProofOp(step[0:1]), step[1:]))
 
-        # more preconditions
-        assert steps[0][1] in (leaf, leaf_hash), 'proof does not reference leaf'
-        assert steps[-1][0] is ProofOp.hash_final, 'proof missing final_hash op'
-        assert steps[-1][1] == root, 'proof does not reference root'
+        # security preconditions
+        eruces(steps[0][1] in (leaf, leaf_hash), 'proof does not reference leaf')
+        eruces(steps[-1][0] is ProofOp.hash_final, 'proof missing final_hash op')
+        eruces(steps[-1][1] == root, 'proof does not reference root')
 
         # run the proof verification calculations
         data = {
             'left': None,
             'right': None,
         }
         for step in steps:
-            match step[0]:
-                case ProofOp.load_left:
-                    if data['left']:
-                        assert data['left'] == step[1], \
-                            'generated hash does not match next step in proof'
-                    data['left'] = step[1]
-                case ProofOp.load_right:
-                    if data['right']:
-                        assert data['right'] == step[1], \
-                            'generated hash does not match next step in proof'
-                    data['right'] = step[1]
-                case ProofOp.hash_left:
-                    data['left'] = sha256(data['left'] + data['right']).digest()
-                    data['right'] = None
-                case ProofOp.hash_right:
-                    data['right'] = sha256(data['left'] + data['right']).digest()
-                    data['left'] = None
-                case ProofOp.hash_final:
-                    result = sha256(data['left'] + data['right']).digest()
-                    assert result == step[1], 'final hash does not match'
+            _run_verification_step(step, data)
+
+
+def _join(parts: list[bytes|Tree]) -> list[Tree]:
+    """Joins every two items together, returning the resulting list of Trees."""
+    new_parts = []
+
+    # join every two together
+    for i in range(0, len(parts), 2):
+        if i+1 < len(parts):
+            new_parts.append(Tree(parts[i], parts[i+1]))
+        else:
+            new_parts.append(parts[i])
+
+    return new_parts
+
+def _traverse(branch: Tree, history: tuple[int], exclude_root: bool = True) -> list:
+    """Returns form [(hash, parent, history),...]."""
+    nodes = []
+    if not exclude_root:
+        root = (branch.root, None, tuple(history))
+        nodes += [root]
+    left = (branch.left_bytes, branch, (*history, -1))
+    right = (branch.right_bytes, branch, (*history, 1))
+    nodes += [left, right]
+
+    if type(branch.left) is Tree:
+        nodes.extend(_traverse(branch.left, (*history, -1)))
+    if type(branch.right) is Tree:
+        nodes.extend(_traverse(branch.right, (*history, 1)))
+
+    return nodes
+
+def _run_verification_step(step: tuple[ProofOp, Optional[bytes]], data: dict) -> None:
+    """Runs an individual verification step. Raises SecurityError on
+        failure; changes data as necessary.
+    """
+    match step[0]:
+        case ProofOp.load_left:
+            if data['left']:
+                eruces(data['left'] == step[1],
+                    'generated hash does not match next step in proof')
+            data['left'] = step[1]
+        case ProofOp.load_right:
+            if data['right']:
+                eruces(data['right'] == step[1], \
+                    'generated hash does not match next step in proof')
+            data['right'] = step[1]
+        case ProofOp.hash_left:
+            data['left'] = get_hash_function()(data['left'] + data['right'])
+            data['right'] = None
+        case ProofOp.hash_right:
+            data['right'] = get_hash_function()(data['left'] + data['right'])
+            data['left'] = None
+        case ProofOp.hash_final:
+            result = get_hash_function()(data['left'] + data['right'])
+            eruces(result == step[1], 'final hash does not match')
```

### Comparing `merkleasy-0.0.2/tests/test_classes.py` & `merkleasy-0.0.3/tests/test_classes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-from context import classes, interfaces
-from hashlib import sha256
+from context import classes, errors
+from hashlib import sha256, sha3_256
 from random import randint
 import unittest
 
 
 class TestMerkle(unittest.TestCase):
     """Test suite for the Merkle project."""
-    def test_merkle_has_TreeProtocol_interface(self):
-        assert hasattr(interfaces, 'TreeProtocol')
+    def setUp(self) -> None:
+        self.original_hash_function = classes.get_hash_function()
+
+    def tearDown(self) -> None:
+        classes.set_hash_function(self.original_hash_function)
 
     def test_merkle_has_class_Tree(self):
         assert hasattr(classes, 'Tree')
         assert isinstance(classes.Tree, type)
 
-    def test_Tree_implements_TreeProtocol(self):
-        assert issubclass(classes.Tree, interfaces.TreeProtocol)
-
     def test_Tree_joins_left_and_right_into_root(self):
-        left = sha256(b'hello').digest()
-        right = sha256(b'world').digest()
-        joined = sha256(left + right).digest()
+        classes.set_hash_function(lambda data: sha3_256(data).digest())
+        left = sha3_256(b'hello').digest()
+        right = sha3_256(b'world').digest()
+        joined = sha3_256(left + right).digest()
         tree = classes.Tree(left, right)
 
         assert hasattr(tree, 'root')
         assert type(tree.root) is bytes
         assert tree.root == joined
 
     def test_Tree_from_leaves_hashes_and_joins_leaves(self):
@@ -34,16 +35,16 @@
 
         assert hasattr(classes.Tree, 'from_leaves')
         tree = classes.Tree.from_leaves(leaves)
         assert tree.left == left_hash
         assert tree.right == right_hash
         assert tree.root == root
 
-    def test_Tree_from_leaves_asserts_at_least_two_leaves(self):
-        with self.assertRaises(AssertionError) as e:
+    def test_Tree_from_leaves_tressas_at_least_two_leaves(self):
+        with self.assertRaises(errors.UsagePreconditionError) as e:
             classes.Tree.from_leaves([b'123'])
         assert str(e.exception) == 'must have at least 2 leaves'
 
     def test_Tree_from_leaves_joins_any_number_of_leaves(self):
         roots = set()
 
         for i in range(2, 300):
@@ -54,22 +55,47 @@
 
     def test_Tree_instance_serializes_to_dict(self):
         tree = classes.Tree(b'left', b'right')
         assert hasattr(tree, 'to_dict') and callable(tree.to_dict)
         serialized = tree.to_dict()
         assert type(serialized) is dict
 
-    def test_Tree_from_dict_unserializes_and_returns_instance(self):
+    def test_Tree_from_dict_deserializes_and_returns_instance(self):
         tree = classes.Tree(b'left', b'right')
         serialized = tree.to_dict()
         assert hasattr(classes.Tree, 'from_dict')
         deserialized = classes.Tree.from_dict(serialized)
         assert type(deserialized) is classes.Tree
         assert tree == deserialized
 
+    def test_Tree_from_dict_raises_errors_for_invalid_params(self):
+        tree = classes.Tree(b'left', b'right')
+        serialized = tree.to_dict()
+
+        with self.assertRaises(errors.UsagePreconditionError) as e:
+            classes.Tree.from_dict('not a dict')
+        assert str(e.exception) == 'data must be dict type'
+
+        with self.assertRaises(errors.UsagePreconditionError) as e:
+            classes.Tree.from_dict({})
+        assert str(e.exception) == 'data must have one key'
+
+        with self.assertRaises(errors.UsagePreconditionError) as e:
+            classes.Tree.from_dict({**serialized, 'what': 'huh'})
+        assert str(e.exception) == 'data must have one key'
+
+        with self.assertRaises(errors.UsagePreconditionError) as e:
+            classes.Tree.from_dict({"3213": [1,2,3]})
+        assert str(e.exception) == 'data[root] must have left and right branch'
+
+        with self.assertRaises(errors.SecurityError) as e:
+            key = list(serialized.keys())[0]
+            classes.Tree.from_dict({"2323": serialized[key]})
+        assert str(e.exception) == 'root mismatch'
+
     def test_Tree_instance_serializes_to_json(self):
         tree = classes.Tree(b'left', b'right')
         assert hasattr(tree, 'to_json') and callable(tree.to_json)
         serialized = tree.to_json()
         assert type(serialized) is str
 
     def test_Tree_from_json_unserializes_and_returns_instance(self):
@@ -93,54 +119,54 @@
             for step in proof_verbose:
                 assert type(step) is bytes
 
     def test_Tree_prove_raises_errors_for_invalid_params(self):
         leaves = [n.to_bytes(2, 'big') for n in range(13)]
         tree = classes.Tree.from_leaves(leaves)
 
-        with self.assertRaises(AssertionError) as e:
+        with self.assertRaises(errors.UsagePreconditionError) as e:
             tree.prove('not bytes')
         assert str(e.exception) == 'leaf must be bytes'
 
-        with self.assertRaises(AssertionError) as e:
+        with self.assertRaises(errors.UsagePreconditionError) as e:
             tree.prove(b'not in tree')
         assert str(e.exception) == 'the given leaf was not found in the tree'
 
     def test_verbose_proof_is_longer_and_has_2_load_steps_after_hash(self):
         leaves = [n.to_bytes(2, 'big') for n in range(17)]
         tree = classes.Tree.from_leaves(leaves)
         leaf_to_prove = randint(3, 15).to_bytes(2, 'big')
         proof = tree.prove(leaf_to_prove)
         verbose = tree.prove(leaf_to_prove, verbose=True)
 
         assert len(verbose) > len(proof)
 
         # normal proof
-        assert interfaces.ProofOp.load_left.value in (proof[0][:1], proof[1][:1])
-        assert interfaces.ProofOp.load_right.value in (proof[0][:1], proof[1][:1])
+        assert classes.ProofOp.load_left.value in (proof[0][:1], proof[1][:1])
+        assert classes.ProofOp.load_right.value in (proof[0][:1], proof[1][:1])
         assert proof[2][:1] in (
-            interfaces.ProofOp.hash_left.value,
-            interfaces.ProofOp.hash_right.value
+            classes.ProofOp.hash_left.value,
+            classes.ProofOp.hash_right.value
         )
-        if proof[2][:1] == interfaces.ProofOp.hash_left.value:
-            assert proof[3][:1] != interfaces.ProofOp.load_left.value
+        if proof[2][:1] == classes.ProofOp.hash_left.value:
+            assert proof[3][:1] != classes.ProofOp.load_left.value
         else:
-            assert proof[3][:1] != interfaces.ProofOp.load_right.value
+            assert proof[3][:1] != classes.ProofOp.load_right.value
 
         # verbose proof
-        assert interfaces.ProofOp.load_left.value in (verbose[0][:1], verbose[1][:1])
-        assert interfaces.ProofOp.load_right.value in (verbose[0][:1], verbose[1][:1])
+        assert classes.ProofOp.load_left.value in (verbose[0][:1], verbose[1][:1])
+        assert classes.ProofOp.load_right.value in (verbose[0][:1], verbose[1][:1])
         assert verbose[2][:1] in (
-            interfaces.ProofOp.hash_left.value,
-            interfaces.ProofOp.hash_right.value
+            classes.ProofOp.hash_left.value,
+            classes.ProofOp.hash_right.value
         )
-        if verbose[2][:1] == interfaces.ProofOp.hash_left.value:
-            assert verbose[3][:1] == interfaces.ProofOp.load_left.value
+        if verbose[2][:1] == classes.ProofOp.hash_left.value:
+            assert verbose[3][:1] == classes.ProofOp.load_left.value
         else:
-            assert verbose[3][:1] == interfaces.ProofOp.load_right.value
+            assert verbose[3][:1] == classes.ProofOp.load_right.value
 
     def test_Tree_verify_executes_without_error_for_valid_proof(self):
         for i in range(2, 300):
             leaves = [n.to_bytes(2, 'big') for n in range(i)]
             tree = classes.Tree.from_leaves(leaves)
             leaf = randint(0, i-1).to_bytes(2, 'big')
             proof = tree.prove(leaf)
@@ -148,84 +174,97 @@
 
     def test_Tree_verify_raises_errors_for_invalid_params(self):
         leaves = [n.to_bytes(2, 'big') for n in range(13)]
         tree = classes.Tree.from_leaves(leaves)
         leaf = leaves[3]
         proof = tree.prove(leaf)
 
-        with self.assertRaises(AssertionError) as e:
+        with self.assertRaises(errors.UsagePreconditionError) as e:
             classes.Tree.verify('tree.root', leaf, proof)
-        assert str(e.exception) == 'root must be 32 bytes'
+        assert str(e.exception) == 'root must be bytes'
 
-        with self.assertRaises(AssertionError) as e:
+        with self.assertRaises(errors.UsagePreconditionError) as e:
             classes.Tree.verify(tree.root, 'leaf', proof)
         assert str(e.exception) == 'leaf must be bytes'
 
-        with self.assertRaises(AssertionError) as e:
+        with self.assertRaises(errors.UsagePreconditionError) as e:
             classes.Tree.verify(tree.root, leaf, {'not': 'list'})
         assert str(e.exception) == 'proof must be list of bytes'
 
-        with self.assertRaises(AssertionError) as e:
+        with self.assertRaises(errors.UsagePreconditionError) as e:
             wrong_proof = ['not bytes']
             classes.Tree.verify(tree.root, leaf, wrong_proof)
         assert str(e.exception) == 'proof must be list of bytes'
 
     def test_Tree_verify_raises_errors_for_invalid_proofs(self):
         leaves = [n.to_bytes(2, 'big') for n in range(13)]
         tree = classes.Tree.from_leaves(leaves)
         leaf = leaves[3]
         proof = tree.prove(leaf)
 
-        with self.assertRaises(AssertionError) as e:
+        with self.assertRaises(errors.SecurityError) as e:
             classes.Tree.verify(tree.root, leaf + b'1', proof)
         assert str(e.exception) == 'proof does not reference leaf'
 
-        with self.assertRaises(AssertionError) as e:
+        with self.assertRaises(errors.SecurityError) as e:
             wrong_proof = proof[1:]
             classes.Tree.verify(tree.root, leaf, wrong_proof)
         assert str(e.exception) == 'proof does not reference leaf'
 
-        with self.assertRaises(AssertionError) as e:
+        with self.assertRaises(errors.SecurityError) as e:
             wrong_proof = proof[:-1]
             classes.Tree.verify(tree.root, leaf, wrong_proof)
         assert str(e.exception) == 'proof missing final_hash op'
 
-        with self.assertRaises(AssertionError) as e:
+        with self.assertRaises(errors.SecurityError) as e:
             wrong_proof = [*proof]
             wrong_proof[-1] = wrong_proof[-1] + b'1'
             classes.Tree.verify(tree.root, leaf, wrong_proof)
         assert str(e.exception) == 'proof does not reference root'
 
         with self.assertRaises(ValueError) as e:
             wrong_proof = [*proof]
             wrong_proof[1] = b'\x99' + wrong_proof[1]
             classes.Tree.verify(tree.root, leaf, wrong_proof)
         assert str(e.exception) == "b'\\x99' is not a valid ProofOp"
 
+        with self.assertRaises(errors.SecurityError) as e:
+            wrong_proof = [*proof]
+            wrong_proof[1] = wrong_proof[1] + b'\x99'
+            classes.Tree.verify(tree.root, leaf, wrong_proof)
+        assert str(e.exception) == "final hash does not match"
+
     def test_Tree_verify_does_not_validate_malicious_proof(self):
         leaves = [b'leaf0', b'leaf1', b'leaf2']
         tree = classes.Tree.from_leaves(leaves)
         legit_proof = tree.prove(b'leaf0')
 
         # first instruction in legit_proof is a load_left operation
-        assert legit_proof[0][:1] == interfaces.ProofOp.load_left.value
+        assert legit_proof[0][:1] == classes.ProofOp.load_left.value
 
         # try to trick the validator by inserting malicious leaf then overwriting
         # with the load_left instruction from the legit_proof, then continuing
         # with the legit_proof
         malicious_proof = [
-            interfaces.ProofOp.load_left.value + sha256(b'malicious leaf').digest(),
+            classes.ProofOp.load_left.value + sha256(b'malicious leaf').digest(),
             *legit_proof
         ]
 
-        with self.assertRaises(AssertionError) as e:
-            # raises AssertionError to prevent proof hijacking
+        with self.assertRaises(errors.SecurityError) as e:
+            # raises errors.SecurityError to prevent proof hijacking
             classes.Tree.verify(tree.root, b'malicious leaf', malicious_proof)
         assert str(e.exception) == 'generated hash does not match next step in proof'
 
+        # try to trick the validator by using a proof for a different tree
+        malicious_proof = classes.Tree.from_leaves([b'malicious', b'leaves']).prove(b'malicious')
+
+        with self.assertRaises(errors.SecurityError) as e:
+            classes.Tree.verify(tree.root, b'malicious', malicious_proof)
+        assert str(e.exception) == 'proof does not reference root'
+
     def test_e2e_arbitrary_branching(self):
         leaves = [sha256(n.to_bytes(2, 'big')).digest() for n in range(13)]
 
         tree = classes.Tree(leaves[0], leaves[1])
         for i in range(2, len(leaves)):
             if randint(0, 1) == 0:
                 tree = classes.Tree(tree, leaves[i])
```

### Comparing `merkleasy-0.0.2/license` & `merkleasy-0.0.3/license`

 * *Files identical despite different names*

### Comparing `merkleasy-0.0.2/pyproject.toml` & `merkleasy-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "merkleasy"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="k98kurz", email="k98kurz@gmail.com" },
 ]
 description = "Simple, easy-to-use merkle tree library"
 readme = "readme.md"
 requires-python = ">=3.7"
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: ISC License (ISCL)",
-    "Operating System :: OS Independent",
-    "Topic :: Security :: Cryptography"
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: ISC License (ISCL)",
+  "Operating System :: OS Independent",
+  "Topic :: Security :: Cryptography"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/k98kurz/merkle"
-"Bug Tracker" = "https://github.com/k98kurz/merkle/issues"
-
-[tool.hatch.build.targets.dist]
-exclude = [
-  "tests"
-]
+"Bug Tracker" = "https://github.com/k98kurz/merkle/issues"
```

