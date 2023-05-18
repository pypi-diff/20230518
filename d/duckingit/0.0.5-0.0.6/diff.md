# Comparing `tmp/duckingit-0.0.5.tar.gz` & `tmp/duckingit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckingit-0.0.5.tar", last modified: Wed May 17 19:33:55 2023, max compression
+gzip compressed data, was "duckingit-0.0.6.tar", last modified: Thu May 18 08:15:41 2023, max compression
```

## Comparing `duckingit-0.0.5.tar` & `duckingit-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:33:55.557663 duckingit-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 19:33:33.000000 duckingit-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-17 19:33:55.557663 duckingit-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-17 19:33:33.000000 duckingit-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:33:55.557663 duckingit-0.0.5/duckingit/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-17 19:33:33.000000 duckingit-0.0.5/duckingit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-05-17 19:33:33.000000 duckingit-0.0.5/duckingit/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-05-17 19:33:33.000000 duckingit-0.0.5/duckingit/_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-05-17 19:33:33.000000 duckingit-0.0.5/duckingit/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-17 19:33:33.000000 duckingit-0.0.5/duckingit/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-17 19:33:33.000000 duckingit-0.0.5/duckingit/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-05-17 19:33:33.000000 duckingit-0.0.5/duckingit/_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-17 19:33:33.000000 duckingit-0.0.5/duckingit/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-17 19:33:33.000000 duckingit-0.0.5/duckingit/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:33:55.557663 duckingit-0.0.5/duckingit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-17 19:33:55.000000 duckingit-0.0.5/duckingit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-17 19:33:55.000000 duckingit-0.0.5/duckingit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:33:55.000000 duckingit-0.0.5/duckingit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-17 19:33:55.000000 duckingit-0.0.5/duckingit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 19:33:55.000000 duckingit-0.0.5/duckingit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-17 19:33:33.000000 duckingit-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:33:55.557663 duckingit-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:15:41.574917 duckingit-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 08:15:25.000000 duckingit-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-18 08:15:41.570917 duckingit-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-18 08:15:25.000000 duckingit-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:15:41.570917 duckingit-0.0.6/duckingit/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-18 08:15:25.000000 duckingit-0.0.6/duckingit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-05-18 08:15:25.000000 duckingit-0.0.6/duckingit/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-18 08:15:25.000000 duckingit-0.0.6/duckingit/_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-18 08:15:25.000000 duckingit-0.0.6/duckingit/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-18 08:15:25.000000 duckingit-0.0.6/duckingit/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-18 08:15:25.000000 duckingit-0.0.6/duckingit/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-05-18 08:15:25.000000 duckingit-0.0.6/duckingit/_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-18 08:15:25.000000 duckingit-0.0.6/duckingit/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-18 08:15:25.000000 duckingit-0.0.6/duckingit/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:15:41.570917 duckingit-0.0.6/duckingit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-18 08:15:41.000000 duckingit-0.0.6/duckingit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-18 08:15:41.000000 duckingit-0.0.6/duckingit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 08:15:41.000000 duckingit-0.0.6/duckingit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 08:15:41.000000 duckingit-0.0.6/duckingit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 08:15:41.000000 duckingit-0.0.6/duckingit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-18 08:15:25.000000 duckingit-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 08:15:41.574917 duckingit-0.0.6/setup.cfg
```

### Comparing `duckingit-0.0.5/LICENSE` & `duckingit-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.5/PKG-INFO` & `duckingit-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckingit
-Version: 0.0.5
+Version: 0.0.6
 Summary: A framework to leverage clusters of serverless functions for analytics. Powered by DuckDB
 Author-email: Tobias Egelund <egelundtobias@gmail.com>
 Project-URL: Homepage, https://github.com/tobiasegelund/duckingit
 Project-URL: Bug Tracker, https://github.com/tobiasegelund/duckingit/issues
 Keywords: Serverless,DuckDB,Data Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckingit-0.0.5/README.md` & `duckingit-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.5/duckingit/_config.py` & `duckingit-0.0.6/duckingit/_config.py`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.5/duckingit/_controller.py` & `duckingit-0.0.6/duckingit/_controller.py`

 * *Files 15% similar despite different names*

```diff
@@ -72,52 +72,77 @@
             # The order of evaluations matters
             if (
                 last_executed_minutes < self.cache_expiration_time
                 and step.subquery_hashed in cached_objects
             ):
                 execution_stage.tasks.remove(step)
 
-    def execute_plan(self, execution_plan: Plan, prefix: str, default_prefix: str):
-        """Executes the execution plan"""
-        completed = set()
-        queue = set(execution_plan.leaves)
-        # TODO: Can this be moved in the loop, so old dependencies are overwritten?
-        dependencies: dict[str, list[str]] = {}
-
-        while queue:
-            stage = queue.pop()
-
-            for deb in stage.dependents:
-                if deb.id not in completed:
-                    queue.add(deb)
-
-            # for _id in list(dependencies):
-            #     if _id not in stage.dependencies:
-            #         _ = dependencies.pop(_id)
-
-            stage.create_tasks(dependencies=dependencies)
-            if self.verbose:
-                print(f"RUNNING STAGE: [{stage}]")
-
-            if stage.id == execution_plan.root.id and prefix != "":
-                default_prefix = prefix
-
-            dependencies[stage.id] = [f"{default_prefix}/{i}.parquet" for i in stage.output]
-            # self.evaluate_execution_stage(execution_stage=stage, prefix=default_prefix)
-
-            execution_time = datetime.datetime.now()
-            if len(stage.tasks) > 0:
-                request_ids = self.provider.invoke(
-                    execution_tasks=stage.tasks, prefix=default_prefix
+    def execute_stage(
+        self,
+        stage: Stage,
+        dag: dict[Stage, t.Set[Stage]],
+        context: dict[str, list[str]],
+        completed: t.Set[Stage],
+        root_id: str,
+        prefix: str,
+        default_prefix: str,
+    ):
+        for dep in dag[stage]:
+            if dep not in completed:
+                self.execute_stage(
+                    stage=dep,
+                    dag=dag,
+                    context=context,
+                    completed=completed,
+                    root_id=root_id,
+                    prefix=prefix,
+                    default_prefix=default_prefix,
                 )
 
-                self.check_status_of_invokations(request_ids=request_ids)
+        stage_deps = {}
+        for dep in stage.dependencies:
+            if dep.id in context:
+                stage_deps[dep.id] = context[dep.id]
+
+        stage.create_tasks(dependencies=context)
+        if self.verbose:
+            print(f"RUNNING STAGE: [{stage}]")
+
+        if stage.id == root_id and prefix != "":
+            default_prefix = prefix
+
+        context[stage.id] = [f"{default_prefix}/{i}.parquet" for i in stage.output]
+        # self.evaluate_execution_stage(execution_stage=stage, prefix=default_prefix)
+
+        execution_time = datetime.datetime.now()
+        if len(stage.tasks) > 0:
+            request_ids = self.provider.invoke(execution_tasks=stage.tasks, prefix=default_prefix)
 
-            completed.add(stage.id)
-            self.update_cache_metadata(execution_stage=stage, execution_time=execution_time)
+            self.check_status_of_invokations(request_ids=request_ids)
+
+        completed.add(stage)
+        self.update_cache_metadata(execution_stage=stage, execution_time=execution_time)
+
+    def execute_plan(self, execution_plan: Plan, prefix: str, default_prefix: str):
+        """Executes the execution plan"""
+        completed: t.Set[Stage] = set()
+        dag = execution_plan.dag
+        context: dict[str, list[str]] = {}
+
+        for stage in dag:
+            if stage not in completed:
+                self.execute_stage(
+                    stage=stage,
+                    dag=dag,
+                    context=context,
+                    completed=completed,
+                    root_id=execution_plan.root.id,
+                    prefix=prefix,
+                    default_prefix=default_prefix,
+                )
 
     def check_status_of_invokations(self, request_ids: dict[str, Task]):
         cnt = 0
 
         total_tasks = len(request_ids)
         while len(request_ids) > 0:
             # Logic to speed up fast queries
```

### Comparing `duckingit-0.0.5/duckingit/_dataset.py` & `duckingit-0.0.6/duckingit/_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,20 +47,14 @@
             self.OVERWRITE: overwrite,
             self.WRITE: write,
         }
 
         return _funcs[self]  # type: ignore
 
 
-# class Formats(Enum):
-#     DELTA = "delta"
-#     ICEBERG = "iceberg"
-#     HUDI = "hudi"
-
-
 class DatasetWriter:
     _mode: Modes = Modes.WRITE
 
     def __init__(self, session: "DuckSession", dataset: "Dataset") -> None:
         self._session = session
         self._dataset = dataset
```

### Comparing `duckingit-0.0.5/duckingit/_parser.py` & `duckingit-0.0.6/duckingit/_parser.py`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.5/duckingit/_planner.py` & `duckingit-0.0.6/duckingit/_planner.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,77 +73,73 @@
     stage_type: Stages
 
     @classmethod
     def from_ast(
         cls,
         ast: exp.Expression,
         previous_stage: t.Optional["Stage"] = None,
-        root_stage: t.Optional["Stage"] = None,
         cte_stages: dict = {},
     ):
         ast = ast.copy()
 
         with_ = ast.args.get("with")
         if with_:
             ast.find(exp.With).pop()  # type: ignore
 
             cte_stages = cte_stages.copy()
             for cte in with_.expressions:
                 stage = Stage.from_ast(
                     cte.this,
                     previous_stage=previous_stage,
-                    root_stage=root_stage,
                     cte_stages=cte_stages,
                 )
                 stage.alias = cte.alias
 
                 cte_stages[cte.alias] = stage
 
         from_ = ast.args.get("from")
         if isinstance(ast, exp.Select) and from_:
             if len(from_.expressions) > 1:
                 raise NotImplementedError("Multi FROM isn't supported")
             expression = from_.expressions[0]
+            assert expression.this
 
             if isinstance(expression, exp.Subquery):
                 stage = select_stage_type(ast)
                 # id must begin with a character
                 stage.id = create_hash_string(ast.sql(), digits=6, first_char="$")
                 stage.alias = expression.alias
                 stage.ast = ast.copy()  # type: ignore
 
                 if previous_stage is not None:
                     previous_stage.add_dependency(stage)
-                if root_stage is None:
-                    root_stage = stage
 
-                assert expression.this
-
-                stage = Stage.from_ast(
+                sub_stage = Stage.from_ast(
                     expression.this,
                     previous_stage=stage,
-                    root_stage=root_stage,
                     cte_stages=cte_stages,
                 )
-                stage._replace_node(child=expression, id=stage.id, alias=expression.alias)
+                stage.replace_child_with_id(
+                    child=expression, id=sub_stage.id, alias=expression.alias
+                )
 
-            if isinstance(expression, exp.Union):
+            elif isinstance(expression, exp.Union):
                 raise NotImplementedError("Cannot handle Unions yet")
 
             else:
                 table_name = str(expression.this)
 
                 stage = select_stage_type(ast)
                 stage.id = create_hash_string(ast.sql(), digits=6, first_char="$")
                 stage.alias = expression.alias
                 stage.ast = ast.copy()  # type: ignore
 
                 if table_name in cte_stages:
                     cte = cte_stages[table_name]
-                    stage._replace_node(child=expression, id=cte.id, alias=expression.alias)
+                    stage.replace_child_with_id(child=expression, id=cte.id, alias=expression.alias)
                     stage.add_dependency(cte)
 
         else:
             stage = Scan()
 
         joins = ast.args.get("joins")
         if joins:
@@ -153,53 +149,49 @@
                 join = join.this
                 alias = join.alias
 
                 if isinstance(join, exp.Subquery):
                     subquery_stage = Stage.from_ast(
                         join.this,  # type: ignore
                         previous_stage=previous_stage,
-                        root_stage=root_stage,
                         cte_stages=cte_stages,
                     )
-                    stage._replace_node(child=join, id=subquery_stage.id, alias=alias)
+                    stage.replace_child_with_id(child=join, id=subquery_stage.id, alias=alias)
                     stage.add_dependency(subquery_stage)
 
                 else:
                     if (table_name := join.this.sql()) in cte_stages:
                         cte = cte_stages[table_name]
-                        stage._replace_node(child=join, id=cte.id, alias=alias)
+                        stage.replace_child_with_id(child=join, id=cte.id, alias=alias)
                         stage.add_dependency(cte)
 
         if previous_stage is not None:
             previous_stage.add_dependency(stage)
 
-        if root_stage is None:
-            root_stage = stage
-
-        return root_stage
+        return stage
 
     def __init__(self):
         self.id: str = ""
         self.name: str = ""
         self.alias: str = ""  # Properbly to be deleted
         self.ast: exp.Expression | None = None
         self._sql: str = ""
 
-        self.dependents = set()
-        self.dependencies = set()
+        self.dependents: t.Set["Stage"] = set()
+        self.dependencies: t.Set["Stage"] = set()
 
         self.tasks: t.Set[Task] = set()
 
     def __repr__(self) -> str:
         return f"{self.stage_type} - {self.id}: {self.sql}"
 
     def __len__(self) -> int:
         return len(self.tasks)
 
-    def _replace_node(self, child: exp.Expression, id: str, alias: str = "") -> None:
+    def replace_child_with_id(self, child: exp.Expression, id: str, alias: str = "") -> None:
         if self.ast is None:
             raise ValueError
 
         for node, *_ in self.ast.walk():
             if node == child:
                 node.replace(sqlglot.parse_one(f"{id} {alias}"))
 
@@ -300,15 +292,15 @@
     if sort:
         return Sort()
 
     return Scan()
 
 
 class Plan:
-    """Class to create an execution plan across nodes
+    """The execution plan
 
     A execution consists of stages, and each stage consists of tasks. A stage is an actual
     operation, such as Scan, Sort, Join, where a task is the actual DuckDB SQL query to run on
     a serverless function
 
     Attributes:
         query, Query: The main query parsed as in the Query class
@@ -328,22 +320,14 @@
         self._length: int | None = None
 
     def __len__(self) -> int:
         if self._length is None:
             self._length = len([node for node, _ in self.dag.items()])
         return self._length
 
-    @property
-    def leaves(self) -> list[Stage]:
-        leaves = []
-        for node in self.dag:
-            if not self.dag[node]:
-                leaves.append(node)
-        return leaves
-
     @classmethod
     def from_query(cls, query: Query):
         root = Stage.from_ast(ast=query.ast)
 
         dag: dict[Stage, t.Set[Stage]] = {root: set()}
         nodes = {root}
         while nodes:
```

### Comparing `duckingit-0.0.5/duckingit/_session.py` & `duckingit-0.0.6/duckingit/_session.py`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.5/duckingit/_utils.py` & `duckingit-0.0.6/duckingit/_utils.py`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.5/duckingit.egg-info/PKG-INFO` & `duckingit-0.0.6/duckingit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckingit
-Version: 0.0.5
+Version: 0.0.6
 Summary: A framework to leverage clusters of serverless functions for analytics. Powered by DuckDB
 Author-email: Tobias Egelund <egelundtobias@gmail.com>
 Project-URL: Homepage, https://github.com/tobiasegelund/duckingit
 Project-URL: Bug Tracker, https://github.com/tobiasegelund/duckingit/issues
 Keywords: Serverless,DuckDB,Data Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckingit-0.0.5/pyproject.toml` & `duckingit-0.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "duckingit"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   {name="Tobias Egelund", email="egelundtobias@gmail.com" },
 ]
 description = "A framework to leverage clusters of serverless functions for analytics. Powered by DuckDB"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["Serverless", "DuckDB", "Data Engineering"]
```

