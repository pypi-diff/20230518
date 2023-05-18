# Comparing `tmp/iosense_connect-2.1.6.tar.gz` & `tmp/iosense_connect-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect-2.1.6.tar", last modified: Wed May 17 08:00:45 2023, max compression
+gzip compressed data, was "dist\iosense_connect-2.1.7.tar", last modified: Thu May 18 09:17:55 2023, max compression
```

## Comparing `iosense_connect-2.1.6.tar` & `iosense_connect-2.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 08:00:45.155023 iosense_connect-2.1.6/
--rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-2.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0     1062 2023-05-17 08:00:45.155023 iosense_connect-2.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-2.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 08:00:45.123750 iosense_connect-2.1.6/iosense_connect/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.1.6/iosense_connect/__init__.py
--rw-rw-rw-   0        0        0    23492 2023-05-17 06:02:27.000000 iosense_connect-2.1.6/iosense_connect/data_access.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:00:45.155023 iosense_connect-2.1.6/iosense_connect.egg-info/
--rw-rw-rw-   0        0        0     1062 2023-05-17 08:00:44.000000 iosense_connect-2.1.6/iosense_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-05-17 08:00:44.000000 iosense_connect-2.1.6/iosense_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 08:00:44.000000 iosense_connect-2.1.6/iosense_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-17 08:00:44.000000 iosense_connect-2.1.6/iosense_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 08:00:45.155023 iosense_connect-2.1.6/setup.cfg
--rw-rw-rw-   0        0        0      614 2023-05-17 08:00:37.000000 iosense_connect-2.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 09:17:55.916821 iosense_connect-2.1.7/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-2.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     1062 2023-05-18 09:17:55.913871 iosense_connect-2.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-2.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 09:17:55.878542 iosense_connect-2.1.7/iosense_connect/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.1.7/iosense_connect/__init__.py
+-rw-rw-rw-   0        0        0    23617 2023-05-18 09:17:04.000000 iosense_connect-2.1.7/iosense_connect/data_access.py
+drwxrwxrwx   0        0        0        0 2023-05-18 09:17:55.909823 iosense_connect-2.1.7/iosense_connect.egg-info/
+-rw-rw-rw-   0        0        0     1062 2023-05-18 09:17:55.000000 iosense_connect-2.1.7/iosense_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-05-18 09:17:55.000000 iosense_connect-2.1.7/iosense_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 09:17:55.000000 iosense_connect-2.1.7/iosense_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-18 09:17:55.000000 iosense_connect-2.1.7/iosense_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 09:17:55.917825 iosense_connect-2.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      614 2023-05-18 09:17:53.000000 iosense_connect-2.1.7/setup.py
```

### Comparing `iosense_connect-2.1.6/LICENSE.txt` & `iosense_connect-2.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iosense_connect-2.1.6/PKG-INFO` & `iosense_connect-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense_connect
-Version: 2.1.6
+Version: 2.1.7
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-2.1.6/README.md` & `iosense_connect-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `iosense_connect-2.1.6/iosense_connect/data_access.py` & `iosense_connect-2.1.7/iosense_connect/data_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -468,36 +468,37 @@
                         end_time = datetime.strptime(end_time, '%Y-%m-%d %H:%M:%S')
                         df = df[(df['time'] >= start_time) & (df['time'] <= end_time)]
                     except ValueError:
                         df = df[(df['time'] >= start_time) & (df['time'] <= end_time)]
                         pass
                     except Exception as e:
                         print('Message: \t',e)
-                    if sensors is None:
-                        sensors = list(df.columns)
-                        sensors.remove('time')
-                    sensor_list_df = list(df.columns)
-                    sensor_list_df.remove('time')
-                    sensors_filtered = list(set(sensor_list_df).intersection(sensors))
-                    if sensors != None and len(sensors_filtered) != 0:
-                        sensors_filtered.insert(0,'time')
-                        df =  df[sensors_filtered]
-                    if len(sensors_filtered) == 0:
-                        df = pd.DataFrame()
-                    df.reset_index(drop=True, inplace=True)
-                    last_date = df['time'].iloc[len(df) - 1]
-                    start_date = last_date.date() + timedelta(days=1)
-                    end_time = pd.to_datetime(end_time)
-                    if last_date.date() != end_time.date():
-                        df1 = DataAccess.fetch_data(self, device_id ,start_time=str(start_date), alias=False,end_time=end_time,sensors=sensors, echo=True,onpremise=False,IST=True)
-                        df = pd.concat([df, df1])
-                    else:
-                        df1 = DataAccess.fetch_data(self, device_id,start_time=str(last_date), alias=False,end_time=end_time,sensors=sensors, echo=True,onpremise=False,IST=True)
-                        df = pd.concat([df, df1])
-                    df.reset_index(drop=True, inplace=True)
+                    if len(df) !=0:
+                        if sensors is None:
+                            sensors = list(df.columns)
+                            sensors.remove('time')
+                        sensor_list_df = list(df.columns)
+                        sensor_list_df.remove('time')
+                        sensors_filtered = list(set(sensor_list_df).intersection(sensors))
+                        if sensors != None and len(sensors_filtered) != 0:
+                            sensors_filtered.insert(0,'time')
+                            df =  df[sensors_filtered]
+                        if len(sensors_filtered) == 0:
+                            df = pd.DataFrame()
+                        df.reset_index(drop=True, inplace=True)
+                        last_date = df['time'].iloc[len(df) - 1]
+                        start_date = last_date.date() + timedelta(days=1)
+                        end_time = pd.to_datetime(end_time)
+                        if last_date.date() != end_time.date():
+                            df1 = DataAccess.fetch_data(self, device_id ,start_time=str(start_date), alias=False,end_time=end_time,sensors=sensors, echo=True,onpremise=False,IST=True)
+                            df = pd.concat([df, df1])
+                        else:
+                            df1 = DataAccess.fetch_data(self, device_id,start_time=str(last_date), alias=False,end_time=end_time,sensors=sensors, echo=True,onpremise=False,IST=True)
+                            df = pd.concat([df, df1])
+                        df.reset_index(drop=True, inplace=True)
             else:
                 df_devices = DataAccess.get_device_details(self,onpremise=onpremise)
                 device_list = df_devices['devID'].tolist()
                 if device_id in device_list:
                     df = DataAccess.fetch_data(self, device_id, start_time,end_time, alias,sensors=sensors,echo=True,onpremise=onpremise,IST=IST)
                 else:
                     raise Exception('Message: Device not added in account')
```

### Comparing `iosense_connect-2.1.6/iosense_connect.egg-info/PKG-INFO` & `iosense_connect-2.1.7/iosense_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense-connect
-Version: 2.1.6
+Version: 2.1.7
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-2.1.6/setup.py` & `iosense_connect-2.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "iosense_connect",
-    version = "2.1.6",
+    version = "2.1.7",
     author = "Faclon-Labs",
     author_email = "reachus@faclon.com",
     description = "iosense connect library",
     packages = ["iosense_connect"],
     long_description = long_description,
     long_description_content_type = "text/markdown",
     classifiers = [
```

