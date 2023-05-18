# Comparing `tmp/shipyard_jira-0.1.2.tar.gz` & `tmp/shipyard_jira-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_jira-0.1.2.tar", max compression
+gzip compressed data, was "shipyard_jira-0.1.3.tar", max compression
```

## Comparing `shipyard_jira-0.1.2.tar` & `shipyard_jira-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      925 2023-05-17 13:52:05.044803 shipyard_jira-0.1.2/README.md
--rw-r--r--   0        0        0      538 2023-05-17 13:45:43.414624 shipyard_jira-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       28 2023-05-16 19:54:06.647847 shipyard_jira-0.1.2/shipyard_jira/__init__.py
--rw-r--r--   0        0        0      962 2023-05-17 13:42:11.918690 shipyard_jira-0.1.2/shipyard_jira/cli/add_comment.py
--rw-r--r--   0        0        0     2283 2023-05-16 19:54:06.648575 shipyard_jira-0.1.2/shipyard_jira/cli/create_ticket.py
--rw-r--r--   0        0        0     2290 2023-05-17 13:30:30.655443 shipyard_jira-0.1.2/shipyard_jira/cli/edit_ticket.py
--rw-r--r--   0        0        0    12673 2023-05-17 13:42:11.929391 shipyard_jira-0.1.2/shipyard_jira/jira.py
--rw-r--r--   0        0        0     1416 1970-01-01 00:00:00.000000 shipyard_jira-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      925 2023-05-18 13:47:13.960890 shipyard_jira-0.1.3/README.md
+-rw-r--r--   0        0        0      511 2023-05-18 14:44:36.174281 shipyard_jira-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-05-16 19:54:06.647847 shipyard_jira-0.1.3/shipyard_jira/__init__.py
+-rw-r--r--   0        0        0      938 2023-05-18 14:39:22.577108 shipyard_jira-0.1.3/shipyard_jira/cli/add_comment.py
+-rw-r--r--   0        0        0     2319 2023-05-18 14:43:09.829284 shipyard_jira-0.1.3/shipyard_jira/cli/create_ticket.py
+-rw-r--r--   0        0        0     2201 2023-05-18 14:38:05.406441 shipyard_jira-0.1.3/shipyard_jira/cli/edit_ticket.py
+-rw-r--r--   0        0        0    12673 2023-05-18 14:10:16.168569 shipyard_jira-0.1.3/shipyard_jira/jira.py
+-rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 shipyard_jira-0.1.3/PKG-INFO
```

### Comparing `shipyard_jira-0.1.2/README.md` & `shipyard_jira-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `shipyard_jira-0.1.2/shipyard_jira/cli/create_ticket.py` & `shipyard_jira-0.1.3/shipyard_jira/cli/create_ticket.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 import sys
-import logging
+
 from shipyard_jira import JiraClient
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("--access-token", dest="access_token", required=True)
     parser.add_argument("--email", dest="email", required=True)
@@ -38,22 +38,23 @@
     # and inadvertently overwriting valid ticket data.
     create_ticket_args = {key: value for key, value in args_dict.items() if value not in (None, '')}
 
     if args.parent_ticket_id:
         try:
             jira.create_subtask(**create_ticket_args)
         except Exception as e:
-            logging.error(e)
+            jira.logger.error(e)
             sys.exit(1)
         else:
             sys.exit(0)
     else:
         try:
             jira.create_ticket(**create_ticket_args)
-        except Exception:
+        except Exception as error:
+            jira.logger.error(error)
             sys.exit(1)
         else:
             sys.exit(0)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `shipyard_jira-0.1.2/shipyard_jira/cli/edit_ticket.py` & `shipyard_jira-0.1.3/shipyard_jira/cli/edit_ticket.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,29 +33,27 @@
     args_dict.pop('email')
     args_dict.pop('domain')
 
     if args_dict['summary']:
         args_dict['summary'] = [{'set': args_dict['summary']}]
     if args_dict['description']:
         args_dict['description'] = [{'set': args_dict['description']}]
-    if args_dict['issue_type']:
-        args_dict['issue_type'] = [{'set': args_dict['issue_type']}]
     if args_dict['assignee']:
         args_dict['assignee'] = [{'set': args_dict['assignee']}]
     if args_dict['labels']:
         args_dict['labels'] = [{'set': args_dict['labels'].split(',')}]
 
     # Filter out blank values from update_ticket_args to avoid sending them to the Jira API
     # and inadvertently overwriting valid ticket data.
     update_ticket_args = {key: value for key, value in args_dict.items() if value not in (None, '')}
 
     try:
         jira.update_ticket(**update_ticket_args)
     except Exception as error:
-        print(error)
+        jira.logger.error(error)
         sys.exit(1)
     else:
         sys.exit(0)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `shipyard_jira-0.1.2/shipyard_jira/jira.py` & `shipyard_jira-0.1.3/shipyard_jira/jira.py`

 * *Files identical despite different names*

### Comparing `shipyard_jira-0.1.2/PKG-INFO` & `shipyard_jira-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: shipyard-jira
-Version: 0.1.2
+Version: 0.1.3
 Summary: A local client for connecting and working with Jira
 Author: JR
 Author-email: johnathan.rodriguez@shipyardapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: shipyard-templates (>=0.1.2,<0.2.0)
 Description-Content-Type: text/markdown
 
 # Shipyard Jira
 Shipyard Jira is a Python library that provides a convenient interface for interacting with the Jira issue tracking system. It simplifies the process of managing Jira issues, allowing users to create, update, and query issues programmatically.
 
 ## Installation
 ```bash
```

