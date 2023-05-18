# Comparing `tmp/DeepRetail-0.0.6.tar.gz` & `tmp/DeepRetail-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\u0138780\yForecasting_Github\DeepRetail\dist\.tmp-16h3am6s\DeepRetail-0.0.6.tar", last modified: Mon May  8 09:04:07 2023, max compression
+gzip compressed data, was "C:\Users\u0138780\yForecasting_Github\DeepRetail\dist\.tmp-xmzzge2k\DeepRetail-0.0.7.tar", last modified: Thu May 18 06:07:51 2023, max compression
```

## Comparing `DeepRetail-0.0.6.tar` & `DeepRetail-0.0.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 09:04:07.040992 DeepRetail-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-05-08 09:04:06.979977 DeepRetail-0.0.6/DeepRetail/
--rw-rw-rw-   0        0        0        0 2023-02-15 11:39:40.000000 DeepRetail-0.0.6/DeepRetail/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:04:07.002993 DeepRetail-0.0.6/DeepRetail/data/
--rw-rw-rw-   0        0        0       18 2023-02-20 14:22:28.000000 DeepRetail-0.0.6/DeepRetail/data/__init__.py
--rw-rw-rw-   0        0        0    17039 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/data/casereaders.py
--rw-rw-rw-   0        0        0     9392 2023-03-23 09:36:05.000000 DeepRetail-0.0.6/DeepRetail/data/dataloader.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:04:07.008993 DeepRetail-0.0.6/DeepRetail/evaluation/
--rw-rw-rw-   0        0        0       41 2023-02-20 14:22:28.000000 DeepRetail-0.0.6/DeepRetail/evaluation/__init__.py
--rw-rw-rw-   0        0        0    12675 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/evaluation/base.py
--rw-rw-rw-   0        0        0     9213 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/evaluation/metrics.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:04:07.014993 DeepRetail-0.0.6/DeepRetail/exploratory/
--rw-rw-rw-   0        0        0        0 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/exploratory/__init__.py
--rw-rw-rw-   0        0        0     2238 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/exploratory/eda.py
--rw-rw-rw-   0        0        0     9337 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/exploratory/visuals.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:04:07.021993 DeepRetail-0.0.6/DeepRetail/forecasting/
--rw-rw-rw-   0        0        0       18 2023-02-20 14:22:28.000000 DeepRetail-0.0.6/DeepRetail/forecasting/__init__.py
--rw-rw-rw-   0        0        0    21566 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/forecasting/ml.py
--rw-rw-rw-   0        0        0    23005 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/forecasting/statistical.py
--rw-rw-rw-   0        0        0     8229 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/forecasting/utils.py
--rw-rw-rw-   0        0        0       49 2023-02-15 11:39:40.000000 DeepRetail-0.0.6/DeepRetail/hierarchical.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:04:07.032994 DeepRetail-0.0.6/DeepRetail/reconciliation/
--rw-rw-rw-   0        0        0        0 2023-03-02 14:21:40.000000 DeepRetail-0.0.6/DeepRetail/reconciliation/__init__.py
--rw-rw-rw-   0        0        0    24670 2023-03-23 09:36:05.000000 DeepRetail-0.0.6/DeepRetail/reconciliation/cross_sectional.py
--rw-rw-rw-   0        0        0    35145 2023-03-23 09:36:05.000000 DeepRetail-0.0.6/DeepRetail/reconciliation/cross_temporal.py
--rw-rw-rw-   0        0        0    32997 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/reconciliation/temporal.py
--rw-rw-rw-   0        0        0    18106 2023-03-23 09:36:05.000000 DeepRetail-0.0.6/DeepRetail/reconciliation/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:04:07.037993 DeepRetail-0.0.6/DeepRetail/transformations/
--rw-rw-rw-   0        0        0       18 2023-02-20 14:22:28.000000 DeepRetail-0.0.6/DeepRetail/transformations/__init__.py
--rw-rw-rw-   0        0        0     9740 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/transformations/decomposition.py
--rw-rw-rw-   0        0        0    14647 2023-05-08 09:01:42.000000 DeepRetail-0.0.6/DeepRetail/transformations/formats.py
--rw-rw-rw-   0        0        0       61 2023-05-08 09:02:57.000000 DeepRetail-0.0.6/DeepRetail/version.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:04:06.997992 DeepRetail-0.0.6/DeepRetail.egg-info/
--rw-rw-rw-   0        0        0     3799 2023-05-08 09:04:06.000000 DeepRetail-0.0.6/DeepRetail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1007 2023-05-08 09:04:06.000000 DeepRetail-0.0.6/DeepRetail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 09:04:06.000000 DeepRetail-0.0.6/DeepRetail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-05-08 09:04:06.000000 DeepRetail-0.0.6/DeepRetail.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-08 09:04:06.000000 DeepRetail-0.0.6/DeepRetail.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2022-06-19 22:52:26.000000 DeepRetail-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     3799 2023-05-08 09:04:07.039993 DeepRetail-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3002 2023-05-08 09:02:57.000000 DeepRetail-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-08 09:04:07.040992 DeepRetail-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1501 2023-05-08 09:02:57.000000 DeepRetail-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 06:07:51.402907 DeepRetail-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-05-18 06:07:50.944069 DeepRetail-0.0.7/DeepRetail/
+-rw-rw-rw-   0        0        0        0 2023-02-15 11:39:40.000000 DeepRetail-0.0.7/DeepRetail/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 06:07:51.021119 DeepRetail-0.0.7/DeepRetail/data/
+-rw-rw-rw-   0        0        0       18 2023-02-20 14:22:28.000000 DeepRetail-0.0.7/DeepRetail/data/__init__.py
+-rw-rw-rw-   0        0        0    19409 2023-05-18 05:45:21.000000 DeepRetail-0.0.7/DeepRetail/data/casereaders.py
+-rw-rw-rw-   0        0        0     9621 2023-05-18 05:45:21.000000 DeepRetail-0.0.7/DeepRetail/data/dataloader.py
+drwxrwxrwx   0        0        0        0 2023-05-18 06:07:51.091776 DeepRetail-0.0.7/DeepRetail/evaluation/
+-rw-rw-rw-   0        0        0       41 2023-02-20 14:22:28.000000 DeepRetail-0.0.7/DeepRetail/evaluation/__init__.py
+-rw-rw-rw-   0        0        0    12675 2023-05-08 09:01:42.000000 DeepRetail-0.0.7/DeepRetail/evaluation/base.py
+-rw-rw-rw-   0        0        0     9213 2023-05-08 09:01:42.000000 DeepRetail-0.0.7/DeepRetail/evaluation/metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-18 06:07:51.155487 DeepRetail-0.0.7/DeepRetail/exploratory/
+-rw-rw-rw-   0        0        0        0 2023-05-08 09:01:42.000000 DeepRetail-0.0.7/DeepRetail/exploratory/__init__.py
+-rw-rw-rw-   0        0        0     4947 2023-05-18 05:45:21.000000 DeepRetail-0.0.7/DeepRetail/exploratory/eda.py
+-rw-rw-rw-   0        0        0     9337 2023-05-08 09:01:42.000000 DeepRetail-0.0.7/DeepRetail/exploratory/visuals.py
+drwxrwxrwx   0        0        0        0 2023-05-18 06:07:51.261950 DeepRetail-0.0.7/DeepRetail/forecasting/
+-rw-rw-rw-   0        0        0       18 2023-02-20 14:22:28.000000 DeepRetail-0.0.7/DeepRetail/forecasting/__init__.py
+-rw-rw-rw-   0        0        0    21566 2023-05-08 09:01:42.000000 DeepRetail-0.0.7/DeepRetail/forecasting/ml.py
+-rw-rw-rw-   0        0        0    23005 2023-05-08 09:01:42.000000 DeepRetail-0.0.7/DeepRetail/forecasting/statistical.py
+-rw-rw-rw-   0        0        0     8229 2023-05-08 09:01:42.000000 DeepRetail-0.0.7/DeepRetail/forecasting/utils.py
+-rw-rw-rw-   0        0        0       49 2023-02-15 11:39:40.000000 DeepRetail-0.0.7/DeepRetail/hierarchical.py
+drwxrwxrwx   0        0        0        0 2023-05-18 06:07:51.347928 DeepRetail-0.0.7/DeepRetail/reconciliation/
+-rw-rw-rw-   0        0        0        0 2023-03-02 14:21:40.000000 DeepRetail-0.0.7/DeepRetail/reconciliation/__init__.py
+-rw-rw-rw-   0        0        0    24670 2023-03-23 09:36:05.000000 DeepRetail-0.0.7/DeepRetail/reconciliation/cross_sectional.py
+-rw-rw-rw-   0        0        0    35145 2023-03-23 09:36:05.000000 DeepRetail-0.0.7/DeepRetail/reconciliation/cross_temporal.py
+-rw-rw-rw-   0        0        0    32997 2023-05-08 09:01:42.000000 DeepRetail-0.0.7/DeepRetail/reconciliation/temporal.py
+-rw-rw-rw-   0        0        0    18106 2023-03-23 09:36:05.000000 DeepRetail-0.0.7/DeepRetail/reconciliation/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-18 06:07:51.396907 DeepRetail-0.0.7/DeepRetail/transformations/
+-rw-rw-rw-   0        0        0       18 2023-02-20 14:22:28.000000 DeepRetail-0.0.7/DeepRetail/transformations/__init__.py
+-rw-rw-rw-   0        0        0     9740 2023-05-08 09:01:42.000000 DeepRetail-0.0.7/DeepRetail/transformations/decomposition.py
+-rw-rw-rw-   0        0        0    14647 2023-05-08 09:01:42.000000 DeepRetail-0.0.7/DeepRetail/transformations/formats.py
+-rw-rw-rw-   0        0        0       61 2023-05-18 05:46:23.000000 DeepRetail-0.0.7/DeepRetail/version.py
+drwxrwxrwx   0        0        0        0 2023-05-18 06:07:50.982096 DeepRetail-0.0.7/DeepRetail.egg-info/
+-rw-rw-rw-   0        0        0     3799 2023-05-18 06:07:50.000000 DeepRetail-0.0.7/DeepRetail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1007 2023-05-18 06:07:50.000000 DeepRetail-0.0.7/DeepRetail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 06:07:50.000000 DeepRetail-0.0.7/DeepRetail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-05-18 06:07:50.000000 DeepRetail-0.0.7/DeepRetail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-18 06:07:50.000000 DeepRetail-0.0.7/DeepRetail.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2022-06-19 22:52:26.000000 DeepRetail-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3799 2023-05-18 06:07:51.400907 DeepRetail-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3002 2023-05-18 05:46:24.000000 DeepRetail-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-18 06:07:51.402907 DeepRetail-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1501 2023-05-18 05:46:24.000000 DeepRetail-0.0.7/setup.py
```

### Comparing `DeepRetail-0.0.6/DeepRetail/data/casereaders.py` & `DeepRetail-0.0.7/DeepRetail/data/casereaders.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,19 +51,22 @@
 
     # drop columns with only zeros
     df = df.loc[~(df == 0).all(axis=1)]
 
     return df
 
 
-def read_case_1(read_filepath, write_filepath, frequency, temporary_save):
+def read_case_1(
+    read_filepath, products_filepath, write_filepath, frequency, temporary_save
+):
     """Reads data for case 1
 
     Args:
         read_filepath (str): Existing loocation of the data file
+        products_filepath (str): Existing location of the products file
         write_filepath (str): Location to save the new file
         frequency (str): The selected frequency.
                     Note: Due to size issues, for case 1 only supports W and M
         temporary_save (bool, Optional): If true it saves the dataframe on chunks
                                          Deals with memory breaks.
     """
     # Initialize parameters to ensure stable loading
@@ -165,16 +168,59 @@
 
         # Add to the main df
         out_df = pd.concat([out_df, temp_df], axis=1)
 
         # Save at each itteration to deal with memory breaks
         if temporary_save:
             out_df.to_csv(write_filepath)
-    # Final save
-    # out_df = fix_duplicate_cols(out_df)
+
+    # Split the index in - and keep only the last part
+    out_df.index = out_df.index.str.split("-").str[-1]
+
+    # fill nans with 0
+    out_df = out_df.fillna(0)
+
+    # Sum all columns for rows with the same index
+    out_df = out_df.groupby(out_df.index).sum()
+
+    # Convert the type of index to int
+    out_df.index = out_df.index.astype(int)
+
+    # Add the product family hierarchical structure
+    # Read the products file
+    metadata = pd.ExcelFile(products_filepath)
+
+    # Prepare the product family
+    out_df = out_df.reset_index()
+    df_products = prepare_product_data(metadata, out_df)
+
+    # Add a unique numeric code for each product family
+    df_products["product_family_code"] = (
+        df_products["ProductFamily"].astype("category").cat.codes
+    )
+
+    # Add the hierarchical information here
+    # add the product_family_code to the df
+    out_df = pd.merge(
+        out_df, df_products[["product_family_code", "unique_id"]], on="unique_id"
+    )
+
+    # Add the new unique_id
+    out_df["unique_id"] = (
+        out_df["product_family_code"].astype(str)
+        + "_"
+        + out_df["unique_id"].astype(str)
+    )
+
+    # drop the product_family_code and the Item columns
+    out_df = out_df.drop(["product_family_code"], axis=1)
+
+    # Set the unique_id as index
+    out_df = out_df.set_index("unique_id")
+
     return out_df
 
 
 def read_case_2(read_filepath):
     """Reads data for case 2
 
     Args:
@@ -239,15 +285,15 @@
     """Reads data for case 4
 
     Args:
         read_filepath (str): Existing loocation of the data file
     """
 
     # Loading
-    df = pd.read_csv(read_filepath)
+    df = pd.read_csv(read_filepath, sep=",", engine="python", error_bad_lines=False)
 
     # Removing instances with bad status
     ids = df[(df["Status"] == 4) | (df["Status"].isna()) | (df["Exclincl"] != 1)].index
     df = df.drop(ids)
 
     # Convert date to datetime
     df["Datum"] = pd.to_datetime(df["Datum"])
@@ -385,14 +431,44 @@
     """
     if (q > 0) & (p == 0):
         return 1
     else:
         return 0
 
 
+def prepare_product_data(metadata, df):
+    """
+    Returns the product family csv from the metadata xlsx.
+
+    Args:
+        metadata (pd.ExcelFile): The excel file with the metadata.
+        df (pd.DataFrame): The dataframe with the time series information.
+
+    Returns:
+        pd.DataFrame: The product family dataframe.
+    """
+
+    # Split the metadata
+    s2 = pd.read_excel(metadata, "Export")
+
+    # Filter and rename columns
+    product_family = s2[["ACG - ACG", "ALDI nr"]]
+    product_family = product_family.rename(
+        columns={"ALDI nr": "unique_id", "ACG - ACG": "ProductFamily"}
+    ).drop_duplicates()
+
+    # Keep only relevant items
+    product_family["unique_id"] = product_family["unique_id"].astype(int)
+    product_family = product_family[
+        product_family["unique_id"].isin(df["unique_id"].unique())
+    ]
+
+    return product_family
+
+
 def read_case_5(read_filepath):
     """Reads data for case 5
 
     Args:
         read_filepath (str): Existing loocation of the data file
     """
     # read
@@ -530,23 +606,23 @@
     df = pd.merge(df, item_per_prod, on="PRODUCT_CODE", how="left")
     # Multiply to get the cigars => the actual sales!
     df["Sales"] = df["QTY_INVOICED"] * df["Cigars_Num"]
     # Drop used columns
     df = df.drop(["Cigars_Num", "QTY_INVOICED"], axis=1)
 
     # filter some nan values
-    df = df[~df['FAM'].isna()]
+    df = df[~df["FAM"].isna()]
     df = df.dropna()
 
     # groupby on product level
     df["product_id"] = [id.split("-")[0] for id in df["PRODUCT_CODE"]]
 
     # Add the family:
     df["product_id"] = [
-        str(fam) + '_' + str(id) for fam, id in zip(df["FAM"], df["product_id"])
+        str(fam) + "_" + str(id) for fam, id in zip(df["FAM"], df["product_id"])
     ]
 
     df = df.groupby(["product_id", "ORDER_DATE"]).agg({"Sales": "sum"}).reset_index()
 
     # keep columns
     cols = ["unique_id", "date", "y"]
     df.columns = cols
```

### Comparing `DeepRetail-0.0.6/DeepRetail/data/dataloader.py` & `DeepRetail-0.0.7/DeepRetail/data/dataloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,32 +15,35 @@
 class Reader(object):
     """
     Reads data of different formats from the provided filepath.
     Converts data into a universal format used through the package.
 
     """
 
-    def __init__(self, filepath, calendar_filepath=None, case=0, temporary_save=False):
+    def __init__(self, filepath, product_filepath=None, calendar_filepath=None, case=0, temporary_save=False):
         """
         Initializes a Reader object.
 
         Args:
             filepath (str): Path to the file to be read.
+            product_filepath (str, optional): Path to the product dataframe.
+                Required for case 1. Default to None.
             calendar_filepath (str, optional): Path to the calendar dataframe.
-                Required for case 3. Defaults to None.
+                Required for case 0. Defaults to None.
             case (int): Specifies the format of the data to be read.
                 Defaults to 0.
 
         Raises:
             AssertionError: If case is not an integer.
         """
 
         assert type(case) == int, "case should be an integer"
         self.case = case
         self.filepath = filepath
+        self.product_filepath = product_filepath
         self.calendar_filepath = calendar_filepath
         self.temporary_save = temporary_save
 
     def call_in_memory(
         self,
         filter_negatives=True,
         filter_negatives_strategy="constant",
@@ -75,15 +78,15 @@
                 raise ValueError("Case 3 requires the calendar dataframe")
             # read
             temp_df = read_case_0(self.filepath, self.calendar_filepath)
 
         if self.case == 1:
             # For case 1 -> we first read the data in the folder
             temp_df = read_case_1(
-                self.filepath, self.save_filepath, self.frequency, self.temporary_save
+                self.filepath, self.product_filepath, self.save_filepath, self.frequency, self.temporary_save
             )
             # converts columns to str to fix a bug
             temp_df.columns = pd.to_datetime(temp_df.columns).astype(str)
 
             # Fix duplicates
             temp_df = fix_duplicate_cols(temp_df)
```

### Comparing `DeepRetail-0.0.6/DeepRetail/evaluation/base.py` & `DeepRetail-0.0.7/DeepRetail/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.6/DeepRetail/evaluation/metrics.py` & `DeepRetail-0.0.7/DeepRetail/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.6/DeepRetail/exploratory/visuals.py` & `DeepRetail-0.0.7/DeepRetail/exploratory/visuals.py`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.6/DeepRetail/forecasting/ml.py` & `DeepRetail-0.0.7/DeepRetail/forecasting/ml.py`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.6/DeepRetail/forecasting/statistical.py` & `DeepRetail-0.0.7/DeepRetail/forecasting/statistical.py`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.6/DeepRetail/forecasting/utils.py` & `DeepRetail-0.0.7/DeepRetail/forecasting/utils.py`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.6/DeepRetail/reconciliation/cross_sectional.py` & `DeepRetail-0.0.7/DeepRetail/reconciliation/cross_sectional.py`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.6/DeepRetail/reconciliation/cross_temporal.py` & `DeepRetail-0.0.7/DeepRetail/reconciliation/cross_temporal.py`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.6/DeepRetail/reconciliation/temporal.py` & `DeepRetail-0.0.7/DeepRetail/reconciliation/temporal.py`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.6/DeepRetail/reconciliation/utils.py` & `DeepRetail-0.0.7/DeepRetail/reconciliation/utils.py`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.6/DeepRetail/transformations/decomposition.py` & `DeepRetail-0.0.7/DeepRetail/transformations/decomposition.py`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.6/DeepRetail/transformations/formats.py` & `DeepRetail-0.0.7/DeepRetail/transformations/formats.py`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.6/DeepRetail.egg-info/PKG-INFO` & `DeepRetail-0.0.7/DeepRetail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepRetail
-Version: 0.0.6
+Version: 0.0.7
 Summary: Forecasting package for retail using Deep Learning AI.
 Home-page: https://github.com/yForecasting/DeepRetail
 Author: Yves R. Sagaert
 Author-email: yves.r.sagaert@gmail.com
 License: GNU GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,15 +15,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DeepRetail
-<img src="https://img.shields.io/badge/Maintained%20by-Vives%20AI%20Lab-red"> [![Downloads](https://static.pepy.tech/personalized-badge/DeepRetail?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/DeepRetail) <img src="https://img.shields.io/badge/python-v3.7%2B-blue"> <img src="https://img.shields.io/badge/pypi-v0.0.6-blue">
+<img src="https://img.shields.io/badge/Maintained%20by-Vives%20AI%20Lab-red"> [![Downloads](https://static.pepy.tech/personalized-badge/DeepRetail?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/DeepRetail) <img src="https://img.shields.io/badge/python-v3.7%2B-blue"> <img src="https://img.shields.io/badge/pypi-v0.0.7-blue">
 
 Python package on deep learning AI and machine learning for Retail
 
 This package is developed by the AI team at [VIVES University of Applied Sciences](https://www.vives.be/en/research/centre-expertise-business-management) and is used in our research on [demand forecasting](https://yvesrsagaert.wordpress.com/).
 
 ___
```

### Comparing `DeepRetail-0.0.6/DeepRetail.egg-info/SOURCES.txt` & `DeepRetail-0.0.7/DeepRetail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.6/LICENSE` & `DeepRetail-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepRetail-0.0.6/PKG-INFO` & `DeepRetail-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepRetail
-Version: 0.0.6
+Version: 0.0.7
 Summary: Forecasting package for retail using Deep Learning AI.
 Home-page: https://github.com/yForecasting/DeepRetail
 Author: Yves R. Sagaert
 Author-email: yves.r.sagaert@gmail.com
 License: GNU GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,15 +15,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DeepRetail
-<img src="https://img.shields.io/badge/Maintained%20by-Vives%20AI%20Lab-red"> [![Downloads](https://static.pepy.tech/personalized-badge/DeepRetail?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/DeepRetail) <img src="https://img.shields.io/badge/python-v3.7%2B-blue"> <img src="https://img.shields.io/badge/pypi-v0.0.6-blue">
+<img src="https://img.shields.io/badge/Maintained%20by-Vives%20AI%20Lab-red"> [![Downloads](https://static.pepy.tech/personalized-badge/DeepRetail?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/DeepRetail) <img src="https://img.shields.io/badge/python-v3.7%2B-blue"> <img src="https://img.shields.io/badge/pypi-v0.0.7-blue">
 
 Python package on deep learning AI and machine learning for Retail
 
 This package is developed by the AI team at [VIVES University of Applied Sciences](https://www.vives.be/en/research/centre-expertise-business-management) and is used in our research on [demand forecasting](https://yvesrsagaert.wordpress.com/).
 
 ___
```

### Comparing `DeepRetail-0.0.6/README.md` & `DeepRetail-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DeepRetail
-<img src="https://img.shields.io/badge/Maintained%20by-Vives%20AI%20Lab-red"> [![Downloads](https://static.pepy.tech/personalized-badge/DeepRetail?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/DeepRetail) <img src="https://img.shields.io/badge/python-v3.7%2B-blue"> <img src="https://img.shields.io/badge/pypi-v0.0.6-blue">
+<img src="https://img.shields.io/badge/Maintained%20by-Vives%20AI%20Lab-red"> [![Downloads](https://static.pepy.tech/personalized-badge/DeepRetail?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/DeepRetail) <img src="https://img.shields.io/badge/python-v3.7%2B-blue"> <img src="https://img.shields.io/badge/pypi-v0.0.7-blue">
 
 Python package on deep learning AI and machine learning for Retail
 
 This package is developed by the AI team at [VIVES University of Applied Sciences](https://www.vives.be/en/research/centre-expertise-business-management) and is used in our research on [demand forecasting](https://yvesrsagaert.wordpress.com/).
 
 ___
```

### Comparing `DeepRetail-0.0.6/setup.py` & `DeepRetail-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 setuptools.setup(
     author="Yves R. Sagaert",
     author_email="yves.r.sagaert@gmail.com",
     name='DeepRetail',
     license="GNU GPLv3",
     description='Forecasting package for retail using Deep Learning AI.',
-    version='v0.0.6',
+    version='v0.0.7',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/yForecasting/DeepRetail',
     packages=setuptools.find_packages(),
     include_package_data=True,
     python_requires=">=3.5",
     # Enable install requires when publishing on the normal PyPi
```

