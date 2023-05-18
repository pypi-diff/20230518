# Comparing `tmp/ontogpt-0.2.6.tar.gz` & `tmp/ontogpt-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontogpt-0.2.6.tar", max compression
+gzip compressed data, was "ontogpt-0.2.7.tar", max compression
```

## Comparing `ontogpt-0.2.6.tar` & `ontogpt-0.2.7.tar`

### file list

```diff
@@ -1,110 +1,112 @@
--rw-r--r--   0        0        0     1485 2023-05-15 22:47:38.293546 ontogpt-0.2.6/LICENSE
--rw-r--r--   0        0        0    13196 2023-05-15 22:47:38.293546 ontogpt-0.2.6/README.md
--rw-r--r--   0        0        0     2417 2023-05-15 22:48:44.354069 ontogpt-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      219 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/__init__.py
--rw-r--r--   0        0        0    32676 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/cli.py
--rw-r--r--   0        0        0      244 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/clients/__init__.py
--rw-r--r--   0        0        0     6962 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/clients/openai_client.py
--rw-r--r--   0        0        0     2921 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/clients/pubmed_client.py
--rw-r--r--   0        0        0      617 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/clients/soup_client.py
--rw-r--r--   0        0        0     1122 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/clients/wikipedia_client.py
--rw-r--r--   0        0        0      684 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/conf/synonymizer-conf.yaml
--rw-r--r--   0        0        0       81 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/converters/__init__.py
--rw-r--r--   0        0        0     5289 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/converters/ontology_converter.py
--rw-r--r--   0        0        0       59 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/engines/__init__.py
--rw-r--r--   0        0        0     3748 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/engines/embedding_similarity_engine.py
--rw-r--r--   0        0        0    12456 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/engines/enrichment.py
--rw-r--r--   0        0        0    19185 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/engines/halo_engine.py
--rw-r--r--   0        0        0    24196 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/engines/knowledge_engine.py
--rw-r--r--   0        0        0      752 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/engines/resolver.py
--rw-r--r--   0        0        0    18520 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/engines/spires_engine.py
--rw-r--r--   0        0        0      719 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/engines/synonym_engine.py
--rw-r--r--   0        0        0       70 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/evaluation/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/evaluation/ctd/__init__.py
--rw-r--r--   0        0        0   425228 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz
--rw-r--r--   0        0        0   409439 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz
--rw-r--r--   0        0        0   413985 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/ctd/database/synonyms.yaml
--rw-r--r--   0        0        0    10390 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/ctd/eval_ctd.py
--rw-r--r--   0        0        0        0 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/drugmechdb/__init__.py
--rw-r--r--   0        0        0     2145 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py
--rw-r--r--   0        0        0     2027 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml
--rw-r--r--   0        0        0    10670 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py
--rw-r--r--   0        0        0        0 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/enrichment/__init__.py
--rw-r--r--   0        0        0    13726 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/enrichment/eval_enrichment.py
--rw-r--r--   0        0        0     2950 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/evaluation_engine.py
--rw-r--r--   0        0        0     6164 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/go/eval_go.py
--rw-r--r--   0        0        0        0 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/hpoa/__init__.py
--rw-r--r--   0        0        0     8973 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/hpoa/eval_hpoa.py
--rw-r--r--   0        0        0     1191 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt
--rw-r--r--   0        0        0        0 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt~
--rw-r--r--   0        0        0     4791 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml
--rwxr-xr-x   0        0        0       95 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/ibd/run.sh
--rwxr-xr-x   0        0        0       99 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/ibd/run.sh~
--rw-r--r--   0        0        0      586 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/resolver.py
--rw-r--r--   0        0        0        0 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/io/__init__.py
--rw-r--r--   0        0        0      386 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/io/exporter.py
--rw-r--r--   0        0        0     4329 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/io/html_exporter.py
--rw-r--r--   0        0        0     3255 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/io/markdown_exporter.py
--rw-r--r--   0        0        0     2350 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/io/owl_exporter.py
--rw-r--r--   0        0        0     1440 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/io/rdf_exporter.py
--rw-r--r--   0        0        0      899 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/io/yaml_wrapper.py
--rw-r--r--   0        0        0        0 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/prompts/__init__.py
--rw-r--r--   0        0        0      159 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/prompts/enrichment/__init__.py
--rw-r--r--   0        0        0     1257 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2
--rw-r--r--   0        0        0     1016 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2
--rw-r--r--   0        0        0      993 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2
--rw-r--r--   0        0        0      994 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2
--rw-r--r--   0        0        0      995 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2
--rw-r--r--   0        0        0      560 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/prompts/similarity/connections.jinja2
--rw-r--r--   0        0        0     2354 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/streamlit/spindoctor.py
--rw-r--r--   0        0        0       68 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/templates/__init__.py
--rw-r--r--   0        0        0     5942 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/templates/biological_process.py
--rw-r--r--   0        0        0     2027 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/templates/biological_process.yaml
--rw-r--r--   0        0        0     2938 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/templates/class_enrichment.py
--rw-r--r--   0        0        0     3192 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/templates/class_enrichment.yaml
--rw-r--r--   0        0        0     4519 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/composite_disease.yaml
--rw-r--r--   0        0        0     3593 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/core.py
--rw-r--r--   0        0        0     3445 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/core.yaml
--rw-r--r--   0        0        0     6210 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/ctd.py
--rw-r--r--   0        0        0     6683 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/ctd.yaml
--rw-r--r--   0        0        0     8878 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/diagnostic_procedure.py
--rw-r--r--   0        0        0     4774 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/diagnostic_procedure.yaml
--rw-r--r--   0        0        0     5466 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/drug.py
--rw-r--r--   0        0        0     1856 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/drug.yaml
--rw-r--r--   0        0        0     6092 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/environmental_sample.py
--rw-r--r--   0        0        0     2900 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/environmental_sample.yaml
--rw-r--r--   0        0        0     4709 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/gene_description_term.py
--rw-r--r--   0        0        0     1614 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/gene_description_term.yaml
--rw-r--r--   0        0        0     8172 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/gocam.py
--rw-r--r--   0        0        0     4871 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/gocam.yaml
--rw-r--r--   0        0        0     6813 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/halo.py
--rw-r--r--   0        0        0     2367 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/halo.yaml
--rw-r--r--   0        0        0     8165 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/ibd.py
--rw-r--r--   0        0        0     4869 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/ibd.yaml
--rw-r--r--   0        0        0     6097 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/mendelian_disease.py
--rw-r--r--   0        0        0     3130 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/mendelian_disease.yaml
--rw-r--r--   0        0        0     5384 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/metabolic_process.py
--rw-r--r--   0        0        0     1633 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/metabolic_process.yaml
--rw-r--r--   0        0        0     7156 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/metagenome_study.py
--rw-r--r--   0        0        0     3910 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/metagenome_study.yaml
--rw-r--r--   0        0        0     5072 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/ontology_class.py
--rw-r--r--   0        0        0     2686 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/ontology_class.yaml
--rw-r--r--   0        0        0     6136 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/ontology_issue.py
--rw-r--r--   0        0        0     3383 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/ontology_issue.yaml
--rw-r--r--   0        0        0     4887 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/phenotype.py
--rw-r--r--   0        0        0     1532 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/phenotype.yaml
--rw-r--r--   0        0        0     7501 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/reaction.py
--rw-r--r--   0        0        0     3187 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/reaction.yaml
--rw-r--r--   0        0        0     7222 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/recipe.py
--rw-r--r--   0        0        0     5792 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/recipe.yaml
--rw-r--r--   0        0        0     7847 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/treatment.py
--rw-r--r--   0        0        0     4485 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/treatment.yaml
--rw-r--r--   0        0        0        0 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/utils/__init__.py
--rw-r--r--   0        0        0     8799 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/utils/gene_set_utils.py
--rw-r--r--   0        0        0        0 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/webapp/__init__.py
--rw-r--r--   0        0        0      861 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/webapp/html/form.html
--rw-r--r--   0        0        0      201 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/webapp/html/results.html
--rw-r--r--   0        0        0      819 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/webapp/html/spindoctor/form.html
--rw-r--r--   0        0        0      205 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/webapp/html/spindoctor/results.html
--rw-r--r--   0        0        0     2767 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/webapp/main.py
--rw-r--r--   0        0        0    15658 1970-01-01 00:00:00.000000 ontogpt-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1485 2023-05-18 20:56:47.378187 ontogpt-0.2.7/LICENSE
+-rw-r--r--   0        0        0    13196 2023-05-18 20:56:47.378187 ontogpt-0.2.7/README.md
+-rw-r--r--   0        0        0     2417 2023-05-18 20:57:52.962670 ontogpt-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/__init__.py
+-rw-r--r--   0        0        0    32669 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/cli.py
+-rw-r--r--   0        0        0      244 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/clients/__init__.py
+-rw-r--r--   0        0        0     6962 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/clients/openai_client.py
+-rw-r--r--   0        0        0     2921 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/clients/pubmed_client.py
+-rw-r--r--   0        0        0      617 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/clients/soup_client.py
+-rw-r--r--   0        0        0     1122 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/clients/wikipedia_client.py
+-rw-r--r--   0        0        0      684 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/conf/synonymizer-conf.yaml
+-rw-r--r--   0        0        0       81 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/converters/__init__.py
+-rw-r--r--   0        0        0     5289 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/converters/ontology_converter.py
+-rw-r--r--   0        0        0       59 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/engines/__init__.py
+-rw-r--r--   0        0        0     3748 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/engines/embedding_similarity_engine.py
+-rw-r--r--   0        0        0    12456 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/engines/enrichment.py
+-rw-r--r--   0        0        0    19185 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/engines/halo_engine.py
+-rw-r--r--   0        0        0    24196 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/engines/knowledge_engine.py
+-rw-r--r--   0        0        0      752 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/engines/resolver.py
+-rw-r--r--   0        0        0    18520 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/engines/spires_engine.py
+-rw-r--r--   0        0        0      719 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/engines/synonym_engine.py
+-rw-r--r--   0        0        0       70 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/evaluation/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/evaluation/ctd/__init__.py
+-rw-r--r--   0        0        0   425228 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz
+-rw-r--r--   0        0        0   409439 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz
+-rw-r--r--   0        0        0   413985 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/ctd/database/synonyms.yaml
+-rw-r--r--   0        0        0    10390 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/ctd/eval_ctd.py
+-rw-r--r--   0        0        0        0 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/drugmechdb/__init__.py
+-rw-r--r--   0        0        0     2145 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py
+-rw-r--r--   0        0        0     2027 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml
+-rw-r--r--   0        0        0    10670 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py
+-rw-r--r--   0        0        0        0 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/enrichment/__init__.py
+-rw-r--r--   0        0        0    13726 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/enrichment/eval_enrichment.py
+-rw-r--r--   0        0        0     2950 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/evaluation_engine.py
+-rw-r--r--   0        0        0     6164 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/go/eval_go.py
+-rw-r--r--   0        0        0        0 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/hpoa/__init__.py
+-rw-r--r--   0        0        0     8973 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/hpoa/eval_hpoa.py
+-rw-r--r--   0        0        0     1191 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt
+-rw-r--r--   0        0        0        0 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt~
+-rw-r--r--   0        0        0     4791 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml
+-rwxr-xr-x   0        0        0       95 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/ibd/run.sh
+-rwxr-xr-x   0        0        0       99 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/ibd/run.sh~
+-rw-r--r--   0        0        0      586 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/resolver.py
+-rw-r--r--   0        0        0        0 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/io/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/io/exporter.py
+-rw-r--r--   0        0        0     4329 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/io/html_exporter.py
+-rw-r--r--   0        0        0     3255 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/io/markdown_exporter.py
+-rw-r--r--   0        0        0     2350 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/io/owl_exporter.py
+-rw-r--r--   0        0        0     1440 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/io/rdf_exporter.py
+-rw-r--r--   0        0        0      899 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/io/yaml_wrapper.py
+-rw-r--r--   0        0        0        0 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/prompts/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/prompts/enrichment/__init__.py
+-rw-r--r--   0        0        0     1257 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2
+-rw-r--r--   0        0        0     1016 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2
+-rw-r--r--   0        0        0      993 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2
+-rw-r--r--   0        0        0      994 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2
+-rw-r--r--   0        0        0      995 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2
+-rw-r--r--   0        0        0      560 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/prompts/similarity/connections.jinja2
+-rw-r--r--   0        0        0     2354 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/streamlit/spindoctor.py
+-rw-r--r--   0        0        0       68 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/__init__.py
+-rw-r--r--   0        0        0     5942 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/biological_process.py
+-rw-r--r--   0        0        0     2027 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/biological_process.yaml
+-rw-r--r--   0        0        0     2938 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/class_enrichment.py
+-rw-r--r--   0        0        0     3192 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/class_enrichment.yaml
+-rw-r--r--   0        0        0     4519 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/composite_disease.yaml
+-rw-r--r--   0        0        0     3593 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/core.py
+-rw-r--r--   0        0        0     3445 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/core.yaml
+-rw-r--r--   0        0        0     6210 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/ctd.py
+-rw-r--r--   0        0        0     6683 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/ctd.yaml
+-rw-r--r--   0        0        0     8878 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/diagnostic_procedure.py
+-rw-r--r--   0        0        0     4774 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/diagnostic_procedure.yaml
+-rw-r--r--   0        0        0     5466 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/drug.py
+-rw-r--r--   0        0        0     1856 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/drug.yaml
+-rw-r--r--   0        0        0     6092 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/environmental_sample.py
+-rw-r--r--   0        0        0     2900 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/environmental_sample.yaml
+-rw-r--r--   0        0        0     4709 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/gene_description_term.py
+-rw-r--r--   0        0        0     1614 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/gene_description_term.yaml
+-rw-r--r--   0        0        0     8172 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/gocam.py
+-rw-r--r--   0        0        0     4871 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/gocam.yaml
+-rw-r--r--   0        0        0     6813 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/halo.py
+-rw-r--r--   0        0        0     2367 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/halo.yaml
+-rw-r--r--   0        0        0     8165 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/ibd.py
+-rw-r--r--   0        0        0     4869 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/ibd.yaml
+-rw-r--r--   0        0        0     6097 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/mendelian_disease.py
+-rw-r--r--   0        0        0     3130 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/mendelian_disease.yaml
+-rw-r--r--   0        0        0     5384 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/metabolic_process.py
+-rw-r--r--   0        0        0     1633 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/metabolic_process.yaml
+-rw-r--r--   0        0        0     7156 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/metagenome_study.py
+-rw-r--r--   0        0        0     3910 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/metagenome_study.yaml
+-rw-r--r--   0        0        0     5072 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/ontology_class.py
+-rw-r--r--   0        0        0     2686 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/ontology_class.yaml
+-rw-r--r--   0        0        0     6136 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/ontology_issue.py
+-rw-r--r--   0        0        0     3383 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/ontology_issue.yaml
+-rw-r--r--   0        0        0     4887 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/phenotype.py
+-rw-r--r--   0        0        0     1532 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/phenotype.yaml
+-rw-r--r--   0        0        0     7501 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/reaction.py
+-rw-r--r--   0        0        0     3187 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/reaction.yaml
+-rw-r--r--   0        0        0     7222 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/recipe.py
+-rw-r--r--   0        0        0     5792 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/recipe.yaml
+-rw-r--r--   0        0        0     5467 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/templates/traits.py
+-rw-r--r--   0        0        0     3502 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/templates/traits.yaml
+-rw-r--r--   0        0        0     7847 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/templates/treatment.py
+-rw-r--r--   0        0        0     4485 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/templates/treatment.yaml
+-rw-r--r--   0        0        0        0 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/utils/__init__.py
+-rw-r--r--   0        0        0     8799 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/utils/gene_set_utils.py
+-rw-r--r--   0        0        0        0 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/webapp/__init__.py
+-rw-r--r--   0        0        0      861 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/webapp/html/form.html
+-rw-r--r--   0        0        0      201 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/webapp/html/results.html
+-rw-r--r--   0        0        0      819 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/webapp/html/spindoctor/form.html
+-rw-r--r--   0        0        0      205 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/webapp/html/spindoctor/results.html
+-rw-r--r--   0        0        0     2767 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/webapp/main.py
+-rw-r--r--   0        0        0    15658 1970-01-01 00:00:00.000000 ontogpt-0.2.7/PKG-INFO
```

### Comparing `ontogpt-0.2.6/LICENSE` & `ontogpt-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/README.md` & `ontogpt-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/pyproject.toml` & `ontogpt-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ontogpt"
-version = "0.2.6"
+version = "0.2.7"
 description = "OntoGPT"
 authors = ["Chris Mungall <cjmungall@lbl.gov>"]
 license = "BSD-3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.9.7 || >3.9.7,<4.0"
```

### Comparing `ontogpt-0.2.6/src/ontogpt/cli.py` & `ontogpt-0.2.7/src/ontogpt/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -411,15 +411,15 @@
     scraper = scrape_me(url)
     template = "recipe"
     logging.info(f"Creating for {template}")
     ke = SPIRESEngine(template, **kwargs)
     if settings.cache_db:
         ke.client.cache_db_path = settings.cache_db
     if settings.skip_annotators:
-        ke.client.skip_annotators = settings.skip_annotators
+        ke.skip_annotators = settings.skip_annotators
     if dictionary:
         ke.load_dictionary(dictionary)
     ingredients = "\n".join(scraper.ingredients())
     instructions = "\n".join(scraper.instructions_list())
     text = f"""
     Recipe: {scraper.title()}
     Ingredients:\n{ingredients}
```

### Comparing `ontogpt-0.2.6/src/ontogpt/clients/openai_client.py` & `ontogpt-0.2.7/src/ontogpt/clients/openai_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/clients/pubmed_client.py` & `ontogpt-0.2.7/src/ontogpt/clients/pubmed_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/clients/soup_client.py` & `ontogpt-0.2.7/src/ontogpt/clients/soup_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/clients/wikipedia_client.py` & `ontogpt-0.2.7/src/ontogpt/clients/wikipedia_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/conf/synonymizer-conf.yaml` & `ontogpt-0.2.7/src/ontogpt/conf/synonymizer-conf.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/converters/ontology_converter.py` & `ontogpt-0.2.7/src/ontogpt/converters/ontology_converter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/engines/embedding_similarity_engine.py` & `ontogpt-0.2.7/src/ontogpt/engines/embedding_similarity_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/engines/enrichment.py` & `ontogpt-0.2.7/src/ontogpt/engines/enrichment.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/engines/halo_engine.py` & `ontogpt-0.2.7/src/ontogpt/engines/halo_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/engines/knowledge_engine.py` & `ontogpt-0.2.7/src/ontogpt/engines/knowledge_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/engines/resolver.py` & `ontogpt-0.2.7/src/ontogpt/engines/resolver.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/engines/spires_engine.py` & `ontogpt-0.2.7/src/ontogpt/engines/spires_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/engines/synonym_engine.py` & `ontogpt-0.2.7/src/ontogpt/engines/synonym_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz` & `ontogpt-0.2.7/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz` & `ontogpt-0.2.7/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/evaluation/ctd/database/synonyms.yaml` & `ontogpt-0.2.7/src/ontogpt/evaluation/ctd/database/synonyms.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/evaluation/ctd/eval_ctd.py` & `ontogpt-0.2.7/src/ontogpt/evaluation/ctd/eval_ctd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py` & `ontogpt-0.2.7/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml` & `ontogpt-0.2.7/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py` & `ontogpt-0.2.7/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/evaluation/enrichment/eval_enrichment.py` & `ontogpt-0.2.7/src/ontogpt/evaluation/enrichment/eval_enrichment.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/evaluation/evaluation_engine.py` & `ontogpt-0.2.7/src/ontogpt/evaluation/evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/evaluation/go/eval_go.py` & `ontogpt-0.2.7/src/ontogpt/evaluation/go/eval_go.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/evaluation/hpoa/eval_hpoa.py` & `ontogpt-0.2.7/src/ontogpt/evaluation/hpoa/eval_hpoa.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt` & `ontogpt-0.2.7/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml` & `ontogpt-0.2.7/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/evaluation/resolver.py` & `ontogpt-0.2.7/src/ontogpt/evaluation/resolver.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/io/html_exporter.py` & `ontogpt-0.2.7/src/ontogpt/io/html_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/io/markdown_exporter.py` & `ontogpt-0.2.7/src/ontogpt/io/markdown_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/io/owl_exporter.py` & `ontogpt-0.2.7/src/ontogpt/io/owl_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/io/rdf_exporter.py` & `ontogpt-0.2.7/src/ontogpt/io/rdf_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/io/yaml_wrapper.py` & `ontogpt-0.2.7/src/ontogpt/io/yaml_wrapper.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2` & `ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2` & `ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2` & `ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2` & `ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2` & `ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/prompts/similarity/connections.jinja2` & `ontogpt-0.2.7/src/ontogpt/prompts/similarity/connections.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/streamlit/spindoctor.py` & `ontogpt-0.2.7/src/ontogpt/streamlit/spindoctor.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/biological_process.py` & `ontogpt-0.2.7/src/ontogpt/templates/biological_process.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/biological_process.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/biological_process.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/class_enrichment.py` & `ontogpt-0.2.7/src/ontogpt/templates/class_enrichment.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/class_enrichment.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/class_enrichment.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/composite_disease.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/composite_disease.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/core.py` & `ontogpt-0.2.7/src/ontogpt/templates/core.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/core.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/core.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/ctd.py` & `ontogpt-0.2.7/src/ontogpt/templates/ctd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/ctd.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/ctd.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/diagnostic_procedure.py` & `ontogpt-0.2.7/src/ontogpt/templates/diagnostic_procedure.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/diagnostic_procedure.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/diagnostic_procedure.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/drug.py` & `ontogpt-0.2.7/src/ontogpt/templates/drug.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/drug.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/drug.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/environmental_sample.py` & `ontogpt-0.2.7/src/ontogpt/templates/environmental_sample.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/environmental_sample.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/environmental_sample.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/gene_description_term.py` & `ontogpt-0.2.7/src/ontogpt/templates/gene_description_term.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/gene_description_term.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/gene_description_term.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/gocam.py` & `ontogpt-0.2.7/src/ontogpt/templates/gocam.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/gocam.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/gocam.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/halo.py` & `ontogpt-0.2.7/src/ontogpt/templates/halo.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/halo.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/halo.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/ibd.py` & `ontogpt-0.2.7/src/ontogpt/templates/ibd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/ibd.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/ibd.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/mendelian_disease.py` & `ontogpt-0.2.7/src/ontogpt/templates/mendelian_disease.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/mendelian_disease.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/mendelian_disease.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/metabolic_process.py` & `ontogpt-0.2.7/src/ontogpt/templates/metabolic_process.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/metabolic_process.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/metabolic_process.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/metagenome_study.py` & `ontogpt-0.2.7/src/ontogpt/templates/metagenome_study.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/metagenome_study.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/metagenome_study.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/ontology_class.py` & `ontogpt-0.2.7/src/ontogpt/templates/ontology_class.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/ontology_class.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/ontology_class.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/ontology_issue.py` & `ontogpt-0.2.7/src/ontogpt/templates/ontology_issue.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/ontology_issue.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/ontology_issue.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/phenotype.py` & `ontogpt-0.2.7/src/ontogpt/templates/phenotype.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/phenotype.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/phenotype.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/reaction.py` & `ontogpt-0.2.7/src/ontogpt/templates/reaction.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/reaction.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/reaction.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/recipe.py` & `ontogpt-0.2.7/src/ontogpt/templates/recipe.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/recipe.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/recipe.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/treatment.py` & `ontogpt-0.2.7/src/ontogpt/templates/treatment.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/templates/treatment.yaml` & `ontogpt-0.2.7/src/ontogpt/templates/treatment.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/utils/gene_set_utils.py` & `ontogpt-0.2.7/src/ontogpt/utils/gene_set_utils.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/webapp/html/form.html` & `ontogpt-0.2.7/src/ontogpt/webapp/html/form.html`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/webapp/html/spindoctor/form.html` & `ontogpt-0.2.7/src/ontogpt/webapp/html/spindoctor/form.html`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/src/ontogpt/webapp/main.py` & `ontogpt-0.2.7/src/ontogpt/webapp/main.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.6/PKG-INFO` & `ontogpt-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontogpt
-Version: 0.2.6
+Version: 0.2.7
 Summary: OntoGPT
 License: BSD-3
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

