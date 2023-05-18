# Comparing `tmp/alibabacloud_resourcemanager20200331-2.1.3.tar.gz` & `tmp/alibabacloud_resourcemanager20200331-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_resourcemanager20200331-2.1.3.tar", last modified: Wed Feb 22 02:23:04 2023, max compression
+gzip compressed data, was "dist/alibabacloud_resourcemanager20200331-2.1.4.tar", last modified: Thu May 18 08:59:18 2023, max compression
```

## Comparing `alibabacloud_resourcemanager20200331-2.1.3.tar` & `alibabacloud_resourcemanager20200331-2.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 02:23:04.000000 alibabacloud_resourcemanager20200331-2.1.3/
--rw-r--r--   0 root         (0) root         (0)      813 2023-02-22 02:23:04.000000 alibabacloud_resourcemanager20200331-2.1.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-02-22 02:23:04.000000 alibabacloud_resourcemanager20200331-2.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-22 02:23:04.000000 alibabacloud_resourcemanager20200331-2.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2400 2023-02-22 02:23:04.000000 alibabacloud_resourcemanager20200331-2.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1058 2023-02-22 02:23:04.000000 alibabacloud_resourcemanager20200331-2.1.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1143 2023-02-22 02:23:04.000000 alibabacloud_resourcemanager20200331-2.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 02:23:04.000000 alibabacloud_resourcemanager20200331-2.1.3/alibabacloud_resourcemanager20200331/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-22 02:23:04.000000 alibabacloud_resourcemanager20200331-2.1.3/alibabacloud_resourcemanager20200331/__init__.py
--rw-r--r--   0 root         (0) root         (0)   281278 2023-02-22 02:23:04.000000 alibabacloud_resourcemanager20200331-2.1.3/alibabacloud_resourcemanager20200331/client.py
--rw-r--r--   0 root         (0) root         (0)   505940 2023-02-22 02:23:04.000000 alibabacloud_resourcemanager20200331-2.1.3/alibabacloud_resourcemanager20200331/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 02:23:04.000000 alibabacloud_resourcemanager20200331-2.1.3/alibabacloud_resourcemanager20200331.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2400 2023-02-22 02:23:04.000000 alibabacloud_resourcemanager20200331-2.1.3/alibabacloud_resourcemanager20200331.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      516 2023-02-22 02:23:04.000000 alibabacloud_resourcemanager20200331-2.1.3/alibabacloud_resourcemanager20200331.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-22 02:23:04.000000 alibabacloud_resourcemanager20200331-2.1.3/alibabacloud_resourcemanager20200331.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-02-22 02:23:04.000000 alibabacloud_resourcemanager20200331-2.1.3/alibabacloud_resourcemanager20200331.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-02-22 02:23:04.000000 alibabacloud_resourcemanager20200331-2.1.3/alibabacloud_resourcemanager20200331.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-22 02:23:04.000000 alibabacloud_resourcemanager20200331-2.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2670 2023-02-22 02:23:04.000000 alibabacloud_resourcemanager20200331-2.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/
+-rw-r--r--   0 root         (0) root         (0)      887 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   388878 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331/client.py
+-rw-r--r--   0 root         (0) root         (0)   589797 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      516 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/setup.py
```

### Comparing `alibabacloud_resourcemanager20200331-2.1.3/ChangeLog.md` & `alibabacloud_resourcemanager20200331-2.1.4/ChangeLog.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-02-22 Version: 2.1.3
+- Supported more language for resourcemanager.
+
 2022-12-01 Version: 2.1.2
 - Supported more language for resourcemanager.
 
 2022-08-03 Version: 2.1.1
 - Supported more query conditions when searching resource group.
 
 2022-01-14 Version: 2.1.0
```

### Comparing `alibabacloud_resourcemanager20200331-2.1.3/LICENSE` & `alibabacloud_resourcemanager20200331-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331-2.1.3/PKG-INFO` & `alibabacloud_resourcemanager20200331-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_resourcemanager20200331
-Version: 2.1.3
+Version: 2.1.4
 Summary: Alibaba Cloud ResourceManager (20200331) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcemanager20200331-2.1.3/README-CN.md` & `alibabacloud_resourcemanager20200331-2.1.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331-2.1.3/README.md` & `alibabacloud_resourcemanager20200331-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331-2.1.3/alibabacloud_resourcemanager20200331/models.py` & `alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 
 class AcceptHandshakeRequest(TeaModel):
     def __init__(
         self,
         handshake_id: str = None,
     ):
+        # The ID of the invitation.
+        # 
+        # You can call the [ListHandshakesForAccount](~~160006~~) operation to obtain the ID.
         self.handshake_id = handshake_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -42,24 +45,44 @@
         modify_time: str = None,
         note: str = None,
         resource_directory_id: str = None,
         status: str = None,
         target_entity: str = None,
         target_type: str = None,
     ):
+        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time
+        # The time when the invitation expires. The time is displayed in UTC.
         self.expire_time = expire_time
+        # The ID of the invitation.
         self.handshake_id = handshake_id
+        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id
+        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name
+        # The time when the invitation was modified. The time is displayed in UTC.
         self.modify_time = modify_time
+        # The comment on the invitation.
         self.note = note
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending: The invitation is waiting for confirmation.
+        # *   Accepted: The invitation is accepted.
+        # *   Cancelled: The invitation is canceled.
+        # *   Declined: The invitation is rejected.
+        # *   Expired: The invitation expires.
         self.status = status
+        # The ID or logon email address of the invited Alibaba Cloud account.
         self.target_entity = target_entity
+        # The type of the invited Alibaba Cloud account. Valid values:
+        # 
+        # *   Account: indicates the ID of the Alibaba Cloud account.
+        # *   Email: indicates the logon email address of the Alibaba Cloud account.
         self.target_type = target_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -120,15 +143,17 @@
 
 class AcceptHandshakeResponseBody(TeaModel):
     def __init__(
         self,
         handshake: AcceptHandshakeResponseBodyHandshake = None,
         request_id: str = None,
     ):
+        # The information of the invitation.
         self.handshake = handshake
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -199,15 +224,21 @@
 
 class AttachControlPolicyRequest(TeaModel):
     def __init__(
         self,
         policy_id: str = None,
         target_id: str = None,
     ):
+        # The ID of the access control policy.
         self.policy_id = policy_id
+        # The ID of the object to which you want to attach the access control policy. Access control policies can be attached to the following objects:
+        # 
+        # *   Root folder
+        # *   Subfolders of the Root folder
+        # *   Members
         self.target_id = target_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -231,14 +262,15 @@
 
 
 class AttachControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -306,18 +338,41 @@
         self,
         policy_name: str = None,
         policy_type: str = None,
         principal_name: str = None,
         principal_type: str = None,
         resource_group_id: str = None,
     ):
+        # The name of the policy.
+        # 
+        # The name must be 1 to 128 characters in length and can contain letters, digits, and hyphens (-).
         self.policy_name = policy_name
+        # The type of the policy. Valid values:
+        # 
+        # *   Custom: custom policy
+        # *   System: system policy
         self.policy_type = policy_type
+        # The name of the object to which you want to attach the policy.
+        # 
+        # *   If you want to attach the policy to a RAM user, specify the name in the \<UserName>@\<AccountAlias>.onaliyun.com format. \<UserName> indicates the name of the RAM user, and \<AccountAlias> indicates the alias of the Alibaba Cloud account to which the RAM user belongs.
+        # *   If you want to attach the policy to a RAM user group, specify the name in the \<GroupName>@group.\<AccountAlias>.onaliyun.com format. \<GroupName> indicates the name of the RAM user group, and \<AccountAlias> indicates the alias of the Alibaba Cloud account to which the RAM user group belongs.
+        # *   If you want to attach the policy to a RAM role, specify the name in the \<RoleName>@role.\<AccountAlias>.onaliyun.com format. \<RoleName> indicates the name of the RAM role, and \<AccountAlias> indicates the alias of the Alibaba Cloud account to which the RAM role belongs.
+        # 
+        # >  The alias of an Alibaba Cloud account is a part of the default domain name. You can call the [GetDefaultDomain](~~186720~~) operation to obtain the alias of an Alibaba Cloud account.
         self.principal_name = principal_name
+        # The type of the object to which you want to attach the policy. Valid values:
+        # 
+        # *   IMSUser: RAM user
+        # *   IMSGroup: RAM user group
+        # *   ServiceRole: RAM role
         self.principal_type = principal_type
+        # The effective scope of the policy. You can set this parameter to one of the following items:
+        # 
+        # *   ID of a resource group: indicates that the policy takes effect for the resources in the resource group.
+        # *   ID of the Alibaba Cloud account to which the authorized object belongs: indicates that the policy takes effect for the resources within the Alibaba Cloud account.
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -353,14 +408,15 @@
 
 
 class AttachPolicyResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -426,16 +482,27 @@
 class BindSecureMobilePhoneRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         secure_mobile_phone: str = None,
         verification_code: str = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
+        # The mobile phone number that you want to bind to the member for security purposes.
+        # 
+        # The mobile phone number you specify must be the same as the mobile phone number that you specify when you call the [SendVerificationCodeForBindSecureMobilePhone](~~372556~~) operation to obtain a verification code.
+        # 
+        # Specify the mobile phone number in the \<Country code>-\<Mobile phone number> format.
+        # 
+        # >  Mobile phone numbers in the `86-<Mobile phone number>` format in the Chinese mainland are not supported.
         self.secure_mobile_phone = secure_mobile_phone
+        # The verification code.
+        # 
+        # You can call the [SendVerificationCodeForBindSecureMobilePhone](~~372556~~) operation to obtain the verification code.
         self.verification_code = verification_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -463,14 +530,15 @@
 
 
 class BindSecureMobilePhoneResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -534,14 +602,15 @@
 
 
 class CancelChangeAccountEmailRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -561,14 +630,15 @@
 
 
 class CancelChangeAccountEmailResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -632,14 +702,15 @@
 
 
 class CancelCreateCloudAccountRequest(TeaModel):
     def __init__(
         self,
         record_id: str = None,
     ):
+        # The account record ID.
         self.record_id = record_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -659,14 +730,15 @@
 
 
 class CancelCreateCloudAccountResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -730,14 +802,15 @@
 
 
 class CancelHandshakeRequest(TeaModel):
     def __init__(
         self,
         handshake_id: str = None,
     ):
+        # The ID of the invitation.
         self.handshake_id = handshake_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -767,24 +840,44 @@
         modify_time: str = None,
         note: str = None,
         resource_directory_id: str = None,
         status: str = None,
         target_entity: str = None,
         target_type: str = None,
     ):
+        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time
+        # The time when the invitation expires. The time is displayed in UTC.
         self.expire_time = expire_time
+        # The ID of the invitation.
         self.handshake_id = handshake_id
+        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id
+        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name
+        # The time when the invitation was modified. The time is displayed in UTC.
         self.modify_time = modify_time
+        # The comment on the invitation.
         self.note = note
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending: The invitation is waiting for confirmation.
+        # *   Accepted: The invitation is accepted.
+        # *   Cancelled: The invitation is canceled.
+        # *   Declined: The invitation is rejected.
+        # *   Expired: The invitation expires.
         self.status = status
+        # The ID or logon email address of the invited account.
         self.target_entity = target_entity
+        # The type of the invited account. Valid values:
+        # 
+        # *   Account: indicates the ID of the account.
+        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -845,15 +938,17 @@
 
 class CancelHandshakeResponseBody(TeaModel):
     def __init__(
         self,
         handshake: CancelHandshakeResponseBodyHandshake = None,
         request_id: str = None,
     ):
+        # The information of the invitation.
         self.handshake = handshake
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -923,14 +1018,15 @@
 
 
 class CancelPromoteResourceAccountRequest(TeaModel):
     def __init__(
         self,
         record_id: str = None,
     ):
+        # The account record ID.
         self.record_id = record_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -950,14 +1046,15 @@
 
 
 class CancelPromoteResourceAccountResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1022,15 +1119,19 @@
 
 class ChangeAccountEmailRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         email: str = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
+        # The email address to be bound to the member.
+        # 
+        # >  The system automatically sends a verification email to the email address. After the verification is passed, the email address takes effect, and the system changes both the logon email address and secure email address of the member.
         self.email = email
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1054,14 +1155,15 @@
 
 
 class ChangeAccountEmailResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1125,14 +1227,15 @@
 
 
 class CheckAccountDeleteRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
     ):
+        # The ID of the member that you want to delete.
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1152,14 +1255,15 @@
 
 
 class CheckAccountDeleteResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1226,17 +1330,25 @@
     def __init__(
         self,
         display_name: str = None,
         email: str = None,
         parent_folder_id: str = None,
         payer_account_id: str = None,
     ):
+        # The display name of the member account.
+        # 
+        # The name must be 2 to 50 characters in length and can contain letters, digits, underscores (\_), periods (.), and hyphens (-).
+        # 
+        # The name must be unique in the current resource directory.
         self.display_name = display_name
+        # The email address used to log on to the cloud account.
         self.email = email
+        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id
+        # The ID of the settlement account. If you do not specify this parameter, the current account is used for settlement.
         self.payer_account_id = payer_account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1277,23 +1389,49 @@
         join_method: str = None,
         modify_time: str = None,
         record_id: str = None,
         resource_directory_id: str = None,
         status: str = None,
         type: str = None,
     ):
+        # The ID of the member account.
         self.account_id = account_id
+        # The name of the member account.
         self.account_name = account_name
+        # The display name of the member account.
         self.display_name = display_name
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The way in which the member account joined the resource directory. Valid values:
+        # 
+        # *   invited: The member account is invited to join the resource directory.
+        # *   created: The member account is directly created in the resource directory.
         self.join_method = join_method
+        # The time when the member account was modified.
         self.modify_time = modify_time
+        # The account record ID.
         self.record_id = record_id
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the member account. Valid values:
+        # 
+        # *   CreateSuccess: The member account is created.
+        # *   CreateVerifying: The creation of the member account is under confirmation.
+        # *   CreateFailed: The member account failed to be created.
+        # *   CreateExpired: The creation of the member account expired.
+        # *   CreateCancelled: The creation of the member account is canceled.
+        # *   PromoteVerifying: The upgrade of the member account is under confirmation.
+        # *   PromoteFailed: The member account failed to be upgraded.
+        # *   PromoteExpired: The upgrade of the member account expired.
+        # *   PromoteCancelled: The upgrade of the member account is canceled.
+        # *   PromoteSuccess: The member account is upgraded.
+        # *   InviteSuccess: The owner of the member account accepted the invitation.
+        # *   Removed: The member account is removed from the resource directory.
         self.status = status
+        # The type of the member account. The value CloudAccount indicates that the member account is a cloud account.
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1350,15 +1488,17 @@
 
 class CreateCloudAccountResponseBody(TeaModel):
     def __init__(
         self,
         account: CreateCloudAccountResponseBodyAccount = None,
         request_id: str = None,
     ):
+        # The information of the member account.
         self.account = account
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.account:
             self.account.validate()
 
     def to_map(self):
@@ -1431,17 +1571,33 @@
     def __init__(
         self,
         description: str = None,
         effect_scope: str = None,
         policy_document: str = None,
         policy_name: str = None,
     ):
+        # The description of the access control policy.
+        # 
+        # The description must be 1 to 1,024 characters in length. The description can contain letters, digits, underscores (\_), and hyphens (-) and must start with a letter.
         self.description = description
+        # The effective scope of the access control policy.
+        # 
+        # The value RAM indicates that the access control policy takes effect only for RAM users and RAM roles.
         self.effect_scope = effect_scope
+        # The document of the access control policy.
+        # 
+        # The document can be a maximum of 4,096 characters in length.
+        # 
+        # For more information about the languages of access control policies, see [Languages of access control policies](~~179096~~).
+        # 
+        # For more information about the examples of access control policies, see [Examples of custom access control policies](~~181474~~).
         self.policy_document = policy_document
+        # The name of the access control policy.
+        # 
+        # The name must be 1 to 128 characters in length. The name can contain letters, digits, and hyphens (-) and must start with a letter.
         self.policy_name = policy_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1480,21 +1636,34 @@
         description: str = None,
         effect_scope: str = None,
         policy_id: str = None,
         policy_name: str = None,
         policy_type: str = None,
         update_date: str = None,
     ):
+        # The number of times that the access control policy is referenced.
         self.attachment_count = attachment_count
+        # The time when the access control policy was created.
         self.create_date = create_date
+        # The description of the access control policy.
         self.description = description
+        # The effective scope of the access control policy.
+        # 
+        # The value RAM indicates that the access control policy takes effect only for RAM users and RAM roles.
         self.effect_scope = effect_scope
+        # The ID of the access control policy.
         self.policy_id = policy_id
+        # The name of the access control policy.
         self.policy_name = policy_name
+        # The type of the access control policy. Valid values:
+        # 
+        # *   System: system access control policy
+        # *   Custom: custom access control policy
         self.policy_type = policy_type
+        # The time when the access control policy was updated.
         self.update_date = update_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1543,15 +1712,17 @@
 
 class CreateControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         control_policy: CreateControlPolicyResponseBodyControlPolicy = None,
         request_id: str = None,
     ):
+        # The details of the access control policy.
         self.control_policy = control_policy
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.control_policy:
             self.control_policy.validate()
 
     def to_map(self):
@@ -1622,15 +1793,19 @@
 
 class CreateFolderRequest(TeaModel):
     def __init__(
         self,
         folder_name: str = None,
         parent_folder_id: str = None,
     ):
+        # The name of the folder.
+        # 
+        # The name must be 1 to 24 characters in length and can contain letters, digits, underscores (\_), periods (.),and hyphens (-).
         self.folder_name = folder_name
+        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1657,17 +1832,21 @@
     def __init__(
         self,
         create_time: str = None,
         folder_id: str = None,
         folder_name: str = None,
         parent_folder_id: str = None,
     ):
+        # The time when the folder was created.
         self.create_time = create_time
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The name of the folder.
         self.folder_name = folder_name
+        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1700,15 +1879,17 @@
 
 class CreateFolderResponseBody(TeaModel):
     def __init__(
         self,
         folder: CreateFolderResponseBodyFolder = None,
         request_id: str = None,
     ):
+        # The information of the folder.
         self.folder = folder
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.folder:
             self.folder.validate()
 
     def to_map(self):
@@ -1780,16 +1961,25 @@
 class CreatePolicyRequest(TeaModel):
     def __init__(
         self,
         description: str = None,
         policy_document: str = None,
         policy_name: str = None,
     ):
+        # The description of the policy.
+        # 
+        # The description must be 1 to 1,024 characters in length.
         self.description = description
+        # The document of the policy.
+        # 
+        # The document must be 1 to 2,048 characters in length.
         self.policy_document = policy_document
+        # The name of the policy.
+        # 
+        # The name must be 1 to 128 characters in length and can contain letters, digits, and hyphens (-).
         self.policy_name = policy_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1821,18 +2011,26 @@
         self,
         create_date: str = None,
         default_version: str = None,
         description: str = None,
         policy_name: str = None,
         policy_type: str = None,
     ):
+        # The time when the policy was created.
         self.create_date = create_date
+        # The version number of the policy. Default value: v1.
         self.default_version = default_version
+        # The description of the policy.
         self.description = description
+        # The name of the policy.
         self.policy_name = policy_name
+        # The type of the policy. Valid values:
+        # 
+        # *   Custom: custom policy
+        # *   System: system policy
         self.policy_type = policy_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1869,15 +2067,17 @@
 
 class CreatePolicyResponseBody(TeaModel):
     def __init__(
         self,
         policy: CreatePolicyResponseBodyPolicy = None,
         request_id: str = None,
     ):
+        # The information of the policy.
         self.policy = policy
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.policy:
             self.policy.validate()
 
     def to_map(self):
@@ -1949,16 +2149,28 @@
 class CreatePolicyVersionRequest(TeaModel):
     def __init__(
         self,
         policy_document: str = None,
         policy_name: str = None,
         set_as_default: bool = None,
     ):
+        # The document of the policy.
+        # 
+        # The document must be 1 to 2,048 characters in length.
         self.policy_document = policy_document
+        # The name of the policy.
+        # 
+        # The name must be 1 to 128 characters in length and can contain letters, digits, and hyphens (-).
         self.policy_name = policy_name
+        # Specifies whether to set the policy version as the default version. Valid values:
+        # 
+        # *   false: The policy version is not set as the default version.
+        # *   true: The policy version is set as the default version.
+        # 
+        # Default value: false.
         self.set_as_default = set_as_default
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1988,16 +2200,19 @@
 class CreatePolicyVersionResponseBodyPolicyVersion(TeaModel):
     def __init__(
         self,
         create_date: str = None,
         is_default_version: bool = None,
         version_id: str = None,
     ):
+        # The time when the policy version was created.
         self.create_date = create_date
+        # Indicates whether the policy version is the default version.
         self.is_default_version = is_default_version
+        # The ID of the policy version.
         self.version_id = version_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2026,15 +2241,17 @@
 
 class CreatePolicyVersionResponseBody(TeaModel):
     def __init__(
         self,
         policy_version: CreatePolicyVersionResponseBodyPolicyVersion = None,
         request_id: str = None,
     ):
+        # The information of the policy version.
         self.policy_version = policy_version
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.policy_version:
             self.policy_version.validate()
 
     def to_map(self):
@@ -2105,15 +2322,17 @@
 
 class CreateResourceAccountRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
+        # A tag key
         self.key = key
+        # A tag value.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2142,18 +2361,42 @@
         account_name_prefix: str = None,
         display_name: str = None,
         parent_folder_id: str = None,
         payer_account_id: str = None,
         resell_account_type: str = None,
         tag: List[CreateResourceAccountRequestTag] = None,
     ):
+        # The prefix for the Alibaba Cloud account name of the member. If you leave this parameter empty, the system randomly generates a prefix.
+        # 
+        # The prefix must be 2 to 37 characters in length.
+        # 
+        # The prefix can contain letters, digits, and special characters but cannot contain consecutive special characters. The prefix must start with a letter or digit and end with a letter or digit. Valid special characters include underscores (`_`), periods (.), and hyphens (`-`).
+        # 
+        # The complete Alibaba Cloud account name of a member in a resource directory is in the \<AccountNamePrefix>@\<ResourceDirectoryId>.aliyunid.com format, such as `alice@rd-3G****.aliyunid.com`.
+        # 
+        # Each name must be unique in the resource directory.
         self.account_name_prefix = account_name_prefix
+        # The display name of the member.
+        # 
+        # The name must be 2 to 50 characters in length.
+        # 
+        # The name can contain letters, digits, underscores (\_), periods (.), hyphens (-), and spaces.
+        # 
+        # The name must be unique in the resource directory.
         self.display_name = display_name
+        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id
+        # The ID of the billing account. If you leave this parameter empty, the member is used as its own billing account.
         self.payer_account_id = payer_account_id
+        # The identity type of the member. Valid values:
+        # 
+        # *   resell: The member is an account for a reseller. This is the default value. A relationship is automatically established between the member and the reseller. The management account of the resource directory must be used as the billing account of the member.
+        # *   non_resell: The member is not an account for a reseller. The member is an account that is not associated with a reseller. You can directly use the account to purchase Alibaba Cloud resources. The member is used as its own billing account.
+        # 
+        # >  This parameter is available only for resellers at the international site (alibabacloud.com).
         self.resell_account_type = resell_account_type
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
@@ -2211,23 +2454,36 @@
         join_method: str = None,
         join_time: str = None,
         modify_time: str = None,
         resource_directory_id: str = None,
         status: str = None,
         type: str = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
+        # The Alibaba Cloud account name of the member.
         self.account_name = account_name
+        # The display name of the member.
         self.display_name = display_name
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The way in which the member joins the resource directory. Valid values:
+        # 
+        # *   invited: The member is invited to join the resource directory.
+        # *   created: The member is directly created in the resource directory.
         self.join_method = join_method
+        # The time when the member joined the resource directory. The time is displayed in UTC.
         self.join_time = join_time
+        # The time when the member was modified. The time is displayed in UTC.
         self.modify_time = modify_time
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the member. The value CreateSuccess indicates that the member is created.
         self.status = status
+        # The type of the member. The value ResourceAccount indicates that the member is a resource account.
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2284,15 +2540,17 @@
 
 class CreateResourceAccountResponseBody(TeaModel):
     def __init__(
         self,
         account: CreateResourceAccountResponseBodyAccount = None,
         request_id: str = None,
     ):
+        # The information of the member.
         self.account = account
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.account:
             self.account.validate()
 
     def to_map(self):
@@ -2363,15 +2621,19 @@
 
 class CreateResourceGroupRequest(TeaModel):
     def __init__(
         self,
         display_name: str = None,
         name: str = None,
     ):
+        # The ID of the request.
         self.display_name = display_name
+        # The display name of the resource group.
+        # 
+        # The name must be 1 to 50 characters in length.
         self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2396,15 +2658,17 @@
 
 class CreateResourceGroupResponseBodyResourceGroupRegionStatusesRegionStatus(TeaModel):
     def __init__(
         self,
         region_id: str = None,
         status: str = None,
     ):
+        # The ID of the Alibaba Cloud account to which the resource group belongs.
         self.region_id = region_id
+        # The region ID.
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2469,20 +2733,32 @@
         create_date: str = None,
         display_name: str = None,
         id: str = None,
         name: str = None,
         region_statuses: CreateResourceGroupResponseBodyResourceGroupRegionStatuses = None,
         status: str = None,
     ):
+        # The unique identifier of the resource group.
         self.account_id = account_id
+        # The ID of the resource group.
         self.create_date = create_date
+        # The status of the resource group. Valid values:
+        # 
+        # *   Creating: The resource group is being created.
+        # *   OK: The resource group is created.
         self.display_name = display_name
         self.id = id
+        # The time when the resource group was created. The time is displayed in UTC.
         self.name = name
+        # The status of the resource group. Valid values:
+        # 
+        # *   Creating: The resource group is being created.
+        # *   OK: The resource group is created.
         self.region_statuses = region_statuses
+        # The status of the resource group in all regions.
         self.status = status
 
     def validate(self):
         if self.region_statuses:
             self.region_statuses.validate()
 
     def to_map(self):
@@ -2529,15 +2805,17 @@
 
 class CreateResourceGroupResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_group: CreateResourceGroupResponseBodyResourceGroup = None,
     ):
+        # The information of the resource group.
         self.request_id = request_id
+        # The display name of the resource group.
         self.resource_group = resource_group
 
     def validate(self):
         if self.resource_group:
             self.resource_group.validate()
 
     def to_map(self):
@@ -2610,17 +2888,31 @@
     def __init__(
         self,
         assume_role_policy_document: str = None,
         description: str = None,
         max_session_duration: int = None,
         role_name: str = None,
     ):
+        # The document of the policy that specifies one or more trusted entities to assume the RAM role. The trusted entities can be Alibaba Cloud accounts, Alibaba Cloud services, or identity providers (IdPs).
+        # 
+        # >  RAM users cannot assume the RAM roles of trusted Alibaba Cloud services.
         self.assume_role_policy_document = assume_role_policy_document
+        # The description of the RAM role.
+        # 
+        # The description must be 1 to 1,024 characters in length.
         self.description = description
+        # The maximum session duration of the RAM role.
+        # 
+        # Unit: seconds. Valid values: 3600 to 43200. Default value: 3600.
+        # 
+        # If you do not specify this parameter, the default value is used.
         self.max_session_duration = max_session_duration
+        # The name of the RAM role.
+        # 
+        # The name must be 1 to 64 characters in length and can contain letters, digits, periods (.), and hyphens (-).
         self.role_name = role_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2659,21 +2951,29 @@
         create_date: str = None,
         description: str = None,
         max_session_duration: int = None,
         role_id: str = None,
         role_name: str = None,
         role_principal_name: str = None,
     ):
+        # The Alibaba Cloud Resource Name (ARN) of the RAM role.
         self.arn = arn
+        # The document of the policy that specifies the trusted entity to assume the RAM role.
         self.assume_role_policy_document = assume_role_policy_document
+        # The time when the RAM role was created.
         self.create_date = create_date
+        # The description of the RAM role.
         self.description = description
+        # The maximum session duration of the RAM role.
         self.max_session_duration = max_session_duration
+        # The ID of the RAM role.
         self.role_id = role_id
+        # The name of the RAM role.
         self.role_name = role_name
+        # The name of the RAM role after authorization.
         self.role_principal_name = role_principal_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2722,15 +3022,17 @@
 
 class CreateRoleResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         role: CreateRoleResponseBodyRole = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
+        # The information of the RAM role.
         self.role = role
 
     def validate(self):
         if self.role:
             self.role.validate()
 
     def to_map(self):
@@ -2802,16 +3104,29 @@
 class CreateServiceLinkedRoleRequest(TeaModel):
     def __init__(
         self,
         custom_suffix: str = None,
         description: str = None,
         service_name: str = None,
     ):
+        # The suffix of the role name.
+        # 
+        # The role name (including its suffix) must be 1 to 64 characters in length and can contain letters, digits, periods (.), and hyphens (-).
+        # 
+        # For example, if the suffix is `Example`, the role name is `ServiceLinkedRoleName_Example`.
         self.custom_suffix = custom_suffix
+        # The description of the service-linked role.
+        # 
+        # You must configure this parameter for service-linked roles that support custom suffixes. Otherwise, the preset value is used and cannot be modified.
+        # 
+        # The description must be 1 to 1,024 characters in length.
         self.description = description
+        # The name of the service.
+        # 
+        # For more information about the service name, see [Alibaba Cloud services that support service-linked roles](~~461722~~).
         self.service_name = service_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2846,21 +3161,32 @@
         create_date: str = None,
         description: str = None,
         is_service_linked_role: bool = None,
         role_id: str = None,
         role_name: str = None,
         role_principal_name: str = None,
     ):
+        # The Alibaba Cloud Resource Name (ARN) of the role.
         self.arn = arn
+        # The document of the trust policy for the role.
         self.assume_role_policy_document = assume_role_policy_document
+        # The time when the role was created. The time is displayed in UTC.
         self.create_date = create_date
+        # The description of the role.
         self.description = description
+        # Indicates whether the role is a service-linked role. Valid values:
+        # 
+        # *   true: The role is a service-linked role.
+        # *   false: The role is not a service-linked role.
         self.is_service_linked_role = is_service_linked_role
+        # The ID of the role.
         self.role_id = role_id
+        # The name of the role.
         self.role_name = role_name
+        # The role name that uses a domain name as the suffix.
         self.role_principal_name = role_principal_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2909,15 +3235,17 @@
 
 class CreateServiceLinkedRoleResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         role: CreateServiceLinkedRoleResponseBodyRole = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
+        # The information about the role.
         self.role = role
 
     def validate(self):
         if self.role:
             self.role.validate()
 
     def to_map(self):
@@ -2987,14 +3315,15 @@
 
 
 class DeclineHandshakeRequest(TeaModel):
     def __init__(
         self,
         handshake_id: str = None,
     ):
+        # The ID of the invitation.
         self.handshake_id = handshake_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3024,24 +3353,44 @@
         modify_time: str = None,
         note: str = None,
         resource_directory_id: str = None,
         status: str = None,
         target_entity: str = None,
         target_type: str = None,
     ):
+        # The time when the invitation was created.
         self.create_time = create_time
+        # The time when the invitation expires.
         self.expire_time = expire_time
+        # The ID of the invitation.
         self.handshake_id = handshake_id
+        # The ID of the enterprise management account of the resource directory.
         self.master_account_id = master_account_id
+        # The name of the enterprise management account of the resource directory.
         self.master_account_name = master_account_name
+        # The time when the invitation was modified.
         self.modify_time = modify_time
+        # The invitation note.
         self.note = note
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending: The invitation is waiting for confirmation.
+        # *   Accepted: The invitation is accepted.
+        # *   Cancelled: The invitation is canceled.
+        # *   Declined: The invitation is rejected.
+        # *   Expired: The invitation expired.
         self.status = status
+        # The ID or logon email address of the invited account.
         self.target_entity = target_entity
+        # The type of the invited account. Valid values:
+        # 
+        # *   Account: indicates the ID of the account.
+        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3102,15 +3451,17 @@
 
 class DeclineHandshakeResponseBody(TeaModel):
     def __init__(
         self,
         handshake: DeclineHandshakeResponseBodyHandshake = None,
         request_id: str = None,
     ):
+        # The information of the invitation.
         self.handshake = handshake
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -3182,14 +3533,18 @@
 class DeleteAccountRequest(TeaModel):
     def __init__(
         self,
         abandonable_check_id: List[str] = None,
         account_id: str = None,
     ):
         self.abandonable_check_id = abandonable_check_id
+        # The type of the deletion. Valid values:
+        # 
+        # *   0: direct deletion. If the member does not have pay-as-you-go resources that are purchased within the previous 30 days, the system directly deletes the member.
+        # *   1: deletion with a silence period. If the member has pay-as-you-go resources that are purchased within the previous 30 days, the member enters a silence period of 45 days. The system starts to delete the member until the silence period ends. For more information about the silence period, see [What is the silence period for member deletion?](~~446079~~)
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3215,14 +3570,18 @@
 class DeleteAccountShrinkRequest(TeaModel):
     def __init__(
         self,
         abandonable_check_id_shrink: str = None,
         account_id: str = None,
     ):
         self.abandonable_check_id_shrink = abandonable_check_id_shrink
+        # The type of the deletion. Valid values:
+        # 
+        # *   0: direct deletion. If the member does not have pay-as-you-go resources that are purchased within the previous 30 days, the system directly deletes the member.
+        # *   1: deletion with a silence period. If the member has pay-as-you-go resources that are purchased within the previous 30 days, the member enters a silence period of 45 days. The system starts to delete the member until the silence period ends. For more information about the silence period, see [What is the silence period for member deletion?](~~446079~~)
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3323,14 +3682,15 @@
 
 
 class DeleteControlPolicyRequest(TeaModel):
     def __init__(
         self,
         policy_id: str = None,
     ):
+        # The ID of the control policy.
         self.policy_id = policy_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3350,14 +3710,15 @@
 
 
 class DeleteControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3421,14 +3782,15 @@
 
 
 class DeleteFolderRequest(TeaModel):
     def __init__(
         self,
         folder_id: str = None,
     ):
+        # The ID of the folder.
         self.folder_id = folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3448,14 +3810,15 @@
 
 
 class DeleteFolderResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3519,14 +3882,17 @@
 
 
 class DeletePolicyRequest(TeaModel):
     def __init__(
         self,
         policy_name: str = None,
     ):
+        # The name of the policy.
+        # 
+        # The name must be 1 to 128 characters in length and can contain letters, digits, and hyphens (-).
         self.policy_name = policy_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3546,14 +3912,15 @@
 
 
 class DeletePolicyResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3618,15 +3985,21 @@
 
 class DeletePolicyVersionRequest(TeaModel):
     def __init__(
         self,
         policy_name: str = None,
         version_id: str = None,
     ):
+        # The name of the policy.
+        # 
+        # The name must be 1 to 128 characters in length and can contain letters, digits, and hyphens (-).
         self.policy_name = policy_name
+        # The ID of the policy version.
+        # 
+        # You can call the [ListPolicyVersions](~~159982~~) operation to query the ID.
         self.version_id = version_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3650,14 +4023,15 @@
 
 
 class DeletePolicyVersionResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3721,14 +4095,17 @@
 
 
 class DeleteResourceGroupRequest(TeaModel):
     def __init__(
         self,
         resource_group_id: str = None,
     ):
+        # The ID of the resource group.
+        # 
+        # You can call the [ListResourceGroups](~~158855~~) operation to obtain the ID.
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3749,15 +4126,22 @@
 
 class DeleteResourceGroupResponseBodyResourceGroupRegionStatusesRegionStatus(TeaModel):
     def __init__(
         self,
         region_id: str = None,
         status: str = None,
     ):
+        # The region ID.
         self.region_id = region_id
+        # The status of the resource group. Valid values:
+        # 
+        # *   Creating: The resource group is being created.
+        # *   OK: The resource group is created.
+        # *   PendingDelete: The resource group is waiting to be deleted.
+        # *   Deleting: The resource group is being deleted.
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3822,20 +4206,31 @@
         create_date: str = None,
         display_name: str = None,
         id: str = None,
         name: str = None,
         region_statuses: DeleteResourceGroupResponseBodyResourceGroupRegionStatuses = None,
         status: str = None,
     ):
+        # The ID of the Alibaba Cloud account to which the resource group belongs.
         self.account_id = account_id
+        # The time when the resource group was created. The time is displayed in UTC.
         self.create_date = create_date
+        # The display name of the resource group.
         self.display_name = display_name
+        # The ID of the resource group.
         self.id = id
+        # The unique identifier of the resource group.
         self.name = name
+        # The status of the resource group in all regions.
         self.region_statuses = region_statuses
+        # The status of the resource group. Valid values:
+        # 
+        # *   Creating: The resource group is being created.
+        # *   OK: The resource group is created.
+        # *   PendingDelete: The resource group is waiting to be deleted.
         self.status = status
 
     def validate(self):
         if self.region_statuses:
             self.region_statuses.validate()
 
     def to_map(self):
@@ -3882,15 +4277,17 @@
 
 class DeleteResourceGroupResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_group: DeleteResourceGroupResponseBodyResourceGroup = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
+        # The information of the resource group.
         self.resource_group = resource_group
 
     def validate(self):
         if self.resource_group:
             self.resource_group.validate()
 
     def to_map(self):
@@ -3960,14 +4357,17 @@
 
 
 class DeleteRoleRequest(TeaModel):
     def __init__(
         self,
         role_name: str = None,
     ):
+        # The name of the RAM role.
+        # 
+        # The name must be 1 to 64 characters in length and can contain letters, digits, periods (.), and hyphens (-).
         self.role_name = role_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3987,14 +4387,15 @@
 
 
 class DeleteRoleResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4058,14 +4459,15 @@
 
 
 class DeleteServiceLinkedRoleRequest(TeaModel):
     def __init__(
         self,
         role_name: str = None,
     ):
+        # The name of the role.
         self.role_name = role_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4086,15 +4488,17 @@
 
 class DeleteServiceLinkedRoleResponseBody(TeaModel):
     def __init__(
         self,
         deletion_task_id: str = None,
         request_id: str = None,
     ):
+        # The ID of the deletion task.
         self.deletion_task_id = deletion_task_id
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4163,15 +4567,19 @@
 
 class DeregisterDelegatedAdministratorRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         service_principal: str = None,
     ):
+        # The ID of the member in the resource directory.
         self.account_id = account_id
+        # The identifier of the trusted service.
+        # 
+        # For more information, see the `Trusted service identifier` column in [Supported trusted services](~~208133~~).
         self.service_principal = service_principal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4195,14 +4603,15 @@
 
 
 class DeregisterDelegatedAdministratorResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4266,14 +4675,15 @@
 
 
 class DestroyResourceDirectoryResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4338,15 +4748,21 @@
 
 class DetachControlPolicyRequest(TeaModel):
     def __init__(
         self,
         policy_id: str = None,
         target_id: str = None,
     ):
+        # The ID of the access control policy.
         self.policy_id = policy_id
+        # The ID of the object from which you want to detach the access control policy. Access control policies can be attached to the following objects:
+        # 
+        # *   Root folder
+        # *   Subfolders of the Root folder
+        # *   Members
         self.target_id = target_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4370,14 +4786,15 @@
 
 
 class DetachControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4445,18 +4862,34 @@
         self,
         policy_name: str = None,
         policy_type: str = None,
         principal_name: str = None,
         principal_type: str = None,
         resource_group_id: str = None,
     ):
+        # The name of the policy.
+        # 
+        # The name must be 1 to 128 characters in length and can contain letters, digits, and hyphens (-).
         self.policy_name = policy_name
+        # The type of the policy. Valid values:
+        # 
+        # *   Custom: custom policy
+        # *   System: system policy
         self.policy_type = policy_type
+        # The name of the object to which the policy is attached.
         self.principal_name = principal_name
+        # The type of the object to which the policy is attached. Valid values:
+        # 
+        # *   IMSUser: RAM user
+        # *   IMSGroup: RAM user group
+        # *   ServiceRole: RAM role
         self.principal_type = principal_type
+        # The ID of the resource group or the ID of the Alibaba Cloud account to which the resource group belongs.
+        # 
+        # This parameter specifies the resource group or Alibaba Cloud account for which you want to revoke permissions.
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4492,14 +4925,15 @@
 
 
 class DetachPolicyResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4564,15 +4998,22 @@
 
 class DisableControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         enablement_status: str = None,
         request_id: str = None,
     ):
+        # The status of the Control Policy feature. Valid values:
+        # 
+        # *   Enabled: The Control Policy feature is enabled.
+        # *   PendingEnable: The Control Policy feature is being enabled.
+        # *   Disabled: The Control Policy feature is disabled.
+        # *   PendingDisable: The Control Policy feature is being disabled.
         self.enablement_status = enablement_status
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4641,15 +5082,22 @@
 
 class EnableControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         enablement_status: str = None,
         request_id: str = None,
     ):
+        # The status of the Control Policy feature. Valid values:
+        # 
+        # *   Enabled: The Control Policy feature is enabled.
+        # *   PendingEnable: The Control Policy feature is being enabled.
+        # *   Disabled: The Control Policy feature is disabled.
+        # *   PendingDisable: The Control Policy feature is being disabled.
         self.enablement_status = enablement_status
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4720,17 +5168,34 @@
     def __init__(
         self,
         enable_mode: str = None,
         maname: str = None,
         masecure_mobile_phone: str = None,
         verification_code: str = None,
     ):
+        # The mode in which you enable a resource directory. Valid values:
+        # 
+        # *   CurrentAccount: indicates that the current account is used to enable a resource directory.
+        # *   NewManagementAccount: indicates that a newly created account is used to enable a resource directory. If you select this mode, you must configure the `MAName`, `MASecureMobilePhone`, and `VerificationCode` parameters.
         self.enable_mode = enable_mode
+        # The name of the newly created account.
+        # 
+        # Specify the name in the `<Prefix>@rdadmin.aliyunid.com` format. The prefix can contain letters, digits, and special characters but cannot contain consecutive special characters. The prefix must start with a letter or digit and end with a letter or digit. Valid special characters include underscores (\_), periods (.), and hyphens (-). The prefix must be 2 to 50 characters in length.
         self.maname = maname
+        # The mobile phone number that is bound to the newly created account.
+        # 
+        # If you leave this parameter empty, the mobile phone number that is bound to the current account is used. The mobile phone number you specify must be the same as the mobile phone number that you specify when you call the [SendVerificationCodeForEnableRD](~~364248~~) operation to obtain a verification code.
+        # 
+        # Specify the mobile phone number in the `<Country code>-<Mobile phone number>` format.
+        # 
+        # >  Mobile phone numbers in the `86-<Mobile phone number>` format in the Chinese mainland are not supported.
         self.masecure_mobile_phone = masecure_mobile_phone
+        # The verification code.
+        # 
+        # You can call the [SendVerificationCodeForEnableRD](~~364248~~) operation to obtain the verification code.
         self.verification_code = verification_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4766,18 +5231,23 @@
         self,
         create_time: str = None,
         master_account_id: str = None,
         master_account_name: str = None,
         resource_directory_id: str = None,
         root_folder_id: str = None,
     ):
+        # The time when the resource directory was enabled.
         self.create_time = create_time
+        # The ID of the management account.
         self.master_account_id = master_account_id
+        # The name of the management account.
         self.master_account_name = master_account_name
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The ID of the Root folder.
         self.root_folder_id = root_folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4814,15 +5284,17 @@
 
 class EnableResourceDirectoryResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_directory: EnableResourceDirectoryResponseBodyResourceDirectory = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
+        # The information of the resource directory.
         self.resource_directory = resource_directory
 
     def validate(self):
         if self.resource_directory:
             self.resource_directory.validate()
 
     def to_map(self):
@@ -4893,15 +5365,20 @@
 
 class GetAccountRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         include_tags: bool = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
+        # Specifies whether to return the information of tags. Valid values:
+        # 
+        # *   false (default value)
+        # *   true
         self.include_tags = include_tags
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4926,15 +5403,17 @@
 
 class GetAccountResponseBodyAccountTags(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
+        # A tag key.
         self.key = key
+        # A tag value.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4972,28 +5451,63 @@
         modify_time: str = None,
         resource_directory_id: str = None,
         resource_directory_path: str = None,
         status: str = None,
         tags: List[GetAccountResponseBodyAccountTags] = None,
         type: str = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
+        # The Alibaba Cloud account name of the member.
         self.account_name = account_name
+        # The display name of the member.
         self.display_name = display_name
+        # The status of the modification for the email address bound to the member. Valid values:
+        # 
+        # *   WAIT_MODIFY: in progress
+        # *   CANCELLED: canceled
+        # *   EXPIRED: expired
+        # 
+        # If the value of this parameter is empty, no modification is performed for the email address.
         self.email_status = email_status
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The real-name verification information.
         self.identity_information = identity_information
+        # The way in which the member joins the resource directory. Valid values:
+        # 
+        # *   invited: The member is invited to join the resource directory.
+        # *   created: The member is directly created in the resource directory.
         self.join_method = join_method
+        # The time when the member joined the resource directory.
         self.join_time = join_time
+        # The location of the member in the resource directory.
         self.location = location
+        # The time when the member was modified.
         self.modify_time = modify_time
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The path of the member in the resource directory.
         self.resource_directory_path = resource_directory_path
+        # The status of the member. Valid values:
+        # 
+        # *   CreateSuccess: The member is created.
+        # *   PromoteVerifying: The upgrade of the member is being confirmed.
+        # *   PromoteFailed: The upgrade of the member fails.
+        # *   PromoteExpired: The upgrade of the member expires.
+        # *   PromoteCancelled: The upgrade of the member is canceled.
+        # *   PromoteSuccess: The member is upgraded.
+        # *   InviteSuccess: The member accepts the invitation.
         self.status = status
+        # The tags that are added to the member.
         self.tags = tags
+        # The type of the member. Valid values:
+        # 
+        # *   CloudAccount: cloud account
+        # *   ResourceAccount: resource account
         self.type = type
 
     def validate(self):
         if self.tags:
             for k in self.tags:
                 if k:
                     k.validate()
@@ -5078,15 +5592,17 @@
 
 class GetAccountResponseBody(TeaModel):
     def __init__(
         self,
         account: GetAccountResponseBodyAccount = None,
         request_id: str = None,
     ):
+        # The information of the member.
         self.account = account
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.account:
             self.account.validate()
 
     def to_map(self):
@@ -5156,14 +5672,15 @@
 
 
 class GetAccountDeletionCheckResultRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
     ):
+        # The ID of the member that you want to delete.
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5185,16 +5702,19 @@
 class GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfoAbandonableChecks(TeaModel):
     def __init__(
         self,
         check_id: str = None,
         check_name: str = None,
         description: str = None,
     ):
+        # The ID of the check item.
         self.check_id = check_id
+        # The name of the cloud service to which the check item belongs.
         self.check_name = check_name
+        # The description of the check item.
         self.description = description
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5224,16 +5744,19 @@
 class GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfoNotAllowReason(TeaModel):
     def __init__(
         self,
         check_id: str = None,
         check_name: str = None,
         description: str = None,
     ):
+        # The ID of the check item.
         self.check_id = check_id
+        # The name of the cloud service to which the check item belongs.
         self.check_name = check_name
+        # The description of the check item.
         self.description = description
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5264,17 +5787,31 @@
     def __init__(
         self,
         abandonable_checks: List[GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfoAbandonableChecks] = None,
         allow_delete: str = None,
         not_allow_reason: List[GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfoNotAllowReason] = None,
         status: str = None,
     ):
+        # The check items that you can choose to ignore for the member deletion.
+        # 
+        # >  This parameter may be returned if the value of AllowDelete is true.
         self.abandonable_checks = abandonable_checks
+        # Indicates whether the member can be deleted. Valid values:
+        # 
+        # *   true: The member can be deleted.
+        # *   false: The member cannot be deleted.
         self.allow_delete = allow_delete
+        # The reasons why the member cannot be deleted.
+        # 
+        # >  This parameter is returned only if the value of AllowDelete is false.
         self.not_allow_reason = not_allow_reason
+        # The status of the check. Valid values:
+        # 
+        # *   PreCheckComplete: The check is complete.
+        # *   PreChecking: The check is in progress.
         self.status = status
 
     def validate(self):
         if self.abandonable_checks:
             for k in self.abandonable_checks:
                 if k:
                     k.validate()
@@ -5324,15 +5861,17 @@
 
 class GetAccountDeletionCheckResultResponseBody(TeaModel):
     def __init__(
         self,
         account_deletion_check_result_info: GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfo = None,
         request_id: str = None,
     ):
+        # The result of the deletion check for the member.
         self.account_deletion_check_result_info = account_deletion_check_result_info
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.account_deletion_check_result_info:
             self.account_deletion_check_result_info.validate()
 
     def to_map(self):
@@ -5607,15 +6146,23 @@
 
 class GetControlPolicyRequest(TeaModel):
     def __init__(
         self,
         language: str = None,
         policy_id: str = None,
     ):
+        # The language in which you want to return the description of the access control policy. Valid values:
+        # 
+        # *   zh-CN (default value): Chinese
+        # *   en: English
+        # *   ja: Japanese
+        # 
+        # >  This parameter is valid only for system access control policies.
         self.language = language
+        # The ID of the access control policy.
         self.policy_id = policy_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5647,22 +6194,37 @@
         effect_scope: str = None,
         policy_document: str = None,
         policy_id: str = None,
         policy_name: str = None,
         policy_type: str = None,
         update_date: str = None,
     ):
+        # The number of times that the access control policy is referenced.
         self.attachment_count = attachment_count
+        # The time when the access control policy was created.
         self.create_date = create_date
+        # The description of the access control policy.
         self.description = description
+        # The effective scope of the access control policy. Valid values:
+        # 
+        # *   All: The access control policy is in effect for Alibaba Cloud accounts, RAM users, and RAM roles.
+        # *   RAM: The access control policy is in effect only for RAM users and RAM roles.
         self.effect_scope = effect_scope
+        # The document of the access control policy.
         self.policy_document = policy_document
+        # The ID of the access control policy.
         self.policy_id = policy_id
+        # The name of the access control policy.
         self.policy_name = policy_name
+        # The type of the access control policy. Valid values:
+        # 
+        # *   System: system access control policy
+        # *   Custom: custom access control policy
         self.policy_type = policy_type
+        # The time when the access control policy was updated.
         self.update_date = update_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5715,15 +6277,17 @@
 
 class GetControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         control_policy: GetControlPolicyResponseBodyControlPolicy = None,
         request_id: str = None,
     ):
+        # The details of the access control policy.
         self.control_policy = control_policy
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.control_policy:
             self.control_policy.validate()
 
     def to_map(self):
@@ -5794,15 +6358,22 @@
 
 class GetControlPolicyEnablementStatusResponseBody(TeaModel):
     def __init__(
         self,
         enablement_status: str = None,
         request_id: str = None,
     ):
+        # The status of the Control Policy feature. Valid values:
+        # 
+        # *   Enabled: The Control Policy feature is enabled.
+        # *   PendingEnable: The Control Policy feature is being enabled.
+        # *   Disabled: The Control Policy feature is disabled.
+        # *   PendingDisable: The Control Policy feature is being disabled.
         self.enablement_status = enablement_status
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5870,14 +6441,15 @@
 
 
 class GetFolderRequest(TeaModel):
     def __init__(
         self,
         folder_id: str = None,
     ):
+        # The ID of the folder.
         self.folder_id = folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5901,18 +6473,23 @@
         self,
         create_time: str = None,
         folder_id: str = None,
         folder_name: str = None,
         parent_folder_id: str = None,
         resource_directory_path: str = None,
     ):
+        # The time when the folder was created.
         self.create_time = create_time
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The name of the folder.
         self.folder_name = folder_name
+        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id
+        # The path of the folder in the resource directory.
         self.resource_directory_path = resource_directory_path
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5949,15 +6526,17 @@
 
 class GetFolderResponseBody(TeaModel):
     def __init__(
         self,
         folder: GetFolderResponseBodyFolder = None,
         request_id: str = None,
     ):
+        # The information of the folder.
         self.folder = folder
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.folder:
             self.folder.validate()
 
     def to_map(self):
@@ -6027,14 +6606,15 @@
 
 
 class GetHandshakeRequest(TeaModel):
     def __init__(
         self,
         handshake_id: str = None,
     ):
+        # The ID of the invitation.
         self.handshake_id = handshake_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6066,26 +6646,52 @@
         modify_time: str = None,
         note: str = None,
         resource_directory_id: str = None,
         status: str = None,
         target_entity: str = None,
         target_type: str = None,
     ):
+        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time
+        # The time when the invitation expires. The time is displayed in UTC.
         self.expire_time = expire_time
+        # The ID of the invitation.
         self.handshake_id = handshake_id
+        # The real-name verification information of the invitee.
+        # 
+        # >  This parameter is available only when an invitee calls this operation.
         self.invited_account_real_name = invited_account_real_name
+        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id
+        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name
+        # The real-name verification information of the management account of the resource directory.
+        # 
+        # >  This parameter is available only when an invitee calls this operation.
         self.master_account_real_name = master_account_real_name
+        # The time when the invitation was modified. The time is displayed in UTC.
         self.modify_time = modify_time
+        # The comment on the invitation.
         self.note = note
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending: The invitation is waiting for confirmation.
+        # *   Accepted: The invitation is accepted.
+        # *   Cancelled: The invitation is canceled.
+        # *   Declined: The invitation is rejected.
+        # *   Expired: The invitation expires.
         self.status = status
+        # The ID or logon email address of the invited account.
         self.target_entity = target_entity
+        # The type of the invited account. Valid values:
+        # 
+        # *   Account: indicates the ID of the account.
+        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6154,15 +6760,17 @@
 
 class GetHandshakeResponseBody(TeaModel):
     def __init__(
         self,
         handshake: GetHandshakeResponseBodyHandshake = None,
         request_id: str = None,
     ):
+        # The information of the invitation.
         self.handshake = handshake
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -6232,14 +6840,15 @@
 
 
 class GetPayerForAccountRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
     ):
+        # The ID of the account.
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6261,16 +6870,19 @@
 class GetPayerForAccountResponseBody(TeaModel):
     def __init__(
         self,
         payer_account_id: str = None,
         payer_account_name: str = None,
         request_id: str = None,
     ):
+        # The ID of the settlement account.
         self.payer_account_id = payer_account_id
+        # The name of the settlement account.
         self.payer_account_name = payer_account_name
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6344,16 +6956,28 @@
 class GetPolicyRequest(TeaModel):
     def __init__(
         self,
         language: str = None,
         policy_name: str = None,
         policy_type: str = None,
     ):
+        # The language that is used to return the description of the system policy. Valid values:
+        # 
+        # *   en: English
+        # *   zh-CN: Chinese
+        # *   ja: Japanese
         self.language = language
+        # The name of the policy.
+        # 
+        # The name must be 1 to 128 characters in length and can contain letters, digits, and hyphens (-).
         self.policy_name = policy_name
+        # The type of the policy. Valid values:
+        # 
+        # *   Custom: custom policy
+        # *   System: system policy
         self.policy_type = policy_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6388,21 +7012,32 @@
         default_version: str = None,
         description: str = None,
         policy_document: str = None,
         policy_name: str = None,
         policy_type: str = None,
         update_date: str = None,
     ):
+        # The number of times the policy is referenced.
         self.attachment_count = attachment_count
+        # The time when the policy was created.
         self.create_date = create_date
+        # The default version of the policy.
         self.default_version = default_version
+        # The description of the policy.
         self.description = description
+        # The document of the policy.
         self.policy_document = policy_document
+        # The name of the policy.
         self.policy_name = policy_name
+        # The type of the policy. Valid values:
+        # 
+        # *   Custom: custom policy
+        # *   System: system policy
         self.policy_type = policy_type
+        # The time when the policy was updated.
         self.update_date = update_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6451,15 +7086,17 @@
 
 class GetPolicyResponseBody(TeaModel):
     def __init__(
         self,
         policy: GetPolicyResponseBodyPolicy = None,
         request_id: str = None,
     ):
+        # The information of the policy.
         self.policy = policy
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.policy:
             self.policy.validate()
 
     def to_map(self):
@@ -6531,16 +7168,24 @@
 class GetPolicyVersionRequest(TeaModel):
     def __init__(
         self,
         policy_name: str = None,
         policy_type: str = None,
         version_id: str = None,
     ):
+        # The name of the policy.
+        # 
+        # The name must be 1 to 128 characters in length and can contain letters, digits, and hyphens (-).
         self.policy_name = policy_name
+        # The type of the policy. Valid values:
+        # 
+        # *   Custom: custom policy
+        # *   System: system policy
         self.policy_type = policy_type
+        # The ID of the policy version.
         self.version_id = version_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6571,17 +7216,21 @@
     def __init__(
         self,
         create_date: str = None,
         is_default_version: bool = None,
         policy_document: str = None,
         version_id: str = None,
     ):
+        # The time when the policy version was created.
         self.create_date = create_date
+        # Indicates whether the policy version is the default version.
         self.is_default_version = is_default_version
+        # The document of the policy.
         self.policy_document = policy_document
+        # The ID of the policy version.
         self.version_id = version_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6614,15 +7263,17 @@
 
 class GetPolicyVersionResponseBody(TeaModel):
     def __init__(
         self,
         policy_version: GetPolicyVersionResponseBodyPolicyVersion = None,
         request_id: str = None,
     ):
+        # The information of the policy version.
         self.policy_version = policy_version
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.policy_version:
             self.policy_version.validate()
 
     def to_map(self):
@@ -6699,21 +7350,37 @@
         identity_information: str = None,
         master_account_id: str = None,
         master_account_name: str = None,
         member_deletion_status: str = None,
         resource_directory_id: str = None,
         root_folder_id: str = None,
     ):
+        # The status of the Control Policy feature. Valid values:
+        # 
+        # *   Enabled: The feature is enabled.
+        # *   PendingEnable: The feature is being enabled.
+        # *   Disabled: The feature is disabled.
+        # *   PendingDisable: The feature is being disabled.
         self.control_policy_status = control_policy_status
+        # The time when the resource directory was enabled.
         self.create_time = create_time
+        # The real-name verification information.
         self.identity_information = identity_information
+        # The ID of the management account.
         self.master_account_id = master_account_id
+        # The name of the management account.
         self.master_account_name = master_account_name
+        # The status of the member deletion feature. Valid values:
+        # 
+        # *   Enabled: The feature is enabled. You can call the [DeleteAccount](~~311546~~) operation to delete members of the resource account type.
+        # *   Disabled: The feature is disabled. You cannot delete members of the resource account type.
         self.member_deletion_status = member_deletion_status
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The ID of the Root folder.
         self.root_folder_id = root_folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6762,15 +7429,17 @@
 
 class GetResourceDirectoryResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_directory: GetResourceDirectoryResponseBodyResourceDirectory = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
+        # The information of the resource directory.
         self.resource_directory = resource_directory
 
     def validate(self):
         if self.resource_directory:
             self.resource_directory.validate()
 
     def to_map(self):
@@ -6841,15 +7510,20 @@
 
 class GetResourceGroupRequest(TeaModel):
     def __init__(
         self,
         include_tags: bool = None,
         resource_group_id: str = None,
     ):
+        # The ID of the request.
         self.include_tags = include_tags
+        # Specifies whether to return the information of tags. Valid values:
+        # 
+        # *   false (default value)
+        # *   true
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6874,15 +7548,17 @@
 
 class GetResourceGroupResponseBodyResourceGroupRegionStatusesRegionStatus(TeaModel):
     def __init__(
         self,
         region_id: str = None,
         status: str = None,
     ):
+        # The ID of the Alibaba Cloud account to which the resource group belongs.
         self.region_id = region_id
+        # The region ID.
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6942,14 +7618,15 @@
 
 class GetResourceGroupResponseBodyResourceGroupTagsTag(TeaModel):
     def __init__(
         self,
         tag_key: str = None,
         tag_value: str = None,
     ):
+        # The tag value.
         self.tag_key = tag_key
         self.tag_value = tag_value
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -7016,21 +7693,38 @@
         display_name: str = None,
         id: str = None,
         name: str = None,
         region_statuses: GetResourceGroupResponseBodyResourceGroupRegionStatuses = None,
         status: str = None,
         tags: GetResourceGroupResponseBodyResourceGroupTags = None,
     ):
+        # The identifier of the resource group.
         self.account_id = account_id
+        # The ID of the resource group.
         self.create_date = create_date
+        # The status of the resource group. Valid values:
+        # 
+        # *   Creating: The resource group is being created.
+        # *   OK: The resource group is created.
+        # *   PendingDelete: The resource group is waiting to be deleted.
         self.display_name = display_name
+        # The tags that are added to the resource group.
         self.id = id
+        # The time when the resource group was created. The time is displayed in UTC.
         self.name = name
+        # The status of the resource group. Valid values:
+        # 
+        # *   Creating: The resource group is being created.
+        # *   OK: The resource group is created.
+        # *   PendingDelete: The resource group is waiting to be deleted.
+        # *   Deleting: The resource group is being deleted.
         self.region_statuses = region_statuses
+        # The status of the resource group in all regions.
         self.status = status
+        # The tag key.
         self.tags = tags
 
     def validate(self):
         if self.region_statuses:
             self.region_statuses.validate()
         if self.tags:
             self.tags.validate()
@@ -7084,15 +7778,17 @@
 
 class GetResourceGroupResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_group: GetResourceGroupResponseBodyResourceGroup = None,
     ):
+        # The information of the resource group.
         self.request_id = request_id
+        # The display name of the resource group.
         self.resource_group = resource_group
 
     def validate(self):
         if self.resource_group:
             self.resource_group.validate()
 
     def to_map(self):
@@ -7157,98 +7853,29 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetResourceGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetResourceGroupListAclModeResponseBody(TeaModel):
-    def __init__(
-        self,
-        mode: str = None,
-        request_id: str = None,
-    ):
-        self.mode = mode
-        self.request_id = request_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.mode is not None:
-            result['Mode'] = self.mode
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('Mode') is not None:
-            self.mode = m.get('Mode')
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        return self
-
-
-class GetResourceGroupListAclModeResponse(TeaModel):
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: GetResourceGroupListAclModeResponseBody = None,
-    ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = GetResourceGroupListAclModeResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class GetRoleRequest(TeaModel):
     def __init__(
         self,
         language: str = None,
         role_name: str = None,
     ):
+        # The language that is used to return the description of the RAM role. Valid values:
+        # 
+        # *   en: English
+        # *   zh-CN: Chinese
+        # *   ja: Japanese
         self.language = language
+        # The name of the RAM role.
+        # 
+        # The name must be 1 to 64 characters in length and can contain letters, digits, periods (.), and hyphens (-).
         self.role_name = role_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7273,15 +7900,17 @@
 
 class GetRoleResponseBodyRoleLatestDeletionTask(TeaModel):
     def __init__(
         self,
         create_date: str = None,
         deletion_task_id: str = None,
     ):
+        # The time when the deletion task was created.
         self.create_date = create_date
+        # The ID of the deletion task.
         self.deletion_task_id = deletion_task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7315,24 +7944,35 @@
         latest_deletion_task: GetRoleResponseBodyRoleLatestDeletionTask = None,
         max_session_duration: int = None,
         role_id: str = None,
         role_name: str = None,
         role_principal_name: str = None,
         update_date: str = None,
     ):
+        # The Alibaba Cloud Resource Name (ARN) of the RAM role.
         self.arn = arn
+        # The document of the policy that specifies the trusted entity to assume the RAM role.
         self.assume_role_policy_document = assume_role_policy_document
+        # The time when the RAM role was created.
         self.create_date = create_date
+        # The description of the RAM role.
         self.description = description
+        # Indicates whether the RAM role is a service linked role.
         self.is_service_linked_role = is_service_linked_role
+        # The information of the most recent deletion task.
         self.latest_deletion_task = latest_deletion_task
+        # The maximum session duration of the RAM role.
         self.max_session_duration = max_session_duration
+        # The ID of the RAM role.
         self.role_id = role_id
+        # The name of the RAM role.
         self.role_name = role_name
+        # The name of the RAM role after authorization.
         self.role_principal_name = role_principal_name
+        # The time when the RAM role was updated.
         self.update_date = update_date
 
     def validate(self):
         if self.latest_deletion_task:
             self.latest_deletion_task.validate()
 
     def to_map(self):
@@ -7395,15 +8035,17 @@
 
 class GetRoleResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         role: GetRoleResponseBodyRole = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
+        # The information of the RAM role.
         self.role = role
 
     def validate(self):
         if self.role:
             self.role.validate()
 
     def to_map(self):
@@ -7473,14 +8115,15 @@
 
 
 class GetServiceLinkedRoleDeletionStatusRequest(TeaModel):
     def __init__(
         self,
         deletion_task_id: str = None,
     ):
+        # The ID of the deletion task.
         self.deletion_task_id = deletion_task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7528,15 +8171,17 @@
 
 class GetServiceLinkedRoleDeletionStatusResponseBodyReasonRoleUsagesRoleUsage(TeaModel):
     def __init__(
         self,
         region: str = None,
         resources: GetServiceLinkedRoleDeletionStatusResponseBodyReasonRoleUsagesRoleUsageResources = None,
     ):
+        # The IDs of the regions in which the resources are to be queried.
         self.region = region
+        # The returned resources.
         self.resources = resources
 
     def validate(self):
         if self.resources:
             self.resources.validate()
 
     def to_map(self):
@@ -7598,15 +8243,17 @@
 
 class GetServiceLinkedRoleDeletionStatusResponseBodyReason(TeaModel):
     def __init__(
         self,
         message: str = None,
         role_usages: GetServiceLinkedRoleDeletionStatusResponseBodyReasonRoleUsages = None,
     ):
+        # Failure information.
         self.message = message
+        # Use resource information of the service linked role.
         self.role_usages = role_usages
 
     def validate(self):
         if self.role_usages:
             self.role_usages.validate()
 
     def to_map(self):
@@ -7634,16 +8281,25 @@
 class GetServiceLinkedRoleDeletionStatusResponseBody(TeaModel):
     def __init__(
         self,
         reason: GetServiceLinkedRoleDeletionStatusResponseBodyReason = None,
         request_id: str = None,
         status: str = None,
     ):
+        # The reason why the deletion task failed.
         self.reason = reason
+        # The ID of the request.
         self.request_id = request_id
+        # The status of the task.
+        # 
+        # - SUCCEEDED
+        # - IN_PROGRESS
+        # - FAILED
+        # - NOT_STARTED
+        # - INTERNAL_ERROR
         self.status = status
 
     def validate(self):
         if self.reason:
             self.reason.validate()
 
     def to_map(self):
@@ -7721,18 +8377,23 @@
         self,
         create_time: str = None,
         master_account_id: str = None,
         master_account_name: str = None,
         resource_directory_id: str = None,
         root_folder_id: str = None,
     ):
+        # The time when the resource directory was enabled.
         self.create_time = create_time
+        # The ID of the enterprise management account.
         self.master_account_id = master_account_id
+        # The name of the enterprise management account.
         self.master_account_name = master_account_name
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The ID of the root folder.
         self.root_folder_id = root_folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7769,15 +8430,17 @@
 
 class InitResourceDirectoryResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_directory: InitResourceDirectoryResponseBodyResourceDirectory = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
+        # The information of the resource directory.
         self.resource_directory = resource_directory
 
     def validate(self):
         if self.resource_directory:
             self.resource_directory.validate()
 
     def to_map(self):
@@ -7848,15 +8511,17 @@
 
 class InviteAccountToResourceDirectoryRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
+        # A tag key.
         self.key = key
+        # A tag value.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7883,17 +8548,25 @@
     def __init__(
         self,
         note: str = None,
         tag: List[InviteAccountToResourceDirectoryRequestTag] = None,
         target_entity: str = None,
         target_type: str = None,
     ):
+        # The comment on the invitation.
+        # 
+        # The comment can be up to 1,024 characters in length.
         self.note = note
         self.tag = tag
+        # The ID or logon email address of the account that you want to invite.
         self.target_entity = target_entity
+        # The type of the account. Valid values:
+        # 
+        # *   Account: indicates the ID of the account.
+        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -7943,24 +8616,44 @@
         modify_time: str = None,
         note: str = None,
         resource_directory_id: str = None,
         status: str = None,
         target_entity: str = None,
         target_type: str = None,
     ):
+        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time
+        # The time when the invitation expires. The time is displayed in UTC.
         self.expire_time = expire_time
+        # The ID of the invitation.
         self.handshake_id = handshake_id
+        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id
+        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name
+        # The time when the invitation was modified. The time is displayed in UTC.
         self.modify_time = modify_time
+        # The comment on the invitation.
         self.note = note
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the invitation.
+        # 
+        # *   Pending: The invitation is waiting for confirmation.
+        # *   Accepted: The invitation is accepted.
+        # *   Cancelled: The invitation is canceled.
+        # *   Declined: The invitation is rejected.
+        # *   Expired: The invitation expires.
         self.status = status
+        # The ID or logon email address of the invited account.
         self.target_entity = target_entity
+        # The type of the invited account. Valid values:
+        # 
+        # *   Account: indicates the ID of the account.
+        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8021,15 +8714,17 @@
 
 class InviteAccountToResourceDirectoryResponseBody(TeaModel):
     def __init__(
         self,
         handshake: InviteAccountToResourceDirectoryResponseBodyHandshake = None,
         request_id: str = None,
     ):
+        # The information of the invitation.
         self.handshake = handshake
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -8100,15 +8795,17 @@
 
 class ListAccountsRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
+        # A tag key.
         self.key = key
+        # A tag value.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8135,16 +8832,26 @@
     def __init__(
         self,
         include_tags: bool = None,
         page_number: int = None,
         page_size: int = None,
         tag: List[ListAccountsRequestTag] = None,
     ):
+        # Specifies whether to return the information of tags. Valid values:
+        # 
+        # *   false (default value)
+        # *   true
         self.include_tags = include_tags
+        # The number of the page to return.
+        # 
+        # Pages start from page 1. Default value: 1.
         self.page_number = page_number
+        # The number of entries to return on each page.
+        # 
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
@@ -8186,15 +8893,17 @@
 
 class ListAccountsResponseBodyAccountsAccountTagsTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
+        # A tag key.
         self.key = key
+        # A tag value.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8263,24 +8972,49 @@
         modify_time: str = None,
         resource_directory_id: str = None,
         resource_directory_path: str = None,
         status: str = None,
         tags: ListAccountsResponseBodyAccountsAccountTags = None,
         type: str = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
+        # The display name of the member.
         self.display_name = display_name
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The way in which the member joins the resource directory. Valid values:
+        # 
+        # *   invited: The member is invited to join the resource directory.
+        # *   created: The member is directly created in the resource directory.
         self.join_method = join_method
+        # The time when the member joined the resource directory. The time is displayed in UTC.
         self.join_time = join_time
+        # The time when the member was modified. The time is displayed in UTC.
         self.modify_time = modify_time
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The path of the member in the resource directory.
         self.resource_directory_path = resource_directory_path
+        # The status of the member. Valid values:
+        # 
+        # *   CreateSuccess: The member is created.
+        # *   PromoteVerifying: The upgrade of the member is being confirmed.
+        # *   PromoteFailed: The upgrade of the member fails.
+        # *   PromoteExpired: The upgrade of the member expires.
+        # *   PromoteCancelled: The upgrade of the member is canceled.
+        # *   PromoteSuccess: The member is upgraded.
+        # *   InviteSuccess: The member accepts the invitation.
         self.status = status
+        # The tags that are added to the member.
         self.tags = tags
+        # The type of the member. Valid values:
+        # 
+        # *   CloudAccount: cloud account
+        # *   ResourceAccount: resource account
         self.type = type
 
     def validate(self):
         if self.tags:
             self.tags.validate()
 
     def to_map(self):
@@ -8381,18 +9115,23 @@
         self,
         accounts: ListAccountsResponseBodyAccounts = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The members returned.
         self.accounts = accounts
+        # The page number of the returned page.
         self.page_number = page_number
+        # The number of entries returned per page.
         self.page_size = page_size
+        # The ID of the request.
         self.request_id = request_id
+        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.accounts:
             self.accounts.validate()
 
     def to_map(self):
@@ -8475,15 +9214,17 @@
 
 class ListAccountsForParentRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
+        # A tag key.
         self.key = key
+        # A tag value.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8512,18 +9253,33 @@
         include_tags: bool = None,
         page_number: int = None,
         page_size: int = None,
         parent_folder_id: str = None,
         query_keyword: str = None,
         tag: List[ListAccountsForParentRequestTag] = None,
     ):
+        # Specifies whether to return the information of tags. Valid values:
+        # 
+        # false (default value)
+        # 
+        # true
         self.include_tags = include_tags
+        # The number of the page to return.
+        # 
+        # Pages start from page 1. Default value: 1.
         self.page_number = page_number
+        # The number of entries to return on each page.
+        # 
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
+        # The ID of the folder.
         self.parent_folder_id = parent_folder_id
+        # The keyword used for the query, such as the display name of a member.
+        # 
+        # Fuzzy match is supported.
         self.query_keyword = query_keyword
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
@@ -8573,15 +9329,17 @@
 
 class ListAccountsForParentResponseBodyAccountsAccountTagsTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
+        # A tag key.
         self.key = key
+        # A tag value.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8649,23 +9407,47 @@
         join_time: str = None,
         modify_time: str = None,
         resource_directory_id: str = None,
         status: str = None,
         tags: ListAccountsForParentResponseBodyAccountsAccountTags = None,
         type: str = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
+        # The display name of the member.
         self.display_name = display_name
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The way in which the member joins the resource directory.
+        # 
+        # *   invited: The member is invited to join the resource directory.
+        # *   created: The member is directly created in the resource directory.
         self.join_method = join_method
+        # The time when the member joined the resource directory. The time is displayed in UTC.
         self.join_time = join_time
+        # The time when the member was modified. The time is displayed in UTC.
         self.modify_time = modify_time
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the member. Valid values:
+        # 
+        # *   CreateSuccess: The member is created.
+        # *   PromoteVerifying: The upgrade of the member is being confirmed.
+        # *   PromoteFailed: The upgrade of the member fails.
+        # *   PromoteExpired: The upgrade of the member expires.
+        # *   PromoteCancelled: The upgrade of the member is canceled.
+        # *   PromoteSuccess: The member is upgraded.
+        # *   InviteSuccess: The member accepts the invitation.
         self.status = status
+        # The tags that are added to the member.
         self.tags = tags
+        # The type of the member.
+        # 
+        # *   CloudAccount: cloud account
+        # *   ResourceAccount: resource account
         self.type = type
 
     def validate(self):
         if self.tags:
             self.tags.validate()
 
     def to_map(self):
@@ -8762,18 +9544,23 @@
         self,
         accounts: ListAccountsForParentResponseBodyAccounts = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The information of the members.
         self.accounts = accounts
+        # The page number of the returned page.
         self.page_number = page_number
+        # The number of entries returned per page.
         self.page_size = page_size
+        # The ID of the request.
         self.request_id = request_id
+        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.accounts:
             self.accounts.validate()
 
     def to_map(self):
@@ -8855,14 +9642,15 @@
 
 
 class ListAncestorsRequest(TeaModel):
     def __init__(
         self,
         child_id: str = None,
     ):
+        # The ID of the child folder.
         self.child_id = child_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8884,16 +9672,19 @@
 class ListAncestorsResponseBodyFoldersFolder(TeaModel):
     def __init__(
         self,
         create_time: str = None,
         folder_id: str = None,
         folder_name: str = None,
     ):
+        # The time when the folder was created.
         self.create_time = create_time
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The name of the folder.
         self.folder_name = folder_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8957,15 +9748,17 @@
 
 class ListAncestorsResponseBody(TeaModel):
     def __init__(
         self,
         folders: ListAncestorsResponseBodyFolders = None,
         request_id: str = None,
     ):
+        # The information of the folders.
         self.folders = folders
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.folders:
             self.folders.validate()
 
     def to_map(self):
@@ -9038,17 +9831,34 @@
     def __init__(
         self,
         language: str = None,
         page_number: int = None,
         page_size: int = None,
         policy_type: str = None,
     ):
+        # The language in which you want to return the descriptions of the access control policies. Valid values:
+        # 
+        # - zh-CN (default value): Chinese
+        # - en: English
+        # - ja: Japanese
+        # 
+        # >  This parameter is valid only for system access control policies.
         self.language = language
+        # The number of the page to return. 
+        # 
+        # Page start from page 1. Default value: 1.
         self.page_number = page_number
+        # The number of entries to return on each page. 
+        # 
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
+        # The type of the access control policy. Valid values:
+        # 
+        # - System: system access control policy
+        # - Custom: custom access control policy
         self.policy_type = policy_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9087,21 +9897,35 @@
         description: str = None,
         effect_scope: str = None,
         policy_id: str = None,
         policy_name: str = None,
         policy_type: str = None,
         update_date: str = None,
     ):
+        # The number of times that the access control policy is referenced.
         self.attachment_count = attachment_count
+        # The time when the access control policy was created.
         self.create_date = create_date
+        # The description of the access control policy.
         self.description = description
+        # The effective scope of the access control policy. Valid values:
+        # 
+        # - All: The access control policy is in effect for Alibaba Cloud accounts, RAM users, and RAM roles.
+        # - RAM: The access control policy is in effect only for RAM users and RAM roles.
         self.effect_scope = effect_scope
+        # The ID of the access control policy.
         self.policy_id = policy_id
+        # The name of the access control policy.
         self.policy_name = policy_name
+        # The type of the access control policy. Valid values:
+        # 
+        # - System: system access control policy
+        # - Custom: custom access control policy
         self.policy_type = policy_type
+        # The time when the access control policy was updated.
         self.update_date = update_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9188,18 +10012,23 @@
         self,
         control_policies: ListControlPoliciesResponseBodyControlPolicies = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The access control policies.
         self.control_policies = control_policies
+        # The number of the returned page.
         self.page_number = page_number
+        # The number of entries returned per page.
         self.page_size = page_size
+        # The ID of the request.
         self.request_id = request_id
+        # The number of access control policies.
         self.total_count = total_count
 
     def validate(self):
         if self.control_policies:
             self.control_policies.validate()
 
     def to_map(self):
@@ -9282,15 +10111,27 @@
 
 class ListControlPolicyAttachmentsForTargetRequest(TeaModel):
     def __init__(
         self,
         language: str = None,
         target_id: str = None,
     ):
+        # The language in which you want to return the descriptions of the access control policies. Valid values:
+        # 
+        # *   zh-CN (default value): Chinese
+        # *   en: English
+        # *   ja: Japanese
+        # 
+        # >  This parameter is valid only for system access control policies.
         self.language = language
+        # The ID of the object whose access control policies you want to query. Access control policies can be attached to the following objects:
+        # 
+        # *   Root folder
+        # *   Subfolders of the Root folder
+        # *   Members
         self.target_id = target_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9319,19 +10160,31 @@
         attach_date: str = None,
         description: str = None,
         effect_scope: str = None,
         policy_id: str = None,
         policy_name: str = None,
         policy_type: str = None,
     ):
+        # The time when the access control policy was attached.
         self.attach_date = attach_date
+        # The description of the access control policy.
         self.description = description
+        # The effective scope of the access control policy. Valid values:
+        # 
+        # *   All: The access control policy is in effect for Alibaba Cloud accounts, RAM users, and RAM roles.
+        # *   RAM: The access control policy is in effect only for RAM users and RAM roles.
         self.effect_scope = effect_scope
+        # The ID of the access control policy.
         self.policy_id = policy_id
+        # The name of the access control policy.
         self.policy_name = policy_name
+        # The type of the access control policy. Valid values:
+        # 
+        # *   System: system access control policy
+        # *   Custom: custom access control policy
         self.policy_type = policy_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9407,15 +10260,17 @@
 
 class ListControlPolicyAttachmentsForTargetResponseBody(TeaModel):
     def __init__(
         self,
         control_policy_attachments: ListControlPolicyAttachmentsForTargetResponseBodyControlPolicyAttachments = None,
         request_id: str = None,
     ):
+        # The attached access control policies.
         self.control_policy_attachments = control_policy_attachments
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.control_policy_attachments:
             self.control_policy_attachments.validate()
 
     def to_map(self):
@@ -9487,16 +10342,25 @@
 class ListDelegatedAdministratorsRequest(TeaModel):
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
         service_principal: str = None,
     ):
+        # The number of the page to return.
+        # 
+        # Pages start from page 1. Default value: 1.
         self.page_number = page_number
+        # The number of entries to return on each page.
+        # 
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
+        # The identifier of the trusted service.
+        # 
+        # For more information, see the `Trusted service identifier` column in [Supported trusted services](~~208133~~).
         self.service_principal = service_principal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9528,18 +10392,26 @@
         self,
         account_id: str = None,
         delegation_enabled_time: str = None,
         display_name: str = None,
         join_method: str = None,
         service_principal: str = None,
     ):
+        # The ID of the member.
         self.account_id = account_id
+        # The time when the member was specified as a delegated administrator account.
         self.delegation_enabled_time = delegation_enabled_time
+        # The display name of the member.
         self.display_name = display_name
+        # The way in which the member joins the resource directory. Valid values:
+        # 
+        # *   invited: The member is invited to join the resource directory.
+        # *   created: The member is directly created in the resource directory.
         self.join_method = join_method
+        # The identifier of the trusted service.
         self.service_principal = service_principal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9614,18 +10486,23 @@
         self,
         accounts: ListDelegatedAdministratorsResponseBodyAccounts = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The information of the delegated administrator accounts.
         self.accounts = accounts
+        # The page number of the returned page.
         self.page_number = page_number
+        # The number of entries returned per page.
         self.page_size = page_size
+        # The ID of the request.
         self.request_id = request_id
+        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.accounts:
             self.accounts.validate()
 
     def to_map(self):
@@ -9707,14 +10584,15 @@
 
 
 class ListDelegatedServicesForAccountRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
     ):
+        # The ID of the member.
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9736,16 +10614,22 @@
 class ListDelegatedServicesForAccountResponseBodyDelegatedServicesDelegatedService(TeaModel):
     def __init__(
         self,
         delegation_enabled_time: str = None,
         service_principal: str = None,
         status: str = None,
     ):
+        # The time when the member was specified as a delegated administrator account of the trusted service.
         self.delegation_enabled_time = delegation_enabled_time
+        # The identification of the trusted service.
         self.service_principal = service_principal
+        # The status of the trusted service. Valid values:
+        # 
+        # *   ENABLED: enabled
+        # *   DISABLED: disabled
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9809,15 +10693,19 @@
 
 class ListDelegatedServicesForAccountResponseBody(TeaModel):
     def __init__(
         self,
         delegated_services: ListDelegatedServicesForAccountResponseBodyDelegatedServices = None,
         request_id: str = None,
     ):
+        # The trusted services.
+        # 
+        # >  If the value of this parameter is empty, the member is not specified as a delegated administrator account.
         self.delegated_services = delegated_services
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.delegated_services:
             self.delegated_services.validate()
 
     def to_map(self):
@@ -9890,17 +10778,29 @@
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
         parent_folder_id: str = None,
         query_keyword: str = None,
     ):
+        # The number of the page to return.
+        # 
+        # Pages start from page 1. Default value: 1.
         self.page_number = page_number
+        # The number of entries to return on each page.
+        # 
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
+        # The ID of the parent folder.
+        # 
+        # If you leave this parameter empty, the information of the first-level subfolders of the Root folder is queried.
         self.parent_folder_id = parent_folder_id
+        # The keyword used for the query, such as a folder name.
+        # 
+        # Fuzzy match is supported.
         self.query_keyword = query_keyword
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9934,16 +10834,19 @@
 class ListFoldersForParentResponseBodyFoldersFolder(TeaModel):
     def __init__(
         self,
         create_time: str = None,
         folder_id: str = None,
         folder_name: str = None,
     ):
+        # The time when the folder was created.
         self.create_time = create_time
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The name of the folder.
         self.folder_name = folder_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10010,18 +10913,23 @@
         self,
         folders: ListFoldersForParentResponseBodyFolders = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The information of the folders.
         self.folders = folders
+        # The page number of the returned page.
         self.page_number = page_number
+        # The number of entries returned per page.
         self.page_size = page_size
+        # The ID of the request.
         self.request_id = request_id
+        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.folders:
             self.folders.validate()
 
     def to_map(self):
@@ -10104,15 +11012,21 @@
 
 class ListHandshakesForAccountRequest(TeaModel):
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
     ):
+        # The number of the page to return.
+        # 
+        # Pages start from page 1. Default value: 1.
         self.page_number = page_number
+        # The number of entries to return on each page.
+        # 
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10146,24 +11060,44 @@
         modify_time: str = None,
         note: str = None,
         resource_directory_id: str = None,
         status: str = None,
         target_entity: str = None,
         target_type: str = None,
     ):
+        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time
+        # The time when the invitation expires. The time is displayed in UTC.
         self.expire_time = expire_time
+        # The ID of the invitation.
         self.handshake_id = handshake_id
+        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id
+        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name
+        # The time when the invitation was modified. The time is displayed in UTC.
         self.modify_time = modify_time
+        # The comment on the invitation.
         self.note = note
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending: The invitation is waiting for confirmation.
+        # *   Accepted: The invitation is accepted.
+        # *   Cancelled: The invitation is canceled.
+        # *   Declined: The invitation is rejected.
+        # *   Expired: The invitation expires.
         self.status = status
+        # The ID or logon email address of the invited Alibaba Cloud account.
         self.target_entity = target_entity
+        # The type of the invited Alibaba Cloud account. Valid values:
+        # 
+        # *   Account: indicates the ID of the account.
+        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10262,18 +11196,23 @@
         self,
         handshakes: ListHandshakesForAccountResponseBodyHandshakes = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The information of the invitations.
         self.handshakes = handshakes
+        # The page number of the returned page.
         self.page_number = page_number
+        # The number of entries returned per page.
         self.page_size = page_size
+        # The ID of the request.
         self.request_id = request_id
+        # The total number of invitations.
         self.total_count = total_count
 
     def validate(self):
         if self.handshakes:
             self.handshakes.validate()
 
     def to_map(self):
@@ -10356,15 +11295,21 @@
 
 class ListHandshakesForResourceDirectoryRequest(TeaModel):
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
     ):
+        # The number of the page to return.
+        # 
+        # Pages start from page 1. Default value: 1.
         self.page_number = page_number
+        # The number of entries to return on each page.
+        # 
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10398,24 +11343,44 @@
         modify_time: str = None,
         note: str = None,
         resource_directory_id: str = None,
         status: str = None,
         target_entity: str = None,
         target_type: str = None,
     ):
+        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time
+        # The time when the invitation expires. The time is displayed in UTC.
         self.expire_time = expire_time
+        # The ID of the invitation.
         self.handshake_id = handshake_id
+        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id
+        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name
+        # The time when the invitation was modified. The time is displayed in UTC.
         self.modify_time = modify_time
+        # The comment on the invitation.
         self.note = note
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending: The invitation is waiting for confirmation.
+        # *   Accepted: The invitation is accepted.
+        # *   Cancelled: The invitation is canceled.
+        # *   Declined: The invitation is rejected.
+        # *   Expired: The invitation expires.
         self.status = status
+        # The ID or logon email address of the invited account.
         self.target_entity = target_entity
+        # The type of the invited account. Valid values:
+        # 
+        # *   Account: indicates the ID of the account.
+        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10514,18 +11479,23 @@
         self,
         handshakes: ListHandshakesForResourceDirectoryResponseBodyHandshakes = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The information of the invitations.
         self.handshakes = handshakes
+        # The page number of the returned page.
         self.page_number = page_number
+        # The number of entries returned per page.
         self.page_size = page_size
+        # The ID of the request.
         self.request_id = request_id
+        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.handshakes:
             self.handshakes.validate()
 
     def to_map(self):
@@ -10610,17 +11580,32 @@
     def __init__(
         self,
         language: str = None,
         page_number: int = None,
         page_size: int = None,
         policy_type: str = None,
     ):
+        # The language that is used to return the description of the system policy. Valid values:
+        # 
+        # *   en: English
+        # *   zh-CN: Chinese
+        # *   ja: Japanese
         self.language = language
+        # The number of the page to return.
+        # 
+        # Pages start from page 1. Default value: 1.
         self.page_number = page_number
+        # The number of entries to return on each page.
+        # 
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
+        # The type of the policy. If you do not specify this parameter, the system lists all types of policies. Valid values:
+        # 
+        # *   Custom: custom policy
+        # *   System: system policy
         self.policy_type = policy_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10658,20 +11643,30 @@
         create_date: str = None,
         default_version: str = None,
         description: str = None,
         policy_name: str = None,
         policy_type: str = None,
         update_date: str = None,
     ):
+        # The number of times the policy is referenced.
         self.attachment_count = attachment_count
+        # The time when the policy was created.
         self.create_date = create_date
+        # The default version of the policy.
         self.default_version = default_version
+        # The description of the policy.
         self.description = description
+        # The name of the policy.
         self.policy_name = policy_name
+        # The type of the policy. Valid values:
+        # 
+        # *   Custom: custom policy
+        # *   System: system policy
         self.policy_type = policy_type
+        # The time when the policy was updated.
         self.update_date = update_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10754,18 +11749,23 @@
         self,
         page_number: int = None,
         page_size: int = None,
         policies: ListPoliciesResponseBodyPolicies = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The page number of the returned page.
         self.page_number = page_number
+        # The number of entries returned per page.
         self.page_size = page_size
+        # The information of the policies.
         self.policies = policies
+        # The ID of the request.
         self.request_id = request_id
+        # The total number of returned entries.
         self.total_count = total_count
 
     def validate(self):
         if self.policies:
             self.policies.validate()
 
     def to_map(self):
@@ -10854,21 +11854,46 @@
         page_size: int = None,
         policy_name: str = None,
         policy_type: str = None,
         principal_name: str = None,
         principal_type: str = None,
         resource_group_id: str = None,
     ):
+        # The language that is used to return the description of the system policy. Valid values:
+        # 
+        # *   en: English
+        # *   zh-CN: Chinese
+        # *   ja: Japanese
         self.language = language
+        # The number of the page to return.
+        # 
+        # Pages start from page 1. Default value: 1.
         self.page_number = page_number
+        # The number of entries to return on each page.
+        # 
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
+        # The name of the policy.
+        # 
+        # The name must be 1 to 128 characters in length and can contain letters, digits, and hyphens (-).
         self.policy_name = policy_name
+        # The type of the policy. If you do not specify this parameter, the system lists all types of policies. Valid values:
+        # 
+        # *   Custom: custom policy
+        # *   System: system policy
         self.policy_type = policy_type
+        # The name of the object to which the policy is attached.
         self.principal_name = principal_name
+        # The type of the object to which the policy is attached. If you do not specify this parameter, the system lists all types of objects. Valid values:
+        # 
+        # *   IMSUser: RAM user
+        # *   IMSGroup: RAM user group
+        # *   ServiceRole: RAM role
         self.principal_type = principal_type
+        # The ID of the resource group or the ID of the Alibaba Cloud account to which the resource group belongs. If you do not specify this parameter, the system lists all policy attachment records under the current account.
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10922,20 +11947,34 @@
         description: str = None,
         policy_name: str = None,
         policy_type: str = None,
         principal_name: str = None,
         principal_type: str = None,
         resource_group_id: str = None,
     ):
+        # The time when the policy was attached.
         self.attach_date = attach_date
+        # The description of the policy.
         self.description = description
+        # The name of the policy.
         self.policy_name = policy_name
+        # The type of the policy. Valid values:
+        # 
+        # *   Custom: custom policy
+        # *   System: system policy
         self.policy_type = policy_type
+        # The name of the object to which the policy is attached.
         self.principal_name = principal_name
+        # The type of the object to which the policy is attached. Valid values:
+        # 
+        # *   IMSUser: RAM user
+        # *   IMSGroup: RAM user group
+        # *   ServiceRole: RAM role
         self.principal_type = principal_type
+        # The ID of the resource group or the ID of the Alibaba Cloud account to which the resource group belongs.
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11018,18 +12057,23 @@
         self,
         page_number: int = None,
         page_size: int = None,
         policy_attachments: ListPolicyAttachmentsResponseBodyPolicyAttachments = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The page number of the returned page.
         self.page_number = page_number
+        # The number of entries returned per page.
         self.page_size = page_size
+        # The policy attachment records.
         self.policy_attachments = policy_attachments
+        # The ID of the request.
         self.request_id = request_id
+        # The total number of returned entries.
         self.total_count = total_count
 
     def validate(self):
         if self.policy_attachments:
             self.policy_attachments.validate()
 
     def to_map(self):
@@ -11112,15 +12156,22 @@
 
 class ListPolicyVersionsRequest(TeaModel):
     def __init__(
         self,
         policy_name: str = None,
         policy_type: str = None,
     ):
+        # The name of the policy.
+        # 
+        # The name must be 1 to 128 characters in length and can contain letters, digits, and hyphens (-).
         self.policy_name = policy_name
+        # The type of the policy. Valid values:
+        # 
+        # *   Custom: custom policy
+        # *   System: system policy
         self.policy_type = policy_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11146,16 +12197,19 @@
 class ListPolicyVersionsResponseBodyPolicyVersionsPolicyVersion(TeaModel):
     def __init__(
         self,
         create_date: str = None,
         is_default_version: bool = None,
         version_id: str = None,
     ):
+        # The time when the policy version was created.
         self.create_date = create_date
+        # Indicates whether the policy version is the default version.
         self.is_default_version = is_default_version
+        # The ID of the policy version.
         self.version_id = version_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11219,15 +12273,17 @@
 
 class ListPolicyVersionsResponseBody(TeaModel):
     def __init__(
         self,
         policy_versions: ListPolicyVersionsResponseBodyPolicyVersions = None,
         request_id: str = None,
     ):
+        # The information of the policy versions.
         self.policy_versions = policy_versions
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.policy_versions:
             self.policy_versions.validate()
 
     def to_map(self):
@@ -11298,15 +12354,17 @@
 
 class ListResourceGroupsRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
+        # The tag key.
         self.key = key
+        # The tag value.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11338,22 +12396,56 @@
         page_number: int = None,
         page_size: int = None,
         resource_group_id: str = None,
         resource_group_ids: List[str] = None,
         status: str = None,
         tag: List[ListResourceGroupsRequestTag] = None,
     ):
+        # The display name of the resource group. This parameter specifies a filter condition for the query. Fuzzy match is supported.
+        # 
+        # The display name can be a maximum of 50 characters in length.
         self.display_name = display_name
+        # Specifies whether to return the information of tags. Valid values:
+        # 
+        # *   false (default value)
+        # *   true
+        # 
+        # >  If you configure the Tag parameter, the system returns the information of tags regardless of the setting of the `IncludeTags` parameter.
         self.include_tags = include_tags
+        # The identifier of the resource group. This parameter specifies a filter condition for the query. Fuzzy match is supported.
+        # 
+        # The identifier can be a maximum of 50 characters in length and can contain letters, digits, and hyphens (-).
         self.name = name
+        # The number of the page to return.
+        # 
+        # Pages start from page 1. Default value: 1.
         self.page_number = page_number
+        # The number of entries to return on each page.
+        # 
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
+        # The ID of the resource group. This parameter specifies a filter condition for the query.
+        # 
+        # The ID can be a maximum of 18 characters in length and must start with `rg-`.
+        # 
+        # >  This parameter is incorporated into the `ResourceGroupIds` parameter. If you configure both the `ResourceGroupId` and `ResourceGroupIds` parameters, the value of the `ResourceGroupIds` parameter prevails.
         self.resource_group_id = resource_group_id
+        # The IDs of the resource groups. This parameter specifies a filter condition for the query.
+        # 
+        # You can specify a maximum of 100 resource group IDs.
+        # 
+        # >  If you configure both the `ResourceGroupId` and `ResourceGroupIds` parameters, the value of the `ResourceGroupIds` parameter prevails.
         self.resource_group_ids = resource_group_ids
+        # The status of the resource group. This parameter specifies a filter condition for the query. Valid values:
+        # 
+        # *   Creating: The resource group is being created.
+        # *   OK: The resource group is created.
+        # *   PendingDelete: The resource group is waiting to be deleted.
         self.status = status
+        # The tag. This parameter specifies a filter condition for the query.
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -11414,15 +12506,17 @@
 
 class ListResourceGroupsResponseBodyResourceGroupsResourceGroupTagsTag(TeaModel):
     def __init__(
         self,
         tag_key: str = None,
         tag_value: str = None,
     ):
+        # The tag key.
         self.tag_key = tag_key
+        # The tag value.
         self.tag_value = tag_value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11487,20 +12581,31 @@
         create_date: str = None,
         display_name: str = None,
         id: str = None,
         name: str = None,
         status: str = None,
         tags: ListResourceGroupsResponseBodyResourceGroupsResourceGroupTags = None,
     ):
+        # The ID of the Alibaba Cloud account to which the resource group belongs.
         self.account_id = account_id
+        # The time when the resource group was created. The time is displayed in UTC.
         self.create_date = create_date
+        # The display name of the resource group.
         self.display_name = display_name
+        # The ID of the resource group.
         self.id = id
+        # The identifier of the resource group.
         self.name = name
+        # The status of the resource group. Valid values:
+        # 
+        # *   Creating: The resource group is being created.
+        # *   OK: The resource group is created.
+        # *   PendingDelete: The resource group is waiting to be deleted.
         self.status = status
+        # The tags that are added to the resource group.
         self.tags = tags
 
     def validate(self):
         if self.tags:
             self.tags.validate()
 
     def to_map(self):
@@ -11585,18 +12690,23 @@
         self,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         resource_groups: ListResourceGroupsResponseBodyResourceGroups = None,
         total_count: int = None,
     ):
+        # The page number of the returned page.
         self.page_number = page_number
+        # The number of entries returned per page.
         self.page_size = page_size
+        # The ID of the request.
         self.request_id = request_id
+        # The information of the resource groups.
         self.resource_groups = resource_groups
+        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.resource_groups:
             self.resource_groups.validate()
 
     def to_map(self):
@@ -11684,20 +12794,35 @@
         page_size: int = None,
         region: str = None,
         resource_group_id: str = None,
         resource_id: str = None,
         resource_type: str = None,
         service: str = None,
     ):
+        # The number of the page to return.
+        # 
+        # Pages start from page 1. Default value: 1.
         self.page_number = page_number
+        # The number of entries to return on each page.
+        # 
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
+        # The region ID.
         self.region = region
+        # The ID of the resource group.
         self.resource_group_id = resource_group_id
+        # The ID of the resource.
         self.resource_id = resource_id
+        # The resource type.
+        # 
+        # For more information about the supported resource types, see the **Resource type** column in [Alibaba Cloud services that support resource groups](~~94479~~).
         self.resource_type = resource_type
+        # The ID of the Alibaba Cloud service.
+        # 
+        # You can obtain the ID from the **Service code** column in [Alibaba Cloud services that support resource groups](~~94479~~).
         self.service = service
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11746,19 +12871,25 @@
         create_date: str = None,
         region_id: str = None,
         resource_group_id: str = None,
         resource_id: str = None,
         resource_type: str = None,
         service: str = None,
     ):
+        # The time when the resource was created. The time is displayed in UTC.
         self.create_date = create_date
+        # The region ID.
         self.region_id = region_id
+        # The ID of the resource group.
         self.resource_group_id = resource_group_id
+        # The ID of the resource.
         self.resource_id = resource_id
+        # The type of the resource.
         self.resource_type = resource_type
+        # The ID of the Alibaba Cloud service.
         self.service = service
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11837,18 +12968,23 @@
         self,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         resources: ListResourcesResponseBodyResources = None,
         total_count: int = None,
     ):
+        # The page number of the returned page.
         self.page_number = page_number
+        # The number of entries returned per page.
         self.page_size = page_size
+        # The ID of the request.
         self.request_id = request_id
+        # The information of the resources.
         self.resources = resources
+        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.resources:
             self.resources.validate()
 
     def to_map(self):
@@ -11932,16 +13068,27 @@
 class ListRolesRequest(TeaModel):
     def __init__(
         self,
         language: str = None,
         page_number: int = None,
         page_size: int = None,
     ):
+        # The language that is used to return the descriptions of the RAM roles. Valid values:
+        # 
+        # *   en: English
+        # *   zh-CN: Chinese
+        # *   ja: Japanese
         self.language = language
+        # The number of the page to return.
+        # 
+        # Pages start from page 1. Default value: 1.
         self.page_number = page_number
+        # The number of entries to return on each page.
+        # 
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11970,15 +13117,17 @@
 
 class ListRolesResponseBodyRolesRoleLatestDeletionTask(TeaModel):
     def __init__(
         self,
         create_date: str = None,
         deletion_task_id: str = None,
     ):
+        # The time when the deletion task was created.
         self.create_date = create_date
+        # The ID of the deletion task.
         self.deletion_task_id = deletion_task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12011,23 +13160,33 @@
         latest_deletion_task: ListRolesResponseBodyRolesRoleLatestDeletionTask = None,
         max_session_duration: int = None,
         role_id: str = None,
         role_name: str = None,
         role_principal_name: str = None,
         update_date: str = None,
     ):
+        # The Alibaba Cloud Resource Name (ARN) of the RAM role.
         self.arn = arn
+        # The time when the RAM role was created.
         self.create_date = create_date
+        # The description of the RAM role.
         self.description = description
+        # Indicates whether the RAM role is a service linked role.
         self.is_service_linked_role = is_service_linked_role
+        # The information of the most recent deletion task.
         self.latest_deletion_task = latest_deletion_task
+        # The maximum session duration of the RAM role.
         self.max_session_duration = max_session_duration
+        # The ID of the RAM role.
         self.role_id = role_id
+        # The name of the RAM role.
         self.role_name = role_name
+        # The name of the RAM role after authorization.
         self.role_principal_name = role_principal_name
+        # The time when the RAM role was updated.
         self.update_date = update_date
 
     def validate(self):
         if self.latest_deletion_task:
             self.latest_deletion_task.validate()
 
     def to_map(self):
@@ -12124,18 +13283,23 @@
         self,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         roles: ListRolesResponseBodyRoles = None,
         total_count: int = None,
     ):
+        # The page number of the returned page.
         self.page_number = page_number
+        # The number of entries returned per page.
         self.page_size = page_size
+        # The ID of the request.
         self.request_id = request_id
+        # The information of the RAM roles.
         self.roles = roles
+        # The total number of RAM roles.
         self.total_count = total_count
 
     def validate(self):
         if self.roles:
             self.roles.validate()
 
     def to_map(self):
@@ -12220,17 +13384,25 @@
     def __init__(
         self,
         key_filter: str = None,
         max_results: int = None,
         next_token: str = None,
         resource_type: str = None,
     ):
+        # The tag key for a fuzzy query.
         self.key_filter = key_filter
+        # The maximum number of entries to return for a single request.
+        # 
+        # Valid values: 1 to 100. Default value: 10.
         self.max_results = max_results
+        # The token that is used to start the next query.
         self.next_token = next_token
+        # The resource type.
+        # 
+        # The value Account indicates the members of the resource directory.
         self.resource_type = resource_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12262,14 +13434,15 @@
 
 
 class ListTagKeysResponseBodyTags(TeaModel):
     def __init__(
         self,
         key: str = None,
     ):
+        # The tag key.
         self.key = key
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12291,16 +13464,22 @@
 class ListTagKeysResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         request_id: str = None,
         tags: List[ListTagKeysResponseBodyTags] = None,
     ):
+        # Indicates whether the next query is required.
+        # 
+        # *   If the value of this parameter is empty (`"NextToken": ""`), all results are returned, and the next query is not required.
+        # *   If the value of this parameter is not empty, the next query is required, and the value is the token used to start the next query.
         self.next_token = next_token
+        # The ID of the request.
         self.request_id = request_id
+        # The information of the tag keys.
         self.tags = tags
 
     def validate(self):
         if self.tags:
             for k in self.tags:
                 if k:
                     k.validate()
@@ -12381,15 +13560,17 @@
 
 class ListTagResourcesRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
+        # A tag key.
         self.key = key
+        # A tag value.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12417,17 +13598,25 @@
         self,
         max_results: int = None,
         next_token: str = None,
         resource_id: List[str] = None,
         resource_type: str = None,
         tag: List[ListTagResourcesRequestTag] = None,
     ):
+        # The number of entries to return on each page.
+        # 
+        # Valid values: 1 to 100. Default value: 10.
         self.max_results = max_results
+        # The token that is used to start the next query.
         self.next_token = next_token
         self.resource_id = resource_id
+        # The type of the objects whose tags you want to query. This parameter specifies a filter condition for the query. Valid values:
+        # 
+        # *   ResourceGroup: resource group. This is the default value.
+        # *   Account: member.
         self.resource_type = resource_type
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
@@ -12475,17 +13664,24 @@
     def __init__(
         self,
         resource_id: str = None,
         resource_type: str = None,
         tag_key: str = None,
         tag_value: str = None,
     ):
+        # The ID of the resource group or member.
         self.resource_id = resource_id
+        # The type of the object whose tags are queried. Valid values:
+        # 
+        # *   resourcegroup: resource group
+        # *   Account: member
         self.resource_type = resource_type
+        # The tag key.
         self.tag_key = tag_key
+        # The tag value.
         self.tag_value = tag_value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12519,16 +13715,22 @@
 class ListTagResourcesResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         request_id: str = None,
         tag_resources: List[ListTagResourcesResponseBodyTagResources] = None,
     ):
+        # Indicates whether the next query is required.
+        # 
+        # *   If the value of this parameter is empty (`"NextToken": ""`), all results are returned, and the next query is not required.
+        # *   If the value of this parameter is not empty, the next query is required, and the value is the token used to start the next query.
         self.next_token = next_token
+        # The ID of the request.
         self.request_id = request_id
+        # The tags.
         self.tag_resources = tag_resources
 
     def validate(self):
         if self.tag_resources:
             for k in self.tag_resources:
                 if k:
                     k.validate()
@@ -12612,18 +13814,27 @@
         self,
         max_results: int = None,
         next_token: str = None,
         resource_type: str = None,
         tag_key: str = None,
         value_filter: str = None,
     ):
+        # The maximum number of entries to return for a single request.
+        # 
+        # Valid values: 1 to 100. Default value: 10.
         self.max_results = max_results
+        # The token that is used to start the next query.
         self.next_token = next_token
+        # The resource type.
+        # 
+        # The value Account indicates the members of the resource directory.
         self.resource_type = resource_type
+        # The tag key. This parameter specifies a filter condition for the query.
         self.tag_key = tag_key
+        # The tag value for a fuzzy query.
         self.value_filter = value_filter
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12659,14 +13870,15 @@
 
 
 class ListTagValuesResponseBodyTags(TeaModel):
     def __init__(
         self,
         value: str = None,
     ):
+        # The tag value.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12688,16 +13900,22 @@
 class ListTagValuesResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         request_id: str = None,
         tags: List[ListTagValuesResponseBodyTags] = None,
     ):
+        # Indicates whether the next query is required.
+        # 
+        # *   If the value of this parameter is empty (`"NextToken": ""`), all results are returned, and the next query is not required.
+        # *   If the value of this parameter is not empty, the next query is required, and the value is the token used to start the next query.
         self.next_token = next_token
+        # The ID of the request.
         self.request_id = request_id
+        # The information of the tag values.
         self.tags = tags
 
     def validate(self):
         if self.tags:
             for k in self.tags:
                 if k:
                     k.validate()
@@ -12779,16 +13997,23 @@
 class ListTargetAttachmentsForControlPolicyRequest(TeaModel):
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
         policy_id: str = None,
     ):
+        # The number of the page to return.
+        # 
+        # Pages start from page 1. Default value: 1.
         self.page_number = page_number
+        # The number of entries to return on each page.
+        # 
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
+        # The ID of the control policy.
         self.policy_id = policy_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12819,17 +14044,25 @@
     def __init__(
         self,
         attach_date: str = None,
         target_id: str = None,
         target_name: str = None,
         target_type: str = None,
     ):
+        # The time when the control policy was attached to the object.
         self.attach_date = attach_date
+        # The ID of the object.
         self.target_id = target_id
+        # The name of the object.
         self.target_name = target_name
+        # The type of the object. Valid values:
+        # 
+        # *   Root: Root folder
+        # *   Folder: child folder of the Root folder
+        # *   Account: member account
         self.target_type = target_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12900,18 +14133,23 @@
         self,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         target_attachments: ListTargetAttachmentsForControlPolicyResponseBodyTargetAttachments = None,
         total_count: int = None,
     ):
+        # The page number of the returned page.
         self.page_number = page_number
+        # The number of entries returned per page.
         self.page_size = page_size
+        # The ID of the request.
         self.request_id = request_id
+        # The list of objects to which the control policy is attached.
         self.target_attachments = target_attachments
+        # The total number of objects to which the control policy is attached.
         self.total_count = total_count
 
     def validate(self):
         if self.target_attachments:
             self.target_attachments.validate()
 
     def to_map(self):
@@ -12995,16 +14233,28 @@
 class ListTrustedServiceStatusRequest(TeaModel):
     def __init__(
         self,
         admin_account_id: str = None,
         page_number: int = None,
         page_size: int = None,
     ):
+        # The ID of the enterprise management account or delegated administrator account.
+        # 
+        # *   If you set this parameter to the ID of an enterprise management account, the trusted services that are enabled within the enterprise management account are queried. The default value of this parameter is the ID of an enterprise management account.
+        # *   If you set this parameter to the ID of a delegated administrator account, the trusted services that are enabled within the delegated administrator account are queried.
+        # 
+        # For more information about trusted services and delegated administrator accounts, see [Overview of trusted services](~~208133~~) and [Delegated administrator accounts](~~208117~~).
         self.admin_account_id = admin_account_id
+        # The number of the page to return.
+        # 
+        # Pages start from page 1. Default value: 1.
         self.page_number = page_number
+        # The number of entries to return on each page.
+        # 
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13033,15 +14283,17 @@
 
 class ListTrustedServiceStatusResponseBodyEnabledServicePrincipalsEnabledServicePrincipal(TeaModel):
     def __init__(
         self,
         enable_time: str = None,
         service_principal: str = None,
     ):
+        # The time when the trusted service was enabled.
         self.enable_time = enable_time
+        # The identification of the trusted service.
         self.service_principal = service_principal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13104,18 +14356,23 @@
         self,
         enabled_service_principals: ListTrustedServiceStatusResponseBodyEnabledServicePrincipals = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The trusted services that are enabled.
         self.enabled_service_principals = enabled_service_principals
+        # The page number of the returned page.
         self.page_number = page_number
+        # The number of entries returned per page.
         self.page_size = page_size
+        # The ID of the request.
         self.request_id = request_id
+        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.enabled_service_principals:
             self.enabled_service_principals.validate()
 
     def to_map(self):
@@ -13198,15 +14455,17 @@
 
 class MoveAccountRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         destination_folder_id: str = None,
     ):
+        # The ID of the account you want to move.
         self.account_id = account_id
+        # The ID of the destination folder.
         self.destination_folder_id = destination_folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13230,14 +14489,15 @@
 
 
 class MoveAccountResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13304,17 +14564,21 @@
     def __init__(
         self,
         region_id: str = None,
         resource_id: str = None,
         resource_type: str = None,
         service: str = None,
     ):
+        # The region ID of the resource.
         self.region_id = region_id
+        # The ID of the resource.
         self.resource_id = resource_id
+        # The type of the resource.
         self.resource_type = resource_type
+        # The ID of the Alibaba Cloud service to which the resource belongs.
         self.service = service
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13347,15 +14611,19 @@
 
 class MoveResourcesRequest(TeaModel):
     def __init__(
         self,
         resource_group_id: str = None,
         resources: List[MoveResourcesRequestResources] = None,
     ):
+        # The ID of the resource group to which you want to move the resources.
         self.resource_group_id = resource_group_id
+        # The resources that you want to move.
+        # 
+        # >  You can move a maximum of 10 resources at a time. If you want to move more than 10 resources, move them in batches.
         self.resources = resources
 
     def validate(self):
         if self.resources:
             for k in self.resources:
                 if k:
                     k.validate()
@@ -13394,21 +14662,36 @@
         region_id: str = None,
         request_id: str = None,
         resource_id: str = None,
         resource_type: str = None,
         service: str = None,
         status: str = None,
     ):
+        # The error code returned.
+        # 
+        # >  This parameter is returned if the resource failed to be moved.
         self.error_code = error_code
+        # The error message returned.
+        # 
+        # >  This parameter is returned if the resource failed to be moved.
         self.error_msg = error_msg
+        # The region ID of the resource.
         self.region_id = region_id
+        # The ID of the request.
         self.request_id = request_id
+        # The ID of the resource.
         self.resource_id = resource_id
+        # The type of the resource.
         self.resource_type = resource_type
+        # The ID of the Alibaba Cloud service.
         self.service = service
+        # The status of the move task. Valid values:
+        # 
+        # *   SUCCESS
+        # *   FAIL
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13457,15 +14740,17 @@
 
 class MoveResourcesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         responses: List[MoveResourcesResponseBodyResponses] = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
+        # The returned results.
         self.responses = responses
 
     def validate(self):
         if self.responses:
             for k in self.responses:
                 if k:
                     k.validate()
@@ -13542,15 +14827,17 @@
 
 class PromoteResourceAccountRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         email: str = None,
     ):
+        # The ID of the resource account you want to upgrade.
         self.account_id = account_id
+        # The email address used to log on to the cloud account after the upgrade.
         self.email = email
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13584,24 +14871,54 @@
         join_time: str = None,
         modify_time: str = None,
         record_id: str = None,
         resource_directory_id: str = None,
         status: str = None,
         type: str = None,
     ):
+        # The ID of the member account.
         self.account_id = account_id
+        # The name of the member account.
         self.account_name = account_name
+        # The display name of the member account.
         self.display_name = display_name
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The way in which the member account joined the resource directory. Valid values:
+        # 
+        # *   invited: The member account is invited to join the resource directory.
+        # *   created: The member account is directly created in the resource directory.
         self.join_method = join_method
+        # The time when the member account joined the resource directory.
         self.join_time = join_time
+        # The time when the member account was modified.
         self.modify_time = modify_time
+        # The account record ID.
         self.record_id = record_id
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the member account. Valid values:
+        # 
+        # *   CreateSuccess: The member account is created.
+        # *   CreateVerifying: The creation of the member account is under confirmation.
+        # *   CreateFailed: The member account failed to be created.
+        # *   CreateExpired: The creation of the member account expired.
+        # *   CreateCancelled: The creation of the member account is canceled.
+        # *   PromoteVerifying: The upgrade of the member account is under confirmation.
+        # *   PromoteFailed: The member account failed to be upgraded.
+        # *   PromoteExpired: The upgrade of the member account expired.
+        # *   PromoteCancelled: The upgrade of the member account is canceled.
+        # *   PromoteSuccess: The member account is upgraded.
+        # *   InviteSuccess: The owner of the member account accepted the invitation.
+        # *   Removed: The member account is removed from the resource directory.
         self.status = status
+        # The type of the member account. Valid values:
+        # 
+        # *   CloudAccount
+        # *   ResourceAccount
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13662,15 +14979,17 @@
 
 class PromoteResourceAccountResponseBody(TeaModel):
     def __init__(
         self,
         account: PromoteResourceAccountResponseBodyAccount = None,
         request_id: str = None,
     ):
+        # The information of the member account.
         self.account = account
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.account:
             self.account.validate()
 
     def to_map(self):
@@ -13741,15 +15060,19 @@
 
 class RegisterDelegatedAdministratorRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         service_principal: str = None,
     ):
+        # The ID of the member in the resource directory.
         self.account_id = account_id
+        # The identifier of the trusted service.
+        # 
+        # For more information, see the `Trusted service identifier` column in [Supported trusted services](~~208133~~).
         self.service_principal = service_principal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13773,14 +15096,15 @@
 
 
 class RegisterDelegatedAdministratorResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13844,14 +15168,15 @@
 
 
 class RemoveCloudAccountRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
     ):
+        # The ID of the member.
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13871,14 +15196,15 @@
 
 
 class RemoveCloudAccountResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13942,14 +15268,15 @@
 
 
 class ResendCreateCloudAccountEmailRequest(TeaModel):
     def __init__(
         self,
         record_id: str = None,
     ):
+        # The account record ID.
         self.record_id = record_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13979,24 +15306,51 @@
         join_time: str = None,
         modify_time: str = None,
         record_id: str = None,
         resource_directory_id: str = None,
         status: str = None,
         type: str = None,
     ):
+        # The ID of the account.
         self.account_id = account_id
+        # The name of the account.
         self.account_name = account_name
+        # The display name of the member account.
         self.display_name = display_name
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The way in which the member account joined the resource directory. Valid values:
+        # 
+        # *   invited: The member account is invited to join the resource directory.
+        # *   created: The member account is directly created in the resource directory.
         self.join_method = join_method
+        # The time when the member account joined the resource directory.
         self.join_time = join_time
+        # The time when the member account was modified.
         self.modify_time = modify_time
+        # The account record ID.
         self.record_id = record_id
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the member account. Valid values:
+        # 
+        # *   CreateSuccess: The member account is created.
+        # *   CreateVerifying: The creation of the member account is under confirmation.
+        # *   CreateFailed: The member account failed to be created.
+        # *   CreateExpired: The creation of the member account expired.
+        # *   CreateCancelled: The creation of the member account is canceled.
+        # *   PromoteVerifying: The upgrade of the member account is under confirmation.
+        # *   PromoteFailed: The member account failed to be upgraded.
+        # *   PromoteExpired: The upgrade of the member account expired.
+        # *   PromoteCancelled: The upgrade of the member account is canceled.
+        # *   PromoteSuccess: The member account is upgraded.
+        # *   InviteSuccess: The owner of the member account accepted the invitation.
+        # *   Removed: The member account is removed from the resource directory.
         self.status = status
+        # The type of the member account. The value CloudAccount indicates that the member account is a cloud account.
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14057,15 +15411,17 @@
 
 class ResendCreateCloudAccountEmailResponseBody(TeaModel):
     def __init__(
         self,
         account: ResendCreateCloudAccountEmailResponseBodyAccount = None,
         request_id: str = None,
     ):
+        # The information of the member account.
         self.account = account
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.account:
             self.account.validate()
 
     def to_map(self):
@@ -14135,14 +15491,15 @@
 
 
 class ResendPromoteResourceAccountEmailRequest(TeaModel):
     def __init__(
         self,
         record_id: str = None,
     ):
+        # The account record ID.
         self.record_id = record_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14172,24 +15529,54 @@
         join_time: str = None,
         modify_time: str = None,
         record_id: str = None,
         resource_directory_id: str = None,
         status: str = None,
         type: str = None,
     ):
+        # The ID of the account.
         self.account_id = account_id
+        # The name of the account.
         self.account_name = account_name
+        # The display name of the member account.
         self.display_name = display_name
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The way in which the member account joined the resource directory. Valid values:
+        # 
+        # *   invited: The member account is invited to join the resource directory.
+        # *   created: The member account is directly created in the resource directory.
         self.join_method = join_method
+        # The time when the member account joined the resource directory.
         self.join_time = join_time
+        # The time when the member account was modified.
         self.modify_time = modify_time
+        # The account record ID.
         self.record_id = record_id
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the member account. Valid values:
+        # 
+        # *   CreateSuccess: The member account is created.
+        # *   CreateVerifying: The creation of the member account is under confirmation.
+        # *   CreateFailed: The member account failed to be created.
+        # *   CreateExpired: The creation of the member account expired.
+        # *   CreateCancelled: The creation of the member account is canceled.
+        # *   PromoteVerifying: The upgrade of the member account is under confirmation.
+        # *   PromoteFailed: The member account failed to be upgraded.
+        # *   PromoteExpired: The upgrade of the member account expired.
+        # *   PromoteCancelled: The upgrade of the member account is canceled.
+        # *   PromoteSuccess: The member account is upgraded.
+        # *   InviteSuccess: The owner of the member account accepted the invitation.
+        # *   Removed: The member account is removed from the resource directory.
         self.status = status
+        # The type of the member account. Valid values:
+        # 
+        # *   CloudAccount: cloud account
+        # *   ResourceAccount: resource account
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14250,15 +15637,17 @@
 
 class ResendPromoteResourceAccountEmailResponseBody(TeaModel):
     def __init__(
         self,
         account: ResendPromoteResourceAccountEmailResponseBodyAccount = None,
         request_id: str = None,
     ):
+        # The information of the member account.
         self.account = account
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.account:
             self.account.validate()
 
     def to_map(self):
@@ -14328,14 +15717,15 @@
 
 
 class RetryChangeAccountEmailRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14355,14 +15745,15 @@
 
 
 class RetryChangeAccountEmailResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14427,15 +15818,21 @@
 
 class SendVerificationCodeForBindSecureMobilePhoneRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         secure_mobile_phone: str = None,
     ):
+        # The ID of the resource account.
         self.account_id = account_id
+        # The mobile phone number that you want to bind to the resource account.
+        # 
+        # Specify the mobile phone number in the \<Country code>-\<Mobile phone number> format.
+        # 
+        # >  Mobile phone numbers in the `86-<Mobile phone number>` format in the Chinese mainland are not supported.
         self.secure_mobile_phone = secure_mobile_phone
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14460,15 +15857,17 @@
 
 class SendVerificationCodeForBindSecureMobilePhoneResponseBody(TeaModel):
     def __init__(
         self,
         expiration_date: str = None,
         request_id: str = None,
     ):
+        # The time when the verification code expires.
         self.expiration_date = expiration_date
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14536,14 +15935,19 @@
 
 
 class SendVerificationCodeForEnableRDRequest(TeaModel):
     def __init__(
         self,
         secure_mobile_phone: str = None,
     ):
+        # The mobile phone number that is bound to the newly created account. If you leave this parameter empty, the mobile phone number that is bound to the current account is used.
+        # 
+        # Specify the mobile phone number in the `<Country code>-<Mobile phone number>` format.
+        # 
+        # >  Mobile phone numbers in the `86-<Mobile phone number>` format in the Chinese mainland are not supported.
         self.secure_mobile_phone = secure_mobile_phone
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14563,14 +15967,15 @@
 
 
 class SendVerificationCodeForEnableRDResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14635,15 +16040,19 @@
 
 class SetDefaultPolicyVersionRequest(TeaModel):
     def __init__(
         self,
         policy_name: str = None,
         version_id: str = None,
     ):
+        # The name of the policy.
+        # 
+        # The name must be 1 to 128 characters in length and can contain letters, digits, and hyphens (-).
         self.policy_name = policy_name
+        # The ID of the policy version.
         self.version_id = version_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14667,14 +16076,15 @@
 
 
 class SetDefaultPolicyVersionResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14738,14 +16148,18 @@
 
 
 class SetMemberDeletionPermissionRequest(TeaModel):
     def __init__(
         self,
         status: str = None,
     ):
+        # Specifies whether to enable the member deletion feature. Valid values:
+        # 
+        # *   Enabled: enables the member deletion feature
+        # *   Disabled: disables the member deletion feature
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14768,17 +16182,24 @@
     def __init__(
         self,
         management_account_id: str = None,
         member_deletion_status: str = None,
         request_id: str = None,
         resource_directory_id: str = None,
     ):
+        # The ID of the management account of the resource directory.
         self.management_account_id = management_account_id
+        # The status of the member deletion feature. Valid values:
+        # 
+        # *   Enabled: The feature is enabled.
+        # *   Disabled: The feature is disabled.
         self.member_deletion_status = member_deletion_status
+        # The ID of the request.
         self.request_id = request_id
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14855,15 +16276,21 @@
 
 class TagResourcesRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
+        # A tag key.
+        # 
+        # A tag key can be a maximum of 128 characters in length. It cannot contain `http://` or `https://` and cannot start with `acs:` or `aliyun`.
         self.key = key
+        # A tag value.
+        # 
+        # A tag value can be a maximum of 128 characters in length. It cannot contain `http://` or `https://` and cannot start with `acs:`.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14890,14 +16317,20 @@
     def __init__(
         self,
         resource_id: List[str] = None,
         resource_type: str = None,
         tag: List[TagResourcesRequestTag] = None,
     ):
         self.resource_id = resource_id
+        # The type of the objects to which you want to add tags. Valid values:
+        # 
+        # *   ResourceGroup : resource group. This is the default value.
+        # *   Account: member.
+        # 
+        # >  This parameter is required if you add tags to members in a resource directory.
         self.resource_type = resource_type
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
@@ -14934,14 +16367,15 @@
 
 
 class TagResourcesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15008,16 +16442,26 @@
     def __init__(
         self,
         all: bool = None,
         resource_id: List[str] = None,
         resource_type: str = None,
         tag_key: List[str] = None,
     ):
+        # Specifies whether to remove all tags from the specified resource groups or members. Valid values:
+        # 
+        # *   false (default value)
+        # *   true
         self.all = all
         self.resource_id = resource_id
+        # The type of the objects from which you want to remove tags. Valid values:
+        # 
+        # *   ResourceGroup: resource group. This is the default value.
+        # *   Account: member.
+        # 
+        # >  This parameter is required if you remove tags from members in a resource directory.
         self.resource_type = resource_type
         self.tag_key = tag_key
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -15050,14 +16494,15 @@
 
 
 class UntagResourcesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15123,16 +16568,26 @@
 class UpdateAccountRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         new_account_type: str = None,
         new_display_name: str = None,
     ):
+        # The ID of the Alibaba Cloud account that corresponds to the member.
         self.account_id = account_id
+        # The new type of the member. Valid values:
+        # 
+        # *   ResourceAccount: resource account
+        # *   CloudAccount: cloud account
+        # 
+        # >  You can configure either the `NewDisplayName` or `NewAccountType` parameter.
         self.new_account_type = new_account_type
+        # The new display name of the member.
+        # 
+        # >  You can configure either the `NewDisplayName` or `NewAccountType` parameter.
         self.new_display_name = new_display_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15169,23 +16624,44 @@
         join_method: str = None,
         join_time: str = None,
         modify_time: str = None,
         resource_directory_id: str = None,
         status: str = None,
         type: str = None,
     ):
+        # The ID of the Alibaba Cloud account that corresponds to the member.
         self.account_id = account_id
+        # The name of the Alibaba Cloud account that corresponds to the member.
         self.account_name = account_name
+        # The display name of the member.
         self.display_name = display_name
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The way in which the member joins the resource directory. Valid values:
+        # 
+        # *   invited: The member is invited to join the resource directory.
+        # *   created: The member is directly created in the resource directory.
         self.join_method = join_method
+        # The time when the member joined the resource directory. The time is displayed in UTC.
         self.join_time = join_time
+        # The time when the member was modified. The time is displayed in UTC.
         self.modify_time = modify_time
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the member. Valid values:
+        # 
+        # *   CreateSuccess: The member is created.
+        # *   InviteSuccess: The member accepts the invitation.
+        # *   Removed: The member is removed.
+        # *   SwitchSuccess: The type of the member is switched.
         self.status = status
+        # The type of the member. Valid values:
+        # 
+        # *   CloudAccount: cloud account
+        # *   ResourceAccount: resource account
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15242,15 +16718,17 @@
 
 class UpdateAccountResponseBody(TeaModel):
     def __init__(
         self,
         account: UpdateAccountResponseBodyAccount = None,
         request_id: str = None,
     ):
+        # The information of the member.
         self.account = account
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.account:
             self.account.validate()
 
     def to_map(self):
@@ -15323,17 +16801,31 @@
     def __init__(
         self,
         new_description: str = None,
         new_policy_document: str = None,
         new_policy_name: str = None,
         policy_id: str = None,
     ):
+        # The new description of the access control policy.
+        # 
+        # The description must be 1 to 1,024 characters in length. The description can contain letters, digits, underscores (\_), and hyphens (-) and must start with a letter.
         self.new_description = new_description
+        # The new document of the access control policy.
+        # 
+        # The document can be a maximum of 4,096 characters in length.
+        # 
+        # For more information about the languages of access control policies, see [Languages of access control policies](~~179096~~).
+        # 
+        # For more information about the examples of access control policies, see [Examples of custom access control policies](~~181474~~).
         self.new_policy_document = new_policy_document
+        # The new name of the access control policy.
+        # 
+        # The name must be 1 to 128 characters in length. The name can contain letters, digits, and hyphens (-) and must start with a letter.
         self.new_policy_name = new_policy_name
+        # The ID of the access control policy.
         self.policy_id = policy_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15372,21 +16864,35 @@
         description: str = None,
         effect_scope: str = None,
         policy_id: str = None,
         policy_name: str = None,
         policy_type: str = None,
         update_date: str = None,
     ):
+        # The number of times that the access control policy is referenced.
         self.attachment_count = attachment_count
+        # The time when the access control policy was created.
         self.create_date = create_date
+        # The description of the access control policy.
         self.description = description
+        # The effective scope of the access control policy. Valid values:
+        # 
+        # *   All: The access control policy is in effect for Alibaba Cloud accounts, RAM users, and RAM roles.
+        # *   RAM: The access control policy is in effect only for RAM users and RAM roles.
         self.effect_scope = effect_scope
+        # The ID of the access control policy.
         self.policy_id = policy_id
+        # The name of the access control policy.
         self.policy_name = policy_name
+        # The type of the access control policy. Valid values:
+        # 
+        # *   System: system access control policy
+        # *   Custom: custom access control policy
         self.policy_type = policy_type
+        # The time when the access control policy was updated.
         self.update_date = update_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15435,15 +16941,17 @@
 
 class UpdateControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         control_policy: UpdateControlPolicyResponseBodyControlPolicy = None,
         request_id: str = None,
     ):
+        # The details of the access control policy.
         self.control_policy = control_policy
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.control_policy:
             self.control_policy.validate()
 
     def to_map(self):
@@ -15514,15 +17022,19 @@
 
 class UpdateFolderRequest(TeaModel):
     def __init__(
         self,
         folder_id: str = None,
         new_folder_name: str = None,
     ):
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The new name of the folder.
+        # 
+        # The name must be 1 to 24 characters in length and can contain letters, digits, underscores (\_), periods (.), and hyphens (-).
         self.new_folder_name = new_folder_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15549,17 +17061,21 @@
     def __init__(
         self,
         create_time: str = None,
         folder_id: str = None,
         folder_name: str = None,
         parent_folder_id: str = None,
     ):
+        # The time when the folder was created.
         self.create_time = create_time
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The name of the folder.
         self.folder_name = folder_name
+        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15592,15 +17108,17 @@
 
 class UpdateFolderResponseBody(TeaModel):
     def __init__(
         self,
         folder: UpdateFolderResponseBodyFolder = None,
         request_id: str = None,
     ):
+        # The information of the folder.
         self.folder = folder
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.folder:
             self.folder.validate()
 
     def to_map(self):
@@ -15671,15 +17189,21 @@
 
 class UpdateResourceGroupRequest(TeaModel):
     def __init__(
         self,
         new_display_name: str = None,
         resource_group_id: str = None,
     ):
+        # The display name of the resource group.
+        # 
+        # The name must be 1 to 50 characters in length.
         self.new_display_name = new_display_name
+        # The ID of the resource group.
+        # 
+        # You can call the [ListResourceGroups](~~158855~~) operation to obtain the ID.
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15707,18 +17231,23 @@
         self,
         account_id: str = None,
         create_date: str = None,
         display_name: str = None,
         id: str = None,
         name: str = None,
     ):
+        # The ID of the Alibaba Cloud account to which the resource group belongs.
         self.account_id = account_id
+        # The time when the resource group was created. The time is displayed in UTC.
         self.create_date = create_date
+        # The display name of the resource group.
         self.display_name = display_name
+        # The ID of the resource group.
         self.id = id
+        # The unique identifier of the resource group.
         self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15755,15 +17284,17 @@
 
 class UpdateResourceGroupResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_group: UpdateResourceGroupResponseBodyResourceGroup = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
+        # The information of the resource group.
         self.resource_group = resource_group
 
     def validate(self):
         if self.resource_group:
             self.resource_group.validate()
 
     def to_map(self):
@@ -15836,17 +17367,29 @@
     def __init__(
         self,
         new_assume_role_policy_document: str = None,
         new_description: str = None,
         new_max_session_duration: int = None,
         role_name: str = None,
     ):
+        # The document of the policy that specifies the trusted entity to assume the RAM role.
         self.new_assume_role_policy_document = new_assume_role_policy_document
+        # The description of the RAM role.
+        # 
+        # The description must be 1 to 1,024 characters in length.
         self.new_description = new_description
+        # The maximum session duration of the RAM role.
+        # 
+        # Unit: seconds. Valid values: 3600 to 43200. Default value: 3600.
+        # 
+        # If you do not specify this parameter, the default value is used.
         self.new_max_session_duration = new_max_session_duration
+        # The name of the RAM role.
+        # 
+        # The name must be 1 to 64 characters in length and can contain letters, digits, periods (.),and hyphens (-).
         self.role_name = role_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15886,22 +17429,31 @@
         description: str = None,
         max_session_duration: int = None,
         role_id: str = None,
         role_name: str = None,
         role_principal_name: str = None,
         update_date: str = None,
     ):
+        # The Alibaba Cloud Resource Name (ARN) of the RAM role.
         self.arn = arn
+        # The document of the policy that specifies the trusted entity to assume the RAM role.
         self.assume_role_policy_document = assume_role_policy_document
+        # The time when the RAM role was created.
         self.create_date = create_date
+        # The description of the RAM role.
         self.description = description
+        # The maximum session duration of the RAM role.
         self.max_session_duration = max_session_duration
+        # The ID of the RAM role.
         self.role_id = role_id
+        # The name of the RAM role.
         self.role_name = role_name
+        # The name of the RAM role after authorization.
         self.role_principal_name = role_principal_name
+        # The time when the RAM role was updated.
         self.update_date = update_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15954,15 +17506,17 @@
 
 class UpdateRoleResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         role: UpdateRoleResponseBodyRole = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
+        # The information of the RAM role.
         self.role = role
 
     def validate(self):
         if self.role:
             self.role.validate()
 
     def to_map(self):
```

### Comparing `alibabacloud_resourcemanager20200331-2.1.3/alibabacloud_resourcemanager20200331.egg-info/PKG-INFO` & `alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-resourcemanager20200331
-Version: 2.1.3
+Version: 2.1.4
 Summary: Alibaba Cloud ResourceManager (20200331) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcemanager20200331-2.1.3/alibabacloud_resourcemanager20200331.egg-info/SOURCES.txt` & `alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331-2.1.3/setup.py` & `alibabacloud_resourcemanager20200331-2.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_resourcemanager20200331.
 
-Created on 22/02/2023
+Created on 18/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_resourcemanager20200331"
 NAME = "alibabacloud_resourcemanager20200331" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ResourceManager (20200331) SDK Library for Python"
```

