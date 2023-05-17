# Comparing `tmp/quivr-0.2.3.tar.gz` & `tmp/quivr-0.3.0.tar.gz`

## Comparing `quivr-0.2.3.tar` & `quivr-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 quivr-0.2.3/quivr/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.2.3/quivr/__version__.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 quivr-0.2.3/quivr/concat.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 quivr-0.2.3/quivr/defragment.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 quivr-0.2.3/quivr/errors.py
--rw-r--r--   0        0        0    22772 2020-02-02 00:00:00.000000 quivr-0.2.3/quivr/fields.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 quivr-0.2.3/quivr/indexing.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.2.3/quivr/matrix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.2.3/quivr/py.typed
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 quivr-0.2.3/quivr/schemagraph.py
--rw-r--r--   0        0        0    18416 2020-02-02 00:00:00.000000 quivr-0.2.3/quivr/tables.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 quivr-0.2.3/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.2.3/LICENSE
--rw-r--r--   0        0        0     7894 2020-02-02 00:00:00.000000 quivr-0.2.3/README.md
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 quivr-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     8292 2020-02-02 00:00:00.000000 quivr-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 quivr-0.3.0/quivr/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.3.0/quivr/__version__.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 quivr-0.3.0/quivr/concat.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 quivr-0.3.0/quivr/defragment.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 quivr-0.3.0/quivr/errors.py
+-rw-r--r--   0        0        0    22772 2020-02-02 00:00:00.000000 quivr-0.3.0/quivr/fields.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 quivr-0.3.0/quivr/indexing.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.3.0/quivr/matrix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.3.0/quivr/py.typed
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 quivr-0.3.0/quivr/schemagraph.py
+-rw-r--r--   0        0        0    19299 2020-02-02 00:00:00.000000 quivr-0.3.0/quivr/tables.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.3.0/LICENSE
+-rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 quivr-0.3.0/README.md
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 quivr-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9741 2020-02-02 00:00:00.000000 quivr-0.3.0/PKG-INFO
```

### Comparing `quivr-0.2.3/quivr/__init__.py` & `quivr-0.3.0/quivr/__init__.py`

 * *Files identical despite different names*

### Comparing `quivr-0.2.3/quivr/concat.py` & `quivr-0.3.0/quivr/concat.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,11 +25,11 @@
     first = True
     for v in values:
         batches += v.table.to_batches()
         if first:
             cls = v.__class__
             first = False
     table = pa.Table.from_batches(batches)
-    result = cls(pa_table=table)
+    result = cls(table=table)
     if defrag:
         result = defragment(result)
     return result
```

### Comparing `quivr-0.2.3/quivr/fields.py` & `quivr-0.3.0/quivr/fields.py`

 * *Files identical despite different names*

### Comparing `quivr-0.2.3/quivr/indexing.py` & `quivr-0.3.0/quivr/indexing.py`

 * *Files identical despite different names*

### Comparing `quivr-0.2.3/quivr/matrix.py` & `quivr-0.3.0/quivr/matrix.py`

 * *Files identical despite different names*

### Comparing `quivr-0.2.3/quivr/schemagraph.py` & `quivr-0.3.0/quivr/schemagraph.py`

 * *Files identical despite different names*

### Comparing `quivr-0.2.3/quivr/tables.py` & `quivr-0.3.0/quivr/tables.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,18 +24,27 @@
         for name, field in cls.__dict__.items():
             if isinstance(field, Field):
                 fields.append(field.pyarrow_field())
 
         # Generate a pyarrow schema
         schema = pa.schema(fields)
         cls.schema = schema
+
+        # If the subclass has an __init__ override, it must have a
+        # with_table override as well.
+        if "__init__" in cls.__dict__ and "with_table" not in cls.__dict__:
+            raise TypeError(
+                f"{cls.__name__} has an __init__ override, but does not have a with_table "
+                + "override. You must implement both or neither."
+            )
+
         super().__init_subclass__(**kwargs)
 
-    def __init__(self, pa_table: pa.Table):
-        self.table = pa_table
+    def __init__(self, table: pa.Table):
+        self.table = table
 
     @classmethod
     def from_data(cls, data: Optional[Any] = None, **kwargs) -> Self:
         """
         Create an instance of the Table and populate it with data.
 
         This is a convenience method which tries to infer the right
@@ -66,26 +75,26 @@
             >>> MyTable.from_data(a=np.array(["a", "b"]), b=np.array([1, 2]))
             MyTable(size=2)
         """
         if data is None:
             return cls.from_kwargs(**kwargs)
 
         if isinstance(data, pa.Table):
-            return cls(pa_table=data)
+            return cls(table=data, **kwargs)
         if isinstance(data, dict):
-            return cls.from_pydict(data)
+            return cls.from_pydict(data, **kwargs)
         if isinstance(data, list):
             if len(data) == 0:
-                return cls.from_rows(data)
+                return cls.from_rows(data, **kwargs)
             if isinstance(data[0], dict):
-                return cls.from_rows(data)
+                return cls.from_rows(data, **kwargs)
             elif isinstance(data[0], list):
-                return cls.from_lists(data)
+                return cls.from_lists(data, **kwargs)
         if isinstance(data, pd.DataFrame):
-            return cls.from_dataframe(data)
+            return cls.from_dataframe(data, **kwargs)
         raise TypeError(f"Unsupported type: {type(data)}")
 
     @classmethod
     def as_field(cls, nullable: bool = True, metadata: Optional[MetadataDict] = None) -> SubTableField[Self]:
         return SubTableField(cls, nullable=nullable, metadata=metadata)
 
     @classmethod
@@ -105,15 +114,16 @@
         # Therefore, we need to keep track of which columns are empty
         # *before* we've discovered the size of the table so we can
         # populate them with nulls later.
         empty_columns = []
 
         for i, field in enumerate(cls.schema):
             column_name = field.name
-            value = kwargs.get(column_name)
+            value = kwargs.pop(column_name, None)
+
             if value is None:
                 if not field.nullable:
                     raise ValueError(f"Missing non-nullable column {column_name}")
                 else:
                     if size is not None:
                         arrays.append(pa.nulls(size, type=cls.schema[i].type))
                     else:
@@ -141,42 +151,44 @@
                 raise TypeError(f"Unsupported type for {column_name}: {type(value)}")
 
         if size is None:
             raise ValueError("No data provided")
 
         for idx in empty_columns:
             arrays[idx] = pa.nulls(size, type=cls.schema[idx].type)
-        return cls.from_arrays(arrays)
+        return cls.from_arrays(arrays, **kwargs)
 
     @classmethod
-    def from_arrays(cls, arrays: list[pa.array]) -> Self:
+    def from_arrays(cls, arrays: list[pa.array], **kwargs) -> Self:
         """Create a Table object from a list of arrays.
 
         Args:
             arrays: A list of pyarrow.Array objects.
+            **kwargs: Additional keyword arguments to pass to the Table's __init__ method.
 
         Returns:
             A Table object.
 
         """
         table = pa.Table.from_arrays(arrays, schema=cls.schema)
-        return cls(pa_table=table)
+        return cls(table=table, **kwargs)
 
     @classmethod
-    def from_pydict(cls, d: dict[str, Union[pa.array, list, np.ndarray]]) -> Self:
+    def from_pydict(cls, d: dict[str, Union[pa.array, list, np.ndarray]], **kwargs) -> Self:
         table = pa.Table.from_pydict(d, schema=cls.schema)
-        return cls(pa_table=table)
+        return cls(table=table, **kwargs)
 
     @classmethod
-    def from_rows(cls, rows: list[dict]) -> Self:
+    def from_rows(cls, rows: list[dict], **kwargs) -> Self:
         """
         Create a Table object from a list of dictionaries.
 
         Args:
             rows: A list of values. Each value corresponds to a row in the table.
+            **kwargs: Additional keyword arguments to pass to the Table's __init__ method.
 
         Returns:
             A Table object.
 
         Examples:
             >>> import quivr
             >>> class Inner(quivr.Table):
@@ -187,69 +199,68 @@
             ...     i = Inner.as_field()
             ...
             >>> data = [{"z": "v1", "i": {"a": "v1_in"}}, {"z": "v2", "i": {"a": "v2_in"}}]
             >>> Outer.from_pylist(data)
             Outer(size=2)
         """
         table = pa.Table.from_pylist(rows, schema=cls.schema)
-        return cls(pa_table=table)
+        return cls(table=table, **kwargs)
 
     @classmethod
-    def from_lists(cls, lists: list[list]) -> Self:
+    def from_lists(cls, lists: list[list], **kwargs) -> Self:
         """Create a Table object from a list of lists.
 
         Each inner list corresponds to a field in the Table. They
         should be specified in the same order as the fields in the
         class.
 
         Args:
             lists: A list of lists. Each inner list corresponds to a column in the table.
+            **kwargs: Additional keyword arguments to pass to the Table's __init__ method.
+
 
         Returns:
             A TableBase object.
 
         """
         table = pa.Table.from_arrays(list(map(pa.array, lists)), schema=cls.schema)
-        return cls(pa_table=table)
+        return cls(table=table, **kwargs)
 
     @classmethod
-    def from_dataframe(cls, df: pd.DataFrame):
+    def from_dataframe(cls, df: pd.DataFrame, **kwargs):
         """Load a DataFrame into the Table.
 
         If the DataFrame is missing any of the Table's columns, an
         error is raised. If the DataFrame has extra columns, they are
         ignored.
 
         This function cannot load "flattened" dataframes. This only
         matters for nested Tables which contain other Table
         definitions as fields. For that use case, either load an
         unflattened DataFrame, or use from_flat_dataframe.
         """
 
         table = pa.Table.from_pandas(df, schema=cls.schema)
-        return cls(pa_table=table)
+        return cls(table=table, **kwargs)
 
     @classmethod
     def _unflatten_table(cls, table: pa.Table):
         """Unflatten a Table.
 
-        This is used when loading a flattened DataFrame into a nested
+        This is used when loading a flattened CSV into a nested
         Table. It takes a Table with a flat schema, and returns a
         Table with a nested schema.
 
         """
         struct_fields = []
 
         for field in cls.schema:
             if pa.types.is_struct(field.type):
                 struct_fields.append(field)
 
-        if len(struct_fields) == 0:
-            return cls(pa_table=table)
-
         # Walk the schema, and build a StructArray for each embedded
         # type.
 
         def struct_array_for(field: pa.Field, ancestors: list[pa.Field]):
             prefix = ".".join([f.name for f in ancestors if f.name] + [field.name])
 
             child_arrays = []
@@ -267,26 +278,26 @@
                 child_arrays.append(struct_array_for(field, []))
             else:
                 child_arrays.append(table.column(field.name).combine_chunks())
 
         return pa.Table.from_arrays(child_arrays, schema=cls.schema)
 
     @classmethod
-    def from_flat_dataframe(cls, df: pd.DataFrame):
+    def from_flat_dataframe(cls, df: pd.DataFrame, **kwargs):
         """Load a flattened DataFrame into the Table.
 
         known bug: Doesn't correctly interpret fixed-length lists.
         """
         struct_fields = []
         for field in cls.schema:
             if pa.types.is_struct(field.type):
                 struct_fields.append(field)
 
         if len(struct_fields) == 0:
-            return cls(pa_table=pa.from_dataframe(df, schema=cls.schema))
+            return cls(table=pa.Table.from_pandas(df, schema=cls.schema), **kwargs)
 
         root = pa.field("", pa.struct(cls.schema))
 
         # Walk the schema, and build a StructArray for each embedded
         # type. These are stored in a dictionary, keyed by their
         # dot-separated path. For example, if the schema is:
         #
@@ -346,15 +357,15 @@
 
         table_arrays = []
         for subfield in cls.schema:
             # Pull out the fields of that root-level struct array.
             table_arrays.append(sa.field(subfield.name))
 
         table = pa.Table.from_arrays(table_arrays, schema=cls.schema)
-        return cls(pa_table=table)
+        return cls(table=table, **kwargs)
 
     def flattened_table(self) -> pa.Table:
         """Completely flatten the Table's underlying Arrow table,
         taking into account any nested structure, and return the data
         table itself.
         """
 
@@ -442,21 +453,26 @@
 
     def __repr__(self):
         return f"{self.__class__.__name__}(size={len(self.table)})"
 
     def __len__(self):
         return len(self.table)
 
+    def with_table(self, table: pa.Table) -> Self:
+        return self.__class__(table)
+
     def __getitem__(self, idx):
         # TODO: This comes out a little funky. You get chunked arrays
         # instead of arrays. Is there a way to flatten them safely?
 
         if isinstance(idx, int):
-            return self.__class__(self.table[idx : idx + 1])
-        return self.__class__(self.table[idx])
+            table = self.table[idx : idx + 1]
+        else:
+            table = self.table[idx]
+        return self.with_table(table)
 
     def __iter__(self):
         for i in range(len(self)):
             yield self[i : i + 1]
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, Table):
@@ -472,27 +488,27 @@
     def to_parquet(self, path: str, **kwargs):
         """Write the table to a Parquet file."""
         pyarrow.parquet.write_table(self.table, path, **kwargs)
 
     @classmethod
     def from_parquet(cls, path: str, **kwargs):
         """Read a table from a Parquet file."""
-        return cls(pa_table=pyarrow.parquet.read_table(path, **kwargs))
+        return cls(table=pyarrow.parquet.read_table(path), **kwargs)
 
     def to_feather(self, path: str, **kwargs):
         """Write the table to a Feather file."""
         pyarrow.feather.write_feather(self.table, path, **kwargs)
 
     @classmethod
     def from_feather(cls, path: str, **kwargs):
         """Read a table from a Feather file."""
-        return cls(pa_table=pyarrow.feather.read_table(path, **kwargs))
+        return cls(table=pyarrow.feather.read_table(path), **kwargs)
 
     def to_csv(self, path: str):
         """Write the table to a CSV file. Any nested structure is flattened."""
         pyarrow.csv.write_csv(self.flattened_table(), path)
 
     @classmethod
-    def from_csv(cls, input_file: Union[str, os.PathLike, IOBase]):
+    def from_csv(cls, input_file: Union[str, os.PathLike, IOBase], **kwargs):
         """Read a table from a CSV file."""
         flat_table = pyarrow.csv.read_csv(input_file)
-        return cls(pa_table=cls._unflatten_table(flat_table))
+        return cls(table=cls._unflatten_table(flat_table), **kwargs)
```

### Comparing `quivr-0.2.3/LICENSE` & `quivr-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quivr-0.2.3/README.md` & `quivr-0.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -182,14 +182,55 @@
 
 orbits = load_orbits() # Analogous to the example above
 
 # Compute the determinant of the covariance matrix for each asteroid
 determinants = np.linalg.det(orbits.covariance.matrix)
 ```
 
+### Adding instance attributes
+
+You can also add more attributes (that is, non-Field ones) to your
+class and its instances, but doing so requires a bit more attention.
+
+You can override `__init__` to add instance-level attributes. However,
+if you do this, there are a few rules:
+
+ 1. Your `__init__` method must have an attribute called `table`, with
+    type `pyarrow.Table`, and you must pass this to Table's `__init__`
+    (via `super().__init__(table)`).
+ 2. You must implement a `with_table(self, table: pa.Table) -> Self`
+    method which returns a **new** instance with the provided table,
+    bringing along the current values of all instance attributes.
+
+For example:
+
+```python
+from typing import Self
+
+class AsteroidOrbit(Table):
+    designation = StringField()
+	mass = Float64Field(nullable=True)
+	
+	def __init__(self, table: pa.Table, mu: float):
+	    super().__init__(table)
+		self.mu = mu
+		
+	def with_table(self, table: pa.Table) -> Self:
+        return AsteroidOrbit(table, self.mu)
+```
+
+The `with_table` method will be used in iteration, slicing and
+indexing operations, so try to make it pretty quick.
+
+In addition, note that serialization methods (`to_csv`, `to_feather`,
+and `to_parquet`) will not, by default, bring along your instance
+attributes. If you would like to serialize the instance attributes,
+either override those methods or add additional serialization methods
+of your own, and similarly implement deserializers.
+
 
 ### Filtering
 You can also filter by expressions on the data. See [Arrow
 documentation](https://arrow.apache.org/docs/python/compute.html) for
 more details. You can use this to construct a quivr Table using an
 appropriately-schemaed Arrow Table:
```

### Comparing `quivr-0.2.3/pyproject.toml` & `quivr-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quivr-0.2.3/PKG-INFO` & `quivr-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quivr
-Version: 0.2.3
+Version: 0.3.0
 Summary: Container library for working with tabular Arrow data
 Project-URL: Source, https://github.com/spenczar/quivr
 Author-email: Spencer Nelson <spencer@spencerwnelson.com>
 License-File: LICENSE
 Requires-Python: >=3.11
 Requires-Dist: mmh3
 Requires-Dist: numpy
@@ -196,14 +196,55 @@
 
 orbits = load_orbits() # Analogous to the example above
 
 # Compute the determinant of the covariance matrix for each asteroid
 determinants = np.linalg.det(orbits.covariance.matrix)
 ```
 
+### Adding instance attributes
+
+You can also add more attributes (that is, non-Field ones) to your
+class and its instances, but doing so requires a bit more attention.
+
+You can override `__init__` to add instance-level attributes. However,
+if you do this, there are a few rules:
+
+ 1. Your `__init__` method must have an attribute called `table`, with
+    type `pyarrow.Table`, and you must pass this to Table's `__init__`
+    (via `super().__init__(table)`).
+ 2. You must implement a `with_table(self, table: pa.Table) -> Self`
+    method which returns a **new** instance with the provided table,
+    bringing along the current values of all instance attributes.
+
+For example:
+
+```python
+from typing import Self
+
+class AsteroidOrbit(Table):
+    designation = StringField()
+	mass = Float64Field(nullable=True)
+	
+	def __init__(self, table: pa.Table, mu: float):
+	    super().__init__(table)
+		self.mu = mu
+		
+	def with_table(self, table: pa.Table) -> Self:
+        return AsteroidOrbit(table, self.mu)
+```
+
+The `with_table` method will be used in iteration, slicing and
+indexing operations, so try to make it pretty quick.
+
+In addition, note that serialization methods (`to_csv`, `to_feather`,
+and `to_parquet`) will not, by default, bring along your instance
+attributes. If you would like to serialize the instance attributes,
+either override those methods or add additional serialization methods
+of your own, and similarly implement deserializers.
+
 
 ### Filtering
 You can also filter by expressions on the data. See [Arrow
 documentation](https://arrow.apache.org/docs/python/compute.html) for
 more details. You can use this to construct a quivr Table using an
 appropriately-schemaed Arrow Table:
```

