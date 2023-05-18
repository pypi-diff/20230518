# Comparing `tmp/ansible-variables-0.4.3.tar.gz` & `tmp/ansible-variables-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-variables-0.4.3.tar", last modified: Mon May  1 16:10:58 2023, max compression
+gzip compressed data, was "ansible-variables-0.5.0.tar", last modified: Thu May 18 15:09:43 2023, max compression
```

## Comparing `ansible-variables-0.4.3.tar` & `ansible-variables-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:58.651362 ansible-variables-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-01 16:10:58.651362 ansible-variables-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:58.647362 ansible-variables-0.4.3/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:58.647362 ansible-variables-0.4.3/lib/ansible_variables/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/lib/ansible_variables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:58.647362 ansible-variables-0.4.3/lib/ansible_variables/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/lib/ansible_variables/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/lib/ansible_variables/cli/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:58.647362 ansible-variables-0.4.3/lib/ansible_variables/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/lib/ansible_variables/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/lib/ansible_variables/utils/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:58.647362 ansible-variables-0.4.3/lib/ansible_variables.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-01 16:10:58.000000 ansible-variables-0.4.3/lib/ansible_variables.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-01 16:10:58.000000 ansible-variables-0.4.3/lib/ansible_variables.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:10:58.000000 ansible-variables-0.4.3/lib/ansible_variables.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-01 16:10:58.000000 ansible-variables-0.4.3/lib/ansible_variables.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:10:58.000000 ansible-variables-0.4.3/lib/ansible_variables.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-01 16:10:58.000000 ansible-variables-0.4.3/lib/ansible_variables.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 16:10:58.000000 ansible-variables-0.4.3/lib/ansible_variables.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-01 16:10:58.651362 ansible-variables-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:58.651362 ansible-variables-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/tests/test_variablesource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:43.199601 ansible-variables-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 15:09:32.000000 ansible-variables-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-18 15:09:43.199601 ansible-variables-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-18 15:09:32.000000 ansible-variables-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:43.195601 ansible-variables-0.5.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:43.195601 ansible-variables-0.5.0/lib/ansible_variables/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-18 15:09:32.000000 ansible-variables-0.5.0/lib/ansible_variables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:43.199601 ansible-variables-0.5.0/lib/ansible_variables/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-18 15:09:32.000000 ansible-variables-0.5.0/lib/ansible_variables/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-18 15:09:32.000000 ansible-variables-0.5.0/lib/ansible_variables/cli/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:43.199601 ansible-variables-0.5.0/lib/ansible_variables/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:32.000000 ansible-variables-0.5.0/lib/ansible_variables/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-18 15:09:32.000000 ansible-variables-0.5.0/lib/ansible_variables/utils/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:43.199601 ansible-variables-0.5.0/lib/ansible_variables.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-18 15:09:43.000000 ansible-variables-0.5.0/lib/ansible_variables.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-18 15:09:43.000000 ansible-variables-0.5.0/lib/ansible_variables.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:09:43.000000 ansible-variables-0.5.0/lib/ansible_variables.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-18 15:09:43.000000 ansible-variables-0.5.0/lib/ansible_variables.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:09:42.000000 ansible-variables-0.5.0/lib/ansible_variables.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-18 15:09:43.000000 ansible-variables-0.5.0/lib/ansible_variables.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-18 15:09:43.000000 ansible-variables-0.5.0/lib/ansible_variables.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-18 15:09:32.000000 ansible-variables-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-18 15:09:43.199601 ansible-variables-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-18 15:09:32.000000 ansible-variables-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:43.199601 ansible-variables-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-18 15:09:32.000000 ansible-variables-0.5.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-18 15:09:32.000000 ansible-variables-0.5.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-18 15:09:32.000000 ansible-variables-0.5.0/tests/test_variablesource.py
```

### Comparing `ansible-variables-0.4.3/LICENSE` & `ansible-variables-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.4.3/PKG-INFO` & `ansible-variables-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-variables
-Version: 0.4.3
+Version: 0.5.0
 Summary: Keep track of Ansible host context variables
 Home-page: https://github.com/hille721/ansible-variables
 Author: Christoph Hille
 Author-email: hille721@gmail.com
 License: GPLv3+
 Project-URL: Documentation, https://github.com/hille721/ansible-variables/blob/main/README.md
 Project-URL: Repository, https://github.com/hille721/ansible-variables
```

### Comparing `ansible-variables-0.4.3/README.md` & `ansible-variables-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.4.3/lib/ansible_variables/cli/variables.py` & `ansible-variables-0.5.0/lib/ansible_variables/cli/variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import argparse
 
 import rich
 from ansible import context
-from ansible.cli import CLI
 from ansible.cli.arguments import option_helpers as opt_help
 from ansible.errors import AnsibleOptionsError
 from ansible.module_utils._text import to_native
 from ansible.utils.display import Display
 
 from ansible_variables import __version__
+from ansible_variables.cli import CLI
 from ansible_variables.utils.vars import variable_sources
 
 display = Display()
 
 # Internal vars same as defined for ansible-inventory
 # pylint: disable=line-too-long
 # (https://github.com/ansible/ansible/blob/d081ed36169f4f74512d1707909185281a30e29b/lib/ansible/cli/inventory.py#L28-L46
```

### Comparing `ansible-variables-0.4.3/lib/ansible_variables/utils/vars.py` & `ansible-variables-0.5.0/lib/ansible_variables/utils/vars.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,19 @@
 
     def file_occurrences(self, loader: DataLoader):
         """Open the files and check if the variables occur in it"""
         occurrences = []
 
         for ffile in self.files:
             display.vvv("Checking file %s for occurrence of variable %s" % (ffile, self.name))
-            if loader.load_from_file(ffile) and self.name in loader.load_from_file(ffile):
+
+            # Setting unsafe=True will prevent deepcopy and will help with performance
+            # and it's safe because we're not modifying the content
+            content = loader.load_from_file(ffile, unsafe=True)
+            if content and self.name in content:
                 occurrences.append(ffile)
 
         return occurrences
 
 
 def variable_sources(
     variable_manager: VariableManager,
```

### Comparing `ansible-variables-0.4.3/lib/ansible_variables.egg-info/PKG-INFO` & `ansible-variables-0.5.0/lib/ansible_variables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-variables
-Version: 0.4.3
+Version: 0.5.0
 Summary: Keep track of Ansible host context variables
 Home-page: https://github.com/hille721/ansible-variables
 Author: Christoph Hille
 Author-email: hille721@gmail.com
 License: GPLv3+
 Project-URL: Documentation, https://github.com/hille721/ansible-variables/blob/main/README.md
 Project-URL: Repository, https://github.com/hille721/ansible-variables
```

### Comparing `ansible-variables-0.4.3/lib/ansible_variables.egg-info/SOURCES.txt` & `ansible-variables-0.5.0/lib/ansible_variables.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.4.3/setup.cfg` & `ansible-variables-0.5.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ansible-variables
-version = 0.4.3
+version = 0.5.0
 description = Keep track of Ansible host context variables
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Christoph Hille
 author_email = hille721@gmail.com
 url = https://github.com/hille721/ansible-variables
 project_urls =
```

### Comparing `ansible-variables-0.4.3/tests/test_cli.py` & `ansible-variables-0.5.0/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import pytest
 from ansible import constants as C
 
-from ansible_variables.cli.variables import VariablesCLI
+from ansible_variables.cli.variables import VariablesCLI, main
 
 C.set_constant("CONFIG_FILE", "tests/test_data/ansible.cfg")
 C.set_constant("DEFAULT_HOST_LIST", "tests/test_data/inventory")
 
 
-def test_parse(capsys):
-    """Test ansible-variables parse"""
-
-    variables_cli = VariablesCLI(["ansible-variables"])
+def test_main(capsys):
     with pytest.raises(SystemExit) as pytest_wrapped_e:
-        variables_cli.parse()
+        main(["ansible-variables"])
     assert pytest_wrapped_e.type == SystemExit
     assert "ansible-variables: error: the following arguments are required: host" in capsys.readouterr().err
 
 
 def test_cli_config(capsys):
     variables_cli = VariablesCLI(["ansible-variables", "--version"])
     with pytest.raises(SystemExit):
```

### Comparing `ansible-variables-0.4.3/tests/test_utils.py` & `ansible-variables-0.5.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.4.3/tests/test_variablesource.py` & `ansible-variables-0.5.0/tests/test_variablesource.py`

 * *Files identical despite different names*

