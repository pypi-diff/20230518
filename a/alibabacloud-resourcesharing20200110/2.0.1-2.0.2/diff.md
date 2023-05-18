# Comparing `tmp/alibabacloud_resourcesharing20200110-2.0.1.tar.gz` & `tmp/alibabacloud_resourcesharing20200110-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_resourcesharing20200110-2.0.1.tar", last modified: Mon Dec  5 07:18:24 2022, max compression
+gzip compressed data, was "dist/alibabacloud_resourcesharing20200110-2.0.2.tar", last modified: Thu May 18 09:11:21 2023, max compression
```

## Comparing `alibabacloud_resourcesharing20200110-2.0.1.tar` & `alibabacloud_resourcesharing20200110-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 07:18:24.000000 alibabacloud_resourcesharing20200110-2.0.1/
--rw-r--r--   0 root         (0) root         (0)      179 2022-12-05 07:18:24.000000 alibabacloud_resourcesharing20200110-2.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-12-05 07:18:24.000000 alibabacloud_resourcesharing20200110-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-12-05 07:18:24.000000 alibabacloud_resourcesharing20200110-2.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2400 2022-12-05 07:18:24.000000 alibabacloud_resourcesharing20200110-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1058 2022-12-05 07:18:24.000000 alibabacloud_resourcesharing20200110-2.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1143 2022-12-05 07:18:24.000000 alibabacloud_resourcesharing20200110-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 07:18:24.000000 alibabacloud_resourcesharing20200110-2.0.1/alibabacloud_resourcesharing20200110/
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-05 07:18:24.000000 alibabacloud_resourcesharing20200110-2.0.1/alibabacloud_resourcesharing20200110/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69358 2022-12-05 07:18:24.000000 alibabacloud_resourcesharing20200110-2.0.1/alibabacloud_resourcesharing20200110/client.py
--rw-r--r--   0 root         (0) root         (0)   124658 2022-12-05 07:18:24.000000 alibabacloud_resourcesharing20200110-2.0.1/alibabacloud_resourcesharing20200110/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 07:18:24.000000 alibabacloud_resourcesharing20200110-2.0.1/alibabacloud_resourcesharing20200110.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2400 2022-12-05 07:18:24.000000 alibabacloud_resourcesharing20200110-2.0.1/alibabacloud_resourcesharing20200110.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      516 2022-12-05 07:18:24.000000 alibabacloud_resourcesharing20200110-2.0.1/alibabacloud_resourcesharing20200110.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-05 07:18:24.000000 alibabacloud_resourcesharing20200110-2.0.1/alibabacloud_resourcesharing20200110.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-12-05 07:18:24.000000 alibabacloud_resourcesharing20200110-2.0.1/alibabacloud_resourcesharing20200110.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2022-12-05 07:18:24.000000 alibabacloud_resourcesharing20200110-2.0.1/alibabacloud_resourcesharing20200110.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-12-05 07:18:24.000000 alibabacloud_resourcesharing20200110-2.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2670 2022-12-05 07:18:24.000000 alibabacloud_resourcesharing20200110-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:11:21.000000 alibabacloud_resourcesharing20200110-2.0.2/
+-rw-r--r--   0 root         (0) root         (0)      216 2023-05-18 09:11:21.000000 alibabacloud_resourcesharing20200110-2.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-18 09:11:21.000000 alibabacloud_resourcesharing20200110-2.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-18 09:11:21.000000 alibabacloud_resourcesharing20200110-2.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-05-18 09:11:21.000000 alibabacloud_resourcesharing20200110-2.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-05-18 09:11:21.000000 alibabacloud_resourcesharing20200110-2.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-05-18 09:11:21.000000 alibabacloud_resourcesharing20200110-2.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:11:21.000000 alibabacloud_resourcesharing20200110-2.0.2/alibabacloud_resourcesharing20200110/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 09:11:21.000000 alibabacloud_resourcesharing20200110-2.0.2/alibabacloud_resourcesharing20200110/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   101534 2023-05-18 09:11:21.000000 alibabacloud_resourcesharing20200110-2.0.2/alibabacloud_resourcesharing20200110/client.py
+-rw-r--r--   0 root         (0) root         (0)   154079 2023-05-18 09:11:21.000000 alibabacloud_resourcesharing20200110-2.0.2/alibabacloud_resourcesharing20200110/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:11:21.000000 alibabacloud_resourcesharing20200110-2.0.2/alibabacloud_resourcesharing20200110.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-05-18 09:11:21.000000 alibabacloud_resourcesharing20200110-2.0.2/alibabacloud_resourcesharing20200110.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      516 2023-05-18 09:11:21.000000 alibabacloud_resourcesharing20200110-2.0.2/alibabacloud_resourcesharing20200110.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 09:11:21.000000 alibabacloud_resourcesharing20200110-2.0.2/alibabacloud_resourcesharing20200110.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-18 09:11:21.000000 alibabacloud_resourcesharing20200110-2.0.2/alibabacloud_resourcesharing20200110.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-05-18 09:11:21.000000 alibabacloud_resourcesharing20200110-2.0.2/alibabacloud_resourcesharing20200110.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-18 09:11:21.000000 alibabacloud_resourcesharing20200110-2.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-05-18 09:11:21.000000 alibabacloud_resourcesharing20200110-2.0.2/setup.py
```

### Comparing `alibabacloud_resourcesharing20200110-2.0.1/LICENSE` & `alibabacloud_resourcesharing20200110-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcesharing20200110-2.0.1/PKG-INFO` & `alibabacloud_resourcesharing20200110-2.0.2/alibabacloud_resourcesharing20200110.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_resourcesharing20200110
-Version: 2.0.1
+Name: alibabacloud-resourcesharing20200110
+Version: 2.0.2
 Summary: Alibaba Cloud ResourceSharing (20200110) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcesharing20200110-2.0.1/README-CN.md` & `alibabacloud_resourcesharing20200110-2.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcesharing20200110-2.0.1/README.md` & `alibabacloud_resourcesharing20200110-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcesharing20200110-2.0.1/alibabacloud_resourcesharing20200110/models.py` & `alibabacloud_resourcesharing20200110-2.0.2/alibabacloud_resourcesharing20200110/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 
 class AcceptResourceShareInvitationRequest(TeaModel):
     def __init__(
         self,
         resource_share_invitation_id: str = None,
     ):
+        # The ID of the invitation.
         self.resource_share_invitation_id = resource_share_invitation_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -40,17 +41,27 @@
         resource_share_invitation_id: str = None,
         resource_share_name: str = None,
         sender_account_id: str = None,
         status: str = None,
     ):
         self.create_time = create_time
         self.receiver_account_id = receiver_account_id
+        # The Alibaba Cloud account ID of the invitee.
         self.resource_share_id = resource_share_id
+        # The Alibaba Cloud account ID of the inviter.
         self.resource_share_invitation_id = resource_share_invitation_id
+        # The time when the invitation was created. The time is displayed in UTC.
         self.resource_share_name = resource_share_name
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending: The invitation is waiting for confirmation.
+        # *   Accepted: The invitation is accepted.
+        # *   Cancelled: The invitation is canceled.
+        # *   Rejected: The invitation is rejected.
+        # *   Expired: The invitation has expired.
         self.sender_account_id = sender_account_id
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -96,15 +107,17 @@
 
 class AcceptResourceShareInvitationResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_share_invitation: AcceptResourceShareInvitationResponseBodyResourceShareInvitation = None,
     ):
+        # The ID of the resource share.
         self.request_id = request_id
+        # The name of the resource share.
         self.resource_share_invitation = resource_share_invitation
 
     def validate(self):
         if self.resource_share_invitation:
             self.resource_share_invitation.validate()
 
     def to_map(self):
@@ -175,15 +188,24 @@
 
 class AssociateResourceShareRequestResources(TeaModel):
     def __init__(
         self,
         resource_id: str = None,
         resource_type: str = None,
     ):
+        # The name of a permission. If you do not configure this parameter, the system automatically associates the default permission for the specified resource type with the resource share. For more information, see [Permission library](~~465474~~).
         self.resource_id = resource_id
+        # The ID of a principal.
+        # 
+        # *   If the value of `AllowExternalTargets` for the resource share is `false` in the response of the ListResourceShares operation, the resource share supports only resource sharing within a resource directory. In this case, you can set this parameter to the ID of the resource directory, ID of a folder in the resource directory, or ID of a member in the resource directory.
+        # *   If the value of `AllowExternalTargets` for the resource share is `true` in the response of the ListResourceShares operation, the resource share supports both resource sharing within a resource directory and resource sharing outside a resource directory. In this case, you can set this parameter to the ID of an independent Alibaba Cloud account, ID of the resource directory, ID of a folder in the resource directory, or ID of a member in the resource directory.
+        # 
+        # For more information, see [Resource sharing modes](~~160622~~), [View the ID of a resource directory](~~111217~~), [View the ID of a folder](~~111223~~), or [View the ID of a member](~~111624~~).
+        # 
+        # Valid values of N: 1 to 5. This indicates that a maximum of five principals can be specified at a time.
         self.resource_type = resource_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -211,14 +233,19 @@
         self,
         permission_names: List[str] = None,
         resource_share_id: str = None,
         resources: List[AssociateResourceShareRequestResources] = None,
         targets: List[str] = None,
     ):
         self.permission_names = permission_names
+        # The ID of a shared resource.
+        # 
+        # Valid values of N: 1 to 5. This indicates that a maximum of five shared resources can be specified at a time.
+        # 
+        # >  Resources.N.ResourceId and Resources.N.ResourceType must be used in pairs.
         self.resource_share_id = resource_share_id
         self.resources = resources
         self.targets = targets
 
     def validate(self):
         if self.resources:
             for k in self.resources:
@@ -269,21 +296,45 @@
         entity_id: str = None,
         entity_type: str = None,
         resource_share_id: str = None,
         resource_share_name: str = None,
         update_time: str = None,
     ):
         self.association_status = association_status
+        # The association status. Valid values:
+        # 
+        # *   Associating: The entity is being associated.
+        # *   Associated: The entity is associated.
+        # *   Failed: The entity fails to be associated.
+        # *   Disassociating: The entity is being disassociated.
+        # *   Disassociated: The entity is disassociated.
+        # 
+        # >  The system deletes the records of entities in the `Failed` or `Disassociated` state within 48 hours to 96 hours.
         self.association_status_message = association_status_message
         self.association_type = association_type
+        # The ID of the resource share.
         self.create_time = create_time
+        # The time when the association of the entity was created. The value of this parameter depends on the value of the AssociationType parameter:
+        # 
+        # *   If the value of `AssociationType` is `Resource`, the value of this parameter is the time when the shared resource was associated with the resource share.
+        # *   If the value of `AssociationType` is `Target`, the value of this parameter is the time when the principal was associated with the resource share.
         self.entity_id = entity_id
+        # The cause of the association failure.
         self.entity_type = entity_type
+        # The association type. Valid values:
+        # 
+        # *   Resource
+        # *   Target
         self.resource_share_id = resource_share_id
+        # The type of the entity. The value of this parameter depends on the value of the AssociationType parameter:
+        # 
+        # *   If the value of AssociationType is Resource, the value of this parameter is the type of the shared resource. For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
+        # *   If the value of AssociationType is Target, the value of this parameter is `Account`.
         self.resource_share_name = resource_share_name
+        # The name of the resource share.
         self.update_time = update_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -336,15 +387,23 @@
 
 class AssociateResourceShareResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_share_associations: List[AssociateResourceShareResponseBodyResourceShareAssociations] = None,
     ):
+        # The time when the association of the entity was updated. The value of this parameter depends on the value of the AssociationType parameter:
+        # 
+        # *   If the value of `AssociationType` is `Resource`, the value of this parameter is the time when the association of the shared resource was updated.
+        # *   If the value of `AssociationType` is `Target`, the value of this parameter is the time when the association of the principal was updated.
         self.request_id = request_id
+        # The ID of the entity. The value of this parameter depends on the value of the AssociationType parameter:
+        # 
+        # *   If the value of `AssociationType` is `Resource`, the value of this parameter is the ID of the shared resource.
+        # *   If the value of `AssociationType` is `Target`, the value of this parameter is the ID of the principal.
         self.resource_share_associations = resource_share_associations
 
     def validate(self):
         if self.resource_share_associations:
             for k in self.resource_share_associations:
                 if k:
                     k.validate()
@@ -531,15 +590,24 @@
 
 class CreateResourceShareRequestResources(TeaModel):
     def __init__(
         self,
         resource_id: str = None,
         resource_type: str = None,
     ):
+        # The name of a permission. If you do not configure this parameter, the system automatically associates the default permission for the specified resource type with the resource share. For more information, see [Permission library](~~465474~~).
         self.resource_id = resource_id
+        # The ID of a principal. Valid values:
+        # 
+        # *   If you set `AllowExternalTargets` to `false`, set this parameter to the ID of a resource directory, ID of a folder in a resource directory, or ID of a member in a resource directory.
+        # *   If you set `AllowExternalTargets` to `true`, set this parameter to the ID of an independent Alibaba Cloud account, ID of a resource directory, ID of a folder in a resource directory, or ID of a member in a resource directory.
+        # 
+        # For more information, see [Resource sharing modes](~~160622~~), [View the ID of a resource directory](~~111217~~), [View the ID of a folder](~~111223~~), or [View the ID of a member](~~111624~~).
+        # 
+        # Valid values of N: 1 to 5. This indicates that a maximum of five principals can be specified at a time.
         self.resource_type = resource_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -567,16 +635,22 @@
         self,
         allow_external_targets: bool = None,
         permission_names: List[str] = None,
         resource_share_name: str = None,
         resources: List[CreateResourceShareRequestResources] = None,
         targets: List[str] = None,
     ):
+        # The information of the resource share.
         self.allow_external_targets = allow_external_targets
         self.permission_names = permission_names
+        # The ID of a shared resource.
+        # 
+        # Valid values of N: 1 to 5. This indicates that a maximum of five shared resources can be specified at a time.
+        # 
+        # >  `Resources.N.ResourceId` and `Resources.N.ResourceType` must be used in pairs.
         self.resource_share_name = resource_share_name
         self.resources = resources
         self.targets = targets
 
     def validate(self):
         if self.resources:
             for k in self.resources:
@@ -629,19 +703,34 @@
         resource_share_id: str = None,
         resource_share_name: str = None,
         resource_share_owner: str = None,
         resource_share_status: str = None,
         update_time: str = None,
     ):
         self.allow_external_targets = allow_external_targets
+        # The status of the resource share. Valid values:
+        # 
+        # *   Active: The resource share is enabled.
+        # *   Pending: The resource share is associated with one or more resource sharing invitations that are waiting for confirmation.
+        # *   Deleting: The resource share is being deleted.
+        # *   Deleted: The resource share is deleted.
+        # 
+        # >  The system deletes the records of resource shares in the Deleted state within 48 hours to 96 hours after you delete the resource shares.
         self.create_time = create_time
+        # Indicates whether resources in the resource share can be shared with accounts outside the resource directory. Valid values:
+        # 
+        # *   false: Resources in the resource share can be shared only with accounts in the resource directory.
+        # *   true: Resources in the resource share can be shared with both accounts in the resource directory and accounts outside the resource directory.
         self.resource_share_id = resource_share_id
+        # The time when the resource share was created.
         self.resource_share_name = resource_share_name
+        # The ID of the resource share.
         self.resource_share_owner = resource_share_owner
         self.resource_share_status = resource_share_status
+        # The owner of the resource share.
         self.update_time = update_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -686,15 +775,17 @@
 
 class CreateResourceShareResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_share: CreateResourceShareResponseBodyResourceShare = None,
     ):
+        # The time when the resource share was updated.
         self.request_id = request_id
+        # The name of the resource share.
         self.resource_share = resource_share
 
     def validate(self):
         if self.resource_share:
             self.resource_share.validate()
 
     def to_map(self):
@@ -862,14 +953,18 @@
 
 
 class DescribeRegionsRequest(TeaModel):
     def __init__(
         self,
         accept_language: str = None,
     ):
+        # The supported natural language. Valid values:
+        # 
+        # *   zh-CN: Chinese
+        # *   en-US: English
         self.accept_language = accept_language
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -891,16 +986,19 @@
 class DescribeRegionsResponseBodyRegions(TeaModel):
     def __init__(
         self,
         local_name: str = None,
         region_endpoint: str = None,
         region_id: str = None,
     ):
+        # The name of the region.
         self.local_name = local_name
+        # The endpoint of the Resource Sharing service in the region.
         self.region_endpoint = region_endpoint
+        # The ID of the region.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -929,15 +1027,17 @@
 
 class DescribeRegionsResponseBody(TeaModel):
     def __init__(
         self,
         regions: List[DescribeRegionsResponseBodyRegions] = None,
         request_id: str = None,
     ):
+        # The information of the regions.
         self.regions = regions
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.regions:
             for k in self.regions:
                 if k:
                     k.validate()
@@ -1014,15 +1114,22 @@
 
 class DisassociateResourceShareRequestResources(TeaModel):
     def __init__(
         self,
         resource_id: str = None,
         resource_type: str = None,
     ):
+        # The owner of the resource share. Valid values:
+        # 
+        # *   Self: The resource share belongs to the current account. This is the default value. If you are the management account or a member of a resource directory and you want to remove resources or principals from a resource share, set this parameter to Self.
+        # *   OtherAccounts: The resource share belongs to another account. If you are not the management account or a member of a resource directory and you want to exit a resource share, set this parameter to OtherAccounts.
         self.resource_id = resource_id
+        # The ID of a principal.
+        # 
+        # Valid values of N: 1 to 5. This indicates that a maximum of five principals can be specified at a time.
         self.resource_type = resource_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1049,15 +1156,21 @@
     def __init__(
         self,
         resource_owner: str = None,
         resource_share_id: str = None,
         resources: List[DisassociateResourceShareRequestResources] = None,
         targets: List[str] = None,
     ):
+        # The information of the entities that are associated with the resource share.
         self.resource_owner = resource_owner
+        # The ID of a shared resource.
+        # 
+        # Valid values of N: 1 to 5. This indicates that a maximum of five shared resources can be specified at a time.
+        # 
+        # >  Resources.N.ResourceId and Resources.N.ResourceType must be used in pairs.
         self.resource_share_id = resource_share_id
         self.resources = resources
         self.targets = targets
 
     def validate(self):
         if self.resources:
             for k in self.resources:
@@ -1108,21 +1221,45 @@
         entity_id: str = None,
         entity_type: str = None,
         resource_share_id: str = None,
         resource_share_name: str = None,
         update_time: str = None,
     ):
         self.association_status = association_status
+        # The association status. Valid values:
+        # 
+        # *   Associating: The entity is being associated.
+        # *   Associated: The entity is associated.
+        # *   Failed: The entity fails to be associated.
+        # *   Disassociating: The entity is being disassociated.
+        # *   Disassociated: The entity is disassociated.
+        # 
+        # >  The system deletes the records of entities in the `Failed` or `Disassociated` state within 48 hours to 96 hours.
         self.association_status_message = association_status_message
         self.association_type = association_type
+        # The ID of the resource share.
         self.create_time = create_time
+        # The time when the disassociation of the entity was performed. The value of this parameter depends on the value of the AssociationType parameter:
+        # 
+        # *   If the value of `AssociationType` is `Resource`, the value of this parameter is the time when the resource was disassociated from the resource share.
+        # *   If the value of `AssociationType` is `Target`, the value of this parameter is the time when the principal was disassociated from the resource share.
         self.entity_id = entity_id
+        # The cause of the disassociation failure.
         self.entity_type = entity_type
+        # The association type. Valid values:
+        # 
+        # *   Resource
+        # *   Target
         self.resource_share_id = resource_share_id
+        # The type of the entity. The value of this parameter depends on the value of the AssociationType parameter:
+        # 
+        # *   If the value of AssociationType is Resource, the value of this parameter is the type of the resource. For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
+        # *   If the value of AssociationType is Target, the value of this parameter is Account.
         self.resource_share_name = resource_share_name
+        # The name of the resource share.
         self.update_time = update_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1175,15 +1312,23 @@
 
 class DisassociateResourceShareResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_share_associations: List[DisassociateResourceShareResponseBodyResourceShareAssociations] = None,
     ):
+        # The time when the disassociation of the entity was updated. The value of this parameter depends on the value of the AssociationType parameter:
+        # 
+        # *   If the value of `AssociationType` is `Resource`, the value of this parameter is the time when the disassociation of the resource was updated.
+        # *   If the value of `AssociationType` is `Target`, the value of this parameter is the time when the disassociation of the principal was updated.
         self.request_id = request_id
+        # The ID of the entity. The value of this parameter depends on the value of the AssociationType parameter:
+        # 
+        # *   If the value of `AssociationType` is `Resource`, the value of this parameter is the ID of the resource.
+        # *   If the value of `AssociationType` is `Target`, the value of this parameter is the ID of the resource directory, folder, or member.
         self.resource_share_associations = resource_share_associations
 
     def validate(self):
         if self.resource_share_associations:
             for k in self.resource_share_associations:
                 if k:
                     k.validate()
@@ -1260,15 +1405,17 @@
 
 class DisassociateResourceSharePermissionRequest(TeaModel):
     def __init__(
         self,
         permission_name: str = None,
         resource_share_id: str = None,
     ):
+        # The ID of the request.
         self.permission_name = permission_name
+        # The name of the permission. For more information, see [Permission library](~~465474~~).
         self.resource_share_id = resource_share_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1435,15 +1582,17 @@
 
 class GetPermissionRequest(TeaModel):
     def __init__(
         self,
         permission_name: str = None,
         permission_version: str = None,
     ):
+        # The name of the permission.
         self.permission_name = permission_name
+        # The version of the permission.
         self.permission_version = permission_version
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1477,17 +1626,27 @@
         permission_version: str = None,
         resource_type: str = None,
         update_time: str = None,
     ):
         self.create_time = create_time
         self.default_permission = default_permission
         self.default_version = default_version
+        # The update time.
         self.permission = permission
+        # Indicates whether the version is the default version. Valid values:
+        # 
+        # *   false: The version is not the default version.
+        # *   true: The version is the default version.
         self.permission_name = permission_name
+        # The creation time.
         self.permission_version = permission_version
+        # Indicates whether the permission is the default permission. Valid values:
+        # 
+        # *   false: The permission is not the default permission.
+        # *   true: The permission is the default permission.
         self.resource_type = resource_type
         self.update_time = update_time
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1537,15 +1696,19 @@
 
 class GetPermissionResponseBody(TeaModel):
     def __init__(
         self,
         permission: GetPermissionResponseBodyPermission = None,
         request_id: str = None,
     ):
+        # The type of the shared resources.
+        # 
+        # For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
         self.permission = permission
+        # The document of the policy related to the permission.
         self.request_id = request_id
 
     def validate(self):
         if self.permission:
             self.permission.validate()
 
     def to_map(self):
@@ -1617,16 +1780,19 @@
 class ListPermissionVersionsRequest(TeaModel):
     def __init__(
         self,
         max_results: int = None,
         next_token: str = None,
         permission_name: str = None,
     ):
+        # The information about the permission.
         self.max_results = max_results
+        # The name of the permission.
         self.next_token = next_token
+        # The ID of the request.
         self.permission_name = permission_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1662,16 +1828,24 @@
         permission_name: str = None,
         permission_version: str = None,
         resource_type: str = None,
         update_time: str = None,
     ):
         self.create_time = create_time
         self.default_permission = default_permission
+        # Indicates whether the permission is the default permission. Valid values:
+        # 
+        # *   false: The permission is not the default permission.
+        # *   true: The permission is the default permission.
         self.default_version = default_version
+        # The update time.
         self.permission_name = permission_name
+        # The type of the shared resources.
+        # 
+        # For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
         self.permission_version = permission_version
         self.resource_type = resource_type
         self.update_time = update_time
 
     def validate(self):
         pass
 
@@ -1719,16 +1893,22 @@
 class ListPermissionVersionsResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         permissions: List[ListPermissionVersionsResponseBodyPermissions] = None,
         request_id: str = None,
     ):
+        # The version of the permission.
         self.next_token = next_token
+        # The creation time.
         self.permissions = permissions
+        # Indicates whether the version is the default version. Valid values:
+        # 
+        # *   false: The version is not the default version.
+        # *   true: The version is the default version.
         self.request_id = request_id
 
     def validate(self):
         if self.permissions:
             for k in self.permissions:
                 if k:
                     k.validate()
@@ -1810,16 +1990,19 @@
 class ListPermissionsRequest(TeaModel):
     def __init__(
         self,
         max_results: int = None,
         next_token: str = None,
         resource_type: str = None,
     ):
+        # The information about the permission.
         self.max_results = max_results
+        # The name of the permission.
         self.next_token = next_token
+        # The ID of the request.
         self.resource_type = resource_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1855,16 +2038,24 @@
         permission_name: str = None,
         permission_version: str = None,
         resource_type: str = None,
         update_time: str = None,
     ):
         self.create_time = create_time
         self.default_permission = default_permission
+        # Indicates whether the permission is the default permission. Valid values:
+        # 
+        # *   false: The permission is not the default permission.
+        # *   true: The permission is the default permission.
         self.default_version = default_version
+        # The update time.
         self.permission_name = permission_name
+        # The type of the shared resources.
+        # 
+        # For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
         self.permission_version = permission_version
         self.resource_type = resource_type
         self.update_time = update_time
 
     def validate(self):
         pass
 
@@ -1912,16 +2103,22 @@
 class ListPermissionsResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         permissions: List[ListPermissionsResponseBodyPermissions] = None,
         request_id: str = None,
     ):
+        # The version of the permission.
         self.next_token = next_token
+        # The creation time.
         self.permissions = permissions
+        # Indicates whether the version is the default version. Valid values:
+        # 
+        # *   false: The version is not the default version.
+        # *   true: The version is the default version.
         self.request_id = request_id
 
     def validate(self):
         if self.permissions:
             for k in self.permissions:
                 if k:
                     k.validate()
@@ -2007,20 +2204,43 @@
         association_type: str = None,
         max_results: int = None,
         next_token: str = None,
         resource_id: str = None,
         resource_share_ids: List[str] = None,
         target: str = None,
     ):
+        # The association status. Valid values:
+        # 
+        # *   Associating: The entity is being associated.
+        # *   Associated: The entity is associated.
+        # *   Failed: The entity fails to be associated.
+        # *   Disassociating: The entity is being disassociated.
+        # *   Disassociated: The entity is disassociated.
+        # 
+        # >  The system deletes the records of entities in the `Failed` or `Disassociated` state within 48 hours to 96 hours.
         self.association_status = association_status
+        # The association type. Valid values:
+        # 
+        # *   Resource
+        # *   Target
         self.association_type = association_type
+        # The maximum number of entries to return for a single request.
+        # 
+        # Valid values: 1 to 100. Default value: 20.
         self.max_results = max_results
+        # The `token` that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
         self.next_token = next_token
+        # The ID of the resource.
+        # 
+        # >  This parameter is unavailable if you set the `AssociationType` parameter to `Target`.
         self.resource_id = resource_id
         self.resource_share_ids = resource_share_ids
+        # The ID of the principal.
+        # 
+        # >  This parameter is unavailable if you set the `AssociationType` parameter to `Resource`.
         self.target = target
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2073,23 +2293,59 @@
         entity_id: str = None,
         entity_type: str = None,
         external: bool = None,
         resource_share_id: str = None,
         resource_share_name: str = None,
         update_time: str = None,
     ):
+        # The association status. Valid values:
+        # 
+        # *   Associating: The entity is being associated.
+        # *   Associated: The entity is associated.
+        # *   Failed: The entity fails to be associated.
+        # *   Disassociating: The entity is being disassociated.
+        # *   Disassociated: The entity is disassociated.
+        # 
+        # >  The system deletes the records of entities in the `Failed` or `Disassociated` state within 48 hours to 96 hours.
         self.association_status = association_status
+        # The cause of the association failure.
         self.association_status_message = association_status_message
+        # The association type. Valid values:
+        # 
+        # *   Resource
+        # *   Target
         self.association_type = association_type
+        # The time when the association of the entity was created. The value of this parameter depends on the value of the AssociationType parameter:
+        # 
+        # *   If the value of `AssociationType` is `Resource`, the value of this parameter is the time when the shared resource was associated with or disassociated from the resource share.
+        # *   If the value of `AssociationType` is `Target`, the value of this parameter is the time when the principal was associated with or disassociated from the resource share.
         self.create_time = create_time
+        # The ID of the entity. The value of this parameter depends on the value of the AssociationType parameter:
+        # 
+        # *   If the value of `AssociationType` is `Resource`, the value of this parameter is the ID of the shared resource.
+        # *   If the value of `AssociationType` is `Target`, the value of this parameter is the ID of the principal.
         self.entity_id = entity_id
+        # The type of the entity. The value of this parameter depends on the value of the AssociationType parameter:
+        # 
+        # *   If the value of AssociationType is Resource, the value of this parameter is the type of the resource. For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
+        # *   If the value of AssociationType is Target, the value of this parameter is `Account`.
         self.entity_type = entity_type
+        # Indicates whether the principal is outside the resource directory. Valid values:
+        # 
+        # *   true: The principal is outside the resource directory.
+        # *   false: The principal is in the resource directory.
         self.external = external
+        # The ID of the resource share.
         self.resource_share_id = resource_share_id
+        # The name of the resource share.
         self.resource_share_name = resource_share_name
+        # The time when the association of the entity was updated. The value of this parameter depends on the value of the AssociationType parameter:
+        # 
+        # *   If the value of `AssociationType` is `Resource`, the value of this parameter is the time when the association of the shared resource was updated.
+        # *   If the value of `AssociationType` is `Target`, the value of this parameter is the time when the association of the principal was updated.
         self.update_time = update_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2147,16 +2403,19 @@
 class ListResourceShareAssociationsResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         request_id: str = None,
         resource_share_associations: List[ListResourceShareAssociationsResponseBodyResourceShareAssociations] = None,
     ):
+        # The `token` that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
         self.next_token = next_token
+        # The ID of the request.
         self.request_id = request_id
+        # The information of the entities.
         self.resource_share_associations = resource_share_associations
 
     def validate(self):
         if self.resource_share_associations:
             for k in self.resource_share_associations:
                 if k:
                     k.validate()
@@ -2239,15 +2498,17 @@
     def __init__(
         self,
         max_results: int = None,
         next_token: str = None,
         resource_share_ids: List[str] = None,
         resource_share_invitation_ids: List[str] = None,
     ):
+        # The IDs of the resource sharing invitations.
         self.max_results = max_results
+        # The `token` that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
         self.next_token = next_token
         self.resource_share_ids = resource_share_ids
         self.resource_share_invitation_ids = resource_share_invitation_ids
 
     def validate(self):
         pass
 
@@ -2287,20 +2548,24 @@
         receiver_account_id: str = None,
         resource_share_id: str = None,
         resource_share_invitation_id: str = None,
         resource_share_name: str = None,
         sender_account_id: str = None,
         status: str = None,
     ):
+        # The Alibaba Cloud account ID of the inviter.
         self.create_time = create_time
         self.receiver_account_id = receiver_account_id
+        # The Alibaba Cloud account ID of the invitee.
         self.resource_share_id = resource_share_id
         self.resource_share_invitation_id = resource_share_invitation_id
+        # The ID of the invitation.
         self.resource_share_name = resource_share_name
         self.sender_account_id = sender_account_id
+        # The name of the resource share.
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2346,16 +2611,25 @@
 class ListResourceShareInvitationsResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         request_id: str = None,
         resource_share_invitations: List[ListResourceShareInvitationsResponseBodyResourceShareInvitations] = None,
     ):
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending: The invitation is waiting for confirmation.
+        # *   Accepted: The invitation is accepted.
+        # *   Cancelled: The invitation is canceled.
+        # *   Rejected: The invitation is rejected.
+        # *   Expired: The invitation has expired.
         self.next_token = next_token
+        # The time when the invitation was created. The time is displayed in UTC.
         self.request_id = request_id
+        # The ID of the resource share.
         self.resource_share_invitations = resource_share_invitations
 
     def validate(self):
         if self.resource_share_invitations:
             for k in self.resource_share_invitations:
                 if k:
                     k.validate()
@@ -2438,17 +2712,21 @@
     def __init__(
         self,
         max_results: int = None,
         next_token: str = None,
         resource_owner: str = None,
         resource_share_id: str = None,
     ):
+        # The ID of the request.
         self.max_results = max_results
+        # The information about the permissions.
         self.next_token = next_token
+        # The name of the permission.
         self.resource_owner = resource_owner
+        # The `token` that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
         self.resource_share_id = resource_share_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2488,16 +2766,24 @@
         permission_name: str = None,
         permission_version: str = None,
         resource_type: str = None,
         update_time: str = None,
     ):
         self.create_time = create_time
         self.default_permission = default_permission
+        # Indicates whether the permission is the default permission. Valid values:
+        # 
+        # *   false: The permission is not the default permission.
+        # *   true: The permission is the default permission.
         self.default_version = default_version
+        # The update time.
         self.permission_name = permission_name
+        # The type of the shared resources.
+        # 
+        # For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
         self.permission_version = permission_version
         self.resource_type = resource_type
         self.update_time = update_time
 
     def validate(self):
         pass
 
@@ -2545,16 +2831,22 @@
 class ListResourceSharePermissionsResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         permissions: List[ListResourceSharePermissionsResponseBodyPermissions] = None,
         request_id: str = None,
     ):
+        # The version of the permission.
         self.next_token = next_token
+        # The creation time.
         self.permissions = permissions
+        # Indicates whether the version is the default version. Valid values:
+        # 
+        # *   false: The version is not the default version.
+        # *   true: The version is the default version.
         self.request_id = request_id
 
     def validate(self):
         if self.permissions:
             for k in self.permissions:
                 if k:
                     k.validate()
@@ -2640,20 +2932,35 @@
         next_token: str = None,
         permission_name: str = None,
         resource_owner: str = None,
         resource_share_ids: List[str] = None,
         resource_share_name: str = None,
         resource_share_status: str = None,
     ):
+        # The ID of a resource share.
         self.max_results = max_results
+        # The name of the permission. For more information, see [Permission library](~~465474~~).
         self.next_token = next_token
+        # The ID of the request.
         self.permission_name = permission_name
+        # The status of the resource share. Valid values:
+        # 
+        # *   Active: The resource share is enabled.
+        # *   Pending: The resource share is associated with one or more resource sharing invitations that are waiting for confirmation.
+        # *   Deleting: The resource share is being deleted.
+        # *   Deleted: The resource share is deleted.
+        # 
+        # >  The system deletes the records of resource shares in the Deleted state within 48 hours to 96 hours after you delete the resource shares.
         self.resource_owner = resource_owner
         self.resource_share_ids = resource_share_ids
+        # The maximum number of entries to return for a single request.
+        # 
+        # Valid values: 1 to 100. Default value: 20.
         self.resource_share_name = resource_share_name
+        # The `token` that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
         self.resource_share_status = resource_share_status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2704,19 +3011,34 @@
         resource_share_id: str = None,
         resource_share_name: str = None,
         resource_share_owner: str = None,
         resource_share_status: str = None,
         update_time: str = None,
     ):
         self.allow_external_targets = allow_external_targets
+        # The status of the resource share. Valid values:
+        # 
+        # *   Active: The resource share is enabled.
+        # *   Pending: The resource share is associated with one or more resource sharing invitations that are waiting for confirmation.
+        # *   Deleting: The resource share is being deleted.
+        # *   Deleted: The resource share is deleted.
+        # 
+        # >  The system deletes the records of resource shares in the Deleted state within 48 hours to 96 hours after you delete the resource shares.
         self.create_time = create_time
+        # Indicates whether resources in the resource share can be shared with accounts outside the resource directory. Valid values:
+        # 
+        # *   false: Resources in the resource share can be shared only with accounts in the resource directory.
+        # *   true: Resources in the resource share can be shared with both accounts in the resource directory and accounts outside the resource directory.
         self.resource_share_id = resource_share_id
+        # The time when the resource share was created.
         self.resource_share_name = resource_share_name
+        # The ID of the resource share.
         self.resource_share_owner = resource_share_owner
         self.resource_share_status = resource_share_status
+        # The owner of the resource share.
         self.update_time = update_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2762,16 +3084,19 @@
 class ListResourceSharesResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         request_id: str = None,
         resource_shares: List[ListResourceSharesResponseBodyResourceShares] = None,
     ):
+        # The information of the resource shares.
         self.next_token = next_token
+        # The time when the resource share was updated.
         self.request_id = request_id
+        # The name of the resource share.
         self.resource_shares = resource_shares
 
     def validate(self):
         if self.resource_shares:
             for k in self.resource_shares:
                 if k:
                     k.validate()
@@ -2857,20 +3182,35 @@
         next_token: str = None,
         resource_ids: List[str] = None,
         resource_owner: str = None,
         resource_share_ids: List[str] = None,
         resource_type: str = None,
         target: str = None,
     ):
+        # The maximum number of entries to return for a single request.
+        # 
+        # Valid values: 1 to 100. Default value: 20.
         self.max_results = max_results
+        # The `token` that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
         self.next_token = next_token
         self.resource_ids = resource_ids
+        # The owner of the resource shares. Valid values:
+        # 
+        # *   Self: your account. If you set the value to Self, the resources you share with other accounts are queried.
+        # *   OtherAccounts: another account. If you set the value to OtherAccounts, the resources other accounts share with you are queried.
         self.resource_owner = resource_owner
         self.resource_share_ids = resource_share_ids
+        # The type of the shared resources.
+        # 
+        # For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
         self.resource_type = resource_type
+        # The ID of the principal or resource owner.
+        # 
+        # *   If the value of `ResourceOwner` is `Self`, set this parameter to the ID of a principal.
+        # *   If the value of `ResourceOwner` is `OtherAccounts`, set this parameter to the ID of a resource owner.
         self.target = target
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2920,20 +3260,36 @@
         resource_id: str = None,
         resource_share_id: str = None,
         resource_status: str = None,
         resource_status_message: str = None,
         resource_type: str = None,
         update_time: str = None,
     ):
+        # The time when the shared resource was associated with the resource share.
         self.create_time = create_time
+        # The ID of the shared resource.
         self.resource_id = resource_id
+        # The ID of the resource share.
         self.resource_share_id = resource_share_id
+        # The status of the shared resource. This parameter is returned only when you query the resources that other accounts share with you.
+        # 
+        # Valid values:
+        # 
+        # *   Available: The resource is available.
+        # *   ZonalResourceInaccessible: The resource is unavailable in the current zone.
+        # *   LimitExceeded: The resource is unavailable because the maximum number of resources that other accounts can share with you exceeds the upper limit.
+        # *   Unavailable: The resource is unavailable.
         self.resource_status = resource_status
+        # The cause of the association failure.
         self.resource_status_message = resource_status_message
+        # The type of the shared resource.
+        # 
+        # For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
         self.resource_type = resource_type
+        # The time when the association of the shared resource was updated.
         self.update_time = update_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2979,16 +3335,19 @@
 class ListSharedResourcesResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         request_id: str = None,
         shared_resources: List[ListSharedResourcesResponseBodySharedResources] = None,
     ):
+        # The token that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
         self.next_token = next_token
+        # The ID of the request.
         self.request_id = request_id
+        # The information of the shared resources.
         self.shared_resources = shared_resources
 
     def validate(self):
         if self.shared_resources:
             for k in self.shared_resources:
                 if k:
                     k.validate()
@@ -3074,19 +3433,31 @@
         next_token: str = None,
         resource_id: str = None,
         resource_owner: str = None,
         resource_share_ids: List[str] = None,
         resource_type: str = None,
         targets: List[str] = None,
     ):
+        # The maximum number of entries to return for a single request.
+        # 
+        # Valid values: 1 to 100. Default value: 20.
         self.max_results = max_results
+        # The `token` that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
         self.next_token = next_token
+        # The ID of the shared resource.
         self.resource_id = resource_id
+        # The owner of the resource share.
+        # 
+        # *   Self: your account. If you set the value to Self, the principals that are associated with your resource shares are queried.
+        # *   OtherAccounts: another account. If you set the value to OtherAccounts, the resource shares with which your account is associated and the owners of the resource shares are queried.
         self.resource_owner = resource_owner
         self.resource_share_ids = resource_share_ids
+        # The type of the shared resources.
+        # 
+        # For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
         self.resource_type = resource_type
         self.targets = targets
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -3135,18 +3506,29 @@
         self,
         create_time: str = None,
         external: bool = None,
         resource_share_id: str = None,
         target_id: str = None,
         update_time: str = None,
     ):
+        # The time when the principal was associated with the resource share.
         self.create_time = create_time
+        # Indicates whether the principal is outside the resource directory. Valid values:
+        # 
+        # *   true: The principal is outside the resource directory.
+        # *   false: The principal is in the resource directory.
         self.external = external
+        # The ID of the resource share.
         self.resource_share_id = resource_share_id
+        # The ID of the principal or resource owner.
+        # 
+        # *   If the value of `ResourceOwner` is `Self`, the value of this parameter is the ID of a principal.
+        # *   If the value of `ResourceOwner` is `OtherAccounts`, the value of this parameter is the ID of a resource owner.
         self.target_id = target_id
+        # The time when the association of the principal was updated.
         self.update_time = update_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3184,16 +3566,19 @@
 class ListSharedTargetsResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         request_id: str = None,
         shared_targets: List[ListSharedTargetsResponseBodySharedTargets] = None,
     ):
+        # The `token` that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
         self.next_token = next_token
+        # The ID of the request.
         self.request_id = request_id
+        # The information of the principals.
         self.shared_targets = shared_targets
 
     def validate(self):
         if self.shared_targets:
             for k in self.shared_targets:
                 if k:
                     k.validate()
@@ -3273,14 +3658,15 @@
 
 
 class RejectResourceShareInvitationRequest(TeaModel):
     def __init__(
         self,
         resource_share_invitation_id: str = None,
     ):
+        # The ID of the invitation.
         self.resource_share_invitation_id = resource_share_invitation_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3308,17 +3694,27 @@
         resource_share_invitation_id: str = None,
         resource_share_name: str = None,
         sender_account_id: str = None,
         status: str = None,
     ):
         self.create_time = create_time
         self.receiver_account_id = receiver_account_id
+        # The Alibaba Cloud account ID of the invitee.
         self.resource_share_id = resource_share_id
+        # The Alibaba Cloud account ID of the inviter.
         self.resource_share_invitation_id = resource_share_invitation_id
+        # The time when the invitation was created. The time is displayed in UTC.
         self.resource_share_name = resource_share_name
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending: The invitation is waiting for confirmation.
+        # *   Accepted: The invitation is accepted.
+        # *   Cancelled: The invitation is canceled.
+        # *   Rejected: The invitation is rejected.
+        # *   Expired: The invitation has expired.
         self.sender_account_id = sender_account_id
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -3364,15 +3760,17 @@
 
 class RejectResourceShareInvitationResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_share_invitation: RejectResourceShareInvitationResponseBodyResourceShareInvitation = None,
     ):
+        # The ID of the resource share.
         self.request_id = request_id
+        # The name of the resource share.
         self.resource_share_invitation = resource_share_invitation
 
     def validate(self):
         if self.resource_share_invitation:
             self.resource_share_invitation.validate()
 
     def to_map(self):
@@ -3444,16 +3842,22 @@
 class UpdateResourceShareRequest(TeaModel):
     def __init__(
         self,
         allow_external_targets: bool = None,
         resource_share_id: str = None,
         resource_share_name: str = None,
     ):
+        # The information of the resource share.
         self.allow_external_targets = allow_external_targets
+        # Specifies whether resources in the resource share can be shared with accounts outside the resource directory. Valid values:
+        # 
+        # *   false: Resources in the resource share can be shared only with accounts in the resource directory.
+        # *   true: Resources in the resource share can be shared with both accounts in the resource directory and accounts outside the resource directory.
         self.resource_share_id = resource_share_id
+        # The ID of the request.
         self.resource_share_name = resource_share_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3488,19 +3892,34 @@
         resource_share_id: str = None,
         resource_share_name: str = None,
         resource_share_owner: str = None,
         resource_share_status: str = None,
         update_time: str = None,
     ):
         self.allow_external_targets = allow_external_targets
+        # The status of the resource share. Valid values:
+        # 
+        # *   Active: The resource share is enabled.
+        # *   Pending: The resource share is associated with one or more resource sharing invitations that are waiting for confirmation.
+        # *   Deleting: The resource share is being deleted.
+        # *   Deleted: The resource share is deleted.
+        # 
+        # >  The system deletes the records of resource shares in the Deleted state within 48 hours to 96 hours after you delete the resource shares.
         self.create_time = create_time
+        # Indicates whether resources in the resource share can be shared with accounts outside the resource directory. Valid values:
+        # 
+        # *   false: Resources in the resource share can be shared only with accounts in the resource directory.
+        # *   true: Resources in the resource share can be shared with both accounts in the resource directory and accounts outside the resource directory.
         self.resource_share_id = resource_share_id
+        # The time when the resource share was created.
         self.resource_share_name = resource_share_name
+        # The ID of the resource share.
         self.resource_share_owner = resource_share_owner
         self.resource_share_status = resource_share_status
+        # The owner of the resource share.
         self.update_time = update_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3545,15 +3964,17 @@
 
 class UpdateResourceShareResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_share: UpdateResourceShareResponseBodyResourceShare = None,
     ):
+        # The time when the resource share was updated.
         self.request_id = request_id
+        # The name of the resource share.
         self.resource_share = resource_share
 
     def validate(self):
         if self.resource_share:
             self.resource_share.validate()
 
     def to_map(self):
```

### Comparing `alibabacloud_resourcesharing20200110-2.0.1/alibabacloud_resourcesharing20200110.egg-info/PKG-INFO` & `alibabacloud_resourcesharing20200110-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-resourcesharing20200110
-Version: 2.0.1
+Name: alibabacloud_resourcesharing20200110
+Version: 2.0.2
 Summary: Alibaba Cloud ResourceSharing (20200110) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcesharing20200110-2.0.1/alibabacloud_resourcesharing20200110.egg-info/SOURCES.txt` & `alibabacloud_resourcesharing20200110-2.0.2/alibabacloud_resourcesharing20200110.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcesharing20200110-2.0.1/setup.py` & `alibabacloud_resourcesharing20200110-2.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_resourcesharing20200110.
 
-Created on 05/12/2022
+Created on 18/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_resourcesharing20200110"
 NAME = "alibabacloud_resourcesharing20200110" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ResourceSharing (20200110) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.0, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

