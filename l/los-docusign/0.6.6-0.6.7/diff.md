# Comparing `tmp/los_docusign-0.6.6.tar.gz` & `tmp/los_docusign-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "los_docusign-0.6.6.tar", max compression
+gzip compressed data, was "los_docusign-0.6.7.tar", max compression
```

## Comparing `los_docusign-0.6.6.tar` & `los_docusign-0.6.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1571 2022-02-09 21:29:17.720800 los_docusign-0.6.6/LICENSE
--rw-r--r--   0        0        0     3650 2022-03-21 11:49:57.380120 los_docusign-0.6.6/README.md
--rw-r--r--   0        0        0        0 2022-02-09 21:29:17.720971 los_docusign-0.6.6/los_docusign/__init__.py
--rw-r--r--   0        0        0     5794 2023-04-03 18:34:44.502327 los_docusign-0.6.6/los_docusign/admin.py
--rw-r--r--   0        0        0      219 2022-02-09 21:29:17.721103 los_docusign-0.6.6/los_docusign/apps.py
--rw-r--r--   0        0        0      401 2022-02-09 21:29:17.721157 los_docusign-0.6.6/los_docusign/asgi.py
--rw-r--r--   0        0        0    17806 2022-02-09 21:29:17.721263 los_docusign-0.6.6/los_docusign/migrations/0001_initial.py
--rw-r--r--   0        0        0     6960 2022-02-09 21:29:17.721334 los_docusign-0.6.6/los_docusign/migrations/0002_auto_20211125_0208.py
--rw-r--r--   0        0        0     2174 2022-02-09 21:29:17.721402 los_docusign-0.6.6/los_docusign/migrations/0003_auto_20211227_1445.py
--rw-r--r--   0        0        0      716 2022-02-09 21:29:17.721456 los_docusign-0.6.6/los_docusign/migrations/0004_auto_20220119_1610.py
--rw-r--r--   0        0        0      582 2022-02-09 21:29:17.721507 los_docusign-0.6.6/los_docusign/migrations/0005_docusignenvelopeauditlog_recipient_details.py
--rw-r--r--   0        0        0      385 2022-03-21 10:17:43.895436 los_docusign-0.6.6/los_docusign/migrations/0006_remove_docusignuserauth_two_factor_enabled_flag.py
--rw-r--r--   0        0        0      485 2023-02-10 16:58:05.166483 los_docusign-0.6.6/los_docusign/migrations/0007_alter_docusignenvelopestagedata_error_message.py
--rw-r--r--   0        0        0     3368 2023-05-05 20:44:43.455719 los_docusign-0.6.6/los_docusign/migrations/0008_auto_20230412_2119.py
--rw-r--r--   0        0        0        0 2022-02-09 21:29:17.721530 los_docusign-0.6.6/los_docusign/migrations/__init__.py
--rw-r--r--   0        0        0    12038 2023-05-05 20:44:43.457031 los_docusign-0.6.6/los_docusign/models.py
--rw-r--r--   0        0        0        0 2022-02-09 21:29:17.721654 los_docusign-0.6.6/los_docusign/tests.py
--rw-r--r--   0        0        0      754 2022-02-09 21:29:17.721713 los_docusign-0.6.6/los_docusign/urls.py
--rw-r--r--   0        0        0     2690 2022-02-09 21:29:17.721801 los_docusign-0.6.6/los_docusign/utils/XmlParser.py
--rw-r--r--   0        0        0      233 2022-02-09 21:29:17.721848 los_docusign-0.6.6/los_docusign/utils/__init__.py
--rw-r--r--   0        0        0     7771 2023-04-12 09:35:46.064826 los_docusign-0.6.6/los_docusign/utils/api_handler.py
--rw-r--r--   0        0        0     9718 2023-04-12 09:35:46.065116 los_docusign-0.6.6/los_docusign/utils/client.py
--rw-r--r--   0        0        0    16929 2023-04-12 09:35:46.065491 los_docusign-0.6.6/los_docusign/utils/docusign_adapter.py
--rw-r--r--   0        0        0    23671 2023-04-12 09:35:46.066247 los_docusign-0.6.6/los_docusign/utils/docusign_helper.py
--rw-r--r--   0        0        0     4652 2022-02-25 19:02:11.957541 los_docusign-0.6.6/los_docusign/utils/validators.py
--rw-r--r--   0        0        0       26 2022-02-09 21:29:17.722208 los_docusign-0.6.6/los_docusign/views.py
--rw-r--r--   0        0        0      401 2022-02-09 21:29:17.722254 los_docusign-0.6.6/los_docusign/wsgi.py
--rw-r--r--   0        0        0     1012 2023-05-05 20:44:43.458238 los_docusign-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     4535 1970-01-01 00:00:00.000000 los_docusign-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1571 2022-02-09 21:29:17.720800 los_docusign-0.6.7/LICENSE
+-rw-r--r--   0        0        0     3650 2022-03-21 11:49:57.380120 los_docusign-0.6.7/README.md
+-rw-r--r--   0        0        0        0 2022-02-09 21:29:17.720971 los_docusign-0.6.7/los_docusign/__init__.py
+-rw-r--r--   0        0        0     6078 2023-05-18 13:06:33.637061 los_docusign-0.6.7/los_docusign/admin.py
+-rw-r--r--   0        0        0      219 2022-02-09 21:29:17.721103 los_docusign-0.6.7/los_docusign/apps.py
+-rw-r--r--   0        0        0      401 2022-02-09 21:29:17.721157 los_docusign-0.6.7/los_docusign/asgi.py
+-rw-r--r--   0        0        0    18782 2023-05-18 13:06:21.959311 los_docusign-0.6.7/los_docusign/migrations/0001_initial.py
+-rw-r--r--   0        0        0     6959 2023-05-18 12:04:41.356126 los_docusign-0.6.7/los_docusign/migrations/0002_auto_20211125_0208.py
+-rw-r--r--   0        0        0     2173 2023-05-18 12:04:41.023588 los_docusign-0.6.7/los_docusign/migrations/0003_auto_20211227_1445.py
+-rw-r--r--   0        0        0      715 2023-05-18 12:04:41.003085 los_docusign-0.6.7/los_docusign/migrations/0004_auto_20220119_1610.py
+-rw-r--r--   0        0        0      581 2023-05-18 12:04:40.982165 los_docusign-0.6.7/los_docusign/migrations/0005_docusignenvelopeauditlog_recipient_details.py
+-rw-r--r--   0        0        0      384 2023-05-18 12:04:40.989549 los_docusign-0.6.7/los_docusign/migrations/0006_remove_docusignuserauth_two_factor_enabled_flag.py
+-rw-r--r--   0        0        0      484 2023-05-18 12:04:40.995327 los_docusign-0.6.7/los_docusign/migrations/0007_alter_docusignenvelopestagedata_error_message.py
+-rw-r--r--   0        0        0     4124 2023-05-18 12:04:41.143904 los_docusign-0.6.7/los_docusign/migrations/0008_auto_20230412_2119.py
+-rw-r--r--   0        0        0        0 2022-02-09 21:29:17.721530 los_docusign-0.6.7/los_docusign/migrations/__init__.py
+-rw-r--r--   0        0        0    12141 2023-05-18 13:10:48.187867 los_docusign-0.6.7/los_docusign/models.py
+-rw-r--r--   0        0        0        0 2022-02-09 21:29:17.721654 los_docusign-0.6.7/los_docusign/tests.py
+-rw-r--r--   0        0        0      754 2022-02-09 21:29:17.721713 los_docusign-0.6.7/los_docusign/urls.py
+-rw-r--r--   0        0        0     2690 2023-05-18 13:01:37.308303 los_docusign-0.6.7/los_docusign/utils/XmlParser.py
+-rw-r--r--   0        0        0      233 2022-02-09 21:29:17.721848 los_docusign-0.6.7/los_docusign/utils/__init__.py
+-rw-r--r--   0        0        0     7956 2023-05-18 13:03:11.879583 los_docusign-0.6.7/los_docusign/utils/api_handler.py
+-rw-r--r--   0        0        0    10336 2023-05-18 13:02:45.202611 los_docusign-0.6.7/los_docusign/utils/client.py
+-rw-r--r--   0        0        0    17898 2023-05-18 14:18:13.516222 los_docusign-0.6.7/los_docusign/utils/docusign_adapter.py
+-rw-r--r--   0        0        0    24198 2023-05-18 13:00:59.193682 los_docusign-0.6.7/los_docusign/utils/docusign_helper.py
+-rw-r--r--   0        0        0     4793 2023-05-18 13:02:55.707475 los_docusign-0.6.7/los_docusign/utils/validators.py
+-rw-r--r--   0        0        0       26 2022-02-09 21:29:17.722208 los_docusign-0.6.7/los_docusign/views.py
+-rw-r--r--   0        0        0      401 2022-02-09 21:29:17.722254 los_docusign-0.6.7/los_docusign/wsgi.py
+-rw-r--r--   0        0        0     1035 2023-05-18 13:46:46.738039 los_docusign-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0     4567 1970-01-01 00:00:00.000000 los_docusign-0.6.7/PKG-INFO
```

### Comparing `los_docusign-0.6.6/LICENSE` & `los_docusign-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `los_docusign-0.6.6/README.md` & `los_docusign-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `los_docusign-0.6.6/los_docusign/admin.py` & `los_docusign-0.6.7/los_docusign/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,52 +35,67 @@
         "modified",
     )
     search_fields = ("envelope_id", "object_pk")
     readonly_fields = ["content_type", "docusign_user"]
 
     def get_actions(self, request):
         # Disable delete
-        actions = super(DocusignEnvelopeStageDataAdmin, self).get_actions(request)
+        actions = super(DocusignEnvelopeStageDataAdmin, self).get_actions(
+            request
+        )
         return actions
 
     actions = ["clear_docusign_throttling_locks", "clear_docusign_app_locks"]
 
     def clear_docusign_throttling_locks(self, request, queryset):
         rate_reset_lock = cache.delete("docusign_rate_reset")
-        self.message_user(request, f"DocuSign Throttling Lock Released: {rate_reset_lock}")
+        self.message_user(
+            request, f"DocuSign Throttling Lock Released: {rate_reset_lock}"
+        )
 
-    clear_docusign_throttling_locks.short_description = "Clear Docusign Throttling Lock"
+    clear_docusign_throttling_locks.short_description = (
+        "Clear Docusign Throttling Lock"
+    )
 
     def clear_docusign_app_locks(self, request, queryset):
         delete_count = 0
         for envelope in queryset.all():
-            envlope_obj = DocusignEnvelopeStageData.objects.get(envelope_id=envelope)
+            envlope_obj = DocusignEnvelopeStageData.objects.get(
+                envelope_id=envelope
+            )
             if cache.delete(f"send_for_docusign:{envlope_obj.object_pk}"):
                 delete_count += 1
         self.message_user(
             request,
             f"{delete_count} successfully released redis locks on applications for docusign.",
         )
 
-    clear_docusign_app_locks.short_description = "Clear Docusign Application Lock"
+    clear_docusign_app_locks.short_description = (
+        "Clear Docusign Application Lock"
+    )
 
     def has_add_permission(self, request):
         return False
 
     def has_delete_permission(self, request, obj=None):
         return False
 
     def has_change_permission(self, request, obj=None):
         return False
 
 
 @admin.register(DocusignOrgTemplate)
 class DocusignOrgTemplateAdmin(admin.ModelAdmin):
     model = DocusignOrgTemplate
-    list_display = ("organization_model", "docusign_template", "created", "modified")
+    list_display = (
+        "organization_model",
+        "docusign_template",
+        "created",
+        "modified",
+    )
     readonly_fields = ["organization_model", "docusign_template"]
     list_filter = (
         "organization_model",
         "docusign_template",
     )
 
     # def has_delete_permission(self, request, obj=None):
@@ -116,15 +131,21 @@
     # def has_delete_permission(self, request, obj=None):
     #     return False
 
 
 @admin.register(DocusignTemplateOrgExclusion)
 class DocusignTemplateOrgExclusionAdmin(admin.ModelAdmin):
     model = DocusignTemplateOrgExclusion
-    list_display = ("organization_model", "document_name", "template", "created", "modified")
+    list_display = (
+        "organization_model",
+        "document_name",
+        "template",
+        "created",
+        "modified",
+    )
     list_filter = ("organization_model", "template")
     readonly_fields = ["organization_model", "document_name", "template"]
 
     # def has_delete_permission(self, request, obj=None):
     #     return False
 
 
@@ -147,23 +168,29 @@
         for org in queryset:
             # loan = EtranLoan.objects.filter(organization_id=org.id).last()
             consent_url = check_docusign_access_token(org)
             if consent_url.get("consent_url", None):
                 print(f"Consent URL: {consent_url}")
                 print(f"Current Path: {request.get_full_path()}")
                 # /admin/
-                request.session["docusign_redirect_path"] = request.get_full_path()
+                request.session[
+                    "docusign_redirect_path"
+                ] = request.get_full_path()
                 BASE_URL = settings.BASE_URL
                 DOCUSIGN_REDIRECT_APP_URL = settings.DOCUSIGN_REDIRECT_APP_URL
                 redirect_uri = BASE_URL + "/docusign_redirect"
-                final_consent_url = consent_url["consent_url"].replace(DOCUSIGN_REDIRECT_APP_URL, redirect_uri)
+                final_consent_url = consent_url["consent_url"].replace(
+                    DOCUSIGN_REDIRECT_APP_URL, redirect_uri
+                )
                 print(f"Final Consent URL: {final_consent_url}")
                 return redirect(final_consent_url)
 
-    check_docusign_consent.short_description = "Check if consent is required from Docusign"
+    check_docusign_consent.short_description = (
+        "Check if consent is required from Docusign"
+    )
 
     def get_actions(self, request):
         # Disable delete
         actions = super(DocuSignUserAuthAdmin, self).get_actions(request)
         return actions
 
     actions = [check_docusign_consent]
```

### Comparing `los_docusign-0.6.6/los_docusign/migrations/0001_initial.py` & `los_docusign-0.6.7/los_docusign/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import django.db.models.deletion
 import los_docusign.models
 import los_docusign.utils.validators
 import uuid
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ("contenttypes", "0002_remove_content_type_name"),
     ]
 
     operations = [
@@ -42,15 +41,18 @@
                         max_length=128,
                     ),
                 ),
                 (
                     "config_key",
                     models.CharField(max_length=128, verbose_name="Config Key"),
                 ),
-                ("created_at", models.DateTimeField(auto_now_add=True, null=True)),
+                (
+                    "created_at",
+                    models.DateTimeField(auto_now_add=True, null=True),
+                ),
                 ("updated_at", models.DateTimeField(auto_now=True, null=True)),
             ],
             options={
                 "verbose_name": "Docusign Choice Config",
                 "verbose_name_plural": "Docusign Choice Configs",
                 "db_table": "docusign_choice_configs",
             },
@@ -63,24 +65,32 @@
                     models.AutoField(
                         auto_created=True,
                         primary_key=True,
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
-                ("docusign_payload", models.TextField(verbose_name="Docusign Payload")),
+                (
+                    "docusign_payload",
+                    models.TextField(verbose_name="Docusign Payload"),
+                ),
                 (
                     "is_active",
                     models.BooleanField(default=True, verbose_name="Is Active"),
                 ),
-                ("created_at", models.DateTimeField(auto_now_add=True, null=True)),
+                (
+                    "created_at",
+                    models.DateTimeField(auto_now_add=True, null=True),
+                ),
                 ("updated_at", models.DateTimeField(auto_now=True, null=True)),
                 (
                     "is_default",
-                    models.BooleanField(default=False, verbose_name="Default Template"),
+                    models.BooleanField(
+                        default=False, verbose_name="Default Template"
+                    ),
                 ),
                 (
                     "template_type",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
                         to="los_docusign.docusignchoiceconfig",
                     ),
@@ -101,18 +111,23 @@
                         auto_created=True,
                         primary_key=True,
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
                 ("access_token", models.TextField(verbose_name="Access Token")),
-                ("expires_at", models.DateTimeField(verbose_name="Token Expires At")),
+                (
+                    "expires_at",
+                    models.DateTimeField(verbose_name="Token Expires At"),
+                ),
                 (
                     "organization_pk",
-                    models.CharField(max_length=255, verbose_name="organization pk"),
+                    models.CharField(
+                        max_length=255, verbose_name="organization pk"
+                    ),
                 ),
                 (
                     "two_factor_enabled_flag",
                     models.BooleanField(
                         default=False, verbose_name="Two Factor Enabled?"
                     ),
                 ),
@@ -121,15 +136,17 @@
                     models.CharField(
                         max_length=255, verbose_name="Docusign API Username"
                     ),
                 ),
                 (
                     "default_user",
                     models.BooleanField(
-                        default=False, max_length=255, verbose_name="Default User?"
+                        default=False,
+                        max_length=255,
+                        verbose_name="Default User?",
                     ),
                 ),
                 (
                     "organization_model",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="+",
@@ -154,15 +171,17 @@
                         primary_key=True,
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
                 (
                     "organization_pk",
-                    models.CharField(max_length=255, verbose_name="organization pk"),
+                    models.CharField(
+                        max_length=255, verbose_name="organization pk"
+                    ),
                 ),
                 (
                     "docusign_template",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
                         to="los_docusign.docusigntemplate",
                     ),
@@ -194,30 +213,39 @@
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
                 (
                     "slug",
                     models.UUIDField(
-                        blank=True, db_index=True, default=uuid.uuid4, editable=False
+                        blank=True,
+                        db_index=True,
+                        default=uuid.uuid4,
+                        editable=False,
                     ),
                 ),
                 (
                     "envelope_id",
                     models.CharField(
-                        db_index=True, max_length=255, verbose_name="Envelope ID"
+                        db_index=True,
+                        max_length=255,
+                        verbose_name="Envelope ID",
                     ),
                 ),
                 (
                     "record_status",
-                    models.CharField(max_length=255, verbose_name="Record Status"),
+                    models.CharField(
+                        max_length=255, verbose_name="Record Status"
+                    ),
                 ),
                 (
                     "envelope_status",
-                    models.CharField(max_length=255, verbose_name="Envelope Status"),
+                    models.CharField(
+                        max_length=255, verbose_name="Envelope Status"
+                    ),
                 ),
                 (
                     "recipient_status",
                     models.CharField(
                         blank=True,
                         default=None,
                         max_length=255,
@@ -236,15 +264,17 @@
                             los_docusign.utils.validators.validate_file_extension
                         ],
                         verbose_name="Document",
                     ),
                 ),
                 (
                     "envelope_response",
-                    models.CharField(max_length=255, verbose_name="Envelope Response"),
+                    models.CharField(
+                        max_length=255, verbose_name="Envelope Response"
+                    ),
                 ),
                 (
                     "error_message",
                     models.CharField(
                         blank=True,
                         max_length=255,
                         null=True,
@@ -311,18 +341,23 @@
                 ),
                 (
                     "object_pk",
                     models.CharField(
                         db_index=True, max_length=255, verbose_name="object pk"
                     ),
                 ),
-                ("event_received_at", models.DateTimeField(blank=True, null=True)),
+                (
+                    "event_received_at",
+                    models.DateTimeField(blank=True, null=True),
+                ),
                 (
                     "envelope_id",
-                    models.CharField(max_length=255, verbose_name="Envelope ID"),
+                    models.CharField(
+                        max_length=255, verbose_name="Envelope ID"
+                    ),
                 ),
                 (
                     "event_type",
                     models.CharField(
                         blank=True, db_index=True, max_length=125, null=True
                     ),
                 ),
@@ -382,15 +417,17 @@
                         primary_key=True,
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
                 (
                     "organization_pk",
-                    models.CharField(max_length=255, verbose_name="organization pk"),
+                    models.CharField(
+                        max_length=255, verbose_name="organization pk"
+                    ),
                 ),
                 (
                     "document_name",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
                         to="los_docusign.docusignchoiceconfig",
                     ),
@@ -412,15 +449,17 @@
                     ),
                 ),
             ],
             options={
                 "verbose_name": "Docusign Organization Template Exclusion",
                 "verbose_name_plural": "Docusign Organization Template Exclusions",
                 "db_table": "docusign_template_org_exclulsions",
-                "unique_together": {("organization_pk", "document_name", "template")},
+                "unique_together": {
+                    ("organization_pk", "document_name", "template")
+                },
             },
         ),
         migrations.CreateModel(
             name="DocusignOrgTemplateConfig",
             fields=[
                 (
                     "id",
@@ -441,19 +480,24 @@
                     "template_config",
                     models.JSONField(verbose_name="Template Configuration"),
                 ),
                 (
                     "is_active",
                     models.BooleanField(default=True, verbose_name="Is Active"),
                 ),
-                ("created_at", models.DateTimeField(auto_now_add=True, null=True)),
+                (
+                    "created_at",
+                    models.DateTimeField(auto_now_add=True, null=True),
+                ),
                 ("updated_at", models.DateTimeField(auto_now=True, null=True)),
                 (
                     "is_default",
-                    models.BooleanField(default=False, verbose_name="Default Config"),
+                    models.BooleanField(
+                        default=False, verbose_name="Default Config"
+                    ),
                 ),
                 (
                     "organization_model",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="+",
                         to="contenttypes.contenttype",
```

### Comparing `los_docusign-0.6.6/los_docusign/migrations/0002_auto_20211125_0208.py` & `los_docusign-0.6.7/los_docusign/migrations/0002_auto_20211125_0208.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from django.db import migrations, models
 import django.utils.timezone
 import model_utils.fields
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("los_docusign", "0001_initial"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="docusignchoiceconfig",
```

### Comparing `los_docusign-0.6.6/los_docusign/migrations/0003_auto_20211227_1445.py` & `los_docusign-0.6.7/los_docusign/migrations/0003_auto_20211227_1445.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.2.9 on 2021-12-27 19:45
 
 import django.core.serializers.json
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("los_docusign", "0002_auto_20211125_0208"),
     ]
 
     operations = [
         migrations.RemoveField(
             model_name="docusignchoiceconfig",
```

### Comparing `los_docusign-0.6.6/los_docusign/migrations/0004_auto_20220119_1610.py` & `los_docusign-0.6.7/los_docusign/migrations/0004_auto_20220119_1610.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.9 on 2022-01-19 21:10
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("los_docusign", "0003_auto_20211227_1445"),
     ]
 
     operations = [
         migrations.RemoveConstraint(
             model_name="docusignenvelopestagedata",
```

### Comparing `los_docusign-0.6.6/los_docusign/migrations/0005_docusignenvelopeauditlog_recipient_details.py` & `los_docusign-0.6.7/los_docusign/migrations/0005_docusignenvelopeauditlog_recipient_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.1.13 on 2022-01-29 00:23
 
 import django.core.serializers.json
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("los_docusign", "0004_auto_20220119_1610"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="docusignenvelopeauditlog",
```

### Comparing `los_docusign-0.6.6/los_docusign/models.py` & `los_docusign-0.6.7/los_docusign/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,20 +33,26 @@
         null=True,
         related_name="+",
         verbose_name=_("Organization Model"),
     )
     organization_pk = models.CharField(
         max_length=255, verbose_name=_("organization pk")
     )
-    docusign_api_username = models.CharField("Docusign API Username", max_length=255)
-    default_user = models.BooleanField("Default User?", max_length=255, default=False)
+    docusign_api_username = models.CharField(
+        "Docusign API Username", max_length=255
+    )
+    default_user = models.BooleanField(
+        "Default User?", max_length=255, default=False
+    )
 
     def save(self, *args, **kwargs):
         # Do not allow more than 1 default user
-        dsua = DocuSignUserAuth.objects.filter(default_user=True).exclude(id=self.id)
+        dsua = DocuSignUserAuth.objects.filter(default_user=True).exclude(
+            id=self.id
+        )
         if dsua.exists():
             self.default_user = False
         super().save(*args, **kwargs)
 
     def __str__(self):
         if self.default_user:
             return "Default Docusign User"
@@ -87,17 +93,15 @@
         upload_to=return_slug_for_url,
         max_length=255,
         validators=[validate_file_extension],
         blank=True,
         null=True,
     )
     envelope_response = models.CharField("Envelope Response", max_length=255)
-    error_message = models.TextField(
-        "Error Message", blank=True, null=True
-    )
+    error_message = models.TextField("Error Message", blank=True, null=True)
     docusign_user = models.ForeignKey(
         "los_docusign.DocuSignUserAuth", on_delete=models.PROTECT
     )
     # etran_loan = models.ForeignKey("loans.EtranLoan",on_delete=models.PROTECT, blank=True, null=True, related_name='envelopes')
     client_user_id = models.CharField(
         "Client User Id", max_length=255, null=True, blank=True
     )
@@ -109,15 +113,18 @@
         on_delete=models.SET_NULL,
         null=True,
         related_name="+",
         verbose_name=_("content type"),
     )
     object_pk = models.CharField(max_length=255, verbose_name=_("object pk"))
     phase = models.CharField(
-        max_length=255, blank=True, null=True, verbose_name=_("Application Phase")
+        max_length=255,
+        blank=True,
+        null=True,
+        verbose_name=_("Application Phase"),
     )
     current_status = JSONField(
         "Current status of the envelope received from webhook",
         blank=True,
         null=True,
         encoder=DjangoJSONEncoder,
     )
@@ -193,15 +200,17 @@
     DOCUSIGN_TEMPLATE_ORG_EXCLUSIONS = "docusign_template_org_exclulsions"
 
     MODEL_TYPE_CHOICES = (
         (DOCUSIGN_TEMPLATE, "docusign_templates"),
         (DOCUSIGN_TEMPLATE_ORG_EXCLUSIONS, "docusign_template_org_exclulsions"),
     )
 
-    docusign_model = models.CharField(choices=MODEL_TYPE_CHOICES, max_length=128)
+    docusign_model = models.CharField(
+        choices=MODEL_TYPE_CHOICES, max_length=128
+    )
     config_key = models.CharField("Config Key", max_length=128)
 
     def __str__(self):
         return f"{self.docusign_model}-{self.config_key}"
 
 
 class DocusignTemplate(TimeStampedModel, SoftDeleteMixin):
@@ -283,16 +292,20 @@
         verbose_name=_("content type"),
     )
     object_pk = models.CharField(
         db_index=True, max_length=255, verbose_name=_("object pk")
     )
     event_received_at = models.DateTimeField(null=True, blank=True)
     envelope_id = models.CharField("Envelope ID", max_length=255)
-    event_type = models.CharField(max_length=125, null=True, blank=True, db_index=True)
-    event_value = models.CharField(max_length=125, null=True, blank=True, db_index=True)
+    event_type = models.CharField(
+        max_length=125, null=True, blank=True, db_index=True
+    )
+    event_value = models.CharField(
+        max_length=125, null=True, blank=True, db_index=True
+    )
     tin = models.CharField(
         "TIN",
         max_length=9,
         null=True,
         blank=True,
         db_index=True,
         validators=[
```

### Comparing `los_docusign-0.6.6/los_docusign/urls.py` & `los_docusign-0.6.7/los_docusign/urls.py`

 * *Files identical despite different names*

### Comparing `los_docusign-0.6.6/los_docusign/utils/XmlParser.py` & `los_docusign-0.6.7/los_docusign/utils/XmlParser.py`

 * *Files identical despite different names*

### Comparing `los_docusign-0.6.6/los_docusign/utils/api_handler.py` & `los_docusign-0.6.7/los_docusign/utils/api_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 #
 # Copyright (c) 2021 Lenders Cooperative, a division of Summit Technology Group, Inc.
 #
 """Module to define base handler for external API calls"""
 
 import json
 import logging
-import typing
 
 import requests
 from requests.exceptions import (
     ConnectionError,
     HTTPError,
     ProxyError,
     ReadTimeout,
@@ -22,15 +21,22 @@
 
 LOGGER = logging.getLogger("root")
 
 
 class ApiHandler:
     """Base class for calling any external APIs"""
 
-    def __init__(self, url: str, api_key: str, tenant_schema: str, timeout: int, logging: bool = True):
+    def __init__(
+        self,
+        url: str,
+        api_key: str,
+        tenant_schema: str,
+        timeout: int,
+        logging: bool = True,
+    ):
         self.url = url
         self.__api_key = api_key
         self.__logging = logging
         self.__tenant_schema = tenant_schema
 
         self._timeout = timeout
 
@@ -89,15 +95,17 @@
                         "listItems": ["TenantSchema"],
                         "fieldId": "1",
                         "name": "TenantSchema",
                         "value": self.__tenant_schema,
                         "show": False,
                         "required": False,
                     }
-                    payload["customFields"]["listCustomFields"].append(custom_fields)
+                    payload["customFields"]["listCustomFields"].append(
+                        custom_fields
+                    )
                 payload = json.dumps(payload)
 
         try:
             if log_config:
                 log_entry = log_config.get("model")(
                     loan=log_config.get("loan"),
                     object_pk=log_config.get("object_pk"),
@@ -132,23 +140,28 @@
                     self.url,
                 )
 
             response_text = response.text
             if (
                 method
                 and method == "GET"
-                and ("/documents/combined" in self.url or "/documents/archive" in self.url)
+                and (
+                    "/documents/combined" in self.url
+                    or "/documents/archive" in self.url
+                )
                 and response.status_code == 200
             ):
                 response_text = f"Document download successfull for {self.url}"
 
             if log_entry:
                 log_entry.response_code = response.status_code
                 log_entry.response_body = response_text
-                log_entry.response_time = log_entry.request_time + response.elapsed
+                log_entry.response_time = (
+                    log_entry.request_time + response.elapsed
+                )
                 log_entry.response_headers = dict(response.headers)
                 log_entry.save()
 
             response.raise_for_status()
             return response
         except self.connection_exceptions as excp:
             if log_config:
```

### Comparing `los_docusign-0.6.6/los_docusign/utils/client.py` & `los_docusign-0.6.7/los_docusign/utils/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #
 # Created on Tue Dec 21 2021
 #
 # Copyright (c) 2021 Lenders Cooperative, a division of Summit Technology Group, Inc.
 #
 import json
 import logging
-import typing
 
 from django.conf import settings
 
 from los_docusign.utils.validators import validate_payload
 
 from .api_handler import ApiHandler
 from .docusign_helper import process_docusign_webhook, process_webhook_response
@@ -24,15 +23,17 @@
         DEFAULT_TIMEOUT = 60
         if timeout:
             self.timeout = timeout
         else:
             self.timeout = DEFAULT_TIMEOUT
         self.tenant_schema = tenant_schema
 
-    def generate_docusign_preview_url(self, params: dict, log_config: dict = None):
+    def generate_docusign_preview_url(
+        self, params: dict, log_config: dict = None
+    ):
         LOGGER.info("Generating Docusign Preview Url")
         if not (
             "envelope_id" in params
             and params["envelope_id"] is not None
             or "authentication_method" in params
             and params["authentication_method"] is not None
             or "email" in params
@@ -41,38 +42,50 @@
             and params["user_name"] is not None
             or "client_user_id" not in params
             and params["client_user_id"] is not None
             or "return_url" not in params
             and params["return_url"] is not None
         ):
             LOGGER.error("Invalid input dict for generate_docusign_preview_url")
-            raise Exception("Invalid input dict for generate_docusign_preview_url")
+            raise Exception(
+                "Invalid input dict for generate_docusign_preview_url"
+            )
 
         envelope_id = params["envelope_id"]
         authentication_method = params["authenticationMethod"]
         email = params["email"]
         user_name = params["userName"]
         client_user_id = params["clientUserId"]
         return_url = params["returnUrl"]
 
         url = settings.DOCUSIGN_API_ENDPOINT
 
-        preview_resource_path = f"{self.account_id}/envelopes/{envelope_id}/views/recipient"
+        preview_resource_path = (
+            f"{self.account_id}/envelopes/{envelope_id}/views/recipient"
+        )
         preview_url = url + preview_resource_path
         preview_data = {
             "authenticationMethod": authentication_method,
             "email": email,
             "userName": user_name,
             "clientUserId": client_user_id,
             "returnUrl": return_url,
         }
-        LOGGER.info("Calling API Handler's send request for generate_docusign_preview_url: [%s]", preview_url)
-        docusign_handler = ApiHandler(preview_url, self.api_key, self.tenant_schema, timeout=self.timeout)
+        LOGGER.info(
+            "Calling API Handler's send request for generate_docusign_preview_url: [%s]",
+            preview_url,
+        )
+        docusign_handler = ApiHandler(
+            preview_url, self.api_key, self.tenant_schema, timeout=self.timeout
+        )
         envelope_result = docusign_handler.send_request(
-            method="POST", payload=json.dumps(preview_data), log_config=log_config, event="EMBEDDED_URL"
+            method="POST",
+            payload=json.dumps(preview_data),
+            log_config=log_config,
+            event="EMBEDDED_URL",
         )
 
         LOGGER.debug(
             f"generate_docusign_preview_url completed for envelope {envelope_id} with status; {envelope_result.status_code}. Preview Url Data: {envelope_result.text}"
         )
         return envelope_result
 
@@ -102,17 +115,23 @@
             raise Exception(response)
 
         url = settings.DOCUSIGN_API_ENDPOINT
 
         resource_path = self.account_id + "/envelopes"
         envelope_url = url + resource_path
         LOGGER.info("Creating envelope for given payload")
-        docusign_handler = ApiHandler(envelope_url, self.api_key, self.tenant_schema, timeout=self.timeout)
+        docusign_handler = ApiHandler(
+            envelope_url, self.api_key, self.tenant_schema, timeout=self.timeout
+        )
         envelope_result = docusign_handler.send_request(
-            method="POST", payload=json.dumps(payload), log_config=log_config, add_custom_fields=True, event="SENT"
+            method="POST",
+            payload=json.dumps(payload),
+            log_config=log_config,
+            add_custom_fields=True,
+            event="SENT",
         )
 
         LOGGER.debug(
             f"create_envelope completed with status; {envelope_result.status_code}. Envelope Creation Data: {envelope_result.text}"
         )
         return envelope_result
 
@@ -121,41 +140,60 @@
         envelopeId = params["envelope_id"]
         # Value can be combined, archive
         document_download_option = params["doc_download_option"]
 
         account_id = settings.DOCUSIGN_API_ACCOUNT_ID
         headers = None
         if document_download_option == "archive":
-            resource_path = f"{account_id}/envelopes/{envelopeId}/documents/archive"
+            resource_path = (
+                f"{account_id}/envelopes/{envelopeId}/documents/archive"
+            )
             headers = {}
             headers["Accept"] = "application/zip, application/octet-stream"
         elif document_download_option == "combined":
-            resource_path = f"{account_id}/envelopes/{envelopeId}/documents/combined"
+            resource_path = (
+                f"{account_id}/envelopes/{envelopeId}/documents/combined"
+            )
 
         url = settings.DOCUSIGN_API_ENDPOINT
         doc_url = url + resource_path
 
-        docusign_handler = ApiHandler(doc_url, self.api_key, self.tenant_schema, timeout=self.timeout)
-        doc_download_result = docusign_handler.send_request(method="GET", log_config=log_config, event="DOWNLOAD_DOC")
+        docusign_handler = ApiHandler(
+            doc_url, self.api_key, self.tenant_schema, timeout=self.timeout
+        )
+        doc_download_result = docusign_handler.send_request(
+            method="GET", log_config=log_config, event="DOWNLOAD_DOC"
+        )
         LOGGER.info(
             f"download_docusign_document completed with status: {doc_download_result.status_code} for envelope id: {envelopeId}"
         )
         return doc_download_result
 
     def process_docusign_notification(
-        self, xml_string: str, log_config: dict | None = None, webhook_json_sim_enabled: bool | None = False
+        self,
+        xml_string: str,
+        log_config: dict | None = None,
+        webhook_json_sim_enabled: bool | None = False,
     ):
         LOGGER.debug(f"JSON Webhook: {webhook_json_sim_enabled}")
-        return process_docusign_webhook(xml_string, log_config, webhook_json_sim_enabled)
+        return process_docusign_webhook(
+            xml_string, log_config, webhook_json_sim_enabled
+        )
 
-    def extract_docusign_documents(self, xml_string: str, webhook_json_sim_enabled: bool = False):
-        docusign_data_dict = process_webhook_response(xml_string, webhook_json_sim_enabled)
+    def extract_docusign_documents(
+        self, xml_string: str, webhook_json_sim_enabled: bool = False
+    ):
+        docusign_data_dict = process_webhook_response(
+            xml_string, webhook_json_sim_enabled
+        )
         return docusign_data_dict["documents"]
 
-    def update_envelope_and_resend(self, envelope_id, signers_data: dict, log_config: dict | None = None):
+    def update_envelope_and_resend(
+        self, envelope_id, signers_data: dict, log_config: dict | None = None
+    ):
         url = settings.DOCUSIGN_API_ENDPOINT
 
         signer_payload = {}
         signers = []
         for signer in signers_data:
             signer_data = {}
             signer_data["recipientId"] = signer["recipientId"]
@@ -164,52 +202,68 @@
                 if signer["phone"]:
                     phoneAuthentication = {}
                     phoneAuthentication["recipMayProvideNumber"] = False
                     phoneAuthentication["validateRecipProvidedNumber"] = False
                     phoneAuthentication["recordVoicePrint"] = False
                     senderProvidedNumbers = []
                     senderProvidedNumbers.append(signer["phone"])
-                    phoneAuthentication["senderProvidedNumbers"] = senderProvidedNumbers
+                    phoneAuthentication[
+                        "senderProvidedNumbers"
+                    ] = senderProvidedNumbers
                     signer_data["phoneAuthentication"] = phoneAuthentication
-            except KeyError as e:
+            except KeyError:
                 pass
             signers.append(signer_data)
         signer_payload["signers"] = signers
-        resource_path = self.account_id + f"/envelopes/{envelope_id}/recipients?resend_envelope=true"
+        resource_path = (
+            self.account_id
+            + f"/envelopes/{envelope_id}/recipients?resend_envelope=true"
+        )
         envelope_url = url + resource_path
         LOGGER.info(f"Resending envelope: {envelope_id}")
 
-        docusign_handler = ApiHandler(envelope_url, self.api_key, self.tenant_schema, timeout=self.timeout)
+        docusign_handler = ApiHandler(
+            envelope_url, self.api_key, self.tenant_schema, timeout=self.timeout
+        )
         envelope_result = docusign_handler.send_request(
-            method="PUT", payload=json.dumps(signer_payload), log_config=log_config, event="RESEND"
+            method="PUT",
+            payload=json.dumps(signer_payload),
+            log_config=log_config,
+            event="RESEND",
         )
 
         LOGGER.debug(
             f"update_envelope_and_resend completed with status; {envelope_result.status_code}. update_envelope_and_resend data: {envelope_result.text}"
         )
         return envelope_result
 
-    def update_envelope_status(self, status_info: dict, log_config: dict = None):
+    def update_envelope_status(
+        self, status_info: dict, log_config: dict = None
+    ):
         url = settings.DOCUSIGN_API_ENDPOINT
 
         status_update_payload = {}
         envelope_id = status_info["envelope_id"]
         status = status_info["status"]
         reason = status_info["reason"]
 
         if status.lower() == "voided":
             status_update_payload["voidedReason"] = reason
 
         status_update_payload["status"] = status
 
         resource_path = self.account_id + f"/envelopes/{envelope_id}"
         envelope_url = url + resource_path
-        LOGGER.info(f"Updating envelope status to {status} for envelope : {envelope_id}")
+        LOGGER.info(
+            f"Updating envelope status to {status} for envelope : {envelope_id}"
+        )
 
-        docusign_handler = ApiHandler(envelope_url, self.api_key, self.tenant_schema, timeout=self.timeout)
+        docusign_handler = ApiHandler(
+            envelope_url, self.api_key, self.tenant_schema, timeout=self.timeout
+        )
         envelope_result = docusign_handler.send_request(
             method="PUT",
             payload=json.dumps(status_update_payload),
             log_config=log_config,
             event="UPDATE_ENVELOPE_STATUS",
         )
```

### Comparing `los_docusign-0.6.6/los_docusign/utils/docusign_adapter.py` & `los_docusign-0.6.7/los_docusign/utils/docusign_adapter.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,63 +5,75 @@
 import time
 from random import randint
 
 from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.core.cache import cache, caches
 from django.core.exceptions import ValidationError
+from django.db import connection
 from django.utils.translation import gettext_lazy as _
 
 from los_docusign.models import (
     DocusignChoiceConfig,
     DocusignEnvelopeStageData,
     DocusignOrgTemplate,
     DocuSignUserAuth,
 )
 from los_docusign.utils.client import DocuSignClient
-from los_docusign.utils.docusign_helper import get_access_token, get_docusign_user
+from los_docusign.utils.docusign_helper import (
+    get_access_token,
+    get_docusign_user,
+)
 
 LOGGER = logging.getLogger("root")
 
 
 class DocusignAdapter(metaclass=abc.ABCMeta):
     config_key = None  # abstract, should be defined by child classes
 
     def __init__(self, *args, **kwargs):
         self._setup_organization()
-        self.docusign_user = get_docusign_user(organization_pk=self.organization.pk)
+        self.request_timeout = kwargs.get(
+            "request_timeout",
+            getattr(settings, "DOCUSIGN_REQUEST_TIMEOUT", None),
+        )
+        self.docusign_user = get_docusign_user(
+            organization_pk=self.organization.pk
+        )
         self.access_token = get_access_token(self.docusign_user)
         self._setup_docusign_template()
         self._setup_docusign_client()
         self._setup_log_config()
         self._setup_signing_cache()
 
     def _setup_signing_cache(self, use_signing_cache=False):
         self.use_signing_cache = use_signing_cache
 
     def _setup_docusign_template(self):
         try:
             template = DocusignOrgTemplate.objects.get(
-                organization_model=ContentType.objects.get(model="organization"),
+                organization_model=ContentType.objects.get(
+                    model="organization"
+                ),
                 organization_pk=self.organization.pk,
                 docusign_template__template_type__config_key=self.config_key,
             ).docusign_template
         except DocusignOrgTemplate.DoesNotExist:
             dsua = DocuSignUserAuth.objects.get(default_user=True)
             template = DocusignOrgTemplate.objects.get(
                 organization=dsua.organization,
                 docusign_template__template_type=DocusignChoiceConfig.DOCUSIGN_TEMPLATE,
             ).docusign_template
         self.docusign_template = template
 
     def _setup_docusign_client(self):
         self.docusign_client = DocuSignClient(
             access_token=self.access_token,
-            timeout=settings.DOCUSIGN_REQUEST_TIMEOUT,
-            tenant_schema=settings.SCHEMA_NAME,
+            timeout=self.request_timeout,
+            tenant_schema=connection.schema_name or settings.SCHEMA_NAME,
         )
 
     def _setup_log_config(self, *args, **kwargs):
         """
         Dictionary used by ApiHandler to log actions in the database
         """
         self.log_config = None
@@ -71,26 +83,33 @@
         """
         This should be implemented by the application, and should set the
         organization to self.organization
         """
         raise NotImplementedError("You must implement this method")
 
     @abc.abstractmethod
-    def prepare_payload(self, instance, payload, client_user_id, is_embedded_docusign, **kwargs) -> dict:
+    def prepare_payload(
+        self, instance, payload, client_user_id, is_embedded_docusign, **kwargs
+    ) -> dict:
         """
-        This should be implemented by the application, and should return a dictionary in the form of
+        This should be implemented by the application, and should return
+        a dictionary
         """
         raise NotImplementedError("You must implement this method")
 
-    def _error_payload_not_configured_0001(self, connection):
-        raise ValidationError(_("Docusign payload not configured"))
+    def _error_payload_not_configured_0001(self, schema_name):
+        raise ValidationError(
+            _(f"Docusign payload not configured for {schema_name}")
+        )
 
     def _error_in_progress_0002(self):
         raise ValidationError(
-            _("DocuSign for this application is already in process, please try again after some time.")
+            _(
+                "DocuSign for this application is already in process, please try again after some time."
+            )
         )
 
     def _error_high_volume_throttle_0003(self):
         raise ValidationError(
             _(
                 "Our electronic signature process is currently experiencing high volume and we are throttling requests to protect your experience. Please return after one or two hours to complete your signature process. Your application is complete and your place in line is reserved."
             )
@@ -109,44 +128,49 @@
     def _error_high_volume_throttle_0006(self):
         raise ValidationError(
             _(
                 "Our electronic signature process is currently experiencing high volume and we are throttling requests to protect your experience. Please return after one or two hours to complete your signature process. Your application is complete and your place in line is reserved."
             )
         )
 
-    def _error_unknown_0007(self, loan, exception):
+    def _error_unknown_0007(self, instance, exception):
         raise ValidationError(
             _(
-                "Our electronic signature process is currently experiencing high volume and we are throttling requests to protect your experience. Please return after one or two hours to complete your signature process. Your application is complete and your place in line is reserved."
+                f"Failed to initiate docusign for instance: [{instance}]. Error: [{exception}]"
             )
         )
 
-    def process_docusign_error(self, instance, docusign_envelope_stage_data, envelope_result):
+    def process_docusign_error(
+        self, instance, docusign_envelope_stage_data, envelope_result
+    ):
         error_text = json.loads(envelope_result.text)
         error_code = error_text["errorCode"]
 
         if error_code in [
             "HOURLY_APIINVOCATION_LIMIT_EXCEEDED",
             "BURST_APIINVOCATION_LIMIT_EXCEEDED",
             "HOURLY_APIINVOCATION_ENVELOPE_LIMIT_EXCEEDED",
         ]:
-            raise Exception("DocuSign API THROTTLING Error: {error_text}".format(error_text=envelope_result.text))
+            raise Exception(
+                f"DocuSign API THROTTLING Error: {envelope_result.text}"
+            )
 
         docusign_envelope_stage_data.record_status = "F"
         docusign_envelope_stage_data.error_message = envelope_result.text
 
         # Since we are creating a new instance
         docusign_envelope_stage_data.save()  # nosemgrep
         raise Exception(
-            "DocuSign Error: Failed to create the envelope for application"
-            " id: {instance_id} : {error_text}".format(instance_id=instance, error_text=envelope_result.text)
+            f"DocuSign Error: Failed to create the envelope for application id: {instance} : {envelope_result.text}"
         )
 
     def _get_envelope_content_type(self, instance):
-        return ContentType.objects.get(model=instance._meta.model_name, app_label=instance._meta.app_label)
+        return ContentType.objects.get(
+            model=instance._meta.model_name, app_label=instance._meta.app_label
+        )
 
     def get_client_user_id(self, is_embedded_docusign):
         return str(randint(10000, 99999)) if is_embedded_docusign else None
 
     def _create_current_status(self, envelope_id, envelope_status, signers):
         recipients = []
         for signer in signers:
@@ -186,17 +210,21 @@
         docusign_envelope_stage_data = DocusignEnvelopeStageData(
             docusign_user=self.docusign_user,
             object_pk=instance.pk if instance else None,
         )
 
         docusign_envelope_stage_data.docusign_user = self.docusign_user
 
-        docusign_envelope_stage_data.object_pk = instance.pk if instance else None
+        docusign_envelope_stage_data.object_pk = (
+            instance.pk if instance else None
+        )
 
-        docusign_envelope_stage_data.content_type = self._get_envelope_content_type(instance)
+        docusign_envelope_stage_data.content_type = (
+            self._get_envelope_content_type(instance)
+        )
 
         if not payload:
             docusign_template = self.docusign_template
             docusign_los_payload = docusign_template.docusign_payload
         else:
             docusign_los_payload = payload
 
@@ -207,18 +235,20 @@
             request_payload = docusign_los_payload
         else:
             request_payload = json.loads(docusign_los_payload)
 
         # If consent is required, then a dict with consent url will be returned by the wrapper.
         if isinstance(self.access_token, dict):
             raise Exception(
-                "Docusign Consent is required for the user: {error_text}".format(error_text=self.access_token)
+                f"Docusign Consent is required for the user: {self.access_token}"
             )
 
-        client_user_id = self.get_client_user_id(is_embedded_docusign=is_embedded_docusign)
+        client_user_id = self.get_client_user_id(
+            is_embedded_docusign=is_embedded_docusign
+        )
 
         docusign_payload = self.prepare_payload(
             payload=request_payload,
             instance=instance,
             client_user_id=client_user_id,
             is_embedded_docusign=is_embedded_docusign,
             phase=phase,
@@ -240,20 +270,22 @@
         instance,
         return_url,
         phase,
         signer_email,
         signer_name,
         docusign_envelope_stage_data,
     ):
-        latest_unsigned_embedded_envelope = DocusignEnvelopeStageData.objects.filter(
-            object_pk=instance.pk if instance else None,
-            envelope_status="sent",
-            phase=phase,
-            is_removed=False,
-        ).first()
+        latest_unsigned_embedded_envelope = (
+            DocusignEnvelopeStageData.objects.filter(
+                object_pk=instance.pk if instance else None,
+                envelope_status="sent",
+                phase=phase,
+                is_removed=False,
+            ).first()
+        )
         if latest_unsigned_embedded_envelope:
             client_user_id = latest_unsigned_embedded_envelope.client_user_id
             envelope_id = latest_unsigned_embedded_envelope.envelope_id
 
             # WIP DocuSign from the application directly
             # TODO: move to process_embedded_docusign
             params = {
@@ -261,19 +293,25 @@
                 "authenticationMethod": "None",
                 "email": signer_email,
                 "userName": signer_name,
                 "clientUserId": client_user_id,
                 "access_token": "Bearer " + self.access_token,
                 "returnUrl": return_url,
             }
-            envelope_result = self.docusign_client.generate_docusign_preview_url(params, self.log_config)
+            envelope_result = (
+                self.docusign_client.generate_docusign_preview_url(
+                    params, self.log_config
+                )
+            )
             if self.use_signing_cache:
                 cache.set(f"docusign_embedded_signing:{instance.id}", True, 600)
             if envelope_result.status_code != 201:
-                return self.process_docusign_error(instance, docusign_envelope_stage_data, envelope_result)
+                return self.process_docusign_error(
+                    instance, docusign_envelope_stage_data, envelope_result
+                )
 
             return envelope_result
 
     def _send_for_docusign(
         self,
         docusign_envelope_stage_data,
         client_user_id,
@@ -298,15 +336,17 @@
             signer_email,
             signer_name,
             docusign_envelope_stage_data,
         )
         if existing_envelope_result:
             return existing_envelope_result
 
-        envelope_result = self.docusign_client.create_envelope(request_payload, self.log_config)
+        envelope_result = self.docusign_client.create_envelope(
+            request_payload, self.log_config
+        )
         docusign_envelope_stage_data.envelope_response = envelope_result.text
 
         if envelope_result.status_code == 201:
             resp = json.loads(envelope_result.text)
             docusign_envelope_stage_data.record_status = "S"
             docusign_envelope_stage_data.envelope_id = resp["envelopeId"]
             docusign_envelope_stage_data.envelope_status = resp["status"]
@@ -314,38 +354,52 @@
             current_status = self._create_current_status(
                 resp["envelopeId"],
                 resp["status"],
                 request_payload["recipients"]["signers"],
             )
             docusign_envelope_stage_data.current_status = current_status
 
-            self._envelope_response_audit_log(instance, docusign_envelope_stage_data, current_status, resp)
+            self._envelope_response_audit_log(
+                instance, docusign_envelope_stage_data, current_status, resp
+            )
 
             if is_embedded_docusign:
                 params = {
                     "envelope_id": resp["envelopeId"],
                     "authenticationMethod": "None",
                     "email": signer_email,
                     "userName": signer_name,
                     "clientUserId": client_user_id,
                     "returnUrl": return_url,
                 }
-                envelope_result = self.docusign_client.generate_docusign_preview_url(params, self.log_config)
+                envelope_result = (
+                    self.docusign_client.generate_docusign_preview_url(
+                        params, self.log_config
+                    )
+                )
                 if envelope_result.status_code != 201:
-                    return self.process_docusign_error(instance, docusign_envelope_stage_data, envelope_result)
+                    return self.process_docusign_error(
+                        instance, docusign_envelope_stage_data, envelope_result
+                    )
                 if self.use_signing_cache:
-                    cache.set(f"docusign_embedded_signing:{instance.id}", True, 600)
+                    cache.set(
+                        f"docusign_embedded_signing:{instance.id}", True, 600
+                    )
         else:
-            return self.process_docusign_error(instance, docusign_envelope_stage_data, envelope_result)
+            return self.process_docusign_error(
+                instance, docusign_envelope_stage_data, envelope_result
+            )
 
         # Since we are creating a new instance
         docusign_envelope_stage_data.save()  # nosemgrep
         return envelope_result
 
-    def _envelope_response_audit_log(self, instance, docusign_envelope_stage_data, current_status, resp):
+    def _envelope_response_audit_log(
+        self, instance, docusign_envelope_stage_data, current_status, resp
+    ):
         pass
 
     def initiate_docusign(
         self,
         return_url,
         phase,
         instance,
@@ -369,48 +423,63 @@
             )
 
             if response.status_code == http.HTTPStatus.CREATED:
                 # check the rate limit remaining.
                 # x_rate_limit = int(response.headers["X-RateLimit-Limit"])
                 # ten_percent_of_rate_limit = x_rate_limit * 0.1
 
-                x_rate_limit_remaining = int(response.headers["X-RateLimit-Remaining"])
+                x_rate_limit_remaining = int(
+                    response.headers["X-RateLimit-Remaining"]
+                )
                 if x_rate_limit_remaining == 0:
                     reset_timestamp = int(response.headers["X-RateLimit-Reset"])
                     calculated_timeout = reset_timestamp - int(time.time())
                     cache.set(
                         "docusign_rate_reset",
                         reset_timestamp,
                         timeout=calculated_timeout,
                     )
-                return response.json()["url"] if is_embedded_docusign else return_url
+                return (
+                    response.json()["url"]
+                    if is_embedded_docusign
+                    else return_url
+                )
             elif response.status_code in [
                 http.HTTPStatus.BAD_REQUEST,
                 http.HTTPStatus.UNAUTHORIZED,
                 http.HTTPStatus.NOT_FOUND,
                 http.HTTPStatus.UNSUPPORTED_MEDIA_TYPE,
             ]:
                 error_text = json.loads(response.text)
                 error_code = error_text["errorCode"]
 
                 if error_code == "HOURLY_APIINVOCATION_LIMIT_EXCEEDED":
                     if not cache.get("docusign_rate_reset", None):
-                        reset_timestamp = int(response.headers["X-RateLimit-Reset"])
+                        reset_timestamp = int(
+                            response.headers["X-RateLimit-Reset"]
+                        )
                         calculated_timeout = reset_timestamp - int(time.time())
-                        cache.set("docusign_rate_reset", reset_timestamp, timeout=calculated_timeout)
+                        cache.set(
+                            "docusign_rate_reset",
+                            reset_timestamp,
+                            timeout=calculated_timeout,
+                        )
 
                     return self._error_high_volume_throttle_0006()
 
                 elif error_code == "BURST_APIINVOCATION_LIMIT_EXCEEDED":
                     if not cache.get("docusign_rate_reset", None):
                         # Setting the timeout to 30 seconds as for burst limit
-                        reset_timestamp = int(response.headers["X-RateLimit-Reset"])
-                        cache.set("docusign_rate_reset", reset_timestamp, timeout=30)
+                        reset_timestamp = int(
+                            response.headers["X-RateLimit-Reset"]
+                        )
+                        cache.set(
+                            "docusign_rate_reset", reset_timestamp, timeout=30
+                        )
 
                     return self._error_high_volume_throttle_0005()
 
                 else:
                     return self._error_docusigning_failed_0004()
         except Exception as excp:
             # TODO: Handle this with correct error code.
             return self._error_unknown_0007(instance, excp)
-            raise
```

### Comparing `los_docusign-0.6.6/los_docusign/utils/docusign_helper.py` & `los_docusign-0.6.7/los_docusign/utils/docusign_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #
 # Created on Tue Dec 21 2021
 #
-# Copyright (c) 2021 Lenders Cooperative, a division of Summit Technology Group, Inc.
+# Copyright (c) 2021 Lenders Cooperative, a division of
+# Summit Technology Group, Inc.
 #
 import base64
 import hashlib
 import hmac
 import json
 import logging
 import re
@@ -32,58 +33,67 @@
 SCOPES = ["signature"]
 
 LOGGER = logging.getLogger("root")
 
 
 def get_webhook_is_json(default: bool | None = None):
     # `default` will allow other fn's to be able to accept input,
-    #  and keep the same logic without repeated if statements everywhere this is called
+    #  and keep the same logic without repeated if statements everywhere this
+    # is called
     if default is not None:
         return default
     # if nothing was passed in, check settings
     if hasattr(settings, "DOCUSIGN_ENABLE_JSON_SIM"):
         return settings.DOCUSIGN_ENABLE_JSON_SIM
     # if the setting is not found, fall back to xml
     return False
 
 
 def get_docusign_user(organization_pk):
     try:
         # Try if the user is the available and has the docusign account
-        docusign_user = DocuSignUserAuth.objects.get(organization_pk=organization_pk)
+        docusign_user = DocuSignUserAuth.objects.get(
+            organization_pk=organization_pk
+        )
     except DocuSignUserAuth.DoesNotExist:
         # Else use the default user
         docusign_user = DocuSignUserAuth.objects.get(default_user=True)
 
     return docusign_user
 
 
 def get_access_token(docusign_user, redirect_url=None):
     docusign_token_expiry = settings.DOCUSIGN_TOKEN_EXPIRY_IN_SECONDS
 
     if docusign_user.expires_at >= timezone.now():
         access_token = docusign_user.access_token
     else:
-        token_response = _jwt_auth(docusign_user.docusign_api_username, redirect_url)
+        token_response = _jwt_auth(
+            docusign_user.docusign_api_username, redirect_url
+        )
         try:
             if token_response["consent_url"]:
                 return token_response
-        except TypeError as e:
+        except TypeError:
             pass
         access_token = token_response.access_token
         docusign_user.access_token = access_token
-        docusign_user.expires_at = timezone.now() + timedelta(seconds=int(docusign_token_expiry))
+        docusign_user.expires_at = timezone.now() + timedelta(
+            seconds=int(docusign_token_expiry)
+        )
         docusign_user.save()
 
     return access_token
 
 
 def check_docusign_access_token(organization_pk, redirect_uri=None):
     docusign_user = get_docusign_user(organization_pk)
-    token_response = _jwt_auth(docusign_user.docusign_api_username, redirect_uri)
+    token_response = _jwt_auth(
+        docusign_user.docusign_api_username, redirect_uri
+    )
     LOGGER.info("Checking DocuSign Access Token")
     if token_response and isinstance(token_response, dict):
         # return the consent_url here
         return token_response
     return None
 
 
@@ -95,16 +105,15 @@
     if "impersonation" not in use_scopes:
         use_scopes.append("impersonation")
 
     # Catch IO error
     try:
         private_key = _get_private_key().encode("ascii").decode("utf-8")
 
-    except (OSError, IOError) as err:
-        # sentry_sdk.capture_exception(Exception(f'OSError, IOError in Docusign JWT Auth'))
+    except (OSError, IOError):
         return "error"
 
     try:
         jwtTokenResponse = api_client.request_jwt_user_token(
             client_id=str(settings.DOCUSIGN_CLIENT_ID),
             user_id=docusign_api_username,
             oauth_host_name=str(settings.DOCUSIGN_AUTHORIZATION_SERVER),
@@ -126,31 +135,36 @@
                 f"https://{settings.DOCUSIGN_AUTHORIZATION_SERVER}/oauth/auth?response_type=code&"
                 f"scope={consent_scopes}&client_id={settings.DOCUSIGN_CLIENT_ID}&redirect_uri={redirect_uri}"
             )
             consent_url_dict = {}
             consent_url_dict["consent_url"] = consent_url
             return consent_url_dict
         else:
-            LOGGER.error(f"Error while getting the jwt token for docusign: {err}")
+            LOGGER.error(
+                f"Error while getting the jwt token for docusign: {err}"
+            )
             raise
 
     return jwtTokenResponse
 
 
 def _get_private_key():
     """
-    Check that the private key present in the file and if it is, get it from the file.
+    Check that the private key present in the file and if it is, get it from
+    the file.
     In the opposite way get it from config variable.
     """
     private_key_file = path.abspath(settings.DOCUSIGN_PRIVATE_KEY_FILE)
     if path.isfile(private_key_file):
         with open(private_key_file) as private_key_file:
             private_key = private_key_file.read()
     else:
-        private_key = settings.DOCUSIGN_PRIVATE_KEY_FILE.encode().decode("unicode-escape")
+        private_key = settings.DOCUSIGN_PRIVATE_KEY_FILE.encode().decode(
+            "unicode-escape"
+        )
 
     return private_key
 
 
 def populate_text_tabs(text_tabs_forms, text_tabs_data: dict):
     # Need to populate all the text tabs with the values
     for textTabsInfo in text_tabs_forms:
@@ -168,58 +182,72 @@
             organization_model="organization",
             docusign_template__template_type=template_name,
             organization_pk=organization_pk,
         ).docusign_template
     except DocusignOrgTemplate.DoesNotExist:
         dsua = DocuSignUserAuth.objects.get(default_user=True)
         docusign_template = DocusignOrgTemplate.objects.get(
-            object_pk=dsua.object_pk, docusign_template__template_type=template_name
+            object_pk=dsua.object_pk,
+            docusign_template__template_type=template_name,
         ).docusign_template
 
     docusign_payload = docusign_template.docusign_payload
     if docusign_payload is None:
-        LOGGER.error(f"Payload Not found for org {organization_pk}. Check database..return")
+        LOGGER.error(
+            f"Payload Not found for org {organization_pk}. Check database..return"
+        )
         return
 
     # resp = json.loads(docusign_payload)
     return docusign_payload
 
 
 def _process_json_webhook_response(json_str):
     docusign_response_obj = json.loads(json_str)
 
     trimmed_object = {
         "raw": docusign_response_obj,
         "event": docusign_response_obj["event"],
         "envelope_id": docusign_response_obj["data"]["envelopeId"],
-        "envelope_status": str(docusign_response_obj["data"]["envelopeSummary"]["status"]).lower(),
+        "envelope_status": str(
+            docusign_response_obj["data"]["envelopeSummary"]["status"]
+        ).lower(),
         "custom_fields": {
             field["name"]: field["value"]
-            for field in docusign_response_obj["data"]["envelopeSummary"]["customFields"]["listCustomFields"]
+            for field in docusign_response_obj["data"]["envelopeSummary"][
+                "customFields"
+            ]["listCustomFields"]
         },
         "recipients": [],
     }
 
-    for raw_recipient in docusign_response_obj["data"]["envelopeSummary"].get("recipients", {}).get("signers", []):
+    for raw_recipient in (
+        docusign_response_obj["data"]["envelopeSummary"]
+        .get("recipients", {})
+        .get("signers", [])
+    ):
         recipient_data = {
             "recipient_id": raw_recipient["recipientId"],
             "email": raw_recipient["email"],
             "name": raw_recipient["name"],
             "sent_time": raw_recipient.get("sentDateTime", None),
             "routing_order": raw_recipient["routingOrder"],
             "custom_fields": raw_recipient.get("customFields"),
             "status": raw_recipient["status"],
         }
 
-        # recipient_auth_status = raw_recipient.get("RecipientAuthenticationStatus")
-        if recipient_auth_status := raw_recipient.get("RecipientAuthenticationStatus"):
+        if recipient_auth_status := raw_recipient.get(
+            "RecipientAuthenticationStatus"
+        ):
             phone_auth_status = recipient_auth_status.get("PhoneAuthResult", {})
 
             recipient_data["raw_auth_status"] = recipient_auth_status
-            recipient_data["phone_auth_timestamp"] = phone_auth_status.get("EventTimestamp")
+            recipient_data["phone_auth_timestamp"] = phone_auth_status.get(
+                "EventTimestamp"
+            )
 
         # XXX: this is missing from the sample json
         # for rd_key, ras_key in (
         #     ('id_question_status',"IDQuestionsResult"),
         #     ('id_lookup_status',"IDLookupResult"),
         #     ('phone_auth_status',"PhoneAuthResult"),
         # ):
@@ -228,15 +256,17 @@
         #         status = str(status.get("Status")).lower()
 
         #     recipient_data[rd_key] = status
 
         trimmed_object["recipients"].append(recipient_data)
 
     # read and map documents
-    document_pdfs = docusign_response_obj["data"]["envelopeSummary"].get("envelopeDocuments", [])
+    document_pdfs = docusign_response_obj["data"]["envelopeSummary"].get(
+        "envelopeDocuments", []
+    )
     if not isinstance(document_pdfs, list):
         document_pdfs = [document_pdfs]
 
     documents = []
     for document_pdf in document_pdfs:
         document = {
             "name": document_pdf["name"],
@@ -250,28 +280,34 @@
 
     return trimmed_object
 
 
 def _process_xml_webhook_response(xml_string):
     root = ElementTree.XML(xml_string)
     request_data_dict = XmlDictConfig(root)
-    m = re.search("{http://www.docusign.net/API/(.+?)}EnvelopeStatus", str(request_data_dict))
+    m = re.search(
+        "{http://www.docusign.net/API/(.+?)}EnvelopeStatus",
+        str(request_data_dict),
+    )
     api_version = None
     if m:
         api_version = m.group(1)
     else:
-        # sentry_sdk.capture_exception(Exception(f'Failed to retrieve API Version for the DocuSign Webhook: {str(request_data_dict)}'))
+        # sentry_sdk.capture_exception(Exception(f'Failed to retrieve
+        # API Version for the DocuSign Webhook: {str(request_data_dict)}'))
         raise Http404
 
     docusign_schema = f"{{http://www.docusign.net/API/{api_version}}}"
 
-    # Since we are not using any of the data sent back by DocuSign, we clear those fields which potentially causes json.dumps to fail to parse Decimal Values which are set by the Parser
-    recipient_signers = request_data_dict[f"{docusign_schema}EnvelopeStatus"][f"{docusign_schema}RecipientStatuses"][
-        f"{docusign_schema}RecipientStatus"
-    ]
+    # Since we are not using any of the data sent back by DocuSign, we
+    # clear those fields which potentially causes json.dumps to fail to '
+    # parse Decimal Values which are set by the Parser
+    recipient_signers = request_data_dict[f"{docusign_schema}EnvelopeStatus"][
+        f"{docusign_schema}RecipientStatuses"
+    ][f"{docusign_schema}RecipientStatus"]
 
     if not isinstance(recipient_signers, list):
         recipient_signers = [recipient_signers]
 
     for recipients in recipient_signers:
         recipients[f"{docusign_schema}TabStatuses"] = None
         recipients[f"{docusign_schema}FormData"] = None
@@ -282,42 +318,56 @@
         json.dumps(request_data_dict),
     )
     docusign_response_obj = json.loads(line)
 
     trimmed_object = {
         "raw": docusign_response_obj,
         "envelope_id": docusign_response_obj["EnvelopeStatus"]["EnvelopeID"],
-        "envelope_status": str(docusign_response_obj["EnvelopeStatus"]["Status"]).lower(),
+        "envelope_status": str(
+            docusign_response_obj["EnvelopeStatus"]["Status"]
+        ).lower(),
         "custom_fields": {
-            docusign_response_obj["EnvelopeStatus"]["CustomFields"][field]["Name"]: docusign_response_obj[
-                "EnvelopeStatus"
-            ]["CustomFields"][field]["Value"]
+            docusign_response_obj["EnvelopeStatus"]["CustomFields"][field][
+                "Name"
+            ]: docusign_response_obj["EnvelopeStatus"]["CustomFields"][field][
+                "Value"
+            ]
             for field in docusign_response_obj["EnvelopeStatus"]["CustomFields"]
         },
         "recipients": [],
     }
-    recipient_statues = docusign_response_obj["EnvelopeStatus"]["RecipientStatuses"]
+    recipient_statues = docusign_response_obj["EnvelopeStatus"][
+        "RecipientStatuses"
+    ]
     for raw_recipient in recipient_statues:
         recipient_data = {
             "recipient_id": recipient_statues[raw_recipient]["RecipientId"],
             "email": recipient_statues[raw_recipient]["Email"],
             "name": recipient_statues[raw_recipient]["UserName"],
             "sent_time": recipient_statues[raw_recipient].get("Sent", None),
             "routing_order": recipient_statues[raw_recipient]["RoutingOrder"],
-            "custom_fields": recipient_statues[raw_recipient].get("CustomFields"),
+            "custom_fields": recipient_statues[raw_recipient].get(
+                "CustomFields"
+            ),
             "status": recipient_statues[raw_recipient]["Status"],
         }
 
-        recipient_auth_status = recipient_statues[raw_recipient].get("RecipientAuthenticationStatus", {})
+        recipient_auth_status = recipient_statues[raw_recipient].get(
+            "RecipientAuthenticationStatus", {}
+        )
         phone_auth_status = (
-            recipient_statues[raw_recipient].get("RecipientAuthenticationStatus", {}).get("PhoneAuthResult", {})
+            recipient_statues[raw_recipient]
+            .get("RecipientAuthenticationStatus", {})
+            .get("PhoneAuthResult", {})
         )
 
         recipient_data["raw_auth_status"] = recipient_auth_status
-        recipient_data["phone_auth_timestamp"] = phone_auth_status.get("EventTimestamp")
+        recipient_data["phone_auth_timestamp"] = phone_auth_status.get(
+            "EventTimestamp"
+        )
 
         for rd_key, ras_key in (
             ("id_question_status", "IDQuestionsResult"),
             ("id_lookup_status", "IDLookupResult"),
             ("phone_auth_status", "PhoneAuthResult"),
         ):
             status = recipient_auth_status.get(ras_key)
@@ -359,27 +409,38 @@
 def process_docusign_webhook(
     xml_string,
     log_config,
     webhook_json_sim_enabled=None,
     event=None,
     event_type="WEBHOOK",
 ):
-    docusign_data_dict = process_webhook_response(xml_string, webhook_json_sim_enabled)
+    docusign_data_dict = process_webhook_response(
+        xml_string, webhook_json_sim_enabled
+    )
     envelopeId = docusign_data_dict["envelope_id"]
 
     try:
-        envelope_stage_data = DocusignEnvelopeStageData.objects.get(envelope_id=envelopeId)
+        envelope_stage_data = DocusignEnvelopeStageData.objects.get(
+            envelope_id=envelopeId
+        )
     except DocusignEnvelopeStageData.DoesNotExist:
         LOGGER.error(f"Envelope id  {envelopeId} not found in system")
         raise Exception(f"Envelope id  {envelopeId} not found in system")
 
-    return _extract_envelope_information(envelope_stage_data, docusign_data_dict, log_config, event_type)
+    return _extract_envelope_information(
+        envelope_stage_data, docusign_data_dict, log_config, event_type
+    )
 
 
-def _extract_envelope_information(envelope_stage_data, docusign_data_dict, log_config=None, event_type="WEBHOOK"):
+def _extract_envelope_information(
+    envelope_stage_data,
+    docusign_data_dict,
+    log_config=None,
+    event_type="WEBHOOK",
+):
     event_value = None
     try:
         envelope_id = docusign_data_dict["envelope_id"]
         recipients = docusign_data_dict["recipients"]
         envelope_status = str(docusign_data_dict["envelope_status"]).lower()
 
         if not isinstance(recipients, list):
@@ -421,28 +482,41 @@
                     recipient_status = "authentication failed"
                     recipient_failed_authentication = True
 
                 if current_status is None:
                     if recipient_phone_auth_status:
                         phone_auth = {
                             "status": recipient_phone_auth_status,
-                            "last_event_time": recipient["phone_auth_timestamp"],
-                            "fail_count": (0 if recipient_phone_auth_status == "passed" else 1),
+                            "last_event_time": recipient[
+                                "phone_auth_timestamp"
+                            ],
+                            "fail_count": (
+                                0
+                                if recipient_phone_auth_status == "passed"
+                                else 1
+                            ),
                         }
                     recipient_data["phone_auth"] = phone_auth
                 else:
                     current_status_recipients = current_status["recipients"]
                     for current_recipient in current_status_recipients:
                         phone_auth = current_recipient.get("phone_auth")
                         if (
-                            current_recipient["email"] == recipient_data["email"]
-                            and current_recipient["name"] == recipient_data["name"]
-                            and current_recipient["custom_fields"]["CustomField"] in recipient_data["custom_fields"]
+                            current_recipient["email"]
+                            == recipient_data["email"]
+                            and current_recipient["name"]
+                            == recipient_data["name"]
+                            and current_recipient["custom_fields"][
+                                "CustomField"
+                            ]
+                            in recipient_data["custom_fields"]
                         ):
-                            # Currently not relying on the recipient id as we do store the sent recipient id and we receive the Docusign internal recipient id
+                            # Currently not relying on the recipient id as we
+                            # do store the sent recipient id and we receive
+                            # the Docusign internal recipient id
                             if phone_auth is None:
                                 phone_auth = {
                                     "fail_count": None,
                                     "status": None,
                                     "last_event_time": None,
                                 }
 
@@ -450,25 +524,32 @@
                                 if recipient_phone_auth_status == "passed":
                                     phone_auth["fail_count"] = 0
                                 else:
                                     if phone_auth.get("fail_count"):
                                         phone_auth["fail_count"] += 1
                                     else:
                                         phone_auth["fail_count"] = 1
-                                        phone_auth["status"] = recipient_phone_auth_status
-                                        phone_auth["last_event_time"] = recipient["phone_auth_timestamp"]
+                                        phone_auth[
+                                            "status"
+                                        ] = recipient_phone_auth_status
+                                        phone_auth[
+                                            "last_event_time"
+                                        ] = recipient["phone_auth_timestamp"]
                             recipient_data["phone_auth"] = phone_auth
                             break
 
             recipients_data.append(recipient_data)
 
-        # Let's not overwrite the status of authentication failed if the recipient failed authentication.
-        # We need this to know if the receipient failed authentication and later on completed the application
-        # Assigning the envelope status value to recipient status as the for multiple signers,
-        # Env status will be updated to "Completed" only when all signers sign.
+        # Let's not overwrite the status of authentication failed if the
+        # recipient failed authentication.
+        # We need this to know if the receipient failed authentication and
+        # later on completed the application
+        # Assigning the envelope status value to recipient status as the for
+        # multiple signers, Env status will be updated to "Completed" only
+        # when all signers sign.
 
         if not envelope_stage_data.recipient_status == "authentication failed":
             envelope_stage_data.recipient_status = envelope_status
 
         if "failed" in (
             recipient_id_lookup_status,
             recipient_id_question_status,
@@ -483,32 +564,22 @@
         elif recipient_failed_delivery:
             recipient_status = "autoresponded"
         else:
             recipient_status = ""
 
         event_value = envelope_status
 
-        if recipient_status == "authentication failed" and envelope_status == "sent":
+        if (
+            recipient_status == "authentication failed"
+            and envelope_status == "sent"
+        ):
             event_value = "authentication failed"
         elif recipient_status == "autoresponded" and envelope_status == "sent":
             event_value = "autoresponded"
 
-        # TODO: Need to understand how can we log this in the DocuSignEnvelopeAuditLog, since we do not have the content type?
-        # log = DocusignEnvelopeAuditLog(
-        #     content_type=envelope_stage_data.content_type,
-        #     object_pk=envelope_stage_data.object_pk,
-        #     event_received_at=datetime.now(),
-        #     envelope_id=envelope_stage_data.envelope_id,
-        #     event_type="WEBHOOK",
-        #     event_value=event_value,
-        #     remote_addr="0.0.0.0",
-        #     recipient_details=recipients_data,
-        # )
-        # log.save()
-
         if log_config:
             log_entry = log_config.get("model")(
                 loan=log_config.get("loan"),
                 object_pk=log_config.get("object_pk"),
                 content_type=log_config.get("content_type"),
                 requested_by=log_config.get("user"),
                 request_url=log_config.get("request_url"),
@@ -538,15 +609,17 @@
         envelope_stage_data.recipient_status = recipient_status
         # envelope_stage_data.updated_at = timezone.now()
         envelope_stage_data.save()
 
         LOGGER.debug(f"END process_docusign_notification: {envelope_id}")
 
     except Exception as e:
-        LOGGER.error(f"Exception while extracting status from Webhook notification: {e}")
+        LOGGER.error(
+            f"Exception while extracting status from Webhook notification: {e}"
+        )
         if log_config:
             log_entry = log_config.get("model")(
                 loan=log_config.get("loan"),
                 object_pk=log_config.get("object_pk"),
                 content_type=log_config.get("content_type"),
                 requested_by=log_config.get("user"),
                 request_url=log_config.get("request_url"),
@@ -558,23 +631,27 @@
                 tin=log_config.get("tin"),
                 request_ip=log_config.get("request_ip"),
                 response_code=log_config.get("response_code"),
                 event_type=event_type,
                 event=event_value,
             )
             log_entry.save()
-        raise Exception("Exception while extracting status from Webhook notification!") from e
+        raise Exception(
+            "Exception while extracting status from Webhook notification!"
+        ) from e
     return envelope_output
 
 
 def ComputeHash(secret, payload):
     hashBytes = hmac.new(secret, msg=payload, digestmod=hashlib.sha256).digest()
     base64Hash = base64.b64encode(hashBytes)
     return base64Hash
 
 
 def HashIsValid(secret, payload, verify):
     return hmac.compare_digest(verify, ComputeHash(secret, payload))
 
 
 def validate_received_webhook(secret, payload, verify):
-    return HashIsValid(secret=secret.encode(), payload=payload, verify=verify.encode())
+    return HashIsValid(
+        secret=secret.encode(), payload=payload, verify=verify.encode()
+    )
```

### Comparing `los_docusign-0.6.6/los_docusign/utils/validators.py` & `los_docusign-0.6.7/los_docusign/utils/validators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #
 # Created on Tue Dec 21 2021
 #
 # Copyright (c) 2021 Lenders Cooperative, a division of Summit Technology Group, Inc.
 #
 import os
-from urllib import request, response
+
 import phonenumbers
-from phonenumbers.phonenumberutil import NumberParseException
 from django.core.exceptions import ValidationError
+from phonenumbers.phonenumberutil import NumberParseException
 
 
 def validate_excel_file_extension(value):
     ext = os.path.splitext(value.name)[1]  # [0] returns path+filename
     valid_extensions = [".xls", ".xlsx", ".csv"]
     if not ext.lower() in valid_extensions:
-        raise ValidationError(u"Unsupported file extension. Must be Excel File")
+        raise ValidationError("Unsupported file extension. Must be Excel File")
 
 
 def validate_file_extension(value):
     ext = os.path.splitext(value.name)[1]  # [0] returns path+filename
     valid_extensions = [
         ".pdf",
         ".xls",
@@ -27,15 +27,16 @@
         ".doc",
         ".docx",
         ".jpg",
         ".jpeg",
         ".png",
     ]
     if not ext.lower() in valid_extensions:
-        raise ValidationError(u"Unsupported file extension.")
+        raise ValidationError("Unsupported file extension.")
+
 
 def validate_payload(payload):
     request_payload = payload
     signers = request_payload["recipients"]["signers"]
     documents = request_payload["documents"]
     status = request_payload["status"]
     emailSubject = request_payload["emailSubject"]
@@ -44,63 +45,72 @@
         response = "DocuSign Failure : Status is not set"
         return response
     if emailSubject is None or emailSubject == "":
         response = "DocuSign Failure : Email Subject is not set"
         return response
 
     for signer in signers:
-
         role = signer["roleName"]
         recipient_id = signer["recipientId"]
         recipient_type = signer["recipientType"]
         routingOrder = signer["routingOrder"]
         email = signer["email"]
         name = signer["name"]
 
         if "customFields" in signer:
             customfield = signer["customFields"]
             if customfield is None or customfield == "":
-                response = "DocuSign Failure : Signer's custom details are incorrect."
+                response = (
+                    "DocuSign Failure : Signer's custom details are incorrect."
+                )
                 return response
 
         if role is None or role == "":
             response = "DocuSign Failure : Signer's Role is not set"
             return response
         elif recipient_id is None or recipient_id == "":
-            response = "DocuSign Failure : Signer's Recipient Id is not present."
+            response = (
+                "DocuSign Failure : Signer's Recipient Id is not present."
+            )
             return response
         elif recipient_type is None or recipient_type == "":
-            response = "DocuSign Failure : Signer's Recipient Type is not present."
+            response = (
+                "DocuSign Failure : Signer's Recipient Type is not present."
+            )
             return response
         elif routingOrder is None or routingOrder == "":
             response = "DocuSign Failure : Signer's Routing Order is not set."
             return response
         elif email is None or email == "":
             response = "DocuSign Failure : Signer's email is not set."
             return response
         elif name is None or name == "":
             response = "DocuSign Failure : Signer's Name is not set."
             return response
 
-        if "idCheckConfigurationName" in signer and "phoneAuthentication" in signer:
+        if (
+            "idCheckConfigurationName" in signer
+            and "phoneAuthentication" in signer
+        ):
             authentication = signer["idCheckConfigurationName"]
             phone = signer["phoneAuthentication"]["senderProvidedNumbers"]
             if authentication == "Phone Auth $":
                 for phonenumber in phone:
                     phone_number = "+1" + phonenumber
                     try:
                         phone_number = phonenumbers.parse(phone_number, None)
                         if not phonenumbers.is_valid_number(phone_number):
                             response = "DocuSign Failure : Invalid phone number"
                             return response
-                    except NumberParseException as e:
-                        response = "DocuSign Failure : Phone Number must be 10 digits"
+                    except NumberParseException:
+                        response = (
+                            "DocuSign Failure : Phone Number must be 10 digits"
+                        )
                         return response
 
-            
     for document in documents:
         docName = document["name"]
         docExt = document["fileExtension"]
         docbase64 = document["documentBase64"]
         docId = document["documentId"]
 
         if docName is None or docName == "":
@@ -112,8 +122,8 @@
         elif docbase64 is None or docbase64 == "":
             response = "DocuSign Failure : Signer's Document is not present."
             return response
         elif docId is None or docId == "":
             response = "DocuSign Failure : Signer's Document Id is not set."
             return response
 
-    return "Success"
+    return "Success"
```

### Comparing `los_docusign-0.6.6/pyproject.toml` & `los_docusign-0.6.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "los_docusign"
-version = "0.6.6"
+version = "0.6.7"
 description = "Docusign Django Wrapper for integrating DocuSign with Django Application"
 authors = ["tejasb <tejas@thesummitgrp.com>"]
 homepage = "https://github.com/Lenders-Cooperative/Django-DocuSign"
 license = "BSD-3-Clause"
 readme = "README.md"
 include = [
     "LICENSE",
@@ -17,19 +17,20 @@
 django-utils-six = "^2.0"
 django-environ = "^0.4.5"
 PyJWT = "2.4"
 django-model-utils = "^4.1.1"
 django-lc-utils = "^0.2.1"
 requests = "^2.26.0"
 phonenumbers = "8.12.26"
+black = "22.3.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^5.2"
-black = "^21.8b0"
-isort = "^5.9.3"
+black = "22.3.0"
+isort = "^5.12.0"
 autoflake = "^1.4"
 pre-commit = "^2.15.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `los_docusign-0.6.6/PKG-INFO` & `los_docusign-0.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: los-docusign
-Version: 0.6.6
+Version: 0.6.7
 Summary: Docusign Django Wrapper for integrating DocuSign with Django Application
 Home-page: https://github.com/Lenders-Cooperative/Django-DocuSign
 License: BSD-3-Clause
 Author: tejasb
 Author-email: tejas@thesummitgrp.com
 Requires-Python: >=3.10.2,<4.0.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (==3.2.15)
 Requires-Dist: PyJWT (==2.4)
+Requires-Dist: black (==22.3.0)
 Requires-Dist: django-environ (>=0.4.5,<0.5.0)
 Requires-Dist: django-lc-utils (>=0.2.1,<0.3.0)
 Requires-Dist: django-model-utils (>=4.1.1,<5.0.0)
 Requires-Dist: django-utils-six (>=2.0,<3.0)
 Requires-Dist: docusign-esign (>=3.6.0,<4.0.0)
 Requires-Dist: phonenumbers (==8.12.26)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
```

