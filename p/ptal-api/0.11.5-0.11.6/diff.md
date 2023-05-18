# Comparing `tmp/ptal_api-0.11.5.tar.gz` & `tmp/ptal_api-0.11.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptal_api-0.11.5.tar", max compression
+gzip compressed data, was "ptal_api-0.11.6.tar", max compression
```

## Comparing `ptal_api-0.11.5.tar` & `ptal_api-0.11.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      627 2023-04-24 11:37:57.778944 ptal_api-0.11.5/README.md
--rw-r--r--   0        0        0        0 2023-05-02 11:50:59.012123 ptal_api-0.11.5/ptal_api/__init__.py
--rw-r--r--   0        0        0    99057 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/adapter.py
--rw-r--r--   0        0        0      127 2023-04-24 11:37:57.778944 ptal_api-0.11.5/ptal_api/core/kb_sync/kb_iterator_config.py
--rw-r--r--   0        0        0      160 2023-04-24 11:37:57.778944 ptal_api-0.11.5/ptal_api/core/kb_sync/object_time_interval.py
--rw-r--r--   0        0        0      435 2023-04-24 11:37:57.778944 ptal_api-0.11.5/ptal_api/core/type_mapper/app_settings/logging.conf
--rw-r--r--   0        0        0      737 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/type_mapper/common/common.py
--rw-r--r--   0        0        0    12302 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/type_mapper/data_model/base_data_model.py
--rw-r--r--   0        0        0      904 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/type_mapper/data_model/config_data_model.py
--rw-r--r--   0        0        0     3255 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/type_mapper/data_model/custom_data_model.py
--rw-r--r--   0        0        0     3501 2023-04-24 11:37:57.778944 ptal_api-0.11.5/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
--rw-r--r--   0        0        0     2194 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/type_mapper/modules/custom_data_handler.py
--rw-r--r--   0        0        0     1464 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/type_mapper/modules/file_generator.py
--rw-r--r--   0        0        0     4556 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/type_mapper/modules/object_name_transformer.py
--rw-r--r--   0        0        0    23314 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/type_mapper/modules/type_mapping_generator.py
--rw-r--r--   0        0        0     1800 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
--rw-r--r--   0        0        0      418 2023-04-24 11:37:57.782944 ptal_api-0.11.5/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
--rw-r--r--   0        0        0      192 2023-04-24 11:37:57.782944 ptal_api-0.11.5/ptal_api/core/values/date_dataclass.py
--rw-r--r--   0        0        0     3279 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/values/value_mapping.py
--rw-r--r--   0        0        0        0 2023-05-02 11:50:59.016123 ptal_api-0.11.5/ptal_api/providers/__init__.py
--rw-r--r--   0        0        0     4668 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/providers/gql_providers.py
--rw-r--r--   0        0        0     1186 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/schema/README.md
--rw-r--r--   0        0        0        0 2023-05-02 11:50:59.016123 ptal_api-0.11.5/ptal_api/schema/__init__.py
--rw-r--r--   0        0        0   288920 2023-05-02 11:50:58.956123 ptal_api-0.11.5/ptal_api/schema/api_schema.py
--rw-r--r--   0        0        0    92810 2023-05-02 11:50:58.956123 ptal_api-0.11.5/ptal_api/schema/crawlers_api_schema.py
--rw-r--r--   0        0        0    74033 2023-05-02 11:50:58.956123 ptal_api-0.11.5/ptal_api/schema/tcontroller_api_schema.py
--rw-r--r--   0        0        0   136157 2023-05-02 11:50:58.956123 ptal_api-0.11.5/ptal_api/schema/utils_api_schema.py
--rw-r--r--   0        0        0     3662 2023-05-02 11:50:58.960123 ptal_api-0.11.5/ptal_api/scripts/type_mapper.py
--rw-r--r--   0        0        0        0 2023-05-02 11:50:59.016123 ptal_api-0.11.5/ptal_api/tdm_builder/__init__.py
--rw-r--r--   0        0        0     1211 2023-05-02 11:50:58.960123 ptal_api-0.11.5/ptal_api/tdm_builder/tdm_builder.py
--rw-r--r--   0        0        0     1871 2023-05-02 11:50:58.960123 ptal_api-0.11.5/pyproject.toml
--rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 ptal_api-0.11.5/PKG-INFO
+-rw-r--r--   0        0        0      627 2023-05-10 15:03:49.316666 ptal_api-0.11.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-18 08:44:15.320708 ptal_api-0.11.6/ptal_api/__init__.py
+-rw-r--r--   0        0        0    99304 2023-05-18 08:13:25.673710 ptal_api-0.11.6/ptal_api/adapter.py
+-rw-r--r--   0        0        0      184 2023-05-15 08:57:46.905949 ptal_api-0.11.6/ptal_api/core/kb_sync/kb_iterator_config.py
+-rw-r--r--   0        0        0      160 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/kb_sync/object_time_interval.py
+-rw-r--r--   0        0        0      435 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/app_settings/logging.conf
+-rw-r--r--   0        0        0      737 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/common/common.py
+-rw-r--r--   0        0        0    12302 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/data_model/base_data_model.py
+-rw-r--r--   0        0        0      904 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/data_model/config_data_model.py
+-rw-r--r--   0        0        0     3255 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/data_model/custom_data_model.py
+-rw-r--r--   0        0        0     3501 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
+-rw-r--r--   0        0        0     2194 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/modules/custom_data_handler.py
+-rw-r--r--   0        0        0     1464 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/modules/file_generator.py
+-rw-r--r--   0        0        0     4556 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/modules/object_name_transformer.py
+-rw-r--r--   0        0        0    23314 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/modules/type_mapping_generator.py
+-rw-r--r--   0        0        0     1800 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
+-rw-r--r--   0        0        0      418 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
+-rw-r--r--   0        0        0      192 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/values/date_dataclass.py
+-rw-r--r--   0        0        0     3279 2023-05-18 08:13:25.673710 ptal_api-0.11.6/ptal_api/core/values/value_mapping.py
+-rw-r--r--   0        0        0        0 2023-05-18 08:44:15.320708 ptal_api-0.11.6/ptal_api/providers/__init__.py
+-rw-r--r--   0        0        0     4668 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/providers/gql_providers.py
+-rw-r--r--   0        0        0     1186 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/schema/README.md
+-rw-r--r--   0        0        0        0 2023-05-18 08:44:15.320708 ptal_api-0.11.6/ptal_api/schema/__init__.py
+-rw-r--r--   0        0        0   289804 2023-05-18 08:28:23.351074 ptal_api-0.11.6/ptal_api/schema/api_schema.py
+-rw-r--r--   0        0        0    93413 2023-05-18 08:28:23.351074 ptal_api-0.11.6/ptal_api/schema/crawlers_api_schema.py
+-rw-r--r--   0        0        0    74033 2023-05-10 15:03:49.320666 ptal_api-0.11.6/ptal_api/schema/tcontroller_api_schema.py
+-rw-r--r--   0        0        0   136845 2023-05-18 08:28:23.351074 ptal_api-0.11.6/ptal_api/schema/utils_api_schema.py
+-rw-r--r--   0        0        0     3662 2023-05-10 15:03:49.320666 ptal_api-0.11.6/ptal_api/scripts/type_mapper.py
+-rw-r--r--   0        0        0        0 2023-05-18 08:44:15.320708 ptal_api-0.11.6/ptal_api/tdm_builder/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-10 15:03:49.320666 ptal_api-0.11.6/ptal_api/tdm_builder/tdm_builder.py
+-rw-r--r--   0        0        0     1871 2023-05-18 08:28:23.351074 ptal_api-0.11.6/pyproject.toml
+-rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 ptal_api-0.11.6/PKG-INFO
```

### Comparing `ptal_api-0.11.5/README.md` & `ptal_api-0.11.6/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.5/ptal_api/adapter.py` & `ptal_api-0.11.6/ptal_api/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         self._gql_client = gql_client
         self._utils_gql_client = utils_gql_client
         self._type_mapping_loader = type_mapping_loader if type_mapping_loader else TypeMappingLoader(logger)
         self._type_mapping = self._type_mapping_loader.load_type_mapping(type_mapping)
         self._limit = limit
         self._perform_synchronously = perform_synchronously
 
-        self.document_fields_truncated = ("id", "external_url")
+        self.document_fields_truncated = ("id", "external_url", "uuid",)
         self.document_fields = (
             "id",
             "title",
             "external_url",
             "publication_author",
             "publication_date",
             "internal_url",
@@ -144,25 +144,14 @@
             "system_registration_date",
             "system_update_date",
             "notes",
             "access_level",
             "trust_level",
             "uuid",
         )
-        self.document_fields_extended = (
-            "id",
-            "title",
-            "publication_author",
-            "publication_date",
-            "external_url",
-            "markers",
-            "notes",
-            "access_level",
-            "trust_level",
-        )
 
         self.document_text_fields_truncated = ("text",)
         self.document_text_fields = ("node_id", "text")
         self.document_text_metadata_fields = ("paragraph_type",)
 
         self.document_platform_fields = ("id", "name")
         self.document_account_fields = ("id", "name")
@@ -310,53 +299,53 @@
         concept_object.concept_type.__fields__(*self.concept_type_fields)
         if with_aliases:
             sv_frag = Fragment(StringValue, "StringFull")
             sv_frag.value()
             concept_object.list_alias.value.__fragment__(sv_frag)
         if with_properties:
             pcp: ConceptPropertyPagination = concept_object.pagination_concept_property(
-                offset=0, limit=10000, filter_settings=ConceptPropertyFilterSettings()
+                offset=0, limit=10000, filter_settings={}
             )
             lcp = pcp.list_concept_property()
             lcp.__fields__(*self.concept_property_fields)
             lcp.property_type().__fields__(*self.concept_property_type_fields)
             self._configure_output_value_fields(lcp.value)
         if with_links:
             pcl: ConceptLinkPagination = concept_object.pagination_concept_link(
-                offset=0, limit=10000, filter_settings=ConceptLinkFilterSettings()
+                offset=0, limit=10000, filter_settings={}
             )
             self._configure_output_link_fields(pcl.list_concept_link(), with_link_properties=with_link_properties)
         if with_facts:
             pcf: ConceptFactPagination = concept_object.pagination_concept_fact(
-                offset=0, limit=10000, filter_settings=DocumentLinkFilterSetting()
+                offset=0, limit=10000, filter_settings={}
             )
             lcf = pcf.list_concept_fact()
             lcf.__fields__(*self.concept_fact_fields)
             d = lcf.document()
-            d.__fields__(*self.document_fields_extended)
+            d.__fields__(*self.document_fields)
             dm = d.metadata()
             dm.platform().__fields__(*self.document_platform_fields)
             dm.account().__fields__(*self.document_account_fields)
         if with_potential_facts:
             lccf: List[ConceptCandidateFact] = concept_object.list_concept_candidate_fact()
             lccf.__fields__(*self.concept_fact_fields)
             d = lccf.document()
-            d.__fields__(*self.document_fields_extended)
+            d.__fields__(*self.document_fields)
             dm = d.metadata()
             dm.platform().__fields__(*self.document_platform_fields)
             dm.account().__fields__(*self.document_account_fields)
 
     def _configure_output_link_fields(self, link_object, with_link_properties=False):
         link_object.__fields__(*self.concept_link_fields)
         link_object.concept_from().__fields__(*self.concept_link_concept_from_fields)
         link_object.concept_to().__fields__(*self.concept_link_concept_to_fields)
         link_object.concept_link_type().__fields__(*self.concept_link_type_fields_truncated)
         if with_link_properties:
             pcp: ConceptPropertyPagination = link_object.pagination_concept_link_property(
-                offset=0, limit=10000, filter_settings=ConceptPropertyFilterSettings()
+                offset=0, limit=10000, filter_settings={}
             )
             lcp = pcp.list_concept_property()
             lcp.__fields__(*self.concept_property_fields)
             lcp.property_type().__fields__(*self.concept_property_type_fields)
             self._configure_output_value_fields(lcp.value)
 
     def _create_concept_with_input(
@@ -438,17 +427,20 @@
             old_timestamp_interval = None
             if had_creation_date:
                 old_timestamp_interval = copy(filter_settings.registration_date)
             start: int = getattr(old_timestamp_interval, "start", self.kb_iterator_config.earliest_created_time)
             end: int = getattr(old_timestamp_interval, "end", int(time()))
             middle: int = (end + start) // 2
 
-            for next_start, next_end in (start, middle), (middle, end):
+            for next_start, next_end in (start, middle), (middle + 1, end):
                 if next_start == start and next_end == end:
-                    logger.info(f"Processed only {self._limit} documents, {total - self._limit} ignored")
+                    logger.info(
+                        f"Processed only {self.kb_iterator_config.max_total_count} documents, "
+                        f"{total - self.kb_iterator_config.max_total_count} ignored"
+                    )
                     continue
                 filter_settings.registration_date = TimestampInterval(start=next_start, end=next_end)
                 yield from self.get_all_documents(
                     grouping=grouping,
                     filter_settings=filter_settings,
                     direction=direction,
                     sort_field=sort_field,
@@ -463,24 +455,25 @@
             return
         elif not total:
             return
 
         documents: Iterable = [None]
         i: int = 0
         while documents:
-            yield from self.get_documents(
+            documents = self.get_documents(
                 skip=i * self._limit,
                 take=self._limit,
                 grouping=grouping,
                 filter_settings=filter_settings,
                 direction=direction,
                 sort_field=sort_field,
                 extra_settings=extra_settings,
                 with_extended_information=with_extended_information,
             )
+            yield from documents
             i += 1
 
     def get_documents(
         self,
         skip: int = 0,
         take: Optional[int] = None,
         grouping: DocumentGrouping = "none",
@@ -507,15 +500,15 @@
             sort_field=sort_field,
             extra_settings=extra_settings,
             **pagination_story_kwargs,
         )
         ps.list_story().list_document().__fields__(*self.document_fields_truncated)
         m = ps.list_story().main()
         if with_extended_information:
-            m.__fields__(*self.document_fields_extended)
+            m.__fields__(*self.document_fields)
             mdm = m.metadata()
             mdm.platform().__fields__(*self.document_platform_fields)
             mdm.account().__fields__(*self.document_account_fields)
         else:
             m.__fields__(*self.document_fields_truncated)
         m.text().__fields__(*self.document_text_fields_truncated)
 
@@ -643,15 +636,15 @@
         c: Concept = op.concept(id=concept_id)
         pcf: ConceptFactPagination = c.pagination_concept_fact(
             filter_settings=filter_settings if filter_settings else DocumentLinkFilterSetting()
         )
         lcf = pcf.list_concept_fact()
         lcf.__fields__(*self.concept_fact_fields)
         d = lcf.document()
-        d.__fields__(*self.document_fields_extended)
+        d.__fields__(*self.document_fields)
         dm = d.metadata()
         dm.platform().__fields__(*self.document_platform_fields)
         dm.account().__fields__(*self.document_account_fields)
 
         res = self._gql_client.execute(op)
         res = op + res
 
@@ -695,17 +688,20 @@
             old_timestamp_interval = None
             if had_creation_date:
                 old_timestamp_interval = copy(filter_settings.creation_date)
             start: int = getattr(old_timestamp_interval, "start", self.kb_iterator_config.earliest_created_time)
             end: int = getattr(old_timestamp_interval, "end", int(time()))
             middle: int = (end + start) // 2
 
-            for next_start, next_end in (start, middle), (middle, end):
+            for next_start, next_end in (start, middle), (middle + 1, end):
                 if next_start == start and next_end == end:
-                    logger.info(f"Processed only {self._limit} concepts, {total - self._limit} ignored")
+                    logger.info(
+                        f"Processed only {self.kb_iterator_config.max_total_count} concepts, "
+                        f"{total - self.kb_iterator_config.max_total_count} ignored"
+                    )
                     continue
                 filter_settings.creation_date = TimestampInterval(start=next_start, end=next_end)
                 yield from self.get_all_concepts(
                     filter_settings=filter_settings,
                     direction=direction,
                     sort_field=sort_field,
                     with_aliases=with_aliases,
@@ -821,17 +817,20 @@
             old_timestamp_interval = None
             if had_creation_date:
                 old_timestamp_interval = copy(filter_settings.creation_date)
             start: int = getattr(old_timestamp_interval, "start", self.kb_iterator_config.earliest_created_time)
             end: int = getattr(old_timestamp_interval, "end", int(time()))
             middle: int = (end + start) // 2
 
-            for next_start, next_end in (start, middle), (middle, end):
+            for next_start, next_end in (start, middle), (middle + 1, end):
                 if next_start == start and next_end == end:
-                    logger.info(f"Processed only {self._limit} links, {total - self._limit} ignored")
+                    logger.info(
+                        f"Processed only {self.kb_iterator_config.max_total_count} links, "
+                        f"{total - self.kb_iterator_config.max_total_count} ignored"
+                    )
                     continue
                 filter_settings.creation_date = TimestampInterval(start=next_start, end=next_end)
                 for c in self.get_all_concept_links(
                     filter_settings=filter_settings, with_link_properties=with_link_properties
                 ):
                     yield c
 
@@ -2283,30 +2282,39 @@
         name: str,
         type_id: str,
         notes: str = None,
         take_first_result: bool = False,
         with_properties=False,
         with_links=False,
         with_link_properties=False,
+        with_facts=False,
+        with_potential_facts=False,
     ) -> Concept:
+        """Finds concept by near name"""
+
         if type_id:
             concept_filter_settings: ConceptFilterSettings = uas.ConceptFilterSettings(
                 exact_name=name, concept_type_ids=[type_id]
             )
         else:
             concept_filter_settings: ConceptFilterSettings = uas.ConceptFilterSettings(exact_name=name)
 
         op = Operation(uas.Mutation)
         goac = op.get_or_add_concept(
             filter_settings=concept_filter_settings,
             form=uas.ConceptMutationInput(name=name, concept_type_id=type_id, notes=notes),
             take_first_result=take_first_result,
         )
         self._configure_output_concept_fields(
-            goac, with_properties=with_properties, with_links=with_links, with_link_properties=with_link_properties
+            goac,
+            with_properties=with_properties,
+            with_links=with_links,
+            with_link_properties=with_link_properties,
+            with_facts=with_facts,
+            with_potential_facts=with_potential_facts
         )
 
         res = self._utils_gql_client.execute(op)
         res = op + res  # type: uas.Mutation
 
         if self.tdm_builder is not None:
             self.tdm_builder.add_concept_fact(res.get_or_add_concept)
```

### Comparing `ptal_api-0.11.5/ptal_api/core/type_mapper/common/common.py` & `ptal_api-0.11.6/ptal_api/core/type_mapper/common/common.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.5/ptal_api/core/type_mapper/data_model/base_data_model.py` & `ptal_api-0.11.6/ptal_api/core/type_mapper/data_model/base_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.5/ptal_api/core/type_mapper/data_model/config_data_model.py` & `ptal_api-0.11.6/ptal_api/core/type_mapper/data_model/config_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.5/ptal_api/core/type_mapper/data_model/custom_data_model.py` & `ptal_api-0.11.6/ptal_api/core/type_mapper/data_model/custom_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.5/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml` & `ptal_api-0.11.6/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.5/ptal_api/core/type_mapper/modules/custom_data_handler.py` & `ptal_api-0.11.6/ptal_api/core/type_mapper/modules/custom_data_handler.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.5/ptal_api/core/type_mapper/modules/file_generator.py` & `ptal_api-0.11.6/ptal_api/core/type_mapper/modules/file_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.5/ptal_api/core/type_mapper/modules/object_name_transformer.py` & `ptal_api-0.11.6/ptal_api/core/type_mapper/modules/object_name_transformer.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.5/ptal_api/core/type_mapper/modules/type_mapping_generator.py` & `ptal_api-0.11.6/ptal_api/core/type_mapper/modules/type_mapping_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.5/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py` & `ptal_api-0.11.6/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.5/ptal_api/core/values/value_mapping.py` & `ptal_api-0.11.6/ptal_api/core/values/value_mapping.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.5/ptal_api/providers/gql_providers.py` & `ptal_api-0.11.6/ptal_api/providers/gql_providers.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.5/ptal_api/schema/README.md` & `ptal_api-0.11.6/ptal_api/schema/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.5/ptal_api/schema/api_schema.py` & `ptal_api-0.11.6/ptal_api/schema/api_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,44 +456,46 @@
     markers = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(String)), graphql_name='markers')
     has_linked_issues = sgqlc.types.Field(Boolean, graphql_name='hasLinkedIssues')
     composite_concept_type_ids = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='compositeConceptTypeIds')
 
 
 class CompositeConceptTypeCreationInput(sgqlc.types.Input):
     __schema__ = api_schema
-    __field_names__ = ('name', 'root_concept_type_id', 'is_default', 'layout', 'has_supporting_documents', 'has_header_information', 'show_in_menu')
+    __field_names__ = ('name', 'root_concept_type_id', 'is_default', 'layout', 'has_supporting_documents', 'has_header_information', 'show_in_menu', 'hide_empty_rows')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     root_concept_type_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='rootConceptTypeId')
     is_default = sgqlc.types.Field(Boolean, graphql_name='isDefault')
     layout = sgqlc.types.Field(String, graphql_name='layout')
     has_supporting_documents = sgqlc.types.Field(Boolean, graphql_name='hasSupportingDocuments')
     has_header_information = sgqlc.types.Field(Boolean, graphql_name='hasHeaderInformation')
     show_in_menu = sgqlc.types.Field(Boolean, graphql_name='showInMenu')
+    hide_empty_rows = sgqlc.types.Field(Boolean, graphql_name='hideEmptyRows')
 
 
 class CompositeConceptTypeFilterSettings(sgqlc.types.Input):
     __schema__ = api_schema
     __field_names__ = ('name', 'creator', 'last_updater', 'registration_date', 'update_date')
     name = sgqlc.types.Field(String, graphql_name='name')
     creator = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='creator')
     last_updater = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='lastUpdater')
     registration_date = sgqlc.types.Field('TimestampInterval', graphql_name='registrationDate')
     update_date = sgqlc.types.Field('TimestampInterval', graphql_name='updateDate')
 
 
 class CompositeConceptTypeUpdateInput(sgqlc.types.Input):
     __schema__ = api_schema
-    __field_names__ = ('id', 'name', 'is_default', 'layout', 'has_supporting_documents', 'has_header_information', 'show_in_menu')
+    __field_names__ = ('id', 'name', 'is_default', 'layout', 'has_supporting_documents', 'has_header_information', 'show_in_menu', 'hide_empty_rows')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     is_default = sgqlc.types.Field(Boolean, graphql_name='isDefault')
     layout = sgqlc.types.Field(String, graphql_name='layout')
     has_supporting_documents = sgqlc.types.Field(Boolean, graphql_name='hasSupportingDocuments')
     has_header_information = sgqlc.types.Field(Boolean, graphql_name='hasHeaderInformation')
     show_in_menu = sgqlc.types.Field(Boolean, graphql_name='showInMenu')
+    hide_empty_rows = sgqlc.types.Field(Boolean, graphql_name='hideEmptyRows')
 
 
 class CompositeConceptTypeUpdateTemplateFilenameInput(sgqlc.types.Input):
     __schema__ = api_schema
     __field_names__ = ('id', 'filename', 'bucket')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     filename = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='filename')
@@ -647,20 +649,23 @@
     start_date = sgqlc.types.Field('DateTimeValueInput', graphql_name='startDate')
     end_date = sgqlc.types.Field('DateTimeValueInput', graphql_name='endDate')
     access_level_id = sgqlc.types.Field(ID, graphql_name='accessLevelId')
 
 
 class ConceptLinkFilterSettings(sgqlc.types.Input):
     __schema__ = api_schema
-    __field_names__ = ('is_event', 'concept_link_type', 'document_id', 'creation_date', 'update_date')
+    __field_names__ = ('is_event', 'concept_link_type', 'document_id', 'creation_date', 'update_date', 'other_concept_name', 'value_type', 'value')
     is_event = sgqlc.types.Field(Boolean, graphql_name='isEvent')
     concept_link_type = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='conceptLinkType')
     document_id = sgqlc.types.Field(ID, graphql_name='documentId')
     creation_date = sgqlc.types.Field('TimestampInterval', graphql_name='creationDate')
     update_date = sgqlc.types.Field('TimestampInterval', graphql_name='updateDate')
+    other_concept_name = sgqlc.types.Field(String, graphql_name='otherConceptName')
+    value_type = sgqlc.types.Field(ValueType, graphql_name='valueType')
+    value = sgqlc.types.Field('ValueFilter', graphql_name='value')
 
 
 class ConceptLinkPropertyInput(sgqlc.types.Input):
     __schema__ = api_schema
     __field_names__ = ('property_type_id', 'fact_info', 'notes', 'value_input', 'computable_value', 'link_id', 'is_main', 'start_date', 'end_date', 'access_level_id')
     property_type_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='propertyTypeId')
     fact_info = sgqlc.types.Field('FactInput', graphql_name='factInfo')
@@ -788,17 +793,19 @@
     start_date = sgqlc.types.Field('DateTimeValueInput', graphql_name='startDate')
     end_date = sgqlc.types.Field('DateTimeValueInput', graphql_name='endDate')
     access_level_id = sgqlc.types.Field(ID, graphql_name='accessLevelId')
 
 
 class ConceptPropertyFilterSettings(sgqlc.types.Input):
     __schema__ = api_schema
-    __field_names__ = ('only_main', 'document_id')
+    __field_names__ = ('only_main', 'document_id', 'value_type', 'value')
     only_main = sgqlc.types.Field(Boolean, graphql_name='onlyMain')
     document_id = sgqlc.types.Field(ID, graphql_name='documentId')
+    value_type = sgqlc.types.Field(ValueType, graphql_name='valueType')
+    value = sgqlc.types.Field('ValueFilter', graphql_name='value')
 
 
 class ConceptPropertyTypeCreationInput(sgqlc.types.Input):
     __schema__ = api_schema
     __field_names__ = ('concept_type_id', 'name', 'value_type_id', 'computable_formula', 'pretrained_rel_ext_models', 'notify_on_update')
     concept_type_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='conceptTypeId')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
@@ -1000,21 +1007,14 @@
 class DateTimeIntervalInput(sgqlc.types.Input):
     __schema__ = api_schema
     __field_names__ = ('start', 'end')
     start = sgqlc.types.Field('DateTimeValueInput', graphql_name='start')
     end = sgqlc.types.Field('DateTimeValueInput', graphql_name='end')
 
 
-class DateTimeIntervalPairInput(sgqlc.types.Input):
-    __schema__ = api_schema
-    __field_names__ = ('start', 'end')
-    start = sgqlc.types.Field(sgqlc.types.non_null(DateTimeIntervalInput), graphql_name='start')
-    end = sgqlc.types.Field(sgqlc.types.non_null(DateTimeIntervalInput), graphql_name='end')
-
-
 class DateTimeValueInput(sgqlc.types.Input):
     __schema__ = api_schema
     __field_names__ = ('date', 'time')
     date = sgqlc.types.Field(sgqlc.types.non_null(DateInput), graphql_name='date')
     time = sgqlc.types.Field('TimeInput', graphql_name='time')
 
 
@@ -1521,23 +1521,22 @@
     language = sgqlc.types.Field(String, graphql_name='language')
     markers = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='markers')
     params = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ParameterInput))), graphql_name='params')
 
 
 class PropertyFilterSettings(sgqlc.types.Input):
     __schema__ = api_schema
-    __field_names__ = ('property_type_id', 'component_id', 'property_type', 'string_filter', 'int_filter', 'double_filter', 'date_time_filter', 'date_time_interval_filter', 'geo_filter')
+    __field_names__ = ('property_type_id', 'component_id', 'property_type', 'string_filter', 'int_filter', 'double_filter', 'date_time_filter', 'geo_filter')
     property_type_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='propertyTypeId')
     component_id = sgqlc.types.Field(ID, graphql_name='componentId')
     property_type = sgqlc.types.Field(sgqlc.types.non_null(PropLinkOrConcept), graphql_name='propertyType')
     string_filter = sgqlc.types.Field('StringFilter', graphql_name='stringFilter')
     int_filter = sgqlc.types.Field(IntervalInt, graphql_name='intFilter')
     double_filter = sgqlc.types.Field(IntervalDouble, graphql_name='doubleFilter')
     date_time_filter = sgqlc.types.Field(DateTimeIntervalInput, graphql_name='dateTimeFilter')
-    date_time_interval_filter = sgqlc.types.Field(DateTimeIntervalPairInput, graphql_name='dateTimeIntervalFilter')
     geo_filter = sgqlc.types.Field(GeoPointWithNameFormInput, graphql_name='geoFilter')
 
 
 class RedmineIssueCreationInput(sgqlc.types.Input):
     __schema__ = api_schema
     __field_names__ = ('obj_ids', 'issue_type', 'subject', 'assignee_id', 'tracker_id', 'status_id', 'priority_id', 'due_to', 'description', 'related_issues')
     obj_ids = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='objIds')
@@ -1735,14 +1734,24 @@
 class UpdateCommentInput(sgqlc.types.Input):
     __schema__ = api_schema
     __field_names__ = ('task_change_id', 'comment')
     task_change_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='taskChangeId')
     comment = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='comment')
 
 
+class ValueFilter(sgqlc.types.Input):
+    __schema__ = api_schema
+    __field_names__ = ('string_filter', 'int_filter', 'double_filter', 'date_time_filter', 'geo_filter')
+    string_filter = sgqlc.types.Field(StringFilter, graphql_name='stringFilter')
+    int_filter = sgqlc.types.Field(IntervalInt, graphql_name='intFilter')
+    double_filter = sgqlc.types.Field(IntervalDouble, graphql_name='doubleFilter')
+    date_time_filter = sgqlc.types.Field(DateTimeIntervalInput, graphql_name='dateTimeFilter')
+    geo_filter = sgqlc.types.Field(GeoPointWithNameFormInput, graphql_name='geoFilter')
+
+
 class ValueInput(sgqlc.types.Input):
     __schema__ = api_schema
     __field_names__ = ('string_value_input', 'string_locale_value_input', 'int_value_input', 'double_value_input', 'geo_point_value_input', 'date_time_value_input', 'link_value_input')
     string_value_input = sgqlc.types.Field(StringValueInput, graphql_name='stringValueInput')
     string_locale_value_input = sgqlc.types.Field(StringLocaleValueInput, graphql_name='stringLocaleValueInput')
     int_value_input = sgqlc.types.Field(IntValueInput, graphql_name='intValueInput')
     double_value_input = sgqlc.types.Field(DoubleValueInput, graphql_name='doubleValueInput')
@@ -3852,22 +3861,23 @@
     image = sgqlc.types.Field(Image, graphql_name='image')
     metric = sgqlc.types.Field(sgqlc.types.non_null(AccountStatistics), graphql_name='metric')
     period = sgqlc.types.Field(sgqlc.types.non_null(DateTimeInterval), graphql_name='period')
 
 
 class CompositeConceptType(sgqlc.types.Type, RecordInterface):
     __schema__ = api_schema
-    __field_names__ = ('id', 'name', 'root_concept_type', 'is_default', 'layout', 'has_supporting_documents', 'has_header_information', 'metric', 'pagination_widget_type', 'list_widget_type', 'list_concept_link_types_composite_concept_type_consists_of', 'show_in_menu', 'internal_url')
+    __field_names__ = ('id', 'name', 'root_concept_type', 'is_default', 'layout', 'has_supporting_documents', 'has_header_information', 'hide_empty_rows', 'metric', 'pagination_widget_type', 'list_widget_type', 'list_concept_link_types_composite_concept_type_consists_of', 'show_in_menu', 'internal_url')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     root_concept_type = sgqlc.types.Field(sgqlc.types.non_null('ConceptType'), graphql_name='rootConceptType')
     is_default = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isDefault')
     layout = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='layout')
     has_supporting_documents = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hasSupportingDocuments')
     has_header_information = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hasHeaderInformation')
+    hide_empty_rows = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hideEmptyRows')
     metric = sgqlc.types.Field(sgqlc.types.non_null(CompositeConceptStatistics), graphql_name='metric')
     pagination_widget_type = sgqlc.types.Field(sgqlc.types.non_null(CompositeConceptTypeWidgetTypePagination), graphql_name='paginationWidgetType', args=sgqlc.types.ArgDict((
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('sort_direction', sgqlc.types.Arg(SortDirection, graphql_name='sortDirection', default='ascending')),
         ('sorting', sgqlc.types.Arg(CompositeConceptTypeWidgetTypeSorting, graphql_name='sorting', default='order')),
 ))
@@ -4049,23 +4059,23 @@
     parent_concept_link = sgqlc.types.Field(sgqlc.types.non_null(ConceptLink), graphql_name='parentConceptLink')
     access_level = sgqlc.types.Field(sgqlc.types.non_null(AccessLevel), graphql_name='accessLevel')
     concept_link_property = sgqlc.types.Field(sgqlc.types.non_null('ConceptProperty'), graphql_name='conceptLinkProperty')
 
 
 class ConceptLinkType(sgqlc.types.Type, RecordInterface):
     __schema__ = api_schema
-    __field_names__ = ('id', 'name', 'is_directed', 'is_hierarchical', 'concept_from_type', 'concept_to_type', 'pretrained_rel_ext_models', 'notify_on_update', 'pagination_concept_link_property_type', 'list_concept_link_property_type', 'metric')
+    __field_names__ = ('id', 'name', 'is_directed', 'is_hierarchical', 'pretrained_rel_ext_models', 'notify_on_update', 'concept_from_type', 'concept_to_type', 'pagination_concept_link_property_type', 'list_concept_link_property_type', 'metric')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     is_directed = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isDirected')
     is_hierarchical = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isHierarchical')
-    concept_from_type = sgqlc.types.Field(sgqlc.types.non_null('ConceptType'), graphql_name='conceptFromType')
-    concept_to_type = sgqlc.types.Field(sgqlc.types.non_null('ConceptType'), graphql_name='conceptToType')
     pretrained_rel_ext_models = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(RelExtModel))), graphql_name='pretrainedRelExtModels')
     notify_on_update = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='notifyOnUpdate')
+    concept_from_type = sgqlc.types.Field(sgqlc.types.non_null('ConceptType'), graphql_name='conceptFromType')
+    concept_to_type = sgqlc.types.Field(sgqlc.types.non_null('ConceptType'), graphql_name='conceptToType')
     pagination_concept_link_property_type = sgqlc.types.Field(sgqlc.types.non_null(ConceptPropertyTypePagination), graphql_name='paginationConceptLinkPropertyType', args=sgqlc.types.ArgDict((
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('filter_settings', sgqlc.types.Arg(sgqlc.types.non_null(ConceptPropertyTypeFilterSettings), graphql_name='filterSettings', default=None)),
         ('sort_direction', sgqlc.types.Arg(sgqlc.types.non_null(SortDirection), graphql_name='sortDirection', default=None)),
         ('sorting', sgqlc.types.Arg(sgqlc.types.non_null(ConceptTypeSorting), graphql_name='sorting', default=None)),
 ))
```

### Comparing `ptal_api-0.11.5/ptal_api/schema/crawlers_api_schema.py` & `ptal_api-0.11.6/ptal_api/schema/crawlers_api_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -736,15 +736,15 @@
     __field_names__ = ('total', 'list_metric')
     total = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='total')
     list_metric = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Metric))), graphql_name='listMetric')
 
 
 class Mutation(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('update_crawler', 'update_crawler_settings_arguments', 'delete_crawler_versions', 'delete_crawlers', 'update_site_map_crawler_body', 'add_crawl_state', 'update_crawl_state', 'delete_crawl_state', 'add_credential', 'update_credential', 'delete_credential', 'single_upload', 'add_job', 'delete_job', 'cancel_job', 'download_pending_jobs', 'schedule_uploaded_jobs', 'add_periodic_job', 'run_periodic_jobs', 'update_enable_jobs_scheduling', 'update_disable_jobs_scheduling', 'delete_periodic_job', 'update_periodic_job', 'update_periodic_job_settings_and_arguments', 'delete_project', 'delete_project_versions', 'add_project', 'update_project', 'update_project_settings_and_arguments', 'add_information_source_loader', 'delete_information_source_loader', 'add_recovery_job', 'cancel_recovery_job')
+    __field_names__ = ('update_crawler', 'update_crawler_settings_arguments', 'delete_crawler_versions', 'delete_crawlers', 'update_site_map_crawler_body', 'add_crawl_state', 'update_crawl_state', 'delete_crawl_state', 'add_credential', 'update_credential', 'delete_credential', 'single_upload', 'add_job', 'delete_job', 'cancel_job', 'suspend_job', 'resume_job', 'download_pending_jobs', 'schedule_uploaded_jobs', 'add_periodic_job', 'run_periodic_jobs', 'update_enable_jobs_scheduling', 'update_disable_jobs_scheduling', 'delete_periodic_job', 'update_periodic_job', 'update_periodic_job_settings_and_arguments', 'delete_project', 'delete_project_versions', 'add_project', 'update_project', 'update_project_settings_and_arguments', 'add_information_source_loader', 'delete_information_source_loader', 'add_recovery_job', 'cancel_recovery_job')
     update_crawler = sgqlc.types.Field(sgqlc.types.non_null('Crawler'), graphql_name='updateCrawler', args=sgqlc.types.ArgDict((
         ('crawler_update_input', sgqlc.types.Arg(sgqlc.types.non_null(CrawlerUpdateInput), graphql_name='crawlerUpdateInput', default=None)),
         ('crawler_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='crawlerId', default=None)),
         ('project_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='projectId', default=None)),
 ))
     )
     update_crawler_settings_arguments = sgqlc.types.Field(sgqlc.types.non_null('Crawler'), graphql_name='updateCrawlerSettingsArguments', args=sgqlc.types.ArgDict((
@@ -807,14 +807,22 @@
         ('ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='ids', default=None)),
 ))
     )
     cancel_job = sgqlc.types.Field(sgqlc.types.non_null('State'), graphql_name='cancelJob', args=sgqlc.types.ArgDict((
         ('ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='ids', default=None)),
 ))
     )
+    suspend_job = sgqlc.types.Field(sgqlc.types.non_null('State'), graphql_name='suspendJob', args=sgqlc.types.ArgDict((
+        ('ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='ids', default=None)),
+))
+    )
+    resume_job = sgqlc.types.Field(sgqlc.types.non_null('State'), graphql_name='resumeJob', args=sgqlc.types.ArgDict((
+        ('ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='ids', default=None)),
+))
+    )
     download_pending_jobs = sgqlc.types.Field(sgqlc.types.non_null(JSON), graphql_name='downloadPendingJobs')
     schedule_uploaded_jobs = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('Job'))), graphql_name='scheduleUploadedJobs', args=sgqlc.types.ArgDict((
         ('file_uuid', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='fileUUID', default=None)),
 ))
     )
     add_periodic_job = sgqlc.types.Field(sgqlc.types.non_null('PeriodicJob'), graphql_name='addPeriodicJob', args=sgqlc.types.ArgDict((
         ('periodic_job_input', sgqlc.types.Arg(sgqlc.types.non_null(PeriodicJobInput), graphql_name='periodicJobInput', default=None)),
@@ -1011,33 +1019,33 @@
     )
     pagination_job_logs = sgqlc.types.Field(sgqlc.types.non_null(LogPagination), graphql_name='paginationJobLogs', args=sgqlc.types.ArgDict((
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
         ('filter_settings', sgqlc.types.Arg(LogFilterSettings, graphql_name='filterSettings', default={})),
         ('direction', sgqlc.types.Arg(SortDirection, graphql_name='direction', default='descending')),
-        ('sort_field', sgqlc.types.Arg(LogSorting, graphql_name='sortField', default=None)),
+        ('sort_field', sgqlc.types.Arg(LogSorting, graphql_name='sortField', default='timestamp')),
 ))
     )
     pagination_job_requests = sgqlc.types.Field(sgqlc.types.non_null('RequestPagination'), graphql_name='paginationJobRequests', args=sgqlc.types.ArgDict((
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
         ('filter_settings', sgqlc.types.Arg(RequestFilterSettings, graphql_name='filterSettings', default={})),
         ('direction', sgqlc.types.Arg(SortDirection, graphql_name='direction', default='descending')),
-        ('sort_field', sgqlc.types.Arg(RequestSorting, graphql_name='sortField', default=None)),
+        ('sort_field', sgqlc.types.Arg(RequestSorting, graphql_name='sortField', default='timestamp')),
 ))
     )
     pagination_job_metrics = sgqlc.types.Field(sgqlc.types.non_null(MetricPagination), graphql_name='paginationJobMetrics', args=sgqlc.types.ArgDict((
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
         ('filter_settings', sgqlc.types.Arg(MetricFilterSettings, graphql_name='filterSettings', default={})),
         ('direction', sgqlc.types.Arg(SortDirection, graphql_name='direction', default='descending')),
-        ('sort_field', sgqlc.types.Arg(MetricSorting, graphql_name='sortField', default=None)),
+        ('sort_field', sgqlc.types.Arg(MetricSorting, graphql_name='sortField', default='timestamp')),
 ))
     )
     pagination_job = sgqlc.types.Field(sgqlc.types.non_null(JobPagination), graphql_name='paginationJob', args=sgqlc.types.ArgDict((
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('sort', sgqlc.types.Arg(JobSorting, graphql_name='sort', default={'jobPendingSorting': {'sort': 'id', 'direction': 'descending'}, 'jobRunningSorting': {'sort': 'id', 'direction': 'descending'}, 'jobFinishedSorting': {'sort': 'id', 'direction': 'descending'}})),
         ('jobs_filter_settings', sgqlc.types.Arg(JobsFilterSettings, graphql_name='jobsFilterSettings', default={})),
@@ -1057,33 +1065,33 @@
     )
     pagination_periodic_job_logs = sgqlc.types.Field(sgqlc.types.non_null(LogPagination), graphql_name='paginationPeriodicJobLogs', args=sgqlc.types.ArgDict((
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
         ('filter_settings', sgqlc.types.Arg(LogFilterSettings, graphql_name='filterSettings', default={})),
         ('direction', sgqlc.types.Arg(SortDirection, graphql_name='direction', default='descending')),
-        ('sort_field', sgqlc.types.Arg(LogSorting, graphql_name='sortField', default=None)),
+        ('sort_field', sgqlc.types.Arg(LogSorting, graphql_name='sortField', default='timestamp')),
 ))
     )
     pagination_periodic_job_requests = sgqlc.types.Field(sgqlc.types.non_null('RequestPagination'), graphql_name='paginationPeriodicJobRequests', args=sgqlc.types.ArgDict((
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
         ('filter_settings', sgqlc.types.Arg(RequestFilterSettings, graphql_name='filterSettings', default={})),
         ('direction', sgqlc.types.Arg(SortDirection, graphql_name='direction', default='descending')),
-        ('sort_field', sgqlc.types.Arg(RequestSorting, graphql_name='sortField', default=None)),
+        ('sort_field', sgqlc.types.Arg(RequestSorting, graphql_name='sortField', default='timestamp')),
 ))
     )
     pagination_periodic_job_metrics = sgqlc.types.Field(sgqlc.types.non_null(MetricPagination), graphql_name='paginationPeriodicJobMetrics', args=sgqlc.types.ArgDict((
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
         ('filter_settings', sgqlc.types.Arg(MetricFilterSettings, graphql_name='filterSettings', default={})),
         ('direction', sgqlc.types.Arg(SortDirection, graphql_name='direction', default='descending')),
-        ('sort_field', sgqlc.types.Arg(MetricSorting, graphql_name='sortField', default=None)),
+        ('sort_field', sgqlc.types.Arg(MetricSorting, graphql_name='sortField', default='timestamp')),
 ))
     )
     check_periodic_job_by_input = sgqlc.types.Field('PeriodicJob', graphql_name='checkPeriodicJobByInput', args=sgqlc.types.ArgDict((
         ('periodic_job_input', sgqlc.types.Arg(sgqlc.types.non_null(PeriodicJobInput), graphql_name='periodicJobInput', default=None)),
 ))
     )
     project = sgqlc.types.Field(sgqlc.types.non_null('Project'), graphql_name='project', args=sgqlc.types.ArgDict((
```

### Comparing `ptal_api-0.11.5/ptal_api/schema/tcontroller_api_schema.py` & `ptal_api-0.11.6/ptal_api/schema/tcontroller_api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.5/ptal_api/schema/utils_api_schema.py` & `ptal_api-0.11.6/ptal_api/schema/utils_api_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,20 +273,23 @@
     update_date = sgqlc.types.Field('TimestampInterval', graphql_name='updateDate')
     markers = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(String)), graphql_name='markers')
     has_linked_issues = sgqlc.types.Field(Boolean, graphql_name='hasLinkedIssues')
 
 
 class ConceptLinkFilterSettings(sgqlc.types.Input):
     __schema__ = utils_api_schema
-    __field_names__ = ('is_event', 'concept_link_type', 'document_id', 'creation_date', 'update_date')
+    __field_names__ = ('is_event', 'concept_link_type', 'document_id', 'creation_date', 'update_date', 'other_concept_name', 'value_type', 'value')
     is_event = sgqlc.types.Field(Boolean, graphql_name='isEvent')
     concept_link_type = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='conceptLinkType')
     document_id = sgqlc.types.Field(ID, graphql_name='documentId')
     creation_date = sgqlc.types.Field('TimestampInterval', graphql_name='creationDate')
     update_date = sgqlc.types.Field('TimestampInterval', graphql_name='updateDate')
+    other_concept_name = sgqlc.types.Field(String, graphql_name='otherConceptName')
+    value_type = sgqlc.types.Field(ValueType, graphql_name='valueType')
+    value = sgqlc.types.Field('ValueFilter', graphql_name='value')
 
 
 class ConceptLinkTypeFilterSettings(sgqlc.types.Input):
     __schema__ = utils_api_schema
     __field_names__ = ('name', 'concept_from_type_id', 'concept_to_type_id', 'concept_type_and_event_filter', 'is_directed', 'is_hierarchical', 'creator', 'last_updater', 'registration_date', 'update_date', 'has_rel_ext_models')
     name = sgqlc.types.Field(String, graphql_name='name')
     concept_from_type_id = sgqlc.types.Field(ID, graphql_name='conceptFromTypeId')
@@ -327,17 +330,19 @@
     access_level_id = sgqlc.types.Field(ID, graphql_name='accessLevelId')
     start_date = sgqlc.types.Field('DateTimeValueInput', graphql_name='startDate')
     end_date = sgqlc.types.Field('DateTimeValueInput', graphql_name='endDate')
 
 
 class ConceptPropertyFilterSettings(sgqlc.types.Input):
     __schema__ = utils_api_schema
-    __field_names__ = ('only_main', 'document_id')
+    __field_names__ = ('only_main', 'document_id', 'value_type', 'value')
     only_main = sgqlc.types.Field(Boolean, graphql_name='onlyMain')
     document_id = sgqlc.types.Field(ID, graphql_name='documentId')
+    value_type = sgqlc.types.Field(ValueType, graphql_name='valueType')
+    value = sgqlc.types.Field('ValueFilter', graphql_name='value')
 
 
 class ConceptPropertyTypeFilterSettings(sgqlc.types.Input):
     __schema__ = utils_api_schema
     __field_names__ = ('name', 'concept_type_id', 'concept_link_type_id', 'concept_value_type_id', 'value_type', 'concept_type_from_link_type_id')
     name = sgqlc.types.Field(String, graphql_name='name')
     concept_type_id = sgqlc.types.Field(ID, graphql_name='conceptTypeId')
@@ -358,21 +363,14 @@
 class DateTimeIntervalInput(sgqlc.types.Input):
     __schema__ = utils_api_schema
     __field_names__ = ('start', 'end')
     start = sgqlc.types.Field('DateTimeValueInput', graphql_name='start')
     end = sgqlc.types.Field('DateTimeValueInput', graphql_name='end')
 
 
-class DateTimeIntervalPairInput(sgqlc.types.Input):
-    __schema__ = utils_api_schema
-    __field_names__ = ('start', 'end')
-    start = sgqlc.types.Field(sgqlc.types.non_null(DateTimeIntervalInput), graphql_name='start')
-    end = sgqlc.types.Field(sgqlc.types.non_null(DateTimeIntervalInput), graphql_name='end')
-
-
 class DateTimeValueInput(sgqlc.types.Input):
     __schema__ = utils_api_schema
     __field_names__ = ('date', 'time')
     date = sgqlc.types.Field(sgqlc.types.non_null(DateInput), graphql_name='date')
     time = sgqlc.types.Field('TimeInput', graphql_name='time')
 
 
@@ -558,23 +556,22 @@
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     platform_type = sgqlc.types.Field(sgqlc.types.non_null(PlatformType), graphql_name='platformType')
     url = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='url')
 
 
 class PropertyFilterSettings(sgqlc.types.Input):
     __schema__ = utils_api_schema
-    __field_names__ = ('property_type_id', 'component_id', 'property_type', 'string_filter', 'int_filter', 'double_filter', 'date_time_filter', 'date_time_interval_filter', 'geo_filter')
+    __field_names__ = ('property_type_id', 'component_id', 'property_type', 'string_filter', 'int_filter', 'double_filter', 'date_time_filter', 'geo_filter')
     property_type_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='propertyTypeId')
     component_id = sgqlc.types.Field(ID, graphql_name='componentId')
     property_type = sgqlc.types.Field(sgqlc.types.non_null(PropLinkOrConcept), graphql_name='propertyType')
     string_filter = sgqlc.types.Field('StringFilter', graphql_name='stringFilter')
     int_filter = sgqlc.types.Field(IntervalInt, graphql_name='intFilter')
     double_filter = sgqlc.types.Field(IntervalDouble, graphql_name='doubleFilter')
     date_time_filter = sgqlc.types.Field(DateTimeIntervalInput, graphql_name='dateTimeFilter')
-    date_time_interval_filter = sgqlc.types.Field(DateTimeIntervalPairInput, graphql_name='dateTimeIntervalFilter')
     geo_filter = sgqlc.types.Field(GeoPointWithNameFormInput, graphql_name='geoFilter')
 
 
 class ResearchMapContentSelectInput(sgqlc.types.Input):
     __schema__ = utils_api_schema
     __field_names__ = ('nodes',)
     nodes = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='nodes')
@@ -625,14 +622,24 @@
 class TimestampInterval(sgqlc.types.Input):
     __schema__ = utils_api_schema
     __field_names__ = ('start', 'end')
     start = sgqlc.types.Field(UnixTime, graphql_name='start')
     end = sgqlc.types.Field(UnixTime, graphql_name='end')
 
 
+class ValueFilter(sgqlc.types.Input):
+    __schema__ = utils_api_schema
+    __field_names__ = ('string_filter', 'int_filter', 'double_filter', 'date_time_filter', 'geo_filter')
+    string_filter = sgqlc.types.Field(StringFilter, graphql_name='stringFilter')
+    int_filter = sgqlc.types.Field(IntervalInt, graphql_name='intFilter')
+    double_filter = sgqlc.types.Field(IntervalDouble, graphql_name='doubleFilter')
+    date_time_filter = sgqlc.types.Field(DateTimeIntervalInput, graphql_name='dateTimeFilter')
+    geo_filter = sgqlc.types.Field(GeoPointWithNameFormInput, graphql_name='geoFilter')
+
+
 class conceptTypeAndEventFilter(sgqlc.types.Input):
     __schema__ = utils_api_schema
     __field_names__ = ('full_type', 'is_event')
     full_type = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='fullType')
     is_event = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isEvent')
 
 
@@ -1529,22 +1536,23 @@
     image = sgqlc.types.Field(Image, graphql_name='image')
     metric = sgqlc.types.Field(sgqlc.types.non_null(AccountStatistics), graphql_name='metric')
     period = sgqlc.types.Field(sgqlc.types.non_null(DateTimeInterval), graphql_name='period')
 
 
 class CompositeConceptType(sgqlc.types.Type, RecordInterface):
     __schema__ = utils_api_schema
-    __field_names__ = ('id', 'name', 'root_concept_type', 'is_default', 'layout', 'has_supporting_documents', 'has_header_information', 'metric', 'pagination_widget_type', 'list_widget_type', 'list_concept_link_types_composite_concept_type_consists_of', 'show_in_menu', 'internal_url')
+    __field_names__ = ('id', 'name', 'root_concept_type', 'is_default', 'layout', 'has_supporting_documents', 'has_header_information', 'hide_empty_rows', 'metric', 'pagination_widget_type', 'list_widget_type', 'list_concept_link_types_composite_concept_type_consists_of', 'show_in_menu', 'internal_url')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     root_concept_type = sgqlc.types.Field(sgqlc.types.non_null('ConceptType'), graphql_name='rootConceptType')
     is_default = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isDefault')
     layout = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='layout')
     has_supporting_documents = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hasSupportingDocuments')
     has_header_information = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hasHeaderInformation')
+    hide_empty_rows = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hideEmptyRows')
     metric = sgqlc.types.Field(sgqlc.types.non_null(CompositeConceptStatistics), graphql_name='metric')
     pagination_widget_type = sgqlc.types.Field(sgqlc.types.non_null(CompositeConceptTypeWidgetTypePagination), graphql_name='paginationWidgetType', args=sgqlc.types.ArgDict((
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('sort_direction', sgqlc.types.Arg(SortDirection, graphql_name='sortDirection', default='ascending')),
         ('sorting', sgqlc.types.Arg(CompositeConceptTypeWidgetTypeSorting, graphql_name='sorting', default='order')),
 ))
@@ -1726,23 +1734,23 @@
     parent_concept_link = sgqlc.types.Field(sgqlc.types.non_null(ConceptLink), graphql_name='parentConceptLink')
     access_level = sgqlc.types.Field(sgqlc.types.non_null(AccessLevel), graphql_name='accessLevel')
     concept_link_property = sgqlc.types.Field(sgqlc.types.non_null('ConceptProperty'), graphql_name='conceptLinkProperty')
 
 
 class ConceptLinkType(sgqlc.types.Type, RecordInterface):
     __schema__ = utils_api_schema
-    __field_names__ = ('id', 'name', 'is_directed', 'is_hierarchical', 'concept_from_type', 'concept_to_type', 'pretrained_rel_ext_models', 'notify_on_update', 'pagination_concept_link_property_type', 'list_concept_link_property_type', 'metric')
+    __field_names__ = ('id', 'name', 'is_directed', 'is_hierarchical', 'pretrained_rel_ext_models', 'notify_on_update', 'concept_from_type', 'concept_to_type', 'pagination_concept_link_property_type', 'list_concept_link_property_type', 'metric')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     is_directed = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isDirected')
     is_hierarchical = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isHierarchical')
-    concept_from_type = sgqlc.types.Field(sgqlc.types.non_null('ConceptType'), graphql_name='conceptFromType')
-    concept_to_type = sgqlc.types.Field(sgqlc.types.non_null('ConceptType'), graphql_name='conceptToType')
     pretrained_rel_ext_models = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(RelExtModel))), graphql_name='pretrainedRelExtModels')
     notify_on_update = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='notifyOnUpdate')
+    concept_from_type = sgqlc.types.Field(sgqlc.types.non_null('ConceptType'), graphql_name='conceptFromType')
+    concept_to_type = sgqlc.types.Field(sgqlc.types.non_null('ConceptType'), graphql_name='conceptToType')
     pagination_concept_link_property_type = sgqlc.types.Field(sgqlc.types.non_null(ConceptPropertyTypePagination), graphql_name='paginationConceptLinkPropertyType', args=sgqlc.types.ArgDict((
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('filter_settings', sgqlc.types.Arg(sgqlc.types.non_null(ConceptPropertyTypeFilterSettings), graphql_name='filterSettings', default=None)),
         ('sort_direction', sgqlc.types.Arg(sgqlc.types.non_null(SortDirection), graphql_name='sortDirection', default=None)),
         ('sorting', sgqlc.types.Arg(sgqlc.types.non_null(ConceptTypeSorting), graphql_name='sorting', default=None)),
 ))
```

### Comparing `ptal_api-0.11.5/ptal_api/scripts/type_mapper.py` & `ptal_api-0.11.6/ptal_api/scripts/type_mapper.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.5/ptal_api/tdm_builder/tdm_builder.py` & `ptal_api-0.11.6/ptal_api/tdm_builder/tdm_builder.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.5/pyproject.toml` & `ptal_api-0.11.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ptal-api"
-version = "0.11.5"
+version = "0.11.6"
 description = "TALISMAN API adapter"
 authors = ["Evgeny Bechkalo <bechkalo@ispras.ru>", "Ivan Medvedev <medvedev.iv@ispras.ru>", "Alexey Isakov <isakov@ispras.ru>"]
 readme = "README.md"
 packages = [{include = "ptal_api"}]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Programming Language :: Python :: 3',
```

### Comparing `ptal_api-0.11.5/PKG-INFO` & `ptal_api-0.11.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptal-api
-Version: 0.11.5
+Version: 0.11.6
 Summary: TALISMAN API adapter
 Author: Evgeny Bechkalo
 Author-email: bechkalo@ispras.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

