# Comparing `tmp/usearch-0.2.4-cp39-cp39-win_amd64.whl.zip` & `tmp/usearch-0.3.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 132841 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-17 16:23 usearch/__init__.py
--rw-rw-rw-  2.0 fat     1051 b- defN 23-May-17 16:23 usearch/client.py
--rw-rw-rw-  2.0 fat   270848 b- defN 23-May-17 16:35 usearch/index.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2298 b- defN 23-May-17 16:23 usearch/io.py
--rw-rw-rw-  2.0 fat     1203 b- defN 23-May-17 16:23 usearch/server.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-17 16:35 usearch-0.2.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    19110 b- defN 23-May-17 16:35 usearch-0.2.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-17 16:35 usearch-0.2.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-17 16:35 usearch-0.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      770 b- defN 23-May-17 16:35 usearch-0.2.4.dist-info/RECORD
-10 files, 306946 bytes uncompressed, 131545 bytes compressed:  57.1%
+Zip file size: 132686 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-17 22:28 usearch/__init__.py
+-rw-rw-rw-  2.0 fat     1051 b- defN 23-May-17 22:28 usearch/client.py
+-rw-rw-rw-  2.0 fat   273408 b- defN 23-May-17 22:40 usearch/index.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2298 b- defN 23-May-17 22:28 usearch/io.py
+-rw-rw-rw-  2.0 fat     1203 b- defN 23-May-17 22:28 usearch/server.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-17 22:40 usearch-0.3.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    19489 b- defN 23-May-17 22:40 usearch-0.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-17 22:40 usearch-0.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-17 22:40 usearch-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      770 b- defN 23-May-17 22:40 usearch-0.3.0.dist-info/RECORD
+10 files, 309885 bytes uncompressed, 131390 bytes compressed:  57.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: usearch/io.py
 Comment: 
 
 Filename: usearch/server.py
 Comment: 
 
-Filename: usearch-0.2.4.dist-info/LICENSE
+Filename: usearch-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: usearch-0.2.4.dist-info/METADATA
+Filename: usearch-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: usearch-0.2.4.dist-info/WHEEL
+Filename: usearch-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: usearch-0.2.4.dist-info/top_level.txt
+Filename: usearch-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: usearch-0.2.4.dist-info/RECORD
+Filename: usearch-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `usearch-0.2.4.dist-info/LICENSE` & `usearch-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `usearch-0.2.4.dist-info/METADATA` & `usearch-0.3.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usearch
-Version: 0.2.4
+Version: 0.3.0
 Summary: Smaller & Faster Single-File Vector Search Engine from Unum
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
@@ -100,39 +100,39 @@
 > connectivity `M=16`,
 > expansion @ construction `efConstruction=128`,
 > and expansion @ search `ef=64`.
 > Both libraries were compiled for the target architecture.
 > Jump to the [Performance Tuning][benchmarking] section to read about the effects of those hyper-parameters.
 
 [sloc]: https://en.wikipedia.org/wiki/Source_lines_of_code
-[benchmarking]: https://github.com/unum-cloud/usearch
+[benchmarking]: https://github.com/unum-cloud/usearch/blob/main/docs/benchmarks.md
 
 ## User-Defined Functions
 
 Most vector-search packages focus on just 2 metrics - "Inner Product distance" and "Euclidean distance".
 That only partially exhausts the list of possible metrics.
 A good example would be the rare [Haversine][haversine] distance, used to compute the distance between geo-spatial coordinates, extending Vector Search into the GIS domain.
 Another example would be designing a custom metric for **composite embeddings** concatenated from multiple AI models in real-world applications. 
 USearch supports that: [Python](#user-defined-functions-in-python) and [C++](#user-defined-functions-in-c) examples.
 
-![USearch: Vector Search Approaches](assets/usearch-approaches-white.png)
+![USearch: Vector Search Approaches](https://github.com/unum-cloud/usearch/blob/main/assets/usearch-approaches-white.png?raw=true)
 
 Unlike older approaches indexing high-dimensional spaces, like KD-Trees and Locality Sensitive Hashing, HNSW doesn't require vectors to be identical in length.
 They only have to be comparable.
 So you can apply it in [obscure][obscure] applications, like searching for similar sets or fuzzy text matching.
 
 [haversine]: https://ashvardanian.com/posts/abusing-vector-search#geo-spatial-indexing
 [obscure]: https://ashvardanian.com/posts/abusing-vector-search
 
 ## Memory Efficiency, Downcasting, and Quantization
 
 Training a quantization model and dimension-reduction is a common approach to accelerate vector search.
 Those, however, are only sometimes reliable, can significantly affect the statistical properties of your data, and require regular adjustments if your distribution shifts.
 
-![USearch uint40_t support](assets/usearch-neighbor-types.png)
+![USearch uint40_t support](https://github.com/unum-cloud/usearch/blob/main/assets/usearch-neighbor-types.png?raw=true)
 
 Instead, we have focused on high-precision arithmetic over low-precision downcasted vectors.
 The same index, and `add` and `search` operations will automatically down-cast or up-cast between `f32_t`, `f16_t`, `f64_t`, and `f8_t` representations, even if the hardware doesn't natively support it.
 Continuing the topic of memory-efficiency, we provide a `uint40_t` to allow collection with over 4B+ vectors without allocating 8 bytes for every neighbor reference in the proximity graph.
 
 ## View Larger Indexes from Disk
 
@@ -223,23 +223,23 @@
 - `ip_gt<scalar_t>` for "Inner Product" or "Dot Product" distance.
 - `l2sq_gt<scalar_t>` for the squared "L2" or "Euclidean" distance.
 - `jaccard_gt<scalar_t>` for "Jaccard" distance between two ordered sets of unique elements.
 - `bit_hamming_gt<scalar_t>` for "Hamming" distance, as the number of shared bits in hashes.
 - `pearson_correlation_gt<scalar_t>` for "Pearson" correlation between probability distributions.
 - `haversine_gt<scalar_t>` for "Haversine" or "Great Circle" distance between coordinates.
 
-#### Bring your Threads
+#### Multi-Threading
 
 Most AI, HPC, or Big Data packages use some form of a thread pool.
 Instead of spawning additional threads within USearch, we focus on the thread safety of `add()` function, simplifying resource management.
 
 ```cpp
 #pragma omp parallel for
     for (std::size_t i = 0; i < n; ++i)
-        native.add(label, span_t{vector, dims}, omp_get_thread_num());
+        native.add(label, span_t{vector, dims}, add_config_t { .thread = omp_get_thread_num() });
 ```
 
 During initialization, we allocate enough temporary memory for all the cores on the machine.
 On the call, the user can supply the identifier of the current thread, making this library easy to integrate with OpenMP and similar tools.
 
 ### Python
 
@@ -401,14 +401,22 @@
 assert_eq!(index.size(), 2);
 
 // Read back the tags
 let results = index.search(&first, 10).unwrap();
 assert_eq!(results.count, 2);
 ```
 
+#### Multi-Threading
+
+```rust
+assert!(index.add_in_thread(42, &first, 0).is_ok());
+assert!(index.add_in_thread(43, &second, 0).is_ok());
+let results = index.search_in_thread(&first, 10, 0).unwrap();
+```
+
 Being a systems-programming language, Rust has better control over memory management and concurrency but lacks function overloading.
 Aside from the `add` and `search`, USearch Rust binding also provides `add_in_thread` and `search_in_thread`, which let users identify the calling thread to use underlying temporary memory more efficiently.
 
 #### Serialization
 
 ```rust
 assert!(index.save("index.usearch").is_ok());
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: usearch Version: 0.2.4 Summary: Smaller & Faster
+Metadata-Version: 2.1 Name: usearch Version: 0.3.0 Summary: Smaller & Faster
 Single-File Vector Search Engine from Unum License: Apache-2.0 Classifier:
 Development Status :: 4 - Beta Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: C++ Classifier: Operating System :: MacOS Classifier:
@@ -51,61 +51,64 @@
 99.2% | 98% | **99.2%** | > Dataset: 1M vectors sample of the Deep1B dataset. >
 Hardware: `c7g.metal` AWS instance with 64 cores and DDR5 memory. > HNSW was
 configured with identical hyper-parameters: > connectivity `M=16`, > expansion
 @ construction `efConstruction=128`, > and expansion @ search `ef=64`. > Both
 libraries were compiled for the target architecture. > Jump to the [Performance
 Tuning][benchmarking] section to read about the effects of those hyper-
 parameters. [sloc]: https://en.wikipedia.org/wiki/Source_lines_of_code
-[benchmarking]: https://github.com/unum-cloud/usearch ## User-Defined Functions
-Most vector-search packages focus on just 2 metrics - "Inner Product distance"
-and "Euclidean distance". That only partially exhausts the list of possible
-metrics. A good example would be the rare [Haversine][haversine] distance, used
-to compute the distance between geo-spatial coordinates, extending Vector
-Search into the GIS domain. Another example would be designing a custom metric
-for **composite embeddings** concatenated from multiple AI models in real-world
-applications. USearch supports that: [Python](#user-defined-functions-in-
-python) and [C++](#user-defined-functions-in-c) examples. ![USearch: Vector
-Search Approaches](assets/usearch-approaches-white.png) Unlike older approaches
-indexing high-dimensional spaces, like KD-Trees and Locality Sensitive Hashing,
-HNSW doesn't require vectors to be identical in length. They only have to be
-comparable. So you can apply it in [obscure][obscure] applications, like
-searching for similar sets or fuzzy text matching. [haversine]: https://
-ashvardanian.com/posts/abusing-vector-search#geo-spatial-indexing [obscure]:
-https://ashvardanian.com/posts/abusing-vector-search ## Memory Efficiency,
-Downcasting, and Quantization Training a quantization model and dimension-
-reduction is a common approach to accelerate vector search. Those, however, are
-only sometimes reliable, can significantly affect the statistical properties of
-your data, and require regular adjustments if your distribution shifts. !
-[USearch uint40_t support](assets/usearch-neighbor-types.png) Instead, we have
-focused on high-precision arithmetic over low-precision downcasted vectors. The
-same index, and `add` and `search` operations will automatically down-cast or
-up-cast between `f32_t`, `f16_t`, `f64_t`, and `f8_t` representations, even if
-the hardware doesn't natively support it. Continuing the topic of memory-
-efficiency, we provide a `uint40_t` to allow collection with over 4B+ vectors
-without allocating 8 bytes for every neighbor reference in the proximity graph.
-## View Larger Indexes from Disk Modern search systems often suggest using
-different servers to maximize indexing speed and minimize serving costs.
-Memory-optimized for the first task, and storage-optimized for the second, if
-the index can be served from external memory, which USearch can. | | To Build |
-To Serve | | :------- | :-------------: | :--------------------: | | Instance |
-u-24tb1.metal | is4gen.8xlarge | | Price | ~ $200/h | ~$4.5/h | | Memory | 24
-TB RAM + EBS | 192 GB RAM + 30 TB SSD | There is a 50x difference between the
-cost of such instances for identical capacity. Of course, the latency of
-external memory access will be higher, but it is in part compensated with an
-excellent prefetching mechanism. ## Usage There are two usage patters: 1. Bare-
-bones with `usearch/usearch.hpp`, only available in C++. 2. Full-fat version
-with it's own threads, mutexes, type-punning, quantization, that is available
-both in C++ and is wrapped for higher-level bindings. ### C++ #### Installation
-To use in a C++ project simply copy the `include/usearch/usearch.hpp` header
-into your project. Alternatively fetch it with CMake: ```cmake
-FetchContent_Declare(usearch GIT_REPOSITORY https://github.com/unum-cloud/
-usearch.git) FetchContent_MakeAvailable(usearch) ``` #### Quickstart Once
-included, the low-level C++11 interface is as simple as it gets: `reserve()`,
-`add()`, `search()`, `size()`, `capacity()`, `save()`, `load()`, `view()`. This
-covers 90% of use-cases. ```c++ using namespace unum::usearch; index_gt
+[benchmarking]: https://github.com/unum-cloud/usearch/blob/main/docs/
+benchmarks.md ## User-Defined Functions Most vector-search packages focus on
+just 2 metrics - "Inner Product distance" and "Euclidean distance". That only
+partially exhausts the list of possible metrics. A good example would be the
+rare [Haversine][haversine] distance, used to compute the distance between geo-
+spatial coordinates, extending Vector Search into the GIS domain. Another
+example would be designing a custom metric for **composite embeddings**
+concatenated from multiple AI models in real-world applications. USearch
+supports that: [Python](#user-defined-functions-in-python) and [C++](#user-
+defined-functions-in-c) examples. ![USearch: Vector Search Approaches](https://
+github.com/unum-cloud/usearch/blob/main/assets/usearch-approaches-
+white.png?raw=true) Unlike older approaches indexing high-dimensional spaces,
+like KD-Trees and Locality Sensitive Hashing, HNSW doesn't require vectors to
+be identical in length. They only have to be comparable. So you can apply it in
+[obscure][obscure] applications, like searching for similar sets or fuzzy text
+matching. [haversine]: https://ashvardanian.com/posts/abusing-vector-
+search#geo-spatial-indexing [obscure]: https://ashvardanian.com/posts/abusing-
+vector-search ## Memory Efficiency, Downcasting, and Quantization Training a
+quantization model and dimension-reduction is a common approach to accelerate
+vector search. Those, however, are only sometimes reliable, can significantly
+affect the statistical properties of your data, and require regular adjustments
+if your distribution shifts. ![USearch uint40_t support](https://github.com/
+unum-cloud/usearch/blob/main/assets/usearch-neighbor-types.png?raw=true)
+Instead, we have focused on high-precision arithmetic over low-precision
+downcasted vectors. The same index, and `add` and `search` operations will
+automatically down-cast or up-cast between `f32_t`, `f16_t`, `f64_t`, and
+`f8_t` representations, even if the hardware doesn't natively support it.
+Continuing the topic of memory-efficiency, we provide a `uint40_t` to allow
+collection with over 4B+ vectors without allocating 8 bytes for every neighbor
+reference in the proximity graph. ## View Larger Indexes from Disk Modern
+search systems often suggest using different servers to maximize indexing speed
+and minimize serving costs. Memory-optimized for the first task, and storage-
+optimized for the second, if the index can be served from external memory,
+which USearch can. | | To Build | To Serve | | :------- | :-------------: | :--
+------------------: | | Instance | u-24tb1.metal | is4gen.8xlarge | | Price | ~
+$200/h | ~$4.5/h | | Memory | 24 TB RAM + EBS | 192 GB RAM + 30 TB SSD | There
+is a 50x difference between the cost of such instances for identical capacity.
+Of course, the latency of external memory access will be higher, but it is in
+part compensated with an excellent prefetching mechanism. ## Usage There are
+two usage patters: 1. Bare-bones with `usearch/usearch.hpp`, only available in
+C++. 2. Full-fat version with it's own threads, mutexes, type-punning,
+quantization, that is available both in C++ and is wrapped for higher-level
+bindings. ### C++ #### Installation To use in a C++ project simply copy the
+`include/usearch/usearch.hpp` header into your project. Alternatively fetch it
+with CMake: ```cmake FetchContent_Declare(usearch GIT_REPOSITORY https://
+github.com/unum-cloud/usearch.git) FetchContent_MakeAvailable(usearch) ``` ####
+Quickstart Once included, the low-level C++11 interface is as simple as it
+gets: `reserve()`, `add()`, `search()`, `size()`, `capacity()`, `save()`, `load
+()`, `view()`. This covers 90% of use-cases. ```c++ using namespace unum::
+usearch; index_gt
 float>> index; float vec[3] = {0.1, 0.3, 0.2}; index.reserve(10); index.add(/
 * label: */ 42, /* vector: */ {&vec, 3}); index.search( /* query: */ {&vec, 3},
 /* top */ 5 /* results */, /* with callback: */ [](std::size_t label, float
 distance) { }); ``` The `add` is thread-safe for concurrent index construction.
 #### Serialization ```c++ index.save("index.usearch"); index.load
 ("index.usearch"); // Copying from disk index.view("index.usearch"); // Memory-
 mapping from disk ``` #### User-Defined Metrics in C++ For advanced users, more
@@ -120,106 +123,109 @@
 size_t a_length, std::size_t b_length) const; }; ``` The following distances
 are pre-packaged: - `cos_gt` for "Cosine" or "Angular" distance. - `ip_gt` for
 "Inner Product" or "Dot Product" distance. - `l2sq_gt` for the squared "L2" or
 "Euclidean" distance. - `jaccard_gt` for "Jaccard" distance between two ordered
 sets of unique elements. - `bit_hamming_gt` for "Hamming" distance, as the
 number of shared bits in hashes. - `pearson_correlation_gt` for "Pearson"
 correlation between probability distributions. - `haversine_gt` for "Haversine"
-or "Great Circle" distance between coordinates. #### Bring your Threads Most
-AI, HPC, or Big Data packages use some form of a thread pool. Instead of
-spawning additional threads within USearch, we focus on the thread safety of
-`add()` function, simplifying resource management. ```cpp #pragma omp parallel
-for for (std::size_t i = 0; i < n; ++i) native.add(label, span_t{vector, dims},
-omp_get_thread_num()); ``` During initialization, we allocate enough temporary
-memory for all the cores on the machine. On the call, the user can supply the
-identifier of the current thread, making this library easy to integrate with
-OpenMP and similar tools. ### Python #### Installation ```sh pip install
-usearch ``` #### Quickstart ```python import numpy as np from usearch.index
-import Index index = Index( ndim=3, # Define the number of dimensions in input
-vectors metric='cos', # Choose 'l2', 'haversine' or other metric, default =
-'ip' dtype='f32', # Quantize to 'f16' or 'f8' if needed, default = 'f32'
-connectivity=16, # How frequent should the connections in the graph be,
-optional expansion_add=128, # Control the recall of indexing, optional
-expansion_search=64, # Control the quality of search, optional ) vector =
-np.array([0.2, 0.6, 0.4], dtype=np.float32) index.add(42, vector) matches,
-distances, count = index.search(vector, 10) assert len(index) == 1 assert count
-== 1 assert matches[0] == 42 assert distances[0] <= 0.001 ``` Python bindings
-are implemented with [`pybind/pybind11`](https://github.com/pybind/pybind11).
-Assuming the presence of Global Interpreter Lock in Python, we spawn threads in
-the C++ layer on large insertions. #### Serialization ```py index.save
-('index.usearch') index.load('index.usearch') # Copy the whole index into
-memory index.view('index.usearch') # View from disk without loading in memory
-``` #### Batch Operations Adding or querying a batch of entries is identical to
-adding a single vector. The difference would be in the shape of the tensors.
-```py n = 100 labels = np.array(range(n), dtype=np.longlong) vectors =
-np.random.uniform(0, 0.3, (n, index.ndim)).astype(np.float32) index.add(labels,
-vectors, threads=..., copy=...) matches, distances, counts = index.search
-(vectors, 10, threads=...) assert matches.shape[0] == vectors.shape[0] assert
-counts[0] <= 10 ``` You can also override the default `threads` and `copy`
-arguments in bulk workloads. The first controls the number of threads spawned
-for the task. The second controls whether the vector itself will be persisted
-inside the index. If you can preserve the lifetime of the vector somewhere
-else, you can avoid the copy. #### User-Defined Metrics in Python Assuming the
-language boundary exists between Python user code and C++ implementation, there
-are more efficient solutions than passing a Python callable to the engine.
-Luckily, with the help of [Numba][numba], we can JIT compile a function with a
-matching signature and pass it down to the engine. ```py from numba import
-cfunc, types, carray signature = types.float32( types.CPointer(types.float32),
-types.CPointer(types.float32), types.size_t, types.size_t) @cfunc(signature)
-def python_dot(a, b, n, m): a_array = carray(a, n) b_array = carray(b, n) c =
-0.0 for i in range(n): c += a_array[i] * b_array[i] return c index = Index
-(ndim=ndim, metric_pointer=python_dot.address) ``` [numba]: https://
-numba.readthedocs.io/en/stable/reference/jit-compilation.html#c-callbacks ####
-Tooling ```py from usearch.index import Index from usearch.io import
-load_matrix, save_matrix vectors = load_matrix('deep1B.fbin') index = Index
-(ndim=vectors.shape[1]) index.add(labels, vectors) ``` ### JavaScript ####
-Installation ```sh npm install usearch ``` #### Quickstart ```js var index =
-new usearch.Index({ metric: 'cos', connectivity: 16, dimensions: 3 }) index.add
-(42, new Float32Array([0.2, 0.6, 0.4])) var results = index.search(new
-Float32Array([0.2, 0.6, 0.4]), 10) assert.equal(index.size(), 1)
-assert.deepEqual(results.labels, new Uint32Array([42])) assert.deepEqual
-(results.distances, new Float32Array([0])) ``` #### Serialization ```js
-index.save('index.usearch') index.load('index.usearch') index.view
-('index.usearch') ``` ### Rust #### Installation ```sh cargo add usearch ```
-#### Quickstart ```rust let quant: &str = "f16"; let index = new_ip(3, &quant,
-0, 0, 0).unwrap(); assert!(index.reserve(10).is_ok()); assert!(index.capacity()
->= 10); assert!(index.connectivity() != 0); assert_eq!(index.dimensions(), 3);
-assert_eq!(index.size(), 0); let first: [f32; 3] = [0.2, 0.1, 0.2]; let second:
-[f32; 3] = [0.2, 0.1, 0.2]; assert!(index.add(42, &first).is_ok()); assert!
-(index.add(43, &second).is_ok()); assert_eq!(index.size(), 2); // Read back the
-tags let results = index.search(&first, 10).unwrap(); assert_eq!(results.count,
-2); ``` Being a systems-programming language, Rust has better control over
-memory management and concurrency but lacks function overloading. Aside from
-the `add` and `search`, USearch Rust binding also provides `add_in_thread` and
-`search_in_thread`, which let users identify the calling thread to use
-underlying temporary memory more efficiently. #### Serialization ```rust
-assert!(index.save("index.usearch").is_ok()); assert!(index.load
-("index.usearch").is_ok()); assert!(index.view("index.usearch").is_ok()); ```
-#### Metrics ```rust assert!(new_l2(3, &quant, 0, 0, 0).is_ok()); assert!
-(new_cos(3, &quant, 0, 0, 0).is_ok()); assert!(new_haversine(&quant, 0, 0,
-0).is_ok()); ``` ### Java #### Installation ```xml  cloud.unum.usearch usearch
-0.2.3  ``` Add that snippet to your `pom.xml` and hit `mvn install`. ####
-Quickstart ```java Index index = new Index.Config().metric("cos").dimensions
-(2).build(); float vec[] = {10, 20}; index.add(42, vec); int[] labels =
-index.search(vec, 5); ``` ### Swift #### Installation ```txt https://
-github.com/unum-cloud/usearch ``` #### Quickstart ```swift let index = Index.l2
-(dimensions: 3, connectivity: 8) let vectorA: [Float32] = [0.3, 0.5, 1.2] let
-vectorB: [Float32] = [0.4, 0.2, 1.2] index.add(label: 42, vector: vectorA[...])
-index.add(label: 43, vector: vectorB[...]) let results = index.search(vector:
-vectorA[...], count: 10) assert(results.0[0] == 42) ``` ### GoLang ### Wolfram
-## TODO - JavaScript: Allow calling from "worker threads". - Rust: Allow
-passing a custom thread ID. - C# .NET bindings. ## AI + Vector Search =
-Semantic Search AI has a growing number of applications, but one of the coolest
-classic ideas is to use it for Semantic Search. One can take an encoder model,
-like the multi-modal UForm, and a web-programming framework, like UCall, and
-build an image search platform in just 20 lines of Python. ```python import
-ucall.rich_posix as ucall import uform from usearch.index import Index import
-numpy as np from PIL import Image server = ucall.Server() model =
-uform.get_model('unum-cloud/uform-vl-multilingual') index = Index(ndim=256)
-@server def add(label: int, photo: Image.Image): image = model.preprocess_image
-(photo) vector = model.encode_image(image).detach().numpy() index.add(label,
-vector.flatten(), copy=True) @server def search(query: str) -> np.ndarray:
-tokens = model.preprocess_text(query) vector = model.encode_text(tokens).detach
-().numpy() neighbors, _, _ = index.search(vector.flatten(), 3) return neighbors
-server.run() ``` Check [that](https://github.com/ashvardanian/image-search) and
-[other](https://github.com/unum-cloud/examples) examples on our corporate
-GitHub ð¤
+or "Great Circle" distance between coordinates. #### Multi-Threading Most AI,
+HPC, or Big Data packages use some form of a thread pool. Instead of spawning
+additional threads within USearch, we focus on the thread safety of `add()`
+function, simplifying resource management. ```cpp #pragma omp parallel for for
+(std::size_t i = 0; i < n; ++i) native.add(label, span_t{vector, dims},
+add_config_t { .thread = omp_get_thread_num() }); ``` During initialization, we
+allocate enough temporary memory for all the cores on the machine. On the call,
+the user can supply the identifier of the current thread, making this library
+easy to integrate with OpenMP and similar tools. ### Python #### Installation
+```sh pip install usearch ``` #### Quickstart ```python import numpy as np from
+usearch.index import Index index = Index( ndim=3, # Define the number of
+dimensions in input vectors metric='cos', # Choose 'l2', 'haversine' or other
+metric, default = 'ip' dtype='f32', # Quantize to 'f16' or 'f8' if needed,
+default = 'f32' connectivity=16, # How frequent should the connections in the
+graph be, optional expansion_add=128, # Control the recall of indexing,
+optional expansion_search=64, # Control the quality of search, optional )
+vector = np.array([0.2, 0.6, 0.4], dtype=np.float32) index.add(42, vector)
+matches, distances, count = index.search(vector, 10) assert len(index) == 1
+assert count == 1 assert matches[0] == 42 assert distances[0] <= 0.001 ```
+Python bindings are implemented with [`pybind/pybind11`](https://github.com/
+pybind/pybind11). Assuming the presence of Global Interpreter Lock in Python,
+we spawn threads in the C++ layer on large insertions. #### Serialization ```py
+index.save('index.usearch') index.load('index.usearch') # Copy the whole index
+into memory index.view('index.usearch') # View from disk without loading in
+memory ``` #### Batch Operations Adding or querying a batch of entries is
+identical to adding a single vector. The difference would be in the shape of
+the tensors. ```py n = 100 labels = np.array(range(n), dtype=np.longlong)
+vectors = np.random.uniform(0, 0.3, (n, index.ndim)).astype(np.float32)
+index.add(labels, vectors, threads=..., copy=...) matches, distances, counts =
+index.search(vectors, 10, threads=...) assert matches.shape[0] == vectors.shape
+[0] assert counts[0] <= 10 ``` You can also override the default `threads` and
+`copy` arguments in bulk workloads. The first controls the number of threads
+spawned for the task. The second controls whether the vector itself will be
+persisted inside the index. If you can preserve the lifetime of the vector
+somewhere else, you can avoid the copy. #### User-Defined Metrics in Python
+Assuming the language boundary exists between Python user code and C++
+implementation, there are more efficient solutions than passing a Python
+callable to the engine. Luckily, with the help of [Numba][numba], we can JIT
+compile a function with a matching signature and pass it down to the engine.
+```py from numba import cfunc, types, carray signature = types.float32
+( types.CPointer(types.float32), types.CPointer(types.float32), types.size_t,
+types.size_t) @cfunc(signature) def python_dot(a, b, n, m): a_array = carray(a,
+n) b_array = carray(b, n) c = 0.0 for i in range(n): c += a_array[i] * b_array
+[i] return c index = Index(ndim=ndim, metric_pointer=python_dot.address) ```
+[numba]: https://numba.readthedocs.io/en/stable/reference/jit-
+compilation.html#c-callbacks #### Tooling ```py from usearch.index import Index
+from usearch.io import load_matrix, save_matrix vectors = load_matrix
+('deep1B.fbin') index = Index(ndim=vectors.shape[1]) index.add(labels, vectors)
+``` ### JavaScript #### Installation ```sh npm install usearch ``` ####
+Quickstart ```js var index = new usearch.Index({ metric: 'cos', connectivity:
+16, dimensions: 3 }) index.add(42, new Float32Array([0.2, 0.6, 0.4])) var
+results = index.search(new Float32Array([0.2, 0.6, 0.4]), 10) assert.equal
+(index.size(), 1) assert.deepEqual(results.labels, new Uint32Array([42]))
+assert.deepEqual(results.distances, new Float32Array([0])) ``` ####
+Serialization ```js index.save('index.usearch') index.load('index.usearch')
+index.view('index.usearch') ``` ### Rust #### Installation ```sh cargo add
+usearch ``` #### Quickstart ```rust let quant: &str = "f16"; let index = new_ip
+(3, &quant, 0, 0, 0).unwrap(); assert!(index.reserve(10).is_ok()); assert!
+(index.capacity() >= 10); assert!(index.connectivity() != 0); assert_eq!
+(index.dimensions(), 3); assert_eq!(index.size(), 0); let first: [f32; 3] =
+[0.2, 0.1, 0.2]; let second: [f32; 3] = [0.2, 0.1, 0.2]; assert!(index.add(42,
+&first).is_ok()); assert!(index.add(43, &second).is_ok()); assert_eq!
+(index.size(), 2); // Read back the tags let results = index.search(&first,
+10).unwrap(); assert_eq!(results.count, 2); ``` #### Multi-Threading ```rust
+assert!(index.add_in_thread(42, &first, 0).is_ok()); assert!
+(index.add_in_thread(43, &second, 0).is_ok()); let results =
+index.search_in_thread(&first, 10, 0).unwrap(); ``` Being a systems-programming
+language, Rust has better control over memory management and concurrency but
+lacks function overloading. Aside from the `add` and `search`, USearch Rust
+binding also provides `add_in_thread` and `search_in_thread`, which let users
+identify the calling thread to use underlying temporary memory more
+efficiently. #### Serialization ```rust assert!(index.save
+("index.usearch").is_ok()); assert!(index.load("index.usearch").is_ok());
+assert!(index.view("index.usearch").is_ok()); ``` #### Metrics ```rust assert!
+(new_l2(3, &quant, 0, 0, 0).is_ok()); assert!(new_cos(3, &quant, 0, 0, 0).is_ok
+()); assert!(new_haversine(&quant, 0, 0, 0).is_ok()); ``` ### Java ####
+Installation ```xml  cloud.unum.usearch usearch 0.2.3  ``` Add that snippet to
+your `pom.xml` and hit `mvn install`. #### Quickstart ```java Index index = new
+Index.Config().metric("cos").dimensions(2).build(); float vec[] = {10, 20};
+index.add(42, vec); int[] labels = index.search(vec, 5); ``` ### Swift ####
+Installation ```txt https://github.com/unum-cloud/usearch ``` #### Quickstart
+```swift let index = Index.l2(dimensions: 3, connectivity: 8) let vectorA:
+[Float32] = [0.3, 0.5, 1.2] let vectorB: [Float32] = [0.4, 0.2, 1.2] index.add
+(label: 42, vector: vectorA[...]) index.add(label: 43, vector: vectorB[...])
+let results = index.search(vector: vectorA[...], count: 10) assert(results.0[0]
+== 42) ``` ### GoLang ### Wolfram ## TODO - JavaScript: Allow calling from
+"worker threads". - Rust: Allow passing a custom thread ID. - C# .NET bindings.
+## AI + Vector Search = Semantic Search AI has a growing number of
+applications, but one of the coolest classic ideas is to use it for Semantic
+Search. One can take an encoder model, like the multi-modal UForm, and a web-
+programming framework, like UCall, and build an image search platform in just
+20 lines of Python. ```python import ucall.rich_posix as ucall import uform
+from usearch.index import Index import numpy as np from PIL import Image server
+= ucall.Server() model = uform.get_model('unum-cloud/uform-vl-multilingual')
+index = Index(ndim=256) @server def add(label: int, photo: Image.Image): image
+= model.preprocess_image(photo) vector = model.encode_image(image).detach
+().numpy() index.add(label, vector.flatten(), copy=True) @server def search
+(query: str) -> np.ndarray: tokens = model.preprocess_text(query) vector =
+model.encode_text(tokens).detach().numpy() neighbors, _, _ = index.search
+(vector.flatten(), 3) return neighbors server.run() ``` Check [that](https://
+github.com/ashvardanian/image-search) and [other](https://github.com/unum-
+cloud/examples) examples on our corporate GitHub ð¤
```

