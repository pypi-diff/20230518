# Comparing `tmp/hnsqlite-0.2.2.tar.gz` & `tmp/hnsqlite-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnsqlite-0.2.2.tar", last modified: Sun May  7 01:38:27 2023, max compression
+gzip compressed data, was "hnsqlite-0.2.4.tar", last modified: Thu May 18 01:35:22 2023, max compression
```

## Comparing `hnsqlite-0.2.2.tar` & `hnsqlite-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 01:38:27.316337 hnsqlite-0.2.2/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-03-20 17:17:48.000000 hnsqlite-0.2.2/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)     7584 2023-05-07 01:38:27.316063 hnsqlite-0.2.2/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     6980 2023-05-01 19:05:01.000000 hnsqlite-0.2.2/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 01:38:27.313661 hnsqlite-0.2.2/hnsqlite/
--rw-r--r--   0 wsk        (501) staff       (20)      116 2023-03-26 23:42:40.000000 hnsqlite-0.2.2/hnsqlite/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)    30561 2023-05-07 01:27:15.000000 hnsqlite-0.2.2/hnsqlite/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)     4758 2023-03-27 02:41:29.000000 hnsqlite-0.2.2/hnsqlite/filter.py
--rw-r--r--   0 wsk        (501) staff       (20)     1238 2023-03-19 01:38:08.000000 hnsqlite-0.2.2/hnsqlite/util.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 01:38:27.314948 hnsqlite-0.2.2/hnsqlite.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     7584 2023-05-07 01:38:27.000000 hnsqlite-0.2.2/hnsqlite.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      346 2023-05-07 01:38:27.000000 hnsqlite-0.2.2/hnsqlite.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-07 01:38:27.000000 hnsqlite-0.2.2/hnsqlite.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       37 2023-05-07 01:38:27.000000 hnsqlite-0.2.2/hnsqlite.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)        9 2023-05-07 01:38:27.000000 hnsqlite-0.2.2/hnsqlite.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      747 2023-05-07 00:12:17.000000 hnsqlite-0.2.2/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-07 01:38:27.316411 hnsqlite-0.2.2/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 01:38:27.315741 hnsqlite-0.2.2/test/
--rw-r--r--   0 wsk        (501) staff       (20)    12583 2023-05-01 19:05:01.000000 hnsqlite-0.2.2/test/test_collection.py
--rw-r--r--   0 wsk        (501) staff       (20)     2832 2023-05-01 19:05:01.000000 hnsqlite-0.2.2/test/test_collection_filter.py
--rw-r--r--   0 wsk        (501) staff       (20)    12321 2023-03-20 05:54:20.000000 hnsqlite-0.2.2/test/test_filter.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-18 01:35:22.104004 hnsqlite-0.2.4/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-03-20 17:17:48.000000 hnsqlite-0.2.4/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     7584 2023-05-18 01:35:22.103608 hnsqlite-0.2.4/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     6980 2023-05-01 19:05:01.000000 hnsqlite-0.2.4/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-18 01:35:22.079541 hnsqlite-0.2.4/hnsqlite/
+-rw-r--r--   0 wsk        (501) staff       (20)      116 2023-03-26 23:42:40.000000 hnsqlite-0.2.4/hnsqlite/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)    31399 2023-05-18 01:34:17.000000 hnsqlite-0.2.4/hnsqlite/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4758 2023-03-27 02:41:29.000000 hnsqlite-0.2.4/hnsqlite/filter.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1238 2023-03-19 01:38:08.000000 hnsqlite-0.2.4/hnsqlite/util.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-18 01:35:22.101437 hnsqlite-0.2.4/hnsqlite.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     7584 2023-05-18 01:35:22.000000 hnsqlite-0.2.4/hnsqlite.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      346 2023-05-18 01:35:22.000000 hnsqlite-0.2.4/hnsqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-18 01:35:22.000000 hnsqlite-0.2.4/hnsqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       37 2023-05-18 01:35:22.000000 hnsqlite-0.2.4/hnsqlite.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        9 2023-05-18 01:35:22.000000 hnsqlite-0.2.4/hnsqlite.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      747 2023-05-17 01:56:22.000000 hnsqlite-0.2.4/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-18 01:35:22.104097 hnsqlite-0.2.4/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-18 01:35:22.102470 hnsqlite-0.2.4/test/
+-rw-r--r--   0 wsk        (501) staff       (20)    13832 2023-05-18 01:32:00.000000 hnsqlite-0.2.4/test/test_collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2832 2023-05-01 19:05:01.000000 hnsqlite-0.2.4/test/test_collection_filter.py
+-rw-r--r--   0 wsk        (501) staff       (20)    12321 2023-03-20 05:54:20.000000 hnsqlite-0.2.4/test/test_filter.py
```

### Comparing `hnsqlite-0.2.2/LICENSE` & `hnsqlite-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hnsqlite-0.2.2/PKG-INFO` & `hnsqlite-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hnsqlite
-Version: 0.2.2
+Version: 0.2.4
 Summary: A minimalist integration of sqlite and hnswlib focused on providing simple embedding persistence and search for text applications.
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/hnsqlite
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/hnsqlite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `hnsqlite-0.2.2/README.md` & `hnsqlite-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `hnsqlite-0.2.2/hnsqlite/collection.py` & `hnsqlite-0.2.4/hnsqlite/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,15 @@
 
 
 
 class Embedding(BaseModel):
     """
     An Embedding as sent to/from the Collection API
     """
+    id:             Optional[int]   = Field(description='Unique database identifier for a given embedding.')
     vector:         list[float]     = Field(description='The user-supplied vector element as stored as a list of floats. Can be sent in as a numpy array and will be converted to a list of floats.')   
     text:           str             = Field(description="The text that was input to the model to generate this embedding.")
     doc_id:         Optional[str]   = Field(description="An optional document_id associated with the embedding.")
     metadata:       Optional[dict]  = Field(description="An optional dictionary of metadata associated with the text")
     created_at:     float           = Field(default_factory=time, description='The epoch timestamp when the embedding was created.')
 
     def __str__(self) -> str:
@@ -144,15 +145,16 @@
         if self.metadata is not None:
             estr += f"metadata={self.metadata}, "
         estr += f"text='{text}')"
         return estr
     
     @classmethod
     def from_db(cls, db_embedding: dbEmbedding) -> "Embedding":
-        return Embedding(vector=db_embedding.vector_as_list(),
+        return Embedding(id=db_embedding.id,
+                         vector=db_embedding.vector_as_list(),                         
                          text=db_embedding.text,
                          doc_id=db_embedding.doc_id,
                          metadata=db_embedding.metadata_as_dict(),
                          created_at=db_embedding.created_at)
                          
     @root_validator(pre=True)
     def convert_vector(cls, values):
@@ -206,14 +208,16 @@
             _is_valid_namestr(collection_name, 'name')
         if not sqlite_filename:   # find sqlite file if not specified
             sqlite_files = glob.glob("*.sqlite")
             if len(sqlite_files) == 1:
                 sqlite_filename = sqlite_files[0]
                 logger.info(f"using sqlite_filename {sqlite_filename}")
             elif len(sqlite_files) > 1:
+                raise Exception(f"sqlite_filename was not specified and there are multiple sqlite files here: {sqlite_files}.")
+            else:
                 sqlite_filename = 'hnsqlite.sqlite'  # default name
         if not os.path.exists(sqlite_filename):        
             logger.warning(f"sqlite_filename {sqlite_filename} does not exist; create new database")
         else:
             logger.info(f"sqlite_filename {sqlite_filename} exists; using existing database")
         db_engine = create_engine(f'sqlite:///{sqlite_filename}')
         SQLModel.metadata.create_all(db_engine)                    
@@ -509,14 +513,24 @@
             docs_dl[doc_id].sort(key=lambda e: e.created_at)
         if max_per_doc is None:
             docs = [docs_dl[doc_id] for doc_id in docs_dl]
         else:
             docs = [docs_dl[doc_id][:max_per_doc] for doc_id in docs_dl]
         return docs, index
 
+    def get_embedding_by_id(self, id: int) -> Embedding:
+        """
+        get a specific embedding by its unique numeric id
+        """
+        with Session(self.db_engine) as session:
+            e = session.get(dbEmbedding, id)
+            if not e or e.collection_id != self.config.id:
+                raise ValueError(f"Invalid id: {id}")
+            return Embedding.from_db(e)
+        
     def search(self, vector: np.array, k = 12, filter=None) -> List[SearchResponse]:        
         """
         query the hnsw index for the nearest neighbors of the given vector
         unlike hnswlib which takes a 2D array of vectors, this method takes a single vector
         since the common use case for this in production is searching for a single vector at a time
         """
         if isinstance(vector, list):
@@ -574,15 +588,18 @@
             return
         count = 0           
         if doc_ids:        
             logger.info(f"deleting doc_ids {doc_ids} from {self.config.name}")
             with Session(self.db_engine) as session:
                 for embedding in session.exec(select(dbEmbedding).where(dbEmbedding.collection_id == self.config.id).where(dbEmbedding.doc_id.in_(doc_ids))):
                     count += 1
-                    self.hnsw_ix.mark_deleted(embedding.id)
+                    try:
+                        self.hnsw_ix.mark_deleted(embedding.id)
+                    except RuntimeError as e: 
+                        logger.warning(e)
                     session.delete(embedding)
                 session.commit()
         elif filter:
             logger.info(f"deleting items from {self.config.name} with filter: {filter}")
             with Session(self.db_engine) as session:
                 for embedding in session.exec(select(dbEmbedding).where(dbEmbedding.collection_id == self.config.id)).all():
                     if filter_item(filter, embedding.metadata_as_dict()):
```

### Comparing `hnsqlite-0.2.2/hnsqlite/filter.py` & `hnsqlite-0.2.4/hnsqlite/filter.py`

 * *Files identical despite different names*

### Comparing `hnsqlite-0.2.2/hnsqlite/util.py` & `hnsqlite-0.2.4/hnsqlite/util.py`

 * *Files identical despite different names*

### Comparing `hnsqlite-0.2.2/hnsqlite.egg-info/PKG-INFO` & `hnsqlite-0.2.4/hnsqlite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hnsqlite
-Version: 0.2.2
+Version: 0.2.4
 Summary: A minimalist integration of sqlite and hnswlib focused on providing simple embedding persistence and search for text applications.
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/hnsqlite
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/hnsqlite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `hnsqlite-0.2.2/pyproject.toml` & `hnsqlite-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hnsqlite"
-version = "0.2.2"
+version = "0.2.4"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['sqlmodel', 'hnswlib', 'psutil', 'numpy', 'loguru']
 description = "A minimalist integration of sqlite and hnswlib focused on providing simple embedding persistence and search for text applications."
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `hnsqlite-0.2.2/test/test_collection.py` & `hnsqlite-0.2.4/test/test_collection.py`

 * *Files 8% similar despite different names*

```diff
@@ -289,9 +289,39 @@
             self.assertEqual(len(embeddings2), 7)
             for i, e in enumerate(embeddings2):
                 self.assertEqual(e.text, f"Collection2 text {i}")
                 self.assertTrue(np.allclose(e.vector_as_array(), self.vectors2[i], rtol=tolerance, atol=tolerance))
 
 
 
+                
+class TestGetEmbeddingById(unittest.TestCase):
+    @classmethod
+    def setUpClass(cls):
+        cls.collection = Collection(collection_name="test-collection-id", dimension=128)
+        vectors = [np.random.rand(128) for _ in range(3)]
+        texts = ["id text1", "id text2", "id text3"]
+        cls.collection.add_items(vectors, texts)
+
+    @classmethod
+    def tearDownClass(cls):
+        cls.collection.delete(delete_all=True)
+        for f in os.listdir("."):
+            if f.endswith('.sqlite'):
+                os.remove(f)
+            if f.endswith('.hnsw'):
+                os.remove(f) 
+
+    def test_get_embedding_by_id(self):
+        # Get Embedding using the get_embeddings() method to compare
+        target_embedding = self.collection.get_embeddings(start=0, limit=1, reverse=False)[0]
+
+        # Get Embedding using the new get_embedding_by_id() method
+        result_embedding = self.collection.get_embedding_by_id(target_embedding.id)
+        
+        # Check if the embeddings are the same
+        self.assertEqual(result_embedding.text, target_embedding.text)
+        self.assertEqual(result_embedding.vector, target_embedding.vector)
+        self.assertEqual(result_embedding.doc_id, target_embedding.doc_id)
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `hnsqlite-0.2.2/test/test_collection_filter.py` & `hnsqlite-0.2.4/test/test_collection_filter.py`

 * *Files identical despite different names*

### Comparing `hnsqlite-0.2.2/test/test_filter.py` & `hnsqlite-0.2.4/test/test_filter.py`

 * *Files identical despite different names*

