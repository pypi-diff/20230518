# Comparing `tmp/alibabacloud_resourcesharing20200110_py2-1.0.0.tar.gz` & `tmp/alibabacloud_resourcesharing20200110_py2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_resourcesharing20200110_py2-1.0.0.tar", last modified: Wed Mar  8 07:04:49 2023, max compression
+gzip compressed data, was "dist/alibabacloud_resourcesharing20200110_py2-1.0.1.tar", last modified: Thu May 18 09:11:30 2023, max compression
```

## Comparing `alibabacloud_resourcesharing20200110_py2-1.0.0.tar` & `alibabacloud_resourcesharing20200110_py2-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 07:04:49.000000 alibabacloud_resourcesharing20200110_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      588 2023-03-08 07:04:49.000000 alibabacloud_resourcesharing20200110_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-08 07:04:49.000000 alibabacloud_resourcesharing20200110_py2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2544 2023-03-08 07:04:49.000000 alibabacloud_resourcesharing20200110_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1069 2023-03-08 07:04:49.000000 alibabacloud_resourcesharing20200110_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1152 2023-03-08 07:04:49.000000 alibabacloud_resourcesharing20200110_py2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 07:04:49.000000 alibabacloud_resourcesharing20200110_py2-1.0.0/alibabacloud_resourcesharing20200110/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-08 07:04:49.000000 alibabacloud_resourcesharing20200110_py2-1.0.0/alibabacloud_resourcesharing20200110/__init__.py
--rw-r--r--   0 root         (0) root         (0)    59594 2023-03-08 07:04:49.000000 alibabacloud_resourcesharing20200110_py2-1.0.0/alibabacloud_resourcesharing20200110/client.py
--rw-r--r--   0 root         (0) root         (0)   160456 2023-03-08 07:04:49.000000 alibabacloud_resourcesharing20200110_py2-1.0.0/alibabacloud_resourcesharing20200110/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 07:04:49.000000 alibabacloud_resourcesharing20200110_py2-1.0.0/alibabacloud_resourcesharing20200110_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2544 2023-03-08 07:04:49.000000 alibabacloud_resourcesharing20200110_py2-1.0.0/alibabacloud_resourcesharing20200110_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      523 2023-03-08 07:04:49.000000 alibabacloud_resourcesharing20200110_py2-1.0.0/alibabacloud_resourcesharing20200110_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-08 07:04:49.000000 alibabacloud_resourcesharing20200110_py2-1.0.0/alibabacloud_resourcesharing20200110_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-03-08 07:04:49.000000 alibabacloud_resourcesharing20200110_py2-1.0.0/alibabacloud_resourcesharing20200110_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-03-08 07:04:49.000000 alibabacloud_resourcesharing20200110_py2-1.0.0/alibabacloud_resourcesharing20200110_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-08 07:04:49.000000 alibabacloud_resourcesharing20200110_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2963 2023-03-08 07:04:49.000000 alibabacloud_resourcesharing20200110_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:11:30.000000 alibabacloud_resourcesharing20200110_py2-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-18 09:11:30.000000 alibabacloud_resourcesharing20200110_py2-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-18 09:11:30.000000 alibabacloud_resourcesharing20200110_py2-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-18 09:11:30.000000 alibabacloud_resourcesharing20200110_py2-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-05-18 09:11:30.000000 alibabacloud_resourcesharing20200110_py2-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-05-18 09:11:30.000000 alibabacloud_resourcesharing20200110_py2-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-05-18 09:11:30.000000 alibabacloud_resourcesharing20200110_py2-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:11:30.000000 alibabacloud_resourcesharing20200110_py2-1.0.1/alibabacloud_resourcesharing20200110/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 09:11:30.000000 alibabacloud_resourcesharing20200110_py2-1.0.1/alibabacloud_resourcesharing20200110/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44228 2023-05-18 09:11:30.000000 alibabacloud_resourcesharing20200110_py2-1.0.1/alibabacloud_resourcesharing20200110/client.py
+-rw-r--r--   0 root         (0) root         (0)   155344 2023-05-18 09:11:30.000000 alibabacloud_resourcesharing20200110_py2-1.0.1/alibabacloud_resourcesharing20200110/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:11:30.000000 alibabacloud_resourcesharing20200110_py2-1.0.1/alibabacloud_resourcesharing20200110_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-05-18 09:11:30.000000 alibabacloud_resourcesharing20200110_py2-1.0.1/alibabacloud_resourcesharing20200110_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      536 2023-05-18 09:11:30.000000 alibabacloud_resourcesharing20200110_py2-1.0.1/alibabacloud_resourcesharing20200110_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 09:11:30.000000 alibabacloud_resourcesharing20200110_py2-1.0.1/alibabacloud_resourcesharing20200110_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-18 09:11:30.000000 alibabacloud_resourcesharing20200110_py2-1.0.1/alibabacloud_resourcesharing20200110_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-05-18 09:11:30.000000 alibabacloud_resourcesharing20200110_py2-1.0.1/alibabacloud_resourcesharing20200110_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-18 09:11:30.000000 alibabacloud_resourcesharing20200110_py2-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-05-18 09:11:30.000000 alibabacloud_resourcesharing20200110_py2-1.0.1/setup.py
```

### Comparing `alibabacloud_resourcesharing20200110_py2-1.0.0/LICENSE` & `alibabacloud_resourcesharing20200110_py2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcesharing20200110_py2-1.0.0/PKG-INFO` & `alibabacloud_resourcesharing20200110_py2-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_resourcesharing20200110_py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud ResourceSharing (20200110) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcesharing20200110_py2-1.0.0/README-CN.md` & `alibabacloud_resourcesharing20200110_py2-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcesharing20200110_py2-1.0.0/README.md` & `alibabacloud_resourcesharing20200110_py2-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcesharing20200110_py2-1.0.0/alibabacloud_resourcesharing20200110/models.py` & `alibabacloud_resourcesharing20200110_py2-1.0.1/alibabacloud_resourcesharing20200110/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 
 
 class AcceptResourceShareInvitationRequest(TeaModel):
     def __init__(self, resource_share_invitation_id=None):
-        # The ID of the resource sharing invitation.
-        # 
-        # You can call the [ListResourceShareInvitations](~~450564~~) operation to obtain the ID of a resource sharing invitation.
+        # The ID of the invitation.
         self.resource_share_invitation_id = resource_share_invitation_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AcceptResourceShareInvitationRequest, self).to_map()
@@ -29,33 +27,30 @@
             self.resource_share_invitation_id = m.get('ResourceShareInvitationId')
         return self
 
 
 class AcceptResourceShareInvitationResponseBodyResourceShareInvitation(TeaModel):
     def __init__(self, create_time=None, receiver_account_id=None, resource_share_id=None,
                  resource_share_invitation_id=None, resource_share_name=None, sender_account_id=None, status=None):
-        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time  # type: str
-        # The Alibaba Cloud account ID of the invitee.
         self.receiver_account_id = receiver_account_id  # type: str
-        # The ID of the resource share.
+        # The Alibaba Cloud account ID of the invitee.
         self.resource_share_id = resource_share_id  # type: str
-        # The ID of the invitation.
+        # The Alibaba Cloud account ID of the inviter.
         self.resource_share_invitation_id = resource_share_invitation_id  # type: str
-        # The name of the resource share.
+        # The time when the invitation was created. The time is displayed in UTC.
         self.resource_share_name = resource_share_name  # type: str
-        # The Alibaba Cloud account ID of the inviter.
-        self.sender_account_id = sender_account_id  # type: str
         # The status of the invitation. Valid values:
         # 
         # *   Pending: The invitation is waiting for confirmation.
         # *   Accepted: The invitation is accepted.
         # *   Cancelled: The invitation is canceled.
         # *   Rejected: The invitation is rejected.
         # *   Expired: The invitation has expired.
+        self.sender_account_id = sender_account_id  # type: str
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AcceptResourceShareInvitationResponseBodyResourceShareInvitation, self).to_map()
@@ -96,17 +91,17 @@
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
 
 
 class AcceptResourceShareInvitationResponseBody(TeaModel):
     def __init__(self, request_id=None, resource_share_invitation=None):
-        # The ID of the request.
+        # The ID of the resource share.
         self.request_id = request_id  # type: str
-        # The information of the resource sharing invitation.
+        # The name of the resource share.
         self.resource_share_invitation = resource_share_invitation  # type: AcceptResourceShareInvitationResponseBodyResourceShareInvitation
 
     def validate(self):
         if self.resource_share_invitation:
             self.resource_share_invitation.validate()
 
     def to_map(self):
@@ -168,27 +163,24 @@
             temp_model = AcceptResourceShareInvitationResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class AssociateResourceShareRequestResources(TeaModel):
     def __init__(self, resource_id=None, resource_type=None):
-        # The ID of a shared resource.
-        # 
-        # Valid values of N: 1 to 5. This indicates that a maximum of five shared resources can be specified at a time.
-        # 
-        # >  Resources.N.ResourceId and Resources.N.ResourceType must be used in pairs.
+        # The name of a permission. If you do not configure this parameter, the system automatically associates the default permission for the specified resource type with the resource share. For more information, see [Permission library](~~465474~~).
         self.resource_id = resource_id  # type: str
-        # The type of a shared resource.
+        # The ID of a principal.
         # 
-        # Valid values of N: 1 to 5. This indicates that a maximum of five shared resources can be specified at a time.
+        # *   If the value of `AllowExternalTargets` for the resource share is `false` in the response of the ListResourceShares operation, the resource share supports only resource sharing within a resource directory. In this case, you can set this parameter to the ID of the resource directory, ID of a folder in the resource directory, or ID of a member in the resource directory.
+        # *   If the value of `AllowExternalTargets` for the resource share is `true` in the response of the ListResourceShares operation, the resource share supports both resource sharing within a resource directory and resource sharing outside a resource directory. In this case, you can set this parameter to the ID of an independent Alibaba Cloud account, ID of the resource directory, ID of a folder in the resource directory, or ID of a member in the resource directory.
         # 
-        # For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
+        # For more information, see [Resource sharing modes](~~160622~~), [View the ID of a resource directory](~~111217~~), [View the ID of a folder](~~111223~~), or [View the ID of a member](~~111624~~).
         # 
-        # >  `Resources.N.ResourceId` and `Resources.N.ResourceType` must be used in pairs.
+        # Valid values of N: 1 to 5. This indicates that a maximum of five principals can be specified at a time.
         self.resource_type = resource_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AssociateResourceShareRequestResources, self).to_map()
@@ -210,15 +202,19 @@
             self.resource_type = m.get('ResourceType')
         return self
 
 
 class AssociateResourceShareRequest(TeaModel):
     def __init__(self, permission_names=None, resource_share_id=None, resources=None, targets=None):
         self.permission_names = permission_names  # type: list[str]
-        # The ID of the resource share.
+        # The ID of a shared resource.
+        # 
+        # Valid values of N: 1 to 5. This indicates that a maximum of five shared resources can be specified at a time.
+        # 
+        # >  Resources.N.ResourceId and Resources.N.ResourceType must be used in pairs.
         self.resource_share_id = resource_share_id  # type: str
         self.resources = resources  # type: list[AssociateResourceShareRequestResources]
         self.targets = targets  # type: list[str]
 
     def validate(self):
         if self.resources:
             for k in self.resources:
@@ -259,54 +255,46 @@
         return self
 
 
 class AssociateResourceShareResponseBodyResourceShareAssociations(TeaModel):
     def __init__(self, association_status=None, association_status_message=None, association_type=None,
                  create_time=None, entity_id=None, entity_type=None, resource_share_id=None, resource_share_name=None,
                  update_time=None):
+        self.association_status = association_status  # type: str
         # The association status. Valid values:
         # 
         # *   Associating: The entity is being associated.
         # *   Associated: The entity is associated.
         # *   Failed: The entity fails to be associated.
         # *   Disassociating: The entity is being disassociated.
         # *   Disassociated: The entity is disassociated.
         # 
         # >  The system deletes the records of entities in the `Failed` or `Disassociated` state within 48 hours to 96 hours.
-        self.association_status = association_status  # type: str
-        # The cause of the association failure.
         self.association_status_message = association_status_message  # type: str
-        # The association type. Valid values:
-        # 
-        # *   Resource
-        # *   Target
         self.association_type = association_type  # type: str
+        # The ID of the resource share.
+        self.create_time = create_time  # type: str
         # The time when the association of the entity was created. The value of this parameter depends on the value of the AssociationType parameter:
         # 
         # *   If the value of `AssociationType` is `Resource`, the value of this parameter is the time when the shared resource was associated with the resource share.
         # *   If the value of `AssociationType` is `Target`, the value of this parameter is the time when the principal was associated with the resource share.
-        self.create_time = create_time  # type: str
-        # The ID of the entity. The value of this parameter depends on the value of the AssociationType parameter:
-        # 
-        # *   If the value of `AssociationType` is `Resource`, the value of this parameter is the ID of the shared resource.
-        # *   If the value of `AssociationType` is `Target`, the value of this parameter is the ID of the principal.
         self.entity_id = entity_id  # type: str
+        # The cause of the association failure.
+        self.entity_type = entity_type  # type: str
+        # The association type. Valid values:
+        # 
+        # *   Resource
+        # *   Target
+        self.resource_share_id = resource_share_id  # type: str
         # The type of the entity. The value of this parameter depends on the value of the AssociationType parameter:
         # 
         # *   If the value of AssociationType is Resource, the value of this parameter is the type of the shared resource. For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
         # *   If the value of AssociationType is Target, the value of this parameter is `Account`.
-        self.entity_type = entity_type  # type: str
-        # The ID of the resource share.
-        self.resource_share_id = resource_share_id  # type: str
-        # The name of the resource share.
         self.resource_share_name = resource_share_name  # type: str
-        # The time when the association of the entity was updated. The value of this parameter depends on the value of the AssociationType parameter:
-        # 
-        # *   If the value of `AssociationType` is `Resource`, the value of this parameter is the time when the association of the shared resource was updated.
-        # *   If the value of `AssociationType` is `Target`, the value of this parameter is the time when the association of the principal was updated.
+        # The name of the resource share.
         self.update_time = update_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AssociateResourceShareResponseBodyResourceShareAssociations, self).to_map()
@@ -355,17 +343,23 @@
         if m.get('UpdateTime') is not None:
             self.update_time = m.get('UpdateTime')
         return self
 
 
 class AssociateResourceShareResponseBody(TeaModel):
     def __init__(self, request_id=None, resource_share_associations=None):
-        # The ID of the request.
+        # The time when the association of the entity was updated. The value of this parameter depends on the value of the AssociationType parameter:
+        # 
+        # *   If the value of `AssociationType` is `Resource`, the value of this parameter is the time when the association of the shared resource was updated.
+        # *   If the value of `AssociationType` is `Target`, the value of this parameter is the time when the association of the principal was updated.
         self.request_id = request_id  # type: str
-        # The information of the entities that are associated with the resource share.
+        # The ID of the entity. The value of this parameter depends on the value of the AssociationType parameter:
+        # 
+        # *   If the value of `AssociationType` is `Resource`, the value of this parameter is the ID of the shared resource.
+        # *   If the value of `AssociationType` is `Target`, the value of this parameter is the ID of the principal.
         self.resource_share_associations = resource_share_associations  # type: list[AssociateResourceShareResponseBodyResourceShareAssociations]
 
     def validate(self):
         if self.resource_share_associations:
             for k in self.resource_share_associations:
                 if k:
                     k.validate()
@@ -433,22 +427,16 @@
             temp_model = AssociateResourceShareResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class AssociateResourceSharePermissionRequest(TeaModel):
     def __init__(self, permission_name=None, replace=None, resource_share_id=None):
-        # The name of the permission.
         self.permission_name = permission_name  # type: str
-        # Specifies whether to use the specified permission to replace an existing permission. Valid values:
-        # 
-        # *   false: does not use the specified permission to replace an existing permission. This is the default value. If you set the value to false for a resource share that does not have associated permissions, the system associates the specified permission with the resource share. In a resource share, one resource type can have only one permission. If you set the value to false for a resource share that already has a permission for the resource type indicated by the specified permission, the system reports an error. This prevents you from replacing the existing permission by mistake.
-        # *   true: uses the specified permission to replace an existing permission of the same resource type.
         self.replace = replace  # type: bool
-        # The ID of the resource share.
         self.resource_share_id = resource_share_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AssociateResourceSharePermissionRequest, self).to_map()
@@ -473,15 +461,14 @@
         if m.get('ResourceShareId') is not None:
             self.resource_share_id = m.get('ResourceShareId')
         return self
 
 
 class AssociateResourceSharePermissionResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AssociateResourceSharePermissionResponseBody, self).to_map()
@@ -537,27 +524,24 @@
             temp_model = AssociateResourceSharePermissionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateResourceShareRequestResources(TeaModel):
     def __init__(self, resource_id=None, resource_type=None):
-        # The ID of a shared resource.
-        # 
-        # Valid values of N: 1 to 5. This indicates that a maximum of five shared resources can be specified at a time.
-        # 
-        # >  `Resources.N.ResourceId` and `Resources.N.ResourceType` must be used in pairs.
+        # The name of a permission. If you do not configure this parameter, the system automatically associates the default permission for the specified resource type with the resource share. For more information, see [Permission library](~~465474~~).
         self.resource_id = resource_id  # type: str
-        # The type of a shared resource.
+        # The ID of a principal. Valid values:
         # 
-        # Valid values of N: 1 to 5. This indicates that a maximum of five shared resources can be specified at a time.
+        # *   If you set `AllowExternalTargets` to `false`, set this parameter to the ID of a resource directory, ID of a folder in a resource directory, or ID of a member in a resource directory.
+        # *   If you set `AllowExternalTargets` to `true`, set this parameter to the ID of an independent Alibaba Cloud account, ID of a resource directory, ID of a folder in a resource directory, or ID of a member in a resource directory.
         # 
-        # For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
+        # For more information, see [Resource sharing modes](~~160622~~), [View the ID of a resource directory](~~111217~~), [View the ID of a folder](~~111223~~), or [View the ID of a member](~~111624~~).
         # 
-        # >  `Resources.N.ResourceId` and `Resources.N.ResourceType` must be used in pairs.
+        # Valid values of N: 1 to 5. This indicates that a maximum of five principals can be specified at a time.
         self.resource_type = resource_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateResourceShareRequestResources, self).to_map()
@@ -577,28 +561,24 @@
             self.resource_id = m.get('ResourceId')
         if m.get('ResourceType') is not None:
             self.resource_type = m.get('ResourceType')
         return self
 
 
 class CreateResourceShareRequest(TeaModel):
-    def __init__(self, allow_external_targets=None, permission_names=None, resource_group_id=None,
-                 resource_share_name=None, resources=None, targets=None):
-        # Specifies whether resources in the resource share can be shared with accounts outside the resource directory. Valid values:
-        # 
-        # *   false: Resources in the resource share can be shared only with accounts in the resource directory. This is the default value.
-        # *   true: Resources in the resource share can be shared with both accounts in the resource directory and accounts outside the resource directory.
+    def __init__(self, allow_external_targets=None, permission_names=None, resource_share_name=None,
+                 resources=None, targets=None):
+        # The information of the resource share.
         self.allow_external_targets = allow_external_targets  # type: bool
         self.permission_names = permission_names  # type: list[str]
-        self.resource_group_id = resource_group_id  # type: str
-        # The name of the resource share.
+        # The ID of a shared resource.
         # 
-        # The name must be 1 to 50 characters in length.
+        # Valid values of N: 1 to 5. This indicates that a maximum of five shared resources can be specified at a time.
         # 
-        # The name can contain letters, digits, periods (.), underscores (\_), and hyphens (-).
+        # >  `Resources.N.ResourceId` and `Resources.N.ResourceType` must be used in pairs.
         self.resource_share_name = resource_share_name  # type: str
         self.resources = resources  # type: list[CreateResourceShareRequestResources]
         self.targets = targets  # type: list[str]
 
     def validate(self):
         if self.resources:
             for k in self.resources:
@@ -611,16 +591,14 @@
             return _map
 
         result = dict()
         if self.allow_external_targets is not None:
             result['AllowExternalTargets'] = self.allow_external_targets
         if self.permission_names is not None:
             result['PermissionNames'] = self.permission_names
-        if self.resource_group_id is not None:
-            result['ResourceGroupId'] = self.resource_group_id
         if self.resource_share_name is not None:
             result['ResourceShareName'] = self.resource_share_name
         result['Resources'] = []
         if self.resources is not None:
             for k in self.resources:
                 result['Resources'].append(k.to_map() if k else None)
         if self.targets is not None:
@@ -629,16 +607,14 @@
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('AllowExternalTargets') is not None:
             self.allow_external_targets = m.get('AllowExternalTargets')
         if m.get('PermissionNames') is not None:
             self.permission_names = m.get('PermissionNames')
-        if m.get('ResourceGroupId') is not None:
-            self.resource_group_id = m.get('ResourceGroupId')
         if m.get('ResourceShareName') is not None:
             self.resource_share_name = m.get('ResourceShareName')
         self.resources = []
         if m.get('Resources') is not None:
             for k in m.get('Resources'):
                 temp_model = CreateResourceShareRequestResources()
                 self.resources.append(temp_model.from_map(k))
@@ -646,37 +622,35 @@
             self.targets = m.get('Targets')
         return self
 
 
 class CreateResourceShareResponseBodyResourceShare(TeaModel):
     def __init__(self, allow_external_targets=None, create_time=None, resource_share_id=None,
                  resource_share_name=None, resource_share_owner=None, resource_share_status=None, update_time=None):
-        # Indicates whether resources in the resource share can be shared with accounts outside the resource directory. Valid values:
-        # 
-        # *   false: Resources in the resource share can be shared only with accounts in the resource directory.
-        # *   true: Resources in the resource share can be shared with both accounts in the resource directory and accounts outside the resource directory.
         self.allow_external_targets = allow_external_targets  # type: bool
-        # The time when the resource share was created.
-        self.create_time = create_time  # type: str
-        # The ID of the resource share.
-        self.resource_share_id = resource_share_id  # type: str
-        # The name of the resource share.
-        self.resource_share_name = resource_share_name  # type: str
-        # The owner of the resource share.
-        self.resource_share_owner = resource_share_owner  # type: str
         # The status of the resource share. Valid values:
         # 
         # *   Active: The resource share is enabled.
         # *   Pending: The resource share is associated with one or more resource sharing invitations that are waiting for confirmation.
         # *   Deleting: The resource share is being deleted.
         # *   Deleted: The resource share is deleted.
         # 
         # >  The system deletes the records of resource shares in the Deleted state within 48 hours to 96 hours after you delete the resource shares.
+        self.create_time = create_time  # type: str
+        # Indicates whether resources in the resource share can be shared with accounts outside the resource directory. Valid values:
+        # 
+        # *   false: Resources in the resource share can be shared only with accounts in the resource directory.
+        # *   true: Resources in the resource share can be shared with both accounts in the resource directory and accounts outside the resource directory.
+        self.resource_share_id = resource_share_id  # type: str
+        # The time when the resource share was created.
+        self.resource_share_name = resource_share_name  # type: str
+        # The ID of the resource share.
+        self.resource_share_owner = resource_share_owner  # type: str
         self.resource_share_status = resource_share_status  # type: str
-        # The time when the resource share was updated.
+        # The owner of the resource share.
         self.update_time = update_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateResourceShareResponseBodyResourceShare, self).to_map()
@@ -717,17 +691,17 @@
         if m.get('UpdateTime') is not None:
             self.update_time = m.get('UpdateTime')
         return self
 
 
 class CreateResourceShareResponseBody(TeaModel):
     def __init__(self, request_id=None, resource_share=None):
-        # The ID of the request.
+        # The time when the resource share was updated.
         self.request_id = request_id  # type: str
-        # The information of the resource share.
+        # The name of the resource share.
         self.resource_share = resource_share  # type: CreateResourceShareResponseBodyResourceShare
 
     def validate(self):
         if self.resource_share:
             self.resource_share.validate()
 
     def to_map(self):
@@ -789,15 +763,14 @@
             temp_model = CreateResourceShareResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteResourceShareRequest(TeaModel):
     def __init__(self, resource_share_id=None):
-        # The ID of the resource share.
         self.resource_share_id = resource_share_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteResourceShareRequest, self).to_map()
@@ -814,15 +787,14 @@
         if m.get('ResourceShareId') is not None:
             self.resource_share_id = m.get('ResourceShareId')
         return self
 
 
 class DeleteResourceShareResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteResourceShareResponseBody, self).to_map()
@@ -1021,27 +993,22 @@
             temp_model = DescribeRegionsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DisassociateResourceShareRequestResources(TeaModel):
     def __init__(self, resource_id=None, resource_type=None):
-        # The ID of a shared resource.
-        # 
-        # Valid values of N: 1 to 5. This indicates that a maximum of five shared resources can be specified at a time.
+        # The owner of the resource share. Valid values:
         # 
-        # >  Resources.N.ResourceId and Resources.N.ResourceType must be used in pairs.
+        # *   Self: The resource share belongs to the current account. This is the default value. If you are the management account or a member of a resource directory and you want to remove resources or principals from a resource share, set this parameter to Self.
+        # *   OtherAccounts: The resource share belongs to another account. If you are not the management account or a member of a resource directory and you want to exit a resource share, set this parameter to OtherAccounts.
         self.resource_id = resource_id  # type: str
-        # The type of a shared resource.
-        # 
-        # Valid values of N: 1 to 5. This indicates that a maximum of five shared resources can be specified at a time.
+        # The ID of a principal.
         # 
-        # For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
-        # 
-        # >  Resources.N.ResourceId and Resources.N.ResourceType must be used in pairs.
+        # Valid values of N: 1 to 5. This indicates that a maximum of five principals can be specified at a time.
         self.resource_type = resource_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DisassociateResourceShareRequestResources, self).to_map()
@@ -1062,20 +1029,21 @@
         if m.get('ResourceType') is not None:
             self.resource_type = m.get('ResourceType')
         return self
 
 
 class DisassociateResourceShareRequest(TeaModel):
     def __init__(self, resource_owner=None, resource_share_id=None, resources=None, targets=None):
-        # The owner of the resource share. Valid values:
-        # 
-        # *   Self: The resource share belongs to the current account. This is the default value. If you are the management account or a member of a resource directory and you want to remove resources or principals from a resource share, set this parameter to Self.
-        # *   OtherAccounts: The resource share belongs to another account. If you are not the management account or a member of a resource directory and you want to exit a resource share, set this parameter to OtherAccounts.
+        # The information of the entities that are associated with the resource share.
         self.resource_owner = resource_owner  # type: str
-        # The ID of the resource share.
+        # The ID of a shared resource.
+        # 
+        # Valid values of N: 1 to 5. This indicates that a maximum of five shared resources can be specified at a time.
+        # 
+        # >  Resources.N.ResourceId and Resources.N.ResourceType must be used in pairs.
         self.resource_share_id = resource_share_id  # type: str
         self.resources = resources  # type: list[DisassociateResourceShareRequestResources]
         self.targets = targets  # type: list[str]
 
     def validate(self):
         if self.resources:
             for k in self.resources:
@@ -1116,54 +1084,46 @@
         return self
 
 
 class DisassociateResourceShareResponseBodyResourceShareAssociations(TeaModel):
     def __init__(self, association_status=None, association_status_message=None, association_type=None,
                  create_time=None, entity_id=None, entity_type=None, resource_share_id=None, resource_share_name=None,
                  update_time=None):
+        self.association_status = association_status  # type: str
         # The association status. Valid values:
         # 
         # *   Associating: The entity is being associated.
         # *   Associated: The entity is associated.
         # *   Failed: The entity fails to be associated.
         # *   Disassociating: The entity is being disassociated.
         # *   Disassociated: The entity is disassociated.
         # 
         # >  The system deletes the records of entities in the `Failed` or `Disassociated` state within 48 hours to 96 hours.
-        self.association_status = association_status  # type: str
-        # The cause of the disassociation failure.
         self.association_status_message = association_status_message  # type: str
-        # The association type. Valid values:
-        # 
-        # *   Resource
-        # *   Target
         self.association_type = association_type  # type: str
+        # The ID of the resource share.
+        self.create_time = create_time  # type: str
         # The time when the disassociation of the entity was performed. The value of this parameter depends on the value of the AssociationType parameter:
         # 
         # *   If the value of `AssociationType` is `Resource`, the value of this parameter is the time when the resource was disassociated from the resource share.
         # *   If the value of `AssociationType` is `Target`, the value of this parameter is the time when the principal was disassociated from the resource share.
-        self.create_time = create_time  # type: str
-        # The ID of the entity. The value of this parameter depends on the value of the AssociationType parameter:
-        # 
-        # *   If the value of `AssociationType` is `Resource`, the value of this parameter is the ID of the resource.
-        # *   If the value of `AssociationType` is `Target`, the value of this parameter is the ID of the resource directory, folder, or member.
         self.entity_id = entity_id  # type: str
+        # The cause of the disassociation failure.
+        self.entity_type = entity_type  # type: str
+        # The association type. Valid values:
+        # 
+        # *   Resource
+        # *   Target
+        self.resource_share_id = resource_share_id  # type: str
         # The type of the entity. The value of this parameter depends on the value of the AssociationType parameter:
         # 
         # *   If the value of AssociationType is Resource, the value of this parameter is the type of the resource. For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
         # *   If the value of AssociationType is Target, the value of this parameter is Account.
-        self.entity_type = entity_type  # type: str
-        # The ID of the resource share.
-        self.resource_share_id = resource_share_id  # type: str
-        # The name of the resource share.
         self.resource_share_name = resource_share_name  # type: str
-        # The time when the disassociation of the entity was updated. The value of this parameter depends on the value of the AssociationType parameter:
-        # 
-        # *   If the value of `AssociationType` is `Resource`, the value of this parameter is the time when the disassociation of the resource was updated.
-        # *   If the value of `AssociationType` is `Target`, the value of this parameter is the time when the disassociation of the principal was updated.
+        # The name of the resource share.
         self.update_time = update_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DisassociateResourceShareResponseBodyResourceShareAssociations, self).to_map()
@@ -1212,17 +1172,23 @@
         if m.get('UpdateTime') is not None:
             self.update_time = m.get('UpdateTime')
         return self
 
 
 class DisassociateResourceShareResponseBody(TeaModel):
     def __init__(self, request_id=None, resource_share_associations=None):
-        # The ID of the request.
+        # The time when the disassociation of the entity was updated. The value of this parameter depends on the value of the AssociationType parameter:
+        # 
+        # *   If the value of `AssociationType` is `Resource`, the value of this parameter is the time when the disassociation of the resource was updated.
+        # *   If the value of `AssociationType` is `Target`, the value of this parameter is the time when the disassociation of the principal was updated.
         self.request_id = request_id  # type: str
-        # The information of the entities that are associated with the resource share.
+        # The ID of the entity. The value of this parameter depends on the value of the AssociationType parameter:
+        # 
+        # *   If the value of `AssociationType` is `Resource`, the value of this parameter is the ID of the resource.
+        # *   If the value of `AssociationType` is `Target`, the value of this parameter is the ID of the resource directory, folder, or member.
         self.resource_share_associations = resource_share_associations  # type: list[DisassociateResourceShareResponseBodyResourceShareAssociations]
 
     def validate(self):
         if self.resource_share_associations:
             for k in self.resource_share_associations:
                 if k:
                     k.validate()
@@ -1290,17 +1256,17 @@
             temp_model = DisassociateResourceShareResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DisassociateResourceSharePermissionRequest(TeaModel):
     def __init__(self, permission_name=None, resource_share_id=None):
-        # The name of the permission. For more information, see [Permission library](~~465474~~).
+        # The ID of the request.
         self.permission_name = permission_name  # type: str
-        # The ID of the resource share.
+        # The name of the permission. For more information, see [Permission library](~~465474~~).
         self.resource_share_id = resource_share_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DisassociateResourceSharePermissionRequest, self).to_map()
@@ -1321,15 +1287,14 @@
         if m.get('ResourceShareId') is not None:
             self.resource_share_id = m.get('ResourceShareId')
         return self
 
 
 class DisassociateResourceSharePermissionResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DisassociateResourceSharePermissionResponseBody, self).to_map()
@@ -1385,15 +1350,14 @@
             temp_model = DisassociateResourceSharePermissionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class EnableSharingWithResourceDirectoryResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(EnableSharingWithResourceDirectoryResponseBody, self).to_map()
@@ -1481,37 +1445,31 @@
             self.permission_version = m.get('PermissionVersion')
         return self
 
 
 class GetPermissionResponseBodyPermission(TeaModel):
     def __init__(self, create_time=None, default_permission=None, default_version=None, permission=None,
                  permission_name=None, permission_version=None, resource_type=None, update_time=None):
-        # The creation time.
         self.create_time = create_time  # type: str
-        # Indicates whether the permission is the default permission. Valid values:
-        # 
-        # *   false: The permission is not the default permission.
-        # *   true: The permission is the default permission.
         self.default_permission = default_permission  # type: bool
+        self.default_version = default_version  # type: bool
+        # The update time.
+        self.permission = permission  # type: str
         # Indicates whether the version is the default version. Valid values:
         # 
         # *   false: The version is not the default version.
         # *   true: The version is the default version.
-        self.default_version = default_version  # type: bool
-        # The document of the policy related to the permission.
-        self.permission = permission  # type: str
-        # The name of the permission.
         self.permission_name = permission_name  # type: str
-        # The version of the permission.
+        # The creation time.
         self.permission_version = permission_version  # type: str
-        # The type of the shared resources.
+        # Indicates whether the permission is the default permission. Valid values:
         # 
-        # For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
+        # *   false: The permission is not the default permission.
+        # *   true: The permission is the default permission.
         self.resource_type = resource_type  # type: str
-        # The update time.
         self.update_time = update_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetPermissionResponseBodyPermission, self).to_map()
@@ -1556,17 +1514,19 @@
         if m.get('UpdateTime') is not None:
             self.update_time = m.get('UpdateTime')
         return self
 
 
 class GetPermissionResponseBody(TeaModel):
     def __init__(self, permission=None, request_id=None):
-        # The information about the permission.
+        # The type of the shared resources.
+        # 
+        # For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
         self.permission = permission  # type: GetPermissionResponseBodyPermission
-        # The ID of the request.
+        # The document of the policy related to the permission.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.permission:
             self.permission.validate()
 
     def to_map(self):
@@ -1628,21 +1588,19 @@
             temp_model = GetPermissionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListPermissionVersionsRequest(TeaModel):
     def __init__(self, max_results=None, next_token=None, permission_name=None):
-        # The maximum number of entries to return for a single request.
-        # 
-        # Valid values: 1 to 100. Default value: 20.
+        # The information about the permission.
         self.max_results = max_results  # type: int
-        # The `token` that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
-        self.next_token = next_token  # type: str
         # The name of the permission.
+        self.next_token = next_token  # type: str
+        # The ID of the request.
         self.permission_name = permission_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListPermissionVersionsRequest, self).to_map()
@@ -1668,35 +1626,28 @@
             self.permission_name = m.get('PermissionName')
         return self
 
 
 class ListPermissionVersionsResponseBodyPermissions(TeaModel):
     def __init__(self, create_time=None, default_permission=None, default_version=None, permission_name=None,
                  permission_version=None, resource_type=None, update_time=None):
-        # The creation time.
         self.create_time = create_time  # type: str
+        self.default_permission = default_permission  # type: bool
         # Indicates whether the permission is the default permission. Valid values:
         # 
         # *   false: The permission is not the default permission.
         # *   true: The permission is the default permission.
-        self.default_permission = default_permission  # type: bool
-        # Indicates whether the version is the default version. Valid values:
-        # 
-        # *   false: The version is not the default version.
-        # *   true: The version is the default version.
         self.default_version = default_version  # type: bool
-        # The name of the permission.
+        # The update time.
         self.permission_name = permission_name  # type: str
-        # The version of the permission.
-        self.permission_version = permission_version  # type: str
         # The type of the shared resources.
         # 
         # For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
+        self.permission_version = permission_version  # type: str
         self.resource_type = resource_type  # type: str
-        # The update time.
         self.update_time = update_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListPermissionVersionsResponseBodyPermissions, self).to_map()
@@ -1737,19 +1688,22 @@
         if m.get('UpdateTime') is not None:
             self.update_time = m.get('UpdateTime')
         return self
 
 
 class ListPermissionVersionsResponseBody(TeaModel):
     def __init__(self, next_token=None, permissions=None, request_id=None):
-        # The token that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
+        # The version of the permission.
         self.next_token = next_token  # type: str
-        # The information about the permission.
+        # The creation time.
         self.permissions = permissions  # type: list[ListPermissionVersionsResponseBodyPermissions]
-        # The ID of the request.
+        # Indicates whether the version is the default version. Valid values:
+        # 
+        # *   false: The version is not the default version.
+        # *   true: The version is the default version.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.permissions:
             for k in self.permissions:
                 if k:
                     k.validate()
@@ -1821,23 +1775,19 @@
             temp_model = ListPermissionVersionsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListPermissionsRequest(TeaModel):
     def __init__(self, max_results=None, next_token=None, resource_type=None):
-        # The maximum number of entries to return for a single request.
-        # 
-        # Valid values: 1 to 100. Default value: 20.
+        # The information about the permission.
         self.max_results = max_results  # type: int
-        # The `token` that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
+        # The name of the permission.
         self.next_token = next_token  # type: str
-        # The type of the shared resources.
-        # 
-        # For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
+        # The ID of the request.
         self.resource_type = resource_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListPermissionsRequest, self).to_map()
@@ -1863,35 +1813,28 @@
             self.resource_type = m.get('ResourceType')
         return self
 
 
 class ListPermissionsResponseBodyPermissions(TeaModel):
     def __init__(self, create_time=None, default_permission=None, default_version=None, permission_name=None,
                  permission_version=None, resource_type=None, update_time=None):
-        # The creation time.
         self.create_time = create_time  # type: str
+        self.default_permission = default_permission  # type: bool
         # Indicates whether the permission is the default permission. Valid values:
         # 
         # *   false: The permission is not the default permission.
         # *   true: The permission is the default permission.
-        self.default_permission = default_permission  # type: bool
-        # Indicates whether the version is the default version. Valid values:
-        # 
-        # *   false: The version is not the default version.
-        # *   true: The version is the default version.
         self.default_version = default_version  # type: bool
-        # The name of the permission.
+        # The update time.
         self.permission_name = permission_name  # type: str
-        # The version of the permission.
-        self.permission_version = permission_version  # type: str
         # The type of the shared resources.
         # 
         # For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
+        self.permission_version = permission_version  # type: str
         self.resource_type = resource_type  # type: str
-        # The update time.
         self.update_time = update_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListPermissionsResponseBodyPermissions, self).to_map()
@@ -1932,19 +1875,22 @@
         if m.get('UpdateTime') is not None:
             self.update_time = m.get('UpdateTime')
         return self
 
 
 class ListPermissionsResponseBody(TeaModel):
     def __init__(self, next_token=None, permissions=None, request_id=None):
-        # The token that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
+        # The version of the permission.
         self.next_token = next_token  # type: str
-        # The information about the permission.
+        # The creation time.
         self.permissions = permissions  # type: list[ListPermissionsResponseBodyPermissions]
-        # The ID of the request.
+        # Indicates whether the version is the default version. Valid values:
+        # 
+        # *   false: The version is not the default version.
+        # *   true: The version is the default version.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.permissions:
             for k in self.permissions:
                 if k:
                     k.validate()
@@ -2286,17 +2232,15 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListResourceShareInvitationsRequest(TeaModel):
     def __init__(self, max_results=None, next_token=None, resource_share_ids=None,
                  resource_share_invitation_ids=None):
-        # The maximum number of entries to return for a single request.
-        # 
-        # Valid values: 1 to 100. Default value: 20.
+        # The IDs of the resource sharing invitations.
         self.max_results = max_results  # type: int
         # The `token` that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
         self.next_token = next_token  # type: str
         self.resource_share_ids = resource_share_ids  # type: list[str]
         self.resource_share_invitation_ids = resource_share_invitation_ids  # type: list[str]
 
     def validate(self):
@@ -2330,33 +2274,24 @@
             self.resource_share_invitation_ids = m.get('ResourceShareInvitationIds')
         return self
 
 
 class ListResourceShareInvitationsResponseBodyResourceShareInvitations(TeaModel):
     def __init__(self, create_time=None, receiver_account_id=None, resource_share_id=None,
                  resource_share_invitation_id=None, resource_share_name=None, sender_account_id=None, status=None):
-        # The time when the invitation was created. The time is displayed in UTC.
+        # The Alibaba Cloud account ID of the inviter.
         self.create_time = create_time  # type: str
-        # The Alibaba Cloud account ID of the invitee.
         self.receiver_account_id = receiver_account_id  # type: str
-        # The ID of the resource share.
+        # The Alibaba Cloud account ID of the invitee.
         self.resource_share_id = resource_share_id  # type: str
-        # The ID of the invitation.
         self.resource_share_invitation_id = resource_share_invitation_id  # type: str
-        # The name of the resource share.
+        # The ID of the invitation.
         self.resource_share_name = resource_share_name  # type: str
-        # The Alibaba Cloud account ID of the inviter.
         self.sender_account_id = sender_account_id  # type: str
-        # The status of the invitation. Valid values:
-        # 
-        # *   Pending: The invitation is waiting for confirmation.
-        # *   Accepted: The invitation is accepted.
-        # *   Cancelled: The invitation is canceled.
-        # *   Rejected: The invitation is rejected.
-        # *   Expired: The invitation has expired.
+        # The name of the resource share.
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListResourceShareInvitationsResponseBodyResourceShareInvitations, self).to_map()
@@ -2397,19 +2332,25 @@
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
 
 
 class ListResourceShareInvitationsResponseBody(TeaModel):
     def __init__(self, next_token=None, request_id=None, resource_share_invitations=None):
-        # The `token` that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending: The invitation is waiting for confirmation.
+        # *   Accepted: The invitation is accepted.
+        # *   Cancelled: The invitation is canceled.
+        # *   Rejected: The invitation is rejected.
+        # *   Expired: The invitation has expired.
         self.next_token = next_token  # type: str
-        # The ID of the request.
+        # The time when the invitation was created. The time is displayed in UTC.
         self.request_id = request_id  # type: str
-        # The information of the resource sharing invitations.
+        # The ID of the resource share.
         self.resource_share_invitations = resource_share_invitations  # type: list[ListResourceShareInvitationsResponseBodyResourceShareInvitations]
 
     def validate(self):
         if self.resource_share_invitations:
             for k in self.resource_share_invitations:
                 if k:
                     k.validate()
@@ -2481,26 +2422,21 @@
             temp_model = ListResourceShareInvitationsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListResourceSharePermissionsRequest(TeaModel):
     def __init__(self, max_results=None, next_token=None, resource_owner=None, resource_share_id=None):
-        # The maximum number of entries to return for a single request.
-        # 
-        # Valid values: 1 to 100. Default value: 20.
+        # The ID of the request.
         self.max_results = max_results  # type: int
-        # The `token` that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
+        # The information about the permissions.
         self.next_token = next_token  # type: str
-        # The owner of the resource share. Valid values:
-        # 
-        # *   Self: the current account
-        # *   OtherAccounts: an account other than the current account
+        # The name of the permission.
         self.resource_owner = resource_owner  # type: str
-        # The ID of the resource share.
+        # The `token` that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
         self.resource_share_id = resource_share_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListResourceSharePermissionsRequest, self).to_map()
@@ -2530,35 +2466,28 @@
             self.resource_share_id = m.get('ResourceShareId')
         return self
 
 
 class ListResourceSharePermissionsResponseBodyPermissions(TeaModel):
     def __init__(self, create_time=None, default_permission=None, default_version=None, permission_name=None,
                  permission_version=None, resource_type=None, update_time=None):
-        # The creation time.
         self.create_time = create_time  # type: str
+        self.default_permission = default_permission  # type: bool
         # Indicates whether the permission is the default permission. Valid values:
         # 
         # *   false: The permission is not the default permission.
         # *   true: The permission is the default permission.
-        self.default_permission = default_permission  # type: bool
-        # Indicates whether the version is the default version. Valid values:
-        # 
-        # *   false: The version is not the default version.
-        # *   true: The version is the default version.
         self.default_version = default_version  # type: bool
-        # The name of the permission.
+        # The update time.
         self.permission_name = permission_name  # type: str
-        # The version of the permission.
-        self.permission_version = permission_version  # type: str
         # The type of the shared resources.
         # 
         # For more information about the types of resources that can be shared, see [Services that work with Resource Sharing](~~450526~~).
+        self.permission_version = permission_version  # type: str
         self.resource_type = resource_type  # type: str
-        # The update time.
         self.update_time = update_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListResourceSharePermissionsResponseBodyPermissions, self).to_map()
@@ -2599,19 +2528,22 @@
         if m.get('UpdateTime') is not None:
             self.update_time = m.get('UpdateTime')
         return self
 
 
 class ListResourceSharePermissionsResponseBody(TeaModel):
     def __init__(self, next_token=None, permissions=None, request_id=None):
-        # The `token` that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
+        # The version of the permission.
         self.next_token = next_token  # type: str
-        # The information about the permissions.
+        # The creation time.
         self.permissions = permissions  # type: list[ListResourceSharePermissionsResponseBodyPermissions]
-        # The ID of the request.
+        # Indicates whether the version is the default version. Valid values:
+        # 
+        # *   false: The version is not the default version.
+        # *   true: The version is the default version.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.permissions:
             for k in self.permissions:
                 if k:
                     k.validate()
@@ -2682,41 +2614,37 @@
         if m.get('body') is not None:
             temp_model = ListResourceSharePermissionsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListResourceSharesRequest(TeaModel):
-    def __init__(self, max_results=None, next_token=None, permission_name=None, resource_group_id=None,
-                 resource_owner=None, resource_share_ids=None, resource_share_name=None, resource_share_status=None):
-        # The maximum number of entries to return for a single request.
-        # 
-        # Valid values: 1 to 100. Default value: 20.
+    def __init__(self, max_results=None, next_token=None, permission_name=None, resource_owner=None,
+                 resource_share_ids=None, resource_share_name=None, resource_share_status=None):
+        # The ID of a resource share.
         self.max_results = max_results  # type: int
-        # The `token` that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
-        self.next_token = next_token  # type: str
         # The name of the permission. For more information, see [Permission library](~~465474~~).
+        self.next_token = next_token  # type: str
+        # The ID of the request.
         self.permission_name = permission_name  # type: str
-        self.resource_group_id = resource_group_id  # type: str
-        # The owner of the resource shares. Valid values:
-        # 
-        # *   Self: the current account
-        # *   OtherAccounts: an account other than the current account
-        self.resource_owner = resource_owner  # type: str
-        self.resource_share_ids = resource_share_ids  # type: list[str]
-        # The name of the resource share.
-        self.resource_share_name = resource_share_name  # type: str
         # The status of the resource share. Valid values:
         # 
         # *   Active: The resource share is enabled.
         # *   Pending: The resource share is associated with one or more resource sharing invitations that are waiting for confirmation.
         # *   Deleting: The resource share is being deleted.
         # *   Deleted: The resource share is deleted.
         # 
         # >  The system deletes the records of resource shares in the Deleted state within 48 hours to 96 hours after you delete the resource shares.
+        self.resource_owner = resource_owner  # type: str
+        self.resource_share_ids = resource_share_ids  # type: list[str]
+        # The maximum number of entries to return for a single request.
+        # 
+        # Valid values: 1 to 100. Default value: 20.
+        self.resource_share_name = resource_share_name  # type: str
+        # The `token` that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
         self.resource_share_status = resource_share_status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListResourceSharesRequest, self).to_map()
@@ -2726,16 +2654,14 @@
         result = dict()
         if self.max_results is not None:
             result['MaxResults'] = self.max_results
         if self.next_token is not None:
             result['NextToken'] = self.next_token
         if self.permission_name is not None:
             result['PermissionName'] = self.permission_name
-        if self.resource_group_id is not None:
-            result['ResourceGroupId'] = self.resource_group_id
         if self.resource_owner is not None:
             result['ResourceOwner'] = self.resource_owner
         if self.resource_share_ids is not None:
             result['ResourceShareIds'] = self.resource_share_ids
         if self.resource_share_name is not None:
             result['ResourceShareName'] = self.resource_share_name
         if self.resource_share_status is not None:
@@ -2746,55 +2672,49 @@
         m = m or dict()
         if m.get('MaxResults') is not None:
             self.max_results = m.get('MaxResults')
         if m.get('NextToken') is not None:
             self.next_token = m.get('NextToken')
         if m.get('PermissionName') is not None:
             self.permission_name = m.get('PermissionName')
-        if m.get('ResourceGroupId') is not None:
-            self.resource_group_id = m.get('ResourceGroupId')
         if m.get('ResourceOwner') is not None:
             self.resource_owner = m.get('ResourceOwner')
         if m.get('ResourceShareIds') is not None:
             self.resource_share_ids = m.get('ResourceShareIds')
         if m.get('ResourceShareName') is not None:
             self.resource_share_name = m.get('ResourceShareName')
         if m.get('ResourceShareStatus') is not None:
             self.resource_share_status = m.get('ResourceShareStatus')
         return self
 
 
 class ListResourceSharesResponseBodyResourceShares(TeaModel):
-    def __init__(self, allow_external_targets=None, create_time=None, resource_group_id=None,
-                 resource_share_id=None, resource_share_name=None, resource_share_owner=None, resource_share_status=None,
-                 update_time=None):
-        # Indicates whether resources in the resource share can be shared with accounts outside the resource directory. Valid values:
-        # 
-        # *   false: Resources in the resource share can be shared only with accounts in the resource directory.
-        # *   true: Resources in the resource share can be shared with both accounts in the resource directory and accounts outside the resource directory.
+    def __init__(self, allow_external_targets=None, create_time=None, resource_share_id=None,
+                 resource_share_name=None, resource_share_owner=None, resource_share_status=None, update_time=None):
         self.allow_external_targets = allow_external_targets  # type: bool
-        # The time when the resource share was created.
-        self.create_time = create_time  # type: str
-        self.resource_group_id = resource_group_id  # type: str
-        # The ID of the resource share.
-        self.resource_share_id = resource_share_id  # type: str
-        # The name of the resource share.
-        self.resource_share_name = resource_share_name  # type: str
-        # The owner of the resource share.
-        self.resource_share_owner = resource_share_owner  # type: str
         # The status of the resource share. Valid values:
         # 
         # *   Active: The resource share is enabled.
         # *   Pending: The resource share is associated with one or more resource sharing invitations that are waiting for confirmation.
         # *   Deleting: The resource share is being deleted.
         # *   Deleted: The resource share is deleted.
         # 
         # >  The system deletes the records of resource shares in the Deleted state within 48 hours to 96 hours after you delete the resource shares.
+        self.create_time = create_time  # type: str
+        # Indicates whether resources in the resource share can be shared with accounts outside the resource directory. Valid values:
+        # 
+        # *   false: Resources in the resource share can be shared only with accounts in the resource directory.
+        # *   true: Resources in the resource share can be shared with both accounts in the resource directory and accounts outside the resource directory.
+        self.resource_share_id = resource_share_id  # type: str
+        # The time when the resource share was created.
+        self.resource_share_name = resource_share_name  # type: str
+        # The ID of the resource share.
+        self.resource_share_owner = resource_share_owner  # type: str
         self.resource_share_status = resource_share_status  # type: str
-        # The time when the resource share was updated.
+        # The owner of the resource share.
         self.update_time = update_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListResourceSharesResponseBodyResourceShares, self).to_map()
@@ -2802,16 +2722,14 @@
             return _map
 
         result = dict()
         if self.allow_external_targets is not None:
             result['AllowExternalTargets'] = self.allow_external_targets
         if self.create_time is not None:
             result['CreateTime'] = self.create_time
-        if self.resource_group_id is not None:
-            result['ResourceGroupId'] = self.resource_group_id
         if self.resource_share_id is not None:
             result['ResourceShareId'] = self.resource_share_id
         if self.resource_share_name is not None:
             result['ResourceShareName'] = self.resource_share_name
         if self.resource_share_owner is not None:
             result['ResourceShareOwner'] = self.resource_share_owner
         if self.resource_share_status is not None:
@@ -2822,16 +2740,14 @@
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('AllowExternalTargets') is not None:
             self.allow_external_targets = m.get('AllowExternalTargets')
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
-        if m.get('ResourceGroupId') is not None:
-            self.resource_group_id = m.get('ResourceGroupId')
         if m.get('ResourceShareId') is not None:
             self.resource_share_id = m.get('ResourceShareId')
         if m.get('ResourceShareName') is not None:
             self.resource_share_name = m.get('ResourceShareName')
         if m.get('ResourceShareOwner') is not None:
             self.resource_share_owner = m.get('ResourceShareOwner')
         if m.get('ResourceShareStatus') is not None:
@@ -2839,19 +2755,19 @@
         if m.get('UpdateTime') is not None:
             self.update_time = m.get('UpdateTime')
         return self
 
 
 class ListResourceSharesResponseBody(TeaModel):
     def __init__(self, next_token=None, request_id=None, resource_shares=None):
-        # The `token` that is used to initiate the next request. If the response of the current request is truncated, you can use the token to initiate another request and obtain the remaining records.
+        # The information of the resource shares.
         self.next_token = next_token  # type: str
-        # The ID of the request.
+        # The time when the resource share was updated.
         self.request_id = request_id  # type: str
-        # The information of the resource shares.
+        # The name of the resource share.
         self.resource_shares = resource_shares  # type: list[ListResourceSharesResponseBodyResourceShares]
 
     def validate(self):
         if self.resource_shares:
             for k in self.resource_shares:
                 if k:
                     k.validate()
@@ -3354,17 +3270,15 @@
             temp_model = ListSharedTargetsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RejectResourceShareInvitationRequest(TeaModel):
     def __init__(self, resource_share_invitation_id=None):
-        # The ID of the resource sharing invitation.
-        # 
-        # You can call the [ListResourceShareInvitations](~~450564~~) operation to obtain the ID of a resource sharing invitation.
+        # The ID of the invitation.
         self.resource_share_invitation_id = resource_share_invitation_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RejectResourceShareInvitationRequest, self).to_map()
@@ -3382,33 +3296,30 @@
             self.resource_share_invitation_id = m.get('ResourceShareInvitationId')
         return self
 
 
 class RejectResourceShareInvitationResponseBodyResourceShareInvitation(TeaModel):
     def __init__(self, create_time=None, receiver_account_id=None, resource_share_id=None,
                  resource_share_invitation_id=None, resource_share_name=None, sender_account_id=None, status=None):
-        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time  # type: str
-        # The Alibaba Cloud account ID of the invitee.
         self.receiver_account_id = receiver_account_id  # type: str
-        # The ID of the resource share.
+        # The Alibaba Cloud account ID of the invitee.
         self.resource_share_id = resource_share_id  # type: str
-        # The ID of the invitation.
+        # The Alibaba Cloud account ID of the inviter.
         self.resource_share_invitation_id = resource_share_invitation_id  # type: str
-        # The name of the resource share.
+        # The time when the invitation was created. The time is displayed in UTC.
         self.resource_share_name = resource_share_name  # type: str
-        # The Alibaba Cloud account ID of the inviter.
-        self.sender_account_id = sender_account_id  # type: str
         # The status of the invitation. Valid values:
         # 
         # *   Pending: The invitation is waiting for confirmation.
         # *   Accepted: The invitation is accepted.
         # *   Cancelled: The invitation is canceled.
         # *   Rejected: The invitation is rejected.
         # *   Expired: The invitation has expired.
+        self.sender_account_id = sender_account_id  # type: str
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RejectResourceShareInvitationResponseBodyResourceShareInvitation, self).to_map()
@@ -3449,17 +3360,17 @@
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
 
 
 class RejectResourceShareInvitationResponseBody(TeaModel):
     def __init__(self, request_id=None, resource_share_invitation=None):
-        # The ID of the request.
+        # The ID of the resource share.
         self.request_id = request_id  # type: str
-        # The information of the resource sharing invitation.
+        # The name of the resource share.
         self.resource_share_invitation = resource_share_invitation  # type: RejectResourceShareInvitationResponseBodyResourceShareInvitation
 
     def validate(self):
         if self.resource_share_invitation:
             self.resource_share_invitation.validate()
 
     def to_map(self):
@@ -3521,26 +3432,22 @@
             temp_model = RejectResourceShareInvitationResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateResourceShareRequest(TeaModel):
     def __init__(self, allow_external_targets=None, resource_share_id=None, resource_share_name=None):
+        # The information of the resource share.
+        self.allow_external_targets = allow_external_targets  # type: bool
         # Specifies whether resources in the resource share can be shared with accounts outside the resource directory. Valid values:
         # 
         # *   false: Resources in the resource share can be shared only with accounts in the resource directory.
         # *   true: Resources in the resource share can be shared with both accounts in the resource directory and accounts outside the resource directory.
-        self.allow_external_targets = allow_external_targets  # type: bool
-        # The ID of the resource share.
         self.resource_share_id = resource_share_id  # type: str
-        # The new name of the resource share.
-        # 
-        # The name must be 1 to 50 characters in length.
-        # 
-        # The name can contain letters, digits, periods (.), underscores (\_), and hyphens (-).
+        # The ID of the request.
         self.resource_share_name = resource_share_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateResourceShareRequest, self).to_map()
@@ -3566,37 +3473,35 @@
             self.resource_share_name = m.get('ResourceShareName')
         return self
 
 
 class UpdateResourceShareResponseBodyResourceShare(TeaModel):
     def __init__(self, allow_external_targets=None, create_time=None, resource_share_id=None,
                  resource_share_name=None, resource_share_owner=None, resource_share_status=None, update_time=None):
-        # Indicates whether resources in the resource share can be shared with accounts outside the resource directory. Valid values:
-        # 
-        # *   false: Resources in the resource share can be shared only with accounts in the resource directory.
-        # *   true: Resources in the resource share can be shared with both accounts in the resource directory and accounts outside the resource directory.
         self.allow_external_targets = allow_external_targets  # type: bool
-        # The time when the resource share was created.
-        self.create_time = create_time  # type: str
-        # The ID of the resource share.
-        self.resource_share_id = resource_share_id  # type: str
-        # The name of the resource share.
-        self.resource_share_name = resource_share_name  # type: str
-        # The owner of the resource share.
-        self.resource_share_owner = resource_share_owner  # type: str
         # The status of the resource share. Valid values:
         # 
         # *   Active: The resource share is enabled.
         # *   Pending: The resource share is associated with one or more resource sharing invitations that are waiting for confirmation.
         # *   Deleting: The resource share is being deleted.
         # *   Deleted: The resource share is deleted.
         # 
         # >  The system deletes the records of resource shares in the Deleted state within 48 hours to 96 hours after you delete the resource shares.
+        self.create_time = create_time  # type: str
+        # Indicates whether resources in the resource share can be shared with accounts outside the resource directory. Valid values:
+        # 
+        # *   false: Resources in the resource share can be shared only with accounts in the resource directory.
+        # *   true: Resources in the resource share can be shared with both accounts in the resource directory and accounts outside the resource directory.
+        self.resource_share_id = resource_share_id  # type: str
+        # The time when the resource share was created.
+        self.resource_share_name = resource_share_name  # type: str
+        # The ID of the resource share.
+        self.resource_share_owner = resource_share_owner  # type: str
         self.resource_share_status = resource_share_status  # type: str
-        # The time when the resource share was updated.
+        # The owner of the resource share.
         self.update_time = update_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateResourceShareResponseBodyResourceShare, self).to_map()
@@ -3637,17 +3542,17 @@
         if m.get('UpdateTime') is not None:
             self.update_time = m.get('UpdateTime')
         return self
 
 
 class UpdateResourceShareResponseBody(TeaModel):
     def __init__(self, request_id=None, resource_share=None):
-        # The ID of the request.
+        # The time when the resource share was updated.
         self.request_id = request_id  # type: str
-        # The information of the resource share.
+        # The name of the resource share.
         self.resource_share = resource_share  # type: UpdateResourceShareResponseBodyResourceShare
 
     def validate(self):
         if self.resource_share:
             self.resource_share.validate()
 
     def to_map(self):
```

### Comparing `alibabacloud_resourcesharing20200110_py2-1.0.0/alibabacloud_resourcesharing20200110_py2.egg-info/PKG-INFO` & `alibabacloud_resourcesharing20200110_py2-1.0.1/alibabacloud_resourcesharing20200110_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-resourcesharing20200110-py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud ResourceSharing (20200110) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcesharing20200110_py2-1.0.0/setup.py` & `alibabacloud_resourcesharing20200110_py2-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_resourcesharing20200110_py2.
 
-Created on 08/03/2023
+Created on 18/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_resourcesharing20200110"
 NAME = "alibabacloud_resourcesharing20200110_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ResourceSharing (20200110) SDK Library for Python2"
```

