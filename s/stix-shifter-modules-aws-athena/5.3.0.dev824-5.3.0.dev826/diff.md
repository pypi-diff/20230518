# Comparing `tmp/stix_shifter_modules_aws_athena-5.3.0.dev824-py2.py3-none-any.whl.zip` & `tmp/stix_shifter_modules_aws_athena-5.3.0.dev826-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,41 +1,39 @@
-Zip file size: 80875 bytes, number of entries: 39
--rw-rw-r--  2.0 unx        0 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/__init__.py
--rw-rw-r--  2.0 unx     1374 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/entry_point.py
--rw-rw-r--  2.0 unx   241540 b- defN 23-May-18 16:33 stix_shifter_modules/aws_athena/configuration/config.json
--rw-rw-r--  2.0 unx      229 b- defN 23-May-18 16:33 stix_shifter_modules/aws_athena/configuration/dialects.json
--rw-rw-r--  2.0 unx     4766 b- defN 23-May-18 16:33 stix_shifter_modules/aws_athena/configuration/lang_en.json
--rw-rw-r--  2.0 unx        0 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_translation/__init__.py
--rw-rw-r--  2.0 unx    22536 b- defN 23-May-18 16:33 stix_shifter_modules/aws_athena/stix_translation/json_to_stix_translator.py
--rw-rw-r--  2.0 unx    24044 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_translation/query_constructor.py
--rw-rw-r--  2.0 unx     1024 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_translation/query_translator.py
--rw-rw-r--  2.0 unx     1518 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_translation/results_translator.py
--rw-rw-r--  2.0 unx     1075 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_translation/transformers.py
--rw-rw-r--  2.0 unx     4765 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_config.json
--rw-rw-r--  2.0 unx     1894 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_from_stix_map.json
--rw-rw-r--  2.0 unx    10630 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_to_stix_map.json
--rw-rw-r--  2.0 unx      139 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_translation/json/hash_algorithm_map.json
--rw-rw-r--  2.0 unx     2439 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_translation/json/network_protocol_map.json
--rw-rw-r--  2.0 unx    18300 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_from_stix_map.json
--rw-rw-r--  2.0 unx    75711 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_to_stix_map.json
--rw-rw-r--  2.0 unx      591 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_translation/json/operators.json
--rw-rw-r--  2.0 unx      891 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_from_stix_map.json
--rw-rw-r--  2.0 unx     2464 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_to_stix_map.json
--rw-rw-r--  2.0 unx     1894 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/guardduty_from_stix_map.json
--rw-rw-r--  2.0 unx    18297 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/ocsf_from_stix_map.json
--rw-rw-r--  2.0 unx    94538 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/to_stix_map.json
--rw-rw-r--  2.0 unx      891 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/vpcflow_from_stix_map.json
--rw-rw-r--  2.0 unx        0 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_transmission/__init__.py
--rw-rw-r--  2.0 unx     4173 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_transmission/boto3_client.py
--rw-rw-r--  2.0 unx     1207 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_transmission/delete_connector.py
--rw-rw-r--  2.0 unx     1529 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_transmission/error_mapper.py
--rw-rw-r--  2.0 unx      878 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_transmission/ping_connector.py
--rw-rw-r--  2.0 unx     7443 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_transmission/query_connector.py
--rw-rw-r--  2.0 unx    14480 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_transmission/results_connector.py
--rw-rw-r--  2.0 unx     3175 b- defN 23-May-18 16:30 stix_shifter_modules/aws_athena/stix_transmission/status_connector.py
--rw-rw-r--  2.0 unx    12786 b- defN 23-May-18 16:33 stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/LICENSE.md
--rw-rw-r--  2.0 unx     8047 b- defN 23-May-18 16:33 stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/METADATA
--rw-rw-r--  2.0 unx     1418 b- defN 23-May-18 16:33 stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/NOTICE
--rw-rw-r--  2.0 unx      110 b- defN 23-May-18 16:33 stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/WHEEL
--rw-rw-r--  2.0 unx       21 b- defN 23-May-18 16:33 stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4859 b- defN 23-May-18 16:33 stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/RECORD
-39 files, 591676 bytes uncompressed, 72495 bytes compressed:  87.7%
+Zip file size: 79946 bytes, number of entries: 37
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/__init__.py
+-rw-rw-r--  2.0 unx     1374 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/entry_point.py
+-rw-rw-r--  2.0 unx   254103 b- defN 23-May-18 19:30 stix_shifter_modules/aws_athena/configuration/config.json
+-rw-rw-r--  2.0 unx      229 b- defN 23-May-18 19:30 stix_shifter_modules/aws_athena/configuration/dialects.json
+-rw-rw-r--  2.0 unx     4766 b- defN 23-May-18 19:30 stix_shifter_modules/aws_athena/configuration/lang_en.json
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_translation/__init__.py
+-rw-rw-r--  2.0 unx    22536 b- defN 23-May-18 19:30 stix_shifter_modules/aws_athena/stix_translation/json_to_stix_translator.py
+-rw-rw-r--  2.0 unx    24044 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_translation/query_constructor.py
+-rw-rw-r--  2.0 unx     1024 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_translation/query_translator.py
+-rw-rw-r--  2.0 unx     1522 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_translation/results_translator.py
+-rw-rw-r--  2.0 unx     1075 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_translation/transformers.py
+-rw-rw-r--  2.0 unx     4765 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_config.json
+-rw-rw-r--  2.0 unx     1894 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_from_stix_map.json
+-rw-rw-r--  2.0 unx      139 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_translation/json/hash_algorithm_map.json
+-rw-rw-r--  2.0 unx     2439 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_translation/json/network_protocol_map.json
+-rw-rw-r--  2.0 unx    18300 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_from_stix_map.json
+-rw-rw-r--  2.0 unx      591 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_translation/json/operators.json
+-rw-rw-r--  2.0 unx    95113 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_translation/json/to_stix_map.json
+-rw-rw-r--  2.0 unx      891 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_from_stix_map.json
+-rw-rw-r--  2.0 unx     1894 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/guardduty_from_stix_map.json
+-rw-rw-r--  2.0 unx    18297 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/ocsf_from_stix_map.json
+-rw-rw-r--  2.0 unx    94538 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/to_stix_map.json
+-rw-rw-r--  2.0 unx      891 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/vpcflow_from_stix_map.json
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_transmission/__init__.py
+-rw-rw-r--  2.0 unx     4173 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_transmission/boto3_client.py
+-rw-rw-r--  2.0 unx     1207 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_transmission/delete_connector.py
+-rw-rw-r--  2.0 unx     1529 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_transmission/error_mapper.py
+-rw-rw-r--  2.0 unx      878 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_transmission/ping_connector.py
+-rw-rw-r--  2.0 unx     7443 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_transmission/query_connector.py
+-rw-rw-r--  2.0 unx    14478 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_transmission/results_connector.py
+-rw-rw-r--  2.0 unx     3175 b- defN 23-May-18 19:28 stix_shifter_modules/aws_athena/stix_transmission/status_connector.py
+-rw-rw-r--  2.0 unx    12786 b- defN 23-May-18 19:30 stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/LICENSE.md
+-rw-rw-r--  2.0 unx     8047 b- defN 23-May-18 19:30 stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/METADATA
+-rw-rw-r--  2.0 unx     1418 b- defN 23-May-18 19:30 stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/NOTICE
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-18 19:30 stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       21 b- defN 23-May-18 19:30 stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4581 b- defN 23-May-18 19:30 stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/RECORD
+37 files, 610271 bytes uncompressed, 72044 bytes compressed:  88.2%
```

## zipnote {}

```diff
@@ -33,36 +33,30 @@
 
 Filename: stix_shifter_modules/aws_athena/stix_translation/json/guardduty_config.json
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_translation/json/guardduty_from_stix_map.json
 Comment: 
 
-Filename: stix_shifter_modules/aws_athena/stix_translation/json/guardduty_to_stix_map.json
-Comment: 
-
 Filename: stix_shifter_modules/aws_athena/stix_translation/json/hash_algorithm_map.json
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_translation/json/network_protocol_map.json
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_translation/json/ocsf_from_stix_map.json
 Comment: 
 
-Filename: stix_shifter_modules/aws_athena/stix_translation/json/ocsf_to_stix_map.json
-Comment: 
-
 Filename: stix_shifter_modules/aws_athena/stix_translation/json/operators.json
 Comment: 
 
-Filename: stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_from_stix_map.json
+Filename: stix_shifter_modules/aws_athena/stix_translation/json/to_stix_map.json
 Comment: 
 
-Filename: stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_to_stix_map.json
+Filename: stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_from_stix_map.json
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/guardduty_from_stix_map.json
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/ocsf_from_stix_map.json
 Comment: 
@@ -93,26 +87,26 @@
 
 Filename: stix_shifter_modules/aws_athena/stix_transmission/results_connector.py
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_transmission/status_connector.py
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/LICENSE.md
+Filename: stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/LICENSE.md
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/METADATA
+Filename: stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/METADATA
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/NOTICE
+Filename: stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/NOTICE
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/WHEEL
+Filename: stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/WHEEL
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/top_level.txt
+Filename: stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/top_level.txt
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/RECORD
+Filename: stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stix_shifter_modules/aws_athena/configuration/config.json

### Pretty-printed

 * *Similarity: 0.999891672405877%*

 * *Differences: {"'connection'": "{'options': {'result_limit': {'max': 10000000}, 'timeout': {'max': 3600}, "*

 * *                 "'mapping': {'default': {'to_stix_map': OrderedDict([('ocsf', "*

 * *                 "OrderedDict([('_time', [OrderedDict([('key', 'first_observed'), ('cybox', "*

 * *                 "False), ('transformer', 'EpochToTimestamp')]), OrderedDict([('key', "*

 * *                 "'last_observed'), ('cybox', False), ('transformer', 'EpochToTimestamp')]), "*

 * *                 "OrderedDict([('key', 'x-ibm-finding.time_o […]*

```diff
@@ -318,419 +318,14 @@
                                 ],
                                 "start": [
                                     "event_firstseen"
                                 ]
                             }
                         }
                     },
-                    "guardduty_to_stix_map": {
-                        "accountid": {
-                            "key": "x-aws-details.account_id",
-                            "object": "aws_details"
-                        },
-                        "description": {
-                            "key": "x-ibm-finding.description",
-                            "object": "ibm_finding"
-                        },
-                        "dnsrequest_resource_instancedetails_networkinterfaces_0_privateipaddress": [
-                            {
-                                "key": "ipv4-addr.value",
-                                "object": "dns_private_ip1"
-                            },
-                            {
-                                "key": "domain-name.resolves_to_refs",
-                                "object": "private_dns_name",
-                                "references": [
-                                    "dns_private_ip1"
-                                ]
-                            },
-                            {
-                                "key": "x-ibm-finding.src_ip_ref",
-                                "object": "ibm_finding",
-                                "references": "dns_private_ip1"
-                            },
-                            {
-                                "cybox": false,
-                                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
-                                "key": "ipv4-addr.x_aws_interface_id",
-                                "object": "dns_private_ip1"
-                            },
-                            {
-                                "cybox": false,
-                                "key": "ipv4-addr.x_aws_ip_type",
-                                "object": "dns_private_ip1",
-                                "value": "private"
-                            }
-                        ],
-                        "portprobe_resource_instancedetails_networkinterfaces_0_privateipaddress": [
-                            {
-                                "key": "ipv4-addr.value",
-                                "object": "pp_private_ip1"
-                            },
-                            {
-                                "key": "domain-name.resolves_to_refs",
-                                "object": "private_dns_name",
-                                "references": [
-                                    "pp_private_ip1"
-                                ]
-                            },
-                            {
-                                "key": "x-ibm-finding.src_ip_ref",
-                                "object": "ibm_finding",
-                                "references": "pp_private_ip1"
-                            },
-                            {
-                                "cybox": false,
-                                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
-                                "key": "ipv4-addr.x_aws_interface_id",
-                                "object": "pp_private_ip1"
-                            },
-                            {
-                                "cybox": false,
-                                "key": "ipv4-addr.x_aws_ip_type",
-                                "object": "pp_private_ip1",
-                                "value": "private"
-                            }
-                        ],
-                        "region": {
-                            "key": "x-aws-details.region",
-                            "object": "aws_details"
-                        },
-                        "resource_accesskeydetails_accesskeyid": {
-                            "key": "x-aws-api.access_key_id",
-                            "object": "api_details"
-                        },
-                        "resource_accesskeydetails_principalid": {
-                            "key": "user-account.user_id",
-                            "object": "api_user"
-                        },
-                        "resource_accesskeydetails_username": {
-                            "key": "user-account.account_login",
-                            "object": "api_user"
-                        },
-                        "resource_instancedetails_availabilityzone": {
-                            "key": "x-aws-instance.availability_zone",
-                            "object": "instance"
-                        },
-                        "resource_instancedetails_imageid": {
-                            "key": "x-aws-instance.image_id",
-                            "object": "instance"
-                        },
-                        "resource_instancedetails_instanceid": {
-                            "key": "x-aws-instance.instance_id",
-                            "object": "instance"
-                        },
-                        "resource_instancedetails_networkinterfaces_0_ipv6addresses_0": [
-                            {
-                                "key": "ipv6-addr.value",
-                                "object": "nc_ipv6_ip"
-                            },
-                            {
-                                "cybox": false,
-                                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
-                                "key": "ipv6-addr.x_aws_interface_id",
-                                "object": "nc_ipv6_ip"
-                            }
-                        ],
-                        "resource_instancedetails_networkinterfaces_0_privatednsname": [
-                            {
-                                "key": "domain-name.value",
-                                "object": "private_dns_name"
-                            }
-                        ],
-                        "resource_instancedetails_networkinterfaces_0_privateipaddress": [
-                            {
-                                "key": "ipv4-addr.value",
-                                "object": "nc_private_ip1"
-                            },
-                            {
-                                "key": "network-traffic.src_ref",
-                                "object": "nc_nt",
-                                "references": "nc_private_ip1"
-                            },
-                            {
-                                "key": "domain-name.resolves_to_refs",
-                                "object": "private_dns_name",
-                                "references": [
-                                    "nc_private_ip1"
-                                ]
-                            },
-                            {
-                                "key": "x-ibm-finding.src_ip_ref",
-                                "object": "ibm_finding",
-                                "references": "nc_private_ip1"
-                            },
-                            {
-                                "cybox": false,
-                                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
-                                "key": "ipv4-addr.x_aws_interface_id",
-                                "object": "nc_private_ip1"
-                            },
-                            {
-                                "cybox": false,
-                                "key": "ipv4-addr.x_aws_ip_type",
-                                "object": "nc_private_ip1",
-                                "value": "private"
-                            }
-                        ],
-                        "resource_instancedetails_networkinterfaces_0_publicdnsname": [
-                            {
-                                "key": "domain-name.value",
-                                "object": "nc_public_name"
-                            }
-                        ],
-                        "resource_instancedetails_networkinterfaces_0_publicip": [
-                            {
-                                "key": "ipv4-addr.value",
-                                "object": "nc_public_ip"
-                            },
-                            {
-                                "key": "domain-name.resolves_to_refs",
-                                "object": "nc_public_name",
-                                "references": [
-                                    "nc_public_ip"
-                                ]
-                            },
-                            {
-                                "cybox": false,
-                                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
-                                "key": "ipv4-addr.x_aws_interface_id",
-                                "object": "nc_public_ip"
-                            },
-                            {
-                                "cybox": false,
-                                "key": "ipv4-addr.x_aws_ip_type",
-                                "object": "nc_public_ip",
-                                "value": "public"
-                            }
-                        ],
-                        "resource_instancedetails_networkinterfaces_0_securitygroups_0_groupid": {
-                            "key": "x-aws-vpc.security_group_id",
-                            "object": "vpc"
-                        },
-                        "resource_instancedetails_networkinterfaces_0_securitygroups_0_groupname": {
-                            "key": "x-aws-vpc.security_group_name",
-                            "object": "vpc"
-                        },
-                        "resource_instancedetails_networkinterfaces_0_subnetid": {
-                            "key": "x-aws-vpc.subnet_id",
-                            "object": "vpc"
-                        },
-                        "resource_instancedetails_networkinterfaces_0_vpcid": {
-                            "key": "x-aws-vpc.vpc_id",
-                            "object": "vpc"
-                        },
-                        "resource_instancedetails_networkinterfaces_1_privatednsname": [
-                            {
-                                "key": "domain-name.value",
-                                "object": "nc_private_name2"
-                            }
-                        ],
-                        "resource_instancedetails_networkinterfaces_1_privateipaddress": [
-                            {
-                                "key": "ipv4-addr.value",
-                                "object": "nc_private_ip2"
-                            },
-                            {
-                                "key": "domain-name.resolves_to_refs",
-                                "object": "nc_private_name2",
-                                "references": [
-                                    "nc_private_ip2"
-                                ]
-                            },
-                            {
-                                "cybox": false,
-                                "ds_key": "resource_instancedetails_networkinterfaces_1_networkinterfaceid",
-                                "key": "ipv4-addr.x_aws_interface_id",
-                                "object": "nc_private_ip2"
-                            },
-                            {
-                                "cybox": false,
-                                "key": "ipv4-addr.x_aws_ip_type",
-                                "object": "nc_private_ip2",
-                                "value": "private"
-                            }
-                        ],
-                        "resource_instancedetails_platform": [
-                            {
-                                "key": "software.name",
-                                "object": "software"
-                            },
-                            {
-                                "key": "x-ibm-finding.src_os_ref",
-                                "object": "ibm_finding",
-                                "references": "software"
-                            }
-                        ],
-                        "service_action_awsapicallaction_api": {
-                            "key": "x-aws-api.api",
-                            "object": "api_details"
-                        },
-                        "service_action_awsapicallaction_remoteipdetails_ipaddressv4": [
-                            {
-                                "key": "ipv4-addr.value",
-                                "object": "api_remote_ip"
-                            },
-                            {
-                                "key": "x-ibm-finding.dst_ip_ref",
-                                "object": "ibm_finding",
-                                "references": "api_remote_ip"
-                            },
-                            {
-                                "cybox": false,
-                                "ds_key": "service_action_awsapicallaction_remoteipdetails_country_countryname",
-                                "key": "x-ibm-finding.dst_geolocation",
-                                "object": "ibm_finding"
-                            },
-                            {
-                                "cybox": false,
-                                "ds_key": "service_action_awsapicallaction_remoteipdetails_city_cityname",
-                                "key": "ipv4-addr.x_aws_remote_city_name",
-                                "object": "api_remote_ip"
-                            },
-                            {
-                                "cybox": false,
-                                "ds_key": "service_action_awsapicallaction_remoteipdetails_country_countryname",
-                                "key": "ipv4-addr.x_aws_remote_country_name",
-                                "object": "api_remote_ip"
-                            }
-                        ],
-                        "service_action_awsapicallaction_servicename": {
-                            "key": "x-aws-api.service_name",
-                            "object": "api_details"
-                        },
-                        "service_action_dnsrequestaction_domain": [
-                            {
-                                "key": "domain-name.value",
-                                "object": "dns_domain_name"
-                            }
-                        ],
-                        "service_action_networkconnectionaction_localportdetails_port": [
-                            {
-                                "key": "network-traffic.src_port",
-                                "object": "nc_nt",
-                                "transformer": "ToInteger"
-                            }
-                        ],
-                        "service_action_networkconnectionaction_protocol": [
-                            {
-                                "key": "network-traffic.protocols",
-                                "object": "nc_nt",
-                                "transformer": "ToLowercaseArray"
-                            }
-                        ],
-                        "service_action_networkconnectionaction_remoteipdetails_ipaddressv4": [
-                            {
-                                "key": "ipv4-addr.value",
-                                "object": "nc_remote_ip"
-                            },
-                            {
-                                "key": "network-traffic.dst_ref",
-                                "object": "nc_nt",
-                                "references": "nc_remote_ip"
-                            },
-                            {
-                                "key": "x-ibm-finding.dst_ip_ref",
-                                "object": "ibm_finding",
-                                "references": "nc_remote_ip"
-                            },
-                            {
-                                "cybox": false,
-                                "ds_key": "service_action_networkconnectionaction_remoteipdetails_country_countryname",
-                                "key": "x-ibm-finding.dst_geolocation",
-                                "object": "ibm_finding"
-                            },
-                            {
-                                "cybox": false,
-                                "ds_key": "service_action_networkconnectionaction_remoteipdetails_city_cityname",
-                                "key": "ipv4-addr.x_aws_remote_city_name",
-                                "object": "nc_remote_ip"
-                            },
-                            {
-                                "cybox": false,
-                                "ds_key": "service_action_networkconnectionaction_remoteipdetails_country_countryname",
-                                "key": "ipv4-addr.x_aws_remote_country_name",
-                                "object": "nc_remote_ip"
-                            }
-                        ],
-                        "service_action_networkconnectionaction_remoteportdetails_port": [
-                            {
-                                "key": "network-traffic.dst_port",
-                                "object": "nc_nt",
-                                "transformer": "ToInteger"
-                            }
-                        ],
-                        "service_action_portprobeaction_portprobedetails_0_localportdetails_port": [
-                            {
-                                "key": "x-ibm-finding.probe_port",
-                                "object": "ibm_finding"
-                            }
-                        ],
-                        "service_action_portprobeaction_portprobedetails_0_remoteipdetails_ipaddressv4": [
-                            {
-                                "key": "ipv4-addr.value",
-                                "object": "pp_remote_ip"
-                            },
-                            {
-                                "key": "x-ibm-finding.dst_ip_ref",
-                                "object": "ibm_finding",
-                                "references": "pp_remote_ip"
-                            },
-                            {
-                                "cybox": false,
-                                "ds_key": "service_action_portprobeaction_portprobedetails_0_remoteipdetails_country_countryname",
-                                "key": "x-ibm-finding.dst_geolocation",
-                                "object": "ibm_finding"
-                            },
-                            {
-                                "cybox": false,
-                                "ds_key": "service_action_portprobeaction_portprobedetails_0_remoteipdetails_city_cityname",
-                                "key": "ipv4-addr.x_aws_remote_city_name",
-                                "object": "pp_remote_ip"
-                            },
-                            {
-                                "cybox": false,
-                                "ds_key": "service_action_portprobeaction_portprobedetails_0_remoteipdetails_country_countryname",
-                                "key": "ipv4-addr.x_aws_remote_country_name",
-                                "object": "pp_remote_ip"
-                            }
-                        ],
-                        "service_eventfirstseen": [
-                            {
-                                "cybox": false,
-                                "key": "first_observed"
-                            },
-                            {
-                                "key": "x-ibm-finding.start",
-                                "object": "ibm_finding"
-                            }
-                        ],
-                        "service_eventlastseen": [
-                            {
-                                "cybox": false,
-                                "key": "last_observed"
-                            },
-                            {
-                                "key": "x-ibm-finding.end",
-                                "object": "ibm_finding"
-                            }
-                        ],
-                        "severity": {
-                            "key": "x-ibm-finding.severity",
-                            "object": "ibm_finding"
-                        },
-                        "title": {
-                            "key": "x-ibm-finding.name",
-                            "object": "ibm_finding"
-                        },
-                        "type": {
-                            "key": "x-ibm-finding.finding_type",
-                            "object": "ibm_finding"
-                        }
-                    },
                     "hash_algorithm_map": {
                         "0": "Unknown",
                         "1": "MD5",
                         "2": "SHA-1",
                         "3": "SHA-256",
                         "4": "SHA-512",
                         "5": "CTPH",
@@ -1695,2635 +1290,3165 @@
                                 ],
                                 "uid": [
                                     "resources.uid"
                                 ]
                             }
                         }
                     },
-                    "ocsf_to_stix_map": {
-                        "_time": [
-                            {
-                                "cybox": false,
-                                "key": "first_observed",
-                                "transformer": "EpochToTimestamp"
-                            },
-                            {
-                                "cybox": false,
-                                "key": "last_observed",
-                                "transformer": "EpochToTimestamp"
-                            },
-                            {
-                                "key": "x-ibm-finding.time_observed",
-                                "object": "ibm_finding",
-                                "transformer": "EpochToTimestamp"
-                            }
-                        ],
-                        "activity": {
-                            "key": "x-oca-event.action",
-                            "object": "x_oca_event"
-                        },
-                        "activity_id": {
-                            "key": "x-oca-event.code",
-                            "object": "x_oca_event",
-                            "transformer": "ToInteger"
-                        },
-                        "activity_name": {
-                            "key": "x-oca-event.action",
-                            "object": "x_oca_event"
-                        },
-                        "api": {
-                            "operation": {
-                                "key": "x-ocsf-cloud.operation",
-                                "object": "ocsf_cloud_api"
+                    "operators": {
+                        "ComparisonComparators.Equal": "=",
+                        "ComparisonComparators.GreaterThan": ">",
+                        "ComparisonComparators.GreaterThanOrEqual": ">=",
+                        "ComparisonComparators.In": "IN",
+                        "ComparisonComparators.LessThan": "<",
+                        "ComparisonComparators.LessThanOrEqual": "<=",
+                        "ComparisonComparators.Like": "LIKE",
+                        "ComparisonComparators.Matches": "REGEXP_LIKE",
+                        "ComparisonComparators.NotEqual": "!=",
+                        "ComparisonExpressionOperators.And": "AND",
+                        "ComparisonExpressionOperators.Or": "OR",
+                        "ObservationOperators.And": "INTERSECT",
+                        "ObservationOperators.Or": "UNION"
+                    },
+                    "to_stix_map": {
+                        "guardduty": {
+                            "accountid": {
+                                "key": "x-aws-details.account_id",
+                                "object": "aws_details"
                             },
-                            "request": {
-                                "flags": {
-                                    "key": "x-ocsf-cloud.request_flags",
-                                    "object": "ocsf_cloud_api",
-                                    "transformer": "ToLowercaseArray"
-                                },
-                                "uid": {
-                                    "key": "x-ocsf-cloud.request_uid",
-                                    "object": "ocsf_cloud_api"
-                                }
+                            "description": {
+                                "key": "x-ibm-finding.description",
+                                "object": "ibm_finding"
                             },
-                            "response": {
-                                "code": {
-                                    "key": "x-ocsf-cloud.response_code",
-                                    "object": "ocsf_cloud_api",
-                                    "transformer": "ToInteger"
+                            "dnsrequest_resource_instancedetails_networkinterfaces_0_privateipaddress": [
+                                {
+                                    "key": "ipv4-addr.value",
+                                    "object": "dns_private_ip1"
                                 },
-                                "error": {
-                                    "key": "x-ocsf-cloud.response_error",
-                                    "object": "ocsf_cloud_api"
+                                {
+                                    "key": "domain-name.resolves_to_refs",
+                                    "object": "private_dns_name",
+                                    "references": [
+                                        "dns_private_ip1"
+                                    ]
                                 },
-                                "error_message": {
-                                    "key": "x-ocsf-cloud.response_error_message",
-                                    "object": "ocsf_cloud_api"
+                                {
+                                    "key": "x-ibm-finding.src_ip_ref",
+                                    "object": "ibm_finding",
+                                    "references": "dns_private_ip1"
                                 },
-                                "flags": {
-                                    "key": "x-ocsf-cloud.response_flags",
-                                    "object": "ocsf_cloud_api",
-                                    "transformer": "ToLowercaseArray"
+                                {
+                                    "cybox": false,
+                                    "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
+                                    "key": "ipv4-addr.x_aws_interface_id",
+                                    "object": "dns_private_ip1"
                                 },
-                                "message": {
-                                    "key": "x-ocsf-cloud.response_message",
-                                    "object": "ocsf_cloud_api"
+                                {
+                                    "cybox": false,
+                                    "key": "ipv4-addr.x_aws_ip_type",
+                                    "object": "dns_private_ip1",
+                                    "value": "private"
                                 }
-                            },
-                            "service": {
-                                "labels": {
-                                    "key": "x-ocsf-cloud.service_labels",
-                                    "object": "ocsf_cloud_api",
-                                    "transformer": "ToLowercaseArray"
+                            ],
+                            "portprobe_resource_instancedetails_networkinterfaces_0_privateipaddress": [
+                                {
+                                    "key": "ipv4-addr.value",
+                                    "object": "pp_private_ip1"
                                 },
-                                "name": {
-                                    "key": "x-ocsf-cloud.service_name",
-                                    "object": "ocsf_cloud_api"
+                                {
+                                    "key": "domain-name.resolves_to_refs",
+                                    "object": "private_dns_name",
+                                    "references": [
+                                        "pp_private_ip1"
+                                    ]
                                 },
-                                "uid": {
-                                    "key": "x-ocsf-cloud.service_uid",
-                                    "object": "ocsf_cloud_api"
+                                {
+                                    "key": "x-ibm-finding.src_ip_ref",
+                                    "object": "ibm_finding",
+                                    "references": "pp_private_ip1"
                                 },
-                                "version": {
-                                    "key": "x-ocsf-cloud.service_uid",
-                                    "object": "ocsf_cloud_api"
-                                }
-                            },
-                            "version": {
-                                "key": "x-ocsf-cloud.api_version",
-                                "object": "ocsf_cloud_api"
-                            }
-                        },
-                        "attacks": {
-                            "tactics": {
-                                "name": {
-                                    "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.tactic_name",
-                                    "object": "ttp-tagging"
+                                {
+                                    "cybox": false,
+                                    "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
+                                    "key": "ipv4-addr.x_aws_interface_id",
+                                    "object": "pp_private_ip1"
                                 },
-                                "uid": {
-                                    "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.tactic_id",
-                                    "object": "ttp-tagging"
-                                }
-                            },
-                            "technique": {
-                                "name": [
-                                    {
-                                        "key": "x-ibm-ttp-tagging.name",
-                                        "object": "ttp-tagging"
-                                    },
-                                    {
-                                        "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.technique_name",
-                                        "object": "ttp-tagging"
-                                    },
-                                    {
-                                        "key": "x-ibm-finding.ttp_tagging_refs",
-                                        "object": "ibm_finding",
-                                        "references": [
-                                            "ttp-tagging"
-                                        ]
-                                    }
-                                ],
-                                "uid": {
-                                    "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.technique_id",
-                                    "object": "ttp-tagging"
+                                {
+                                    "cybox": false,
+                                    "key": "ipv4-addr.x_aws_ip_type",
+                                    "object": "pp_private_ip1",
+                                    "value": "private"
                                 }
-                            },
-                            "version": {
-                                "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.versoin",
-                                "object": "ttp-tagging"
-                            }
-                        },
-                        "category_name": {
-                            "key": "x-oca-event.category",
-                            "object": "x_oca_event"
-                        },
-                        "category_uid": {
-                            "key": "x-oca-event.code",
-                            "object": "x_oca_event",
-                            "transformer": "ToInteger"
-                        },
-                        "class_name": {
-                            "key": "x-oca-event.module",
-                            "object": "x_oca_event"
-                        },
-                        "class_uid": {
-                            "key": "x-oca-event.extensions.x-cloud-api.class_uid",
-                            "object": "x_oca_event",
-                            "transformer": "ToInteger"
-                        },
-                        "cloud": {
-                            "account_type": {
-                                "key": "x-ocsf-cloud.account_type",
-                                "object": "ocsf_cloud_api"
-                            },
-                            "account_type_id": {
-                                "key": "x-ocsf-cloud.account_type_id",
-                                "object": "ocsf_cloud_api",
-                                "transformer": "ToInteger"
-                            },
-                            "account_uid": {
-                                "key": "x-ocsf-cloud.account_uid",
-                                "object": "ocsf_cloud_api"
-                            },
-                            "org_uid": {
-                                "key": "x-ocsf-cloud.org_uid",
-                                "object": "ocsf_cloud_api"
-                            },
-                            "project_uid": {
-                                "key": "x-ocsf-cloud.project_uid",
-                                "object": "ocsf_cloud_api"
-                            },
-                            "provider": {
-                                "key": "x-ocsf-cloud.provider",
-                                "object": "ocsf_cloud_api"
-                            },
+                            ],
                             "region": {
-                                "key": "x-ocsf-cloud.region",
-                                "object": "ocsf_cloud_api"
+                                "key": "x-aws-details.region",
+                                "object": "aws_details"
                             },
-                            "resource_uid": {
-                                "key": "x-ocsf-cloud.resource_uid",
-                                "object": "ocsf_cloud_api"
+                            "resource_accesskeydetails_accesskeyid": {
+                                "key": "x-aws-api.access_key_id",
+                                "object": "api_details"
+                            },
+                            "resource_accesskeydetails_principalid": {
+                                "key": "user-account.user_id",
+                                "object": "api_user"
+                            },
+                            "resource_accesskeydetails_username": {
+                                "key": "user-account.account_login",
+                                "object": "api_user"
+                            },
+                            "resource_instancedetails_availabilityzone": {
+                                "key": "x-aws-instance.availability_zone",
+                                "object": "instance"
+                            },
+                            "resource_instancedetails_imageid": {
+                                "key": "x-aws-instance.image_id",
+                                "object": "instance"
+                            },
+                            "resource_instancedetails_instanceid": {
+                                "key": "x-aws-instance.instance_id",
+                                "object": "instance"
                             },
-                            "zone": {
-                                "key": "x-ocsf-cloud.zone",
-                                "object": "ocsf_cloud_api"
-                            }
-                        },
-                        "compliance": {
-                            "requirements": {
-                                "key": "x-ocsf-compliance.requirements",
-                                "object": "compliance"
-                            },
-                            "status": {
-                                "key": "x-ocsf-compliance.status",
-                                "object": "compliance"
-                            },
-                            "status_detail": {
-                                "key": "x-ocsf-compliance.status_detail",
-                                "object": "compliance"
-                            }
-                        },
-                        "confidence": {
-                            "key": "x-oca-event.confidence",
-                            "object": "x-oca-event"
-                        },
-                        "connection_info": {
-                            "boundary": {
-                                "key": "network-traffic.extensions.x-network-ext.boundary",
-                                "object": "nt"
-                            },
-                            "boundary_id": {
-                                "key": "network-traffic.extensions.x-network-ext.boundary_id",
-                                "object": "nt"
-                            },
-                            "direction": {
-                                "key": "network-traffic.extensions.x-network-ext.direction",
-                                "object": "nt"
-                            },
-                            "direction_id": {
-                                "key": "network-traffic.extensions.x-network-ext.direction_id",
-                                "object": "nt"
-                            },
-                            "protocol_name": {
-                                "key": "network-traffic.extensions.x-network-ext.protocol_name",
-                                "object": "nt"
-                            },
-                            "protocol_num": {
-                                "group": true,
-                                "key": "network-traffic.protocols",
-                                "object": "nt",
-                                "transformer": "ProtocolNumToName"
-                            },
-                            "protocol_ver": {
-                                "group": true,
-                                "key": "network-traffic.protocols",
-                                "object": "nt",
-                                "transformer": "ToLowercaseArray"
-                            },
-                            "protocol_ver_id": {
-                                "key": "network-traffic.extensions.x-network-ext.protocol_ver_id",
-                                "object": "nt"
-                            },
-                            "tcp_flags": {
-                                "key": "network-traffic.extensions.tcp-ext.src_flags_hex",
-                                "object": "nt"
-                            }
-                        },
-                        "count": [
-                            {
-                                "cybox": false,
-                                "key": "number_observed",
-                                "transformer": "ToInteger"
-                            },
-                            {
-                                "key": "x-ibm-finding.event_count",
-                                "object": "ibm_finding",
-                                "transformer": "ToInteger"
-                            }
-                        ],
-                        "data": {
-                            "key": "x-oca-event.extensions.x-ocsf-data.data",
-                            "object": "x-oca-event"
-                        },
-                        "dst_endpoint": {
-                            "instance_uid": {
-                                "key": "x-oca-asset.extensions.x-dst-endpoint.instance_uid",
-                                "object": "asset"
-                            },
-                            "interface_uid": {
-                                "key": "x-oca-asset.extensions.x-dst-endpoint.interface_uid",
-                                "object": "asset"
-                            },
-                            "intermediate_ips": [
+                            "resource_instancedetails_networkinterfaces_0_ipv6addresses_0": [
+                                {
+                                    "key": "ipv6-addr.value",
+                                    "object": "nc_ipv6_ip"
+                                },
+                                {
+                                    "cybox": false,
+                                    "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
+                                    "key": "ipv6-addr.x_aws_interface_id",
+                                    "object": "nc_ipv6_ip"
+                                }
+                            ],
+                            "resource_instancedetails_networkinterfaces_0_privatednsname": [
+                                {
+                                    "key": "domain-name.value",
+                                    "object": "private_dns_name"
+                                }
+                            ],
+                            "resource_instancedetails_networkinterfaces_0_privateipaddress": [
                                 {
                                     "key": "ipv4-addr.value",
-                                    "object": "dst_ipv4",
-                                    "transformer": "FilterIPv4List",
-                                    "unwrap": true
+                                    "object": "nc_private_ip1"
                                 },
                                 {
-                                    "key": "ipv6-addr.value",
-                                    "object": "dst_ipv6",
-                                    "transformer": "FilterIPv6List",
-                                    "unwrap": true
+                                    "key": "network-traffic.src_ref",
+                                    "object": "nc_nt",
+                                    "references": "nc_private_ip1"
                                 },
                                 {
-                                    "key": "x-oca-asset.ip_refs",
-                                    "object": "asset",
+                                    "key": "domain-name.resolves_to_refs",
+                                    "object": "private_dns_name",
                                     "references": [
-                                        "dst_ipv4",
-                                        "dst_ipv6"
-                                    ],
-                                    "unwrap": true
+                                        "nc_private_ip1"
+                                    ]
+                                },
+                                {
+                                    "key": "x-ibm-finding.src_ip_ref",
+                                    "object": "ibm_finding",
+                                    "references": "nc_private_ip1"
+                                },
+                                {
+                                    "cybox": false,
+                                    "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
+                                    "key": "ipv4-addr.x_aws_interface_id",
+                                    "object": "nc_private_ip1"
+                                },
+                                {
+                                    "cybox": false,
+                                    "key": "ipv4-addr.x_aws_ip_type",
+                                    "object": "nc_private_ip1",
+                                    "value": "private"
+                                }
+                            ],
+                            "resource_instancedetails_networkinterfaces_0_publicdnsname": [
+                                {
+                                    "key": "domain-name.value",
+                                    "object": "nc_public_name"
                                 }
                             ],
-                            "ip": [
+                            "resource_instancedetails_networkinterfaces_0_publicip": [
                                 {
                                     "key": "ipv4-addr.value",
-                                    "object": "dst_ip",
-                                    "transformer": "CheckIPv4"
+                                    "object": "nc_public_ip"
                                 },
                                 {
-                                    "key": "ipv6-addr.value",
-                                    "object": "dst_ip",
-                                    "transformer": "CheckIPv6"
+                                    "key": "domain-name.resolves_to_refs",
+                                    "object": "nc_public_name",
+                                    "references": [
+                                        "nc_public_ip"
+                                    ]
                                 },
                                 {
-                                    "key": "network-traffic.dst_ref",
-                                    "object": "nt",
-                                    "references": "dst_ip"
+                                    "cybox": false,
+                                    "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
+                                    "key": "ipv4-addr.x_aws_interface_id",
+                                    "object": "nc_public_ip"
                                 },
                                 {
-                                    "key": "x-ibm-finding.dst_ip_ref",
-                                    "object": "ibm_finding",
-                                    "references": "dst_ip"
+                                    "cybox": false,
+                                    "key": "ipv4-addr.x_aws_ip_type",
+                                    "object": "nc_public_ip",
+                                    "value": "public"
+                                }
+                            ],
+                            "resource_instancedetails_networkinterfaces_0_securitygroups_0_groupid": {
+                                "key": "x-aws-vpc.security_group_id",
+                                "object": "vpc"
+                            },
+                            "resource_instancedetails_networkinterfaces_0_securitygroups_0_groupname": {
+                                "key": "x-aws-vpc.security_group_name",
+                                "object": "vpc"
+                            },
+                            "resource_instancedetails_networkinterfaces_0_subnetid": {
+                                "key": "x-aws-vpc.subnet_id",
+                                "object": "vpc"
+                            },
+                            "resource_instancedetails_networkinterfaces_0_vpcid": {
+                                "key": "x-aws-vpc.vpc_id",
+                                "object": "vpc"
+                            },
+                            "resource_instancedetails_networkinterfaces_1_privatednsname": [
+                                {
+                                    "key": "domain-name.value",
+                                    "object": "nc_private_name2"
+                                }
+                            ],
+                            "resource_instancedetails_networkinterfaces_1_privateipaddress": [
+                                {
+                                    "key": "ipv4-addr.value",
+                                    "object": "nc_private_ip2"
                                 },
                                 {
-                                    "group": true,
-                                    "key": "x-oca-asset.ip_refs",
-                                    "object": "host",
+                                    "key": "domain-name.resolves_to_refs",
+                                    "object": "nc_private_name2",
                                     "references": [
-                                        "dst_ip"
+                                        "nc_private_ip2"
                                     ]
                                 },
                                 {
-                                    "key": "x-oca-event.network_ref",
-                                    "object": "event",
-                                    "references": "nt"
+                                    "cybox": false,
+                                    "ds_key": "resource_instancedetails_networkinterfaces_1_networkinterfaceid",
+                                    "key": "ipv4-addr.x_aws_interface_id",
+                                    "object": "nc_private_ip2"
+                                },
+                                {
+                                    "cybox": false,
+                                    "key": "ipv4-addr.x_aws_ip_type",
+                                    "object": "nc_private_ip2",
+                                    "value": "private"
                                 }
                             ],
-                            "name": {
-                                "key": "x-oca-asset.name",
-                                "object": "asset"
-                            },
-                            "port": {
-                                "key": "network-traffic.dst_port",
-                                "object": "nt",
-                                "transformer": "ToInteger"
-                            },
-                            "subnet_uid": {
-                                "key": "x-oca-asset.extensions.x-dst-endpoint.subnet_uid",
-                                "object": "asset"
-                            },
-                            "svc_name": {
-                                "key": "x-oca-asset.extensions.x-dst-endpoint.svc_name",
-                                "object": "asset"
-                            },
-                            "vpc_uid": {
-                                "key": "x-oca-asset.extensions.x-dst-endpoint.vpc_uid",
-                                "object": "asset"
-                            }
-                        },
-                        "duration": {
-                            "key": "x-oca-event.duration",
-                            "object": "x_oca_event",
-                            "transformer": "ToInteger"
-                        },
-                        "end_time": [
-                            {
-                                "key": "x-ibm-finding.end",
-                                "object": "ibm_finding",
-                                "transformer": "EpochToTimestamp"
-                            },
-                            {
-                                "cybox": false,
-                                "key": "last_observed",
-                                "transformer": "EpochToTimestamp"
-                            }
-                        ],
-                        "enrichments": {
-                            "data": {
-                                "key": "x-ocsf-enrichments.data",
-                                "object": "enrichments"
-                            },
-                            "name": {
-                                "key": "x-ocsf-enrichments.name",
-                                "object": "enrichments"
-                            },
-                            "provider": {
-                                "key": "x-ocsf-enrichments.provider",
-                                "object": "enrichments"
-                            },
-                            "type": {
-                                "key": "x-ocsf-enrichments.type",
-                                "object": "enrichments"
-                            },
-                            "value": {
-                                "key": "x-ocsf-enrichments.value",
-                                "object": "enrichments"
-                            }
-                        },
-                        "finding": {
-                            "created_time": {
-                                "key": "x-ibm-finding.start",
-                                "object": "ibm_finding"
-                            },
-                            "desc": {
-                                "key": "x-ibm-finding.description",
-                                "object": "ibm_finding"
-                            },
-                            "first_seen_time": {
-                                "key": "x-ibm-finding.time_observed",
-                                "object": "ibm_finding"
-                            },
-                            "last_seen_time": {
-                                "key": "x-ibm-finding.extensions.x-ocsf-findings.last_seen_time",
-                                "object": "ibm_finding"
-                            },
-                            "modified_time": {
-                                "key": "x-ibm-finding.extensions.x-ocsf-findings.modified_time",
-                                "object": "ibm_finding"
-                            },
-                            "product_uid": {
-                                "key": "x-ibm-finding.extensions.x-ocsf-findings.product_uid",
-                                "object": "ibm_finding"
+                            "resource_instancedetails_platform": [
+                                {
+                                    "key": "software.name",
+                                    "object": "software"
+                                },
+                                {
+                                    "key": "x-ibm-finding.src_os_ref",
+                                    "object": "ibm_finding",
+                                    "references": "software"
+                                }
+                            ],
+                            "service_action_awsapicallaction_api": {
+                                "key": "x-aws-api.api",
+                                "object": "api_details"
                             },
-                            "related_events": {
-                                "product_uid": {
-                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.product_uid",
+                            "service_action_awsapicallaction_remoteipdetails_ipaddressv4": [
+                                {
+                                    "key": "ipv4-addr.value",
+                                    "object": "api_remote_ip"
+                                },
+                                {
+                                    "key": "x-ibm-finding.dst_ip_ref",
+                                    "object": "ibm_finding",
+                                    "references": "api_remote_ip"
+                                },
+                                {
+                                    "cybox": false,
+                                    "ds_key": "service_action_awsapicallaction_remoteipdetails_country_countryname",
+                                    "key": "x-ibm-finding.dst_geolocation",
                                     "object": "ibm_finding"
                                 },
-                                "type": {
-                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.type",
+                                {
+                                    "cybox": false,
+                                    "ds_key": "service_action_awsapicallaction_remoteipdetails_city_cityname",
+                                    "key": "ipv4-addr.x_aws_remote_city_name",
+                                    "object": "api_remote_ip"
+                                },
+                                {
+                                    "cybox": false,
+                                    "ds_key": "service_action_awsapicallaction_remoteipdetails_country_countryname",
+                                    "key": "ipv4-addr.x_aws_remote_country_name",
+                                    "object": "api_remote_ip"
+                                }
+                            ],
+                            "service_action_awsapicallaction_servicename": {
+                                "key": "x-aws-api.service_name",
+                                "object": "api_details"
+                            },
+                            "service_action_dnsrequestaction_domain": [
+                                {
+                                    "key": "domain-name.value",
+                                    "object": "dns_domain_name"
+                                }
+                            ],
+                            "service_action_networkconnectionaction_localportdetails_port": [
+                                {
+                                    "key": "network-traffic.src_port",
+                                    "object": "nc_nt",
+                                    "transformer": "ToInteger"
+                                }
+                            ],
+                            "service_action_networkconnectionaction_protocol": [
+                                {
+                                    "key": "network-traffic.protocols",
+                                    "object": "nc_nt",
+                                    "transformer": "ToLowercaseArray"
+                                }
+                            ],
+                            "service_action_networkconnectionaction_remoteipdetails_ipaddressv4": [
+                                {
+                                    "key": "ipv4-addr.value",
+                                    "object": "nc_remote_ip"
+                                },
+                                {
+                                    "key": "network-traffic.dst_ref",
+                                    "object": "nc_nt",
+                                    "references": "nc_remote_ip"
+                                },
+                                {
+                                    "key": "x-ibm-finding.dst_ip_ref",
+                                    "object": "ibm_finding",
+                                    "references": "nc_remote_ip"
+                                },
+                                {
+                                    "cybox": false,
+                                    "ds_key": "service_action_networkconnectionaction_remoteipdetails_country_countryname",
+                                    "key": "x-ibm-finding.dst_geolocation",
                                     "object": "ibm_finding"
                                 },
-                                "type_uid": {
-                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.type_uid",
+                                {
+                                    "cybox": false,
+                                    "ds_key": "service_action_networkconnectionaction_remoteipdetails_city_cityname",
+                                    "key": "ipv4-addr.x_aws_remote_city_name",
+                                    "object": "nc_remote_ip"
+                                },
+                                {
+                                    "cybox": false,
+                                    "ds_key": "service_action_networkconnectionaction_remoteipdetails_country_countryname",
+                                    "key": "ipv4-addr.x_aws_remote_country_name",
+                                    "object": "nc_remote_ip"
+                                }
+                            ],
+                            "service_action_networkconnectionaction_remoteportdetails_port": [
+                                {
+                                    "key": "network-traffic.dst_port",
+                                    "object": "nc_nt",
+                                    "transformer": "ToInteger"
+                                }
+                            ],
+                            "service_action_portprobeaction_portprobedetails_0_localportdetails_port": [
+                                {
+                                    "key": "x-ibm-finding.probe_port",
                                     "object": "ibm_finding"
+                                }
+                            ],
+                            "service_action_portprobeaction_portprobedetails_0_remoteipdetails_ipaddressv4": [
+                                {
+                                    "key": "ipv4-addr.value",
+                                    "object": "pp_remote_ip"
                                 },
-                                "uid": {
-                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.uid",
+                                {
+                                    "key": "x-ibm-finding.dst_ip_ref",
+                                    "object": "ibm_finding",
+                                    "references": "pp_remote_ip"
+                                },
+                                {
+                                    "cybox": false,
+                                    "ds_key": "service_action_portprobeaction_portprobedetails_0_remoteipdetails_country_countryname",
+                                    "key": "x-ibm-finding.dst_geolocation",
                                     "object": "ibm_finding"
+                                },
+                                {
+                                    "cybox": false,
+                                    "ds_key": "service_action_portprobeaction_portprobedetails_0_remoteipdetails_city_cityname",
+                                    "key": "ipv4-addr.x_aws_remote_city_name",
+                                    "object": "pp_remote_ip"
+                                },
+                                {
+                                    "cybox": false,
+                                    "ds_key": "service_action_portprobeaction_portprobedetails_0_remoteipdetails_country_countryname",
+                                    "key": "ipv4-addr.x_aws_remote_country_name",
+                                    "object": "pp_remote_ip"
                                 }
-                            },
-                            "remediation": {
-                                "desc": {
-                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.remediation_desc",
+                            ],
+                            "service_eventfirstseen": [
+                                {
+                                    "cybox": false,
+                                    "key": "first_observed"
+                                },
+                                {
+                                    "key": "x-ibm-finding.start",
                                     "object": "ibm_finding"
+                                }
+                            ],
+                            "service_eventlastseen": [
+                                {
+                                    "cybox": false,
+                                    "key": "last_observed"
                                 },
-                                "kb_articles": {
-                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.remediation_kb_articles",
+                                {
+                                    "key": "x-ibm-finding.end",
                                     "object": "ibm_finding"
                                 }
-                            },
-                            "src_url": {
-                                "key": "x-ibm-finding.extensions.x-ocsf-findings.src_url",
-                                "object": "ibm_finding"
-                            },
-                            "supporting_data": {
-                                "key": "x-ibm-finding.extensions.x-ocsf-findings.upporting_data",
+                            ],
+                            "severity": {
+                                "key": "x-ibm-finding.severity",
                                 "object": "ibm_finding"
                             },
                             "title": {
                                 "key": "x-ibm-finding.name",
                                 "object": "ibm_finding"
                             },
-                            "types": {
-                                "key": "x-ibm-finding.types",
-                                "object": "ibm_finding"
-                            },
-                            "uid": {
-                                "key": "x-ibm-finding.alert_id",
+                            "type": {
+                                "key": "x-ibm-finding.finding_type",
                                 "object": "ibm_finding"
                             }
                         },
-                        "http_request": {
-                            "args": {
-                                "key": "x-ocsf-http-request.value",
-                                "object": "http_request"
-                            },
-                            "http_headers": {
-                                "name": {
-                                    "key": "x-ocsf-http-request.http_headers_name",
-                                    "object": "ocsf_cloud_api"
+                        "ocsf": {
+                            "_time": [
+                                {
+                                    "cybox": false,
+                                    "key": "first_observed",
+                                    "transformer": "EpochToTimestamp"
                                 },
-                                "value": {
-                                    "key": "x-ocsf-http-request.http_headers_value",
-                                    "object": "http_request"
+                                {
+                                    "cybox": false,
+                                    "key": "last_observed",
+                                    "transformer": "EpochToTimestamp"
+                                },
+                                {
+                                    "key": "x-ibm-finding.time_observed",
+                                    "object": "ibm_finding",
+                                    "transformer": "EpochToTimestamp"
                                 }
+                            ],
+                            "activity": {
+                                "key": "x-oca-event.action",
+                                "object": "x_oca_event"
+                            },
+                            "activity_id": {
+                                "key": "x-oca-event.code",
+                                "object": "x_oca_event",
+                                "transformer": "ToInteger"
                             },
-                            "http_method": {
-                                "key": "x-ocsf-http-request.http_method",
-                                "object": "http_request"
-                            },
-                            "prefix": {
-                                "key": "x-ocsf-http-request.prefix",
-                                "object": "http_request"
-                            },
-                            "referrer": {
-                                "key": "x-ocsf-http-request.referrer",
-                                "object": "http_request"
-                            },
-                            "uid": {
-                                "key": "x-ocsf-http-request.uid",
-                                "object": "http_request"
-                            },
-                            "url": {
-                                "key": "url.value",
-                                "object": "url"
-                            },
-                            "user_agent": {
-                                "key": "x-ocsf-http-request.user_agent",
-                                "object": "http_request"
-                            },
-                            "version": {
-                                "key": "x-ocsf-http-request.version",
-                                "object": "http_request"
-                            },
-                            "x_forwarded_for": {
-                                "key": "x-ocsf-http-request.x_forwarded_for",
-                                "object": "http_request"
-                            }
-                        },
-                        "identity": {
-                            "authorizations": {
-                                "decision": {
-                                    "key": "x-ocsf-identity.authorizations.decision",
-                                    "object": "x-ocsf-identity"
+                            "activity_name": {
+                                "key": "x-oca-event.action",
+                                "object": "x_oca_event"
+                            },
+                            "api": {
+                                "operation": {
+                                    "key": "x-ocsf-cloud.operation",
+                                    "object": "ocsf_cloud_api"
                                 },
-                                "policy": {
-                                    "desc": {
-                                        "key": "x-ocsf-identity.authorizations.policy_desc",
-                                        "object": "x-ocsf-identity"
+                                "request": {
+                                    "flags": {
+                                        "key": "x-ocsf-cloud.request_flags",
+                                        "object": "ocsf_cloud_api",
+                                        "transformer": "ToLowercaseArray"
                                     },
-                                    "group": {
-                                        "desc": {
-                                            "key": "x-ocsf-identity.authorizations.policy_group_desc",
-                                            "object": "x-ocsf-identity"
-                                        },
-                                        "name": {
-                                            "key": "x-ocsf-identity.authorizations.policy_group_namee",
-                                            "object": "x-ocsf-identity"
-                                        },
-                                        "privileges": {
-                                            "key": "x-ocsf-identity.authorizations.policy_group_privileges",
-                                            "object": "x-ocsf-identity"
-                                        },
-                                        "type": {
-                                            "key": "x-ocsf-identity.authorizations.policy_group_type",
-                                            "object": "x-ocsf-identity"
-                                        },
-                                        "uid": {
-                                            "key": "x-ocsf-identity.authorizations.policy_group_uid",
-                                            "object": "x-ocsf-identity"
-                                        }
+                                    "uid": {
+                                        "key": "x-ocsf-cloud.request_uid",
+                                        "object": "ocsf_cloud_api"
+                                    }
+                                },
+                                "response": {
+                                    "code": {
+                                        "key": "x-ocsf-cloud.response_code",
+                                        "object": "ocsf_cloud_api",
+                                        "transformer": "ToInteger"
+                                    },
+                                    "error": {
+                                        "key": "x-ocsf-cloud.response_error",
+                                        "object": "ocsf_cloud_api"
+                                    },
+                                    "error_message": {
+                                        "key": "x-ocsf-cloud.response_error_message",
+                                        "object": "ocsf_cloud_api"
+                                    },
+                                    "flags": {
+                                        "key": "x-ocsf-cloud.response_flags",
+                                        "object": "ocsf_cloud_api",
+                                        "transformer": "ToLowercaseArray"
+                                    },
+                                    "message": {
+                                        "key": "x-ocsf-cloud.response_message",
+                                        "object": "ocsf_cloud_api"
+                                    }
+                                },
+                                "service": {
+                                    "labels": {
+                                        "key": "x-ocsf-cloud.service_labels",
+                                        "object": "ocsf_cloud_api",
+                                        "transformer": "ToLowercaseArray"
                                     },
                                     "name": {
-                                        "key": "x-ocsf-identity.authorizations.name",
-                                        "object": "x-ocsf-identity"
+                                        "key": "x-ocsf-cloud.service_name",
+                                        "object": "ocsf_cloud_api"
                                     },
                                     "uid": {
-                                        "key": "x-ocsf-identity.authorizations.uid",
-                                        "object": "x-ocsf-identity"
+                                        "key": "x-ocsf-cloud.service_uid",
+                                        "object": "ocsf_cloud_api"
                                     },
                                     "version": {
-                                        "key": "x-ocsf-identity.authorizations.version",
-                                        "object": "x-ocsf-identity"
+                                        "key": "x-ocsf-cloud.service_uid",
+                                        "object": "ocsf_cloud_api"
                                     }
+                                },
+                                "version": {
+                                    "key": "x-ocsf-cloud.api_version",
+                                    "object": "ocsf_cloud_api"
                                 }
                             },
-                            "idp": {
-                                "name": {
-                                    "key": "x-ocsf-identity.idp.name",
-                                    "object": "x-ocsf-identity"
+                            "attacks": {
+                                "tactics": {
+                                    "name": {
+                                        "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.tactic_name",
+                                        "object": "ttp-tagging"
+                                    },
+                                    "uid": {
+                                        "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.tactic_id",
+                                        "object": "ttp-tagging"
+                                    }
                                 },
-                                "uid": {
-                                    "key": "x-ocsf-identity.idp.uid",
-                                    "object": "x-ocsf-identity"
+                                "technique": {
+                                    "name": [
+                                        {
+                                            "key": "x-ibm-ttp-tagging.name",
+                                            "object": "ttp-tagging"
+                                        },
+                                        {
+                                            "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.technique_name",
+                                            "object": "ttp-tagging"
+                                        },
+                                        {
+                                            "key": "x-ibm-finding.ttp_tagging_refs",
+                                            "object": "ibm_finding",
+                                            "references": [
+                                                "ttp-tagging"
+                                            ]
+                                        }
+                                    ],
+                                    "uid": {
+                                        "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.technique_id",
+                                        "object": "ttp-tagging"
+                                    }
+                                },
+                                "version": {
+                                    "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.versoin",
+                                    "object": "ttp-tagging"
                                 }
                             },
-                            "invoked_by": {
-                                "key": "x-ocsf-identity.invoked_by",
-                                "object": "x-ocsf-identity"
+                            "category_name": {
+                                "key": "x-oca-event.category",
+                                "object": "x_oca_event"
+                            },
+                            "category_uid": {
+                                "key": "x-oca-event.code",
+                                "object": "x_oca_event",
+                                "transformer": "ToInteger"
                             },
-                            "message": {
-                                "key": "x-ocsf-identity.message",
-                                "object": "x-ocsf-identity"
+                            "class_name": {
+                                "key": "x-oca-event.module",
+                                "object": "x_oca_event"
+                            },
+                            "class_uid": {
+                                "key": "x-oca-event.extensions.x-cloud-api.class_uid",
+                                "object": "x_oca_event",
+                                "transformer": "ToInteger"
                             },
-                            "session": {
-                                "created_time": {
-                                    "key": "x-ocsf-identity.session.created_time",
-                                    "object": "x-ocsf-identity"
+                            "cloud": {
+                                "account_type": {
+                                    "key": "x-ocsf-cloud.account_type",
+                                    "object": "ocsf_cloud_api"
                                 },
-                                "credential_uid": {
-                                    "key": "x-ocsf-identity.session.credential_uid",
-                                    "object": "x-ocsf-identity"
+                                "account_type_id": {
+                                    "key": "x-ocsf-cloud.account_type_id",
+                                    "object": "ocsf_cloud_api",
+                                    "transformer": "ToInteger"
                                 },
-                                "expiration_time": {
-                                    "key": "x-ocsf-identity.session.expiration_time",
-                                    "object": "x-ocsf-identity"
+                                "account_uid": {
+                                    "key": "x-ocsf-cloud.account_uid",
+                                    "object": "ocsf_cloud_api"
                                 },
-                                "issuer": {
-                                    "key": "x-ocsf-identity.session.issuer",
-                                    "object": "x-ocsf-identity"
+                                "org_uid": {
+                                    "key": "x-ocsf-cloud.org_uid",
+                                    "object": "ocsf_cloud_api"
                                 },
-                                "mfa": {
-                                    "key": "x-ocsf-identity.session.mfa",
-                                    "object": "x-ocsf-identity"
+                                "project_uid": {
+                                    "key": "x-ocsf-cloud.project_uid",
+                                    "object": "ocsf_cloud_api"
                                 },
-                                "uid": {
-                                    "key": "x-ocsf-identity.session.uid",
-                                    "object": "x-ocsf-identity"
+                                "provider": {
+                                    "key": "x-ocsf-cloud.provider",
+                                    "object": "ocsf_cloud_api"
+                                },
+                                "region": {
+                                    "key": "x-ocsf-cloud.region",
+                                    "object": "ocsf_cloud_api"
+                                },
+                                "resource_uid": {
+                                    "key": "x-ocsf-cloud.resource_uid",
+                                    "object": "ocsf_cloud_api"
+                                },
+                                "zone": {
+                                    "key": "x-ocsf-cloud.zone",
+                                    "object": "ocsf_cloud_api"
                                 }
                             },
-                            "user": {
-                                "account_type": {
-                                    "key": "user-account.account_type",
-                                    "object": "user"
+                            "compliance": {
+                                "requirements": {
+                                    "key": "x-ocsf-compliance.requirements",
+                                    "object": "compliance"
+                                },
+                                "status": {
+                                    "key": "x-ocsf-compliance.status",
+                                    "object": "compliance"
+                                },
+                                "status_detail": {
+                                    "key": "x-ocsf-compliance.status_detail",
+                                    "object": "compliance"
+                                }
+                            },
+                            "confidence": {
+                                "key": "x-oca-event.confidence",
+                                "object": "x-oca-event"
+                            },
+                            "connection_info": {
+                                "boundary": {
+                                    "key": "network-traffic.extensions.x-network-ext.boundary",
+                                    "object": "nt"
+                                },
+                                "boundary_id": {
+                                    "key": "network-traffic.extensions.x-network-ext.boundary_id",
+                                    "object": "nt"
+                                },
+                                "direction": {
+                                    "key": "network-traffic.extensions.x-network-ext.direction",
+                                    "object": "nt"
+                                },
+                                "direction_id": {
+                                    "key": "network-traffic.extensions.x-network-ext.direction_id",
+                                    "object": "nt"
+                                },
+                                "protocol_name": {
+                                    "key": "network-traffic.extensions.x-network-ext.protocol_name",
+                                    "object": "nt"
                                 },
-                                "account_type_id": {
-                                    "key": "user-account.extensions.aws-account-ext.account_type_id",
-                                    "object": "user",
-                                    "transformer": "ToInteger"
+                                "protocol_num": {
+                                    "group": true,
+                                    "key": "network-traffic.protocols",
+                                    "object": "nt",
+                                    "transformer": "ProtocolNumToName"
                                 },
-                                "account_uid": {
-                                    "key": "user-account.user_id",
-                                    "object": "user"
+                                "protocol_ver": {
+                                    "group": true,
+                                    "key": "network-traffic.protocols",
+                                    "object": "nt",
+                                    "transformer": "ToLowercaseArray"
                                 },
-                                "credential_uid": {
-                                    "key": "user-account.extensions.aws-account-ext.credential_uid",
-                                    "object": "user"
-                                },
-                                "domain": {
-                                    "key": "user-account.extensions.aws-account-ext.domain",
-                                    "object": "user"
-                                },
-                                "email_addr": {
-                                    "key": "email-addr.value",
-                                    "object": "email_addr"
+                                "protocol_ver_id": {
+                                    "key": "network-traffic.extensions.x-network-ext.protocol_ver_id",
+                                    "object": "nt"
+                                },
+                                "tcp_flags": {
+                                    "key": "network-traffic.extensions.tcp-ext.src_flags_hex",
+                                    "object": "nt"
+                                }
+                            },
+                            "count": [
+                                {
+                                    "cybox": false,
+                                    "key": "number_observed",
+                                    "transformer": "ToInteger"
                                 },
-                                "groups": {
-                                    "desc": {
-                                        "key": "user-account.extensions.aws-account-ext.group_desc",
-                                        "object": "user"
+                                {
+                                    "key": "x-ibm-finding.event_count",
+                                    "object": "ibm_finding",
+                                    "transformer": "ToInteger"
+                                }
+                            ],
+                            "data": {
+                                "key": "x-oca-event.extensions.x-ocsf-data.data",
+                                "object": "x-oca-event"
+                            },
+                            "dst_endpoint": {
+                                "instance_uid": {
+                                    "key": "x-oca-asset.extensions.x-dst-endpoint.instance_uid",
+                                    "object": "asset"
+                                },
+                                "interface_uid": {
+                                    "key": "x-oca-asset.extensions.x-dst-endpoint.interface_uid",
+                                    "object": "asset"
+                                },
+                                "intermediate_ips": [
+                                    {
+                                        "key": "ipv4-addr.value",
+                                        "object": "dst_ipv4",
+                                        "transformer": "FilterIPv4List",
+                                        "unwrap": true
                                     },
-                                    "name": {
-                                        "key": "user-account.extensions.aws-account-ext.group_name",
-                                        "object": "user"
+                                    {
+                                        "key": "ipv6-addr.value",
+                                        "object": "dst_ipv6",
+                                        "transformer": "FilterIPv6List",
+                                        "unwrap": true
                                     },
-                                    "privileges": {
-                                        "key": "user-account.extensions.aws-account-ext.group_privileges",
-                                        "object": "user"
+                                    {
+                                        "key": "x-oca-asset.ip_refs",
+                                        "object": "asset",
+                                        "references": [
+                                            "dst_ipv4",
+                                            "dst_ipv6"
+                                        ],
+                                        "unwrap": true
+                                    }
+                                ],
+                                "ip": [
+                                    {
+                                        "key": "ipv4-addr.value",
+                                        "object": "dst_ip",
+                                        "transformer": "CheckIPv4"
                                     },
-                                    "type": {
-                                        "key": "user-account.extensions.aws-account-ext.group_type",
-                                        "object": "user"
+                                    {
+                                        "key": "ipv6-addr.value",
+                                        "object": "dst_ip",
+                                        "transformer": "CheckIPv6"
                                     },
-                                    "uid": {
-                                        "key": "user-account.extensions.aws-account-ext.group_uid",
-                                        "object": "user"
+                                    {
+                                        "key": "network-traffic.dst_ref",
+                                        "object": "nt",
+                                        "references": "dst_ip"
+                                    },
+                                    {
+                                        "key": "x-ibm-finding.dst_ip_ref",
+                                        "object": "ibm_finding",
+                                        "references": "dst_ip"
+                                    },
+                                    {
+                                        "group": true,
+                                        "key": "x-oca-asset.ip_refs",
+                                        "object": "host",
+                                        "references": [
+                                            "dst_ip"
+                                        ]
+                                    },
+                                    {
+                                        "key": "x-oca-event.network_ref",
+                                        "object": "event",
+                                        "references": "nt"
                                     }
-                                },
+                                ],
                                 "name": {
-                                    "key": "user-account.display_name",
-                                    "object": "user"
+                                    "key": "x-oca-asset.name",
+                                    "object": "asset"
                                 },
-                                "org_uid": {
-                                    "key": "user-account.extensions.aws-account-ext.org_uid",
-                                    "object": "user"
+                                "port": {
+                                    "key": "network-traffic.dst_port",
+                                    "object": "nt",
+                                    "transformer": "ToInteger"
                                 },
-                                "session_uid": {
-                                    "key": "user-account.extensions.aws-account-ext.session_uid",
-                                    "object": "user"
-                                },
-                                "session_uuid": {
-                                    "key": "user-account.extensions.aws-account-ext.session_uuid",
-                                    "object": "user"
+                                "subnet_uid": {
+                                    "key": "x-oca-asset.extensions.x-dst-endpoint.subnet_uid",
+                                    "object": "asset"
+                                },
+                                "svc_name": {
+                                    "key": "x-oca-asset.extensions.x-dst-endpoint.svc_name",
+                                    "object": "asset"
+                                },
+                                "vpc_uid": {
+                                    "key": "x-oca-asset.extensions.x-dst-endpoint.vpc_uid",
+                                    "object": "asset"
+                                }
+                            },
+                            "duration": {
+                                "key": "x-oca-event.duration",
+                                "object": "x_oca_event",
+                                "transformer": "ToInteger"
+                            },
+                            "end_time": [
+                                {
+                                    "key": "x-ibm-finding.end",
+                                    "object": "ibm_finding",
+                                    "transformer": "EpochToTimestamp"
                                 },
-                                "type": {
-                                    "key": "user-account.extensions.aws-account-ext.type",
-                                    "object": "user"
+                                {
+                                    "cybox": false,
+                                    "key": "last_observed",
+                                    "transformer": "EpochToTimestamp"
+                                }
+                            ],
+                            "enrichments": {
+                                "data": {
+                                    "key": "x-ocsf-enrichments.data",
+                                    "object": "enrichments"
                                 },
-                                "type_id": {
-                                    "key": "user-account.extensions.aws-account-ext.type_id",
-                                    "object": "user",
-                                    "transformer": "ToInteger"
+                                "name": {
+                                    "key": "x-ocsf-enrichments.name",
+                                    "object": "enrichments"
                                 },
-                                "uid": {
-                                    "key": "user-account.extensions.aws-account-ext.uid",
-                                    "object": "user"
+                                "provider": {
+                                    "key": "x-ocsf-enrichments.provider",
+                                    "object": "enrichments"
                                 },
-                                "uuid": {
-                                    "key": "user-account.extensions.aws-account-ext.uuid",
-                                    "object": "user"
+                                "type": {
+                                    "key": "x-ocsf-enrichments.type",
+                                    "object": "enrichments"
+                                },
+                                "value": {
+                                    "key": "x-ocsf-enrichments.value",
+                                    "object": "enrichments"
                                 }
-                            }
-                        },
-                        "malware": {
-                            "classification_ids": {
-                                "key": "x-ocsf-malware.classification_ids",
-                                "object": "malware"
-                            },
-                            "classifications": {
-                                "key": "x-ocsf-malware.classifications",
-                                "object": "malware"
                             },
-                            "cves": {
+                            "finding": {
                                 "created_time": {
-                                    "key": "x-ocsf-malware.created_time",
-                                    "object": "malware"
+                                    "key": "x-ibm-finding.start",
+                                    "object": "ibm_finding"
                                 },
-                                "cvss": {
-                                    "base_score": {
-                                        "key": "x-ocsf-malware.base_score",
-                                        "object": "malware"
-                                    },
-                                    "depth": {
-                                        "key": "x-ocsf-malware.depth",
-                                        "object": "malware"
-                                    },
-                                    "metrics": {
-                                        "name": {
-                                            "key": "x-ocsf-malware.name",
-                                            "object": "malware"
-                                        },
-                                        "value": {
-                                            "key": "x-ocsf-malware.value",
-                                            "object": "malware"
-                                        }
-                                    },
-                                    "overall_score": {
-                                        "key": "x-ocsf-malware.overall_score",
-                                        "object": "malware"
-                                    },
-                                    "severity": {
-                                        "key": "x-ocsf-malware.severity",
-                                        "object": "malware"
-                                    },
-                                    "vector_string": {
-                                        "key": "x-ocsf-malware.vector_string",
-                                        "object": "malware"
-                                    },
-                                    "version": {
-                                        "key": "x-ocsf-malware.version",
-                                        "object": "malware"
-                                    }
+                                "desc": {
+                                    "key": "x-ibm-finding.description",
+                                    "object": "ibm_finding"
                                 },
-                                "cwe_uid": {
-                                    "key": "x-ocsf-malware.cwe_uid",
-                                    "object": "malware"
+                                "first_seen_time": {
+                                    "key": "x-ibm-finding.time_observed",
+                                    "object": "ibm_finding"
                                 },
-                                "cwe_url": {
-                                    "key": "x-ocsf-malware.cwe_url",
-                                    "object": "malware"
+                                "last_seen_time": {
+                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.last_seen_time",
+                                    "object": "ibm_finding"
                                 },
                                 "modified_time": {
-                                    "key": "x-ocsf-malware.modified_time",
-                                    "object": "malware"
+                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.modified_time",
+                                    "object": "ibm_finding"
                                 },
-                                "product": {
-                                    "feature": {
-                                        "name": {
-                                            "key": "software.extensions.x-ocsf-product-ext.feature_name",
-                                            "object": "malware-software"
-                                        },
-                                        "uid": {
-                                            "key": "software.extensions.x-ocsf-product-ext.feature_uid",
-                                            "object": "malware-software"
-                                        },
-                                        "version": {
-                                            "key": "software.extensions.x-ocsf-product-ext.feature_version",
-                                            "object": "malware-software"
-                                        }
-                                    },
-                                    "lang": {
-                                        "key": "software.languages",
-                                        "object": "malware-software"
+                                "product_uid": {
+                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.product_uid",
+                                    "object": "ibm_finding"
+                                },
+                                "related_events": {
+                                    "product_uid": {
+                                        "key": "x-ibm-finding.extensions.x-ocsf-findings.product_uid",
+                                        "object": "ibm_finding"
                                     },
-                                    "name": {
-                                        "key": "software.name",
-                                        "object": "malware-software"
+                                    "type": {
+                                        "key": "x-ibm-finding.extensions.x-ocsf-findings.type",
+                                        "object": "ibm_finding"
                                     },
-                                    "path": {
-                                        "key": "software.extensions.x-ocsf-product-ext.installed_path",
-                                        "object": "malware-software"
+                                    "type_uid": {
+                                        "key": "x-ibm-finding.extensions.x-ocsf-findings.type_uid",
+                                        "object": "ibm_finding"
                                     },
                                     "uid": {
-                                        "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                                        "object": "malware-software"
-                                    },
-                                    "vendor_name": {
-                                        "key": "software.vendor",
-                                        "object": "malware-software"
+                                        "key": "x-ibm-finding.extensions.x-ocsf-findings.uid",
+                                        "object": "ibm_finding"
+                                    }
+                                },
+                                "remediation": {
+                                    "desc": {
+                                        "key": "x-ibm-finding.extensions.x-ocsf-findings.remediation_desc",
+                                        "object": "ibm_finding"
                                     },
-                                    "version": {
-                                        "key": "software.version",
-                                        "object": "malware-software"
+                                    "kb_articles": {
+                                        "key": "x-ibm-finding.extensions.x-ocsf-findings.remediation_kb_articles",
+                                        "object": "ibm_finding"
                                     }
                                 },
-                                "type": {
-                                    "key": "x-ocsf-malware.type",
-                                    "object": "malware"
+                                "src_url": {
+                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.src_url",
+                                    "object": "ibm_finding"
+                                },
+                                "supporting_data": {
+                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.upporting_data",
+                                    "object": "ibm_finding"
+                                },
+                                "title": {
+                                    "key": "x-ibm-finding.name",
+                                    "object": "ibm_finding"
+                                },
+                                "types": {
+                                    "key": "x-ibm-finding.types",
+                                    "object": "ibm_finding"
                                 },
                                 "uid": {
-                                    "key": "x-ocsf-malware.uid",
-                                    "object": "malware"
+                                    "key": "x-ibm-finding.alert_id",
+                                    "object": "ibm_finding"
                                 }
                             },
-                            "name": {
-                                "key": "x-ocsf-malware.name",
-                                "object": "malware"
-                            },
-                            "path": {
-                                "key": "x-ocsf-malware.path",
-                                "object": "malware"
-                            },
-                            "provider": {
-                                "key": "x-ocsf-malware.provider",
-                                "object": "malware"
-                            },
-                            "uid": {
-                                "key": "x-ocsf-malware.uid",
-                                "object": "malware"
-                            }
-                        },
-                        "message": {
-                            "key": "x-ocsf-cloud.message",
-                            "object": "ocsf_cloud_api"
-                        },
-                        "metadata": {
-                            "correlation_uid": {
-                                "key": "x-ocsf-metadata.correlation_uid",
-                                "object": "metadata"
-                            },
-                            "labels": {
-                                "key": "x-ocsf-metadata.labels",
-                                "object": "metadata"
-                            },
-                            "logged_time": {
-                                "key": "x-ocsf-metadata.logged_time",
-                                "object": "metadata"
-                            },
-                            "modified_time": {
-                                "key": "x-ocsf-metadata.modified_time",
-                                "object": "metadata"
-                            },
-                            "processed_time": {
-                                "key": "x-ocsf-metadata.processed_time",
-                                "object": "metadata"
-                            },
-                            "product": {
-                                "feature": {
+                            "http_request": {
+                                "args": {
+                                    "key": "x-ocsf-http-request.value",
+                                    "object": "http_request"
+                                },
+                                "http_headers": {
                                     "name": {
-                                        "key": "software.extensions.x-ocsf-product-ext.feature_name",
-                                        "object": "metadata-software"
-                                    },
-                                    "uid": {
-                                        "key": "software.extensions.x-ocsf-product-ext.feature_uid",
-                                        "object": "metadata-software"
+                                        "key": "x-ocsf-http-request.http_headers_name",
+                                        "object": "ocsf_cloud_api"
                                     },
-                                    "version": {
-                                        "key": "software.extensions.x-ocsf-product-ext.feature_version",
-                                        "object": "metadata-software"
+                                    "value": {
+                                        "key": "x-ocsf-http-request.http_headers_value",
+                                        "object": "http_request"
                                     }
                                 },
-                                "lang": {
-                                    "key": "software.languages",
-                                    "object": "metadata-software"
+                                "http_method": {
+                                    "key": "x-ocsf-http-request.http_method",
+                                    "object": "http_request"
                                 },
-                                "name": {
-                                    "key": "software.name",
-                                    "object": "metadata-software"
+                                "prefix": {
+                                    "key": "x-ocsf-http-request.prefix",
+                                    "object": "http_request"
                                 },
-                                "path": {
-                                    "key": "software.extensions.x-ocsf-product-ext.installed_path",
-                                    "object": "metadata-software"
+                                "referrer": {
+                                    "key": "x-ocsf-http-request.referrer",
+                                    "object": "http_request"
                                 },
                                 "uid": {
-                                    "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                                    "object": "metadata-software"
+                                    "key": "x-ocsf-http-request.uid",
+                                    "object": "http_request"
                                 },
-                                "vendor_name": {
-                                    "key": "software.vendor",
-                                    "object": "metadata-software"
+                                "url": {
+                                    "key": "url.value",
+                                    "object": "url"
+                                },
+                                "user_agent": {
+                                    "key": "x-ocsf-http-request.user_agent",
+                                    "object": "http_request"
                                 },
                                 "version": {
-                                    "key": "software.version",
-                                    "object": "metadata-software"
-                                }
-                            },
-                            "sequence": {
-                                "key": "x-ocsf-metadata.sequence",
-                                "object": "metadata",
-                                "transformer": "ToInteger"
-                            },
-                            "uid": {
-                                "key": "x-ocsf-metadata.uid",
-                                "object": "metadata"
-                            },
-                            "version": {
-                                "key": "x-ocsf-metadata.version",
-                                "object": "metadata"
-                            }
-                        },
-                        "observables": {
-                            "name": [
-                                {
-                                    "key": "x-ibm-observables.name",
-                                    "object": "observables"
+                                    "key": "x-ocsf-http-request.version",
+                                    "object": "http_request"
                                 },
-                                {
-                                    "key": "x-ibm-finding.ioc_refs",
-                                    "object": "ibm_finding",
-                                    "references": [
-                                        "observables"
-                                    ]
+                                "x_forwarded_for": {
+                                    "key": "x-ocsf-http-request.x_forwarded_for",
+                                    "object": "http_request"
                                 }
-                            ],
-                            "type": {
-                                "key": "x-ibm-observables.finding_type",
-                                "object": "observables"
-                            },
-                            "type_id": {
-                                "key": "x-ibm-observables.alert_id",
-                                "object": "observables",
-                                "transformer": "ToInteger"
                             },
-                            "value": {
-                                "key": "x-ibm-observables.description",
-                                "object": "observables"
-                            }
-                        },
-                        "process": {
-                            "cmd_line": {
-                                "key": "process.command_line",
-                                "object": "process"
-                            },
-                            "created_time": {
-                                "key": "process.created",
-                                "object": "process"
-                            },
-                            "file": {
-                                "accessed_time": {
-                                    "key": "file.accessed",
-                                    "object": "file"
-                                },
-                                "accessor": {
-                                    "account_type": {
-                                        "key": "user-account.account_type",
-                                        "object": "accessor-user-account"
-                                    },
-                                    "account_type_id": {
-                                        "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                        "object": "accessor-user-account"
-                                    },
-                                    "account_uid": {
-                                        "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                        "object": "accessor-user-account"
-                                    },
-                                    "credential_uid": {
-                                        "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                        "object": "accessor-user-account"
-                                    },
-                                    "domain": {
-                                        "key": "user-account.extensions.x-accessor-ext.domain",
-                                        "object": "accessor-user-account"
-                                    },
-                                    "email_addr": {
-                                        "key": "email-addr.value",
-                                        "object": "email-addr"
+                            "identity": {
+                                "authorizations": {
+                                    "decision": {
+                                        "key": "x-ocsf-identity.authorizations.decision",
+                                        "object": "x-ocsf-identity"
                                     },
-                                    "groups": {
+                                    "policy": {
                                         "desc": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                            "object": "accessor-user-account"
-                                        },
-                                        "name": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_name",
-                                            "object": "accessor-user-account"
+                                            "key": "x-ocsf-identity.authorizations.policy_desc",
+                                            "object": "x-ocsf-identity"
                                         },
-                                        "privileges": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                            "object": "accessor-user-account"
+                                        "group": {
+                                            "desc": {
+                                                "key": "x-ocsf-identity.authorizations.policy_group_desc",
+                                                "object": "x-ocsf-identity"
+                                            },
+                                            "name": {
+                                                "key": "x-ocsf-identity.authorizations.policy_group_namee",
+                                                "object": "x-ocsf-identity"
+                                            },
+                                            "privileges": {
+                                                "key": "x-ocsf-identity.authorizations.policy_group_privileges",
+                                                "object": "x-ocsf-identity"
+                                            },
+                                            "type": {
+                                                "key": "x-ocsf-identity.authorizations.policy_group_type",
+                                                "object": "x-ocsf-identity"
+                                            },
+                                            "uid": {
+                                                "key": "x-ocsf-identity.authorizations.policy_group_uid",
+                                                "object": "x-ocsf-identity"
+                                            }
                                         },
-                                        "type": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_type",
-                                            "object": "accessor-user-account"
+                                        "name": {
+                                            "key": "x-ocsf-identity.authorizations.name",
+                                            "object": "x-ocsf-identity"
                                         },
                                         "uid": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                            "object": "accessor-user-account"
+                                            "key": "x-ocsf-identity.authorizations.uid",
+                                            "object": "x-ocsf-identity"
+                                        },
+                                        "version": {
+                                            "key": "x-ocsf-identity.authorizations.version",
+                                            "object": "x-ocsf-identity"
                                         }
-                                    },
+                                    }
+                                },
+                                "idp": {
                                     "name": {
-                                        "key": "user-account.display_name",
-                                        "object": "accessor-user-account"
-                                    },
-                                    "org_uid": {
-                                        "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                        "object": "accessor-user-account"
-                                    },
-                                    "session_uid": {
-                                        "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                        "object": "accessor-user-account"
-                                    },
-                                    "session_uuid": {
-                                        "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                        "object": "accessor-user-account"
-                                    },
-                                    "type": {
-                                        "key": "user-account.extensions.x-accessor-ext.type",
-                                        "object": "accessor-user-account"
-                                    },
-                                    "type_id": {
-                                        "key": "user-account.extensions.x-accessor-ext.type_id",
-                                        "object": "accessor-user-account"
+                                        "key": "x-ocsf-identity.idp.name",
+                                        "object": "x-ocsf-identity"
                                     },
                                     "uid": {
-                                        "key": "user-account.user_id",
-                                        "object": "accessor-user-account"
-                                    },
-                                    "uuid": {
-                                        "key": "user-account.extensions.x-accessor-ext.uuid",
-                                        "object": "accessor-user-account"
+                                        "key": "x-ocsf-identity.idp.uid",
+                                        "object": "x-ocsf-identity"
                                     }
                                 },
-                                "attributes": {
-                                    "key": "file.extensions.x-ocsf-file-ext.attributes",
-                                    "object": "file"
-                                },
-                                "company_name": {
-                                    "key": "file.extensions.x-ocsf-file-ext.company_name",
-                                    "object": "file"
-                                },
-                                "confidentiality": {
-                                    "key": "file.extensions.x-ocsf-file-ext.confidentiality",
-                                    "object": "file"
-                                },
-                                "confidentiality_id": {
-                                    "key": "file.extensions.x-ocsf-file-ext.confidentiality_id",
-                                    "object": "file"
+                                "invoked_by": {
+                                    "key": "x-ocsf-identity.invoked_by",
+                                    "object": "x-ocsf-identity"
                                 },
-                                "created_time": {
-                                    "key": "file.created",
-                                    "object": "file"
+                                "message": {
+                                    "key": "x-ocsf-identity.message",
+                                    "object": "x-ocsf-identity"
                                 },
-                                "creator": {
-                                    "account_type": {
-                                        "key": "user-account.account_type",
-                                        "object": "creator-user-account"
-                                    },
-                                    "account_type_id": {
-                                        "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                        "object": "creator-user-account"
-                                    },
-                                    "account_uid": {
-                                        "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                        "object": "creator-user-account"
+                                "session": {
+                                    "created_time": {
+                                        "key": "x-ocsf-identity.session.created_time",
+                                        "object": "x-ocsf-identity"
                                     },
                                     "credential_uid": {
-                                        "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                        "object": "creator-user-account"
-                                    },
-                                    "domain": {
-                                        "key": "user-account.extensions.x-accessor-ext.domain",
-                                        "object": "creator-user-account"
-                                    },
-                                    "email_addr": {
-                                        "key": "email-addr.value",
-                                        "object": "creator-email-addr"
-                                    },
-                                    "groups": {
-                                        "desc": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                            "object": "creator-user-account"
-                                        },
-                                        "name": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_name",
-                                            "object": "creator-user-account"
-                                        },
-                                        "privileges": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                            "object": "creator-user-account"
-                                        },
-                                        "type": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_type",
-                                            "object": "creator-user-account"
-                                        },
-                                        "uid": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                            "object": "creator-user-account"
-                                        }
-                                    },
-                                    "name": {
-                                        "key": "user-account.display_name",
-                                        "object": "creator-user-account"
-                                    },
-                                    "org_uid": {
-                                        "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                        "object": "creator-user-account"
-                                    },
-                                    "session_uid": {
-                                        "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                        "object": "creator-user-account"
+                                        "key": "x-ocsf-identity.session.credential_uid",
+                                        "object": "x-ocsf-identity"
                                     },
-                                    "session_uuid": {
-                                        "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                        "object": "creator-user-account"
+                                    "expiration_time": {
+                                        "key": "x-ocsf-identity.session.expiration_time",
+                                        "object": "x-ocsf-identity"
                                     },
-                                    "type": {
-                                        "key": "user-account.extensions.x-accessor-ext.type",
-                                        "object": "creator-user-account"
+                                    "issuer": {
+                                        "key": "x-ocsf-identity.session.issuer",
+                                        "object": "x-ocsf-identity"
                                     },
-                                    "type_id": {
-                                        "key": "user-account.extensions.x-accessor-ext.type_id",
-                                        "object": "creator-user-account"
+                                    "mfa": {
+                                        "key": "x-ocsf-identity.session.mfa",
+                                        "object": "x-ocsf-identity"
                                     },
                                     "uid": {
-                                        "key": "user-account.user_id",
-                                        "object": "creator-user-account"
-                                    },
-                                    "uuid": {
-                                        "key": "user-account.extensions.x-accessor-ext.uuid",
-                                        "object": "creator-user-account"
-                                    }
-                                },
-                                "desc": {
-                                    "key": "file.extensions.x-ocsf-file-ext.description",
-                                    "object": "file"
-                                },
-                                "hashes": {
-                                    "CTPH": {
-                                        "key": "file.hashes.CTPH",
-                                        "object": "file"
-                                    },
-                                    "MD5": {
-                                        "key": "file.hashes.MD5",
-                                        "object": "file"
-                                    },
-                                    "Other": {
-                                        "key": "file.hashes.Other",
-                                        "object": "file"
-                                    },
-                                    "SHA-1": {
-                                        "key": "file.hashes.SHA-1",
-                                        "object": "file"
-                                    },
-                                    "SHA-256": {
-                                        "key": "file.hashes.SHA-256",
-                                        "object": "file"
-                                    },
-                                    "SHA-512": {
-                                        "key": "file.hashes.SHA-512",
-                                        "object": "file"
-                                    },
-                                    "Unknown": {
-                                        "key": "file.hashes.Unknown",
-                                        "object": "file"
+                                        "key": "x-ocsf-identity.session.uid",
+                                        "object": "x-ocsf-identity"
                                     }
                                 },
-                                "is_system": {
-                                    "key": "process.extensions.x-ocsf-process-ext.is_system",
-                                    "object": "process"
-                                },
-                                "mime_type": {
-                                    "key": "process.mime_type",
-                                    "object": "process"
-                                },
-                                "modified_time": {
-                                    "key": "process.extensions.x-ocsf-process-ext.modified_time",
-                                    "object": "process"
-                                },
-                                "modifier": {
+                                "user": {
                                     "account_type": {
                                         "key": "user-account.account_type",
-                                        "object": "modifier-user-account"
+                                        "object": "user"
                                     },
                                     "account_type_id": {
-                                        "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                        "object": "modifier-user-account"
+                                        "key": "user-account.extensions.aws-account-ext.account_type_id",
+                                        "object": "user",
+                                        "transformer": "ToInteger"
                                     },
                                     "account_uid": {
-                                        "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                        "object": "modifier-user-account"
+                                        "key": "user-account.user_id",
+                                        "object": "user"
                                     },
                                     "credential_uid": {
-                                        "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                        "object": "modifier-user-account"
+                                        "key": "user-account.extensions.aws-account-ext.credential_uid",
+                                        "object": "user"
                                     },
                                     "domain": {
-                                        "key": "user-account.extensions.x-accessor-ext.domain",
-                                        "object": "modifier-user-account"
+                                        "key": "user-account.extensions.aws-account-ext.domain",
+                                        "object": "user"
                                     },
                                     "email_addr": {
                                         "key": "email-addr.value",
-                                        "object": "modifier-email-addr"
+                                        "object": "email_addr"
                                     },
                                     "groups": {
                                         "desc": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                            "object": "modifier-user-account"
+                                            "key": "user-account.extensions.aws-account-ext.group_desc",
+                                            "object": "user"
                                         },
                                         "name": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_name",
-                                            "object": "modifier-user-account"
+                                            "key": "user-account.extensions.aws-account-ext.group_name",
+                                            "object": "user"
                                         },
                                         "privileges": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                            "object": "modifier-user-account"
+                                            "key": "user-account.extensions.aws-account-ext.group_privileges",
+                                            "object": "user"
                                         },
                                         "type": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_type",
-                                            "object": "modifier-user-account"
+                                            "key": "user-account.extensions.aws-account-ext.group_type",
+                                            "object": "user"
                                         },
                                         "uid": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                            "object": "modifier-user-account"
+                                            "key": "user-account.extensions.aws-account-ext.group_uid",
+                                            "object": "user"
                                         }
                                     },
                                     "name": {
                                         "key": "user-account.display_name",
-                                        "object": "modifier-user-account"
+                                        "object": "user"
                                     },
                                     "org_uid": {
-                                        "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                        "object": "modifier-user-account"
+                                        "key": "user-account.extensions.aws-account-ext.org_uid",
+                                        "object": "user"
                                     },
                                     "session_uid": {
-                                        "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                        "object": "modifier-user-account"
+                                        "key": "user-account.extensions.aws-account-ext.session_uid",
+                                        "object": "user"
                                     },
                                     "session_uuid": {
-                                        "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                        "object": "modifier-user-account"
+                                        "key": "user-account.extensions.aws-account-ext.session_uuid",
+                                        "object": "user"
                                     },
                                     "type": {
-                                        "key": "user-account.extensions.x-accessor-ext.type",
-                                        "object": "modifier-user-account"
+                                        "key": "user-account.extensions.aws-account-ext.type",
+                                        "object": "user"
                                     },
                                     "type_id": {
-                                        "key": "user-account.extensions.x-accessor-ext.type_id",
-                                        "object": "modifier-user-account"
+                                        "key": "user-account.extensions.aws-account-ext.type_id",
+                                        "object": "user",
+                                        "transformer": "ToInteger"
                                     },
                                     "uid": {
-                                        "key": "user-account.user_id",
-                                        "object": "modifier-user-account"
+                                        "key": "user-account.extensions.aws-account-ext.uid",
+                                        "object": "user"
                                     },
                                     "uuid": {
-                                        "key": "user-account.extensions.x-accessor-ext.uuid",
-                                        "object": "modifier-user-account"
+                                        "key": "user-account.extensions.aws-account-ext.uuid",
+                                        "object": "user"
                                     }
+                                }
+                            },
+                            "malware": {
+                                "classification_ids": {
+                                    "key": "x-ocsf-malware.classification_ids",
+                                    "object": "malware"
                                 },
-                                "name": [
-                                    {
-                                        "key": "file.name",
-                                        "object": "file"
-                                    },
-                                    {
-                                        "key": "process.binary_ref",
-                                        "object": "process",
-                                        "references": "file"
-                                    }
-                                ],
-                                "owner": {
-                                    "account_type": {
-                                        "key": "user-account.account_type",
-                                        "object": "owner-user-account"
-                                    },
-                                    "account_type_id": {
-                                        "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                        "object": "owner-user-account"
+                                "classifications": {
+                                    "key": "x-ocsf-malware.classifications",
+                                    "object": "malware"
+                                },
+                                "cves": {
+                                    "created_time": {
+                                        "key": "x-ocsf-malware.created_time",
+                                        "object": "malware"
                                     },
-                                    "account_uid": {
-                                        "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                        "object": "owner-user-account"
+                                    "cvss": {
+                                        "base_score": {
+                                            "key": "x-ocsf-malware.base_score",
+                                            "object": "malware"
+                                        },
+                                        "depth": {
+                                            "key": "x-ocsf-malware.depth",
+                                            "object": "malware"
+                                        },
+                                        "metrics": {
+                                            "name": {
+                                                "key": "x-ocsf-malware.name",
+                                                "object": "malware"
+                                            },
+                                            "value": {
+                                                "key": "x-ocsf-malware.value",
+                                                "object": "malware"
+                                            }
+                                        },
+                                        "overall_score": {
+                                            "key": "x-ocsf-malware.overall_score",
+                                            "object": "malware"
+                                        },
+                                        "severity": {
+                                            "key": "x-ocsf-malware.severity",
+                                            "object": "malware"
+                                        },
+                                        "vector_string": {
+                                            "key": "x-ocsf-malware.vector_string",
+                                            "object": "malware"
+                                        },
+                                        "version": {
+                                            "key": "x-ocsf-malware.version",
+                                            "object": "malware"
+                                        }
                                     },
-                                    "credential_uid": {
-                                        "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                        "object": "owner-user-account"
+                                    "cwe_uid": {
+                                        "key": "x-ocsf-malware.cwe_uid",
+                                        "object": "malware"
                                     },
-                                    "domain": {
-                                        "key": "user-account.extensions.x-accessor-ext.domain",
-                                        "object": "owner-user-account"
+                                    "cwe_url": {
+                                        "key": "x-ocsf-malware.cwe_url",
+                                        "object": "malware"
                                     },
-                                    "email_addr": {
-                                        "key": "email-addr.value",
-                                        "object": "owner-user-account"
+                                    "modified_time": {
+                                        "key": "x-ocsf-malware.modified_time",
+                                        "object": "malware"
                                     },
-                                    "groups": {
-                                        "desc": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                            "object": "owner-user-account"
+                                    "product": {
+                                        "feature": {
+                                            "name": {
+                                                "key": "software.extensions.x-ocsf-product-ext.feature_name",
+                                                "object": "malware-software"
+                                            },
+                                            "uid": {
+                                                "key": "software.extensions.x-ocsf-product-ext.feature_uid",
+                                                "object": "malware-software"
+                                            },
+                                            "version": {
+                                                "key": "software.extensions.x-ocsf-product-ext.feature_version",
+                                                "object": "malware-software"
+                                            }
                                         },
-                                        "name": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_name",
-                                            "object": "owner-user-account"
+                                        "lang": {
+                                            "key": "software.languages",
+                                            "object": "malware-software"
                                         },
-                                        "privileges": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                            "object": "owner-user-account"
+                                        "name": {
+                                            "key": "software.name",
+                                            "object": "malware-software"
                                         },
-                                        "type": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_type",
-                                            "object": "owner-user-account"
+                                        "path": {
+                                            "key": "software.extensions.x-ocsf-product-ext.installed_path",
+                                            "object": "malware-software"
                                         },
                                         "uid": {
-                                            "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                            "object": "owner-user-account"
+                                            "key": "software.extensions.x-ocsf-product-ext.product_uid",
+                                            "object": "malware-software"
+                                        },
+                                        "vendor_name": {
+                                            "key": "software.vendor",
+                                            "object": "malware-software"
+                                        },
+                                        "version": {
+                                            "key": "software.version",
+                                            "object": "malware-software"
                                         }
                                     },
-                                    "name": {
-                                        "key": "user-account.display_name",
-                                        "object": "owner-user-account"
-                                    },
-                                    "org_uid": {
-                                        "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                        "object": "owner-user-account"
-                                    },
-                                    "session_uid": {
-                                        "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                        "object": "owner-user-account"
-                                    },
-                                    "session_uuid": {
-                                        "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                        "object": "owner-user-account"
-                                    },
                                     "type": {
-                                        "key": "user-account.extensions.x-accessor-ext.type",
-                                        "object": "owner-user-account"
-                                    },
-                                    "type_id": {
-                                        "key": "user-account.extensions.x-accessor-ext.type_id",
-                                        "object": "owner-user-account"
+                                        "key": "x-ocsf-malware.type",
+                                        "object": "malware"
                                     },
                                     "uid": {
-                                        "key": "user-account.user_id",
-                                        "object": "owner-user-account"
-                                    },
-                                    "uuid": {
-                                        "key": "user-account.extensions.x-accessor-ext.uuid",
-                                        "object": "owner-user-account"
+                                        "key": "x-ocsf-malware.uid",
+                                        "object": "malware"
                                     }
                                 },
-                                "parent_folder": [
-                                    {
-                                        "key": "directory.path",
-                                        "object": "directory"
-                                    },
-                                    {
-                                        "key": "file.parent_directory_ref",
-                                        "object": "file",
-                                        "references": "directory"
-                                    }
-                                ],
+                                "name": {
+                                    "key": "x-ocsf-malware.name",
+                                    "object": "malware"
+                                },
                                 "path": {
-                                    "key": "file.extensions.x-ocsf-file-ext.path",
-                                    "object": "file"
+                                    "key": "x-ocsf-malware.path",
+                                    "object": "malware"
+                                },
+                                "provider": {
+                                    "key": "x-ocsf-malware.provider",
+                                    "object": "malware"
+                                },
+                                "uid": {
+                                    "key": "x-ocsf-malware.uid",
+                                    "object": "malware"
+                                }
+                            },
+                            "message": {
+                                "key": "x-ocsf-cloud.message",
+                                "object": "ocsf_cloud_api"
+                            },
+                            "metadata": {
+                                "correlation_uid": {
+                                    "key": "x-ocsf-metadata.correlation_uid",
+                                    "object": "metadata"
+                                },
+                                "labels": {
+                                    "key": "x-ocsf-metadata.labels",
+                                    "object": "metadata"
+                                },
+                                "logged_time": {
+                                    "key": "x-ocsf-metadata.logged_time",
+                                    "object": "metadata"
+                                },
+                                "modified_time": {
+                                    "key": "x-ocsf-metadata.modified_time",
+                                    "object": "metadata"
+                                },
+                                "processed_time": {
+                                    "key": "x-ocsf-metadata.processed_time",
+                                    "object": "metadata"
                                 },
                                 "product": {
                                     "feature": {
                                         "name": {
                                             "key": "software.extensions.x-ocsf-product-ext.feature_name",
-                                            "object": "file1-software"
+                                            "object": "metadata-software"
                                         },
                                         "uid": {
                                             "key": "software.extensions.x-ocsf-product-ext.feature_uid",
-                                            "object": "file1-software"
+                                            "object": "metadata-software"
                                         },
                                         "version": {
                                             "key": "software.extensions.x-ocsf-product-ext.feature_version",
-                                            "object": "file1-software"
+                                            "object": "metadata-software"
                                         }
                                     },
                                     "lang": {
                                         "key": "software.languages",
-                                        "object": "file1-software"
+                                        "object": "metadata-software"
                                     },
                                     "name": {
                                         "key": "software.name",
-                                        "object": "file1-software"
+                                        "object": "metadata-software"
                                     },
                                     "path": {
                                         "key": "software.extensions.x-ocsf-product-ext.installed_path",
-                                        "object": "file1-software"
+                                        "object": "metadata-software"
                                     },
                                     "uid": {
                                         "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                                        "object": "file1-software"
+                                        "object": "metadata-software"
                                     },
                                     "vendor_name": {
                                         "key": "software.vendor",
-                                        "object": "file1-software"
+                                        "object": "metadata-software"
                                     },
                                     "version": {
                                         "key": "software.version",
-                                        "object": "file1-software"
+                                        "object": "metadata-software"
                                     }
                                 },
-                                "security_descriptor": {
-                                    "key": "file.extensions.x-ocsf-file-ext.security_descriptor",
-                                    "object": "file"
-                                },
-                                "signature": {
-                                    "key": "file.extensions.x-ocsf-file-ext.signature",
-                                    "object": "file"
-                                },
-                                "size": {
-                                    "key": "file.size",
-                                    "object": "file"
-                                },
-                                "type": {
-                                    "key": "file.extensions.x-ocsf-file-ext.type",
-                                    "object": "file"
-                                },
-                                "type_id": {
-                                    "key": "file.extensions.x-ocsf-file-ext.type_id",
-                                    "object": "file"
+                                "sequence": {
+                                    "key": "x-ocsf-metadata.sequence",
+                                    "object": "metadata",
+                                    "transformer": "ToInteger"
                                 },
                                 "uid": {
-                                    "key": "file.extensions.x-ocsf-file-ext.uid",
-                                    "object": "file"
+                                    "key": "x-ocsf-metadata.uid",
+                                    "object": "metadata"
                                 },
                                 "version": {
-                                    "key": "file.extensions.x-ocsf-file-ext.version",
-                                    "object": "file"
-                                },
-                                "xattributes": {
-                                    "key": "process.extensions.x-ocsf-process-ext.xattributes",
-                                    "object": "process"
+                                    "key": "x-ocsf-metadata.version",
+                                    "object": "metadata"
                                 }
                             },
-                            "integrity": {
-                                "key": "process.extensions.x-ocsf-process-ext.integrity",
-                                "object": "process"
-                            },
-                            "integrity_id": {
-                                "key": "process.extensions.x-ocsf-process-ext.integrity_id",
-                                "object": "process"
-                            },
-                            "lineage": {
-                                "key": "process.extensions.x-ocsf-process-ext.lineage",
-                                "object": "process"
-                            },
-                            "loaded_modules": {
-                                "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
-                                "object": "process"
-                            },
-                            "name": {
-                                "key": "process.name",
-                                "object": "process"
+                            "observables": {
+                                "name": [
+                                    {
+                                        "key": "x-ibm-observables.name",
+                                        "object": "observables"
+                                    },
+                                    {
+                                        "key": "x-ibm-finding.ioc_refs",
+                                        "object": "ibm_finding",
+                                        "references": [
+                                            "observables"
+                                        ]
+                                    }
+                                ],
+                                "type": {
+                                    "key": "x-ibm-observables.finding_type",
+                                    "object": "observables"
+                                },
+                                "type_id": {
+                                    "key": "x-ibm-observables.alert_id",
+                                    "object": "observables",
+                                    "transformer": "ToInteger"
+                                },
+                                "value": {
+                                    "key": "x-ibm-observables.description",
+                                    "object": "observables"
+                                }
                             },
-                            "parent_process": {
+                            "process": {
                                 "cmd_line": {
                                     "key": "process.command_line",
-                                    "object": "parent-process"
+                                    "object": "process"
                                 },
                                 "created_time": {
                                     "key": "process.created",
-                                    "object": "parent-process"
+                                    "object": "process"
                                 },
                                 "file": {
                                     "accessed_time": {
                                         "key": "file.accessed",
-                                        "object": "parent-file"
+                                        "object": "file"
                                     },
                                     "accessor": {
                                         "account_type": {
                                             "key": "user-account.account_type",
-                                            "object": "parent-accessor-user-account"
+                                            "object": "accessor-user-account"
                                         },
                                         "account_type_id": {
                                             "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                            "object": "parent-accessor-user-account"
+                                            "object": "accessor-user-account"
                                         },
                                         "account_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                            "object": "parent-accessor-user-account"
+                                            "object": "accessor-user-account"
                                         },
                                         "credential_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                            "object": "parent-accessor-user-account"
+                                            "object": "accessor-user-account"
                                         },
                                         "domain": {
                                             "key": "user-account.extensions.x-accessor-ext.domain",
-                                            "object": "parent-accessor-user-account"
+                                            "object": "accessor-user-account"
                                         },
                                         "email_addr": {
                                             "key": "email-addr.value",
-                                            "object": "parent-email-addr"
+                                            "object": "email-addr"
                                         },
                                         "groups": {
                                             "desc": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                                "object": "parent-accessor-user-account"
+                                                "object": "accessor-user-account"
                                             },
                                             "name": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_name",
-                                                "object": "parent-accessor-user-account"
+                                                "object": "accessor-user-account"
                                             },
                                             "privileges": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                                "object": "parent-accessor-user-account"
+                                                "object": "accessor-user-account"
                                             },
                                             "type": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_type",
-                                                "object": "parent-accessor-user-account"
+                                                "object": "accessor-user-account"
                                             },
                                             "uid": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                                "object": "parent-accessor-user-account"
+                                                "object": "accessor-user-account"
                                             }
                                         },
                                         "name": {
                                             "key": "user-account.display_name",
-                                            "object": "parent-accessor-user-account"
+                                            "object": "accessor-user-account"
                                         },
                                         "org_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                            "object": "parent-accessor-user-account"
+                                            "object": "accessor-user-account"
                                         },
                                         "session_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                            "object": "parent-accessor-user-account"
+                                            "object": "accessor-user-account"
                                         },
                                         "session_uuid": {
                                             "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                            "object": "parent-accessor-user-account"
+                                            "object": "accessor-user-account"
                                         },
                                         "type": {
                                             "key": "user-account.extensions.x-accessor-ext.type",
-                                            "object": "parent-accessor-user-account"
+                                            "object": "accessor-user-account"
                                         },
                                         "type_id": {
                                             "key": "user-account.extensions.x-accessor-ext.type_id",
-                                            "object": "parent-accessor-user-account"
+                                            "object": "accessor-user-account"
                                         },
                                         "uid": {
                                             "key": "user-account.user_id",
-                                            "object": "parent-accessor-user-account"
+                                            "object": "accessor-user-account"
                                         },
                                         "uuid": {
                                             "key": "user-account.extensions.x-accessor-ext.uuid",
-                                            "object": "parent-accessor-user-account"
+                                            "object": "accessor-user-account"
                                         }
                                     },
                                     "attributes": {
                                         "key": "file.extensions.x-ocsf-file-ext.attributes",
-                                        "object": "parent-file"
+                                        "object": "file"
                                     },
                                     "company_name": {
                                         "key": "file.extensions.x-ocsf-file-ext.company_name",
-                                        "object": "parent-file"
+                                        "object": "file"
                                     },
                                     "confidentiality": {
                                         "key": "file.extensions.x-ocsf-file-ext.confidentiality",
-                                        "object": "parent-file"
+                                        "object": "file"
                                     },
                                     "confidentiality_id": {
                                         "key": "file.extensions.x-ocsf-file-ext.confidentiality_id",
-                                        "object": "parent-file"
+                                        "object": "file"
                                     },
                                     "created_time": {
                                         "key": "file.created",
-                                        "object": "parent-file"
+                                        "object": "file"
                                     },
                                     "creator": {
                                         "account_type": {
                                             "key": "user-account.account_type",
-                                            "object": "parent-creator-user-account"
+                                            "object": "creator-user-account"
                                         },
                                         "account_type_id": {
                                             "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                            "object": "parent-creator-user-account"
+                                            "object": "creator-user-account"
                                         },
                                         "account_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                            "object": "parent-creator-user-account"
+                                            "object": "creator-user-account"
                                         },
                                         "credential_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                            "object": "parent-creator-user-account"
+                                            "object": "creator-user-account"
                                         },
                                         "domain": {
                                             "key": "user-account.extensions.x-accessor-ext.domain",
-                                            "object": "parent-creator-user-account"
+                                            "object": "creator-user-account"
                                         },
                                         "email_addr": {
                                             "key": "email-addr.value",
-                                            "object": "parent-creator-email-addr"
+                                            "object": "creator-email-addr"
                                         },
                                         "groups": {
                                             "desc": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                                "object": "parent-creator-user-account"
+                                                "object": "creator-user-account"
                                             },
                                             "name": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_name",
-                                                "object": "parent-creator-user-account"
+                                                "object": "creator-user-account"
                                             },
                                             "privileges": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                                "object": "parent-creator-user-account"
+                                                "object": "creator-user-account"
                                             },
                                             "type": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_type",
-                                                "object": "parent-creator-user-account"
+                                                "object": "creator-user-account"
                                             },
                                             "uid": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                                "object": "parent-creator-user-account"
+                                                "object": "creator-user-account"
                                             }
                                         },
                                         "name": {
                                             "key": "user-account.display_name",
-                                            "object": "parent-creator-user-account"
+                                            "object": "creator-user-account"
                                         },
                                         "org_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                            "object": "parent-creator-user-account"
+                                            "object": "creator-user-account"
                                         },
                                         "session_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                            "object": "parent-creator-user-account"
+                                            "object": "creator-user-account"
                                         },
                                         "session_uuid": {
                                             "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                            "object": "parent-creator-user-account"
+                                            "object": "creator-user-account"
                                         },
                                         "type": {
                                             "key": "user-account.extensions.x-accessor-ext.type",
-                                            "object": "parent-creator-user-account"
+                                            "object": "creator-user-account"
                                         },
                                         "type_id": {
                                             "key": "user-account.extensions.x-accessor-ext.type_id",
-                                            "object": "parent-creator-user-account"
+                                            "object": "creator-user-account"
                                         },
                                         "uid": {
                                             "key": "user-account.user_id",
-                                            "object": "parent-creator-user-account"
+                                            "object": "creator-user-account"
                                         },
                                         "uuid": {
                                             "key": "user-account.extensions.x-accessor-ext.uuid",
-                                            "object": "parent-creator-user-account"
+                                            "object": "creator-user-account"
                                         }
                                     },
                                     "desc": {
                                         "key": "file.extensions.x-ocsf-file-ext.description",
-                                        "object": "parent-file"
+                                        "object": "file"
                                     },
                                     "hashes": {
                                         "CTPH": {
                                             "key": "file.hashes.CTPH",
-                                            "object": "parent-file"
+                                            "object": "file"
                                         },
                                         "MD5": {
                                             "key": "file.hashes.MD5",
-                                            "object": "parent-file"
+                                            "object": "file"
                                         },
                                         "Other": {
                                             "key": "file.hashes.Other",
-                                            "object": "parent-file"
+                                            "object": "file"
                                         },
                                         "SHA-1": {
                                             "key": "file.hashes.SHA-1",
-                                            "object": "parent-file"
+                                            "object": "file"
                                         },
                                         "SHA-256": {
                                             "key": "file.hashes.SHA-256",
-                                            "object": "parent-file"
+                                            "object": "file"
                                         },
                                         "SHA-512": {
                                             "key": "file.hashes.SHA-512",
-                                            "object": "parent-file"
+                                            "object": "file"
                                         },
                                         "Unknown": {
                                             "key": "file.hashes.Unknown",
-                                            "object": "parent-file"
+                                            "object": "file"
                                         }
                                     },
                                     "is_system": {
                                         "key": "process.extensions.x-ocsf-process-ext.is_system",
-                                        "object": "parent-process"
+                                        "object": "process"
                                     },
                                     "mime_type": {
                                         "key": "process.mime_type",
-                                        "object": "parent-process"
+                                        "object": "process"
                                     },
                                     "modified_time": {
                                         "key": "process.extensions.x-ocsf-process-ext.modified_time",
-                                        "object": "parent-process"
+                                        "object": "process"
                                     },
                                     "modifier": {
                                         "account_type": {
                                             "key": "user-account.account_type",
-                                            "object": "parent-modifier-user-account"
+                                            "object": "modifier-user-account"
                                         },
                                         "account_type_id": {
                                             "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                            "object": "parent-modifier-user-account"
+                                            "object": "modifier-user-account"
                                         },
                                         "account_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                            "object": "parent-modifier-user-account"
+                                            "object": "modifier-user-account"
                                         },
                                         "credential_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                            "object": "parent-modifier-user-account"
+                                            "object": "modifier-user-account"
                                         },
                                         "domain": {
                                             "key": "user-account.extensions.x-accessor-ext.domain",
-                                            "object": "parent-modifier-user-account"
+                                            "object": "modifier-user-account"
                                         },
                                         "email_addr": {
                                             "key": "email-addr.value",
-                                            "object": "parent-modifier-email-addr"
+                                            "object": "modifier-email-addr"
                                         },
                                         "groups": {
                                             "desc": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                                "object": "parent-modifier-user-account"
+                                                "object": "modifier-user-account"
                                             },
                                             "name": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_name",
-                                                "object": "parent-modifier-user-account"
+                                                "object": "modifier-user-account"
                                             },
                                             "privileges": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                                "object": "parent-modifier-user-account"
+                                                "object": "modifier-user-account"
                                             },
                                             "type": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_type",
-                                                "object": "parent-modifier-user-account"
+                                                "object": "modifier-user-account"
                                             },
                                             "uid": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                                "object": "parent-modifier-user-account"
+                                                "object": "modifier-user-account"
                                             }
                                         },
                                         "name": {
                                             "key": "user-account.display_name",
-                                            "object": "parent-modifier-user-account"
+                                            "object": "modifier-user-account"
                                         },
                                         "org_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                            "object": "parent-modifier-user-account"
+                                            "object": "modifier-user-account"
                                         },
                                         "session_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                            "object": "parent-modifier-user-account"
+                                            "object": "modifier-user-account"
                                         },
                                         "session_uuid": {
                                             "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                            "object": "parent-modifier-user-account"
+                                            "object": "modifier-user-account"
                                         },
                                         "type": {
                                             "key": "user-account.extensions.x-accessor-ext.type",
-                                            "object": "parent-modifier-user-account"
+                                            "object": "modifier-user-account"
                                         },
                                         "type_id": {
                                             "key": "user-account.extensions.x-accessor-ext.type_id",
-                                            "object": "parent-modifier-user-account"
+                                            "object": "modifier-user-account"
                                         },
                                         "uid": {
                                             "key": "user-account.user_id",
-                                            "object": "parent-modifier-user-account"
+                                            "object": "modifier-user-account"
                                         },
                                         "uuid": {
                                             "key": "user-account.extensions.x-accessor-ext.uuid",
-                                            "object": "parent-modifier-user-account"
+                                            "object": "modifier-user-account"
                                         }
                                     },
                                     "name": [
                                         {
                                             "key": "file.name",
-                                            "object": "parent-file"
+                                            "object": "file"
                                         },
                                         {
                                             "key": "process.binary_ref",
-                                            "object": "parent-process",
-                                            "references": "parent-file"
+                                            "object": "process",
+                                            "references": "file"
                                         }
                                     ],
                                     "owner": {
                                         "account_type": {
                                             "key": "user-account.account_type",
-                                            "object": "parent-owner-user-account"
+                                            "object": "owner-user-account"
                                         },
                                         "account_type_id": {
                                             "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                            "object": "parent-owner-user-account"
+                                            "object": "owner-user-account"
                                         },
                                         "account_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                            "object": "parent-owner-user-account"
+                                            "object": "owner-user-account"
                                         },
                                         "credential_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                            "object": "parent-owner-user-account"
+                                            "object": "owner-user-account"
                                         },
                                         "domain": {
                                             "key": "user-account.extensions.x-accessor-ext.domain",
-                                            "object": "parent-owner-user-account"
+                                            "object": "owner-user-account"
                                         },
                                         "email_addr": {
                                             "key": "email-addr.value",
-                                            "object": "parent-owner-email-addr"
+                                            "object": "owner-user-account"
                                         },
                                         "groups": {
                                             "desc": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                                "object": "parent-owner-user-account"
+                                                "object": "owner-user-account"
                                             },
                                             "name": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_name",
-                                                "object": "parent-owner-user-account"
+                                                "object": "owner-user-account"
                                             },
                                             "privileges": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                                "object": "parent-owner-user-account"
+                                                "object": "owner-user-account"
                                             },
                                             "type": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_type",
-                                                "object": "parent-owner-user-account"
+                                                "object": "owner-user-account"
                                             },
                                             "uid": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                                "object": "parent-owner-user-account"
+                                                "object": "owner-user-account"
                                             }
                                         },
                                         "name": {
                                             "key": "user-account.display_name",
-                                            "object": "parent-owner-user-account"
+                                            "object": "owner-user-account"
                                         },
                                         "org_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                            "object": "parent-owner-user-account"
+                                            "object": "owner-user-account"
                                         },
                                         "session_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                            "object": "parent-owner-user-account"
+                                            "object": "owner-user-account"
                                         },
                                         "session_uuid": {
                                             "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                            "object": "parent-owner-user-account"
+                                            "object": "owner-user-account"
                                         },
                                         "type": {
                                             "key": "user-account.extensions.x-accessor-ext.type",
-                                            "object": "parent-owner-user-account"
+                                            "object": "owner-user-account"
                                         },
                                         "type_id": {
                                             "key": "user-account.extensions.x-accessor-ext.type_id",
-                                            "object": "parent-owner-user-account"
+                                            "object": "owner-user-account"
                                         },
                                         "uid": {
                                             "key": "user-account.user_id",
-                                            "object": "parent-owner-user-account"
+                                            "object": "owner-user-account"
                                         },
                                         "uuid": {
                                             "key": "user-account.extensions.x-accessor-ext.uuid",
-                                            "object": "parent-owner-user-account"
+                                            "object": "owner-user-account"
                                         }
                                     },
                                     "parent_folder": [
                                         {
                                             "key": "directory.path",
-                                            "object": "parent-directory"
+                                            "object": "directory"
                                         },
                                         {
                                             "key": "file.parent_directory_ref",
-                                            "object": "parent-file",
-                                            "references": "parent-directory"
+                                            "object": "file",
+                                            "references": "directory"
                                         }
                                     ],
                                     "path": {
                                         "key": "file.extensions.x-ocsf-file-ext.path",
-                                        "object": "parent-file"
+                                        "object": "file"
                                     },
                                     "product": {
                                         "feature": {
                                             "name": {
                                                 "key": "software.extensions.x-ocsf-product-ext.feature_name",
-                                                "object": "file-software"
+                                                "object": "file1-software"
                                             },
                                             "uid": {
                                                 "key": "software.extensions.x-ocsf-product-ext.feature_uid",
-                                                "object": "file-software"
+                                                "object": "file1-software"
                                             },
                                             "version": {
                                                 "key": "software.extensions.x-ocsf-product-ext.feature_version",
-                                                "object": "file-software"
+                                                "object": "file1-software"
                                             }
                                         },
                                         "lang": {
                                             "key": "software.languages",
-                                            "object": "file-software"
+                                            "object": "file1-software"
                                         },
                                         "name": {
                                             "key": "software.name",
-                                            "object": "file-software"
+                                            "object": "file1-software"
                                         },
                                         "path": {
                                             "key": "software.extensions.x-ocsf-product-ext.installed_path",
-                                            "object": "file-software"
+                                            "object": "file1-software"
                                         },
                                         "uid": {
                                             "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                                            "object": "file-software"
+                                            "object": "file1-software"
                                         },
                                         "vendor_name": {
                                             "key": "software.vendor",
-                                            "object": "file-software"
+                                            "object": "file1-software"
                                         },
                                         "version": {
                                             "key": "software.version",
-                                            "object": "file-software"
+                                            "object": "file1-software"
                                         }
                                     },
                                     "security_descriptor": {
                                         "key": "file.extensions.x-ocsf-file-ext.security_descriptor",
-                                        "object": "parent-file"
+                                        "object": "file"
                                     },
                                     "signature": {
                                         "key": "file.extensions.x-ocsf-file-ext.signature",
-                                        "object": "parent-file"
+                                        "object": "file"
                                     },
                                     "size": {
                                         "key": "file.size",
-                                        "object": "parent-file"
+                                        "object": "file"
                                     },
                                     "type": {
                                         "key": "file.extensions.x-ocsf-file-ext.type",
-                                        "object": "parent-file"
+                                        "object": "file"
                                     },
                                     "type_id": {
                                         "key": "file.extensions.x-ocsf-file-ext.type_id",
-                                        "object": "parent-file"
+                                        "object": "file"
                                     },
                                     "uid": {
                                         "key": "file.extensions.x-ocsf-file-ext.uid",
-                                        "object": "parent-file"
+                                        "object": "file"
                                     },
                                     "version": {
                                         "key": "file.extensions.x-ocsf-file-ext.version",
-                                        "object": "parent-file"
+                                        "object": "file"
                                     },
                                     "xattributes": {
                                         "key": "process.extensions.x-ocsf-process-ext.xattributes",
-                                        "object": "parent-process"
+                                        "object": "process"
                                     }
                                 },
                                 "integrity": {
                                     "key": "process.extensions.x-ocsf-process-ext.integrity",
-                                    "object": "parent-process"
+                                    "object": "process"
                                 },
                                 "integrity_id": {
                                     "key": "process.extensions.x-ocsf-process-ext.integrity_id",
-                                    "object": "parent-process"
+                                    "object": "process"
                                 },
                                 "lineage": {
                                     "key": "process.extensions.x-ocsf-process-ext.lineage",
-                                    "object": "parent-process"
+                                    "object": "process"
                                 },
                                 "loaded_modules": {
                                     "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
-                                    "object": "parent-process"
+                                    "object": "process"
                                 },
                                 "name": {
                                     "key": "process.name",
-                                    "object": "parent-process"
+                                    "object": "process"
+                                },
+                                "parent_process": {
+                                    "cmd_line": {
+                                        "key": "process.command_line",
+                                        "object": "parent-process"
+                                    },
+                                    "created_time": {
+                                        "key": "process.created",
+                                        "object": "parent-process"
+                                    },
+                                    "file": {
+                                        "accessed_time": {
+                                            "key": "file.accessed",
+                                            "object": "parent-file"
+                                        },
+                                        "accessor": {
+                                            "account_type": {
+                                                "key": "user-account.account_type",
+                                                "object": "parent-accessor-user-account"
+                                            },
+                                            "account_type_id": {
+                                                "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                                                "object": "parent-accessor-user-account"
+                                            },
+                                            "account_uid": {
+                                                "key": "user-account.extensions.x-accessor-ext.account_uid",
+                                                "object": "parent-accessor-user-account"
+                                            },
+                                            "credential_uid": {
+                                                "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                                                "object": "parent-accessor-user-account"
+                                            },
+                                            "domain": {
+                                                "key": "user-account.extensions.x-accessor-ext.domain",
+                                                "object": "parent-accessor-user-account"
+                                            },
+                                            "email_addr": {
+                                                "key": "email-addr.value",
+                                                "object": "parent-email-addr"
+                                            },
+                                            "groups": {
+                                                "desc": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_desc",
+                                                    "object": "parent-accessor-user-account"
+                                                },
+                                                "name": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_name",
+                                                    "object": "parent-accessor-user-account"
+                                                },
+                                                "privileges": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                                                    "object": "parent-accessor-user-account"
+                                                },
+                                                "type": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_type",
+                                                    "object": "parent-accessor-user-account"
+                                                },
+                                                "uid": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_uid",
+                                                    "object": "parent-accessor-user-account"
+                                                }
+                                            },
+                                            "name": {
+                                                "key": "user-account.display_name",
+                                                "object": "parent-accessor-user-account"
+                                            },
+                                            "org_uid": {
+                                                "key": "user-account.extensions.x-accessor-ext.org_uid",
+                                                "object": "parent-accessor-user-account"
+                                            },
+                                            "session_uid": {
+                                                "key": "user-account.extensions.x-accessor-ext.session_uid",
+                                                "object": "parent-accessor-user-account"
+                                            },
+                                            "session_uuid": {
+                                                "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                                                "object": "parent-accessor-user-account"
+                                            },
+                                            "type": {
+                                                "key": "user-account.extensions.x-accessor-ext.type",
+                                                "object": "parent-accessor-user-account"
+                                            },
+                                            "type_id": {
+                                                "key": "user-account.extensions.x-accessor-ext.type_id",
+                                                "object": "parent-accessor-user-account"
+                                            },
+                                            "uid": {
+                                                "key": "user-account.user_id",
+                                                "object": "parent-accessor-user-account"
+                                            },
+                                            "uuid": {
+                                                "key": "user-account.extensions.x-accessor-ext.uuid",
+                                                "object": "parent-accessor-user-account"
+                                            }
+                                        },
+                                        "attributes": {
+                                            "key": "file.extensions.x-ocsf-file-ext.attributes",
+                                            "object": "parent-file"
+                                        },
+                                        "company_name": {
+                                            "key": "file.extensions.x-ocsf-file-ext.company_name",
+                                            "object": "parent-file"
+                                        },
+                                        "confidentiality": {
+                                            "key": "file.extensions.x-ocsf-file-ext.confidentiality",
+                                            "object": "parent-file"
+                                        },
+                                        "confidentiality_id": {
+                                            "key": "file.extensions.x-ocsf-file-ext.confidentiality_id",
+                                            "object": "parent-file"
+                                        },
+                                        "created_time": {
+                                            "key": "file.created",
+                                            "object": "parent-file"
+                                        },
+                                        "creator": {
+                                            "account_type": {
+                                                "key": "user-account.account_type",
+                                                "object": "parent-creator-user-account"
+                                            },
+                                            "account_type_id": {
+                                                "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                                                "object": "parent-creator-user-account"
+                                            },
+                                            "account_uid": {
+                                                "key": "user-account.extensions.x-accessor-ext.account_uid",
+                                                "object": "parent-creator-user-account"
+                                            },
+                                            "credential_uid": {
+                                                "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                                                "object": "parent-creator-user-account"
+                                            },
+                                            "domain": {
+                                                "key": "user-account.extensions.x-accessor-ext.domain",
+                                                "object": "parent-creator-user-account"
+                                            },
+                                            "email_addr": {
+                                                "key": "email-addr.value",
+                                                "object": "parent-creator-email-addr"
+                                            },
+                                            "groups": {
+                                                "desc": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_desc",
+                                                    "object": "parent-creator-user-account"
+                                                },
+                                                "name": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_name",
+                                                    "object": "parent-creator-user-account"
+                                                },
+                                                "privileges": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                                                    "object": "parent-creator-user-account"
+                                                },
+                                                "type": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_type",
+                                                    "object": "parent-creator-user-account"
+                                                },
+                                                "uid": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_uid",
+                                                    "object": "parent-creator-user-account"
+                                                }
+                                            },
+                                            "name": {
+                                                "key": "user-account.display_name",
+                                                "object": "parent-creator-user-account"
+                                            },
+                                            "org_uid": {
+                                                "key": "user-account.extensions.x-accessor-ext.org_uid",
+                                                "object": "parent-creator-user-account"
+                                            },
+                                            "session_uid": {
+                                                "key": "user-account.extensions.x-accessor-ext.session_uid",
+                                                "object": "parent-creator-user-account"
+                                            },
+                                            "session_uuid": {
+                                                "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                                                "object": "parent-creator-user-account"
+                                            },
+                                            "type": {
+                                                "key": "user-account.extensions.x-accessor-ext.type",
+                                                "object": "parent-creator-user-account"
+                                            },
+                                            "type_id": {
+                                                "key": "user-account.extensions.x-accessor-ext.type_id",
+                                                "object": "parent-creator-user-account"
+                                            },
+                                            "uid": {
+                                                "key": "user-account.user_id",
+                                                "object": "parent-creator-user-account"
+                                            },
+                                            "uuid": {
+                                                "key": "user-account.extensions.x-accessor-ext.uuid",
+                                                "object": "parent-creator-user-account"
+                                            }
+                                        },
+                                        "desc": {
+                                            "key": "file.extensions.x-ocsf-file-ext.description",
+                                            "object": "parent-file"
+                                        },
+                                        "hashes": {
+                                            "CTPH": {
+                                                "key": "file.hashes.CTPH",
+                                                "object": "parent-file"
+                                            },
+                                            "MD5": {
+                                                "key": "file.hashes.MD5",
+                                                "object": "parent-file"
+                                            },
+                                            "Other": {
+                                                "key": "file.hashes.Other",
+                                                "object": "parent-file"
+                                            },
+                                            "SHA-1": {
+                                                "key": "file.hashes.SHA-1",
+                                                "object": "parent-file"
+                                            },
+                                            "SHA-256": {
+                                                "key": "file.hashes.SHA-256",
+                                                "object": "parent-file"
+                                            },
+                                            "SHA-512": {
+                                                "key": "file.hashes.SHA-512",
+                                                "object": "parent-file"
+                                            },
+                                            "Unknown": {
+                                                "key": "file.hashes.Unknown",
+                                                "object": "parent-file"
+                                            }
+                                        },
+                                        "is_system": {
+                                            "key": "process.extensions.x-ocsf-process-ext.is_system",
+                                            "object": "parent-process"
+                                        },
+                                        "mime_type": {
+                                            "key": "process.mime_type",
+                                            "object": "parent-process"
+                                        },
+                                        "modified_time": {
+                                            "key": "process.extensions.x-ocsf-process-ext.modified_time",
+                                            "object": "parent-process"
+                                        },
+                                        "modifier": {
+                                            "account_type": {
+                                                "key": "user-account.account_type",
+                                                "object": "parent-modifier-user-account"
+                                            },
+                                            "account_type_id": {
+                                                "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                                                "object": "parent-modifier-user-account"
+                                            },
+                                            "account_uid": {
+                                                "key": "user-account.extensions.x-accessor-ext.account_uid",
+                                                "object": "parent-modifier-user-account"
+                                            },
+                                            "credential_uid": {
+                                                "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                                                "object": "parent-modifier-user-account"
+                                            },
+                                            "domain": {
+                                                "key": "user-account.extensions.x-accessor-ext.domain",
+                                                "object": "parent-modifier-user-account"
+                                            },
+                                            "email_addr": {
+                                                "key": "email-addr.value",
+                                                "object": "parent-modifier-email-addr"
+                                            },
+                                            "groups": {
+                                                "desc": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_desc",
+                                                    "object": "parent-modifier-user-account"
+                                                },
+                                                "name": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_name",
+                                                    "object": "parent-modifier-user-account"
+                                                },
+                                                "privileges": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                                                    "object": "parent-modifier-user-account"
+                                                },
+                                                "type": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_type",
+                                                    "object": "parent-modifier-user-account"
+                                                },
+                                                "uid": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_uid",
+                                                    "object": "parent-modifier-user-account"
+                                                }
+                                            },
+                                            "name": {
+                                                "key": "user-account.display_name",
+                                                "object": "parent-modifier-user-account"
+                                            },
+                                            "org_uid": {
+                                                "key": "user-account.extensions.x-accessor-ext.org_uid",
+                                                "object": "parent-modifier-user-account"
+                                            },
+                                            "session_uid": {
+                                                "key": "user-account.extensions.x-accessor-ext.session_uid",
+                                                "object": "parent-modifier-user-account"
+                                            },
+                                            "session_uuid": {
+                                                "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                                                "object": "parent-modifier-user-account"
+                                            },
+                                            "type": {
+                                                "key": "user-account.extensions.x-accessor-ext.type",
+                                                "object": "parent-modifier-user-account"
+                                            },
+                                            "type_id": {
+                                                "key": "user-account.extensions.x-accessor-ext.type_id",
+                                                "object": "parent-modifier-user-account"
+                                            },
+                                            "uid": {
+                                                "key": "user-account.user_id",
+                                                "object": "parent-modifier-user-account"
+                                            },
+                                            "uuid": {
+                                                "key": "user-account.extensions.x-accessor-ext.uuid",
+                                                "object": "parent-modifier-user-account"
+                                            }
+                                        },
+                                        "name": [
+                                            {
+                                                "key": "file.name",
+                                                "object": "parent-file"
+                                            },
+                                            {
+                                                "key": "process.binary_ref",
+                                                "object": "parent-process",
+                                                "references": "parent-file"
+                                            }
+                                        ],
+                                        "owner": {
+                                            "account_type": {
+                                                "key": "user-account.account_type",
+                                                "object": "parent-owner-user-account"
+                                            },
+                                            "account_type_id": {
+                                                "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                                                "object": "parent-owner-user-account"
+                                            },
+                                            "account_uid": {
+                                                "key": "user-account.extensions.x-accessor-ext.account_uid",
+                                                "object": "parent-owner-user-account"
+                                            },
+                                            "credential_uid": {
+                                                "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                                                "object": "parent-owner-user-account"
+                                            },
+                                            "domain": {
+                                                "key": "user-account.extensions.x-accessor-ext.domain",
+                                                "object": "parent-owner-user-account"
+                                            },
+                                            "email_addr": {
+                                                "key": "email-addr.value",
+                                                "object": "parent-owner-email-addr"
+                                            },
+                                            "groups": {
+                                                "desc": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_desc",
+                                                    "object": "parent-owner-user-account"
+                                                },
+                                                "name": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_name",
+                                                    "object": "parent-owner-user-account"
+                                                },
+                                                "privileges": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                                                    "object": "parent-owner-user-account"
+                                                },
+                                                "type": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_type",
+                                                    "object": "parent-owner-user-account"
+                                                },
+                                                "uid": {
+                                                    "key": "user-account.extensions.x-accessor-ext.group_uid",
+                                                    "object": "parent-owner-user-account"
+                                                }
+                                            },
+                                            "name": {
+                                                "key": "user-account.display_name",
+                                                "object": "parent-owner-user-account"
+                                            },
+                                            "org_uid": {
+                                                "key": "user-account.extensions.x-accessor-ext.org_uid",
+                                                "object": "parent-owner-user-account"
+                                            },
+                                            "session_uid": {
+                                                "key": "user-account.extensions.x-accessor-ext.session_uid",
+                                                "object": "parent-owner-user-account"
+                                            },
+                                            "session_uuid": {
+                                                "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                                                "object": "parent-owner-user-account"
+                                            },
+                                            "type": {
+                                                "key": "user-account.extensions.x-accessor-ext.type",
+                                                "object": "parent-owner-user-account"
+                                            },
+                                            "type_id": {
+                                                "key": "user-account.extensions.x-accessor-ext.type_id",
+                                                "object": "parent-owner-user-account"
+                                            },
+                                            "uid": {
+                                                "key": "user-account.user_id",
+                                                "object": "parent-owner-user-account"
+                                            },
+                                            "uuid": {
+                                                "key": "user-account.extensions.x-accessor-ext.uuid",
+                                                "object": "parent-owner-user-account"
+                                            }
+                                        },
+                                        "parent_folder": [
+                                            {
+                                                "key": "directory.path",
+                                                "object": "parent-directory"
+                                            },
+                                            {
+                                                "key": "file.parent_directory_ref",
+                                                "object": "parent-file",
+                                                "references": "parent-directory"
+                                            }
+                                        ],
+                                        "path": {
+                                            "key": "file.extensions.x-ocsf-file-ext.path",
+                                            "object": "parent-file"
+                                        },
+                                        "product": {
+                                            "feature": {
+                                                "name": {
+                                                    "key": "software.extensions.x-ocsf-product-ext.feature_name",
+                                                    "object": "file-software"
+                                                },
+                                                "uid": {
+                                                    "key": "software.extensions.x-ocsf-product-ext.feature_uid",
+                                                    "object": "file-software"
+                                                },
+                                                "version": {
+                                                    "key": "software.extensions.x-ocsf-product-ext.feature_version",
+                                                    "object": "file-software"
+                                                }
+                                            },
+                                            "lang": {
+                                                "key": "software.languages",
+                                                "object": "file-software"
+                                            },
+                                            "name": {
+                                                "key": "software.name",
+                                                "object": "file-software"
+                                            },
+                                            "path": {
+                                                "key": "software.extensions.x-ocsf-product-ext.installed_path",
+                                                "object": "file-software"
+                                            },
+                                            "uid": {
+                                                "key": "software.extensions.x-ocsf-product-ext.product_uid",
+                                                "object": "file-software"
+                                            },
+                                            "vendor_name": {
+                                                "key": "software.vendor",
+                                                "object": "file-software"
+                                            },
+                                            "version": {
+                                                "key": "software.version",
+                                                "object": "file-software"
+                                            }
+                                        },
+                                        "security_descriptor": {
+                                            "key": "file.extensions.x-ocsf-file-ext.security_descriptor",
+                                            "object": "parent-file"
+                                        },
+                                        "signature": {
+                                            "key": "file.extensions.x-ocsf-file-ext.signature",
+                                            "object": "parent-file"
+                                        },
+                                        "size": {
+                                            "key": "file.size",
+                                            "object": "parent-file"
+                                        },
+                                        "type": {
+                                            "key": "file.extensions.x-ocsf-file-ext.type",
+                                            "object": "parent-file"
+                                        },
+                                        "type_id": {
+                                            "key": "file.extensions.x-ocsf-file-ext.type_id",
+                                            "object": "parent-file"
+                                        },
+                                        "uid": {
+                                            "key": "file.extensions.x-ocsf-file-ext.uid",
+                                            "object": "parent-file"
+                                        },
+                                        "version": {
+                                            "key": "file.extensions.x-ocsf-file-ext.version",
+                                            "object": "parent-file"
+                                        },
+                                        "xattributes": {
+                                            "key": "process.extensions.x-ocsf-process-ext.xattributes",
+                                            "object": "parent-process"
+                                        }
+                                    },
+                                    "integrity": {
+                                        "key": "process.extensions.x-ocsf-process-ext.integrity",
+                                        "object": "parent-process"
+                                    },
+                                    "integrity_id": {
+                                        "key": "process.extensions.x-ocsf-process-ext.integrity_id",
+                                        "object": "parent-process"
+                                    },
+                                    "lineage": {
+                                        "key": "process.extensions.x-ocsf-process-ext.lineage",
+                                        "object": "parent-process"
+                                    },
+                                    "loaded_modules": {
+                                        "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
+                                        "object": "parent-process"
+                                    },
+                                    "name": {
+                                        "key": "process.name",
+                                        "object": "parent-process"
+                                    },
+                                    "pid": [
+                                        {
+                                            "key": "process.pid",
+                                            "object": "parent-process"
+                                        },
+                                        {
+                                            "key": "process.child_refs",
+                                            "object": "parent-process",
+                                            "references": [
+                                                "process"
+                                            ]
+                                        }
+                                    ],
+                                    "sandbox": {
+                                        "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
+                                        "object": "parent-process"
+                                    },
+                                    "terminated_time": {
+                                        "key": "process.extensions.x-ocsf-process-ext.terminated_time",
+                                        "object": "parent-process"
+                                    },
+                                    "tid": {
+                                        "key": "process.extensions.x-ocsf-process-ext.tid",
+                                        "object": "parent-process"
+                                    },
+                                    "uid": {
+                                        "key": "process.x_unique_id",
+                                        "object": "parent-process"
+                                    },
+                                    "user": {
+                                        "account_type": {
+                                            "key": "user-account.account_type",
+                                            "object": "parent-process-user-account"
+                                        },
+                                        "account_type_id": {
+                                            "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                                            "object": "parent-process-user-account"
+                                        },
+                                        "account_uid": {
+                                            "key": "user-account.extensions.x-accessor-ext.account_uid",
+                                            "object": "parent-process-user-account"
+                                        },
+                                        "credential_uid": {
+                                            "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                                            "object": "parent-process-user-account"
+                                        },
+                                        "domain": {
+                                            "key": "user-account.extensions.x-accessor-ext.domain",
+                                            "object": "parent-process-user-account"
+                                        },
+                                        "email_addr": {
+                                            "key": "email-addr.value",
+                                            "object": "parent-process-email-addr"
+                                        },
+                                        "groups": {
+                                            "desc": {
+                                                "key": "user-account.extensions.x-accessor-ext.group_desc",
+                                                "object": "parent-process-user-account"
+                                            },
+                                            "name": {
+                                                "key": "user-account.extensions.x-accessor-ext.group_name",
+                                                "object": "parent-process-user-account"
+                                            },
+                                            "privileges": {
+                                                "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                                                "object": "parent-process-user-account"
+                                            },
+                                            "type": {
+                                                "key": "user-account.extensions.x-accessor-ext.group_type",
+                                                "object": "parent-process-user-account"
+                                            },
+                                            "uid": {
+                                                "key": "user-account.extensions.x-accessor-ext.group_uid",
+                                                "object": "parent-process-user-account"
+                                            }
+                                        },
+                                        "name": {
+                                            "key": "user-account.display_name",
+                                            "object": "parent-process-user-account"
+                                        },
+                                        "org_uid": {
+                                            "key": "user-account.extensions.x-accessor-ext.org_uid",
+                                            "object": "parent-process-user-account"
+                                        },
+                                        "session_uid": {
+                                            "key": "user-account.extensions.x-accessor-ext.session_uid",
+                                            "object": "parent-process-user-account"
+                                        },
+                                        "session_uuid": {
+                                            "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                                            "object": "parent-process-user-account"
+                                        },
+                                        "type": {
+                                            "key": "user-account.extensions.x-accessor-ext.type",
+                                            "object": "parent-process-user-account"
+                                        },
+                                        "type_id": {
+                                            "key": "user-account.extensions.x-accessor-ext.type_id",
+                                            "object": "parent-process-user-account"
+                                        },
+                                        "uid": [
+                                            {
+                                                "key": "user-account.user_id",
+                                                "object": "parent-process-user-account"
+                                            },
+                                            {
+                                                "key": "user-account.creator_user_ref",
+                                                "object": "parent-process",
+                                                "references": "process-user-account"
+                                            }
+                                        ],
+                                        "uuid": {
+                                            "key": "user-account.extensions.x-accessor-ext.uuid",
+                                            "object": "parent-process-user-account"
+                                        }
+                                    },
+                                    "xattributes": {
+                                        "key": "process.extensions.x-ocsf-process-ext.xattributes",
+                                        "object": "parent-process"
+                                    }
                                 },
                                 "pid": [
                                     {
                                         "key": "process.pid",
-                                        "object": "parent-process"
+                                        "object": "process"
                                     },
                                     {
-                                        "key": "process.child_refs",
-                                        "object": "parent-process",
+                                        "key": "process.parent_ref",
+                                        "object": "process",
                                         "references": [
-                                            "process"
+                                            "parent-process"
                                         ]
                                     }
                                 ],
                                 "sandbox": {
                                     "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
-                                    "object": "parent-process"
+                                    "object": "process"
                                 },
                                 "terminated_time": {
                                     "key": "process.extensions.x-ocsf-process-ext.terminated_time",
-                                    "object": "parent-process"
+                                    "object": "process"
                                 },
                                 "tid": {
                                     "key": "process.extensions.x-ocsf-process-ext.tid",
-                                    "object": "parent-process"
+                                    "object": "process"
                                 },
                                 "uid": {
                                     "key": "process.x_unique_id",
-                                    "object": "parent-process"
+                                    "object": "process"
                                 },
                                 "user": {
                                     "account_type": {
                                         "key": "user-account.account_type",
-                                        "object": "parent-process-user-account"
+                                        "object": "process-user-account"
                                     },
                                     "account_type_id": {
                                         "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                        "object": "parent-process-user-account"
+                                        "object": "process-user-account"
                                     },
                                     "account_uid": {
                                         "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                        "object": "parent-process-user-account"
+                                        "object": "process-user-account"
                                     },
                                     "credential_uid": {
                                         "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                        "object": "parent-process-user-account"
+                                        "object": "process-user-account"
                                     },
                                     "domain": {
                                         "key": "user-account.extensions.x-accessor-ext.domain",
-                                        "object": "parent-process-user-account"
+                                        "object": "process-user-account"
                                     },
                                     "email_addr": {
                                         "key": "email-addr.value",
-                                        "object": "parent-process-email-addr"
+                                        "object": "process-email-addr"
                                     },
                                     "groups": {
                                         "desc": {
                                             "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                            "object": "parent-process-user-account"
+                                            "object": "process-user-account"
                                         },
                                         "name": {
                                             "key": "user-account.extensions.x-accessor-ext.group_name",
-                                            "object": "parent-process-user-account"
+                                            "object": "process-user-account"
                                         },
                                         "privileges": {
                                             "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                            "object": "parent-process-user-account"
+                                            "object": "process-user-account"
                                         },
                                         "type": {
                                             "key": "user-account.extensions.x-accessor-ext.group_type",
-                                            "object": "parent-process-user-account"
+                                            "object": "process-user-account"
                                         },
                                         "uid": {
                                             "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                            "object": "parent-process-user-account"
+                                            "object": "process-user-account"
                                         }
                                     },
                                     "name": {
                                         "key": "user-account.display_name",
-                                        "object": "parent-process-user-account"
+                                        "object": "process-user-account"
                                     },
                                     "org_uid": {
                                         "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                        "object": "parent-process-user-account"
+                                        "object": "process-user-account"
                                     },
                                     "session_uid": {
                                         "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                        "object": "parent-process-user-account"
+                                        "object": "process-user-account"
                                     },
                                     "session_uuid": {
                                         "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                        "object": "parent-process-user-account"
+                                        "object": "process-user-account"
                                     },
                                     "type": {
                                         "key": "user-account.extensions.x-accessor-ext.type",
-                                        "object": "parent-process-user-account"
+                                        "object": "process-user-account"
                                     },
                                     "type_id": {
                                         "key": "user-account.extensions.x-accessor-ext.type_id",
-                                        "object": "parent-process-user-account"
+                                        "object": "process-user-account"
                                     },
                                     "uid": [
                                         {
                                             "key": "user-account.user_id",
-                                            "object": "parent-process-user-account"
+                                            "object": "process-user-account"
                                         },
                                         {
                                             "key": "user-account.creator_user_ref",
-                                            "object": "parent-process",
+                                            "object": "process",
                                             "references": "process-user-account"
                                         }
                                     ],
                                     "uuid": {
                                         "key": "user-account.extensions.x-accessor-ext.uuid",
-                                        "object": "parent-process-user-account"
+                                        "object": "process-user-account"
                                     }
                                 },
                                 "xattributes": {
                                     "key": "process.extensions.x-ocsf-process-ext.xattributes",
-                                    "object": "parent-process"
-                                }
-                            },
-                            "pid": [
-                                {
-                                    "key": "process.pid",
                                     "object": "process"
-                                },
-                                {
-                                    "key": "process.parent_ref",
-                                    "object": "process",
-                                    "references": [
-                                        "parent-process"
-                                    ]
                                 }
-                            ],
-                            "sandbox": {
-                                "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
-                                "object": "process"
-                            },
-                            "terminated_time": {
-                                "key": "process.extensions.x-ocsf-process-ext.terminated_time",
-                                "object": "process"
-                            },
-                            "tid": {
-                                "key": "process.extensions.x-ocsf-process-ext.tid",
-                                "object": "process"
-                            },
-                            "uid": {
-                                "key": "process.x_unique_id",
-                                "object": "process"
                             },
-                            "user": {
-                                "account_type": {
-                                    "key": "user-account.account_type",
-                                    "object": "process-user-account"
+                            "profiles": {
+                                "key": "x-ocsf-cloud.profiles",
+                                "object": "ocsf_cloud_api"
+                            },
+                            "raw_data": {
+                                "key": "x-ocsf-cloud.raw_data",
+                                "object": "ocsf_cloud_api"
+                            },
+                            "ref_event_code": {
+                                "key": "x-ocsf-cloud.ref_event_code",
+                                "object": "ocsf_cloud_api"
+                            },
+                            "ref_event_name": {
+                                "key": "x-ocsf-cloud.ref_event_name",
+                                "object": "ocsf_cloud_api"
+                            },
+                            "ref_event_uid": {
+                                "key": "x-ocsf-cloud.ref_event_uid",
+                                "object": "ocsf_cloud_api"
+                            },
+                            "ref_time": {
+                                "key": "x-ocsf-cloud.ref_time",
+                                "object": "ocsf_cloud_api"
+                            },
+                            "resources": {
+                                "account_uid": [
+                                    {
+                                        "key": "x-ocsf-resources.account_uid",
+                                        "object": "resources"
+                                    },
+                                    {
+                                        "key": "x-ocsf-resources.cloud_api_ref",
+                                        "object": "resources",
+                                        "references": "ocsf_cloud_api"
+                                    }
+                                ],
+                                "cloud_partition": {
+                                    "key": "x-ocsf-resources.cloud_partition",
+                                    "object": "resources"
                                 },
-                                "account_type_id": {
-                                    "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                    "object": "process-user-account"
+                                "criticality": {
+                                    "key": "x-ocsf-resources.criticality",
+                                    "object": "resources"
                                 },
-                                "account_uid": {
-                                    "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                    "object": "process-user-account"
+                                "details": {
+                                    "key": "x-ocsf-resources.details",
+                                    "object": "resources"
                                 },
-                                "credential_uid": {
-                                    "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                    "object": "process-user-account"
-                                },
-                                "domain": {
-                                    "key": "user-account.extensions.x-accessor-ext.domain",
-                                    "object": "process-user-account"
-                                },
-                                "email_addr": {
-                                    "key": "email-addr.value",
-                                    "object": "process-email-addr"
+                                "group_name": {
+                                    "key": "x-ocsf-resources.group_name",
+                                    "object": "resources"
                                 },
-                                "groups": {
-                                    "desc": {
-                                        "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                        "object": "process-user-account"
-                                    },
-                                    "name": {
-                                        "key": "user-account.extensions.x-accessor-ext.group_name",
-                                        "object": "process-user-account"
-                                    },
-                                    "privileges": {
-                                        "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                        "object": "process-user-account"
-                                    },
-                                    "type": {
-                                        "key": "user-account.extensions.x-accessor-ext.group_type",
-                                        "object": "process-user-account"
-                                    },
-                                    "uid": {
-                                        "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                        "object": "process-user-account"
-                                    }
+                                "labels": {
+                                    "key": "x-ocsf-resources.labels",
+                                    "object": "resources"
                                 },
                                 "name": {
-                                    "key": "user-account.display_name",
-                                    "object": "process-user-account"
+                                    "key": "x-ocsf-resources.name",
+                                    "object": "resources"
                                 },
-                                "org_uid": {
-                                    "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                    "object": "process-user-account"
+                                "owner": {
+                                    "key": "x-ocsf-resources.owner",
+                                    "object": "resources"
                                 },
-                                "session_uid": {
-                                    "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                    "object": "process-user-account"
-                                },
-                                "session_uuid": {
-                                    "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                    "object": "process-user-account"
+                                "region": {
+                                    "key": "x-ocsf-resources.region",
+                                    "object": "resources"
                                 },
                                 "type": {
-                                    "key": "user-account.extensions.x-accessor-ext.type",
-                                    "object": "process-user-account"
+                                    "key": "x-ocsf-resources.type",
+                                    "object": "resources"
                                 },
-                                "type_id": {
-                                    "key": "user-account.extensions.x-accessor-ext.type_id",
-                                    "object": "process-user-account"
+                                "uid": {
+                                    "key": "x-ocsf-resources.uid",
+                                    "object": "resources"
+                                }
+                            },
+                            "severity": {
+                                "key": "x-ocsf-cloud.severity",
+                                "object": "ocsf_cloud_api"
+                            },
+                            "severity_id": {
+                                "key": "x-ibm-finding.severity",
+                                "object": "ibm_finding",
+                                "transformer": "ToInteger"
+                            },
+                            "src_endpoint": {
+                                "instance_uid": {
+                                    "key": "x-oca-asset.extensions.x-src-endpoint.instance_uid",
+                                    "object": "asset"
+                                },
+                                "interface_uid": {
+                                    "key": "x-oca-asset.extensions.x-src-endpoint.interface_uid",
+                                    "object": "asset"
                                 },
-                                "uid": [
+                                "intermediate_ips": [
                                     {
-                                        "key": "user-account.user_id",
-                                        "object": "process-user-account"
+                                        "key": "ipv4-addr.value",
+                                        "object": "src_ipv4",
+                                        "transformer": "FilterIPv4List",
+                                        "unwrap": true
                                     },
                                     {
-                                        "key": "user-account.creator_user_ref",
-                                        "object": "process",
-                                        "references": "process-user-account"
+                                        "key": "ipv6-addr.value",
+                                        "object": "src_ipv6",
+                                        "transformer": "FilterIPv6List",
+                                        "unwrap": true
+                                    },
+                                    {
+                                        "key": "x-oca-asset.ip_refs",
+                                        "object": "asset",
+                                        "references": [
+                                            "src_ipv4",
+                                            "src_ipv6"
+                                        ],
+                                        "unwrap": true
                                     }
                                 ],
-                                "uuid": {
-                                    "key": "user-account.extensions.x-accessor-ext.uuid",
-                                    "object": "process-user-account"
-                                }
-                            },
-                            "xattributes": {
-                                "key": "process.extensions.x-ocsf-process-ext.xattributes",
-                                "object": "process"
-                            }
-                        },
-                        "profiles": {
-                            "key": "x-ocsf-cloud.profiles",
-                            "object": "ocsf_cloud_api"
-                        },
-                        "raw_data": {
-                            "key": "x-ocsf-cloud.raw_data",
-                            "object": "ocsf_cloud_api"
-                        },
-                        "ref_event_code": {
-                            "key": "x-ocsf-cloud.ref_event_code",
-                            "object": "ocsf_cloud_api"
-                        },
-                        "ref_event_name": {
-                            "key": "x-ocsf-cloud.ref_event_name",
-                            "object": "ocsf_cloud_api"
-                        },
-                        "ref_event_uid": {
-                            "key": "x-ocsf-cloud.ref_event_uid",
-                            "object": "ocsf_cloud_api"
-                        },
-                        "ref_time": {
-                            "key": "x-ocsf-cloud.ref_time",
-                            "object": "ocsf_cloud_api"
-                        },
-                        "resources": {
-                            "account_uid": [
-                                {
-                                    "key": "x-ocsf-resources.account_uid",
-                                    "object": "resources"
+                                "ip": [
+                                    {
+                                        "key": "ipv4-addr.value",
+                                        "object": "src_ip",
+                                        "transformer": "CheckIPv4"
+                                    },
+                                    {
+                                        "key": "ipv6-addr.value",
+                                        "object": "src_ip",
+                                        "transformer": "CheckIPv6"
+                                    },
+                                    {
+                                        "key": "network-traffic.src_ref",
+                                        "object": "nt",
+                                        "references": "src_ip"
+                                    },
+                                    {
+                                        "key": "x-ibm-finding.src_ip_ref",
+                                        "object": "ibm_finding",
+                                        "references": "src_ip"
+                                    },
+                                    {
+                                        "group": true,
+                                        "key": "x-oca-asset.ip_refs",
+                                        "object": "host",
+                                        "references": [
+                                            "src_ip"
+                                        ]
+                                    },
+                                    {
+                                        "key": "x-oca-event.network_ref",
+                                        "object": "event",
+                                        "references": "nt"
+                                    }
+                                ],
+                                "name": {
+                                    "key": "x-oca-asset.name",
+                                    "object": "asset"
                                 },
-                                {
-                                    "key": "x-ocsf-resources.cloud_api_ref",
-                                    "object": "resources",
-                                    "references": "ocsf_cloud_api"
+                                "port": {
+                                    "key": "network-traffic.src_port",
+                                    "object": "nt",
+                                    "transformer": "ToInteger"
+                                },
+                                "subnet_uid": {
+                                    "key": "x-oca-asset.extensions.x-src-endpoint.subnet_uid",
+                                    "object": "asset"
+                                },
+                                "svc_name": {
+                                    "key": "x-oca-asset.extensions.x-src-endpoint.svc_name",
+                                    "object": "asset"
+                                },
+                                "vpc_uid": {
+                                    "key": "x-oca-asset.extensions.x-src-endpoint.vpc_uid",
+                                    "object": "asset"
                                 }
-                            ],
-                            "cloud_partition": {
-                                "key": "x-ocsf-resources.cloud_partition",
-                                "object": "resources"
-                            },
-                            "criticality": {
-                                "key": "x-ocsf-resources.criticality",
-                                "object": "resources"
-                            },
-                            "details": {
-                                "key": "x-ocsf-resources.details",
-                                "object": "resources"
-                            },
-                            "group_name": {
-                                "key": "x-ocsf-resources.group_name",
-                                "object": "resources"
-                            },
-                            "labels": {
-                                "key": "x-ocsf-resources.labels",
-                                "object": "resources"
                             },
-                            "name": {
-                                "key": "x-ocsf-resources.name",
-                                "object": "resources"
+                            "start_time": {
+                                "cybox": false,
+                                "key": "first_observed",
+                                "transformer": "EpochToTimestamp"
                             },
-                            "owner": {
-                                "key": "x-ocsf-resources.owner",
-                                "object": "resources"
+                            "status": {
+                                "key": "x-ocsf-cloud.status",
+                                "object": "ocsf_cloud_api"
                             },
-                            "region": {
-                                "key": "x-ocsf-resources.region",
-                                "object": "resources"
+                            "status_code": {
+                                "key": "x-ocsf-cloud.status_code",
+                                "object": "ocsf_cloud_api"
                             },
-                            "type": {
-                                "key": "x-ocsf-resources.type",
-                                "object": "resources"
+                            "status_detail": {
+                                "key": "x-ocsf-cloud.status_detail",
+                                "object": "ocsf_cloud_api"
                             },
-                            "uid": {
-                                "key": "x-ocsf-resources.uid",
-                                "object": "resources"
-                            }
-                        },
-                        "severity": {
-                            "key": "x-ocsf-cloud.severity",
-                            "object": "ocsf_cloud_api"
-                        },
-                        "severity_id": {
-                            "key": "x-ibm-finding.severity",
-                            "object": "ibm_finding",
-                            "transformer": "ToInteger"
-                        },
-                        "src_endpoint": {
-                            "instance_uid": {
-                                "key": "x-oca-asset.extensions.x-src-endpoint.instance_uid",
-                                "object": "asset"
-                            },
-                            "interface_uid": {
-                                "key": "x-oca-asset.extensions.x-src-endpoint.interface_uid",
-                                "object": "asset"
+                            "status_id": {
+                                "key": "x-ocsf-cloud.status_id",
+                                "object": "ocsf_cloud_api",
+                                "transformer": "ToInteger"
                             },
-                            "intermediate_ips": [
-                                {
-                                    "key": "ipv4-addr.value",
-                                    "object": "src_ipv4",
-                                    "transformer": "FilterIPv4List",
-                                    "unwrap": true
-                                },
-                                {
-                                    "key": "ipv6-addr.value",
-                                    "object": "src_ipv6",
-                                    "transformer": "FilterIPv6List",
-                                    "unwrap": true
-                                },
-                                {
-                                    "key": "x-oca-asset.ip_refs",
-                                    "object": "asset",
-                                    "references": [
-                                        "src_ipv4",
-                                        "src_ipv6"
-                                    ],
-                                    "unwrap": true
-                                }
-                            ],
-                            "ip": [
-                                {
-                                    "key": "ipv4-addr.value",
-                                    "object": "src_ip",
-                                    "transformer": "CheckIPv4"
-                                },
-                                {
-                                    "key": "ipv6-addr.value",
-                                    "object": "src_ip",
-                                    "transformer": "CheckIPv6"
-                                },
-                                {
-                                    "key": "network-traffic.src_ref",
-                                    "object": "nt",
-                                    "references": "src_ip"
-                                },
-                                {
-                                    "key": "x-ibm-finding.src_ip_ref",
-                                    "object": "ibm_finding",
-                                    "references": "src_ip"
-                                },
-                                {
-                                    "group": true,
-                                    "key": "x-oca-asset.ip_refs",
-                                    "object": "host",
-                                    "references": [
-                                        "src_ip"
-                                    ]
-                                },
-                                {
-                                    "key": "x-oca-event.network_ref",
-                                    "object": "event",
-                                    "references": "nt"
+                            "time": {
+                                "key": "x-oca-event.created",
+                                "object": "x_oca_event"
+                            },
+                            "timezone_offset": {
+                                "key": "x-oca-event.timezone",
+                                "object": "x_oca_event",
+                                "transformer": "ToInteger"
+                            },
+                            "traffic": {
+                                "bytes": {
+                                    "key": "network-traffic.extensions.x-network-ext.bytes",
+                                    "object": "nt"
+                                },
+                                "bytes_in": {
+                                    "key": "network-traffic.dst_byte_count",
+                                    "object": "nt"
+                                },
+                                "bytes_out": {
+                                    "key": "network-traffic.src_byte_count",
+                                    "object": "nt"
+                                },
+                                "packets": {
+                                    "key": "network-traffic.extensions.x-network-ext.packets",
+                                    "object": "nt"
+                                },
+                                "packets_in": {
+                                    "key": "network-traffic.dst_packets",
+                                    "object": "nt"
+                                },
+                                "packets_out": {
+                                    "key": "network-traffic.src_packets",
+                                    "object": "nt"
                                 }
-                            ],
-                            "name": {
-                                "key": "x-oca-asset.name",
-                                "object": "asset"
                             },
-                            "port": {
-                                "key": "network-traffic.src_port",
-                                "object": "nt",
+                            "type_name": {
+                                "key": "x-ocsf-cloud.type_name",
+                                "object": "ocsf_cloud_api"
+                            },
+                            "type_uid": {
+                                "key": "x-ocsf-cloud.type_uid",
+                                "object": "ocsf_cloud_api",
                                 "transformer": "ToInteger"
                             },
-                            "subnet_uid": {
-                                "key": "x-oca-asset.extensions.x-src-endpoint.subnet_uid",
-                                "object": "asset"
-                            },
-                            "svc_name": {
-                                "key": "x-oca-asset.extensions.x-src-endpoint.svc_name",
-                                "object": "asset"
-                            },
-                            "vpc_uid": {
-                                "key": "x-oca-asset.extensions.x-src-endpoint.vpc_uid",
-                                "object": "asset"
-                            }
-                        },
-                        "start_time": {
-                            "cybox": false,
-                            "key": "first_observed",
-                            "transformer": "EpochToTimestamp"
-                        },
-                        "status": {
-                            "key": "x-ocsf-cloud.status",
-                            "object": "ocsf_cloud_api"
-                        },
-                        "status_code": {
-                            "key": "x-ocsf-cloud.status_code",
-                            "object": "ocsf_cloud_api"
-                        },
-                        "status_detail": {
-                            "key": "x-ocsf-cloud.status_detail",
-                            "object": "ocsf_cloud_api"
-                        },
-                        "status_id": {
-                            "key": "x-ocsf-cloud.status_id",
-                            "object": "ocsf_cloud_api",
-                            "transformer": "ToInteger"
-                        },
-                        "time": {
-                            "key": "x-oca-event.created",
-                            "object": "x_oca_event"
-                        },
-                        "timezone_offset": {
-                            "key": "x-oca-event.timezone",
-                            "object": "x_oca_event",
-                            "transformer": "ToInteger"
-                        },
-                        "traffic": {
-                            "bytes": {
-                                "key": "network-traffic.extensions.x-network-ext.bytes",
-                                "object": "nt"
-                            },
-                            "bytes_in": {
-                                "key": "network-traffic.dst_byte_count",
-                                "object": "nt"
-                            },
-                            "bytes_out": {
-                                "key": "network-traffic.src_byte_count",
-                                "object": "nt"
-                            },
-                            "packets": {
-                                "key": "network-traffic.extensions.x-network-ext.packets",
-                                "object": "nt"
-                            },
-                            "packets_in": {
-                                "key": "network-traffic.dst_packets",
-                                "object": "nt"
-                            },
-                            "packets_out": {
-                                "key": "network-traffic.src_packets",
-                                "object": "nt"
-                            }
-                        },
-                        "type_name": {
-                            "key": "x-ocsf-cloud.type_name",
-                            "object": "ocsf_cloud_api"
-                        },
-                        "type_uid": {
-                            "key": "x-ocsf-cloud.type_uid",
-                            "object": "ocsf_cloud_api",
-                            "transformer": "ToInteger"
-                        },
-                        "vulnerabilities": {
-                            "cve": {
-                                "created_time": {
-                                    "key": "x-ocsf-vulnerabilities.created_time",
-                                    "object": "vulnerabilities"
-                                },
-                                "cvss": {
-                                    "base_score": {
-                                        "key": "x-ocsf-vulnerabilities.base_score",
-                                        "object": "vulnerabilities"
-                                    },
-                                    "depth": {
-                                        "key": "x-ocsf-vulnerabilities.depth",
+                            "vulnerabilities": {
+                                "cve": {
+                                    "created_time": {
+                                        "key": "x-ocsf-vulnerabilities.created_time",
                                         "object": "vulnerabilities"
                                     },
-                                    "metrics": {
-                                        "name": {
-                                            "key": "x-ocsf-vulnerabilities.name",
+                                    "cvss": {
+                                        "base_score": {
+                                            "key": "x-ocsf-vulnerabilities.base_score",
                                             "object": "vulnerabilities"
                                         },
-                                        "value": {
-                                            "key": "x-ocsf-vulnerabilities.value",
+                                        "depth": {
+                                            "key": "x-ocsf-vulnerabilities.depth",
+                                            "object": "vulnerabilities"
+                                        },
+                                        "metrics": {
+                                            "name": {
+                                                "key": "x-ocsf-vulnerabilities.name",
+                                                "object": "vulnerabilities"
+                                            },
+                                            "value": {
+                                                "key": "x-ocsf-vulnerabilities.value",
+                                                "object": "vulnerabilities"
+                                            }
+                                        },
+                                        "overall_score": {
+                                            "key": "x-ocsf-vulnerabilities.overall_score",
+                                            "object": "vulnerabilities"
+                                        },
+                                        "severity": {
+                                            "key": "x-ocsf-vulnerabilities.severity",
+                                            "object": "vulnerabilities"
+                                        },
+                                        "vector_string": {
+                                            "key": "x-ocsf-vulnerabilities.vector_string",
+                                            "object": "vulnerabilities"
+                                        },
+                                        "version": {
+                                            "key": "x-ocsf-vulnerabilities.version",
                                             "object": "vulnerabilities"
                                         }
                                     },
-                                    "overall_score": {
-                                        "key": "x-ocsf-vulnerabilities.overall_score",
+                                    "cwe_uid": {
+                                        "key": "x-ocsf-vulnerabilities.cwe_uid",
                                         "object": "vulnerabilities"
                                     },
-                                    "severity": {
-                                        "key": "x-ocsf-vulnerabilities.severity",
+                                    "cwe_url": {
+                                        "key": "x-ocsf-vulnerabilities.cwe_url",
                                         "object": "vulnerabilities"
                                     },
-                                    "vector_string": {
-                                        "key": "x-ocsf-vulnerabilities.vector_string",
+                                    "modified_time": {
+                                        "key": "x-ocsf-vulnerabilities.modified_time",
                                         "object": "vulnerabilities"
                                     },
-                                    "version": {
-                                        "key": "x-ocsf-vulnerabilities.version",
-                                        "object": "vulnerabilities"
-                                    }
-                                },
-                                "cwe_uid": {
-                                    "key": "x-ocsf-vulnerabilities.cwe_uid",
-                                    "object": "vulnerabilities"
-                                },
-                                "cwe_url": {
-                                    "key": "x-ocsf-vulnerabilities.cwe_url",
-                                    "object": "vulnerabilities"
-                                },
-                                "modified_time": {
-                                    "key": "x-ocsf-vulnerabilities.modified_time",
-                                    "object": "vulnerabilities"
-                                },
-                                "product": {
-                                    "feature": {
+                                    "product": {
+                                        "feature": {
+                                            "name": {
+                                                "key": "software.extensions.x-ocsf-product-ext.feature_name",
+                                                "object": "vulnerabilities-software"
+                                            },
+                                            "uid": {
+                                                "key": "software.extensions.x-ocsf-product-ext.feature_uid",
+                                                "object": "vulnerabilities-software"
+                                            },
+                                            "version": {
+                                                "key": "software.extensions.x-ocsf-product-ext.feature_version",
+                                                "object": "vulnerabilities-software"
+                                            }
+                                        },
+                                        "lang": {
+                                            "key": "software.languages",
+                                            "object": "vulnerabilities-software"
+                                        },
                                         "name": {
-                                            "key": "software.extensions.x-ocsf-product-ext.feature_name",
+                                            "key": "software.name",
+                                            "object": "vulnerabilities-software"
+                                        },
+                                        "path": {
+                                            "key": "software.extensions.x-ocsf-product-ext.installed_path",
                                             "object": "vulnerabilities-software"
                                         },
                                         "uid": {
-                                            "key": "software.extensions.x-ocsf-product-ext.feature_uid",
+                                            "key": "software.extensions.x-ocsf-product-ext.product_uid",
+                                            "object": "vulnerabilities-software"
+                                        },
+                                        "vendor_name": {
+                                            "key": "software.vendor",
                                             "object": "vulnerabilities-software"
                                         },
                                         "version": {
-                                            "key": "software.extensions.x-ocsf-product-ext.feature_version",
+                                            "key": "software.version",
                                             "object": "vulnerabilities-software"
                                         }
                                     },
-                                    "lang": {
-                                        "key": "software.languages",
-                                        "object": "vulnerabilities-software"
+                                    "type": {
+                                        "key": "x-ocsf-vulnerabilities.type",
+                                        "object": "vulnerabilities"
                                     },
-                                    "name": {
-                                        "key": "software.name",
-                                        "object": "vulnerabilities-software"
+                                    "uid": {
+                                        "key": "x-ocsf-vulnerabilities.uid",
+                                        "object": "vulnerabilities"
+                                    }
+                                },
+                                "desc": {
+                                    "key": "x-ocsf-vulnerabilities.desc",
+                                    "object": "vulnerabilities"
+                                },
+                                "kb_articles": {
+                                    "key": "x-ocsf-vulnerabilities.kb_articles",
+                                    "object": "vulnerabilities"
+                                },
+                                "packages": {
+                                    "architecture": {
+                                        "key": "x-ocsf-vulnerabilities.packages_architecture",
+                                        "object": "vulnerabilities"
                                     },
-                                    "path": {
-                                        "key": "software.extensions.x-ocsf-product-ext.installed_path",
-                                        "object": "vulnerabilities-software"
+                                    "epoch": {
+                                        "key": "x-ocsf-vulnerabilities.packages_epoch",
+                                        "object": "vulnerabilities"
                                     },
-                                    "uid": {
-                                        "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                                        "object": "vulnerabilities-software"
+                                    "license": {
+                                        "key": "x-ocsf-vulnerabilities.packages_license",
+                                        "object": "vulnerabilities"
                                     },
-                                    "vendor_name": {
-                                        "key": "software.vendor",
-                                        "object": "vulnerabilities-software"
+                                    "name": {
+                                        "key": "x-ocsf-vulnerabilities.packages_name",
+                                        "object": "vulnerabilities"
+                                    },
+                                    "release": {
+                                        "key": "x-ocsf-vulnerabilities.packages_release",
+                                        "object": "vulnerabilities"
                                     },
                                     "version": {
-                                        "key": "software.version",
-                                        "object": "vulnerabilities-software"
+                                        "key": "x-ocsf-vulnerabilities.packages_version",
+                                        "object": "vulnerabilities"
                                     }
                                 },
-                                "type": {
-                                    "key": "x-ocsf-vulnerabilities.type",
+                                "references": {
+                                    "key": "x-ocsf-vulnerabilities.references",
                                     "object": "vulnerabilities"
                                 },
-                                "uid": {
-                                    "key": "x-ocsf-vulnerabilities.uid",
-                                    "object": "vulnerabilities"
-                                }
-                            },
-                            "desc": {
-                                "key": "x-ocsf-vulnerabilities.desc",
-                                "object": "vulnerabilities"
-                            },
-                            "kb_articles": {
-                                "key": "x-ocsf-vulnerabilities.kb_articles",
-                                "object": "vulnerabilities"
-                            },
-                            "packages": {
-                                "architecture": {
-                                    "key": "x-ocsf-vulnerabilities.packages_architecture",
+                                "related_vulnerabilities": {
+                                    "key": "x-ocsf-vulnerabilities.related_vulnerabilities",
                                     "object": "vulnerabilities"
                                 },
-                                "epoch": {
-                                    "key": "x-ocsf-vulnerabilities.packages_epoch",
+                                "severity": {
+                                    "key": "x-ocsf-vulnerabilities.severity",
                                     "object": "vulnerabilities"
                                 },
-                                "license": {
-                                    "key": "x-ocsf-vulnerabilities.packages_license",
+                                "title": {
+                                    "key": "x-ocsf-vulnerabilities.title",
                                     "object": "vulnerabilities"
                                 },
-                                "name": {
-                                    "key": "x-ocsf-vulnerabilities.packages_name",
+                                "vendor_name": {
+                                    "key": "x-ocsf-vulnerabilities.vendor_name",
                                     "object": "vulnerabilities"
+                                }
+                            }
+                        },
+                        "vpcflow": {
+                            "account": [
+                                {
+                                    "key": "x-aws-details.account_id",
+                                    "object": "accountid"
+                                }
+                            ],
+                            "action": {
+                                "key": "x-ibm-finding.finding_type",
+                                "object": "ibm_finding"
+                            },
+                            "destinationaddress": [
+                                {
+                                    "key": "ipv4-addr.value",
+                                    "object": "dst_ip"
                                 },
-                                "release": {
-                                    "key": "x-ocsf-vulnerabilities.packages_release",
-                                    "object": "vulnerabilities"
+                                {
+                                    "key": "ipv6-addr.value",
+                                    "object": "dst_ip"
                                 },
-                                "version": {
-                                    "key": "x-ocsf-vulnerabilities.packages_version",
-                                    "object": "vulnerabilities"
+                                {
+                                    "key": "x-ibm-finding.dst_ip_ref",
+                                    "object": "ibm_finding",
+                                    "references": "dst_ip"
+                                },
+                                {
+                                    "key": "network-traffic.dst_ref",
+                                    "object": "nt",
+                                    "references": "dst_ip"
                                 }
+                            ],
+                            "destinationport": [
+                                {
+                                    "key": "network-traffic.dst_port",
+                                    "object": "nt",
+                                    "transformer": "ToInteger"
+                                }
+                            ],
+                            "endtime": [
+                                {
+                                    "key": "network-traffic.end",
+                                    "object": "nt",
+                                    "transformer": "EpochSecondsToTimestamp"
+                                },
+                                {
+                                    "key": "x-ibm-finding.end",
+                                    "object": "ibm_finding",
+                                    "transformer": "EpochSecondsToTimestamp"
+                                },
+                                {
+                                    "cybox": false,
+                                    "key": "last_observed",
+                                    "transformer": "EpochToTimestamp"
+                                }
+                            ],
+                            "name": {
+                                "key": "x-ibm-finding.name",
+                                "object": "ibm_finding"
                             },
-                            "references": {
-                                "key": "x-ocsf-vulnerabilities.references",
-                                "object": "vulnerabilities"
-                            },
-                            "related_vulnerabilities": {
-                                "key": "x-ocsf-vulnerabilities.related_vulnerabilities",
-                                "object": "vulnerabilities"
-                            },
-                            "severity": {
-                                "key": "x-ocsf-vulnerabilities.severity",
-                                "object": "vulnerabilities"
-                            },
-                            "title": {
-                                "key": "x-ocsf-vulnerabilities.title",
-                                "object": "vulnerabilities"
-                            },
-                            "vendor_name": {
-                                "key": "x-ocsf-vulnerabilities.vendor_name",
-                                "object": "vulnerabilities"
-                            }
+                            "protocol": [
+                                {
+                                    "key": "network-traffic.protocols",
+                                    "object": "nt",
+                                    "transformer": "ToLowercaseArray"
+                                }
+                            ],
+                            "sourceaddress": [
+                                {
+                                    "key": "ipv4-addr.value",
+                                    "object": "src_ip"
+                                },
+                                {
+                                    "key": "ipv6-addr.value",
+                                    "object": "src_ip"
+                                },
+                                {
+                                    "key": "network-traffic.src_ref",
+                                    "object": "nt",
+                                    "references": "src_ip"
+                                },
+                                {
+                                    "key": "x-ibm-finding.src_ip_ref",
+                                    "object": "ibm_finding",
+                                    "references": "src_ip"
+                                },
+                                {
+                                    "cybox": false,
+                                    "ds_key": "interfaceid",
+                                    "key": "ipv4-addr.x_aws_interface_id",
+                                    "object": "src_ip"
+                                },
+                                {
+                                    "cybox": false,
+                                    "ds_key": "interfaceid",
+                                    "key": "ipv6-addr.x_aws_interface_id",
+                                    "object": "src_ip"
+                                }
+                            ],
+                            "sourceport": [
+                                {
+                                    "key": "network-traffic.src_port",
+                                    "object": "nt",
+                                    "transformer": "ToInteger"
+                                }
+                            ],
+                            "starttime": [
+                                {
+                                    "key": "network-traffic.start",
+                                    "object": "nt",
+                                    "transformer": "EpochSecondsToTimestamp"
+                                },
+                                {
+                                    "key": "x-ibm-finding.start",
+                                    "object": "ibm_finding",
+                                    "transformer": "EpochSecondsToTimestamp"
+                                },
+                                {
+                                    "cybox": false,
+                                    "key": "first_observed",
+                                    "transformer": "EpochSecondsToTimestamp"
+                                }
+                            ]
                         }
                     },
-                    "operators": {
-                        "ComparisonComparators.Equal": "=",
-                        "ComparisonComparators.GreaterThan": ">",
-                        "ComparisonComparators.GreaterThanOrEqual": ">=",
-                        "ComparisonComparators.In": "IN",
-                        "ComparisonComparators.LessThan": "<",
-                        "ComparisonComparators.LessThanOrEqual": "<=",
-                        "ComparisonComparators.Like": "LIKE",
-                        "ComparisonComparators.Matches": "REGEXP_LIKE",
-                        "ComparisonComparators.NotEqual": "!=",
-                        "ComparisonExpressionOperators.And": "AND",
-                        "ComparisonExpressionOperators.Or": "OR",
-                        "ObservationOperators.And": "INTERSECT",
-                        "ObservationOperators.Or": "UNION"
-                    },
                     "vpcflow_from_stix_map": {
                         "ipv4-addr": {
                             "fields": {
                                 "value": [
                                     "sourceaddress",
                                     "destinationaddress"
                                 ],
@@ -4390,146 +4515,23 @@
                                     "sourceaddress"
                                 ],
                                 "start": [
                                     "starttime"
                                 ]
                             }
                         }
-                    },
-                    "vpcflow_to_stix_map": {
-                        "account": [
-                            {
-                                "key": "x-aws-details.account_id",
-                                "object": "accountid"
-                            }
-                        ],
-                        "action": {
-                            "key": "x-ibm-finding.finding_type",
-                            "object": "ibm_finding"
-                        },
-                        "destinationaddress": [
-                            {
-                                "key": "ipv4-addr.value",
-                                "object": "dst_ip"
-                            },
-                            {
-                                "key": "ipv6-addr.value",
-                                "object": "dst_ip"
-                            },
-                            {
-                                "key": "x-ibm-finding.dst_ip_ref",
-                                "object": "ibm_finding",
-                                "references": "dst_ip"
-                            },
-                            {
-                                "key": "network-traffic.dst_ref",
-                                "object": "nt",
-                                "references": "dst_ip"
-                            }
-                        ],
-                        "destinationport": [
-                            {
-                                "key": "network-traffic.dst_port",
-                                "object": "nt",
-                                "transformer": "ToInteger"
-                            }
-                        ],
-                        "endtime": [
-                            {
-                                "key": "network-traffic.end",
-                                "object": "nt",
-                                "transformer": "EpochSecondsToTimestamp"
-                            },
-                            {
-                                "key": "x-ibm-finding.end",
-                                "object": "ibm_finding",
-                                "transformer": "EpochSecondsToTimestamp"
-                            },
-                            {
-                                "cybox": false,
-                                "key": "last_observed",
-                                "transformer": "EpochToTimestamp"
-                            }
-                        ],
-                        "name": {
-                            "key": "x-ibm-finding.name",
-                            "object": "ibm_finding"
-                        },
-                        "protocol": [
-                            {
-                                "key": "network-traffic.protocols",
-                                "object": "nt",
-                                "transformer": "ToLowercaseArray"
-                            }
-                        ],
-                        "sourceaddress": [
-                            {
-                                "key": "ipv4-addr.value",
-                                "object": "src_ip"
-                            },
-                            {
-                                "key": "ipv6-addr.value",
-                                "object": "src_ip"
-                            },
-                            {
-                                "key": "network-traffic.src_ref",
-                                "object": "nt",
-                                "references": "src_ip"
-                            },
-                            {
-                                "key": "x-ibm-finding.src_ip_ref",
-                                "object": "ibm_finding",
-                                "references": "src_ip"
-                            },
-                            {
-                                "cybox": false,
-                                "ds_key": "interfaceid",
-                                "key": "ipv4-addr.x_aws_interface_id",
-                                "object": "src_ip"
-                            },
-                            {
-                                "cybox": false,
-                                "ds_key": "interfaceid",
-                                "key": "ipv6-addr.x_aws_interface_id",
-                                "object": "src_ip"
-                            }
-                        ],
-                        "sourceport": [
-                            {
-                                "key": "network-traffic.src_port",
-                                "object": "nt",
-                                "transformer": "ToInteger"
-                            }
-                        ],
-                        "starttime": [
-                            {
-                                "key": "network-traffic.start",
-                                "object": "nt",
-                                "transformer": "EpochSecondsToTimestamp"
-                            },
-                            {
-                                "key": "x-ibm-finding.start",
-                                "object": "ibm_finding",
-                                "transformer": "EpochSecondsToTimestamp"
-                            },
-                            {
-                                "cybox": false,
-                                "key": "first_observed",
-                                "transformer": "EpochSecondsToTimestamp"
-                            }
-                        ]
                     }
                 },
                 "optional": true,
                 "previous": "connection.mapping",
                 "type": "json"
             },
             "result_limit": {
                 "default": 10000,
-                "max": 500000,
+                "max": 10000000,
                 "min": 1,
                 "previous": "connection.resultSizeLimit",
                 "type": "number"
             },
             "stix_2.1": {
                 "default": false,
                 "hidden": true,
@@ -4550,15 +4552,15 @@
                 "nullable": true,
                 "previous": "connection.timerange",
                 "type": "number"
             },
             "timeout": {
                 "default": 30,
                 "hidden": true,
-                "max": 60,
+                "max": 3600,
                 "min": 1,
                 "previous": "connection.timeoutLimit",
                 "type": "number"
             },
             "type": "fields",
             "unmapped_fallback": {
                 "default": false,
```

## stix_shifter_modules/aws_athena/stix_translation/results_translator.py

```diff
@@ -7,16 +7,16 @@
     def __init__(self, options, dialect, base_file_path=None, callback=None):
         super().__init__(options, dialect, base_file_path, callback)
         hash_algorithm_map = os.path.abspath(os.path.join(base_file_path, "json", "hash_algorithm_map.json"))
         self.hash_names = self.read_json(hash_algorithm_map, options)
 
     def translate_results(self, data_source, data):
         for result in data:
-            # ocsf_payload = result['ocsf']
-            process_obj = result.get('process')
+            ocsf_payload = result['ocsf']
+            process_obj = ocsf_payload.get('process')
             if process_obj:
                 file_obj = process_obj.get('file')
                 if file_obj:
                     file_obj['hashes'] = self.update_hash_mapping(file_obj)
             
                 parent_process = process_obj.get('parent_process')
                 if parent_process:
```

## stix_shifter_modules/aws_athena/stix_transmission/results_connector.py

```diff
@@ -193,18 +193,18 @@
         :param flatten_result_cleansed: list, flattened results
         :param service_type: str, service name
         :return: list, formatted result
         """
         formatted_result = []
         transmit_basepath = os.path.abspath(__file__)
         translate_basepath = transmit_basepath.split(os.sep)[:-2]
-        filepath = os.sep.join([*translate_basepath, "stix_translation", "json", service_type + '_to_stix_map.json'])
+        filepath = os.sep.join([*translate_basepath, "stix_translation", "json", 'to_stix_map.json'])
         map_file = open(filepath).read()
         map_data = json.loads(map_file)
-        map_data_keys = list(map_data.keys())
+        map_data_keys = list(map_data[service_type].keys())
         ds_key_values = self.gen_dict_extract(key_to_search='ds_key', var=map_data)
         map_data_keys.extend(ds_key_values)
         flattened_obj = dict()
         obj_to_unflatten = dict()
         singular_obj = dict()
         service_log_dict = dict()
         for obj in flatten_result_cleansed:
```

## Comparing `stix_shifter_modules/aws_athena/stix_translation/json/ocsf_to_stix_map.json` & `stix_shifter_modules/aws_athena/stix_translation/json/to_stix_map.json`

 * *Files 12% similar despite different names*

### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('ocsf', OrderedDict([('_time', [OrderedDict([('key', 'first_observed'), "*

 * *            "('cybox', False), ('transformer', 'EpochToTimestamp')]), OrderedDict([('key', "*

 * *            "'last_observed'), ('cybox', False), ('transformer', 'EpochToTimestamp')]), "*

 * *            "OrderedDict([('key', 'x-ibm-finding.time_observed'), ('object', 'ibm_finding'), "*

 * *            "('transformer', 'EpochToTimestamp')])]), ('activity', OrderedDict([('key', "*

 * *            "'x-oca-event.action'), ('objec […]*

```diff
@@ -1,2606 +1,3136 @@
 {
-    "_time": [
-        {
-            "cybox": false,
-            "key": "first_observed",
-            "transformer": "EpochToTimestamp"
-        },
-        {
-            "cybox": false,
-            "key": "last_observed",
-            "transformer": "EpochToTimestamp"
-        },
-        {
-            "key": "x-ibm-finding.time_observed",
-            "object": "ibm_finding",
-            "transformer": "EpochToTimestamp"
-        }
-    ],
-    "activity": {
-        "key": "x-oca-event.action",
-        "object": "x_oca_event"
-    },
-    "activity_id": {
-        "key": "x-oca-event.code",
-        "object": "x_oca_event",
-        "transformer": "ToInteger"
-    },
-    "activity_name": {
-        "key": "x-oca-event.action",
-        "object": "x_oca_event"
-    },
-    "api": {
-        "operation": {
-            "key": "x-ocsf-cloud.operation",
-            "object": "ocsf_cloud_api"
+    "guardduty": {
+        "accountid": {
+            "key": "x-aws-details.account_id",
+            "object": "aws_details"
         },
-        "request": {
-            "flags": {
-                "key": "x-ocsf-cloud.request_flags",
-                "object": "ocsf_cloud_api",
-                "transformer": "ToLowercaseArray"
-            },
-            "uid": {
-                "key": "x-ocsf-cloud.request_uid",
-                "object": "ocsf_cloud_api"
-            }
+        "description": {
+            "key": "x-ibm-finding.description",
+            "object": "ibm_finding"
         },
-        "response": {
-            "code": {
-                "key": "x-ocsf-cloud.response_code",
-                "object": "ocsf_cloud_api",
-                "transformer": "ToInteger"
+        "dnsrequest_resource_instancedetails_networkinterfaces_0_privateipaddress": [
+            {
+                "key": "ipv4-addr.value",
+                "object": "dns_private_ip1"
             },
-            "error": {
-                "key": "x-ocsf-cloud.response_error",
-                "object": "ocsf_cloud_api"
+            {
+                "key": "domain-name.resolves_to_refs",
+                "object": "private_dns_name",
+                "references": [
+                    "dns_private_ip1"
+                ]
             },
-            "error_message": {
-                "key": "x-ocsf-cloud.response_error_message",
-                "object": "ocsf_cloud_api"
+            {
+                "key": "x-ibm-finding.src_ip_ref",
+                "object": "ibm_finding",
+                "references": "dns_private_ip1"
             },
-            "flags": {
-                "key": "x-ocsf-cloud.response_flags",
-                "object": "ocsf_cloud_api",
-                "transformer": "ToLowercaseArray"
+            {
+                "cybox": false,
+                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
+                "key": "ipv4-addr.x_aws_interface_id",
+                "object": "dns_private_ip1"
             },
-            "message": {
-                "key": "x-ocsf-cloud.response_message",
-                "object": "ocsf_cloud_api"
+            {
+                "cybox": false,
+                "key": "ipv4-addr.x_aws_ip_type",
+                "object": "dns_private_ip1",
+                "value": "private"
             }
-        },
-        "service": {
-            "labels": {
-                "key": "x-ocsf-cloud.service_labels",
-                "object": "ocsf_cloud_api",
-                "transformer": "ToLowercaseArray"
+        ],
+        "portprobe_resource_instancedetails_networkinterfaces_0_privateipaddress": [
+            {
+                "key": "ipv4-addr.value",
+                "object": "pp_private_ip1"
             },
-            "name": {
-                "key": "x-ocsf-cloud.service_name",
-                "object": "ocsf_cloud_api"
+            {
+                "key": "domain-name.resolves_to_refs",
+                "object": "private_dns_name",
+                "references": [
+                    "pp_private_ip1"
+                ]
             },
-            "uid": {
-                "key": "x-ocsf-cloud.service_uid",
-                "object": "ocsf_cloud_api"
+            {
+                "key": "x-ibm-finding.src_ip_ref",
+                "object": "ibm_finding",
+                "references": "pp_private_ip1"
             },
-            "version": {
-                "key": "x-ocsf-cloud.service_uid",
-                "object": "ocsf_cloud_api"
-            }
-        },
-        "version": {
-            "key": "x-ocsf-cloud.api_version",
-            "object": "ocsf_cloud_api"
-        }
-    },
-    "attacks": {
-        "tactics": {
-            "name": {
-                "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.tactic_name",
-                "object": "ttp-tagging"
+            {
+                "cybox": false,
+                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
+                "key": "ipv4-addr.x_aws_interface_id",
+                "object": "pp_private_ip1"
             },
-            "uid": {
-                "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.tactic_id",
-                "object": "ttp-tagging"
-            }
-        },
-        "technique": {
-            "name": [
-                {
-                    "key": "x-ibm-ttp-tagging.name",
-                    "object": "ttp-tagging"
-                },
-                {
-                    "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.technique_name",
-                    "object": "ttp-tagging"
-                },
-                {
-                    "key": "x-ibm-finding.ttp_tagging_refs",
-                    "object": "ibm_finding",
-                    "references": [
-                        "ttp-tagging"
-                    ]
-                }
-            ],
-            "uid": {
-                "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.technique_id",
-                "object": "ttp-tagging"
+            {
+                "cybox": false,
+                "key": "ipv4-addr.x_aws_ip_type",
+                "object": "pp_private_ip1",
+                "value": "private"
             }
-        },
-        "version": {
-            "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.versoin",
-            "object": "ttp-tagging"
-        }
-    },
-    "category_name": {
-        "key": "x-oca-event.category",
-        "object": "x_oca_event"
-    },
-    "category_uid": {
-        "key": "x-oca-event.code",
-        "object": "x_oca_event",
-        "transformer": "ToInteger"
-    },
-    "class_name": {
-        "key": "x-oca-event.module",
-        "object": "x_oca_event"
-    },
-    "class_uid": {
-        "key": "x-oca-event.extensions.x-cloud-api.class_uid",
-        "object": "x_oca_event",
-        "transformer": "ToInteger"
-    },
-    "cloud": {
-        "account_type": {
-            "key": "x-ocsf-cloud.account_type",
-            "object": "ocsf_cloud_api"
-        },
-        "account_type_id": {
-            "key": "x-ocsf-cloud.account_type_id",
-            "object": "ocsf_cloud_api",
-            "transformer": "ToInteger"
-        },
-        "account_uid": {
-            "key": "x-ocsf-cloud.account_uid",
-            "object": "ocsf_cloud_api"
-        },
-        "org_uid": {
-            "key": "x-ocsf-cloud.org_uid",
-            "object": "ocsf_cloud_api"
-        },
-        "project_uid": {
-            "key": "x-ocsf-cloud.project_uid",
-            "object": "ocsf_cloud_api"
-        },
-        "provider": {
-            "key": "x-ocsf-cloud.provider",
-            "object": "ocsf_cloud_api"
-        },
+        ],
         "region": {
-            "key": "x-ocsf-cloud.region",
-            "object": "ocsf_cloud_api"
-        },
-        "resource_uid": {
-            "key": "x-ocsf-cloud.resource_uid",
-            "object": "ocsf_cloud_api"
+            "key": "x-aws-details.region",
+            "object": "aws_details"
         },
-        "zone": {
-            "key": "x-ocsf-cloud.zone",
-            "object": "ocsf_cloud_api"
-        }
-    },
-    "compliance": {
-        "requirements": {
-            "key": "x-ocsf-compliance.requirements",
-            "object": "compliance"
-        },
-        "status": {
-            "key": "x-ocsf-compliance.status",
-            "object": "compliance"
-        },
-        "status_detail": {
-            "key": "x-ocsf-compliance.status_detail",
-            "object": "compliance"
-        }
-    },
-    "confidence": {
-        "key": "x-oca-event.confidence",
-        "object": "x-oca-event"
-    },
-    "connection_info": {
-        "boundary": {
-            "key": "network-traffic.extensions.x-network-ext.boundary",
-            "object": "nt"
-        },
-        "boundary_id": {
-            "key": "network-traffic.extensions.x-network-ext.boundary_id",
-            "object": "nt"
-        },
-        "direction": {
-            "key": "network-traffic.extensions.x-network-ext.direction",
-            "object": "nt"
-        },
-        "direction_id": {
-            "key": "network-traffic.extensions.x-network-ext.direction_id",
-            "object": "nt"
-        },
-        "protocol_name": {
-            "key": "network-traffic.extensions.x-network-ext.protocol_name",
-            "object": "nt"
-        },
-        "protocol_num": {
-            "group": true,
-            "key": "network-traffic.protocols",
-            "object": "nt",
-            "transformer": "ProtocolNumToName"
-        },
-        "protocol_ver": {
-            "group": true,
-            "key": "network-traffic.protocols",
-            "object": "nt",
-            "transformer": "ToLowercaseArray"
-        },
-        "protocol_ver_id": {
-            "key": "network-traffic.extensions.x-network-ext.protocol_ver_id",
-            "object": "nt"
-        },
-        "tcp_flags": {
-            "key": "network-traffic.extensions.tcp-ext.src_flags_hex",
-            "object": "nt"
-        }
-    },
-    "count": [
-        {
-            "cybox": false,
-            "key": "number_observed",
-            "transformer": "ToInteger"
+        "resource_accesskeydetails_accesskeyid": {
+            "key": "x-aws-api.access_key_id",
+            "object": "api_details"
+        },
+        "resource_accesskeydetails_principalid": {
+            "key": "user-account.user_id",
+            "object": "api_user"
+        },
+        "resource_accesskeydetails_username": {
+            "key": "user-account.account_login",
+            "object": "api_user"
+        },
+        "resource_instancedetails_availabilityzone": {
+            "key": "x-aws-instance.availability_zone",
+            "object": "instance"
+        },
+        "resource_instancedetails_imageid": {
+            "key": "x-aws-instance.image_id",
+            "object": "instance"
+        },
+        "resource_instancedetails_instanceid": {
+            "key": "x-aws-instance.instance_id",
+            "object": "instance"
         },
-        {
-            "key": "x-ibm-finding.event_count",
-            "object": "ibm_finding",
-            "transformer": "ToInteger"
-        }
-    ],
-    "data": {
-        "key": "x-oca-event.extensions.x-ocsf-data.data",
-        "object": "x-oca-event"
-    },
-    "dst_endpoint": {
-        "instance_uid": {
-            "key": "x-oca-asset.extensions.x-dst-endpoint.instance_uid",
-            "object": "asset"
-        },
-        "interface_uid": {
-            "key": "x-oca-asset.extensions.x-dst-endpoint.interface_uid",
-            "object": "asset"
-        },
-        "intermediate_ips": [
+        "resource_instancedetails_networkinterfaces_0_ipv6addresses_0": [
+            {
+                "key": "ipv6-addr.value",
+                "object": "nc_ipv6_ip"
+            },
+            {
+                "cybox": false,
+                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
+                "key": "ipv6-addr.x_aws_interface_id",
+                "object": "nc_ipv6_ip"
+            }
+        ],
+        "resource_instancedetails_networkinterfaces_0_privatednsname": [
+            {
+                "key": "domain-name.value",
+                "object": "private_dns_name"
+            }
+        ],
+        "resource_instancedetails_networkinterfaces_0_privateipaddress": [
             {
                 "key": "ipv4-addr.value",
-                "object": "dst_ipv4",
-                "transformer": "FilterIPv4List",
-                "unwrap": true
+                "object": "nc_private_ip1"
             },
             {
-                "key": "ipv6-addr.value",
-                "object": "dst_ipv6",
-                "transformer": "FilterIPv6List",
-                "unwrap": true
+                "key": "network-traffic.src_ref",
+                "object": "nc_nt",
+                "references": "nc_private_ip1"
             },
             {
-                "key": "x-oca-asset.ip_refs",
-                "object": "asset",
+                "key": "domain-name.resolves_to_refs",
+                "object": "private_dns_name",
                 "references": [
-                    "dst_ipv4",
-                    "dst_ipv6"
-                ],
-                "unwrap": true
+                    "nc_private_ip1"
+                ]
+            },
+            {
+                "key": "x-ibm-finding.src_ip_ref",
+                "object": "ibm_finding",
+                "references": "nc_private_ip1"
+            },
+            {
+                "cybox": false,
+                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
+                "key": "ipv4-addr.x_aws_interface_id",
+                "object": "nc_private_ip1"
+            },
+            {
+                "cybox": false,
+                "key": "ipv4-addr.x_aws_ip_type",
+                "object": "nc_private_ip1",
+                "value": "private"
+            }
+        ],
+        "resource_instancedetails_networkinterfaces_0_publicdnsname": [
+            {
+                "key": "domain-name.value",
+                "object": "nc_public_name"
             }
         ],
-        "ip": [
+        "resource_instancedetails_networkinterfaces_0_publicip": [
             {
                 "key": "ipv4-addr.value",
-                "object": "dst_ip",
-                "transformer": "CheckIPv4"
+                "object": "nc_public_ip"
             },
             {
-                "key": "ipv6-addr.value",
-                "object": "dst_ip",
-                "transformer": "CheckIPv6"
+                "key": "domain-name.resolves_to_refs",
+                "object": "nc_public_name",
+                "references": [
+                    "nc_public_ip"
+                ]
             },
             {
-                "key": "network-traffic.dst_ref",
-                "object": "nt",
-                "references": "dst_ip"
+                "cybox": false,
+                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
+                "key": "ipv4-addr.x_aws_interface_id",
+                "object": "nc_public_ip"
             },
             {
-                "key": "x-ibm-finding.dst_ip_ref",
-                "object": "ibm_finding",
-                "references": "dst_ip"
+                "cybox": false,
+                "key": "ipv4-addr.x_aws_ip_type",
+                "object": "nc_public_ip",
+                "value": "public"
+            }
+        ],
+        "resource_instancedetails_networkinterfaces_0_securitygroups_0_groupid": {
+            "key": "x-aws-vpc.security_group_id",
+            "object": "vpc"
+        },
+        "resource_instancedetails_networkinterfaces_0_securitygroups_0_groupname": {
+            "key": "x-aws-vpc.security_group_name",
+            "object": "vpc"
+        },
+        "resource_instancedetails_networkinterfaces_0_subnetid": {
+            "key": "x-aws-vpc.subnet_id",
+            "object": "vpc"
+        },
+        "resource_instancedetails_networkinterfaces_0_vpcid": {
+            "key": "x-aws-vpc.vpc_id",
+            "object": "vpc"
+        },
+        "resource_instancedetails_networkinterfaces_1_privatednsname": [
+            {
+                "key": "domain-name.value",
+                "object": "nc_private_name2"
+            }
+        ],
+        "resource_instancedetails_networkinterfaces_1_privateipaddress": [
+            {
+                "key": "ipv4-addr.value",
+                "object": "nc_private_ip2"
             },
             {
-                "group": true,
-                "key": "x-oca-asset.ip_refs",
-                "object": "host",
+                "key": "domain-name.resolves_to_refs",
+                "object": "nc_private_name2",
                 "references": [
-                    "dst_ip"
+                    "nc_private_ip2"
                 ]
             },
             {
-                "key": "x-oca-event.network_ref",
-                "object": "event",
-                "references": "nt"
+                "cybox": false,
+                "ds_key": "resource_instancedetails_networkinterfaces_1_networkinterfaceid",
+                "key": "ipv4-addr.x_aws_interface_id",
+                "object": "nc_private_ip2"
+            },
+            {
+                "cybox": false,
+                "key": "ipv4-addr.x_aws_ip_type",
+                "object": "nc_private_ip2",
+                "value": "private"
             }
         ],
-        "name": {
-            "key": "x-oca-asset.name",
-            "object": "asset"
-        },
-        "port": {
-            "key": "network-traffic.dst_port",
-            "object": "nt",
-            "transformer": "ToInteger"
-        },
-        "subnet_uid": {
-            "key": "x-oca-asset.extensions.x-dst-endpoint.subnet_uid",
-            "object": "asset"
-        },
-        "svc_name": {
-            "key": "x-oca-asset.extensions.x-dst-endpoint.svc_name",
-            "object": "asset"
-        },
-        "vpc_uid": {
-            "key": "x-oca-asset.extensions.x-dst-endpoint.vpc_uid",
-            "object": "asset"
-        }
-    },
-    "duration": {
-        "key": "x-oca-event.duration",
-        "object": "x_oca_event",
-        "transformer": "ToInteger"
-    },
-    "end_time": [
-        {
-            "key": "x-ibm-finding.end",
-            "object": "ibm_finding",
-            "transformer": "EpochToTimestamp"
-        },
-        {
-            "cybox": false,
-            "key": "last_observed",
-            "transformer": "EpochToTimestamp"
-        }
-    ],
-    "enrichments": {
-        "data": {
-            "key": "x-ocsf-enrichments.data",
-            "object": "enrichments"
-        },
-        "name": {
-            "key": "x-ocsf-enrichments.name",
-            "object": "enrichments"
-        },
-        "provider": {
-            "key": "x-ocsf-enrichments.provider",
-            "object": "enrichments"
-        },
-        "type": {
-            "key": "x-ocsf-enrichments.type",
-            "object": "enrichments"
-        },
-        "value": {
-            "key": "x-ocsf-enrichments.value",
-            "object": "enrichments"
-        }
-    },
-    "finding": {
-        "created_time": {
-            "key": "x-ibm-finding.start",
-            "object": "ibm_finding"
-        },
-        "desc": {
-            "key": "x-ibm-finding.description",
-            "object": "ibm_finding"
-        },
-        "first_seen_time": {
-            "key": "x-ibm-finding.time_observed",
-            "object": "ibm_finding"
-        },
-        "last_seen_time": {
-            "key": "x-ibm-finding.extensions.x-ocsf-findings.last_seen_time",
-            "object": "ibm_finding"
-        },
-        "modified_time": {
-            "key": "x-ibm-finding.extensions.x-ocsf-findings.modified_time",
-            "object": "ibm_finding"
-        },
-        "product_uid": {
-            "key": "x-ibm-finding.extensions.x-ocsf-findings.product_uid",
-            "object": "ibm_finding"
+        "resource_instancedetails_platform": [
+            {
+                "key": "software.name",
+                "object": "software"
+            },
+            {
+                "key": "x-ibm-finding.src_os_ref",
+                "object": "ibm_finding",
+                "references": "software"
+            }
+        ],
+        "service_action_awsapicallaction_api": {
+            "key": "x-aws-api.api",
+            "object": "api_details"
         },
-        "related_events": {
-            "product_uid": {
-                "key": "x-ibm-finding.extensions.x-ocsf-findings.product_uid",
+        "service_action_awsapicallaction_remoteipdetails_ipaddressv4": [
+            {
+                "key": "ipv4-addr.value",
+                "object": "api_remote_ip"
+            },
+            {
+                "key": "x-ibm-finding.dst_ip_ref",
+                "object": "ibm_finding",
+                "references": "api_remote_ip"
+            },
+            {
+                "cybox": false,
+                "ds_key": "service_action_awsapicallaction_remoteipdetails_country_countryname",
+                "key": "x-ibm-finding.dst_geolocation",
                 "object": "ibm_finding"
             },
-            "type": {
-                "key": "x-ibm-finding.extensions.x-ocsf-findings.type",
+            {
+                "cybox": false,
+                "ds_key": "service_action_awsapicallaction_remoteipdetails_city_cityname",
+                "key": "ipv4-addr.x_aws_remote_city_name",
+                "object": "api_remote_ip"
+            },
+            {
+                "cybox": false,
+                "ds_key": "service_action_awsapicallaction_remoteipdetails_country_countryname",
+                "key": "ipv4-addr.x_aws_remote_country_name",
+                "object": "api_remote_ip"
+            }
+        ],
+        "service_action_awsapicallaction_servicename": {
+            "key": "x-aws-api.service_name",
+            "object": "api_details"
+        },
+        "service_action_dnsrequestaction_domain": [
+            {
+                "key": "domain-name.value",
+                "object": "dns_domain_name"
+            }
+        ],
+        "service_action_networkconnectionaction_localportdetails_port": [
+            {
+                "key": "network-traffic.src_port",
+                "object": "nc_nt",
+                "transformer": "ToInteger"
+            }
+        ],
+        "service_action_networkconnectionaction_protocol": [
+            {
+                "key": "network-traffic.protocols",
+                "object": "nc_nt",
+                "transformer": "ToLowercaseArray"
+            }
+        ],
+        "service_action_networkconnectionaction_remoteipdetails_ipaddressv4": [
+            {
+                "key": "ipv4-addr.value",
+                "object": "nc_remote_ip"
+            },
+            {
+                "key": "network-traffic.dst_ref",
+                "object": "nc_nt",
+                "references": "nc_remote_ip"
+            },
+            {
+                "key": "x-ibm-finding.dst_ip_ref",
+                "object": "ibm_finding",
+                "references": "nc_remote_ip"
+            },
+            {
+                "cybox": false,
+                "ds_key": "service_action_networkconnectionaction_remoteipdetails_country_countryname",
+                "key": "x-ibm-finding.dst_geolocation",
                 "object": "ibm_finding"
             },
-            "type_uid": {
-                "key": "x-ibm-finding.extensions.x-ocsf-findings.type_uid",
+            {
+                "cybox": false,
+                "ds_key": "service_action_networkconnectionaction_remoteipdetails_city_cityname",
+                "key": "ipv4-addr.x_aws_remote_city_name",
+                "object": "nc_remote_ip"
+            },
+            {
+                "cybox": false,
+                "ds_key": "service_action_networkconnectionaction_remoteipdetails_country_countryname",
+                "key": "ipv4-addr.x_aws_remote_country_name",
+                "object": "nc_remote_ip"
+            }
+        ],
+        "service_action_networkconnectionaction_remoteportdetails_port": [
+            {
+                "key": "network-traffic.dst_port",
+                "object": "nc_nt",
+                "transformer": "ToInteger"
+            }
+        ],
+        "service_action_portprobeaction_portprobedetails_0_localportdetails_port": [
+            {
+                "key": "x-ibm-finding.probe_port",
                 "object": "ibm_finding"
+            }
+        ],
+        "service_action_portprobeaction_portprobedetails_0_remoteipdetails_ipaddressv4": [
+            {
+                "key": "ipv4-addr.value",
+                "object": "pp_remote_ip"
             },
-            "uid": {
-                "key": "x-ibm-finding.extensions.x-ocsf-findings.uid",
+            {
+                "key": "x-ibm-finding.dst_ip_ref",
+                "object": "ibm_finding",
+                "references": "pp_remote_ip"
+            },
+            {
+                "cybox": false,
+                "ds_key": "service_action_portprobeaction_portprobedetails_0_remoteipdetails_country_countryname",
+                "key": "x-ibm-finding.dst_geolocation",
                 "object": "ibm_finding"
+            },
+            {
+                "cybox": false,
+                "ds_key": "service_action_portprobeaction_portprobedetails_0_remoteipdetails_city_cityname",
+                "key": "ipv4-addr.x_aws_remote_city_name",
+                "object": "pp_remote_ip"
+            },
+            {
+                "cybox": false,
+                "ds_key": "service_action_portprobeaction_portprobedetails_0_remoteipdetails_country_countryname",
+                "key": "ipv4-addr.x_aws_remote_country_name",
+                "object": "pp_remote_ip"
             }
-        },
-        "remediation": {
-            "desc": {
-                "key": "x-ibm-finding.extensions.x-ocsf-findings.remediation_desc",
+        ],
+        "service_eventfirstseen": [
+            {
+                "cybox": false,
+                "key": "first_observed"
+            },
+            {
+                "key": "x-ibm-finding.start",
                 "object": "ibm_finding"
+            }
+        ],
+        "service_eventlastseen": [
+            {
+                "cybox": false,
+                "key": "last_observed"
             },
-            "kb_articles": {
-                "key": "x-ibm-finding.extensions.x-ocsf-findings.remediation_kb_articles",
+            {
+                "key": "x-ibm-finding.end",
                 "object": "ibm_finding"
             }
-        },
-        "src_url": {
-            "key": "x-ibm-finding.extensions.x-ocsf-findings.src_url",
-            "object": "ibm_finding"
-        },
-        "supporting_data": {
-            "key": "x-ibm-finding.extensions.x-ocsf-findings.upporting_data",
+        ],
+        "severity": {
+            "key": "x-ibm-finding.severity",
             "object": "ibm_finding"
         },
         "title": {
             "key": "x-ibm-finding.name",
             "object": "ibm_finding"
         },
-        "types": {
-            "key": "x-ibm-finding.types",
-            "object": "ibm_finding"
-        },
-        "uid": {
-            "key": "x-ibm-finding.alert_id",
+        "type": {
+            "key": "x-ibm-finding.finding_type",
             "object": "ibm_finding"
         }
     },
-    "http_request": {
-        "args": {
-            "key": "x-ocsf-http-request.value",
-            "object": "http_request"
-        },
-        "http_headers": {
-            "name": {
-                "key": "x-ocsf-http-request.http_headers_name",
-                "object": "ocsf_cloud_api"
+    "ocsf": {
+        "_time": [
+            {
+                "cybox": false,
+                "key": "first_observed",
+                "transformer": "EpochToTimestamp"
             },
-            "value": {
-                "key": "x-ocsf-http-request.http_headers_value",
-                "object": "http_request"
+            {
+                "cybox": false,
+                "key": "last_observed",
+                "transformer": "EpochToTimestamp"
+            },
+            {
+                "key": "x-ibm-finding.time_observed",
+                "object": "ibm_finding",
+                "transformer": "EpochToTimestamp"
             }
+        ],
+        "activity": {
+            "key": "x-oca-event.action",
+            "object": "x_oca_event"
+        },
+        "activity_id": {
+            "key": "x-oca-event.code",
+            "object": "x_oca_event",
+            "transformer": "ToInteger"
         },
-        "http_method": {
-            "key": "x-ocsf-http-request.http_method",
-            "object": "http_request"
-        },
-        "prefix": {
-            "key": "x-ocsf-http-request.prefix",
-            "object": "http_request"
-        },
-        "referrer": {
-            "key": "x-ocsf-http-request.referrer",
-            "object": "http_request"
-        },
-        "uid": {
-            "key": "x-ocsf-http-request.uid",
-            "object": "http_request"
-        },
-        "url": {
-            "key": "url.value",
-            "object": "url"
-        },
-        "user_agent": {
-            "key": "x-ocsf-http-request.user_agent",
-            "object": "http_request"
-        },
-        "version": {
-            "key": "x-ocsf-http-request.version",
-            "object": "http_request"
-        },
-        "x_forwarded_for": {
-            "key": "x-ocsf-http-request.x_forwarded_for",
-            "object": "http_request"
-        }
-    },
-    "identity": {
-        "authorizations": {
-            "decision": {
-                "key": "x-ocsf-identity.authorizations.decision",
-                "object": "x-ocsf-identity"
+        "activity_name": {
+            "key": "x-oca-event.action",
+            "object": "x_oca_event"
+        },
+        "api": {
+            "operation": {
+                "key": "x-ocsf-cloud.operation",
+                "object": "ocsf_cloud_api"
             },
-            "policy": {
-                "desc": {
-                    "key": "x-ocsf-identity.authorizations.policy_desc",
-                    "object": "x-ocsf-identity"
+            "request": {
+                "flags": {
+                    "key": "x-ocsf-cloud.request_flags",
+                    "object": "ocsf_cloud_api",
+                    "transformer": "ToLowercaseArray"
                 },
-                "group": {
-                    "desc": {
-                        "key": "x-ocsf-identity.authorizations.policy_group_desc",
-                        "object": "x-ocsf-identity"
-                    },
-                    "name": {
-                        "key": "x-ocsf-identity.authorizations.policy_group_namee",
-                        "object": "x-ocsf-identity"
-                    },
-                    "privileges": {
-                        "key": "x-ocsf-identity.authorizations.policy_group_privileges",
-                        "object": "x-ocsf-identity"
-                    },
-                    "type": {
-                        "key": "x-ocsf-identity.authorizations.policy_group_type",
-                        "object": "x-ocsf-identity"
-                    },
-                    "uid": {
-                        "key": "x-ocsf-identity.authorizations.policy_group_uid",
-                        "object": "x-ocsf-identity"
-                    }
+                "uid": {
+                    "key": "x-ocsf-cloud.request_uid",
+                    "object": "ocsf_cloud_api"
+                }
+            },
+            "response": {
+                "code": {
+                    "key": "x-ocsf-cloud.response_code",
+                    "object": "ocsf_cloud_api",
+                    "transformer": "ToInteger"
+                },
+                "error": {
+                    "key": "x-ocsf-cloud.response_error",
+                    "object": "ocsf_cloud_api"
+                },
+                "error_message": {
+                    "key": "x-ocsf-cloud.response_error_message",
+                    "object": "ocsf_cloud_api"
+                },
+                "flags": {
+                    "key": "x-ocsf-cloud.response_flags",
+                    "object": "ocsf_cloud_api",
+                    "transformer": "ToLowercaseArray"
+                },
+                "message": {
+                    "key": "x-ocsf-cloud.response_message",
+                    "object": "ocsf_cloud_api"
+                }
+            },
+            "service": {
+                "labels": {
+                    "key": "x-ocsf-cloud.service_labels",
+                    "object": "ocsf_cloud_api",
+                    "transformer": "ToLowercaseArray"
                 },
                 "name": {
-                    "key": "x-ocsf-identity.authorizations.name",
-                    "object": "x-ocsf-identity"
+                    "key": "x-ocsf-cloud.service_name",
+                    "object": "ocsf_cloud_api"
                 },
                 "uid": {
-                    "key": "x-ocsf-identity.authorizations.uid",
-                    "object": "x-ocsf-identity"
+                    "key": "x-ocsf-cloud.service_uid",
+                    "object": "ocsf_cloud_api"
                 },
                 "version": {
-                    "key": "x-ocsf-identity.authorizations.version",
-                    "object": "x-ocsf-identity"
+                    "key": "x-ocsf-cloud.service_uid",
+                    "object": "ocsf_cloud_api"
                 }
+            },
+            "version": {
+                "key": "x-ocsf-cloud.api_version",
+                "object": "ocsf_cloud_api"
             }
         },
-        "idp": {
-            "name": {
-                "key": "x-ocsf-identity.idp.name",
-                "object": "x-ocsf-identity"
+        "attacks": {
+            "tactics": {
+                "name": {
+                    "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.tactic_name",
+                    "object": "ttp-tagging"
+                },
+                "uid": {
+                    "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.tactic_id",
+                    "object": "ttp-tagging"
+                }
             },
-            "uid": {
-                "key": "x-ocsf-identity.idp.uid",
-                "object": "x-ocsf-identity"
+            "technique": {
+                "name": [
+                    {
+                        "key": "x-ibm-ttp-tagging.name",
+                        "object": "ttp-tagging"
+                    },
+                    {
+                        "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.technique_name",
+                        "object": "ttp-tagging"
+                    },
+                    {
+                        "key": "x-ibm-finding.ttp_tagging_refs",
+                        "object": "ibm_finding",
+                        "references": [
+                            "ttp-tagging"
+                        ]
+                    }
+                ],
+                "uid": {
+                    "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.technique_id",
+                    "object": "ttp-tagging"
+                }
+            },
+            "version": {
+                "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.versoin",
+                "object": "ttp-tagging"
             }
         },
-        "invoked_by": {
-            "key": "x-ocsf-identity.invoked_by",
-            "object": "x-ocsf-identity"
+        "category_name": {
+            "key": "x-oca-event.category",
+            "object": "x_oca_event"
+        },
+        "category_uid": {
+            "key": "x-oca-event.code",
+            "object": "x_oca_event",
+            "transformer": "ToInteger"
         },
-        "message": {
-            "key": "x-ocsf-identity.message",
-            "object": "x-ocsf-identity"
+        "class_name": {
+            "key": "x-oca-event.module",
+            "object": "x_oca_event"
+        },
+        "class_uid": {
+            "key": "x-oca-event.extensions.x-cloud-api.class_uid",
+            "object": "x_oca_event",
+            "transformer": "ToInteger"
         },
-        "session": {
-            "created_time": {
-                "key": "x-ocsf-identity.session.created_time",
-                "object": "x-ocsf-identity"
+        "cloud": {
+            "account_type": {
+                "key": "x-ocsf-cloud.account_type",
+                "object": "ocsf_cloud_api"
             },
-            "credential_uid": {
-                "key": "x-ocsf-identity.session.credential_uid",
-                "object": "x-ocsf-identity"
+            "account_type_id": {
+                "key": "x-ocsf-cloud.account_type_id",
+                "object": "ocsf_cloud_api",
+                "transformer": "ToInteger"
             },
-            "expiration_time": {
-                "key": "x-ocsf-identity.session.expiration_time",
-                "object": "x-ocsf-identity"
+            "account_uid": {
+                "key": "x-ocsf-cloud.account_uid",
+                "object": "ocsf_cloud_api"
             },
-            "issuer": {
-                "key": "x-ocsf-identity.session.issuer",
-                "object": "x-ocsf-identity"
+            "org_uid": {
+                "key": "x-ocsf-cloud.org_uid",
+                "object": "ocsf_cloud_api"
             },
-            "mfa": {
-                "key": "x-ocsf-identity.session.mfa",
-                "object": "x-ocsf-identity"
+            "project_uid": {
+                "key": "x-ocsf-cloud.project_uid",
+                "object": "ocsf_cloud_api"
             },
-            "uid": {
-                "key": "x-ocsf-identity.session.uid",
-                "object": "x-ocsf-identity"
+            "provider": {
+                "key": "x-ocsf-cloud.provider",
+                "object": "ocsf_cloud_api"
+            },
+            "region": {
+                "key": "x-ocsf-cloud.region",
+                "object": "ocsf_cloud_api"
+            },
+            "resource_uid": {
+                "key": "x-ocsf-cloud.resource_uid",
+                "object": "ocsf_cloud_api"
+            },
+            "zone": {
+                "key": "x-ocsf-cloud.zone",
+                "object": "ocsf_cloud_api"
             }
         },
-        "user": {
-            "account_type": {
-                "key": "user-account.account_type",
-                "object": "user"
+        "compliance": {
+            "requirements": {
+                "key": "x-ocsf-compliance.requirements",
+                "object": "compliance"
+            },
+            "status": {
+                "key": "x-ocsf-compliance.status",
+                "object": "compliance"
+            },
+            "status_detail": {
+                "key": "x-ocsf-compliance.status_detail",
+                "object": "compliance"
+            }
+        },
+        "confidence": {
+            "key": "x-oca-event.confidence",
+            "object": "x-oca-event"
+        },
+        "connection_info": {
+            "boundary": {
+                "key": "network-traffic.extensions.x-network-ext.boundary",
+                "object": "nt"
+            },
+            "boundary_id": {
+                "key": "network-traffic.extensions.x-network-ext.boundary_id",
+                "object": "nt"
+            },
+            "direction": {
+                "key": "network-traffic.extensions.x-network-ext.direction",
+                "object": "nt"
+            },
+            "direction_id": {
+                "key": "network-traffic.extensions.x-network-ext.direction_id",
+                "object": "nt"
+            },
+            "protocol_name": {
+                "key": "network-traffic.extensions.x-network-ext.protocol_name",
+                "object": "nt"
             },
-            "account_type_id": {
-                "key": "user-account.extensions.aws-account-ext.account_type_id",
-                "object": "user",
-                "transformer": "ToInteger"
+            "protocol_num": {
+                "group": true,
+                "key": "network-traffic.protocols",
+                "object": "nt",
+                "transformer": "ProtocolNumToName"
             },
-            "account_uid": {
-                "key": "user-account.user_id",
-                "object": "user"
+            "protocol_ver": {
+                "group": true,
+                "key": "network-traffic.protocols",
+                "object": "nt",
+                "transformer": "ToLowercaseArray"
             },
-            "credential_uid": {
-                "key": "user-account.extensions.aws-account-ext.credential_uid",
-                "object": "user"
-            },
-            "domain": {
-                "key": "user-account.extensions.aws-account-ext.domain",
-                "object": "user"
-            },
-            "email_addr": {
-                "key": "email-addr.value",
-                "object": "email_addr"
+            "protocol_ver_id": {
+                "key": "network-traffic.extensions.x-network-ext.protocol_ver_id",
+                "object": "nt"
             },
-            "groups": {
-                "desc": {
-                    "key": "user-account.extensions.aws-account-ext.group_desc",
-                    "object": "user"
+            "tcp_flags": {
+                "key": "network-traffic.extensions.tcp-ext.src_flags_hex",
+                "object": "nt"
+            }
+        },
+        "count": [
+            {
+                "cybox": false,
+                "key": "number_observed",
+                "transformer": "ToInteger"
+            },
+            {
+                "key": "x-ibm-finding.event_count",
+                "object": "ibm_finding",
+                "transformer": "ToInteger"
+            }
+        ],
+        "data": {
+            "key": "x-oca-event.extensions.x-ocsf-data.data",
+            "object": "x-oca-event"
+        },
+        "dst_endpoint": {
+            "instance_uid": {
+                "key": "x-oca-asset.extensions.x-dst-endpoint.instance_uid",
+                "object": "asset"
+            },
+            "interface_uid": {
+                "key": "x-oca-asset.extensions.x-dst-endpoint.interface_uid",
+                "object": "asset"
+            },
+            "intermediate_ips": [
+                {
+                    "key": "ipv4-addr.value",
+                    "object": "dst_ipv4",
+                    "transformer": "FilterIPv4List",
+                    "unwrap": true
                 },
-                "name": {
-                    "key": "user-account.extensions.aws-account-ext.group_name",
-                    "object": "user"
+                {
+                    "key": "ipv6-addr.value",
+                    "object": "dst_ipv6",
+                    "transformer": "FilterIPv6List",
+                    "unwrap": true
                 },
-                "privileges": {
-                    "key": "user-account.extensions.aws-account-ext.group_privileges",
-                    "object": "user"
+                {
+                    "key": "x-oca-asset.ip_refs",
+                    "object": "asset",
+                    "references": [
+                        "dst_ipv4",
+                        "dst_ipv6"
+                    ],
+                    "unwrap": true
+                }
+            ],
+            "ip": [
+                {
+                    "key": "ipv4-addr.value",
+                    "object": "dst_ip",
+                    "transformer": "CheckIPv4"
                 },
-                "type": {
-                    "key": "user-account.extensions.aws-account-ext.group_type",
-                    "object": "user"
+                {
+                    "key": "ipv6-addr.value",
+                    "object": "dst_ip",
+                    "transformer": "CheckIPv6"
                 },
-                "uid": {
-                    "key": "user-account.extensions.aws-account-ext.group_uid",
-                    "object": "user"
+                {
+                    "key": "network-traffic.dst_ref",
+                    "object": "nt",
+                    "references": "dst_ip"
+                },
+                {
+                    "key": "x-ibm-finding.dst_ip_ref",
+                    "object": "ibm_finding",
+                    "references": "dst_ip"
+                },
+                {
+                    "group": true,
+                    "key": "x-oca-asset.ip_refs",
+                    "object": "host",
+                    "references": [
+                        "dst_ip"
+                    ]
+                },
+                {
+                    "key": "x-oca-event.network_ref",
+                    "object": "event",
+                    "references": "nt"
                 }
-            },
+            ],
             "name": {
-                "key": "user-account.display_name",
-                "object": "user"
+                "key": "x-oca-asset.name",
+                "object": "asset"
             },
-            "org_uid": {
-                "key": "user-account.extensions.aws-account-ext.org_uid",
-                "object": "user"
+            "port": {
+                "key": "network-traffic.dst_port",
+                "object": "nt",
+                "transformer": "ToInteger"
             },
-            "session_uid": {
-                "key": "user-account.extensions.aws-account-ext.session_uid",
-                "object": "user"
-            },
-            "session_uuid": {
-                "key": "user-account.extensions.aws-account-ext.session_uuid",
-                "object": "user"
+            "subnet_uid": {
+                "key": "x-oca-asset.extensions.x-dst-endpoint.subnet_uid",
+                "object": "asset"
+            },
+            "svc_name": {
+                "key": "x-oca-asset.extensions.x-dst-endpoint.svc_name",
+                "object": "asset"
+            },
+            "vpc_uid": {
+                "key": "x-oca-asset.extensions.x-dst-endpoint.vpc_uid",
+                "object": "asset"
+            }
+        },
+        "duration": {
+            "key": "x-oca-event.duration",
+            "object": "x_oca_event",
+            "transformer": "ToInteger"
+        },
+        "end_time": [
+            {
+                "key": "x-ibm-finding.end",
+                "object": "ibm_finding",
+                "transformer": "EpochToTimestamp"
             },
-            "type": {
-                "key": "user-account.extensions.aws-account-ext.type",
-                "object": "user"
+            {
+                "cybox": false,
+                "key": "last_observed",
+                "transformer": "EpochToTimestamp"
+            }
+        ],
+        "enrichments": {
+            "data": {
+                "key": "x-ocsf-enrichments.data",
+                "object": "enrichments"
             },
-            "type_id": {
-                "key": "user-account.extensions.aws-account-ext.type_id",
-                "object": "user",
-                "transformer": "ToInteger"
+            "name": {
+                "key": "x-ocsf-enrichments.name",
+                "object": "enrichments"
             },
-            "uid": {
-                "key": "user-account.extensions.aws-account-ext.uid",
-                "object": "user"
+            "provider": {
+                "key": "x-ocsf-enrichments.provider",
+                "object": "enrichments"
+            },
+            "type": {
+                "key": "x-ocsf-enrichments.type",
+                "object": "enrichments"
             },
-            "uuid": {
-                "key": "user-account.extensions.aws-account-ext.uuid",
-                "object": "user"
+            "value": {
+                "key": "x-ocsf-enrichments.value",
+                "object": "enrichments"
             }
-        }
-    },
-    "malware": {
-        "classification_ids": {
-            "key": "x-ocsf-malware.classification_ids",
-            "object": "malware"
-        },
-        "classifications": {
-            "key": "x-ocsf-malware.classifications",
-            "object": "malware"
         },
-        "cves": {
+        "finding": {
             "created_time": {
-                "key": "x-ocsf-malware.created_time",
-                "object": "malware"
+                "key": "x-ibm-finding.start",
+                "object": "ibm_finding"
             },
-            "cvss": {
-                "base_score": {
-                    "key": "x-ocsf-malware.base_score",
-                    "object": "malware"
-                },
-                "depth": {
-                    "key": "x-ocsf-malware.depth",
-                    "object": "malware"
-                },
-                "metrics": {
-                    "name": {
-                        "key": "x-ocsf-malware.name",
-                        "object": "malware"
-                    },
-                    "value": {
-                        "key": "x-ocsf-malware.value",
-                        "object": "malware"
-                    }
-                },
-                "overall_score": {
-                    "key": "x-ocsf-malware.overall_score",
-                    "object": "malware"
-                },
-                "severity": {
-                    "key": "x-ocsf-malware.severity",
-                    "object": "malware"
-                },
-                "vector_string": {
-                    "key": "x-ocsf-malware.vector_string",
-                    "object": "malware"
-                },
-                "version": {
-                    "key": "x-ocsf-malware.version",
-                    "object": "malware"
-                }
+            "desc": {
+                "key": "x-ibm-finding.description",
+                "object": "ibm_finding"
             },
-            "cwe_uid": {
-                "key": "x-ocsf-malware.cwe_uid",
-                "object": "malware"
+            "first_seen_time": {
+                "key": "x-ibm-finding.time_observed",
+                "object": "ibm_finding"
             },
-            "cwe_url": {
-                "key": "x-ocsf-malware.cwe_url",
-                "object": "malware"
+            "last_seen_time": {
+                "key": "x-ibm-finding.extensions.x-ocsf-findings.last_seen_time",
+                "object": "ibm_finding"
             },
             "modified_time": {
-                "key": "x-ocsf-malware.modified_time",
-                "object": "malware"
+                "key": "x-ibm-finding.extensions.x-ocsf-findings.modified_time",
+                "object": "ibm_finding"
             },
-            "product": {
-                "feature": {
-                    "name": {
-                        "key": "software.extensions.x-ocsf-product-ext.feature_name",
-                        "object": "malware-software"
-                    },
-                    "uid": {
-                        "key": "software.extensions.x-ocsf-product-ext.feature_uid",
-                        "object": "malware-software"
-                    },
-                    "version": {
-                        "key": "software.extensions.x-ocsf-product-ext.feature_version",
-                        "object": "malware-software"
-                    }
-                },
-                "lang": {
-                    "key": "software.languages",
-                    "object": "malware-software"
+            "product_uid": {
+                "key": "x-ibm-finding.extensions.x-ocsf-findings.product_uid",
+                "object": "ibm_finding"
+            },
+            "related_events": {
+                "product_uid": {
+                    "key": "x-ibm-finding.extensions.x-ocsf-findings.product_uid",
+                    "object": "ibm_finding"
                 },
-                "name": {
-                    "key": "software.name",
-                    "object": "malware-software"
+                "type": {
+                    "key": "x-ibm-finding.extensions.x-ocsf-findings.type",
+                    "object": "ibm_finding"
                 },
-                "path": {
-                    "key": "software.extensions.x-ocsf-product-ext.installed_path",
-                    "object": "malware-software"
+                "type_uid": {
+                    "key": "x-ibm-finding.extensions.x-ocsf-findings.type_uid",
+                    "object": "ibm_finding"
                 },
                 "uid": {
-                    "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                    "object": "malware-software"
-                },
-                "vendor_name": {
-                    "key": "software.vendor",
-                    "object": "malware-software"
+                    "key": "x-ibm-finding.extensions.x-ocsf-findings.uid",
+                    "object": "ibm_finding"
+                }
+            },
+            "remediation": {
+                "desc": {
+                    "key": "x-ibm-finding.extensions.x-ocsf-findings.remediation_desc",
+                    "object": "ibm_finding"
                 },
-                "version": {
-                    "key": "software.version",
-                    "object": "malware-software"
+                "kb_articles": {
+                    "key": "x-ibm-finding.extensions.x-ocsf-findings.remediation_kb_articles",
+                    "object": "ibm_finding"
                 }
             },
-            "type": {
-                "key": "x-ocsf-malware.type",
-                "object": "malware"
+            "src_url": {
+                "key": "x-ibm-finding.extensions.x-ocsf-findings.src_url",
+                "object": "ibm_finding"
+            },
+            "supporting_data": {
+                "key": "x-ibm-finding.extensions.x-ocsf-findings.upporting_data",
+                "object": "ibm_finding"
+            },
+            "title": {
+                "key": "x-ibm-finding.name",
+                "object": "ibm_finding"
+            },
+            "types": {
+                "key": "x-ibm-finding.types",
+                "object": "ibm_finding"
             },
             "uid": {
-                "key": "x-ocsf-malware.uid",
-                "object": "malware"
+                "key": "x-ibm-finding.alert_id",
+                "object": "ibm_finding"
             }
         },
-        "name": {
-            "key": "x-ocsf-malware.name",
-            "object": "malware"
-        },
-        "path": {
-            "key": "x-ocsf-malware.path",
-            "object": "malware"
-        },
-        "provider": {
-            "key": "x-ocsf-malware.provider",
-            "object": "malware"
-        },
-        "uid": {
-            "key": "x-ocsf-malware.uid",
-            "object": "malware"
-        }
-    },
-    "message": {
-        "key": "x-ocsf-cloud.message",
-        "object": "ocsf_cloud_api"
-    },
-    "metadata": {
-        "correlation_uid": {
-            "key": "x-ocsf-metadata.correlation_uid",
-            "object": "metadata"
-        },
-        "labels": {
-            "key": "x-ocsf-metadata.labels",
-            "object": "metadata"
-        },
-        "logged_time": {
-            "key": "x-ocsf-metadata.logged_time",
-            "object": "metadata"
-        },
-        "modified_time": {
-            "key": "x-ocsf-metadata.modified_time",
-            "object": "metadata"
-        },
-        "processed_time": {
-            "key": "x-ocsf-metadata.processed_time",
-            "object": "metadata"
-        },
-        "product": {
-            "feature": {
+        "http_request": {
+            "args": {
+                "key": "x-ocsf-http-request.value",
+                "object": "http_request"
+            },
+            "http_headers": {
                 "name": {
-                    "key": "software.extensions.x-ocsf-product-ext.feature_name",
-                    "object": "metadata-software"
+                    "key": "x-ocsf-http-request.http_headers_name",
+                    "object": "ocsf_cloud_api"
                 },
-                "uid": {
-                    "key": "software.extensions.x-ocsf-product-ext.feature_uid",
-                    "object": "metadata-software"
-                },
-                "version": {
-                    "key": "software.extensions.x-ocsf-product-ext.feature_version",
-                    "object": "metadata-software"
+                "value": {
+                    "key": "x-ocsf-http-request.http_headers_value",
+                    "object": "http_request"
                 }
             },
-            "lang": {
-                "key": "software.languages",
-                "object": "metadata-software"
+            "http_method": {
+                "key": "x-ocsf-http-request.http_method",
+                "object": "http_request"
             },
-            "name": {
-                "key": "software.name",
-                "object": "metadata-software"
+            "prefix": {
+                "key": "x-ocsf-http-request.prefix",
+                "object": "http_request"
             },
-            "path": {
-                "key": "software.extensions.x-ocsf-product-ext.installed_path",
-                "object": "metadata-software"
+            "referrer": {
+                "key": "x-ocsf-http-request.referrer",
+                "object": "http_request"
             },
             "uid": {
-                "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                "object": "metadata-software"
+                "key": "x-ocsf-http-request.uid",
+                "object": "http_request"
             },
-            "vendor_name": {
-                "key": "software.vendor",
-                "object": "metadata-software"
+            "url": {
+                "key": "url.value",
+                "object": "url"
+            },
+            "user_agent": {
+                "key": "x-ocsf-http-request.user_agent",
+                "object": "http_request"
             },
             "version": {
-                "key": "software.version",
-                "object": "metadata-software"
-            }
-        },
-        "sequence": {
-            "key": "x-ocsf-metadata.sequence",
-            "object": "metadata",
-            "transformer": "ToInteger"
-        },
-        "uid": {
-            "key": "x-ocsf-metadata.uid",
-            "object": "metadata"
-        },
-        "version": {
-            "key": "x-ocsf-metadata.version",
-            "object": "metadata"
-        }
-    },
-    "observables": {
-        "name": [
-            {
-                "key": "x-ibm-observables.name",
-                "object": "observables"
+                "key": "x-ocsf-http-request.version",
+                "object": "http_request"
             },
-            {
-                "key": "x-ibm-finding.ioc_refs",
-                "object": "ibm_finding",
-                "references": [
-                    "observables"
-                ]
+            "x_forwarded_for": {
+                "key": "x-ocsf-http-request.x_forwarded_for",
+                "object": "http_request"
             }
-        ],
-        "type": {
-            "key": "x-ibm-observables.finding_type",
-            "object": "observables"
-        },
-        "type_id": {
-            "key": "x-ibm-observables.alert_id",
-            "object": "observables",
-            "transformer": "ToInteger"
         },
-        "value": {
-            "key": "x-ibm-observables.description",
-            "object": "observables"
-        }
-    },
-    "process": {
-        "cmd_line": {
-            "key": "process.command_line",
-            "object": "process"
-        },
-        "created_time": {
-            "key": "process.created",
-            "object": "process"
-        },
-        "file": {
-            "accessed_time": {
-                "key": "file.accessed",
-                "object": "file"
-            },
-            "accessor": {
-                "account_type": {
-                    "key": "user-account.account_type",
-                    "object": "accessor-user-account"
-                },
-                "account_type_id": {
-                    "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                    "object": "accessor-user-account"
-                },
-                "account_uid": {
-                    "key": "user-account.extensions.x-accessor-ext.account_uid",
-                    "object": "accessor-user-account"
-                },
-                "credential_uid": {
-                    "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                    "object": "accessor-user-account"
-                },
-                "domain": {
-                    "key": "user-account.extensions.x-accessor-ext.domain",
-                    "object": "accessor-user-account"
-                },
-                "email_addr": {
-                    "key": "email-addr.value",
-                    "object": "email-addr"
+        "identity": {
+            "authorizations": {
+                "decision": {
+                    "key": "x-ocsf-identity.authorizations.decision",
+                    "object": "x-ocsf-identity"
                 },
-                "groups": {
+                "policy": {
                     "desc": {
-                        "key": "user-account.extensions.x-accessor-ext.group_desc",
-                        "object": "accessor-user-account"
-                    },
-                    "name": {
-                        "key": "user-account.extensions.x-accessor-ext.group_name",
-                        "object": "accessor-user-account"
+                        "key": "x-ocsf-identity.authorizations.policy_desc",
+                        "object": "x-ocsf-identity"
                     },
-                    "privileges": {
-                        "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                        "object": "accessor-user-account"
+                    "group": {
+                        "desc": {
+                            "key": "x-ocsf-identity.authorizations.policy_group_desc",
+                            "object": "x-ocsf-identity"
+                        },
+                        "name": {
+                            "key": "x-ocsf-identity.authorizations.policy_group_namee",
+                            "object": "x-ocsf-identity"
+                        },
+                        "privileges": {
+                            "key": "x-ocsf-identity.authorizations.policy_group_privileges",
+                            "object": "x-ocsf-identity"
+                        },
+                        "type": {
+                            "key": "x-ocsf-identity.authorizations.policy_group_type",
+                            "object": "x-ocsf-identity"
+                        },
+                        "uid": {
+                            "key": "x-ocsf-identity.authorizations.policy_group_uid",
+                            "object": "x-ocsf-identity"
+                        }
                     },
-                    "type": {
-                        "key": "user-account.extensions.x-accessor-ext.group_type",
-                        "object": "accessor-user-account"
+                    "name": {
+                        "key": "x-ocsf-identity.authorizations.name",
+                        "object": "x-ocsf-identity"
                     },
                     "uid": {
-                        "key": "user-account.extensions.x-accessor-ext.group_uid",
-                        "object": "accessor-user-account"
+                        "key": "x-ocsf-identity.authorizations.uid",
+                        "object": "x-ocsf-identity"
+                    },
+                    "version": {
+                        "key": "x-ocsf-identity.authorizations.version",
+                        "object": "x-ocsf-identity"
                     }
-                },
+                }
+            },
+            "idp": {
                 "name": {
-                    "key": "user-account.display_name",
-                    "object": "accessor-user-account"
-                },
-                "org_uid": {
-                    "key": "user-account.extensions.x-accessor-ext.org_uid",
-                    "object": "accessor-user-account"
-                },
-                "session_uid": {
-                    "key": "user-account.extensions.x-accessor-ext.session_uid",
-                    "object": "accessor-user-account"
-                },
-                "session_uuid": {
-                    "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                    "object": "accessor-user-account"
-                },
-                "type": {
-                    "key": "user-account.extensions.x-accessor-ext.type",
-                    "object": "accessor-user-account"
-                },
-                "type_id": {
-                    "key": "user-account.extensions.x-accessor-ext.type_id",
-                    "object": "accessor-user-account"
+                    "key": "x-ocsf-identity.idp.name",
+                    "object": "x-ocsf-identity"
                 },
                 "uid": {
-                    "key": "user-account.user_id",
-                    "object": "accessor-user-account"
-                },
-                "uuid": {
-                    "key": "user-account.extensions.x-accessor-ext.uuid",
-                    "object": "accessor-user-account"
+                    "key": "x-ocsf-identity.idp.uid",
+                    "object": "x-ocsf-identity"
                 }
             },
-            "attributes": {
-                "key": "file.extensions.x-ocsf-file-ext.attributes",
-                "object": "file"
-            },
-            "company_name": {
-                "key": "file.extensions.x-ocsf-file-ext.company_name",
-                "object": "file"
-            },
-            "confidentiality": {
-                "key": "file.extensions.x-ocsf-file-ext.confidentiality",
-                "object": "file"
-            },
-            "confidentiality_id": {
-                "key": "file.extensions.x-ocsf-file-ext.confidentiality_id",
-                "object": "file"
+            "invoked_by": {
+                "key": "x-ocsf-identity.invoked_by",
+                "object": "x-ocsf-identity"
             },
-            "created_time": {
-                "key": "file.created",
-                "object": "file"
+            "message": {
+                "key": "x-ocsf-identity.message",
+                "object": "x-ocsf-identity"
             },
-            "creator": {
-                "account_type": {
-                    "key": "user-account.account_type",
-                    "object": "creator-user-account"
-                },
-                "account_type_id": {
-                    "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                    "object": "creator-user-account"
-                },
-                "account_uid": {
-                    "key": "user-account.extensions.x-accessor-ext.account_uid",
-                    "object": "creator-user-account"
+            "session": {
+                "created_time": {
+                    "key": "x-ocsf-identity.session.created_time",
+                    "object": "x-ocsf-identity"
                 },
                 "credential_uid": {
-                    "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                    "object": "creator-user-account"
-                },
-                "domain": {
-                    "key": "user-account.extensions.x-accessor-ext.domain",
-                    "object": "creator-user-account"
-                },
-                "email_addr": {
-                    "key": "email-addr.value",
-                    "object": "creator-email-addr"
-                },
-                "groups": {
-                    "desc": {
-                        "key": "user-account.extensions.x-accessor-ext.group_desc",
-                        "object": "creator-user-account"
-                    },
-                    "name": {
-                        "key": "user-account.extensions.x-accessor-ext.group_name",
-                        "object": "creator-user-account"
-                    },
-                    "privileges": {
-                        "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                        "object": "creator-user-account"
-                    },
-                    "type": {
-                        "key": "user-account.extensions.x-accessor-ext.group_type",
-                        "object": "creator-user-account"
-                    },
-                    "uid": {
-                        "key": "user-account.extensions.x-accessor-ext.group_uid",
-                        "object": "creator-user-account"
-                    }
-                },
-                "name": {
-                    "key": "user-account.display_name",
-                    "object": "creator-user-account"
-                },
-                "org_uid": {
-                    "key": "user-account.extensions.x-accessor-ext.org_uid",
-                    "object": "creator-user-account"
-                },
-                "session_uid": {
-                    "key": "user-account.extensions.x-accessor-ext.session_uid",
-                    "object": "creator-user-account"
+                    "key": "x-ocsf-identity.session.credential_uid",
+                    "object": "x-ocsf-identity"
                 },
-                "session_uuid": {
-                    "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                    "object": "creator-user-account"
+                "expiration_time": {
+                    "key": "x-ocsf-identity.session.expiration_time",
+                    "object": "x-ocsf-identity"
                 },
-                "type": {
-                    "key": "user-account.extensions.x-accessor-ext.type",
-                    "object": "creator-user-account"
+                "issuer": {
+                    "key": "x-ocsf-identity.session.issuer",
+                    "object": "x-ocsf-identity"
                 },
-                "type_id": {
-                    "key": "user-account.extensions.x-accessor-ext.type_id",
-                    "object": "creator-user-account"
+                "mfa": {
+                    "key": "x-ocsf-identity.session.mfa",
+                    "object": "x-ocsf-identity"
                 },
                 "uid": {
-                    "key": "user-account.user_id",
-                    "object": "creator-user-account"
-                },
-                "uuid": {
-                    "key": "user-account.extensions.x-accessor-ext.uuid",
-                    "object": "creator-user-account"
-                }
-            },
-            "desc": {
-                "key": "file.extensions.x-ocsf-file-ext.description",
-                "object": "file"
-            },
-            "hashes": {
-                "CTPH": {
-                    "key": "file.hashes.CTPH",
-                    "object": "file"
-                },
-                "MD5": {
-                    "key": "file.hashes.MD5",
-                    "object": "file"
-                },
-                "Other": {
-                    "key": "file.hashes.Other",
-                    "object": "file"
-                },
-                "SHA-1": {
-                    "key": "file.hashes.SHA-1",
-                    "object": "file"
-                },
-                "SHA-256": {
-                    "key": "file.hashes.SHA-256",
-                    "object": "file"
-                },
-                "SHA-512": {
-                    "key": "file.hashes.SHA-512",
-                    "object": "file"
-                },
-                "Unknown": {
-                    "key": "file.hashes.Unknown",
-                    "object": "file"
+                    "key": "x-ocsf-identity.session.uid",
+                    "object": "x-ocsf-identity"
                 }
             },
-            "is_system": {
-                "key": "process.extensions.x-ocsf-process-ext.is_system",
-                "object": "process"
-            },
-            "mime_type": {
-                "key": "process.mime_type",
-                "object": "process"
-            },
-            "modified_time": {
-                "key": "process.extensions.x-ocsf-process-ext.modified_time",
-                "object": "process"
-            },
-            "modifier": {
+            "user": {
                 "account_type": {
                     "key": "user-account.account_type",
-                    "object": "modifier-user-account"
+                    "object": "user"
                 },
                 "account_type_id": {
-                    "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                    "object": "modifier-user-account"
+                    "key": "user-account.extensions.aws-account-ext.account_type_id",
+                    "object": "user",
+                    "transformer": "ToInteger"
                 },
                 "account_uid": {
-                    "key": "user-account.extensions.x-accessor-ext.account_uid",
-                    "object": "modifier-user-account"
+                    "key": "user-account.user_id",
+                    "object": "user"
                 },
                 "credential_uid": {
-                    "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                    "object": "modifier-user-account"
+                    "key": "user-account.extensions.aws-account-ext.credential_uid",
+                    "object": "user"
                 },
                 "domain": {
-                    "key": "user-account.extensions.x-accessor-ext.domain",
-                    "object": "modifier-user-account"
+                    "key": "user-account.extensions.aws-account-ext.domain",
+                    "object": "user"
                 },
                 "email_addr": {
                     "key": "email-addr.value",
-                    "object": "modifier-email-addr"
+                    "object": "email_addr"
                 },
                 "groups": {
                     "desc": {
-                        "key": "user-account.extensions.x-accessor-ext.group_desc",
-                        "object": "modifier-user-account"
+                        "key": "user-account.extensions.aws-account-ext.group_desc",
+                        "object": "user"
                     },
                     "name": {
-                        "key": "user-account.extensions.x-accessor-ext.group_name",
-                        "object": "modifier-user-account"
+                        "key": "user-account.extensions.aws-account-ext.group_name",
+                        "object": "user"
                     },
                     "privileges": {
-                        "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                        "object": "modifier-user-account"
+                        "key": "user-account.extensions.aws-account-ext.group_privileges",
+                        "object": "user"
                     },
                     "type": {
-                        "key": "user-account.extensions.x-accessor-ext.group_type",
-                        "object": "modifier-user-account"
+                        "key": "user-account.extensions.aws-account-ext.group_type",
+                        "object": "user"
                     },
                     "uid": {
-                        "key": "user-account.extensions.x-accessor-ext.group_uid",
-                        "object": "modifier-user-account"
+                        "key": "user-account.extensions.aws-account-ext.group_uid",
+                        "object": "user"
                     }
                 },
                 "name": {
                     "key": "user-account.display_name",
-                    "object": "modifier-user-account"
+                    "object": "user"
                 },
                 "org_uid": {
-                    "key": "user-account.extensions.x-accessor-ext.org_uid",
-                    "object": "modifier-user-account"
+                    "key": "user-account.extensions.aws-account-ext.org_uid",
+                    "object": "user"
                 },
                 "session_uid": {
-                    "key": "user-account.extensions.x-accessor-ext.session_uid",
-                    "object": "modifier-user-account"
+                    "key": "user-account.extensions.aws-account-ext.session_uid",
+                    "object": "user"
                 },
                 "session_uuid": {
-                    "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                    "object": "modifier-user-account"
+                    "key": "user-account.extensions.aws-account-ext.session_uuid",
+                    "object": "user"
                 },
                 "type": {
-                    "key": "user-account.extensions.x-accessor-ext.type",
-                    "object": "modifier-user-account"
+                    "key": "user-account.extensions.aws-account-ext.type",
+                    "object": "user"
                 },
                 "type_id": {
-                    "key": "user-account.extensions.x-accessor-ext.type_id",
-                    "object": "modifier-user-account"
+                    "key": "user-account.extensions.aws-account-ext.type_id",
+                    "object": "user",
+                    "transformer": "ToInteger"
                 },
                 "uid": {
-                    "key": "user-account.user_id",
-                    "object": "modifier-user-account"
+                    "key": "user-account.extensions.aws-account-ext.uid",
+                    "object": "user"
                 },
                 "uuid": {
-                    "key": "user-account.extensions.x-accessor-ext.uuid",
-                    "object": "modifier-user-account"
+                    "key": "user-account.extensions.aws-account-ext.uuid",
+                    "object": "user"
                 }
+            }
+        },
+        "malware": {
+            "classification_ids": {
+                "key": "x-ocsf-malware.classification_ids",
+                "object": "malware"
             },
-            "name": [
-                {
-                    "key": "file.name",
-                    "object": "file"
-                },
-                {
-                    "key": "process.binary_ref",
-                    "object": "process",
-                    "references": "file"
-                }
-            ],
-            "owner": {
-                "account_type": {
-                    "key": "user-account.account_type",
-                    "object": "owner-user-account"
-                },
-                "account_type_id": {
-                    "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                    "object": "owner-user-account"
+            "classifications": {
+                "key": "x-ocsf-malware.classifications",
+                "object": "malware"
+            },
+            "cves": {
+                "created_time": {
+                    "key": "x-ocsf-malware.created_time",
+                    "object": "malware"
                 },
-                "account_uid": {
-                    "key": "user-account.extensions.x-accessor-ext.account_uid",
-                    "object": "owner-user-account"
+                "cvss": {
+                    "base_score": {
+                        "key": "x-ocsf-malware.base_score",
+                        "object": "malware"
+                    },
+                    "depth": {
+                        "key": "x-ocsf-malware.depth",
+                        "object": "malware"
+                    },
+                    "metrics": {
+                        "name": {
+                            "key": "x-ocsf-malware.name",
+                            "object": "malware"
+                        },
+                        "value": {
+                            "key": "x-ocsf-malware.value",
+                            "object": "malware"
+                        }
+                    },
+                    "overall_score": {
+                        "key": "x-ocsf-malware.overall_score",
+                        "object": "malware"
+                    },
+                    "severity": {
+                        "key": "x-ocsf-malware.severity",
+                        "object": "malware"
+                    },
+                    "vector_string": {
+                        "key": "x-ocsf-malware.vector_string",
+                        "object": "malware"
+                    },
+                    "version": {
+                        "key": "x-ocsf-malware.version",
+                        "object": "malware"
+                    }
                 },
-                "credential_uid": {
-                    "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                    "object": "owner-user-account"
+                "cwe_uid": {
+                    "key": "x-ocsf-malware.cwe_uid",
+                    "object": "malware"
                 },
-                "domain": {
-                    "key": "user-account.extensions.x-accessor-ext.domain",
-                    "object": "owner-user-account"
+                "cwe_url": {
+                    "key": "x-ocsf-malware.cwe_url",
+                    "object": "malware"
                 },
-                "email_addr": {
-                    "key": "email-addr.value",
-                    "object": "owner-user-account"
+                "modified_time": {
+                    "key": "x-ocsf-malware.modified_time",
+                    "object": "malware"
                 },
-                "groups": {
-                    "desc": {
-                        "key": "user-account.extensions.x-accessor-ext.group_desc",
-                        "object": "owner-user-account"
+                "product": {
+                    "feature": {
+                        "name": {
+                            "key": "software.extensions.x-ocsf-product-ext.feature_name",
+                            "object": "malware-software"
+                        },
+                        "uid": {
+                            "key": "software.extensions.x-ocsf-product-ext.feature_uid",
+                            "object": "malware-software"
+                        },
+                        "version": {
+                            "key": "software.extensions.x-ocsf-product-ext.feature_version",
+                            "object": "malware-software"
+                        }
                     },
-                    "name": {
-                        "key": "user-account.extensions.x-accessor-ext.group_name",
-                        "object": "owner-user-account"
+                    "lang": {
+                        "key": "software.languages",
+                        "object": "malware-software"
                     },
-                    "privileges": {
-                        "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                        "object": "owner-user-account"
+                    "name": {
+                        "key": "software.name",
+                        "object": "malware-software"
                     },
-                    "type": {
-                        "key": "user-account.extensions.x-accessor-ext.group_type",
-                        "object": "owner-user-account"
+                    "path": {
+                        "key": "software.extensions.x-ocsf-product-ext.installed_path",
+                        "object": "malware-software"
                     },
                     "uid": {
-                        "key": "user-account.extensions.x-accessor-ext.group_uid",
-                        "object": "owner-user-account"
+                        "key": "software.extensions.x-ocsf-product-ext.product_uid",
+                        "object": "malware-software"
+                    },
+                    "vendor_name": {
+                        "key": "software.vendor",
+                        "object": "malware-software"
+                    },
+                    "version": {
+                        "key": "software.version",
+                        "object": "malware-software"
                     }
                 },
-                "name": {
-                    "key": "user-account.display_name",
-                    "object": "owner-user-account"
-                },
-                "org_uid": {
-                    "key": "user-account.extensions.x-accessor-ext.org_uid",
-                    "object": "owner-user-account"
-                },
-                "session_uid": {
-                    "key": "user-account.extensions.x-accessor-ext.session_uid",
-                    "object": "owner-user-account"
-                },
-                "session_uuid": {
-                    "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                    "object": "owner-user-account"
-                },
                 "type": {
-                    "key": "user-account.extensions.x-accessor-ext.type",
-                    "object": "owner-user-account"
-                },
-                "type_id": {
-                    "key": "user-account.extensions.x-accessor-ext.type_id",
-                    "object": "owner-user-account"
+                    "key": "x-ocsf-malware.type",
+                    "object": "malware"
                 },
                 "uid": {
-                    "key": "user-account.user_id",
-                    "object": "owner-user-account"
-                },
-                "uuid": {
-                    "key": "user-account.extensions.x-accessor-ext.uuid",
-                    "object": "owner-user-account"
+                    "key": "x-ocsf-malware.uid",
+                    "object": "malware"
                 }
             },
-            "parent_folder": [
-                {
-                    "key": "directory.path",
-                    "object": "directory"
-                },
-                {
-                    "key": "file.parent_directory_ref",
-                    "object": "file",
-                    "references": "directory"
-                }
-            ],
+            "name": {
+                "key": "x-ocsf-malware.name",
+                "object": "malware"
+            },
             "path": {
-                "key": "file.extensions.x-ocsf-file-ext.path",
-                "object": "file"
+                "key": "x-ocsf-malware.path",
+                "object": "malware"
+            },
+            "provider": {
+                "key": "x-ocsf-malware.provider",
+                "object": "malware"
+            },
+            "uid": {
+                "key": "x-ocsf-malware.uid",
+                "object": "malware"
+            }
+        },
+        "message": {
+            "key": "x-ocsf-cloud.message",
+            "object": "ocsf_cloud_api"
+        },
+        "metadata": {
+            "correlation_uid": {
+                "key": "x-ocsf-metadata.correlation_uid",
+                "object": "metadata"
+            },
+            "labels": {
+                "key": "x-ocsf-metadata.labels",
+                "object": "metadata"
+            },
+            "logged_time": {
+                "key": "x-ocsf-metadata.logged_time",
+                "object": "metadata"
+            },
+            "modified_time": {
+                "key": "x-ocsf-metadata.modified_time",
+                "object": "metadata"
+            },
+            "processed_time": {
+                "key": "x-ocsf-metadata.processed_time",
+                "object": "metadata"
             },
             "product": {
                 "feature": {
                     "name": {
                         "key": "software.extensions.x-ocsf-product-ext.feature_name",
-                        "object": "file1-software"
+                        "object": "metadata-software"
                     },
                     "uid": {
                         "key": "software.extensions.x-ocsf-product-ext.feature_uid",
-                        "object": "file1-software"
+                        "object": "metadata-software"
                     },
                     "version": {
                         "key": "software.extensions.x-ocsf-product-ext.feature_version",
-                        "object": "file1-software"
+                        "object": "metadata-software"
                     }
                 },
                 "lang": {
                     "key": "software.languages",
-                    "object": "file1-software"
+                    "object": "metadata-software"
                 },
                 "name": {
                     "key": "software.name",
-                    "object": "file1-software"
+                    "object": "metadata-software"
                 },
                 "path": {
                     "key": "software.extensions.x-ocsf-product-ext.installed_path",
-                    "object": "file1-software"
+                    "object": "metadata-software"
                 },
                 "uid": {
                     "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                    "object": "file1-software"
+                    "object": "metadata-software"
                 },
                 "vendor_name": {
                     "key": "software.vendor",
-                    "object": "file1-software"
+                    "object": "metadata-software"
                 },
                 "version": {
                     "key": "software.version",
-                    "object": "file1-software"
+                    "object": "metadata-software"
                 }
             },
-            "security_descriptor": {
-                "key": "file.extensions.x-ocsf-file-ext.security_descriptor",
-                "object": "file"
-            },
-            "signature": {
-                "key": "file.extensions.x-ocsf-file-ext.signature",
-                "object": "file"
+            "sequence": {
+                "key": "x-ocsf-metadata.sequence",
+                "object": "metadata",
+                "transformer": "ToInteger"
             },
-            "size": {
-                "key": "file.size",
-                "object": "file"
+            "uid": {
+                "key": "x-ocsf-metadata.uid",
+                "object": "metadata"
             },
+            "version": {
+                "key": "x-ocsf-metadata.version",
+                "object": "metadata"
+            }
+        },
+        "observables": {
+            "name": [
+                {
+                    "key": "x-ibm-observables.name",
+                    "object": "observables"
+                },
+                {
+                    "key": "x-ibm-finding.ioc_refs",
+                    "object": "ibm_finding",
+                    "references": [
+                        "observables"
+                    ]
+                }
+            ],
             "type": {
-                "key": "file.extensions.x-ocsf-file-ext.type",
-                "object": "file"
+                "key": "x-ibm-observables.finding_type",
+                "object": "observables"
             },
             "type_id": {
-                "key": "file.extensions.x-ocsf-file-ext.type_id",
-                "object": "file"
-            },
-            "uid": {
-                "key": "file.extensions.x-ocsf-file-ext.uid",
-                "object": "file"
-            },
-            "version": {
-                "key": "file.extensions.x-ocsf-file-ext.version",
-                "object": "file"
+                "key": "x-ibm-observables.alert_id",
+                "object": "observables",
+                "transformer": "ToInteger"
             },
-            "xattributes": {
-                "key": "process.extensions.x-ocsf-process-ext.xattributes",
-                "object": "process"
+            "value": {
+                "key": "x-ibm-observables.description",
+                "object": "observables"
             }
         },
-        "integrity": {
-            "key": "process.extensions.x-ocsf-process-ext.integrity",
-            "object": "process"
-        },
-        "integrity_id": {
-            "key": "process.extensions.x-ocsf-process-ext.integrity_id",
-            "object": "process"
-        },
-        "lineage": {
-            "key": "process.extensions.x-ocsf-process-ext.lineage",
-            "object": "process"
-        },
-        "loaded_modules": {
-            "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
-            "object": "process"
-        },
-        "name": {
-            "key": "process.name",
-            "object": "process"
-        },
-        "parent_process": {
+        "process": {
             "cmd_line": {
                 "key": "process.command_line",
-                "object": "parent-process"
+                "object": "process"
             },
             "created_time": {
                 "key": "process.created",
-                "object": "parent-process"
+                "object": "process"
             },
             "file": {
                 "accessed_time": {
                     "key": "file.accessed",
-                    "object": "parent-file"
+                    "object": "file"
                 },
                 "accessor": {
                     "account_type": {
                         "key": "user-account.account_type",
-                        "object": "parent-accessor-user-account"
+                        "object": "accessor-user-account"
                     },
                     "account_type_id": {
                         "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                        "object": "parent-accessor-user-account"
+                        "object": "accessor-user-account"
                     },
                     "account_uid": {
                         "key": "user-account.extensions.x-accessor-ext.account_uid",
-                        "object": "parent-accessor-user-account"
+                        "object": "accessor-user-account"
                     },
                     "credential_uid": {
                         "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                        "object": "parent-accessor-user-account"
+                        "object": "accessor-user-account"
                     },
                     "domain": {
                         "key": "user-account.extensions.x-accessor-ext.domain",
-                        "object": "parent-accessor-user-account"
+                        "object": "accessor-user-account"
                     },
                     "email_addr": {
                         "key": "email-addr.value",
-                        "object": "parent-email-addr"
+                        "object": "email-addr"
                     },
                     "groups": {
                         "desc": {
                             "key": "user-account.extensions.x-accessor-ext.group_desc",
-                            "object": "parent-accessor-user-account"
+                            "object": "accessor-user-account"
                         },
                         "name": {
                             "key": "user-account.extensions.x-accessor-ext.group_name",
-                            "object": "parent-accessor-user-account"
+                            "object": "accessor-user-account"
                         },
                         "privileges": {
                             "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                            "object": "parent-accessor-user-account"
+                            "object": "accessor-user-account"
                         },
                         "type": {
                             "key": "user-account.extensions.x-accessor-ext.group_type",
-                            "object": "parent-accessor-user-account"
+                            "object": "accessor-user-account"
                         },
                         "uid": {
                             "key": "user-account.extensions.x-accessor-ext.group_uid",
-                            "object": "parent-accessor-user-account"
+                            "object": "accessor-user-account"
                         }
                     },
                     "name": {
                         "key": "user-account.display_name",
-                        "object": "parent-accessor-user-account"
+                        "object": "accessor-user-account"
                     },
                     "org_uid": {
                         "key": "user-account.extensions.x-accessor-ext.org_uid",
-                        "object": "parent-accessor-user-account"
+                        "object": "accessor-user-account"
                     },
                     "session_uid": {
                         "key": "user-account.extensions.x-accessor-ext.session_uid",
-                        "object": "parent-accessor-user-account"
+                        "object": "accessor-user-account"
                     },
                     "session_uuid": {
                         "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                        "object": "parent-accessor-user-account"
+                        "object": "accessor-user-account"
                     },
                     "type": {
                         "key": "user-account.extensions.x-accessor-ext.type",
-                        "object": "parent-accessor-user-account"
+                        "object": "accessor-user-account"
                     },
                     "type_id": {
                         "key": "user-account.extensions.x-accessor-ext.type_id",
-                        "object": "parent-accessor-user-account"
+                        "object": "accessor-user-account"
                     },
                     "uid": {
                         "key": "user-account.user_id",
-                        "object": "parent-accessor-user-account"
+                        "object": "accessor-user-account"
                     },
                     "uuid": {
                         "key": "user-account.extensions.x-accessor-ext.uuid",
-                        "object": "parent-accessor-user-account"
+                        "object": "accessor-user-account"
                     }
                 },
                 "attributes": {
                     "key": "file.extensions.x-ocsf-file-ext.attributes",
-                    "object": "parent-file"
+                    "object": "file"
                 },
                 "company_name": {
                     "key": "file.extensions.x-ocsf-file-ext.company_name",
-                    "object": "parent-file"
+                    "object": "file"
                 },
                 "confidentiality": {
                     "key": "file.extensions.x-ocsf-file-ext.confidentiality",
-                    "object": "parent-file"
+                    "object": "file"
                 },
                 "confidentiality_id": {
                     "key": "file.extensions.x-ocsf-file-ext.confidentiality_id",
-                    "object": "parent-file"
+                    "object": "file"
                 },
                 "created_time": {
                     "key": "file.created",
-                    "object": "parent-file"
+                    "object": "file"
                 },
                 "creator": {
                     "account_type": {
                         "key": "user-account.account_type",
-                        "object": "parent-creator-user-account"
+                        "object": "creator-user-account"
                     },
                     "account_type_id": {
                         "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                        "object": "parent-creator-user-account"
+                        "object": "creator-user-account"
                     },
                     "account_uid": {
                         "key": "user-account.extensions.x-accessor-ext.account_uid",
-                        "object": "parent-creator-user-account"
+                        "object": "creator-user-account"
                     },
                     "credential_uid": {
                         "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                        "object": "parent-creator-user-account"
+                        "object": "creator-user-account"
                     },
                     "domain": {
                         "key": "user-account.extensions.x-accessor-ext.domain",
-                        "object": "parent-creator-user-account"
+                        "object": "creator-user-account"
                     },
                     "email_addr": {
                         "key": "email-addr.value",
-                        "object": "parent-creator-email-addr"
+                        "object": "creator-email-addr"
                     },
                     "groups": {
                         "desc": {
                             "key": "user-account.extensions.x-accessor-ext.group_desc",
-                            "object": "parent-creator-user-account"
+                            "object": "creator-user-account"
                         },
                         "name": {
                             "key": "user-account.extensions.x-accessor-ext.group_name",
-                            "object": "parent-creator-user-account"
+                            "object": "creator-user-account"
                         },
                         "privileges": {
                             "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                            "object": "parent-creator-user-account"
+                            "object": "creator-user-account"
                         },
                         "type": {
                             "key": "user-account.extensions.x-accessor-ext.group_type",
-                            "object": "parent-creator-user-account"
+                            "object": "creator-user-account"
                         },
                         "uid": {
                             "key": "user-account.extensions.x-accessor-ext.group_uid",
-                            "object": "parent-creator-user-account"
+                            "object": "creator-user-account"
                         }
                     },
                     "name": {
                         "key": "user-account.display_name",
-                        "object": "parent-creator-user-account"
+                        "object": "creator-user-account"
                     },
                     "org_uid": {
                         "key": "user-account.extensions.x-accessor-ext.org_uid",
-                        "object": "parent-creator-user-account"
+                        "object": "creator-user-account"
                     },
                     "session_uid": {
                         "key": "user-account.extensions.x-accessor-ext.session_uid",
-                        "object": "parent-creator-user-account"
+                        "object": "creator-user-account"
                     },
                     "session_uuid": {
                         "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                        "object": "parent-creator-user-account"
+                        "object": "creator-user-account"
                     },
                     "type": {
                         "key": "user-account.extensions.x-accessor-ext.type",
-                        "object": "parent-creator-user-account"
+                        "object": "creator-user-account"
                     },
                     "type_id": {
                         "key": "user-account.extensions.x-accessor-ext.type_id",
-                        "object": "parent-creator-user-account"
+                        "object": "creator-user-account"
                     },
                     "uid": {
                         "key": "user-account.user_id",
-                        "object": "parent-creator-user-account"
+                        "object": "creator-user-account"
                     },
                     "uuid": {
                         "key": "user-account.extensions.x-accessor-ext.uuid",
-                        "object": "parent-creator-user-account"
+                        "object": "creator-user-account"
                     }
                 },
                 "desc": {
                     "key": "file.extensions.x-ocsf-file-ext.description",
-                    "object": "parent-file"
+                    "object": "file"
                 },
                 "hashes": {
                     "CTPH": {
                         "key": "file.hashes.CTPH",
-                        "object": "parent-file"
+                        "object": "file"
                     },
                     "MD5": {
                         "key": "file.hashes.MD5",
-                        "object": "parent-file"
+                        "object": "file"
                     },
                     "Other": {
                         "key": "file.hashes.Other",
-                        "object": "parent-file"
+                        "object": "file"
                     },
                     "SHA-1": {
                         "key": "file.hashes.SHA-1",
-                        "object": "parent-file"
+                        "object": "file"
                     },
                     "SHA-256": {
                         "key": "file.hashes.SHA-256",
-                        "object": "parent-file"
+                        "object": "file"
                     },
                     "SHA-512": {
                         "key": "file.hashes.SHA-512",
-                        "object": "parent-file"
+                        "object": "file"
                     },
                     "Unknown": {
                         "key": "file.hashes.Unknown",
-                        "object": "parent-file"
+                        "object": "file"
                     }
                 },
                 "is_system": {
                     "key": "process.extensions.x-ocsf-process-ext.is_system",
-                    "object": "parent-process"
+                    "object": "process"
                 },
                 "mime_type": {
                     "key": "process.mime_type",
-                    "object": "parent-process"
+                    "object": "process"
                 },
                 "modified_time": {
                     "key": "process.extensions.x-ocsf-process-ext.modified_time",
-                    "object": "parent-process"
+                    "object": "process"
                 },
                 "modifier": {
                     "account_type": {
                         "key": "user-account.account_type",
-                        "object": "parent-modifier-user-account"
+                        "object": "modifier-user-account"
                     },
                     "account_type_id": {
                         "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                        "object": "parent-modifier-user-account"
+                        "object": "modifier-user-account"
                     },
                     "account_uid": {
                         "key": "user-account.extensions.x-accessor-ext.account_uid",
-                        "object": "parent-modifier-user-account"
+                        "object": "modifier-user-account"
                     },
                     "credential_uid": {
                         "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                        "object": "parent-modifier-user-account"
+                        "object": "modifier-user-account"
                     },
                     "domain": {
                         "key": "user-account.extensions.x-accessor-ext.domain",
-                        "object": "parent-modifier-user-account"
+                        "object": "modifier-user-account"
                     },
                     "email_addr": {
                         "key": "email-addr.value",
-                        "object": "parent-modifier-email-addr"
+                        "object": "modifier-email-addr"
                     },
                     "groups": {
                         "desc": {
                             "key": "user-account.extensions.x-accessor-ext.group_desc",
-                            "object": "parent-modifier-user-account"
+                            "object": "modifier-user-account"
                         },
                         "name": {
                             "key": "user-account.extensions.x-accessor-ext.group_name",
-                            "object": "parent-modifier-user-account"
+                            "object": "modifier-user-account"
                         },
                         "privileges": {
                             "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                            "object": "parent-modifier-user-account"
+                            "object": "modifier-user-account"
                         },
                         "type": {
                             "key": "user-account.extensions.x-accessor-ext.group_type",
-                            "object": "parent-modifier-user-account"
+                            "object": "modifier-user-account"
                         },
                         "uid": {
                             "key": "user-account.extensions.x-accessor-ext.group_uid",
-                            "object": "parent-modifier-user-account"
+                            "object": "modifier-user-account"
                         }
                     },
                     "name": {
                         "key": "user-account.display_name",
-                        "object": "parent-modifier-user-account"
+                        "object": "modifier-user-account"
                     },
                     "org_uid": {
                         "key": "user-account.extensions.x-accessor-ext.org_uid",
-                        "object": "parent-modifier-user-account"
+                        "object": "modifier-user-account"
                     },
                     "session_uid": {
                         "key": "user-account.extensions.x-accessor-ext.session_uid",
-                        "object": "parent-modifier-user-account"
+                        "object": "modifier-user-account"
                     },
                     "session_uuid": {
                         "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                        "object": "parent-modifier-user-account"
+                        "object": "modifier-user-account"
                     },
                     "type": {
                         "key": "user-account.extensions.x-accessor-ext.type",
-                        "object": "parent-modifier-user-account"
+                        "object": "modifier-user-account"
                     },
                     "type_id": {
                         "key": "user-account.extensions.x-accessor-ext.type_id",
-                        "object": "parent-modifier-user-account"
+                        "object": "modifier-user-account"
                     },
                     "uid": {
                         "key": "user-account.user_id",
-                        "object": "parent-modifier-user-account"
+                        "object": "modifier-user-account"
                     },
                     "uuid": {
                         "key": "user-account.extensions.x-accessor-ext.uuid",
-                        "object": "parent-modifier-user-account"
+                        "object": "modifier-user-account"
                     }
                 },
                 "name": [
                     {
                         "key": "file.name",
-                        "object": "parent-file"
+                        "object": "file"
                     },
                     {
                         "key": "process.binary_ref",
-                        "object": "parent-process",
-                        "references": "parent-file"
+                        "object": "process",
+                        "references": "file"
                     }
                 ],
                 "owner": {
                     "account_type": {
                         "key": "user-account.account_type",
-                        "object": "parent-owner-user-account"
+                        "object": "owner-user-account"
                     },
                     "account_type_id": {
                         "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                        "object": "parent-owner-user-account"
+                        "object": "owner-user-account"
                     },
                     "account_uid": {
                         "key": "user-account.extensions.x-accessor-ext.account_uid",
-                        "object": "parent-owner-user-account"
+                        "object": "owner-user-account"
                     },
                     "credential_uid": {
                         "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                        "object": "parent-owner-user-account"
+                        "object": "owner-user-account"
                     },
                     "domain": {
                         "key": "user-account.extensions.x-accessor-ext.domain",
-                        "object": "parent-owner-user-account"
+                        "object": "owner-user-account"
                     },
                     "email_addr": {
                         "key": "email-addr.value",
-                        "object": "parent-owner-email-addr"
+                        "object": "owner-user-account"
                     },
                     "groups": {
                         "desc": {
                             "key": "user-account.extensions.x-accessor-ext.group_desc",
-                            "object": "parent-owner-user-account"
+                            "object": "owner-user-account"
                         },
                         "name": {
                             "key": "user-account.extensions.x-accessor-ext.group_name",
-                            "object": "parent-owner-user-account"
+                            "object": "owner-user-account"
                         },
                         "privileges": {
                             "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                            "object": "parent-owner-user-account"
+                            "object": "owner-user-account"
                         },
                         "type": {
                             "key": "user-account.extensions.x-accessor-ext.group_type",
-                            "object": "parent-owner-user-account"
+                            "object": "owner-user-account"
                         },
                         "uid": {
                             "key": "user-account.extensions.x-accessor-ext.group_uid",
-                            "object": "parent-owner-user-account"
+                            "object": "owner-user-account"
                         }
                     },
                     "name": {
                         "key": "user-account.display_name",
-                        "object": "parent-owner-user-account"
+                        "object": "owner-user-account"
                     },
                     "org_uid": {
                         "key": "user-account.extensions.x-accessor-ext.org_uid",
-                        "object": "parent-owner-user-account"
+                        "object": "owner-user-account"
                     },
                     "session_uid": {
                         "key": "user-account.extensions.x-accessor-ext.session_uid",
-                        "object": "parent-owner-user-account"
+                        "object": "owner-user-account"
                     },
                     "session_uuid": {
                         "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                        "object": "parent-owner-user-account"
+                        "object": "owner-user-account"
                     },
                     "type": {
                         "key": "user-account.extensions.x-accessor-ext.type",
-                        "object": "parent-owner-user-account"
+                        "object": "owner-user-account"
                     },
                     "type_id": {
                         "key": "user-account.extensions.x-accessor-ext.type_id",
-                        "object": "parent-owner-user-account"
+                        "object": "owner-user-account"
                     },
                     "uid": {
                         "key": "user-account.user_id",
-                        "object": "parent-owner-user-account"
+                        "object": "owner-user-account"
                     },
                     "uuid": {
                         "key": "user-account.extensions.x-accessor-ext.uuid",
-                        "object": "parent-owner-user-account"
+                        "object": "owner-user-account"
                     }
                 },
                 "parent_folder": [
                     {
                         "key": "directory.path",
-                        "object": "parent-directory"
+                        "object": "directory"
                     },
                     {
                         "key": "file.parent_directory_ref",
-                        "object": "parent-file",
-                        "references": "parent-directory"
+                        "object": "file",
+                        "references": "directory"
                     }
                 ],
                 "path": {
                     "key": "file.extensions.x-ocsf-file-ext.path",
-                    "object": "parent-file"
+                    "object": "file"
                 },
                 "product": {
                     "feature": {
                         "name": {
                             "key": "software.extensions.x-ocsf-product-ext.feature_name",
-                            "object": "file-software"
+                            "object": "file1-software"
                         },
                         "uid": {
                             "key": "software.extensions.x-ocsf-product-ext.feature_uid",
-                            "object": "file-software"
+                            "object": "file1-software"
                         },
                         "version": {
                             "key": "software.extensions.x-ocsf-product-ext.feature_version",
-                            "object": "file-software"
+                            "object": "file1-software"
                         }
                     },
                     "lang": {
                         "key": "software.languages",
-                        "object": "file-software"
+                        "object": "file1-software"
                     },
                     "name": {
                         "key": "software.name",
-                        "object": "file-software"
+                        "object": "file1-software"
                     },
                     "path": {
                         "key": "software.extensions.x-ocsf-product-ext.installed_path",
-                        "object": "file-software"
+                        "object": "file1-software"
                     },
                     "uid": {
                         "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                        "object": "file-software"
+                        "object": "file1-software"
                     },
                     "vendor_name": {
                         "key": "software.vendor",
-                        "object": "file-software"
+                        "object": "file1-software"
                     },
                     "version": {
                         "key": "software.version",
-                        "object": "file-software"
+                        "object": "file1-software"
                     }
                 },
                 "security_descriptor": {
                     "key": "file.extensions.x-ocsf-file-ext.security_descriptor",
-                    "object": "parent-file"
+                    "object": "file"
                 },
                 "signature": {
                     "key": "file.extensions.x-ocsf-file-ext.signature",
-                    "object": "parent-file"
+                    "object": "file"
                 },
                 "size": {
                     "key": "file.size",
-                    "object": "parent-file"
+                    "object": "file"
                 },
                 "type": {
                     "key": "file.extensions.x-ocsf-file-ext.type",
-                    "object": "parent-file"
+                    "object": "file"
                 },
                 "type_id": {
                     "key": "file.extensions.x-ocsf-file-ext.type_id",
-                    "object": "parent-file"
+                    "object": "file"
                 },
                 "uid": {
                     "key": "file.extensions.x-ocsf-file-ext.uid",
-                    "object": "parent-file"
+                    "object": "file"
                 },
                 "version": {
                     "key": "file.extensions.x-ocsf-file-ext.version",
-                    "object": "parent-file"
+                    "object": "file"
                 },
                 "xattributes": {
                     "key": "process.extensions.x-ocsf-process-ext.xattributes",
-                    "object": "parent-process"
+                    "object": "process"
                 }
             },
             "integrity": {
                 "key": "process.extensions.x-ocsf-process-ext.integrity",
-                "object": "parent-process"
+                "object": "process"
             },
             "integrity_id": {
                 "key": "process.extensions.x-ocsf-process-ext.integrity_id",
-                "object": "parent-process"
+                "object": "process"
             },
             "lineage": {
                 "key": "process.extensions.x-ocsf-process-ext.lineage",
-                "object": "parent-process"
+                "object": "process"
             },
             "loaded_modules": {
                 "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
-                "object": "parent-process"
+                "object": "process"
             },
             "name": {
                 "key": "process.name",
-                "object": "parent-process"
+                "object": "process"
+            },
+            "parent_process": {
+                "cmd_line": {
+                    "key": "process.command_line",
+                    "object": "parent-process"
+                },
+                "created_time": {
+                    "key": "process.created",
+                    "object": "parent-process"
+                },
+                "file": {
+                    "accessed_time": {
+                        "key": "file.accessed",
+                        "object": "parent-file"
+                    },
+                    "accessor": {
+                        "account_type": {
+                            "key": "user-account.account_type",
+                            "object": "parent-accessor-user-account"
+                        },
+                        "account_type_id": {
+                            "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                            "object": "parent-accessor-user-account"
+                        },
+                        "account_uid": {
+                            "key": "user-account.extensions.x-accessor-ext.account_uid",
+                            "object": "parent-accessor-user-account"
+                        },
+                        "credential_uid": {
+                            "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                            "object": "parent-accessor-user-account"
+                        },
+                        "domain": {
+                            "key": "user-account.extensions.x-accessor-ext.domain",
+                            "object": "parent-accessor-user-account"
+                        },
+                        "email_addr": {
+                            "key": "email-addr.value",
+                            "object": "parent-email-addr"
+                        },
+                        "groups": {
+                            "desc": {
+                                "key": "user-account.extensions.x-accessor-ext.group_desc",
+                                "object": "parent-accessor-user-account"
+                            },
+                            "name": {
+                                "key": "user-account.extensions.x-accessor-ext.group_name",
+                                "object": "parent-accessor-user-account"
+                            },
+                            "privileges": {
+                                "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                                "object": "parent-accessor-user-account"
+                            },
+                            "type": {
+                                "key": "user-account.extensions.x-accessor-ext.group_type",
+                                "object": "parent-accessor-user-account"
+                            },
+                            "uid": {
+                                "key": "user-account.extensions.x-accessor-ext.group_uid",
+                                "object": "parent-accessor-user-account"
+                            }
+                        },
+                        "name": {
+                            "key": "user-account.display_name",
+                            "object": "parent-accessor-user-account"
+                        },
+                        "org_uid": {
+                            "key": "user-account.extensions.x-accessor-ext.org_uid",
+                            "object": "parent-accessor-user-account"
+                        },
+                        "session_uid": {
+                            "key": "user-account.extensions.x-accessor-ext.session_uid",
+                            "object": "parent-accessor-user-account"
+                        },
+                        "session_uuid": {
+                            "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                            "object": "parent-accessor-user-account"
+                        },
+                        "type": {
+                            "key": "user-account.extensions.x-accessor-ext.type",
+                            "object": "parent-accessor-user-account"
+                        },
+                        "type_id": {
+                            "key": "user-account.extensions.x-accessor-ext.type_id",
+                            "object": "parent-accessor-user-account"
+                        },
+                        "uid": {
+                            "key": "user-account.user_id",
+                            "object": "parent-accessor-user-account"
+                        },
+                        "uuid": {
+                            "key": "user-account.extensions.x-accessor-ext.uuid",
+                            "object": "parent-accessor-user-account"
+                        }
+                    },
+                    "attributes": {
+                        "key": "file.extensions.x-ocsf-file-ext.attributes",
+                        "object": "parent-file"
+                    },
+                    "company_name": {
+                        "key": "file.extensions.x-ocsf-file-ext.company_name",
+                        "object": "parent-file"
+                    },
+                    "confidentiality": {
+                        "key": "file.extensions.x-ocsf-file-ext.confidentiality",
+                        "object": "parent-file"
+                    },
+                    "confidentiality_id": {
+                        "key": "file.extensions.x-ocsf-file-ext.confidentiality_id",
+                        "object": "parent-file"
+                    },
+                    "created_time": {
+                        "key": "file.created",
+                        "object": "parent-file"
+                    },
+                    "creator": {
+                        "account_type": {
+                            "key": "user-account.account_type",
+                            "object": "parent-creator-user-account"
+                        },
+                        "account_type_id": {
+                            "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                            "object": "parent-creator-user-account"
+                        },
+                        "account_uid": {
+                            "key": "user-account.extensions.x-accessor-ext.account_uid",
+                            "object": "parent-creator-user-account"
+                        },
+                        "credential_uid": {
+                            "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                            "object": "parent-creator-user-account"
+                        },
+                        "domain": {
+                            "key": "user-account.extensions.x-accessor-ext.domain",
+                            "object": "parent-creator-user-account"
+                        },
+                        "email_addr": {
+                            "key": "email-addr.value",
+                            "object": "parent-creator-email-addr"
+                        },
+                        "groups": {
+                            "desc": {
+                                "key": "user-account.extensions.x-accessor-ext.group_desc",
+                                "object": "parent-creator-user-account"
+                            },
+                            "name": {
+                                "key": "user-account.extensions.x-accessor-ext.group_name",
+                                "object": "parent-creator-user-account"
+                            },
+                            "privileges": {
+                                "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                                "object": "parent-creator-user-account"
+                            },
+                            "type": {
+                                "key": "user-account.extensions.x-accessor-ext.group_type",
+                                "object": "parent-creator-user-account"
+                            },
+                            "uid": {
+                                "key": "user-account.extensions.x-accessor-ext.group_uid",
+                                "object": "parent-creator-user-account"
+                            }
+                        },
+                        "name": {
+                            "key": "user-account.display_name",
+                            "object": "parent-creator-user-account"
+                        },
+                        "org_uid": {
+                            "key": "user-account.extensions.x-accessor-ext.org_uid",
+                            "object": "parent-creator-user-account"
+                        },
+                        "session_uid": {
+                            "key": "user-account.extensions.x-accessor-ext.session_uid",
+                            "object": "parent-creator-user-account"
+                        },
+                        "session_uuid": {
+                            "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                            "object": "parent-creator-user-account"
+                        },
+                        "type": {
+                            "key": "user-account.extensions.x-accessor-ext.type",
+                            "object": "parent-creator-user-account"
+                        },
+                        "type_id": {
+                            "key": "user-account.extensions.x-accessor-ext.type_id",
+                            "object": "parent-creator-user-account"
+                        },
+                        "uid": {
+                            "key": "user-account.user_id",
+                            "object": "parent-creator-user-account"
+                        },
+                        "uuid": {
+                            "key": "user-account.extensions.x-accessor-ext.uuid",
+                            "object": "parent-creator-user-account"
+                        }
+                    },
+                    "desc": {
+                        "key": "file.extensions.x-ocsf-file-ext.description",
+                        "object": "parent-file"
+                    },
+                    "hashes": {
+                        "CTPH": {
+                            "key": "file.hashes.CTPH",
+                            "object": "parent-file"
+                        },
+                        "MD5": {
+                            "key": "file.hashes.MD5",
+                            "object": "parent-file"
+                        },
+                        "Other": {
+                            "key": "file.hashes.Other",
+                            "object": "parent-file"
+                        },
+                        "SHA-1": {
+                            "key": "file.hashes.SHA-1",
+                            "object": "parent-file"
+                        },
+                        "SHA-256": {
+                            "key": "file.hashes.SHA-256",
+                            "object": "parent-file"
+                        },
+                        "SHA-512": {
+                            "key": "file.hashes.SHA-512",
+                            "object": "parent-file"
+                        },
+                        "Unknown": {
+                            "key": "file.hashes.Unknown",
+                            "object": "parent-file"
+                        }
+                    },
+                    "is_system": {
+                        "key": "process.extensions.x-ocsf-process-ext.is_system",
+                        "object": "parent-process"
+                    },
+                    "mime_type": {
+                        "key": "process.mime_type",
+                        "object": "parent-process"
+                    },
+                    "modified_time": {
+                        "key": "process.extensions.x-ocsf-process-ext.modified_time",
+                        "object": "parent-process"
+                    },
+                    "modifier": {
+                        "account_type": {
+                            "key": "user-account.account_type",
+                            "object": "parent-modifier-user-account"
+                        },
+                        "account_type_id": {
+                            "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                            "object": "parent-modifier-user-account"
+                        },
+                        "account_uid": {
+                            "key": "user-account.extensions.x-accessor-ext.account_uid",
+                            "object": "parent-modifier-user-account"
+                        },
+                        "credential_uid": {
+                            "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                            "object": "parent-modifier-user-account"
+                        },
+                        "domain": {
+                            "key": "user-account.extensions.x-accessor-ext.domain",
+                            "object": "parent-modifier-user-account"
+                        },
+                        "email_addr": {
+                            "key": "email-addr.value",
+                            "object": "parent-modifier-email-addr"
+                        },
+                        "groups": {
+                            "desc": {
+                                "key": "user-account.extensions.x-accessor-ext.group_desc",
+                                "object": "parent-modifier-user-account"
+                            },
+                            "name": {
+                                "key": "user-account.extensions.x-accessor-ext.group_name",
+                                "object": "parent-modifier-user-account"
+                            },
+                            "privileges": {
+                                "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                                "object": "parent-modifier-user-account"
+                            },
+                            "type": {
+                                "key": "user-account.extensions.x-accessor-ext.group_type",
+                                "object": "parent-modifier-user-account"
+                            },
+                            "uid": {
+                                "key": "user-account.extensions.x-accessor-ext.group_uid",
+                                "object": "parent-modifier-user-account"
+                            }
+                        },
+                        "name": {
+                            "key": "user-account.display_name",
+                            "object": "parent-modifier-user-account"
+                        },
+                        "org_uid": {
+                            "key": "user-account.extensions.x-accessor-ext.org_uid",
+                            "object": "parent-modifier-user-account"
+                        },
+                        "session_uid": {
+                            "key": "user-account.extensions.x-accessor-ext.session_uid",
+                            "object": "parent-modifier-user-account"
+                        },
+                        "session_uuid": {
+                            "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                            "object": "parent-modifier-user-account"
+                        },
+                        "type": {
+                            "key": "user-account.extensions.x-accessor-ext.type",
+                            "object": "parent-modifier-user-account"
+                        },
+                        "type_id": {
+                            "key": "user-account.extensions.x-accessor-ext.type_id",
+                            "object": "parent-modifier-user-account"
+                        },
+                        "uid": {
+                            "key": "user-account.user_id",
+                            "object": "parent-modifier-user-account"
+                        },
+                        "uuid": {
+                            "key": "user-account.extensions.x-accessor-ext.uuid",
+                            "object": "parent-modifier-user-account"
+                        }
+                    },
+                    "name": [
+                        {
+                            "key": "file.name",
+                            "object": "parent-file"
+                        },
+                        {
+                            "key": "process.binary_ref",
+                            "object": "parent-process",
+                            "references": "parent-file"
+                        }
+                    ],
+                    "owner": {
+                        "account_type": {
+                            "key": "user-account.account_type",
+                            "object": "parent-owner-user-account"
+                        },
+                        "account_type_id": {
+                            "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                            "object": "parent-owner-user-account"
+                        },
+                        "account_uid": {
+                            "key": "user-account.extensions.x-accessor-ext.account_uid",
+                            "object": "parent-owner-user-account"
+                        },
+                        "credential_uid": {
+                            "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                            "object": "parent-owner-user-account"
+                        },
+                        "domain": {
+                            "key": "user-account.extensions.x-accessor-ext.domain",
+                            "object": "parent-owner-user-account"
+                        },
+                        "email_addr": {
+                            "key": "email-addr.value",
+                            "object": "parent-owner-email-addr"
+                        },
+                        "groups": {
+                            "desc": {
+                                "key": "user-account.extensions.x-accessor-ext.group_desc",
+                                "object": "parent-owner-user-account"
+                            },
+                            "name": {
+                                "key": "user-account.extensions.x-accessor-ext.group_name",
+                                "object": "parent-owner-user-account"
+                            },
+                            "privileges": {
+                                "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                                "object": "parent-owner-user-account"
+                            },
+                            "type": {
+                                "key": "user-account.extensions.x-accessor-ext.group_type",
+                                "object": "parent-owner-user-account"
+                            },
+                            "uid": {
+                                "key": "user-account.extensions.x-accessor-ext.group_uid",
+                                "object": "parent-owner-user-account"
+                            }
+                        },
+                        "name": {
+                            "key": "user-account.display_name",
+                            "object": "parent-owner-user-account"
+                        },
+                        "org_uid": {
+                            "key": "user-account.extensions.x-accessor-ext.org_uid",
+                            "object": "parent-owner-user-account"
+                        },
+                        "session_uid": {
+                            "key": "user-account.extensions.x-accessor-ext.session_uid",
+                            "object": "parent-owner-user-account"
+                        },
+                        "session_uuid": {
+                            "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                            "object": "parent-owner-user-account"
+                        },
+                        "type": {
+                            "key": "user-account.extensions.x-accessor-ext.type",
+                            "object": "parent-owner-user-account"
+                        },
+                        "type_id": {
+                            "key": "user-account.extensions.x-accessor-ext.type_id",
+                            "object": "parent-owner-user-account"
+                        },
+                        "uid": {
+                            "key": "user-account.user_id",
+                            "object": "parent-owner-user-account"
+                        },
+                        "uuid": {
+                            "key": "user-account.extensions.x-accessor-ext.uuid",
+                            "object": "parent-owner-user-account"
+                        }
+                    },
+                    "parent_folder": [
+                        {
+                            "key": "directory.path",
+                            "object": "parent-directory"
+                        },
+                        {
+                            "key": "file.parent_directory_ref",
+                            "object": "parent-file",
+                            "references": "parent-directory"
+                        }
+                    ],
+                    "path": {
+                        "key": "file.extensions.x-ocsf-file-ext.path",
+                        "object": "parent-file"
+                    },
+                    "product": {
+                        "feature": {
+                            "name": {
+                                "key": "software.extensions.x-ocsf-product-ext.feature_name",
+                                "object": "file-software"
+                            },
+                            "uid": {
+                                "key": "software.extensions.x-ocsf-product-ext.feature_uid",
+                                "object": "file-software"
+                            },
+                            "version": {
+                                "key": "software.extensions.x-ocsf-product-ext.feature_version",
+                                "object": "file-software"
+                            }
+                        },
+                        "lang": {
+                            "key": "software.languages",
+                            "object": "file-software"
+                        },
+                        "name": {
+                            "key": "software.name",
+                            "object": "file-software"
+                        },
+                        "path": {
+                            "key": "software.extensions.x-ocsf-product-ext.installed_path",
+                            "object": "file-software"
+                        },
+                        "uid": {
+                            "key": "software.extensions.x-ocsf-product-ext.product_uid",
+                            "object": "file-software"
+                        },
+                        "vendor_name": {
+                            "key": "software.vendor",
+                            "object": "file-software"
+                        },
+                        "version": {
+                            "key": "software.version",
+                            "object": "file-software"
+                        }
+                    },
+                    "security_descriptor": {
+                        "key": "file.extensions.x-ocsf-file-ext.security_descriptor",
+                        "object": "parent-file"
+                    },
+                    "signature": {
+                        "key": "file.extensions.x-ocsf-file-ext.signature",
+                        "object": "parent-file"
+                    },
+                    "size": {
+                        "key": "file.size",
+                        "object": "parent-file"
+                    },
+                    "type": {
+                        "key": "file.extensions.x-ocsf-file-ext.type",
+                        "object": "parent-file"
+                    },
+                    "type_id": {
+                        "key": "file.extensions.x-ocsf-file-ext.type_id",
+                        "object": "parent-file"
+                    },
+                    "uid": {
+                        "key": "file.extensions.x-ocsf-file-ext.uid",
+                        "object": "parent-file"
+                    },
+                    "version": {
+                        "key": "file.extensions.x-ocsf-file-ext.version",
+                        "object": "parent-file"
+                    },
+                    "xattributes": {
+                        "key": "process.extensions.x-ocsf-process-ext.xattributes",
+                        "object": "parent-process"
+                    }
+                },
+                "integrity": {
+                    "key": "process.extensions.x-ocsf-process-ext.integrity",
+                    "object": "parent-process"
+                },
+                "integrity_id": {
+                    "key": "process.extensions.x-ocsf-process-ext.integrity_id",
+                    "object": "parent-process"
+                },
+                "lineage": {
+                    "key": "process.extensions.x-ocsf-process-ext.lineage",
+                    "object": "parent-process"
+                },
+                "loaded_modules": {
+                    "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
+                    "object": "parent-process"
+                },
+                "name": {
+                    "key": "process.name",
+                    "object": "parent-process"
+                },
+                "pid": [
+                    {
+                        "key": "process.pid",
+                        "object": "parent-process"
+                    },
+                    {
+                        "key": "process.child_refs",
+                        "object": "parent-process",
+                        "references": [
+                            "process"
+                        ]
+                    }
+                ],
+                "sandbox": {
+                    "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
+                    "object": "parent-process"
+                },
+                "terminated_time": {
+                    "key": "process.extensions.x-ocsf-process-ext.terminated_time",
+                    "object": "parent-process"
+                },
+                "tid": {
+                    "key": "process.extensions.x-ocsf-process-ext.tid",
+                    "object": "parent-process"
+                },
+                "uid": {
+                    "key": "process.x_unique_id",
+                    "object": "parent-process"
+                },
+                "user": {
+                    "account_type": {
+                        "key": "user-account.account_type",
+                        "object": "parent-process-user-account"
+                    },
+                    "account_type_id": {
+                        "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                        "object": "parent-process-user-account"
+                    },
+                    "account_uid": {
+                        "key": "user-account.extensions.x-accessor-ext.account_uid",
+                        "object": "parent-process-user-account"
+                    },
+                    "credential_uid": {
+                        "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                        "object": "parent-process-user-account"
+                    },
+                    "domain": {
+                        "key": "user-account.extensions.x-accessor-ext.domain",
+                        "object": "parent-process-user-account"
+                    },
+                    "email_addr": {
+                        "key": "email-addr.value",
+                        "object": "parent-process-email-addr"
+                    },
+                    "groups": {
+                        "desc": {
+                            "key": "user-account.extensions.x-accessor-ext.group_desc",
+                            "object": "parent-process-user-account"
+                        },
+                        "name": {
+                            "key": "user-account.extensions.x-accessor-ext.group_name",
+                            "object": "parent-process-user-account"
+                        },
+                        "privileges": {
+                            "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                            "object": "parent-process-user-account"
+                        },
+                        "type": {
+                            "key": "user-account.extensions.x-accessor-ext.group_type",
+                            "object": "parent-process-user-account"
+                        },
+                        "uid": {
+                            "key": "user-account.extensions.x-accessor-ext.group_uid",
+                            "object": "parent-process-user-account"
+                        }
+                    },
+                    "name": {
+                        "key": "user-account.display_name",
+                        "object": "parent-process-user-account"
+                    },
+                    "org_uid": {
+                        "key": "user-account.extensions.x-accessor-ext.org_uid",
+                        "object": "parent-process-user-account"
+                    },
+                    "session_uid": {
+                        "key": "user-account.extensions.x-accessor-ext.session_uid",
+                        "object": "parent-process-user-account"
+                    },
+                    "session_uuid": {
+                        "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                        "object": "parent-process-user-account"
+                    },
+                    "type": {
+                        "key": "user-account.extensions.x-accessor-ext.type",
+                        "object": "parent-process-user-account"
+                    },
+                    "type_id": {
+                        "key": "user-account.extensions.x-accessor-ext.type_id",
+                        "object": "parent-process-user-account"
+                    },
+                    "uid": [
+                        {
+                            "key": "user-account.user_id",
+                            "object": "parent-process-user-account"
+                        },
+                        {
+                            "key": "user-account.creator_user_ref",
+                            "object": "parent-process",
+                            "references": "process-user-account"
+                        }
+                    ],
+                    "uuid": {
+                        "key": "user-account.extensions.x-accessor-ext.uuid",
+                        "object": "parent-process-user-account"
+                    }
+                },
+                "xattributes": {
+                    "key": "process.extensions.x-ocsf-process-ext.xattributes",
+                    "object": "parent-process"
+                }
             },
             "pid": [
                 {
                     "key": "process.pid",
-                    "object": "parent-process"
+                    "object": "process"
                 },
                 {
-                    "key": "process.child_refs",
-                    "object": "parent-process",
+                    "key": "process.parent_ref",
+                    "object": "process",
                     "references": [
-                        "process"
+                        "parent-process"
                     ]
                 }
             ],
             "sandbox": {
                 "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
-                "object": "parent-process"
+                "object": "process"
             },
             "terminated_time": {
                 "key": "process.extensions.x-ocsf-process-ext.terminated_time",
-                "object": "parent-process"
+                "object": "process"
             },
             "tid": {
                 "key": "process.extensions.x-ocsf-process-ext.tid",
-                "object": "parent-process"
+                "object": "process"
             },
             "uid": {
                 "key": "process.x_unique_id",
-                "object": "parent-process"
+                "object": "process"
             },
             "user": {
                 "account_type": {
                     "key": "user-account.account_type",
-                    "object": "parent-process-user-account"
+                    "object": "process-user-account"
                 },
                 "account_type_id": {
                     "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                    "object": "parent-process-user-account"
+                    "object": "process-user-account"
                 },
                 "account_uid": {
                     "key": "user-account.extensions.x-accessor-ext.account_uid",
-                    "object": "parent-process-user-account"
+                    "object": "process-user-account"
                 },
                 "credential_uid": {
                     "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                    "object": "parent-process-user-account"
+                    "object": "process-user-account"
                 },
                 "domain": {
                     "key": "user-account.extensions.x-accessor-ext.domain",
-                    "object": "parent-process-user-account"
+                    "object": "process-user-account"
                 },
                 "email_addr": {
                     "key": "email-addr.value",
-                    "object": "parent-process-email-addr"
+                    "object": "process-email-addr"
                 },
                 "groups": {
                     "desc": {
                         "key": "user-account.extensions.x-accessor-ext.group_desc",
-                        "object": "parent-process-user-account"
+                        "object": "process-user-account"
                     },
                     "name": {
                         "key": "user-account.extensions.x-accessor-ext.group_name",
-                        "object": "parent-process-user-account"
+                        "object": "process-user-account"
                     },
                     "privileges": {
                         "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                        "object": "parent-process-user-account"
+                        "object": "process-user-account"
                     },
                     "type": {
                         "key": "user-account.extensions.x-accessor-ext.group_type",
-                        "object": "parent-process-user-account"
+                        "object": "process-user-account"
                     },
                     "uid": {
                         "key": "user-account.extensions.x-accessor-ext.group_uid",
-                        "object": "parent-process-user-account"
+                        "object": "process-user-account"
                     }
                 },
                 "name": {
                     "key": "user-account.display_name",
-                    "object": "parent-process-user-account"
+                    "object": "process-user-account"
                 },
                 "org_uid": {
                     "key": "user-account.extensions.x-accessor-ext.org_uid",
-                    "object": "parent-process-user-account"
+                    "object": "process-user-account"
                 },
                 "session_uid": {
                     "key": "user-account.extensions.x-accessor-ext.session_uid",
-                    "object": "parent-process-user-account"
+                    "object": "process-user-account"
                 },
                 "session_uuid": {
                     "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                    "object": "parent-process-user-account"
+                    "object": "process-user-account"
                 },
                 "type": {
                     "key": "user-account.extensions.x-accessor-ext.type",
-                    "object": "parent-process-user-account"
+                    "object": "process-user-account"
                 },
                 "type_id": {
                     "key": "user-account.extensions.x-accessor-ext.type_id",
-                    "object": "parent-process-user-account"
+                    "object": "process-user-account"
                 },
                 "uid": [
                     {
                         "key": "user-account.user_id",
-                        "object": "parent-process-user-account"
+                        "object": "process-user-account"
                     },
                     {
                         "key": "user-account.creator_user_ref",
-                        "object": "parent-process",
+                        "object": "process",
                         "references": "process-user-account"
                     }
                 ],
                 "uuid": {
                     "key": "user-account.extensions.x-accessor-ext.uuid",
-                    "object": "parent-process-user-account"
+                    "object": "process-user-account"
                 }
             },
             "xattributes": {
                 "key": "process.extensions.x-ocsf-process-ext.xattributes",
-                "object": "parent-process"
-            }
-        },
-        "pid": [
-            {
-                "key": "process.pid",
                 "object": "process"
-            },
-            {
-                "key": "process.parent_ref",
-                "object": "process",
-                "references": [
-                    "parent-process"
-                ]
             }
-        ],
-        "sandbox": {
-            "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
-            "object": "process"
-        },
-        "terminated_time": {
-            "key": "process.extensions.x-ocsf-process-ext.terminated_time",
-            "object": "process"
-        },
-        "tid": {
-            "key": "process.extensions.x-ocsf-process-ext.tid",
-            "object": "process"
-        },
-        "uid": {
-            "key": "process.x_unique_id",
-            "object": "process"
         },
-        "user": {
-            "account_type": {
-                "key": "user-account.account_type",
-                "object": "process-user-account"
+        "profiles": {
+            "key": "x-ocsf-cloud.profiles",
+            "object": "ocsf_cloud_api"
+        },
+        "raw_data": {
+            "key": "x-ocsf-cloud.raw_data",
+            "object": "ocsf_cloud_api"
+        },
+        "ref_event_code": {
+            "key": "x-ocsf-cloud.ref_event_code",
+            "object": "ocsf_cloud_api"
+        },
+        "ref_event_name": {
+            "key": "x-ocsf-cloud.ref_event_name",
+            "object": "ocsf_cloud_api"
+        },
+        "ref_event_uid": {
+            "key": "x-ocsf-cloud.ref_event_uid",
+            "object": "ocsf_cloud_api"
+        },
+        "ref_time": {
+            "key": "x-ocsf-cloud.ref_time",
+            "object": "ocsf_cloud_api"
+        },
+        "resources": {
+            "account_uid": [
+                {
+                    "key": "x-ocsf-resources.account_uid",
+                    "object": "resources"
+                },
+                {
+                    "key": "x-ocsf-resources.cloud_api_ref",
+                    "object": "resources",
+                    "references": "ocsf_cloud_api"
+                }
+            ],
+            "cloud_partition": {
+                "key": "x-ocsf-resources.cloud_partition",
+                "object": "resources"
             },
-            "account_type_id": {
-                "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                "object": "process-user-account"
+            "criticality": {
+                "key": "x-ocsf-resources.criticality",
+                "object": "resources"
             },
-            "account_uid": {
-                "key": "user-account.extensions.x-accessor-ext.account_uid",
-                "object": "process-user-account"
+            "details": {
+                "key": "x-ocsf-resources.details",
+                "object": "resources"
             },
-            "credential_uid": {
-                "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                "object": "process-user-account"
-            },
-            "domain": {
-                "key": "user-account.extensions.x-accessor-ext.domain",
-                "object": "process-user-account"
-            },
-            "email_addr": {
-                "key": "email-addr.value",
-                "object": "process-email-addr"
+            "group_name": {
+                "key": "x-ocsf-resources.group_name",
+                "object": "resources"
             },
-            "groups": {
-                "desc": {
-                    "key": "user-account.extensions.x-accessor-ext.group_desc",
-                    "object": "process-user-account"
-                },
-                "name": {
-                    "key": "user-account.extensions.x-accessor-ext.group_name",
-                    "object": "process-user-account"
-                },
-                "privileges": {
-                    "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                    "object": "process-user-account"
-                },
-                "type": {
-                    "key": "user-account.extensions.x-accessor-ext.group_type",
-                    "object": "process-user-account"
-                },
-                "uid": {
-                    "key": "user-account.extensions.x-accessor-ext.group_uid",
-                    "object": "process-user-account"
-                }
+            "labels": {
+                "key": "x-ocsf-resources.labels",
+                "object": "resources"
             },
             "name": {
-                "key": "user-account.display_name",
-                "object": "process-user-account"
+                "key": "x-ocsf-resources.name",
+                "object": "resources"
             },
-            "org_uid": {
-                "key": "user-account.extensions.x-accessor-ext.org_uid",
-                "object": "process-user-account"
+            "owner": {
+                "key": "x-ocsf-resources.owner",
+                "object": "resources"
             },
-            "session_uid": {
-                "key": "user-account.extensions.x-accessor-ext.session_uid",
-                "object": "process-user-account"
-            },
-            "session_uuid": {
-                "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                "object": "process-user-account"
+            "region": {
+                "key": "x-ocsf-resources.region",
+                "object": "resources"
             },
             "type": {
-                "key": "user-account.extensions.x-accessor-ext.type",
-                "object": "process-user-account"
+                "key": "x-ocsf-resources.type",
+                "object": "resources"
             },
-            "type_id": {
-                "key": "user-account.extensions.x-accessor-ext.type_id",
-                "object": "process-user-account"
+            "uid": {
+                "key": "x-ocsf-resources.uid",
+                "object": "resources"
+            }
+        },
+        "severity": {
+            "key": "x-ocsf-cloud.severity",
+            "object": "ocsf_cloud_api"
+        },
+        "severity_id": {
+            "key": "x-ibm-finding.severity",
+            "object": "ibm_finding",
+            "transformer": "ToInteger"
+        },
+        "src_endpoint": {
+            "instance_uid": {
+                "key": "x-oca-asset.extensions.x-src-endpoint.instance_uid",
+                "object": "asset"
+            },
+            "interface_uid": {
+                "key": "x-oca-asset.extensions.x-src-endpoint.interface_uid",
+                "object": "asset"
             },
-            "uid": [
+            "intermediate_ips": [
                 {
-                    "key": "user-account.user_id",
-                    "object": "process-user-account"
+                    "key": "ipv4-addr.value",
+                    "object": "src_ipv4",
+                    "transformer": "FilterIPv4List",
+                    "unwrap": true
                 },
                 {
-                    "key": "user-account.creator_user_ref",
-                    "object": "process",
-                    "references": "process-user-account"
+                    "key": "ipv6-addr.value",
+                    "object": "src_ipv6",
+                    "transformer": "FilterIPv6List",
+                    "unwrap": true
+                },
+                {
+                    "key": "x-oca-asset.ip_refs",
+                    "object": "asset",
+                    "references": [
+                        "src_ipv4",
+                        "src_ipv6"
+                    ],
+                    "unwrap": true
+                }
+            ],
+            "ip": [
+                {
+                    "key": "ipv4-addr.value",
+                    "object": "src_ip",
+                    "transformer": "CheckIPv4"
+                },
+                {
+                    "key": "ipv6-addr.value",
+                    "object": "src_ip",
+                    "transformer": "CheckIPv6"
+                },
+                {
+                    "key": "network-traffic.src_ref",
+                    "object": "nt",
+                    "references": "src_ip"
+                },
+                {
+                    "key": "x-ibm-finding.src_ip_ref",
+                    "object": "ibm_finding",
+                    "references": "src_ip"
+                },
+                {
+                    "group": true,
+                    "key": "x-oca-asset.ip_refs",
+                    "object": "host",
+                    "references": [
+                        "src_ip"
+                    ]
+                },
+                {
+                    "key": "x-oca-event.network_ref",
+                    "object": "event",
+                    "references": "nt"
                 }
             ],
-            "uuid": {
-                "key": "user-account.extensions.x-accessor-ext.uuid",
-                "object": "process-user-account"
+            "name": {
+                "key": "x-oca-asset.name",
+                "object": "asset"
+            },
+            "port": {
+                "key": "network-traffic.src_port",
+                "object": "nt",
+                "transformer": "ToInteger"
+            },
+            "subnet_uid": {
+                "key": "x-oca-asset.extensions.x-src-endpoint.subnet_uid",
+                "object": "asset"
+            },
+            "svc_name": {
+                "key": "x-oca-asset.extensions.x-src-endpoint.svc_name",
+                "object": "asset"
+            },
+            "vpc_uid": {
+                "key": "x-oca-asset.extensions.x-src-endpoint.vpc_uid",
+                "object": "asset"
             }
         },
-        "xattributes": {
-            "key": "process.extensions.x-ocsf-process-ext.xattributes",
-            "object": "process"
-        }
-    },
-    "profiles": {
-        "key": "x-ocsf-cloud.profiles",
-        "object": "ocsf_cloud_api"
-    },
-    "raw_data": {
-        "key": "x-ocsf-cloud.raw_data",
-        "object": "ocsf_cloud_api"
-    },
-    "ref_event_code": {
-        "key": "x-ocsf-cloud.ref_event_code",
-        "object": "ocsf_cloud_api"
-    },
-    "ref_event_name": {
-        "key": "x-ocsf-cloud.ref_event_name",
-        "object": "ocsf_cloud_api"
-    },
-    "ref_event_uid": {
-        "key": "x-ocsf-cloud.ref_event_uid",
-        "object": "ocsf_cloud_api"
-    },
-    "ref_time": {
-        "key": "x-ocsf-cloud.ref_time",
-        "object": "ocsf_cloud_api"
-    },
-    "resources": {
-        "account_uid": [
-            {
-                "key": "x-ocsf-resources.account_uid",
-                "object": "resources"
-            },
-            {
-                "key": "x-ocsf-resources.cloud_api_ref",
-                "object": "resources",
-                "references": "ocsf_cloud_api"
-            }
-        ],
-        "cloud_partition": {
-            "key": "x-ocsf-resources.cloud_partition",
-            "object": "resources"
-        },
-        "criticality": {
-            "key": "x-ocsf-resources.criticality",
-            "object": "resources"
-        },
-        "details": {
-            "key": "x-ocsf-resources.details",
-            "object": "resources"
-        },
-        "group_name": {
-            "key": "x-ocsf-resources.group_name",
-            "object": "resources"
-        },
-        "labels": {
-            "key": "x-ocsf-resources.labels",
-            "object": "resources"
+        "start_time": {
+            "cybox": false,
+            "key": "first_observed",
+            "transformer": "EpochToTimestamp"
         },
-        "name": {
-            "key": "x-ocsf-resources.name",
-            "object": "resources"
+        "status": {
+            "key": "x-ocsf-cloud.status",
+            "object": "ocsf_cloud_api"
         },
-        "owner": {
-            "key": "x-ocsf-resources.owner",
-            "object": "resources"
+        "status_code": {
+            "key": "x-ocsf-cloud.status_code",
+            "object": "ocsf_cloud_api"
         },
-        "region": {
-            "key": "x-ocsf-resources.region",
-            "object": "resources"
+        "status_detail": {
+            "key": "x-ocsf-cloud.status_detail",
+            "object": "ocsf_cloud_api"
         },
-        "type": {
-            "key": "x-ocsf-resources.type",
-            "object": "resources"
+        "status_id": {
+            "key": "x-ocsf-cloud.status_id",
+            "object": "ocsf_cloud_api",
+            "transformer": "ToInteger"
         },
-        "uid": {
-            "key": "x-ocsf-resources.uid",
-            "object": "resources"
-        }
-    },
-    "severity": {
-        "key": "x-ocsf-cloud.severity",
-        "object": "ocsf_cloud_api"
-    },
-    "severity_id": {
-        "key": "x-ibm-finding.severity",
-        "object": "ibm_finding",
-        "transformer": "ToInteger"
-    },
-    "src_endpoint": {
-        "instance_uid": {
-            "key": "x-oca-asset.extensions.x-src-endpoint.instance_uid",
-            "object": "asset"
-        },
-        "interface_uid": {
-            "key": "x-oca-asset.extensions.x-src-endpoint.interface_uid",
-            "object": "asset"
+        "time": {
+            "key": "x-oca-event.created",
+            "object": "x_oca_event"
+        },
+        "timezone_offset": {
+            "key": "x-oca-event.timezone",
+            "object": "x_oca_event",
+            "transformer": "ToInteger"
         },
-        "intermediate_ips": [
-            {
-                "key": "ipv4-addr.value",
-                "object": "src_ipv4",
-                "transformer": "FilterIPv4List",
-                "unwrap": true
-            },
-            {
-                "key": "ipv6-addr.value",
-                "object": "src_ipv6",
-                "transformer": "FilterIPv6List",
-                "unwrap": true
-            },
-            {
-                "key": "x-oca-asset.ip_refs",
-                "object": "asset",
-                "references": [
-                    "src_ipv4",
-                    "src_ipv6"
-                ],
-                "unwrap": true
+        "traffic": {
+            "bytes": {
+                "key": "network-traffic.extensions.x-network-ext.bytes",
+                "object": "nt"
+            },
+            "bytes_in": {
+                "key": "network-traffic.dst_byte_count",
+                "object": "nt"
+            },
+            "bytes_out": {
+                "key": "network-traffic.src_byte_count",
+                "object": "nt"
+            },
+            "packets": {
+                "key": "network-traffic.extensions.x-network-ext.packets",
+                "object": "nt"
+            },
+            "packets_in": {
+                "key": "network-traffic.dst_packets",
+                "object": "nt"
+            },
+            "packets_out": {
+                "key": "network-traffic.src_packets",
+                "object": "nt"
             }
-        ],
-        "ip": [
-            {
-                "key": "ipv4-addr.value",
-                "object": "src_ip",
-                "transformer": "CheckIPv4"
-            },
-            {
-                "key": "ipv6-addr.value",
-                "object": "src_ip",
-                "transformer": "CheckIPv6"
-            },
-            {
-                "key": "network-traffic.src_ref",
-                "object": "nt",
-                "references": "src_ip"
-            },
-            {
-                "key": "x-ibm-finding.src_ip_ref",
-                "object": "ibm_finding",
-                "references": "src_ip"
-            },
-            {
-                "group": true,
-                "key": "x-oca-asset.ip_refs",
-                "object": "host",
-                "references": [
-                    "src_ip"
-                ]
-            },
-            {
-                "key": "x-oca-event.network_ref",
-                "object": "event",
-                "references": "nt"
-            }
-        ],
-        "name": {
-            "key": "x-oca-asset.name",
-            "object": "asset"
         },
-        "port": {
-            "key": "network-traffic.src_port",
-            "object": "nt",
+        "type_name": {
+            "key": "x-ocsf-cloud.type_name",
+            "object": "ocsf_cloud_api"
+        },
+        "type_uid": {
+            "key": "x-ocsf-cloud.type_uid",
+            "object": "ocsf_cloud_api",
             "transformer": "ToInteger"
         },
-        "subnet_uid": {
-            "key": "x-oca-asset.extensions.x-src-endpoint.subnet_uid",
-            "object": "asset"
-        },
-        "svc_name": {
-            "key": "x-oca-asset.extensions.x-src-endpoint.svc_name",
-            "object": "asset"
-        },
-        "vpc_uid": {
-            "key": "x-oca-asset.extensions.x-src-endpoint.vpc_uid",
-            "object": "asset"
-        }
-    },
-    "start_time": {
-        "cybox": false,
-        "key": "first_observed",
-        "transformer": "EpochToTimestamp"
-    },
-    "status": {
-        "key": "x-ocsf-cloud.status",
-        "object": "ocsf_cloud_api"
-    },
-    "status_code": {
-        "key": "x-ocsf-cloud.status_code",
-        "object": "ocsf_cloud_api"
-    },
-    "status_detail": {
-        "key": "x-ocsf-cloud.status_detail",
-        "object": "ocsf_cloud_api"
-    },
-    "status_id": {
-        "key": "x-ocsf-cloud.status_id",
-        "object": "ocsf_cloud_api",
-        "transformer": "ToInteger"
-    },
-    "time": {
-        "key": "x-oca-event.created",
-        "object": "x_oca_event"
-    },
-    "timezone_offset": {
-        "key": "x-oca-event.timezone",
-        "object": "x_oca_event",
-        "transformer": "ToInteger"
-    },
-    "traffic": {
-        "bytes": {
-            "key": "network-traffic.extensions.x-network-ext.bytes",
-            "object": "nt"
-        },
-        "bytes_in": {
-            "key": "network-traffic.dst_byte_count",
-            "object": "nt"
-        },
-        "bytes_out": {
-            "key": "network-traffic.src_byte_count",
-            "object": "nt"
-        },
-        "packets": {
-            "key": "network-traffic.extensions.x-network-ext.packets",
-            "object": "nt"
-        },
-        "packets_in": {
-            "key": "network-traffic.dst_packets",
-            "object": "nt"
-        },
-        "packets_out": {
-            "key": "network-traffic.src_packets",
-            "object": "nt"
-        }
-    },
-    "type_name": {
-        "key": "x-ocsf-cloud.type_name",
-        "object": "ocsf_cloud_api"
-    },
-    "type_uid": {
-        "key": "x-ocsf-cloud.type_uid",
-        "object": "ocsf_cloud_api",
-        "transformer": "ToInteger"
-    },
-    "vulnerabilities": {
-        "cve": {
-            "created_time": {
-                "key": "x-ocsf-vulnerabilities.created_time",
-                "object": "vulnerabilities"
-            },
-            "cvss": {
-                "base_score": {
-                    "key": "x-ocsf-vulnerabilities.base_score",
-                    "object": "vulnerabilities"
-                },
-                "depth": {
-                    "key": "x-ocsf-vulnerabilities.depth",
+        "vulnerabilities": {
+            "cve": {
+                "created_time": {
+                    "key": "x-ocsf-vulnerabilities.created_time",
                     "object": "vulnerabilities"
                 },
-                "metrics": {
-                    "name": {
-                        "key": "x-ocsf-vulnerabilities.name",
+                "cvss": {
+                    "base_score": {
+                        "key": "x-ocsf-vulnerabilities.base_score",
+                        "object": "vulnerabilities"
+                    },
+                    "depth": {
+                        "key": "x-ocsf-vulnerabilities.depth",
+                        "object": "vulnerabilities"
+                    },
+                    "metrics": {
+                        "name": {
+                            "key": "x-ocsf-vulnerabilities.name",
+                            "object": "vulnerabilities"
+                        },
+                        "value": {
+                            "key": "x-ocsf-vulnerabilities.value",
+                            "object": "vulnerabilities"
+                        }
+                    },
+                    "overall_score": {
+                        "key": "x-ocsf-vulnerabilities.overall_score",
+                        "object": "vulnerabilities"
+                    },
+                    "severity": {
+                        "key": "x-ocsf-vulnerabilities.severity",
                         "object": "vulnerabilities"
                     },
-                    "value": {
-                        "key": "x-ocsf-vulnerabilities.value",
+                    "vector_string": {
+                        "key": "x-ocsf-vulnerabilities.vector_string",
+                        "object": "vulnerabilities"
+                    },
+                    "version": {
+                        "key": "x-ocsf-vulnerabilities.version",
                         "object": "vulnerabilities"
                     }
                 },
-                "overall_score": {
-                    "key": "x-ocsf-vulnerabilities.overall_score",
+                "cwe_uid": {
+                    "key": "x-ocsf-vulnerabilities.cwe_uid",
                     "object": "vulnerabilities"
                 },
-                "severity": {
-                    "key": "x-ocsf-vulnerabilities.severity",
+                "cwe_url": {
+                    "key": "x-ocsf-vulnerabilities.cwe_url",
                     "object": "vulnerabilities"
                 },
-                "vector_string": {
-                    "key": "x-ocsf-vulnerabilities.vector_string",
+                "modified_time": {
+                    "key": "x-ocsf-vulnerabilities.modified_time",
                     "object": "vulnerabilities"
                 },
-                "version": {
-                    "key": "x-ocsf-vulnerabilities.version",
-                    "object": "vulnerabilities"
-                }
-            },
-            "cwe_uid": {
-                "key": "x-ocsf-vulnerabilities.cwe_uid",
-                "object": "vulnerabilities"
-            },
-            "cwe_url": {
-                "key": "x-ocsf-vulnerabilities.cwe_url",
-                "object": "vulnerabilities"
-            },
-            "modified_time": {
-                "key": "x-ocsf-vulnerabilities.modified_time",
-                "object": "vulnerabilities"
-            },
-            "product": {
-                "feature": {
+                "product": {
+                    "feature": {
+                        "name": {
+                            "key": "software.extensions.x-ocsf-product-ext.feature_name",
+                            "object": "vulnerabilities-software"
+                        },
+                        "uid": {
+                            "key": "software.extensions.x-ocsf-product-ext.feature_uid",
+                            "object": "vulnerabilities-software"
+                        },
+                        "version": {
+                            "key": "software.extensions.x-ocsf-product-ext.feature_version",
+                            "object": "vulnerabilities-software"
+                        }
+                    },
+                    "lang": {
+                        "key": "software.languages",
+                        "object": "vulnerabilities-software"
+                    },
                     "name": {
-                        "key": "software.extensions.x-ocsf-product-ext.feature_name",
+                        "key": "software.name",
+                        "object": "vulnerabilities-software"
+                    },
+                    "path": {
+                        "key": "software.extensions.x-ocsf-product-ext.installed_path",
                         "object": "vulnerabilities-software"
                     },
                     "uid": {
-                        "key": "software.extensions.x-ocsf-product-ext.feature_uid",
+                        "key": "software.extensions.x-ocsf-product-ext.product_uid",
+                        "object": "vulnerabilities-software"
+                    },
+                    "vendor_name": {
+                        "key": "software.vendor",
                         "object": "vulnerabilities-software"
                     },
                     "version": {
-                        "key": "software.extensions.x-ocsf-product-ext.feature_version",
+                        "key": "software.version",
                         "object": "vulnerabilities-software"
                     }
                 },
-                "lang": {
-                    "key": "software.languages",
-                    "object": "vulnerabilities-software"
+                "type": {
+                    "key": "x-ocsf-vulnerabilities.type",
+                    "object": "vulnerabilities"
                 },
-                "name": {
-                    "key": "software.name",
-                    "object": "vulnerabilities-software"
+                "uid": {
+                    "key": "x-ocsf-vulnerabilities.uid",
+                    "object": "vulnerabilities"
+                }
+            },
+            "desc": {
+                "key": "x-ocsf-vulnerabilities.desc",
+                "object": "vulnerabilities"
+            },
+            "kb_articles": {
+                "key": "x-ocsf-vulnerabilities.kb_articles",
+                "object": "vulnerabilities"
+            },
+            "packages": {
+                "architecture": {
+                    "key": "x-ocsf-vulnerabilities.packages_architecture",
+                    "object": "vulnerabilities"
                 },
-                "path": {
-                    "key": "software.extensions.x-ocsf-product-ext.installed_path",
-                    "object": "vulnerabilities-software"
+                "epoch": {
+                    "key": "x-ocsf-vulnerabilities.packages_epoch",
+                    "object": "vulnerabilities"
                 },
-                "uid": {
-                    "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                    "object": "vulnerabilities-software"
+                "license": {
+                    "key": "x-ocsf-vulnerabilities.packages_license",
+                    "object": "vulnerabilities"
                 },
-                "vendor_name": {
-                    "key": "software.vendor",
-                    "object": "vulnerabilities-software"
+                "name": {
+                    "key": "x-ocsf-vulnerabilities.packages_name",
+                    "object": "vulnerabilities"
+                },
+                "release": {
+                    "key": "x-ocsf-vulnerabilities.packages_release",
+                    "object": "vulnerabilities"
                 },
                 "version": {
-                    "key": "software.version",
-                    "object": "vulnerabilities-software"
+                    "key": "x-ocsf-vulnerabilities.packages_version",
+                    "object": "vulnerabilities"
                 }
             },
-            "type": {
-                "key": "x-ocsf-vulnerabilities.type",
+            "references": {
+                "key": "x-ocsf-vulnerabilities.references",
                 "object": "vulnerabilities"
             },
-            "uid": {
-                "key": "x-ocsf-vulnerabilities.uid",
-                "object": "vulnerabilities"
-            }
-        },
-        "desc": {
-            "key": "x-ocsf-vulnerabilities.desc",
-            "object": "vulnerabilities"
-        },
-        "kb_articles": {
-            "key": "x-ocsf-vulnerabilities.kb_articles",
-            "object": "vulnerabilities"
-        },
-        "packages": {
-            "architecture": {
-                "key": "x-ocsf-vulnerabilities.packages_architecture",
+            "related_vulnerabilities": {
+                "key": "x-ocsf-vulnerabilities.related_vulnerabilities",
                 "object": "vulnerabilities"
             },
-            "epoch": {
-                "key": "x-ocsf-vulnerabilities.packages_epoch",
+            "severity": {
+                "key": "x-ocsf-vulnerabilities.severity",
                 "object": "vulnerabilities"
             },
-            "license": {
-                "key": "x-ocsf-vulnerabilities.packages_license",
+            "title": {
+                "key": "x-ocsf-vulnerabilities.title",
                 "object": "vulnerabilities"
             },
-            "name": {
-                "key": "x-ocsf-vulnerabilities.packages_name",
+            "vendor_name": {
+                "key": "x-ocsf-vulnerabilities.vendor_name",
                 "object": "vulnerabilities"
+            }
+        }
+    },
+    "vpcflow": {
+        "account": [
+            {
+                "key": "x-aws-details.account_id",
+                "object": "accountid"
+            }
+        ],
+        "action": {
+            "key": "x-ibm-finding.finding_type",
+            "object": "ibm_finding"
+        },
+        "destinationaddress": [
+            {
+                "key": "ipv4-addr.value",
+                "object": "dst_ip"
             },
-            "release": {
-                "key": "x-ocsf-vulnerabilities.packages_release",
-                "object": "vulnerabilities"
+            {
+                "key": "ipv6-addr.value",
+                "object": "dst_ip"
             },
-            "version": {
-                "key": "x-ocsf-vulnerabilities.packages_version",
-                "object": "vulnerabilities"
+            {
+                "key": "x-ibm-finding.dst_ip_ref",
+                "object": "ibm_finding",
+                "references": "dst_ip"
+            },
+            {
+                "key": "network-traffic.dst_ref",
+                "object": "nt",
+                "references": "dst_ip"
             }
+        ],
+        "destinationport": [
+            {
+                "key": "network-traffic.dst_port",
+                "object": "nt",
+                "transformer": "ToInteger"
+            }
+        ],
+        "endtime": [
+            {
+                "key": "network-traffic.end",
+                "object": "nt",
+                "transformer": "EpochSecondsToTimestamp"
+            },
+            {
+                "key": "x-ibm-finding.end",
+                "object": "ibm_finding",
+                "transformer": "EpochSecondsToTimestamp"
+            },
+            {
+                "cybox": false,
+                "key": "last_observed",
+                "transformer": "EpochToTimestamp"
+            }
+        ],
+        "name": {
+            "key": "x-ibm-finding.name",
+            "object": "ibm_finding"
         },
-        "references": {
-            "key": "x-ocsf-vulnerabilities.references",
-            "object": "vulnerabilities"
-        },
-        "related_vulnerabilities": {
-            "key": "x-ocsf-vulnerabilities.related_vulnerabilities",
-            "object": "vulnerabilities"
-        },
-        "severity": {
-            "key": "x-ocsf-vulnerabilities.severity",
-            "object": "vulnerabilities"
-        },
-        "title": {
-            "key": "x-ocsf-vulnerabilities.title",
-            "object": "vulnerabilities"
-        },
-        "vendor_name": {
-            "key": "x-ocsf-vulnerabilities.vendor_name",
-            "object": "vulnerabilities"
-        }
+        "protocol": [
+            {
+                "key": "network-traffic.protocols",
+                "object": "nt",
+                "transformer": "ToLowercaseArray"
+            }
+        ],
+        "sourceaddress": [
+            {
+                "key": "ipv4-addr.value",
+                "object": "src_ip"
+            },
+            {
+                "key": "ipv6-addr.value",
+                "object": "src_ip"
+            },
+            {
+                "key": "network-traffic.src_ref",
+                "object": "nt",
+                "references": "src_ip"
+            },
+            {
+                "key": "x-ibm-finding.src_ip_ref",
+                "object": "ibm_finding",
+                "references": "src_ip"
+            },
+            {
+                "cybox": false,
+                "ds_key": "interfaceid",
+                "key": "ipv4-addr.x_aws_interface_id",
+                "object": "src_ip"
+            },
+            {
+                "cybox": false,
+                "ds_key": "interfaceid",
+                "key": "ipv6-addr.x_aws_interface_id",
+                "object": "src_ip"
+            }
+        ],
+        "sourceport": [
+            {
+                "key": "network-traffic.src_port",
+                "object": "nt",
+                "transformer": "ToInteger"
+            }
+        ],
+        "starttime": [
+            {
+                "key": "network-traffic.start",
+                "object": "nt",
+                "transformer": "EpochSecondsToTimestamp"
+            },
+            {
+                "key": "x-ibm-finding.start",
+                "object": "ibm_finding",
+                "transformer": "EpochSecondsToTimestamp"
+            },
+            {
+                "cybox": false,
+                "key": "first_observed",
+                "transformer": "EpochSecondsToTimestamp"
+            }
+        ]
     }
 }
```

## Comparing `stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/LICENSE.md` & `stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/METADATA` & `stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stix-shifter-modules-aws-athena
-Version: 5.3.0.dev824
+Version: 5.3.0.dev826
 Summary: Tools and interface to translate STIX formatted results and queries to different data source formats and to set up appropriate connection strings for invoking and triggering actions in openwhisk
 Home-page: https://github.com/opencybersecurityalliance/stix-shifter
 Author: ibm
 Author-email: 
 Project-URL: Source, https://github.com/opencybersecurityalliance/stix-shifter
 Keywords: datasource stix translate transform transmit
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/NOTICE` & `stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/RECORD` & `stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 stix_shifter_modules/aws_athena/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 stix_shifter_modules/aws_athena/entry_point.py,sha256=FHXjqiWmrOdq31iDqyFzooZyxBGxqUIp3RqWcxcfiOY,1374
-stix_shifter_modules/aws_athena/configuration/config.json,sha256=hcONb519g125xA_z3K2m-wvYxTybWUG5vrgSxEDQoHw,241540
+stix_shifter_modules/aws_athena/configuration/config.json,sha256=1mJSCaiSubfdR51fFjajjYtNlX8-pKKGKIWALHUmV6A,254103
 stix_shifter_modules/aws_athena/configuration/dialects.json,sha256=2nYaixArRUIgorTTWC7QzuuNiHti6tF3gb6y0y91x7Q,229
 stix_shifter_modules/aws_athena/configuration/lang_en.json,sha256=J4SXpSel1epi9EKGVppvLYfXPkbIxfxwJcJ-xwyc2ww,4766
 stix_shifter_modules/aws_athena/stix_translation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 stix_shifter_modules/aws_athena/stix_translation/json_to_stix_translator.py,sha256=8KbNAbPFHVIw6CN4tylW35GqJ1sxBZpaxpQaFAM6e0M,22536
 stix_shifter_modules/aws_athena/stix_translation/query_constructor.py,sha256=IsWNLisRsvduCgv1OrQ05x6llobayfUapumqGLOrZRo,24044
 stix_shifter_modules/aws_athena/stix_translation/query_translator.py,sha256=QyXnF8HPZWYYmNM1WrFqoH3ZaW8S4fOh0oxZFSgmYaE,1024
-stix_shifter_modules/aws_athena/stix_translation/results_translator.py,sha256=fS1N2coH-3lyRkHE3NNjtdJg6FVxUrRP2Oe6uakgqhI,1518
+stix_shifter_modules/aws_athena/stix_translation/results_translator.py,sha256=SkMabFdZ2PxhXy6OZKjf45XRttP-LveVPhzi9ZyAD3s,1522
 stix_shifter_modules/aws_athena/stix_translation/transformers.py,sha256=RmmyKJwXx3XMgvCLKAex2ZgTwmg14REONa-Ai_D2AqE,1075
 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_config.json,sha256=leAlSRCH2F-6GtOewVbFfkaXV_fUY_B3qA-QcQyoOQM,4765
 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_from_stix_map.json,sha256=qdbHf8p71aOUgH29SiCgbW-bm7tyz6TkMVKVJ1XfljY,1894
-stix_shifter_modules/aws_athena/stix_translation/json/guardduty_to_stix_map.json,sha256=BF4bPvgzAX8Zfmekg37i_g3BskFqSo4Qv-jSob7xKVM,10630
 stix_shifter_modules/aws_athena/stix_translation/json/hash_algorithm_map.json,sha256=Mjh6Jl4D14CKVwuQh2ksTIh69hYg-ygZrUBuOigG8pQ,139
 stix_shifter_modules/aws_athena/stix_translation/json/network_protocol_map.json,sha256=Kv22JuyDwUdrLxnhj_789NmXsE9aTRvNKlPM95_Hb5s,2439
 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_from_stix_map.json,sha256=aCIzFD7g24EseM4-VviVumdn6oWvQSjYv4-2ZdefiVQ,18300
-stix_shifter_modules/aws_athena/stix_translation/json/ocsf_to_stix_map.json,sha256=KuBIUXH6fuIyWRPcKDB9UjS-If_iGGulIaiP0xQQhAE,75711
 stix_shifter_modules/aws_athena/stix_translation/json/operators.json,sha256=jLCjazSAKvuvKzZhibBK3_PccQGu0TGF5inbzzzkoR0,591
+stix_shifter_modules/aws_athena/stix_translation/json/to_stix_map.json,sha256=WUnNz_EC9RPD3aga9ysvWoPENtrazAlIPpxOU7wBxtA,95113
 stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_from_stix_map.json,sha256=TDiBsk4GtUH98mK6_KBKfFcDoOo1UzF08lyFpHF9XqM,891
-stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_to_stix_map.json,sha256=Gn0j16snxjOTkIXVGyhk3y3JEEg9kOGX2YXmRoxV_Zc,2464
 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/guardduty_from_stix_map.json,sha256=qdbHf8p71aOUgH29SiCgbW-bm7tyz6TkMVKVJ1XfljY,1894
 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/ocsf_from_stix_map.json,sha256=_lKZSQdQjm7yJZ5ZDCww8rC4QVFtS75cqdUmnQrpBKw,18297
 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/to_stix_map.json,sha256=F5s7ytTJtBYhUtisvZyuj9y_vVryv4oPsTC-03vqTG8,94538
 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/vpcflow_from_stix_map.json,sha256=TDiBsk4GtUH98mK6_KBKfFcDoOo1UzF08lyFpHF9XqM,891
 stix_shifter_modules/aws_athena/stix_transmission/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 stix_shifter_modules/aws_athena/stix_transmission/boto3_client.py,sha256=4hVUN_O77rghatKexuLOPsTGvzi2fHInpFfgYBuTPkM,4173
 stix_shifter_modules/aws_athena/stix_transmission/delete_connector.py,sha256=D2A5li6TWgZvqpnDGLXVveLqYHlWI1evVWKYKeXT60M,1207
 stix_shifter_modules/aws_athena/stix_transmission/error_mapper.py,sha256=rghGzuJb_Av8SG4TBLXTF22OH4kh3ywixNJ4FILSCBw,1529
 stix_shifter_modules/aws_athena/stix_transmission/ping_connector.py,sha256=pLxf6W2ZtM-nHtJzFLjauapvrC5RHNuU2FVDctbjLVA,878
 stix_shifter_modules/aws_athena/stix_transmission/query_connector.py,sha256=eOK6mHRwtASq4gZxOyqmSUvDDThxkDhhbdYQ8jOTweY,7443
-stix_shifter_modules/aws_athena/stix_transmission/results_connector.py,sha256=2nmRHBVqHwbOCYXTH5l8-yYDHe_4L7qf1k7kIuwFcAg,14480
+stix_shifter_modules/aws_athena/stix_transmission/results_connector.py,sha256=RJw9nNCr7FCIqqRJOSUG55k8a9uo0wdk7tYc27NHg7c,14478
 stix_shifter_modules/aws_athena/stix_transmission/status_connector.py,sha256=G-JPjia6t91hGEtvAgImHpoGdO2DNI9ERZB4AAzqf7s,3175
-stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/LICENSE.md,sha256=ssGEKMVW69oFTBblVhD1YPolqCOyOCJi4wRDRI7xCnU,12786
-stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/METADATA,sha256=GqwsHAN41aC_F6Rpfx3H4hoyQl3QnP5NiKbIGUCAN5g,8047
-stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/NOTICE,sha256=wx-gWE9vSnLJ7YQkrGlMp9VNXOXG57TTxDDRd9CEdYg,1418
-stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/top_level.txt,sha256=NX-VgUOr8fI-lMXHt3gtjfsEn1UPaGAVszt6Z_CTp2s,21
-stix_shifter_modules_aws_athena-5.3.0.dev824.dist-info/RECORD,,
+stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/LICENSE.md,sha256=ssGEKMVW69oFTBblVhD1YPolqCOyOCJi4wRDRI7xCnU,12786
+stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/METADATA,sha256=DynCiuKFdQGqtd-lvlo8BDzdu_uVyXbogDj_rlvIPdY,8047
+stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/NOTICE,sha256=wx-gWE9vSnLJ7YQkrGlMp9VNXOXG57TTxDDRd9CEdYg,1418
+stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/top_level.txt,sha256=NX-VgUOr8fI-lMXHt3gtjfsEn1UPaGAVszt6Z_CTp2s,21
+stix_shifter_modules_aws_athena-5.3.0.dev826.dist-info/RECORD,,
```

