# Comparing `tmp/dlt_meta-0.0.1-py3-none-any.whl.zip` & `tmp/dlt_meta-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 20713 bytes, number of entries: 13
--rw-r--r--  2.0 unx       69 b- defN 23-Mar-21 23:28 src/__init__.py
--rw-r--r--  2.0 unx     1664 b- defN 23-Mar-21 23:28 src/__main__.py
--rw-r--r--  2.0 unx    15394 b- defN 23-Mar-21 23:28 src/dataflow_pipeline.py
--rw-r--r--  2.0 unx     9501 b- defN 23-Mar-21 23:28 src/dataflow_spec.py
--rw-r--r--  2.0 unx     3087 b- defN 23-Mar-21 23:28 src/metastore_ops.py
--rw-r--r--  2.0 unx    28362 b- defN 23-Mar-21 23:28 src/onboard_dataflowspec.py
--rw-r--r--  2.0 unx     6411 b- defN 23-Mar-21 23:28 src/pipeline_readers.py
--rw-r--r--  2.0 unx     3597 b- defN 23-Mar-21 23:28 dlt_meta-0.0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    12645 b- defN 23-Mar-21 23:28 dlt_meta-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-21 23:28 dlt_meta-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       33 b- defN 23-Mar-21 23:28 dlt_meta-0.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 23-Mar-21 23:28 dlt_meta-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1034 b- defN 23-Mar-21 23:28 dlt_meta-0.0.1.dist-info/RECORD
-13 files, 81893 bytes uncompressed, 18997 bytes compressed:  76.8%
+Zip file size: 19034 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       69 b- defN 23-May-18 21:04 src/__init__.py
+-rw-r--r--  2.0 unx     1664 b- defN 23-May-18 21:04 src/__main__.py
+-rw-r--r--  2.0 unx    16978 b- defN 23-May-18 21:04 src/dataflow_pipeline.py
+-rw-r--r--  2.0 unx     9779 b- defN 23-May-18 21:04 src/dataflow_spec.py
+-rw-r--r--  2.0 unx     3087 b- defN 23-May-18 21:04 src/metastore_ops.py
+-rw-r--r--  2.0 unx    30274 b- defN 23-May-18 21:04 src/onboard_dataflowspec.py
+-rw-r--r--  2.0 unx     7658 b- defN 23-May-18 21:04 src/pipeline_readers.py
+-rw-r--r--  2.0 unx     3597 b- defN 23-May-18 21:05 dlt_meta-0.0.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     4999 b- defN 23-May-18 21:05 dlt_meta-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-18 21:05 dlt_meta-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       34 b- defN 23-May-18 21:05 dlt_meta-0.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-May-18 21:05 dlt_meta-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1033 b- defN 23-May-18 21:05 dlt_meta-0.0.2.dist-info/RECORD
+13 files, 79268 bytes uncompressed, 17318 bytes compressed:  78.2%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: src/onboard_dataflowspec.py
 Comment: 
 
 Filename: src/pipeline_readers.py
 Comment: 
 
-Filename: dlt_meta-0.0.1.dist-info/LICENSE.txt
+Filename: dlt_meta-0.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dlt_meta-0.0.1.dist-info/METADATA
+Filename: dlt_meta-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: dlt_meta-0.0.1.dist-info/WHEEL
+Filename: dlt_meta-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: dlt_meta-0.0.1.dist-info/entry_points.txt
+Filename: dlt_meta-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: dlt_meta-0.0.1.dist-info/top_level.txt
+Filename: dlt_meta-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dlt_meta-0.0.1.dist-info/RECORD
+Filename: dlt_meta-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## src/dataflow_pipeline.py

```diff
@@ -1,13 +1,14 @@
 """DataflowPipeline provide generic DLT code using dataflowspec."""
 import json
 import logging
 import dlt
 from pyspark.sql import DataFrame
-from pyspark.sql.types import StructType, StructField
+from pyspark.sql.functions import expr
+from pyspark.sql.types import IntegerType, StructType, StructField
 
 from src.dataflow_spec import BronzeDataflowSpec, SilverDataflowSpec, DataflowSpecUtils
 from src.pipeline_readers import PipelineReaders
 
 logger = logging.getLogger("dlt-meta")
 logger.setLevel(logging.INFO)
 
@@ -93,14 +94,16 @@
 
     def read_bronze(self) -> DataFrame:
         """Read Bronze Table."""
         logger.info("In read_bronze func")
         bronze_dataflow_spec: BronzeDataflowSpec = self.dataflowSpec
         if bronze_dataflow_spec.sourceFormat == "cloudFiles":
             return PipelineReaders.read_dlt_cloud_files(self.spark, bronze_dataflow_spec, self.schema_json)
+        elif bronze_dataflow_spec.sourceFormat == "delta":
+            return PipelineReaders.read_dlt_delta(self.spark, bronze_dataflow_spec)
         elif bronze_dataflow_spec.sourceFormat == "eventhub" or bronze_dataflow_spec.sourceFormat == "kafka":
             return PipelineReaders.read_kafka(self.spark, bronze_dataflow_spec, self.schema_json)
         else:
             raise Exception(f"{bronze_dataflow_spec.sourceFormat} source format not supported")
 
     def get_silver_schema(self):
         """Get Silver table Schema."""
@@ -110,38 +113,53 @@
         select_exp = silver_dataflow_spec.selectExp
         where_clause = silver_dataflow_spec.whereClause
         raw_delta_table_stream = self.spark.read.load(
             path=silver_dataflow_spec.sourceDetails["path"],
             format="delta"
             # #f"{source_database}.{source_table}"
         ).selectExpr(*select_exp)
-        where_clause_str = " ".join(where_clause)
-        if len(where_clause_str.strip()) > 0:
-            for where_clause in where_clause:
-                raw_delta_table_stream = raw_delta_table_stream.where(where_clause)
+        raw_delta_table_stream = self.__apply_where_clause(where_clause, raw_delta_table_stream)
         return raw_delta_table_stream.schema
 
+    def __apply_where_clause(self, where_clause, raw_delta_table_stream):
+        """This method apply where clause provided in silver transformations
+
+        Args:
+            where_clause (_type_): _description_
+            raw_delta_table_stream (_type_): _description_
+
+        Returns:
+            _type_: _description_
+        """
+        if where_clause:
+            where_clause_str = " ".join(where_clause)
+            if len(where_clause_str.strip()) > 0:
+                for where_clause in where_clause:
+                    raw_delta_table_stream = raw_delta_table_stream.where(where_clause)
+        return raw_delta_table_stream
+
     def read_silver(self) -> DataFrame:
         """Read Silver tables."""
         silver_dataflow_spec: SilverDataflowSpec = self.dataflowSpec
         # source_database = silver_dataflow_spec.sourceDetails["database"]
         # source_table = silver_dataflow_spec.sourceDetails["table"]
         select_exp = silver_dataflow_spec.selectExp
         where_clause = silver_dataflow_spec.whereClause
         raw_delta_table_stream = self.spark.readStream.load(
             path=silver_dataflow_spec.sourceDetails["path"],
             format="delta"
             # f"{source_database}.{source_table}"
         ).selectExpr(
             *select_exp
         )  # .selectExpr(select_exp.split(","))
-        where_clause_str = " ".join(where_clause)
-        if len(where_clause_str.strip()) > 0:
-            for where_clause in where_clause:
-                raw_delta_table_stream = raw_delta_table_stream.where(where_clause)
+        if where_clause:
+            where_clause_str = " ".join(where_clause)
+            if len(where_clause_str.strip()) > 0:
+                for where_clause in where_clause:
+                    raw_delta_table_stream = raw_delta_table_stream.where(where_clause)
         return raw_delta_table_stream
 
     def write_to_delta(self):
         """Write to Delta."""
         return dlt.read_stream(self.view_name)
 
     def write_bronze_with_dqe(self):
@@ -166,38 +184,41 @@
             self.cdc_apply_changes()
         else:
             if expect_dict:
                 dlt_table_with_expectation = dlt.expect_all(expect_dict)(
                     dlt.table(
                         self.write_to_delta,
                         name=f"{bronzeDataflowSpec.targetDetails['table']}",
+                        table_properties=bronzeDataflowSpec.tableProperties,
                         partition_cols=DataflowSpecUtils.get_partition_cols(bronzeDataflowSpec.partitionColumns),
                         path=bronzeDataflowSpec.targetDetails["path"],
                         comment=f"bronze dlt table{bronzeDataflowSpec.targetDetails['table']}",
                     )
                 )
             if expect_or_fail_dict:
                 if expect_dict is None:
                     dlt_table_with_expectation = dlt.expect_all_or_fail(expect_or_fail_dict)(
                         dlt.table(
                             self.write_to_delta,
                             name=f"{bronzeDataflowSpec.targetDetails['table']}",
+                            table_properties=bronzeDataflowSpec.tableProperties,
                             partition_cols=DataflowSpecUtils.get_partition_cols(bronzeDataflowSpec.partitionColumns),
                             path=bronzeDataflowSpec.targetDetails["path"],
                             comment=f"bronze dlt table{bronzeDataflowSpec.targetDetails['table']}",
                         )
                     )
                 else:
                     dlt_table_with_expectation = dlt.expect_all_or_fail(expect_or_fail_dict)(dlt_table_with_expectation)
             if expect_or_drop_dict:
                 if expect_dict is None and expect_or_fail_dict is None:
                     dlt_table_with_expectation = dlt.expect_all_or_drop(expect_or_drop_dict)(
                         dlt.table(
                             self.write_to_delta,
                             name=f"{bronzeDataflowSpec.targetDetails['table']}",
+                            table_properties=bronzeDataflowSpec.tableProperties,
                             partition_cols=DataflowSpecUtils.get_partition_cols(bronzeDataflowSpec.partitionColumns),
                             path=bronzeDataflowSpec.targetDetails["path"],
                             comment=f"bronze dlt table{bronzeDataflowSpec.targetDetails['table']}",
                         )
                     )
                 else:
                     dlt_table_with_expectation = dlt.expect_all_or_drop(expect_or_drop_dict)(dlt_table_with_expectation)
@@ -208,14 +229,15 @@
                     and bronzeDataflowSpec.quarantineTargetDetails["partition_columns"]
                 ):
                     q_partition_cols = [bronzeDataflowSpec.quarantineTargetDetails["partition_columns"]]
                 dlt.expect_all_or_drop(expect_or_quarantine_dict)(
                     dlt.table(
                         self.write_to_delta,
                         name=f"{bronzeDataflowSpec.quarantineTargetDetails['table']}",
+                        table_properties=bronzeDataflowSpec.quarantineTableProperties,
                         partition_cols=q_partition_cols,
                         path=bronzeDataflowSpec.quarantineTargetDetails["path"],
                         comment=f"""bronze dlt quarantine_path table
                         {bronzeDataflowSpec.quarantineTargetDetails['table']}""",
                     )
                 )
 
@@ -235,67 +257,78 @@
             modified_schema = StructType([])
             for field in struct_schema.fields:
                 if field.name not in cdc_apply_changes.except_column_list:
                     modified_schema.add(field)
             struct_schema = modified_schema
 
         if cdc_apply_changes.scd_type == "2":
-            for field in struct_schema.fields:
-                if field.name == cdc_apply_changes.sequence_by:
-                    struct_schema.add(StructField("__START_AT", field.dataType))
-                    struct_schema.add(StructField("__END_AT", field.dataType))
-                    break
+            struct_schema.add(StructField("__START_AT", IntegerType()))
+            struct_schema.add(StructField("__END_AT", IntegerType()))
 
         dlt.create_streaming_live_table(
             name=f"{self.dataflowSpec.targetDetails['table']}",
+            table_properties=self.dataflowSpec.tableProperties,
             partition_cols=DataflowSpecUtils.get_partition_cols(self.dataflowSpec.partitionColumns),
             path=self.dataflowSpec.targetDetails["path"],
             schema=struct_schema,
         )
 
+        apply_as_deletes = None
+        if cdc_apply_changes.apply_as_deletes:
+            apply_as_deletes = expr(cdc_apply_changes.apply_as_deletes)
+
+        apply_as_truncates = None
+        if cdc_apply_changes.apply_as_truncates:
+            apply_as_truncates = expr(cdc_apply_changes.apply_as_truncates)
+
         dlt.apply_changes(
             target=f"{self.dataflowSpec.targetDetails['table']}",
             source=self.view_name,
             keys=cdc_apply_changes.keys,
             sequence_by=cdc_apply_changes.sequence_by,
             where=cdc_apply_changes.where,
             ignore_null_updates=cdc_apply_changes.ignore_null_updates,
-            apply_as_deletes=cdc_apply_changes.apply_as_deletes,
-            apply_as_truncates=cdc_apply_changes.apply_as_truncates,
+            apply_as_deletes=apply_as_deletes,
+            apply_as_truncates=apply_as_truncates,
             column_list=cdc_apply_changes.column_list,
             except_column_list=cdc_apply_changes.except_column_list,
             stored_as_scd_type=cdc_apply_changes.scd_type,
+            track_history_column_list=cdc_apply_changes.track_history_column_list,
+            track_history_except_column_list=cdc_apply_changes.track_history_except_column_list
+
         )
 
     def write_bronze(self):
         """Write Bronze tables."""
         bronze_dataflow_spec: BronzeDataflowSpec = self.dataflowSpec
         if bronze_dataflow_spec.dataQualityExpectations:
             self.write_bronze_with_dqe()
         elif bronze_dataflow_spec.cdcApplyChanges:
             self.cdc_apply_changes()
         else:
             dlt.table(
                 self.write_to_delta,
                 name=f"{bronze_dataflow_spec.targetDetails['table']}",
                 partition_cols=DataflowSpecUtils.get_partition_cols(bronze_dataflow_spec.partitionColumns),
+                table_properties=bronze_dataflow_spec.tableProperties,
                 path=bronze_dataflow_spec.targetDetails["path"],
                 comment=f"bronze dlt table{bronze_dataflow_spec.targetDetails['table']}",
             )
 
     def write_silver(self):
         """Write silver tables."""
         silver_dataflow_spec: SilverDataflowSpec = self.dataflowSpec
         if silver_dataflow_spec.cdcApplyChanges:
             self.cdc_apply_changes()
         else:
             dlt.table(
                 self.write_to_delta,
                 name=f"{silver_dataflow_spec.targetDetails['table']}",
                 partition_cols=DataflowSpecUtils.get_partition_cols(silver_dataflow_spec.partitionColumns),
+                table_properties=silver_dataflow_spec.tableProperties,
                 path=silver_dataflow_spec.targetDetails["path"],
                 comment=f"silver dlt table{silver_dataflow_spec.targetDetails['table']}",
             )
 
     def run_dlt(self):
         """Run DLT."""
         logger.info("in run_dlt function")
```

## src/dataflow_spec.py

```diff
@@ -21,20 +21,21 @@
     dataFlowId: str
     dataFlowGroup: str
     sourceFormat: str
     sourceDetails: map
     readerConfigOptions: map
     targetFormat: str
     targetDetails: map
-    writerConfigOptions: map
+    tableProperties: map
     schema: str
     partitionColumns: list
     cdcApplyChanges: str
     dataQualityExpectations: str
     quarantineTargetDetails: map
+    quarantineTableProperties: map
     version: str
     createDate: datetime
     createdBy: str
     updateDate: datetime
     updatedBy: str
 
 
@@ -45,15 +46,15 @@
     dataFlowId: str
     dataFlowGroup: str
     sourceFormat: str
     sourceDetails: map
     readerConfigOptions: map
     targetFormat: str
     targetDetails: map
-    writerConfigOptions: map
+    tableProperties: map
     selectExp: list
     whereClause: list
     partitionColumns: list
     cdcApplyChanges: str
     version: str
     createDate: datetime
     createdBy: str
@@ -65,19 +66,21 @@
 class CDCApplyChanges:
     """CDC ApplyChanges structure."""
 
     keys: list
     sequence_by: str
     where: str
     ignore_null_updates: bool
-    apply_as_deletes: bool
-    apply_as_truncates: bool
+    apply_as_deletes: str
+    apply_as_truncates: str
     column_list: list
     except_column_list: list
     scd_type: str
+    track_history_column_list: list
+    track_history_except_column_list: list
 
 
 class DataflowSpecUtils:
     """A collection of methods for working with DataflowSpec."""
 
     cdc_applychanges_api_mandatory_attributes = ["keys", "sequence_by", "scd_type"]
     cdc_applychanges_api_attributes = [
@@ -86,22 +89,28 @@
         "where",
         "ignore_null_updates",
         "apply_as_deletes",
         "apply_as_truncates",
         "column_list",
         "except_column_list",
         "scd_type",
+        "track_history_column_list",
+        "track_history_except_column_list"
+
     ]
     cdc_applychanges_api_attributes_defaults = {
         "where": None,
         "ignore_null_updates": False,
         "apply_as_deletes": None,
         "apply_as_truncates": None,
         "column_list": None,
         "except_column_list": None,
+        "track_history_column_list": None,
+        "track_history_except_column_list": None
+
     }
 
     @staticmethod
     def _get_dataflow_spec(
         spark: SparkSession,
         layer: str,
         dataflow_spec_df: DataFrame = None,
```

## src/onboard_dataflowspec.py

```diff
@@ -170,30 +170,30 @@
         env = dict_obj["env"]
         silver_transformation_json_df = self.spark.createDataFrame(data=emp_rdd, schema=columns)
         silver_transformation_json_file = onboarding_df.select(f"silver_transformation_json_{env}").dropDuplicates()
 
         silver_transformation_json_files = silver_transformation_json_file.collect()
         for row in silver_transformation_json_files:
             silver_transformation_json_df = silver_transformation_json_df.union(
-                self.spark.read.option("multiline", "true").json(row[f"silver_transformation_json_{env}"])
+                self.spark.read.option("multiline", "true")
+                    .schema(columns)
+                    .json(row[f"silver_transformation_json_{env}"])
             )
 
         logger.info(silver_transformation_json_file)
 
         silver_data_flow_spec_df = silver_transformation_json_df.join(
             silver_data_flow_spec_df,
             silver_transformation_json_df.target_table == silver_data_flow_spec_df.targetDetails["table"],
         )
         silver_dataflow_spec_df = (
             silver_data_flow_spec_df.drop("target_table")  # .drop("path")
             .drop("target_partition_cols")
             .withColumnRenamed("select_exp", "selectExp")
             .withColumnRenamed("where_clause", "whereClause")
-            .withColumn("readerConfigOptions", f.create_map(f.lit(""), f.lit("")))
-            .withColumn("writerConfigOptions", f.create_map(f.lit(""), f.lit("")))
         )
 
         silver_dataflow_spec_df = self.__add_audit_columns(
             silver_dataflow_spec_df,
             {"import_author": dict_obj["import_author"], "version": dict_obj["version"]},
         )
 
@@ -282,14 +282,21 @@
                 bronze_dataflow_spec_df,
                 dict_obj["bronze_dataflowspec_path"],
                 ["dataFlowId"],
                 original_dataflow_df.columns,
             )
         self.register_bronze_dataflow_spec_tables()
 
+    def __delete_none(self, _dict):
+        """Delete None values recursively from all of the dictionaries"""
+        filtered = {k: v for k, v in _dict.items() if v is not None}
+        _dict.clear()
+        _dict.update(filtered)
+        return _dict
+
     def __get_onboarding_file_dataframe(self, onboarding_file_path):
         onboarding_df = None
         if onboarding_file_path.lower().endswith(".json"):
             onboarding_df = self.spark.read.option("multiline", "true").json(onboarding_file_path)
             self.onboard_file_type = "json"
             onboarding_df_dupes = onboarding_df.groupBy("data_flow_id").count().filter("count > 1")
             if len(onboarding_df_dupes.head(1)) > 0:
@@ -329,14 +336,19 @@
         """
         ddlSchemaStr = self.spark.read.text(paths=metadata_file, wholetext=True).collect()[0]["value"]
         spark_schema = T._parse_datatype_string(ddlSchemaStr)
         logger.info(spark_schema)
         schema = json.dumps(spark_schema.jsonValue())
         return schema
 
+    def __validate_mandatory_fields(self, onboarding_row, mandatory_fields):
+        for field in mandatory_fields:
+            if not onboarding_row[field]:
+                raise Exception(f"Missing field={field} in onboarding_row")
+
     def __get_bronze_dataflow_spec_dataframe(self, onboarding_df, env):
         """Get bronze dataflow spec method will convert onboarding dataframe to Bronze Dataflowspec dataframe.
 
         Args:
             onboarding_df ([type]): [description]
             spark (SparkSession): [description]
 
@@ -347,77 +359,78 @@
             "dataFlowId",
             "dataFlowGroup",
             "sourceFormat",
             "sourceDetails",
             "readerConfigOptions",
             "targetFormat",
             "targetDetails",
-            "writerConfigOptions",
+            "tableProperties",
             "schema",
             "partitionColumns",
             "cdcApplyChanges",
             "dataQualityExpectations",
             "quarantineTargetDetails",
+            "quarantineTableProperties"
         ]
         data_flow_spec_schema = StructType(
             [
                 StructField("dataFlowId", StringType(), True),
                 StructField("dataFlowGroup", StringType(), True),
                 StructField("sourceFormat", StringType(), True),
                 StructField("sourceDetails", MapType(StringType(), StringType(), True), True),
                 StructField(
                     "readerConfigOptions",
                     MapType(StringType(), StringType(), True),
                     True,
                 ),
                 StructField("targetFormat", StringType(), True),
                 StructField("targetDetails", MapType(StringType(), StringType(), True), True),
-                StructField(
-                    "writerConfigOptions",
-                    MapType(StringType(), StringType(), True),
-                    True,
-                ),
+                StructField("tableProperties", MapType(StringType(), StringType(), True), True),
                 StructField("schema", StringType(), True),
                 StructField("partitionColumns", ArrayType(StringType(), True), True),
                 StructField("cdcApplyChanges", StringType(), True),
                 StructField("dataQualityExpectations", StringType(), True),
                 StructField("quarantineTargetDetails", MapType(StringType(), StringType(), True), True),
+                StructField("quarantineTableProperties", MapType(StringType(), StringType(), True), True)
             ]
         )
         data = []
         onboarding_rows = onboarding_df.collect()
+        mandatory_fields = ["data_flow_id", "data_flow_group", "source_details", f"bronze_database_{env}",
+                            "bronze_table", "bronze_reader_options", f"bronze_table_path_{env}"]
         for onboarding_row in onboarding_rows:
+            self.__validate_mandatory_fields(onboarding_row, mandatory_fields)
             bronze_data_flow_spec_id = onboarding_row["data_flow_id"]
             bronze_data_flow_spec_group = onboarding_row["data_flow_group"]
             if "source_format" not in onboarding_row:
                 raise Exception(f"Source format not provided for row={onboarding_row}")
 
             source_format = onboarding_row["source_format"]
-            if source_format.lower() not in ["cloudfiles", "eventhub", "kafka"]:
+            if source_format.lower() not in ["cloudfiles", "eventhub", "kafka", "delta"]:
                 raise Exception(f"Source format {source_format} not supported in DLT-META! row={onboarding_row}")
             source_details = {}
             bronze_reader_config_options = {}
             schema = None
             bronze_reader_options_json = onboarding_row["bronze_reader_options"]
             if bronze_reader_options_json:
-                bronze_reader_config_options = bronze_reader_options_json.asDict()
+                bronze_reader_config_options = self.__delete_none(bronze_reader_options_json.asDict())
             source_details_json = onboarding_row["source_details"]
             if source_details_json:
-                source_details_file = source_details_json.asDict()
-                if source_format.lower() == "cloudfiles":
+                source_details_file = self.__delete_none(source_details_json.asDict())
+                if source_format.lower() == "cloudfiles" or source_format.lower() == "delta":
                     if f"source_path_{env}" in source_details_file:
                         source_details["path"] = source_details_file[f"source_path_{env}"]
                     if "source_database" in source_details_file:
                         source_details["source_database"] = source_details_file["source_database"]
                     if "source_table" in source_details_file:
                         source_details["source_table"] = source_details_file["source_table"]
                 elif source_format.lower() == "eventhub" or source_format.lower() == "kafka":
                     source_details = source_details_file
-                if "source_schema_path" in source_details:
-                    source_schema_path = source_details["source_schema_path"]
+                if "source_schema_path" in source_details_file:
+                    source_schema_path = source_details_file["source_schema_path"]
                     if source_schema_path:
                         if self.bronze_schema_mapper is not None:
                             schema = self.bronze_schema_mapper(source_schema_path, self.spark)
                         else:
                             schema = self.__get_bronze_schema(source_schema_path)
                     else:
                         logger.info(f"no input schema provided for row={onboarding_row}")
@@ -428,26 +441,29 @@
 
             bronze_target_details = {
                 "database": onboarding_row["bronze_database_{}".format(env)],
                 "table": onboarding_row["bronze_table"],
                 "path": onboarding_row["bronze_table_path_{}".format(env)],
             }
 
-            bronze_writer_config_options = {}
+            bronze_table_properties = {}
+            if "bronze_table_properties" in onboarding_row and onboarding_row["bronze_table_properties"]:
+                bronze_table_properties = self.__delete_none(onboarding_row["bronze_table_properties"].asDict())
 
             partition_columns = [""]
             if "bronze_partition_columns" in onboarding_row and onboarding_row["bronze_partition_columns"]:
                 partition_columns = [onboarding_row["bronze_partition_columns"]]
 
             cdc_apply_changes = None
             if "bronze_cdc_apply_changes" in onboarding_row and onboarding_row["bronze_cdc_apply_changes"]:
-                self.__validateApplyChanges(onboarding_row, "bronze")
-                cdc_apply_changes = json.dumps(onboarding_row["bronze_cdc_apply_changes"].asDict())
+                self.__validate_apply_changes(onboarding_row, "bronze")
+                cdc_apply_changes = json.dumps(self.__delete_none(onboarding_row["bronze_cdc_apply_changes"].asDict()))
             data_quality_expectations = None
             quarantine_target_details = {}
+            quarantine_table_properties = {}
             if f"bronze_data_quality_expectations_json_{env}" in onboarding_row:
                 bronze_data_quality_expectations_json = onboarding_row[f"bronze_data_quality_expectations_json_{env}"]
                 if bronze_data_quality_expectations_json:
                     data_quality_expectations = (
                         self.__get_data_quality_expecations(bronze_data_quality_expectations_json))
                     if onboarding_row["bronze_quarantine_table"]:
                         quarantine_table_partition_columns = ""
@@ -458,37 +474,44 @@
                             quarantine_table_partition_columns = onboarding_row["bronze_quarantine_table_partitions"]
                         quarantine_target_details = {
                             "database": onboarding_row[f"bronze_database_quarantine_{env}"],
                             "table": onboarding_row["bronze_quarantine_table"],
                             "path": onboarding_row[f"bronze_quarantine_table_path_{env}"],
                             "partition_columns": quarantine_table_partition_columns,
                         }
+                        if (
+                            "bronze_quarantine_table_properties" in onboarding_row
+                            and onboarding_row["bronze_quarantine_table_properties"]
+                        ):
+                            quarantine_table_properties = self.__delete_none(
+                                onboarding_row["bronze_quarantine_table_properties"].asDict())
             bronze_row = (
                 bronze_data_flow_spec_id,
                 bronze_data_flow_spec_group,
                 source_format,
                 source_details,
                 bronze_reader_config_options,
                 bronze_target_format,
                 bronze_target_details,
-                bronze_writer_config_options,
+                bronze_table_properties,
                 schema,
                 partition_columns,
                 cdc_apply_changes,
                 data_quality_expectations,
                 quarantine_target_details,
+                quarantine_table_properties
             )
             data.append(bronze_row)
             # logger.info(bronze_parition_columns)
 
         data_flow_spec_rows_df = self.spark.createDataFrame(data, data_flow_spec_schema).toDF(*data_flow_spec_columns)
 
         return data_flow_spec_rows_df
 
-    def __validateApplyChanges(self, onboarding_row, layer):
+    def __validate_apply_changes(self, onboarding_row, layer):
         cdc_apply_changes = onboarding_row[f"{layer}_cdc_apply_changes"]
         json_cdc_apply_changes = cdc_apply_changes.asDict()
         logger.info(f"actual mergeInfo={json_cdc_apply_changes}")
         payload_keys = json_cdc_apply_changes.keys()
         missing_cdc_payload_keys = set(DataflowSpecUtils.cdc_applychanges_api_attributes).difference(payload_keys)
         logger.info(
             f"""missing cdc payload keys:{missing_cdc_payload_keys}
@@ -538,15 +561,15 @@
             "dataFlowId",
             "dataFlowGroup",
             "sourceFormat",
             "sourceDetails",
             "readerConfigOptions",
             "targetFormat",
             "targetDetails",
-            "writerConfigOptions",
+            "tableProperties",
             "partitionColumns",
             "cdcApplyChanges",
         ]
         data_flow_spec_schema = StructType(
             [
                 StructField("dataFlowId", StringType(), True),
                 StructField("dataFlowGroup", StringType(), True),
@@ -555,28 +578,27 @@
                 StructField(
                     "readerConfigOptions",
                     MapType(StringType(), StringType(), True),
                     True,
                 ),
                 StructField("targetFormat", StringType(), True),
                 StructField("targetDetails", MapType(StringType(), StringType(), True), True),
-                StructField(
-                    "writerConfigOptions",
-                    MapType(StringType(), StringType(), True),
-                    True,
-                ),
+                StructField("tableProperties", MapType(StringType(), StringType(), True), True),
                 StructField("partitionColumns", ArrayType(StringType(), True), True),
                 StructField("cdcApplyChanges", StringType(), True),
             ]
         )
         data = []
 
         onboarding_rows = onboarding_df.collect()
+        mandatory_fields = ["data_flow_id", "data_flow_group", "source_details", f"silver_database_{env}",
+                            "silver_table", f"silver_table_path_{env}", f"silver_transformation_json_{env}"]
 
         for onboarding_row in onboarding_rows:
+            self.__validate_mandatory_fields(onboarding_row, mandatory_fields)
             silver_data_flow_spec_id = onboarding_row["data_flow_id"]
             silver_data_flow_spec_group = onboarding_row["data_flow_group"]
             silver_reader_config_options = {}
 
             silver_target_format = "delta"
 
             bronze_target_details = {
@@ -586,35 +608,38 @@
             }
             silver_target_details = {
                 "database": onboarding_row["silver_database_{}".format(env)],
                 "table": onboarding_row["silver_table"],
                 "path": onboarding_row["silver_table_path_{}".format(env)],
             }
 
-            silver_writer_config_options = {}
+            silver_table_properties = {}
+            if "silver_table_properties" in onboarding_row and onboarding_row["silver_table_properties"]:
+                silver_table_properties = self.__delete_none(onboarding_row["silver_table_properties"].asDict())
+
+            silver_parition_columns = [""]
+            if "silver_partition_columns" in onboarding_row and onboarding_row["silver_partition_columns"]:
+                silver_parition_columns = [onboarding_row["silver_partition_columns"]]
 
-            silver_parition_columns = [onboarding_row["silver_partition_columns"]]  # TODO correct typo in tsv
             silver_cdc_apply_changes = None
             if "silver_cdc_apply_changes" in onboarding_row and onboarding_row["silver_cdc_apply_changes"]:
-                self.__validateApplyChanges(onboarding_row, "silver")
+                self.__validate_apply_changes(onboarding_row, "silver")
                 silver_cdc_apply_changes_row = onboarding_row["silver_cdc_apply_changes"]
                 if self.onboard_file_type == "json":
-                    silver_cdc_apply_changes = json.dumps(silver_cdc_apply_changes_row.asDict())
-                elif self.onboard_file_type == "csv" and len(silver_cdc_apply_changes_row.strip()) > 0:
-                    silver_cdc_apply_changes = json.loads(silver_cdc_apply_changes_row)
+                    silver_cdc_apply_changes = json.dumps(self.__delete_none(silver_cdc_apply_changes_row.asDict()))
 
             silver_row = (
                 silver_data_flow_spec_id,
                 silver_data_flow_spec_group,
                 "delta",
                 bronze_target_details,
                 silver_reader_config_options,
                 silver_target_format,
                 silver_target_details,
-                silver_writer_config_options,
+                silver_table_properties,
                 silver_parition_columns,
                 silver_cdc_apply_changes,
             )
             data.append(silver_row)
             logger.info(f"silver_data ==== {data}")
 
         data_flow_spec_rows_df = self.spark.createDataFrame(data, data_flow_spec_schema).toDF(*data_flow_spec_columns)
```

## src/pipeline_readers.py

```diff
@@ -27,15 +27,15 @@
         Returns:
             DataFrame: _description_
         """
         logger.info("In read_dlt_cloud_files func")
         source_path = bronze_dataflow_spec.sourceDetails["path"]
         reader_config_options = bronze_dataflow_spec.readerConfigOptions
 
-        if schema_json:
+        if schema_json and bronze_dataflow_spec.sourceFormat.lower() != "delta":
             schema = StructType.fromJson(schema_json)
             return (
                 spark.readStream.format(bronze_dataflow_spec.sourceFormat)
                 .options(**reader_config_options)
                 .schema(schema)
                 .load(source_path)
             )
@@ -43,14 +43,40 @@
             return (
                 spark.readStream.format(bronze_dataflow_spec.sourceFormat)
                 .options(**reader_config_options)
                 .load(source_path)
             )
 
     @staticmethod
+    def read_dlt_delta(spark, bronze_dataflow_spec) -> DataFrame:
+        """Read dlt delta.
+
+        Args:
+            spark (_type_): _description_
+            bronze_dataflow_spec (_type_): _description_
+        Returns:
+            DataFrame: _description_
+        """
+        logger.info("In read_dlt_cloud_files func")
+        source_path = bronze_dataflow_spec.sourceDetails["path"]
+        reader_config_options = bronze_dataflow_spec.readerConfigOptions
+
+        if reader_config_options and len(reader_config_options) > 0:
+            return (
+                spark.readStream.format(bronze_dataflow_spec.sourceFormat)
+                .options(**reader_config_options)
+                .load(source_path)
+            )
+        else:
+            return (
+                spark.readStream.format(bronze_dataflow_spec.sourceFormat)
+                .load(source_path)
+            )
+
+    @staticmethod
     def get_db_utils(spark):
         """Get databricks utils using DBUtils package."""
         from pyspark.dbutils import DBUtils
         return DBUtils(spark)
 
     @staticmethod
     def read_kafka(spark, bronze_dataflow_spec, schema_json) -> DataFrame:
@@ -132,11 +158,16 @@
                     "kafka.ssl.truststore.location": ssl_truststore_location,
                     "kafka.ssl.keystore.location": ssl_keystore_location,
                     "kafka.ssl.keystore.password": dbutils.secrets.get(keystore_scope, keystore_key),
                     "kafka.ssl.truststore.password": dbutils.secrets.get(truststore_scope, truststore_key)
                 }
                 kafka_options = {**kafka_base_ops, **kafka_ssl_conn, **bronze_dataflow_spec.readerConfigOptions}
             else:
-                raise Exception(f"Kafka ssl options not provided! provided options are :{source_details_map}")
+                params = ["kafka.ssl.truststore.secrets.scope",
+                          "kafka.ssl.truststore.secrets.key",
+                          "kafka.ssl.keystore.secrets.scope",
+                          "kafka.ssl.keystore.secrets.key"
+                          ]
+                raise Exception(f"Kafka ssl required params are: {params}! provided options are :{source_details_map}")
         else:
             kafka_options = {**kafka_base_ops, **bronze_dataflow_spec.readerConfigOptions}
         return kafka_options
```

## Comparing `dlt_meta-0.0.1.dist-info/LICENSE.txt` & `dlt_meta-0.0.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

