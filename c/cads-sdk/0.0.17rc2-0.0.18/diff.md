# Comparing `tmp/cads_sdk-0.0.17rc2-py3-none-any.whl.zip` & `tmp/cads_sdk-0.0.18-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 55338 bytes, number of entries: 18
--rw-rw-r--  2.0 unx     1268 b- defN 23-May-08 07:31 cads_sdk/__init__.py
+Zip file size: 55906 bytes, number of entries: 18
+-rw-rw-r--  2.0 unx     1265 b- defN 23-May-18 07:36 cads_sdk/__init__.py
 -rw-rw-r--  2.0 unx     1264 b- defN 23-Apr-01 02:59 cads_sdk/nosql/__init__.py
 -rw-rw-r--  2.0 unx    11231 b- defN 23-Apr-17 08:04 cads_sdk/nosql/codec.py
--rw-rw-r--  2.0 unx    84516 b- defN 23-May-08 07:30 cads_sdk/nosql/converter.py
--rw-rw-r--  2.0 unx    18788 b- defN 23-May-04 08:32 cads_sdk/nosql/display.py
+-rw-rw-r--  2.0 unx    87328 b- defN 23-May-18 07:33 cads_sdk/nosql/converter.py
+-rw-rw-r--  2.0 unx    18968 b- defN 23-May-17 09:34 cads_sdk/nosql/display.py
 -rw-rw-r--  2.0 unx     1187 b- defN 23-Apr-10 10:46 cads_sdk/nosql/etl.py
--rw-rw-r--  2.0 unx      591 b- defN 23-Apr-09 13:11 cads_sdk/nosql/utils.py
+-rw-rw-r--  2.0 unx      881 b- defN 23-May-14 04:02 cads_sdk/nosql/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 14:03 cads_sdk/petastorm/__init__.py
 -rw-rw-r--  2.0 unx    19967 b- defN 23-Apr-10 04:34 cads_sdk/petastorm/dataset_metadata.py
 -rw-rw-r--  2.0 unx    10508 b- defN 23-Apr-10 07:19 cads_sdk/petastorm/fs_utils.py
 -rw-rw-r--  2.0 unx     5427 b- defN 23-Apr-10 04:42 cads_sdk/petastorm/utils.py
 -rw-rw-r--  2.0 unx    22554 b- defN 23-Apr-18 15:18 cads_sdk/pytorch/__init__.py
 -rw-rw-r--  2.0 unx    10653 b- defN 23-Apr-17 08:05 cads_sdk/pytorch/codec.py
 -rw-rw-r--  2.0 unx    78369 b- defN 23-Apr-20 08:23 cads_sdk/pytorch/converter.py
--rw-rw-r--  2.0 unx     7129 b- defN 23-May-08 07:31 cads_sdk-0.0.17rc2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-08 07:31 cads_sdk-0.0.17rc2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-May-08 07:31 cads_sdk-0.0.17rc2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1491 b- defN 23-May-08 07:31 cads_sdk-0.0.17rc2.dist-info/RECORD
-18 files, 275044 bytes uncompressed, 52908 bytes compressed:  80.8%
+-rw-rw-r--  2.0 unx     7126 b- defN 23-May-18 07:37 cads_sdk-0.0.18.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-18 07:37 cads_sdk-0.0.18.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-18 07:37 cads_sdk-0.0.18.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1479 b- defN 23-May-18 07:37 cads_sdk-0.0.18.dist-info/RECORD
+18 files, 278308 bytes uncompressed, 53500 bytes compressed:  80.8%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: cads_sdk/pytorch/codec.py
 Comment: 
 
 Filename: cads_sdk/pytorch/converter.py
 Comment: 
 
-Filename: cads_sdk-0.0.17rc2.dist-info/METADATA
+Filename: cads_sdk-0.0.18.dist-info/METADATA
 Comment: 
 
-Filename: cads_sdk-0.0.17rc2.dist-info/WHEEL
+Filename: cads_sdk-0.0.18.dist-info/WHEEL
 Comment: 
 
-Filename: cads_sdk-0.0.17rc2.dist-info/top_level.txt
+Filename: cads_sdk-0.0.18.dist-info/top_level.txt
 Comment: 
 
-Filename: cads_sdk-0.0.17rc2.dist-info/RECORD
+Filename: cads_sdk-0.0.18.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cads_sdk/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.17rc2'
+__version__ = '0.0.18'
 
 __doc__ = """
 cads-sdk: Functions to help Data Scientist work more effectively with unstructured data and datalake
 =====================================================================
 **cads-sdk**
 Function to convert 
 -------------
```

## cads_sdk/nosql/converter.py

```diff
@@ -5,14 +5,16 @@
 import tempfile
 import os
 from pathlib import Path, PurePath
 
 import numpy as np
 import pandas as pd
 
+from PIL import Image
+
 try:
     import cv2
     OPENCV_AVAILABLE = True
 except ImportError:
     os.system("pip install --proxy http://proxy.hcm.fpt.vn:80 opencv-python")
     import cv2
     OPENCV_AVAILABLE = False
@@ -81,28 +83,37 @@
             
         
     def _generate_input_files(self):
         if isinstance(self.input_path, str):
             list_file = self.get_all_file_in_directory()
         elif isinstance(self.input_path, (tuple, list)):
             list_file = self.input_path
+        else:
+            raise TypeError("Please input path string or tuple or list")
         if self.shorten:
             self.commonpath = os.path.commonpath(list_file)
         return list_file
     
     def get_all_file_in_directory(self):
         input_files = []
         if isinstance(self.input_type, str):
             if self.input_recursive:
                 self.input_path = os.path.join(self.input_path, "**")
             self.input_path = os.path.join(self.input_path, "*."+self.input_type)
             input_files = glob(self.input_path, recursive=self.input_recursive)
             return input_files
         elif isinstance(self.input_type, (tuple, list)):
             for t in self.input_type:
+                t = t.lower()
+                if self.input_recursive:
+                    self.input_path = os.path.join(self.input_path, "**")
+                self.input_path = os.path.join(self.input_path, "*."+t)
+                input_files.extend(glob(self.input_path, recursive=self.input_recursive))
+            for t in self.input_type:
+                t = t.upper()
                 if self.input_recursive:
                     self.input_path = os.path.join(self.input_path, "**")
                 self.input_path = os.path.join(self.input_path, "*."+t)
                 input_files.extend(glob(self.input_path, recursive=self.input_recursive))
             return input_files
     
     def convert_to_hdfs_path(self, input_path):
@@ -152,15 +163,15 @@
                 else:
                     return spark_df.coalesce(numPartition)
         return spark_df
     
     
     def get_spark(self):
         return ss.PySpark(driver_memory='32G', num_executors='8', executor_memory='4G', port='', yarn=False, 
-                         optimze_file_size=("spark.databricks.delta.optimize.maxFileSize", 268435456)).spark
+                         optimze_file_size=("spark.databricks.delta.optimize.maxFileSize", 536870912)).spark
     
     def create_dataframe(self, 
                          spark, 
                          Schema, 
                          input_files):
         from pyspark.sql.functions import expr
         self.unischema = Schema
@@ -191,18 +202,19 @@
                 .option('compression', compression) \
                 .mode('overwrite') \
                 .option("path", output_path) \
                 .saveAsTable(database + '.' + table_name)
         
         if file_format == 'delta':
             if self.shorten:
-                ss.sql(f"""
-                OPTIMIZE delta.`{output_path}` ZORDER BY(rel_path)
-                """)
-            
+                logging.info("OPTIMIZE")
+                #ss.sql(f"""
+                #OPTIMIZE delta.`{output_path}` ZORDER BY(rel_path)
+                #""")
+            logging.info("VACUUM")
             ss.sql(f"""
             VACUUM delta.`{output_path}` RETAIN 0 HOURS
             """)
 
 
 class ConvertFromFolderImage(ConvertFromFolder):
     """
@@ -414,75 +426,98 @@
                 table_name = self.table_name + "_{s0}_{s1}".format(s0=str(s[0]), s1=str(s[1]))
             else:
                 table_name = ''
         else:
             table_name = self.table_name
         logging.info(f"Save metadata at: {table_name}")
         return table_name
-            
+    
+    def replace_character(self, txt):
+        for i in range(len(txt)):
+            if ord(txt[i]) > 1000:
+                txt = txt[:i] + txt[i].encode('unicode_escape').decode('utf-8') + txt[i+1:]
+        return txt
+
     def create_dataframe(self, 
                          spark, 
                          Schema, 
                          input_files,
                          size):
         from pyspark.sql.functions import expr
         self.unischema = Schema
         self.s = size
-        spark_df = spark.createDataFrame(pd.DataFrame(input_files, columns=['path']))
+        pdf = pd.DataFrame([self.replace_character(i) for i in input_files], columns=['path'])
+        spark_df = spark.createDataFrame(pdf)
         if not self.resize_mode:
             logging.warning(f"Not resize image, If get size error try to turn resize_mode='padding' or resize_mode='resize'")
         if self.shorten:
             return spark.createDataFrame(spark_df.rdd.mapPartitions(self.row_generator), Schema.as_spark_schema()).withColumn("rel_path", expr(f"""replace(path, '{self.commonpath}', '') """))
         else:
             return spark.createDataFrame(spark_df.rdd.mapPartitions(self.row_generator), Schema.as_spark_schema())
-        
+    
+    def replace_special_characters(self, txt: str):
+        if self.debug:
+            print(txt)
+        for i in range(56527, 56576):
+            txt = txt.replace(chr(i).encode('unicode_escape').decode('utf-8'), chr(i))
+        for i in range(7840, 7930):
+            txt = txt.replace(chr(i).encode('unicode_escape').decode('utf-8'), chr(i))
+        return txt
+    
     def row_generator(self, partitionData):
         """Returns a dict of row input to rdd spark dataframe"""
         for row in partitionData:
             path = row.path
             if self.debug:
                 print(f"Convert Image {path}") #, file=self.log_file)
-                
-            img = cv2.imread(path)
+                print(self.replace_special_characters(path))
+            path = self.replace_special_characters(path)
+            try:
+                img = Image.open(path)
+            except Exception as e:
+                print(e)
+                print(path)
+                img = None
             if type(img).__name__ != "NoneType":
                 if self.resize_mode == 'padding':
                     row_dict = {
                         'path': path,
-                        'size': img.shape.__str__(),
-                        'image': padding(img, (self.s[0], self.s[1]))
+                        'size': img.size.__str__(),
+                        'image': padding(np.array(img), (self.s[0], self.s[1]))
                     }
 
                     yield dict_to_spark_row(self.unischema, row_dict)
                 elif self.resize_mode == 'resize':
                     row_dict = {
                         'path': path,
-                        'size': img.shape.__str__(),
-                        'image': cv2.resize(img, (self.s[0], self.s[1]))
+                        'size': img.size.__str__(),
+                        'image': cv2.resize(np.array(img), (self.s[0], self.s[1]))
                     }
 
                     yield dict_to_spark_row(self.unischema, row_dict)
                 else:
                     row_dict = {
                         'path': path,
-                        'size': img.shape.__str__(),
+                        'size': img.size.__str__(),
                         'image': open(path, 'rb').read()
                     }
 
                     yield dict_to_spark_row(self.unischema, row_dict)
             else:
                 row_dict = {
                     'path': path,
                     'size': "Can not get size",
                     'image': open(path, 'rb').read()
                 }
 
                 yield dict_to_spark_row(self.unischema, row_dict)
+
        
                     
-    def create_image_schema(self, size, image_type, image_color):
+    def get_schema(self, size, image_type, image_color):
         """
         :param size: Image size, schema need to be consistency
         :param image_type: Image type is compress JPG or PNG
         :param image_color: 3 dimention color or 1 dimention colors
         """
         if self.resize_mode:
             return Unischema('ImageSchema', [
@@ -529,15 +564,16 @@
                     self.dict_image[self.check_size(img, self.size)].append(p)
         else:
             self.dict_image[self.size[0]] = self._generate_input_files()
 
         for s in self.size:
             if self.dict_image[s]:
                 self.analyze_path = self.dict_image[s]
-                Schema = self.create_image_schema(s, self.image_type, self.image_color)
+                self.numPartition = self.get_num_partition()
+                Schema = self.get_schema(s, self.image_type, self.image_color)
                 self.output_path = self.convert_to_hdfs_path(self.output_path)
                 output_path = self._generate_output_path(s)
                 table_name = self._generate_table_name(s)
                 spark = self.get_spark()
                 
                 with materialize_dataset(spark, output_path, Schema, ROWGROUP_SIZE_MB):
                     self.write_to_path(spark_df = self.create_dataframe(spark=spark,
@@ -796,16 +832,17 @@
         
         for s in self.size:
             self.dict_image[s] = []
         
         self.dict_image[self.size[0]] = self._generate_input_files()
         
         if self.dict_image[s]:
-            self.analyze_path = self.input_path
-            Schema = self.create_image_schema(s, self.image_type, self.image_color)
+            self.analyze_path = self.dict_image[s]
+            self.numPartition = self.get_num_partition()
+            Schema = self.get_schema(s, self.image_type, self.image_color)
             self.output_path = self.convert_to_hdfs_path(self.output_path)
             output_path = self._generate_output_path(s)
             table_name = self._generate_table_name(s)
             spark = self.get_spark()
 
             with materialize_dataset(spark, output_path, Schema, ROWGROUP_SIZE_MB):
                 self.write_to_path(spark_df = self.create_dataframe(spark=spark,
@@ -1005,18 +1042,20 @@
           {sql_compare}
             
           WHEN NOT MATCHED
           THEN INSERT *
         """)
         
         if file_format == 'delta':
+            logging.info("OPTIMIZE")
             ss.sql(f"""
             OPTIMIZE delta.`{output_path}` ZORDER BY(path)
             """)
             
+            logging.info("VACUUM")
             ss.sql(f"""
             VACUUM delta.`{output_path}` RETAIN 0 HOURS
             """)
     
     def execute(self, ROWGROUP_SIZE_MB = 256):
         self.dict_image = {}
 
@@ -1035,16 +1074,17 @@
                 img = cv2.imread(p)
                 self.dict_image[self.check_size(img, self.size)].append(p)
         else:
             self.dict_image[self.size[0]] = self._generate_input_files()
 
         for s in self.size:
             if self.dict_image[s]:
+                self.analyze_path = self.dict_image[s]
+                self.numPartition = self.get_num_partition()
                 Schema = self.create_image_schema(s, self.image_type, self.image_color)
-                self.numPartition = self.get_num_partition(self.dict_image[s])
                 self.output_path = self.convert_to_hdfs_path(self.output_path)
                 output_path = self._generate_output_path(s)
                 self.check_output(output_path)
                 table_name = self._generate_table_name(s)
                 spark = self.get_spark()
                 
                 with materialize_dataset(spark, output_path, Schema, ROWGROUP_SIZE_MB):
@@ -1186,17 +1226,14 @@
                 return input_path
 
         
     def mkdir_folder(self, output_path):
         if not os.path.exists(output_path):
             os.makedirs(output_path)
             
-    def get_spark(self):
-        return ss.PySpark(driver_memory='32G', num_executors='8', executor_memory='4G', port='', yarn=False).spark
-            
     def write_to_folder(self, row):
         if self.write_mode == "recovery":
             output_path = os.path.join(self.output_path, row.path.replace(self.raw_input_path, ""))
         else:
             base_path = os.path.basename(str(row.path))
             output_path = os.path.join(self.output_path, base_path)
         
@@ -1320,30 +1357,37 @@
         
         spark = self.get_spark()
         Schema = self.get_schema()
         
         if input_files:
             input_files = self._generate_input_files()
             self.analyze_path = input_files
+            self.numPartition = self.get_num_partition()
             self.output_path = self.convert_to_hdfs_path(self.output_path)
             output_path = self._generate_output_path()
             table_name = self._generate_table_name()
             Schema = self.get_schema()
             spark = self.get_spark()
             
+            self.write_to_path(spark_df = self.create_dataframe(spark=spark,
+                                  Schema=Schema,
+                                  input_files=input_files),
+
+                            output_path = self.output_path,
+                            table_name = self.table_name, 
+                            database = self.database,
+                            numPartition = self.numPartition,
+                            compression = self.compression)
+                
+            if self.shorten:
+                Schema.__dict__['_fields']['rel_path'] = UnischemaField('rel_path', np.str_, (), ScalarCodec(StringType()), False)
+                Schema.__dict__['rel_path'] = UnischemaField('rel_path', np.str_, (), ScalarCodec(StringType()), False)
             with materialize_dataset(spark, self.output_path, Schema, ROWGROUP_SIZE_MB):
-                self.write_to_path(spark_df = self.create_dataframe(spark=spark,
-                                      Schema=Schema,
-                                      input_files=input_files),
-
-                                output_path = self.output_path,
-                                table_name = self.table_name, 
-                                database = self.database,
-                                numPartition = self.numPartition,
-                                compression = self.compression)
+                print("Write metadata")
+            
         else:
             logging.warn("No files were found, check your input_path")
             
         logging.info("Convert complete")
             
 
 class ConvertFromVideo2Image:
@@ -1570,15 +1614,16 @@
         
         self.thumbnail_width = frame_size[0]
         self.thumbnail_height = frame_size[1]
         
         return spark.createDataFrame(spark_df.rdd.mapPartitions(self.row_generator), Schema.as_spark_schema())
         
     def get_spark(self):
-        return ss.PySpark(driver_memory='32G', num_executors='4', executor_memory='4G', port='', yarn=False).spark
+        return ss.PySpark(driver_memory='32G', num_executors='8', executor_memory='4G', port='', yarn=False, 
+                         optimze_file_size=("spark.databricks.delta.optimize.maxFileSize", 536870912)).spark
     
     def get_schema(self):
         return Unischema('VideoImage', [
             UnischemaField('frame_id', np.int, (), ScalarCodec(IntegerType()), False),
             UnischemaField('path', np.str_, (), ScalarCodec(StringType()), False),
             UnischemaField('duration', np.float_, (), ScalarCodec(FloatType()), False),
             UnischemaField('frame_size', np.str_, (), ScalarCodec(StringType()), False),
@@ -1591,29 +1636,32 @@
         input_files = self.input_path #sorted(glob(self.input_path, recursive=self.input_recursive))
         self.output_path = self.convert_to_hdfs_path(self.output_path)
         
         spark = self.get_spark()
         Schema = self.get_schema()
 
 
-        
         if input_files:
             logging.info(f"Write at path: {self.output_path}")
             logging.info(f"Save metadata at: {self.table_name}")
             
+            self.write_to_path(spark_df = self.create_dataframe(spark=spark,
+                                  Schema=Schema,
+                                  input_files=input_files),
+
+                            output_path = self.output_path,
+                            table_name = self.table_name, 
+                            database = self.database,
+                            numPartition = self.numPartition,
+                            compression = self.compression)
+            if self.shorten:
+                Schema.__dict__['_fields']['rel_path'] = UnischemaField('rel_path', np.str_, (), ScalarCodec(StringType()), False)
+                Schema.__dict__['rel_path'] = UnischemaField('rel_path', np.str_, (), ScalarCodec(StringType()), False)
             with materialize_dataset(spark, self.output_path, Schema, ROWGROUP_SIZE_MB):
-                self.write_to_path(spark_df = self.create_dataframe(spark=spark,
-                                      Schema=Schema,
-                                      input_files=input_files),
-
-                                output_path = self.output_path,
-                                table_name = self.table_name, 
-                                database = self.database,
-                                numPartition = self.numPartition,
-                                compression = self.compression)
+                print("Write metadata")
         else:
             logging.warn("No files were found, check your input_path")
             
         logging.info("Convert complete")
         
 
 class ConvertToFolderVideo:
@@ -1760,18 +1808,14 @@
 #------- AUDIO SESSION -----------#
 #---------------------------------#
 
 import_or_install("pydub")
 import pydub
 import_or_install("scipy")
 from scipy.io import wavfile
-import_or_install("pydub")
-import pydub
-import_or_install("scipy")
-from scipy.io import wavfile
 class ConvertFromFolderAudio(ConvertFromFolder):
     """
     Create a parquet/delta file given local Image directory
     
 
     Parameters
     ----------
@@ -1936,15 +1980,14 @@
                 channels = 1
 
                 data = data.tobytes()
 
             elif self.guess_type(path) == 'wav':
                 samplerate, data = wavfile.read(path)
                 if len(data.shape) == 2:
-                    data = data.T
                     channels = 2
                 else:
                     channels = 1
 
                 with open(path, 'rb') as file:
                     data = file.read()
 
@@ -1972,38 +2015,44 @@
     
     
     def get_schema(self):
         return Unischema('Audio', [
             UnischemaField('path', np.str_, (), ScalarCodec(StringType()), False),
             UnischemaField('samplerate', np.int_, (), ScalarCodec(IntegerType()), False),
             UnischemaField('channels', np.int_, (), ScalarCodec(IntegerType()), False),
-            UnischemaField('audio', self.numpy_map_type(self.analyze_path), (1000,), AudioCodec(self.guess_type(self.analyze_path)), False)
+            UnischemaField('audio', self.numpy_map_type(self.analyze_path), (1000,), AudioCodec(self.guess_type(self.analyze_path[0])), False)
         ])
     
     def execute(self, ROWGROUP_SIZE_MB = 256):
         input_files = self._generate_input_files()
         self.analyze_path = input_files
         self.numPartition = self.get_num_partition()
         self.output_path = self.convert_to_hdfs_path(self.output_path)
         output_path = self._generate_output_path()
         table_name = self._generate_table_name()
         Schema = self.get_schema()
         spark = self.get_spark()
         
+        
         if input_files:
-            with materialize_dataset(spark, output_path, Schema, ROWGROUP_SIZE_MB):
-                self.write_to_path(spark_df = self.create_dataframe(spark=spark,
-                                      Schema=Schema,
-                                      input_files=input_files),
-
-                                output_path = output_path,
-                                table_name = table_name, 
-                                database = self.database,
-                                numPartition = self.numPartition,
-                                compression = self.compression)
+            self.write_to_path(spark_df = self.create_dataframe(spark=spark,
+                                  Schema=Schema,
+                                  input_files=input_files),
+
+                            output_path = output_path,
+                            table_name = table_name, 
+                            database = self.database,
+                            numPartition = self.numPartition,
+                            compression = self.compression)
+            if self.shorten:
+                Schema.__dict__['_fields']['rel_path'] = UnischemaField('rel_path', np.str_, (), ScalarCodec(StringType()), False)
+                Schema.__dict__['rel_path'] = UnischemaField('rel_path', np.str_, (), ScalarCodec(StringType()), False)
+            with materialize_dataset(spark, self.output_path, Schema, ROWGROUP_SIZE_MB):
+                print("DEBUG", Schema)
+                print("Write metadata")
         else:
             logging.warn("No files were found, check your input_path")
             
         logging.info("Convert complete")
 
 
         
@@ -2143,18 +2192,19 @@
           {sql_compare}
             
           WHEN NOT MATCHED
           THEN INSERT *
         """)
         
         if file_format == 'delta':
+            logging.info("OPTIMIZE")
             ss.sql(f"""
             OPTIMIZE delta.`{output_path}` ZORDER BY(path)
             """)
-            
+            logging.info("VACUUM")
             ss.sql(f"""
             VACUUM delta.`{output_path}` RETAIN 0 HOURS
             """)
     
     def execute(self, ROWGROUP_SIZE_MB = 256):
         input_files = self._generate_input_files()
         self.analyze_path = input_files
@@ -2162,24 +2212,28 @@
         self.output_path = self.convert_to_hdfs_path(self.output_path)
         output_path = self._generate_output_path()
         table_name = self._generate_table_name()
         Schema = self.get_schema()
         spark = self.get_spark()
         
         if input_files:
-            with materialize_dataset(spark, output_path, Schema, ROWGROUP_SIZE_MB):
-                self.write_to_path(spark_df = self.create_dataframe(spark=spark,
-                                      Schema=Schema,
-                                      input_files=input_files),
-
-                                output_path = output_path,
-                                table_name = table_name, 
-                                database = self.database,
-                                numPartition = self.numPartition,
-                                compression = self.compression)
+            self.write_to_path(spark_df = self.create_dataframe(spark=spark,
+                                  Schema=Schema,
+                                  input_files=input_files),
+
+                            output_path = output_path,
+                            table_name = table_name, 
+                            database = self.database,
+                            numPartition = self.numPartition,
+                            compression = self.compression)
+            if self.shorten:
+                Schema.__dict__['_fields']['rel_path'] = UnischemaField('rel_path', np.str_, (), ScalarCodec(StringType()), False)
+                Schema.__dict__['rel_path'] = UnischemaField('rel_path', np.str_, (), ScalarCodec(StringType()), False)
+            with materialize_dataset(spark, self.output_path, Schema, ROWGROUP_SIZE_MB):
+                print("Write metadata")
         else:
             logging.warn("No files were found, check your input_path")
             
         logging.info("Convert complete")
```

## cads_sdk/nosql/display.py

```diff
@@ -512,15 +512,21 @@
         elif 'mp3' in row.path:
             samplerate, data = read_mp3(BytesIO(row.audio))
             from IPython.display import Audio, display
             self.output.append_display_data(Audio(data.T, rate=samplerate))
             
     def displayAudio(self, ex):
         get_value = ex.description
-        df = self.generate_sql("*").filter(f"path = '{get_value}'").limit(1)
+        
+        df = self.generate_sql("*")
+        
+        if 'rel_path' in df.schema.name:
+            df = df.filter(f"rel_path like '%{os.path.basename(get_value)}'").limit(1)
+        else:
+            df = df.filter(f"path = '{get_value}'").limit(1)
         
         _ = [self.write_to_folder(row) for row in df.collect()]
         
         # df.foreach(self.write_to_folder)
         
         
     def _repr_html_(self):
```

## cads_sdk/nosql/utils.py

```diff
@@ -14,11 +14,21 @@
         for entry in it:
             if entry.is_file():
                 total += entry.stat().st_size
             elif entry.is_dir():
                 total += get_size_of_dir(entry.path)
     return total
 
+def get_all_file_of_dir(path):
+    total = []
+    with os.scandir(path) as it:
+        for entry in it:
+            if entry.is_file():
+                total.append(entry.path)
+            elif entry.is_dir():
+                total.extend(get_all_file_of_dir(entry.path))
+    return total
+
 
 def get_size_of_list(input_files):
     total = sum([os.stat(path).st_size for path in input_files])
     return total
```

## Comparing `cads_sdk-0.0.17rc2.dist-info/METADATA` & `cads_sdk-0.0.18.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cads-sdk
-Version: 0.0.17rc2
+Version: 0.0.18
 Summary: Function to help Data Scientist work more effectively with DWH
 Home-page: http://git.bigdata.local/data-engineers/sdk/utilities
 Author: duyvnc
 Author-email: duyvnc@fpt.com.vn
 License: duyvnc
 Platform: UNKNOWN
 Requires-Python: >=3.5
```

## Comparing `cads_sdk-0.0.17rc2.dist-info/RECORD` & `cads_sdk-0.0.18.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-cads_sdk/__init__.py,sha256=fHfgZC8CDlsACSZAo931mS4LLDQhWuC6JMkqNepvYYc,1268
+cads_sdk/__init__.py,sha256=HI7WMAX9xElE9f47tdMfq4kvoaM6I2v9pDb7LDEASdU,1265
 cads_sdk/nosql/__init__.py,sha256=Yu2Zt5cpSXSLqIRAvIxaXOtoyj3yBisGTbnFlH4UD2A,1264
 cads_sdk/nosql/codec.py,sha256=Z0RdndLtSHAnqHOpDGE-Wb_jD9eIWvKiuX4Yj1KudX4,11231
-cads_sdk/nosql/converter.py,sha256=1vHieW_nUeHk7Hxk2LS0AAdmC1rMUHPV8DolrdvBIU8,84516
-cads_sdk/nosql/display.py,sha256=xHwRIirQrpYsOuq4lQxgEPXa8LQTzc5GtnEbA_nSMnA,18788
+cads_sdk/nosql/converter.py,sha256=dW0Hghhiqax1dVxJrH3piDwL-_oaaMnbc8qSEqstHAQ,87328
+cads_sdk/nosql/display.py,sha256=lOaFffzd6p5eDIFFoKcw37XgyxhhFVpPkeV_Ipm-DaA,18968
 cads_sdk/nosql/etl.py,sha256=PWhXNWZyIFFEEvTIoUNuKK5cDqTy8A4FPn07BGMr0Vk,1187
-cads_sdk/nosql/utils.py,sha256=5y4Q5ydkesUteW_fqAc3ifwAlARvv9w58PWNyJz6iyA,591
+cads_sdk/nosql/utils.py,sha256=avlOSkBze2SWZnF38kdw15i_lHy57EaZ5AhWgK8J1XI,881
 cads_sdk/petastorm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cads_sdk/petastorm/dataset_metadata.py,sha256=3sXVulFmpZEJC7mM0cwEXBVmB-0TD-U746ltLcsqIno,19967
 cads_sdk/petastorm/fs_utils.py,sha256=qFAzfi_VM4Rr2mBW8JsgxPUojLFFQGZI93MpI4sL_Xo,10508
 cads_sdk/petastorm/utils.py,sha256=CyeRPL_ih9wC1BdElvf1VknF1lBdNvJxgldSiU1OkFs,5427
 cads_sdk/pytorch/__init__.py,sha256=qyLEDZ_2BXLQBqievSj4wg2h4EQf9AdbIi_1SKFyIsM,22554
 cads_sdk/pytorch/codec.py,sha256=5XZulM21El-lsL3jZMexnJAHc2cIeRZj721PMuPhsJU,10653
 cads_sdk/pytorch/converter.py,sha256=lT2c3ix8Q35TEOUdFzlQVIzf7GfRklomwrdfRaXcY7k,78369
-cads_sdk-0.0.17rc2.dist-info/METADATA,sha256=CNg1DAmiHWMnvvBLoP_HBeiYQZMPMzlXLjXOi4Okm1M,7129
-cads_sdk-0.0.17rc2.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-cads_sdk-0.0.17rc2.dist-info/top_level.txt,sha256=OaTWVG-YiGPwrATCivDFDqvFPPP_T6y0TYXz8dkujOU,9
-cads_sdk-0.0.17rc2.dist-info/RECORD,,
+cads_sdk-0.0.18.dist-info/METADATA,sha256=Mr2CqP5dGl3XIadXBsz7cQUF_zs4qNmad3XiYOmzqUs,7126
+cads_sdk-0.0.18.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+cads_sdk-0.0.18.dist-info/top_level.txt,sha256=OaTWVG-YiGPwrATCivDFDqvFPPP_T6y0TYXz8dkujOU,9
+cads_sdk-0.0.18.dist-info/RECORD,,
```

