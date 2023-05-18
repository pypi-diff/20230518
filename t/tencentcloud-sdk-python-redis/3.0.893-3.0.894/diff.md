# Comparing `tmp/tencentcloud-sdk-python-redis-3.0.893.tar.gz` & `tmp/tencentcloud-sdk-python-redis-3.0.894.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.893.tar", last modified: Wed May 17 03:37:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.894.tar", last modified: Thu May 18 00:33:59 2023, max compression
```

## Comparing `tencentcloud-sdk-python-redis-3.0.893.tar` & `tencentcloud-sdk-python-redis-3.0.894.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:37:53.000000 tencentcloud-sdk-python-redis-3.0.893/
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-17 03:37:53.000000 tencentcloud-sdk-python-redis-3.0.893/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:37:53.000000 tencentcloud-sdk-python-redis-3.0.893/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:37:53.000000 tencentcloud-sdk-python-redis-3.0.893/tencentcloud/redis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:37:53.000000 tencentcloud-sdk-python-redis-3.0.893/tencentcloud/redis/v20180412/
--rw-r--r--   0 root         (0) root         (0)    87124 2023-05-17 03:37:53.000000 tencentcloud-sdk-python-redis-3.0.893/tencentcloud/redis/v20180412/redis_client.py
--rw-r--r--   0 root         (0) root         (0)    12423 2023-05-17 03:37:53.000000 tencentcloud-sdk-python-redis-3.0.893/tencentcloud/redis/v20180412/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:37:53.000000 tencentcloud-sdk-python-redis-3.0.893/tencentcloud/redis/v20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)   297155 2023-05-17 03:37:53.000000 tencentcloud-sdk-python-redis-3.0.893/tencentcloud/redis/v20180412/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:37:53.000000 tencentcloud-sdk-python-redis-3.0.893/tencentcloud/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:37:53.000000 tencentcloud-sdk-python-redis-3.0.893/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-17 03:37:53.000000 tencentcloud-sdk-python-redis-3.0.893/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-05-17 03:37:53.000000 tencentcloud-sdk-python-redis-3.0.893/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:37:53.000000 tencentcloud-sdk-python-redis-3.0.893/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:37:53.000000 tencentcloud-sdk-python-redis-3.0.893/tencentcloud_sdk_python_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:37:53.000000 tencentcloud-sdk-python-redis-3.0.893/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-05-17 03:37:53.000000 tencentcloud-sdk-python-redis-3.0.893/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-17 03:37:53.000000 tencentcloud-sdk-python-redis-3.0.893/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:37:53.000000 tencentcloud-sdk-python-redis-3.0.893/tencentcloud_sdk_python_redis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:33:59.000000 tencentcloud-sdk-python-redis-3.0.894/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-18 00:33:59.000000 tencentcloud-sdk-python-redis-3.0.894/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:33:59.000000 tencentcloud-sdk-python-redis-3.0.894/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:33:59.000000 tencentcloud-sdk-python-redis-3.0.894/tencentcloud/redis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:33:59.000000 tencentcloud-sdk-python-redis-3.0.894/tencentcloud/redis/v20180412/
+-rw-r--r--   0 root         (0) root         (0)    87184 2023-05-18 00:33:59.000000 tencentcloud-sdk-python-redis-3.0.894/tencentcloud/redis/v20180412/redis_client.py
+-rw-r--r--   0 root         (0) root         (0)    12423 2023-05-18 00:33:59.000000 tencentcloud-sdk-python-redis-3.0.894/tencentcloud/redis/v20180412/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:33:59.000000 tencentcloud-sdk-python-redis-3.0.894/tencentcloud/redis/v20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   297481 2023-05-18 00:33:59.000000 tencentcloud-sdk-python-redis-3.0.894/tencentcloud/redis/v20180412/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:33:59.000000 tencentcloud-sdk-python-redis-3.0.894/tencentcloud/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:33:59.000000 tencentcloud-sdk-python-redis-3.0.894/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-18 00:33:59.000000 tencentcloud-sdk-python-redis-3.0.894/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-18 00:33:59.000000 tencentcloud-sdk-python-redis-3.0.894/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:33:59.000000 tencentcloud-sdk-python-redis-3.0.894/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:33:59.000000 tencentcloud-sdk-python-redis-3.0.894/tencentcloud_sdk_python_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:33:59.000000 tencentcloud-sdk-python-redis-3.0.894/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-18 00:33:59.000000 tencentcloud-sdk-python-redis-3.0.894/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-18 00:33:59.000000 tencentcloud-sdk-python-redis-3.0.894/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:33:59.000000 tencentcloud-sdk-python-redis-3.0.894/tencentcloud_sdk_python_redis.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-redis-3.0.893/README.rst` & `tencentcloud-sdk-python-redis-3.0.894/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.893/tencentcloud/redis/v20180412/redis_client.py` & `tencentcloud-sdk-python-redis-3.0.894/tencentcloud/redis/v20180412/redis_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,15 +437,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeAutoBackupConfig(self, request):
-        """获取备份配置
+        """本接口（DescribeAutoBackupConfig）用于获取自动备份配置规则。
 
         :param request: Request instance for DescribeAutoBackupConfig.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeAutoBackupConfigRequest`
         :rtype: :class:`tencentcloud.redis.v20180412.models.DescribeAutoBackupConfigResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-redis-3.0.893/tencentcloud/redis/v20180412/errorcodes.py` & `tencentcloud-sdk-python-redis-3.0.894/tencentcloud/redis/v20180412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.893/tencentcloud/redis/v20180412/models.py` & `tencentcloud-sdk-python-redis-3.0.894/tencentcloud/redis/v20180412/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1429,15 +1429,15 @@
 class DescribeAutoBackupConfigRequest(AbstractModel):
     """DescribeAutoBackupConfig请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例ID
+        :param InstanceId: 指定实例 ID。例如：crs-xjhsdj****。请登录[Redis控制台](https://console.cloud.tencent.com/redis)在实例列表复制实例 ID。
         :type InstanceId: str
         """
         self.InstanceId = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
@@ -1453,23 +1453,23 @@
 class DescribeAutoBackupConfigResponse(AbstractModel):
     """DescribeAutoBackupConfig返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param AutoBackupType: 备份类型。自动备份类型： 1 “定时回档”
+        :param AutoBackupType: 该参数因兼容性问题暂时保留，请忽略。
         :type AutoBackupType: int
-        :param WeekDays: Monday，Tuesday，Wednesday，Thursday，Friday，Saturday，Sunday。
+        :param WeekDays: 备份周期，默认为每天自动备份，Monday，Tuesday，Wednesday，Thursday，Friday，Saturday，Sunday。
         :type WeekDays: list of str
-        :param TimePeriod: 时间段。
+        :param TimePeriod: 备份任务发起时间段。
         :type TimePeriod: str
-        :param BackupStorageDays: 全量备份文件保存天数
+        :param BackupStorageDays: 全量备份文件保存天数。默认为7天。如需保存更多天数，请[提交工单](https://console.cloud.tencent.com/workorder/category)申请。
         :type BackupStorageDays: int
-        :param BinlogStorageDays: tendis binlog备份文件保存天数
+        :param BinlogStorageDays: 该参数不再使用，请忽略。
         :type BinlogStorageDays: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.AutoBackupType = None
         self.WeekDays = None
         self.TimePeriod = None
@@ -6916,15 +6916,15 @@
     def __init__(self):
         r"""
         :param StartTime: 备份开始时间。
         :type StartTime: str
         :param BackupId: 备份任务ID。
         :type BackupId: str
         :param BackupType: 备份类型。
-- 1：凌晨系统发起的备份。
+- 1：凌晨系统发起的自动备份。
 - 0：用户发起的手动备份。
         :type BackupType: str
         :param Status: 备份状态。 
 - 1：备份被其它流程锁定。
 - 2：备份正常，没有被任何流程锁定。
 - -1：备份已过期。
 - 3：备份正在被导出。
```

### Comparing `tencentcloud-sdk-python-redis-3.0.893/tencentcloud/__init__.py` & `tencentcloud-sdk-python-redis-3.0.894/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.893'
+__version__ = '3.0.894'
```

### Comparing `tencentcloud-sdk-python-redis-3.0.893/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.894/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.893/setup.py` & `tencentcloud-sdk-python-redis-3.0.894/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.893/tencentcloud_sdk_python_redis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.894/tencentcloud_sdk_python_redis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

