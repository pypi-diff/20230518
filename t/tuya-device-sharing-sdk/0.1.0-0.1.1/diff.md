# Comparing `tmp/tuya_device_sharing_sdk-0.1.0-py2.py3-none-any.whl.zip` & `tmp/tuya_device_sharing_sdk-0.1.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 13739 bytes, number of entries: 16
+Zip file size: 13651 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      588 b- defN 23-May-04 05:58 tuya_sharing/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-13 05:56 tuya_sharing/const.py
 -rw-r--r--  2.0 unx     8807 b- defN 23-May-12 01:59 tuya_sharing/customerapi.py
 -rw-r--r--  2.0 unx      240 b- defN 23-Apr-13 05:56 tuya_sharing/customerlogging.py
 -rw-r--r--  2.0 unx     4359 b- defN 23-May-16 04:24 tuya_sharing/device.py
 -rw-r--r--  2.0 unx      673 b- defN 23-May-04 06:04 tuya_sharing/home.py
 -rw-r--r--  2.0 unx     7334 b- defN 23-May-10 05:48 tuya_sharing/manager.py
 -rw-r--r--  2.0 unx     5744 b- defN 23-May-12 03:32 tuya_sharing/mq.py
 -rw-r--r--  2.0 unx     1230 b- defN 23-May-09 02:24 tuya_sharing/scenes.py
--rw-r--r--  2.0 unx     2092 b- defN 23-May-09 01:07 tuya_sharing/user.py
--rw-r--r--  2.0 unx       62 b- defN 23-Apr-23 09:53 tuya_sharing/version.py
--rw-r--r--  2.0 unx     1079 b- defN 23-May-17 02:31 tuya_device_sharing_sdk-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1692 b- defN 23-May-17 02:31 tuya_device_sharing_sdk-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-17 02:31 tuya_device_sharing_sdk-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-May-17 02:31 tuya_device_sharing_sdk-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1337 b- defN 23-May-17 02:31 tuya_device_sharing_sdk-0.1.0.dist-info/RECORD
-16 files, 35360 bytes uncompressed, 11521 bytes compressed:  67.4%
+-rw-r--r--  2.0 unx     1690 b- defN 23-May-18 03:12 tuya_sharing/user.py
+-rw-r--r--  2.0 unx       62 b- defN 23-May-18 03:32 tuya_sharing/version.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-May-18 03:32 tuya_device_sharing_sdk-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1692 b- defN 23-May-18 03:32 tuya_device_sharing_sdk-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-18 03:32 tuya_device_sharing_sdk-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-May-18 03:32 tuya_device_sharing_sdk-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1337 b- defN 23-May-18 03:32 tuya_device_sharing_sdk-0.1.1.dist-info/RECORD
+16 files, 34958 bytes uncompressed, 11433 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: tuya_sharing/user.py
 Comment: 
 
 Filename: tuya_sharing/version.py
 Comment: 
 
-Filename: tuya_device_sharing_sdk-0.1.0.dist-info/LICENSE
+Filename: tuya_device_sharing_sdk-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: tuya_device_sharing_sdk-0.1.0.dist-info/METADATA
+Filename: tuya_device_sharing_sdk-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: tuya_device_sharing_sdk-0.1.0.dist-info/WHEEL
+Filename: tuya_device_sharing_sdk-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: tuya_device_sharing_sdk-0.1.0.dist-info/top_level.txt
+Filename: tuya_device_sharing_sdk-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: tuya_device_sharing_sdk-0.1.0.dist-info/RECORD
+Filename: tuya_device_sharing_sdk-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tuya_sharing/user.py

```diff
@@ -19,25 +19,16 @@
     def login_result(self, token: str, client_id: str, user_code: str) -> Tuple[bool, Dict[str, Any]]:
         response = self.session.request("GET",
                                         f"https://t7ywzgs6hjbnvnkfqymf7x4zxq0yaouf.lambda-url.us-west-2.on.aws/v1.0/m/life/home-assistant/qrcode/tokens/{token}?clientid={client_id}&usercode={user_code}",
                                         params=None, json=None, headers=None)
         response = response.json()
         if response.get("success"):
             ret = response.get("result", {})
-            token_info = {
-                "t": response.get("t"),
-                "expire_time": ret.get("expireTime"),
-                "access_token": ret.get("accessToken"),
-                "refresh_token": ret.get("refreshToken"),
-                "terminal_id": ret.get("terminalId"),
-                "username": ret.get("username"),
-                "uid": ret.get("uid"),
-                "end_point": ret.get("host")
-            }
-            return True, token_info
+            ret["t"] = response.get("t")
+            return True, ret
 
         return False, response
 
 
 class UserRepository:
     def __init__(self, customer_api: CustomerApi):
         self.api = customer_api
```

## tuya_sharing/version.py

```diff
@@ -1,3 +1,3 @@
 """smartlife device sharing sdk version."""
 
-VERSION = "0.1.0"
+VERSION = "0.1.1"
```

## Comparing `tuya_device_sharing_sdk-0.1.0.dist-info/LICENSE` & `tuya_device_sharing_sdk-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tuya_device_sharing_sdk-0.1.0.dist-info/METADATA` & `tuya_device_sharing_sdk-0.1.1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuya-device-sharing-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python sdk for Tuya Open API, which provides IoT capabilities, maintained by Tuya official
 Home-page: https://github.com/tuya/tuya-device-sharing-sdk-python
 Author: Tuya Inc.
 Author-email: developer@tuya.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/tuya/tuya-device-sharing-sdk/issues
 Project-URL: Changes, https://github.com/tuya/tuya-device-sharing-sdk/wiki/Tuya-Device-Sharing-SDK-Release-Notes
```

## Comparing `tuya_device_sharing_sdk-0.1.0.dist-info/RECORD` & `tuya_device_sharing_sdk-0.1.1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 tuya_sharing/customerapi.py,sha256=GBmkE7aJpJSleMQ2hOfcCV0VkkpQkmCeh4J0QFXrRNE,8807
 tuya_sharing/customerlogging.py,sha256=M_5Y2fj7xe49DmAlT_vOWlnqyXBBr3tzhEyrOOIsgk4,240
 tuya_sharing/device.py,sha256=kB_PZoNCRb079iA4VatjVdlR9_huSQ9weZg9WjVkjig,4359
 tuya_sharing/home.py,sha256=bpclcYMSg-dm-PewGvjcpAW5mYkR9pQqITiVBI9raww,673
 tuya_sharing/manager.py,sha256=2oa0i81sdpXm9Zp9RHEXJxU3kIGGY_w9zC1VupfGjYM,7334
 tuya_sharing/mq.py,sha256=XuagC2oKVCu8HSiIRJVhaVysU5PoT8WhgjOvTWaoKNs,5744
 tuya_sharing/scenes.py,sha256=v_CMW8MPBw7bTPUoSP-ECWSnsRpBSdmkm326TmZu6PA,1230
-tuya_sharing/user.py,sha256=0b1IkwDVl7IrEC1cZGdVSc09DRSlpcUqzuFgiuDBx3o,2092
-tuya_sharing/version.py,sha256=YlKvXLrrL7iZOK9MQeUUFC220Nxm5LX96XM8MX0kQxc,62
-tuya_device_sharing_sdk-0.1.0.dist-info/LICENSE,sha256=9f5L_7FJLj0ifwYsEnCROE4wmMOLJsQW6ce8Z5hP49U,1079
-tuya_device_sharing_sdk-0.1.0.dist-info/METADATA,sha256=FWtgzN93tS5zA0MeSeiPiPxWdhKf9j85ZdZjq1RWeIo,1692
-tuya_device_sharing_sdk-0.1.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-tuya_device_sharing_sdk-0.1.0.dist-info/top_level.txt,sha256=3J7S7-33ciuBSRIIUDSaFN63plHHiPShvGgOyhAY0no,13
-tuya_device_sharing_sdk-0.1.0.dist-info/RECORD,,
+tuya_sharing/user.py,sha256=MLXgxGcPD-xYj7HE1Jfd0MEdYusL6dDMkNLJSweJyd0,1690
+tuya_sharing/version.py,sha256=Aa5vC4grElN_42PCWeBwdqkJMR5BdU2JPDvG9SCy3Ls,62
+tuya_device_sharing_sdk-0.1.1.dist-info/LICENSE,sha256=9f5L_7FJLj0ifwYsEnCROE4wmMOLJsQW6ce8Z5hP49U,1079
+tuya_device_sharing_sdk-0.1.1.dist-info/METADATA,sha256=21Nc-FOy_LOOL1e1lypeafL4wbkyUU2knWBfLMfToCQ,1692
+tuya_device_sharing_sdk-0.1.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+tuya_device_sharing_sdk-0.1.1.dist-info/top_level.txt,sha256=3J7S7-33ciuBSRIIUDSaFN63plHHiPShvGgOyhAY0no,13
+tuya_device_sharing_sdk-0.1.1.dist-info/RECORD,,
```

