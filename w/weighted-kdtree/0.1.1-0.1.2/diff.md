# Comparing `tmp/weighted_kdtree-0.1.1-py3-none-any.whl.zip` & `tmp/weighted_kdtree-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5949 bytes, number of entries: 8
+Zip file size: 5961 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat       34 b- defN 23-May-10 17:25 kd_tree/__init__.py
 -rw-rw-rw-  2.0 fat     7855 b- defN 23-May-09 22:49 kd_tree/kdtree.py
 -rw-rw-rw-  2.0 fat       34 b- defN 23-May-10 17:25 weighted_kdtree/__init__.py
--rw-rw-rw-  2.0 fat     7075 b- defN 23-May-10 17:29 weighted_kdtree/kdtree.py
--rw-rw-rw-  2.0 fat     1458 b- defN 23-May-10 18:09 weighted_kdtree-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-10 18:09 weighted_kdtree-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-May-10 18:09 weighted_kdtree-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      642 b- defN 23-May-10 18:09 weighted_kdtree-0.1.1.dist-info/RECORD
-8 files, 17206 bytes uncompressed, 4823 bytes compressed:  72.0%
+-rw-rw-rw-  2.0 fat     7144 b- defN 23-May-18 16:38 weighted_kdtree/kdtree.py
+-rw-rw-rw-  2.0 fat     1439 b- defN 23-May-18 16:46 weighted_kdtree-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-18 16:46 weighted_kdtree-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-May-18 16:46 weighted_kdtree-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      642 b- defN 23-May-18 16:46 weighted_kdtree-0.1.2.dist-info/RECORD
+8 files, 17256 bytes uncompressed, 4835 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: weighted_kdtree/__init__.py
 Comment: 
 
 Filename: weighted_kdtree/kdtree.py
 Comment: 
 
-Filename: weighted_kdtree-0.1.1.dist-info/METADATA
+Filename: weighted_kdtree-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: weighted_kdtree-0.1.1.dist-info/WHEEL
+Filename: weighted_kdtree-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: weighted_kdtree-0.1.1.dist-info/top_level.txt
+Filename: weighted_kdtree-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: weighted_kdtree-0.1.1.dist-info/RECORD
+Filename: weighted_kdtree-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## weighted_kdtree/kdtree.py

```diff
@@ -125,16 +125,16 @@
                             ]))
         return res
 
     @classmethod
     def nnKDTree(self, queryPoint, root, threshold, noOfPoints):
         neighborsList = []
         heapq.heapify(neighborsList)
-        return self.nnKDTreeRec(queryPoint, root, threshold, noOfPoints, neighborsList)
-
+        neighbors = self.nnKDTreeRec(queryPoint, root, threshold, noOfPoints, neighborsList)
+        return [neighbor[1] for neighbor in neighbors]
     @classmethod
     def getDistance(self, p1, p2, metric="eucledian"):
         if metric == "eucledian":
             retValue = (p1[0] - p2[0]) ** 2 + (p1[1] - p2[1]) ** 2
         return math.sqrt(retValue)
     
     @classmethod
@@ -150,17 +150,17 @@
         if not root:
             return listOfNeighbors
         else:
             distance = self.getDistance(root.val, queryPoint)
             if distance <= threshold:
                 # Remove the point with largest distance and insert the new point
                 if len(listOfNeighbors) >= noOfPoints:
-                    heapq.heappushpop(listOfNeighbors, (distance, root.val))
+                    heapq.heappushpop(listOfNeighbors, (-1 * distance, root.val))
                 else:
-                    heapq.heappush(listOfNeighbors, (distance, root.val))
+                    heapq.heappush(listOfNeighbors, (-1 * distance, root.val))
             
                     
             # If root is leaf, return the list
             if root.left == None and root.right == None:
                 return listOfNeighbors
             else:
```

## Comparing `weighted_kdtree-0.1.1.dist-info/METADATA` & `weighted_kdtree-0.1.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weighted-kdtree
-Version: 0.1.1
+Version: 0.1.2
 Summary: UNKNOWN
 Home-page: https://github.com/moni97/kdtreePython
 Author: Monisha Siddananda Sampaths
 Author-email: monisam97@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -38,12 +38,11 @@
 kdtree.KDTree.nnKDTree((10, 20), kd_tree.root, 15, 3)
 [(10.04987562112089, (9, 10)),
  (12.206555615733702, (20, 27)),
  (14.142135623730951, (12, 34))]
 ```
 Future work:
 Following weights related methods are to be added soon:
-1. nearestNeighbor
-2. Find points in a query rectangle with a weight threshold
-3. Point with minimum weight in a query rectangle
-4. Point with maximum weight in a query rectangle
+1. Find points in a query rectangle with a weight threshold
+2. Point with minimum weight in a query rectangle
+3. Point with maximum weight in a query rectangle
```

## Comparing `weighted_kdtree-0.1.1.dist-info/RECORD` & `weighted_kdtree-0.1.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 kd_tree/__init__.py,sha256=p8fJVgeoTbgV1pxh9Np2OfOEEVlgmY-veskPsjxSkts,34
 kd_tree/kdtree.py,sha256=JFfPQQmnYMBlE_sw6xAZgqlT6vdsnqC3DdKlLjb7d8w,7855
 weighted_kdtree/__init__.py,sha256=p8fJVgeoTbgV1pxh9Np2OfOEEVlgmY-veskPsjxSkts,34
-weighted_kdtree/kdtree.py,sha256=1QXXhD6gCB1Yz45D4bYFDRXXarYbUzGg073QonuEEP8,7075
-weighted_kdtree-0.1.1.dist-info/METADATA,sha256=C2c7dcje6HWIHM2tHe53iKYRE4hCFfkIBEl9fukBd1A,1458
-weighted_kdtree-0.1.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-weighted_kdtree-0.1.1.dist-info/top_level.txt,sha256=psKGSQLnglz7IvyuWu-ESVAt9WtpVY1Q7VV8a7i-S7I,16
-weighted_kdtree-0.1.1.dist-info/RECORD,,
+weighted_kdtree/kdtree.py,sha256=9Pcn_15gDPwQuRLa9j-voqseMJODZMgJ1DkKLFD2-Tc,7144
+weighted_kdtree-0.1.2.dist-info/METADATA,sha256=Fslam0KWkD02en2I0dUAUx5Tuy1DouWSPO1CXkYP8iQ,1439
+weighted_kdtree-0.1.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+weighted_kdtree-0.1.2.dist-info/top_level.txt,sha256=psKGSQLnglz7IvyuWu-ESVAt9WtpVY1Q7VV8a7i-S7I,16
+weighted_kdtree-0.1.2.dist-info/RECORD,,
```

