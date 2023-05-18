# Comparing `tmp/sql-pylib-0.12.tar.gz` & `tmp/sql-pylib-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql-pylib-0.12.tar", last modified: Thu May 18 08:33:18 2023, max compression
+gzip compressed data, was "sql-pylib-0.13.tar", last modified: Thu May 18 09:04:50 2023, max compression
```

## Comparing `sql-pylib-0.12.tar` & `sql-pylib-0.13.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 docquity_prince   (501) staff       (20)        0 2023-05-18 08:33:18.117627 sql-pylib-0.12/
--rw-r--r--   0 docquity_prince   (501) staff       (20)     2862 2023-05-18 08:33:18.117394 sql-pylib-0.12/PKG-INFO
--rw-r--r--   0 docquity_prince   (501) staff       (20)     2403 2023-05-18 08:31:43.000000 sql-pylib-0.12/README.md
--rw-r--r--   0 docquity_prince   (501) staff       (20)       38 2023-05-18 08:33:18.117694 sql-pylib-0.12/setup.cfg
--rw-r--r--   0 docquity_prince   (501) staff       (20)      814 2023-05-18 08:33:15.000000 sql-pylib-0.12/setup.py
-drwxr-xr-x   0 docquity_prince   (501) staff       (20)        0 2023-05-18 08:33:18.105964 sql-pylib-0.12/sql_pylib/
--rw-r--r--   0 docquity_prince   (501) staff       (20)        0 2022-10-27 02:59:22.000000 sql-pylib-0.12/sql_pylib/__init__.py
--rw-r--r--   0 docquity_prince   (501) staff       (20)     3863 2022-10-27 02:59:22.000000 sql-pylib-0.12/sql_pylib/database_download_upload.py
--rw-r--r--   0 docquity_prince   (501) staff       (20)     1538 2022-10-27 02:59:22.000000 sql-pylib-0.12/sql_pylib/load_from_redshift_to_pandas.py
--rw-r--r--   0 docquity_prince   (501) staff       (20)    33155 2023-05-18 07:21:12.000000 sql-pylib-0.12/sql_pylib/sql_builder.py
-drwxr-xr-x   0 docquity_prince   (501) staff       (20)        0 2023-05-18 08:33:18.117093 sql-pylib-0.12/sql_pylib.egg-info/
--rw-r--r--   0 docquity_prince   (501) staff       (20)     2862 2023-05-18 08:33:17.000000 sql-pylib-0.12/sql_pylib.egg-info/PKG-INFO
--rw-r--r--   0 docquity_prince   (501) staff       (20)      309 2023-05-18 08:33:18.000000 sql-pylib-0.12/sql_pylib.egg-info/SOURCES.txt
--rw-r--r--   0 docquity_prince   (501) staff       (20)        1 2023-05-18 08:33:17.000000 sql-pylib-0.12/sql_pylib.egg-info/dependency_links.txt
--rw-r--r--   0 docquity_prince   (501) staff       (20)       90 2023-05-18 08:33:17.000000 sql-pylib-0.12/sql_pylib.egg-info/requires.txt
--rw-r--r--   0 docquity_prince   (501) staff       (20)       10 2023-05-18 08:33:17.000000 sql-pylib-0.12/sql_pylib.egg-info/top_level.txt
+drwxr-xr-x   0 docquity_prince   (501) staff       (20)        0 2023-05-18 09:04:50.122173 sql-pylib-0.13/
+-rw-r--r--   0 docquity_prince   (501) staff       (20)     2862 2023-05-18 09:04:50.121948 sql-pylib-0.13/PKG-INFO
+-rw-r--r--   0 docquity_prince   (501) staff       (20)     2403 2023-05-18 08:31:43.000000 sql-pylib-0.13/README.md
+-rw-r--r--   0 docquity_prince   (501) staff       (20)       38 2023-05-18 09:04:50.122242 sql-pylib-0.13/setup.cfg
+-rw-r--r--   0 docquity_prince   (501) staff       (20)      814 2023-05-18 09:04:27.000000 sql-pylib-0.13/setup.py
+drwxr-xr-x   0 docquity_prince   (501) staff       (20)        0 2023-05-18 09:04:50.110784 sql-pylib-0.13/sql_pylib/
+-rw-r--r--   0 docquity_prince   (501) staff       (20)        0 2022-10-27 02:59:22.000000 sql-pylib-0.13/sql_pylib/__init__.py
+-rw-r--r--   0 docquity_prince   (501) staff       (20)     3829 2023-05-18 09:02:05.000000 sql-pylib-0.13/sql_pylib/database_download_upload.py
+-rw-r--r--   0 docquity_prince   (501) staff       (20)     1538 2022-10-27 02:59:22.000000 sql-pylib-0.13/sql_pylib/load_from_redshift_to_pandas.py
+-rw-r--r--   0 docquity_prince   (501) staff       (20)    24732 2023-05-18 09:03:37.000000 sql-pylib-0.13/sql_pylib/sql_builder.py
+drwxr-xr-x   0 docquity_prince   (501) staff       (20)        0 2023-05-18 09:04:50.121686 sql-pylib-0.13/sql_pylib.egg-info/
+-rw-r--r--   0 docquity_prince   (501) staff       (20)     2862 2023-05-18 09:04:49.000000 sql-pylib-0.13/sql_pylib.egg-info/PKG-INFO
+-rw-r--r--   0 docquity_prince   (501) staff       (20)      309 2023-05-18 09:04:50.000000 sql-pylib-0.13/sql_pylib.egg-info/SOURCES.txt
+-rw-r--r--   0 docquity_prince   (501) staff       (20)        1 2023-05-18 09:04:49.000000 sql-pylib-0.13/sql_pylib.egg-info/dependency_links.txt
+-rw-r--r--   0 docquity_prince   (501) staff       (20)       90 2023-05-18 09:04:49.000000 sql-pylib-0.13/sql_pylib.egg-info/requires.txt
+-rw-r--r--   0 docquity_prince   (501) staff       (20)       10 2023-05-18 09:04:49.000000 sql-pylib-0.13/sql_pylib.egg-info/top_level.txt
```

### Comparing `sql-pylib-0.12/PKG-INFO` & `sql-pylib-0.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-pylib
-Version: 0.12
+Version: 0.13
 Summary: Custom Python library for standard SQL tasks
 Home-page: https://github.com/PrinceJavier/sql_pylib
 Author: Prince Javier
 Author-email: othepjavier@gmail.com
 License: MIT
 Keywords: sql python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sql-pylib-0.12/README.md` & `sql-pylib-0.13/README.md`

 * *Files identical despite different names*

### Comparing `sql-pylib-0.12/setup.py` & `sql-pylib-0.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sql-pylib',
-    version='0.12',
+    version='0.13',
     packages=find_packages(),
     description='Custom Python library for standard SQL tasks',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Prince Javier',
     author_email='othepjavier@gmail.com',
     url='https://github.com/PrinceJavier/sql_pylib',
```

### Comparing `sql-pylib-0.12/sql_pylib/database_download_upload.py` & `sql-pylib-0.13/sql_pylib/database_download_upload.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 from sqlalchemy import types
 
 def create_table_in_redshift(table_name, 
                              columns, 
                              credentials,
                              primary_key = None, 
                              sql_type='postgresql',
-                             schema='docquity_flat_badata', 
+                             schema='schema_name', 
                              delete_existing=False):
     
     """
     Create new table in redshift    
     Prereq: psycopg2 package
     Inputs
         table_name (str) - name of table
         columns (list) - [('id', 'BIGINT'), ('col2', 'DATE')]
         credentials (dict) - Redshift credentials dict(dbname, host, port, user, password)
         primary_key (str) - default=None, column name of primary key e.g. 'id'
         sql_type='postgresql'  or 'mysql'
-        schema (str) - default = docquity_flat_data. schema where we save the table
+        schema (str) - default = schema_name. schema where we save the table
         delete_existing (bool) - default=False. WARNING: will delete existing table and replace
     Outputs
         new table created in Redshift
     """
     
     # convert column list to SQL language
     cols_str = ',\n'.join([' '.join(i) for i in columns])
@@ -78,24 +78,24 @@
 
 
 
 def insert_pandas_data_to_redshift_table(df, 
                                          table_name, 
                                          credentials, 
                                          chunksize=500,
-                                         schema="docquity_flat_badata"):
+                                         schema="schema_name"):
     """
     Insert pandas data to existing redshift table
     prereq: conda install sqlalchemy
     Inputs
         df - pandas dataframe
         table_name (str)
         credentials (dict) - redshift credentials
         chunksize(int) - default = 500, how many rows to upload at a time
-        schema (str) - default = "docquity_flat_badata"
+        schema (str) - default = "schema_name"
     Output
         insert data into table in redshift
     """    
     user = credentials['user']
     host = credentials['host']
     dbname = credentials['dbname']
     port = credentials['port']
```

### Comparing `sql-pylib-0.12/sql_pylib/load_from_redshift_to_pandas.py` & `sql-pylib-0.13/sql_pylib/load_from_redshift_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sql-pylib-0.12/sql_pylib/sql_builder.py` & `sql-pylib-0.13/sql_pylib/sql_builder.py`

 * *Files 25% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         self.has_cols = True
         
         return self
     
 
     def from_table(self, source, alias=None):
         """
-        source (str/SQLBuilder) - table name, e.g. "docquity_db.user_master" or it can be
+        source (str/SQLBuilder) - table name, e.g. "schema_name.table_name" or it can be
                     a query, e.g. "SELECT * FROM table" or an SQLBuilder query object
         alias (str) - default=None. alias of this table, otherwise, automatically add new one
         """
         
         # if source is SQLBuilder object
         if type(source) == type(self):
             source = source.query # get the string query version
@@ -309,15 +309,15 @@
     # CHECK COLUMN NAMES AND TABLE NAMES
     ########################################    
     
     def get_table_names(self, schema):
         """
         Get table names given schema
         Input
-            schema (str) - "docquity_db" or "docquity_analytics"
+            schema (str) - schema name
         Returns
             query for list of table names in schema
         """
         query = f"""
         select t.table_name
         from information_schema.tables t
         where t.table_schema = '{schema}'
@@ -446,25 +446,25 @@
     
     # create new empty table
     def create_table(self,
                      table_name,
                      columns, 
                      primary_key = None, 
                      sql_type='postgresql',
-                     schema='docquity_flat_badata', 
+                     schema='schema_name', 
                      delete_existing=False):
         
         """
         Create new table in redshift    
         Inputs
             table_name (str) - name of table
             columns (list) - [('id', 'BIGINT'), ('col2', 'DATE')]
             primary_key (str) - default=None, column name of primary key e.g. 'id'
             sql_type='postgresql'  or 'mysql'
-            schema (str) - default = docquity_flat_data. schema where we save the table
+            schema (str) - default = schema_name. schema where we save the table
             delete_existing (bool) - default=False. WARNING: will delete existing table and replace
         Outputs
             new table created in Redshift
         """        
     
         db.create_table_in_redshift(table_name, 
                                     columns, 
@@ -473,28 +473,28 @@
                                     delete_existing = delete_existing)    
     
     
     # create and upload new table from pandas dataframe
     def upload_table(self, 
                      df, 
                      table_name, 
-                     schema = 'docquity_flat_badata', 
+                     schema = 'schema_name', 
                      chunksize = 1000,                     
                      delete_existing = False,
                      varchar_len = 1024,
                      primary_key = None,                     
                     ):
         """
         creates new table on redshift based on pandas dataframe
         upload data to table on redshift
         
         Args:
             df - Pandas dataframe
             table_name - string. name of table on redshift
-            schema - string. default = 'docquity_flat_badata'. schema where to create table.
+            schema - string. default = 'schema_name'. schema where to create table.
             chunk_size - int. default = 1000. how many rows to upload at a time
             delete_existing - default = False. whether to delete the existing table
             varchar_len - default = 1024. the lenght of VARCHAR(<length>)
             primary_key - default = None. string. which column to use as primary key
         Returns
             None
         """
@@ -534,23 +534,23 @@
                                                  schema=schema
                                                )
         
     # insert to existing table
     def insert_to_table(self,
                         df, 
                         table_name,
-                        schema="docquity_flat_badata",                       
+                        schema="schema_name",                       
                         chunksize=1000, ):  
         """
         Insert pandas data to existing redshift table
         Inputs
             df - pandas dataframe
             table_name (str)
             chunksize(int) - default = 1000, how many rows to upload at a time
-            schema (str) - default = "docquity_flat_badata"
+            schema (str) - default = "schema_name"
         Output
             insert data into table in redshift
         """            
         # insert to created table
         db.insert_pandas_data_to_redshift_table(df, 
                                                  table_name, 
                                                  self.credentials, 
@@ -560,24 +560,24 @@
     
     ######################################## 
     # GENERATING QUERY FROM EXISTING TABLE
     ########################################        
     
     # GENERAL QUERY
     def make_query(self,
-                    schema='docquity_db', 
+                    schema='schema_name', 
                     table_name=None,
                     cols = None,
                     filters=None,
                     limit=None):
         """
         Load general query
         
         Args:
-            schema - 'docquity_db', can change to 'docquity_db_stage'
+            schema - schema name
             cols - None, if None, download all accessible cols. Otherwise, provide a list, ['col1', 'col2']
             filters = None, string, apply certain filters
             limit - None, can change to how many rows to query, e.g. 5
             
         Returns:
             query object. To get text query, run <output_var>.query
         """
@@ -708,226 +708,10 @@
                     where status = 'Running';"""
         return query
     
     # TERMINATING RUNNING QUERIES
     def terminate_process(self, process_id):
         q = f"SELECT pg_terminate_backend({process_id})"
         return q    
-
-#     # DEPRECATE THIS    
-#     # PREPROCESSING
-#     def conv_to_date(self, column, datatype, new_name=None):
-#         """
-#         column (str) - column name
-#         datatype (str) - 'str', 'epoch_sec', 'epoch_ms'
-#         new_name (str) - new column name, default=None - don't add "AS <name>"
-#         """
-        
-#         if datatype == 'str':
-#             s = f"TO_DATE({column}, 'YYYY-MM-DD')"
-            
-#         elif datatype == 'epoch_sec':
-#             s = f"(TIMESTAMP 'epoch' + {column} * INTERVAL '1 second')"
-            
-#         elif datatype == 'epoch_ms':
-#             s = f"(TIMESTAMP 'epoch' + {column} * INTERVAL '0.001 second')"            
-        
-#         if new_name is not None:        
-#             # new query
-#             s = s + f" AS {new_name}"
-        
-#         return s
-
-#     # DEPRECATE THIS
-#     # PIVOT TABLE
-    
-#     def make_pivot_query(self, table, id_cols, value_cols, category_cols, agg_method='sum'):
-#         """
-#         table (str) - table name or subquery e.g. (SELECT * FROM table)    
-#         id_cols (list) - e.g. ['user_id', 'product_type']
-#         value_cols (list) - columns of values to aggregate
-#         category_cols (list) - categories to use as new columns after pivoting
-#         agg_method (str) - default='sum', can be 'min', 'max', 'avg'
-#         """
-
-#         credentials = self.credentials
-#         txn_col_names = []
-#         ta_pivot_tables = []
-#         for txn in value_cols:
-#             for category in category_cols:        
-#                 # unique values in category
-#                 q = f"SELECT DISTINCT({category}) FROM {table}"
-#                 unique_vals1 = load_from_redshift_to_pandas(q, credentials).values.flatten()
-
-#                 # RUN THIS FIX!!!
-#                 # get unique values in each category column
-#                 unique_vals2 = list(set(unique_vals1))
-#                 unique_vals = str(tuple(unique_vals2)).replace(",)", ")")
-
-#                 # generate column names for new transactions
-#                 txn_col_names_ = []
-#                 for uv in unique_vals2:
-#                     txn_col_names_ += [uv+"_"+category+"_"+txn+f"_{agg_method}"]
-
-
-#                 # generate initial query
-
-#                 q_1 = (SQLBuilder()
-#                       .select(id_cols + [category] + [txn]) # make sure there are no null vaues in category
-#                       .from_table(table)
-#                       )
-
-#                 # pivot query
-#                 q_pivot = f"""
-#                 SELECT *
-#                 FROM ({q_1.query})
-#                 PIVOT
-#                 (
-#                 SUM({txn}) AS {category}_{txn}_{agg_method}
-#                 FOR {category} IN {unique_vals} -- replace null with no_value
-#                 )
-#                 """
-                
-#                 # print(q_pivot)
-                
-#                 #FOR {category} IN (SELECT DISTINCT {category} FROM {q_content}) -- pure SQL, but Python implementation above is more flexible   
-
-#                 # append pivot queries
-#                 txn_col_names += txn_col_names_
-#                 ta_pivot_tables.append(q_pivot)
-
-#          # query to LEFT join all pivot subtables to generate final table
-#         id_cols2 = [f"ta.{i}" for i in id_cols]
-#         txn_col_names = txn_col_names
-
-#         q = (SQLBuilder()
-#             .select(id_cols2 + txn_col_names)
-#              .from_table(ta_pivot_tables[0], alias='ta')
-#          )
-
-#         if len(ta_pivot_tables) > 1:
-#             for pivot_table in ta_pivot_tables[1:]:
-#                 q = (q.join(pivot_table,
-#                            how='left',
-#                            on_left=id_cols,
-#                            on_right=id_cols   
-#                            ))    
-
-#         return q    
-
-    # # DEPRECATE THIS
-    # # STANDARD QUERIES
-    # def user_master(self,
-#                     schema='docquity_db', 
-#                     cols = None,
-#                     apply_filters=False,
-#                     limit=None):
-#         """
-#         Load standard query for user_master
-        
-#         Args:
-#             schema - 'docquity_db', can change to 'docquity_db_stage'
-#             cols - None, if None, download all accessible cols. Otherwise, provide a list, ['col1', 'col2']
-#             apply_filters = False, apply default filters
-#             limit - None, can change to how many rows to query, e.g. 5
-            
-#         Returns:
-#             query object. To get text query, run <output_var>.query
-#         """
-#         table_name = 'user_master'
-
-#         # # get cols
-#         q = SQLBuilder().get_column_names(table_name, schema=schema)
-
-#         if cols is None:
-#             # cols = ["*"] # everything - will throw an error if no permissions on some cols
-#             cols = list(load_from_redshift_to_pandas(q, self.credentials).column_name.values.flatten())
-
-#         table = f"{schema}.{table_name}"
-#         sql_um = (SQLBuilder().select(cols)
-#                       .from_table(table)
-#                  )
-
-#         if apply_filters:
-#             sql_um = (sql_um.where(self.user_filter)
-#                             .condition_and(self.track_id_filter))
-
-#         if limit is not None:
-#             sql_um = sql_um.limit(limit)
-        
-#         return sql_um
-    
-    
-#     def user_demog_feats(self,
-#                         schema='docquity_db', 
-#                         cols = None,
-#                         apply_filters=False,
-#                         limit=None):
-#         """
-#         Load standard query for preprocessed demographics info for users
-#         tables used: user_master, speciality_master, speciality_list, country_master
-#         schema - 'docquity_db', can change to 'docquity_db_stage'
-        
-#         Args:
-#             schema - 'docquity_db', can change to 'docquity_db_stage'
-#             cols - None, if None, download all accessible cols. Otherwise, provide a list, ['col1', 'col2']
-#             apply_filters = False, apply default filters
-#             limit - None, can change to how many rows to query, e.g. 5
-            
-#         Returns:
-#             query object. To get text query, run <output_var>.query
-#         """    
-    
-#         # query user master 1st
-#         q_um = self.user_master(
-#                     schema=schema, 
-#                     cols = None,
-#                     apply_filters=apply_filters,
-#                     limit=None)
-    
-    
-#         # TO TURN THIS TO SQL BUILDER SEPARATE FXN
-#         q_spec = f"""SELECT listagg(SL.speciality_name)
-#                    FROM {schema}.speciality_master SM
-#                    INNER JOIN {schema}.speciality_list SL ON SM.speciality_id=SL.speciality_id
-#                    WHERE SM.user_id=UM.id
-#                      AND SM.status='1'
-#                      AND SL.status='Active'
-#                      AND SM.is_primary='1'"""
-    
-#         # FOR AGE, ETC, LEFT JOIN THEN GET AVG
-#         q_user_demog = f"""
-#         SELECT UM.id AS user_id,
-#                UM.user_report_id,
-#                UM.ic_number,       
-#                DATE_TRUNC('day', UM.created_on) AS reg_date,
-#                UM.gender,
-#                UM.user_type,
-
-#                CASE WHEN DATEDIFF(day, UM.created_on, CURRENT_DATE) < 0 
-#                    THEN NULL 
-#                    ELSE DATEDIFF(day, UM.created_on, CURRENT_DATE)
-#                    END AS age_in_app,
-#                CASE WHEN DATEDIFF(year, UM.date_of_birth, CURRENT_DATE) > 120 OR DATEDIFF(year, UM.date_of_birth, CURRENT_DATE) < 18
-#                    THEN NULL 
-#                    ELSE DATEDIFF(year, UM.date_of_birth, CURRENT_DATE) END AS user_age,
-#                UM.device_type,
-#                UM.permission,
-#                CM.country,       
-#               ({q_spec}) AS speciality
-#         FROM ({q_um.query}) UM
-#         LEFT JOIN ({q_um.query}) CM ON UM.country_id = CM.id
-#         --LEFT JOIN {schema}.city_master CT ON UM.city_id = CT.city_id
-#         """
-        
-#         sql = (SQLBuilder()
-#               .select(['*'])
-#               .from_table(q_user_demog)
-#               )
-
-#         if limit is not None:
-#             sql = sql.limit(limit)
-        
-#         return sql
```

### Comparing `sql-pylib-0.12/sql_pylib.egg-info/PKG-INFO` & `sql-pylib-0.13/sql_pylib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-pylib
-Version: 0.12
+Version: 0.13
 Summary: Custom Python library for standard SQL tasks
 Home-page: https://github.com/PrinceJavier/sql_pylib
 Author: Prince Javier
 Author-email: othepjavier@gmail.com
 License: MIT
 Keywords: sql python
 Classifier: Development Status :: 3 - Alpha
```

