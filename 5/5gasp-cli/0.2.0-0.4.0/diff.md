# Comparing `tmp/5gasp_cli-0.2.0.tar.gz` & `tmp/5gasp_cli-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "5gasp_cli-0.2.0.tar", max compression
+gzip compressed data, was "5gasp_cli-0.4.0.tar", max compression
```

## Comparing `5gasp_cli-0.2.0.tar` & `5gasp_cli-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      910 2023-05-15 16:58:18.115402 5gasp_cli-0.2.0/README.md
--rw-r--r--   0        0        0      607 2023-05-15 22:01:07.194749 5gasp_cli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3684 2023-05-15 16:40:37.677360 5gasp_cli-0.2.0/src/CICDManagerAPIClient/apli_client.py
--rw-r--r--   0        0        0     5614 2023-05-11 22:15:06.228904 5gasp_cli-0.2.0/src/CICDManagerAPIClient/test_classes.py
--rw-r--r--   0        0        0     2414 2023-05-11 22:15:06.229439 5gasp_cli-0.2.0/src/DescriptorParser/parser.py
--rw-r--r--   0        0        0    16426 2023-05-15 17:12:08.185857 5gasp_cli-0.2.0/src/TestingDescriptorGenerator/descriptor_generator.py
--rw-r--r--   0        0        0        0 2023-05-09 15:54:29.636859 5gasp_cli-0.2.0/src/__init__.py
--rw-r--r--   0        0        0      672 2023-05-11 22:15:06.230529 5gasp_cli-0.2.0/src/helpers/base_testing_descriptor.py
--rw-r--r--   0        0        0     1131 2023-05-11 22:15:06.230827 5gasp_cli-0.2.0/src/helpers/beatiful_prints.py
--rw-r--r--   0        0        0      853 2023-05-11 22:15:06.231227 5gasp_cli-0.2.0/src/helpers/connection_point_tags.py
--rw-r--r--   0        0        0      487 2023-05-11 22:15:06.231586 5gasp_cli-0.2.0/src/helpers/constants.py
--rw-r--r--   0        0        0     5427 2023-05-15 21:51:18.512484 5gasp_cli-0.2.0/src/helpers/prompts.py
--rw-r--r--   0        0        0     7039 2023-05-15 16:40:46.698867 5gasp_cli-0.2.0/src/main.py
--rw-r--r--   0        0        0        0 2023-03-06 15:23:29.804346 5gasp_cli-0.2.0/src/tests/__init__.py
--rw-r--r--   0        0        0     1308 2023-04-04 15:56:18.183538 5gasp_cli-0.2.0/src/tests/resources/hackfest_multivdu_nsd.yaml
--rw-r--r--   0        0        0     1620 2023-04-04 15:56:18.184844 5gasp_cli-0.2.0/src/tests/test_cli.py
--rw-r--r--   0        0        0     3208 2023-05-02 13:57:22.146999 5gasp_cli-0.2.0/src/tests/test_output.yaml
--rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 5gasp_cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-18 16:53:02.302855 5gasp_cli-0.4.0/LICENSE
+-rw-r--r--   0        0        0      910 2023-05-18 16:53:02.303644 5gasp_cli-0.4.0/README.md
+-rw-r--r--   0        0        0      714 2023-05-18 17:00:03.475328 5gasp_cli-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3684 2023-05-18 16:53:02.307177 5gasp_cli-0.4.0/src/CICDManagerAPIClient/apli_client.py
+-rw-r--r--   0        0        0     5614 2023-05-11 22:15:06.228904 5gasp_cli-0.4.0/src/CICDManagerAPIClient/test_classes.py
+-rw-r--r--   0        0        0     2460 2023-05-18 16:53:41.081350 5gasp_cli-0.4.0/src/DescriptorParser/parser.py
+-rw-r--r--   0        0        0    16357 2023-05-18 16:58:37.123211 5gasp_cli-0.4.0/src/TestingDescriptorGenerator/descriptor_generator.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:54:29.636859 5gasp_cli-0.4.0/src/__init__.py
+-rw-r--r--   0        0        0      672 2023-05-11 22:15:06.230529 5gasp_cli-0.4.0/src/helpers/base_testing_descriptor.py
+-rw-r--r--   0        0        0     1131 2023-05-11 22:15:06.230827 5gasp_cli-0.4.0/src/helpers/beatiful_prints.py
+-rw-r--r--   0        0        0      853 2023-05-11 22:15:06.231227 5gasp_cli-0.4.0/src/helpers/connection_point_tags.py
+-rw-r--r--   0        0        0      487 2023-05-11 22:15:06.231586 5gasp_cli-0.4.0/src/helpers/constants.py
+-rw-r--r--   0        0        0     5427 2023-05-18 16:53:02.309692 5gasp_cli-0.4.0/src/helpers/prompts.py
+-rw-r--r--   0        0        0     7401 2023-05-18 16:53:02.310598 5gasp_cli-0.4.0/src/main.py
+-rw-r--r--   0        0        0        0 2023-03-06 15:23:29.804346 5gasp_cli-0.4.0/src/tests/__init__.py
+-rw-r--r--   0        0        0     1308 2023-04-04 15:56:18.183538 5gasp_cli-0.4.0/src/tests/resources/hackfest_multivdu_nsd.yaml
+-rw-r--r--   0        0        0     1620 2023-04-04 15:56:18.184844 5gasp_cli-0.4.0/src/tests/test_cli.py
+-rw-r--r--   0        0        0     3208 2023-05-02 13:57:22.146999 5gasp_cli-0.4.0/src/tests/test_output.yaml
+-rw-r--r--   0        0        0    36855 1970-01-01 00:00:00.000000 5gasp_cli-0.4.0/PKG-INFO
```

### Comparing `5gasp_cli-0.2.0/README.md` & `5gasp_cli-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `5gasp_cli-0.2.0/src/CICDManagerAPIClient/apli_client.py` & `5gasp_cli-0.4.0/src/CICDManagerAPIClient/apli_client.py`

 * *Files identical despite different names*

### Comparing `5gasp_cli-0.2.0/src/CICDManagerAPIClient/test_classes.py` & `5gasp_cli-0.4.0/src/CICDManagerAPIClient/test_classes.py`

 * *Files identical despite different names*

### Comparing `5gasp_cli-0.2.0/src/DescriptorParser/parser.py` & `5gasp_cli-0.4.0/src/DescriptorParser/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Eduardo Santos
 # @Date:   2023-02-18 15:26:20
 # @Last Modified by:   Rafael Direito
-# @Last Modified time: 2023-04-26 23:35:08
+# @Last Modified time: 2023-05-18 14:53:36
 
 import yaml
 from typing import List
 
 
 class ConnectionPointsParser:
     """
@@ -59,15 +59,16 @@
         connection_points = []
         for vnf in df['vnf-profile']:
             vnf_id = vnf['id']
             for constituent in vnf['virtual-link-connectivity']:
                 for constituent_cpd in constituent["constituent-cpd-id"]:
                     interface_id = constituent_cpd['constituent-cpd-id']
                     connection_points.append(
-                        "{{" + f"{ns_id}|{vnf_id}|{interface_id}" + "}}"
+                        "{{deployment_info|" + f"{ns_id}|{vnf_id}|" +
+                        f"{interface_id}" + "}}"
                     )
         return connection_points
 
     @property
     def connection_points(self):
         '''
         Get interfaces
```

### Comparing `5gasp_cli-0.2.0/src/TestingDescriptorGenerator/descriptor_generator.py` & `5gasp_cli-0.4.0/src/TestingDescriptorGenerator/descriptor_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Eduardo Santos
 # @Date:   2023-04-03 23:41:36
 # @Last Modified by:   Eduardo Santos
-# @Last Modified time: 2023-05-15 18:12:08
+# @Last Modified time: 2023-05-18 17:57:17
 
 # OS
 import os
 from ..helpers.beatiful_prints import PrintAsTable, PrintAsPanelColumns
 from ..helpers import prompts
 import yaml
 
@@ -322,15 +322,15 @@
     def _confirm_testing_descriptor_output_file(self):
         console = Console()
         location_ok = False
 
         while not location_ok:
             info = Text()
             info.append("\nThe Testing Descriptor will be saved in the " +
-                        "folllowing file: ", style="bold")
+                        "following file: ", style="bold")
             info.append(self.output_filepath + "\n")
             console.print(info)
             change_filepath = Confirm.ask(
                 "Do you wish to save the Testing Descriptor in a different " +
                 "file?")
 
             if not change_filepath:
@@ -350,28 +350,25 @@
                 elif os.path.isdir(file_path):
                     self.output_filepath = os.path.join(
                         file_path,
                         "testing-descriptor.yaml"
                     )
                     location_ok = True
                 else:
-                    print(file_path)
-                    print(os.path.isdir(file_path))
-                    print(os.path.isfile(file_path))
-                    info = Text("Impossible to save the Testing Descriptor " +
+                    info = Text("\nImpossible to save the Testing Descriptor " +
                                 "in the specified location " +
-                                f"{self.output_filepath}!",
+                                f"{file_path}! File or directory does not exist!",
                                 style="red")
                     console.print(info)
 
-            info = Text()
-            info.append("\nThe Testing Descriptor will be saved in the " +
-                        "folllowing file: ", style="bold")
-            info.append(self.output_filepath + "\n")
-            console.print(info)
+            #info = Text()
+            #info.append("\nThe Testing Descriptor will be saved in the " +
+            #            "following file: ", style="bold")
+            #info.append(self.output_filepath + "\n")
+            #console.print(info)
         return True
 
     def _save_testing_decritptor(self):
         testing_descriptor = BASE_TESTING_DESCRIPTOR
         testing_descriptor["test_info"]["netapp_id"] = self.netapp_name
         testing_descriptor["test_info"]["network_service_id"] = self.ns_name
         testing_descriptor["test_info"]["testbed_id"] = self.testbed_id
@@ -379,14 +376,15 @@
             f"Descriptor for the {self.netapp_name} Network Application"
 
         testcases = []
         for tc in self.test_cases:
             tc_dict = {
                 "testcase_id": tc.test_case_id,
                 "type": tc.test.test_type,
+                "scope": tc.test.test_type,
                 "name": tc.test.id,
                 "description": tc.description,
                 "parameters": []
             }
             for key, value in tc.test_variables.items():
                 tc_dict["parameters"].append(
                     {
@@ -406,27 +404,27 @@
                 testing_descriptor,
                 output_file,
                 default_flow_style=False,
                 sort_keys=False
             )
 
         console = Console()
-        console.print(Text("Generated Testing Descriptor:", style="bold"))
+        console.print(Text("\nGenerated Testing Descriptor:", style="bold"))
 
         print(
             yaml.dump(
                 testing_descriptor,
                 default_flow_style=False,
                 sort_keys=False
             )
         )
 
         info = Text()
         info.append("\nThe Testing Descriptor was saved in the " +
-                    "folllowing file: ", style="bold")
+                    "following file: ", style="bold")
         info.append(self.output_filepath)
         console.print(info)
 
     def _test_cases_menu(self):
 
         while True:
             # Show testcases
```

### Comparing `5gasp_cli-0.2.0/src/helpers/base_testing_descriptor.py` & `5gasp_cli-0.4.0/src/helpers/base_testing_descriptor.py`

 * *Files identical despite different names*

### Comparing `5gasp_cli-0.2.0/src/helpers/beatiful_prints.py` & `5gasp_cli-0.4.0/src/helpers/beatiful_prints.py`

 * *Files identical despite different names*

### Comparing `5gasp_cli-0.2.0/src/helpers/connection_point_tags.py` & `5gasp_cli-0.4.0/src/helpers/connection_point_tags.py`

 * *Files identical despite different names*

### Comparing `5gasp_cli-0.2.0/src/helpers/prompts.py` & `5gasp_cli-0.4.0/src/helpers/prompts.py`

 * *Files identical despite different names*

### Comparing `5gasp_cli-0.2.0/src/main.py` & `5gasp_cli-0.4.0/src/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # -*- coding: utf-8 -*-
 # @Author: Eduardo Santos
 # @Date:   2023-02-01 16:31:36
 # @Last Modified by:   Eduardo Santos
-# @Last Modified time: 2023-05-15 17:40:46
+# @Last Modified time: 2023-05-16 16:39:14
 
 from typing import List, Optional
 from .helpers.beatiful_prints import PrintAsTable, PrintAsPanelColumns
 from rich.prompt import Prompt, Confirm
+from rich.text import Text
+from rich.console import Console
 import typer
 
 from .CICDManagerAPIClient import apli_client as CICD_API_Client
 from .DescriptorParser.parser import ConnectionPointsParser
 from .TestingDescriptorGenerator.descriptor_generator import \
     TestingDescriptorGenerator
 from .helpers import constants as Constants
 from .helpers import prompts
 
 app = typer.Typer()
 state = {"verbose": False}
 
-
+ 
 def _list_testbeds(api_client, print_info=False, centered=False):
     testbeds = api_client.get_all_testbeds()
     # Print table with the available testbeds
     if print_info:
         table = PrintAsTable(
             header=["ID", "Name", "Description"],
             rows=[
@@ -52,14 +54,17 @@
         default="testing-descriptor.yaml",
         help="Output filepath"
     ),
     infer_tags_from_nsd: Optional[List[str]] = typer.Option(
         default=None
     )
 ):
+    console = Console()
+    text = Text()
+    
     # 1. Check if the developer wants to infer tags from an NSD
     if infer_tags_from_nsd:
         
         # Information Prompt
         prompts.connection_points_information_prompt()
 
         # Parse connection points information
@@ -92,15 +97,15 @@
         proceed = Confirm.ask(
             "\nDo you wish to proceed with the Test Descriptor's creation?"
             )
 
         # Exit if the developer does not want to proceed
         if not proceed:
             return
-
+    
     # 3. Ask for the Testing Descriptor initial information
     netapp_name = input("\n" + Constants.USER_PROMPTS.NETAPP_NAME.value)
     ns_name = input(Constants.USER_PROMPTS.NS_NAME.value)
 
     api_client = CICD_API_Client.CICDManagerAPIClient()
 
     # Print table with the available testbeds
@@ -119,14 +124,20 @@
 
     tests = _list_tests(
         api_client=api_client,
         testbed_id=testbed_id,
         print_info=False
     )
 
+    if not infer_tags_from_nsd:
+        text = Text("\nAs there was no NSD passed, there are no connection " +
+                    "points to be inferred. You can enter them manually."
+                    , style="bold")
+        console.print(text)
+
     generator = TestingDescriptorGenerator(
         connection_points=existing_connect_points if infer_tags_from_nsd else None,
         netapp_name=netapp_name,
         ns_name=ns_name,
         testbed_id=testbed_id,
         tests=tests,
         output_filepath=output_filepath
```

### Comparing `5gasp_cli-0.2.0/src/tests/resources/hackfest_multivdu_nsd.yaml` & `5gasp_cli-0.4.0/src/tests/resources/hackfest_multivdu_nsd.yaml`

 * *Files identical despite different names*

### Comparing `5gasp_cli-0.2.0/src/tests/test_cli.py` & `5gasp_cli-0.4.0/src/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `5gasp_cli-0.2.0/src/tests/test_output.yaml` & `5gasp_cli-0.4.0/src/tests/test_output.yaml`

 * *Files identical despite different names*

