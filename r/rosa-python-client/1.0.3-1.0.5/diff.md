# Comparing `tmp/rosa_python_client-1.0.3.tar.gz` & `tmp/rosa_python_client-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosa_python_client-1.0.3.tar", max compression
+gzip compressed data, was "rosa_python_client-1.0.5.tar", max compression
```

## Comparing `rosa_python_client-1.0.3.tar` & `rosa_python_client-1.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      511 2023-05-18 13:43:06.930894 rosa_python_client-1.0.3/README.md
--rw-r--r--   0        0        0      353 2023-05-18 13:43:06.930894 rosa_python_client-1.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-18 13:43:06.930894 rosa_python_client-1.0.3/rosa/__init__.py
--rw-r--r--   0        0        0     4568 2023-05-18 13:43:06.930894 rosa_python_client-1.0.3/rosa/cli.py
--rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 rosa_python_client-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      511 2023-05-18 16:29:17.912540 rosa_python_client-1.0.5/README.md
+-rw-r--r--   0        0        0      353 2023-05-18 16:29:17.913540 rosa_python_client-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-18 16:29:17.913540 rosa_python_client-1.0.5/rosa/__init__.py
+-rw-r--r--   0        0        0     5360 2023-05-18 16:29:17.913540 rosa_python_client-1.0.5/rosa/cli.py
+-rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 rosa_python_client-1.0.5/PKG-INFO
```

### Comparing `rosa_python_client-1.0.3/rosa/cli.py` & `rosa_python_client-1.0.5/rosa/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
 
 def parse_help(rosa_cmd="rosa"):
     commands_dict = {}
     _commands = get_available_commands(command=[rosa_cmd])
     output_flag_str = "-o, --output"
     auto_answer_yes_str = "-y, --yes"
+    auto_mode_str = "-m, --mode"
 
     for command in _commands:
         commands_dict.setdefault(command, {})
 
     for top_command in commands_dict.keys():
         _commands = get_available_commands(command=[rosa_cmd, top_command])
         for command in _commands:
@@ -75,27 +76,37 @@
                     )
                     commands_dict[top_command][command][_command][
                         "auto_answer_yes"
                     ] = check_flag_in_flags(
                         command_list=[rosa_cmd, top_command, _command],
                         flag_str=auto_answer_yes_str,
                     )
+                    commands_dict[top_command][command][_command][
+                        "auto_mode"
+                    ] = check_flag_in_flags(
+                        command_list=[rosa_cmd, top_command, _command],
+                        flag_str=auto_mode_str,
+                    )
             else:
                 commands_dict[top_command][command][
                     "json_output"
                 ] = check_flag_in_flags(
                     command_list=[rosa_cmd, top_command, command],
                     flag_str=output_flag_str,
                 )
                 commands_dict[top_command][command][
                     "auto_answer_yes"
                 ] = check_flag_in_flags(
                     command_list=[rosa_cmd, top_command, command],
                     flag_str=auto_answer_yes_str,
                 )
+                commands_dict[top_command][command]["auto_mode"] = check_flag_in_flags(
+                    command_list=[rosa_cmd, top_command, command],
+                    flag_str=auto_mode_str,
+                )
 
     return commands_dict
 
 
 def parse_json_response(response):
     try:
         return json.loads(response)
@@ -106,27 +117,33 @@
 def execute(command, allowed_commands=None):
     allowed_commands = allowed_commands or parse_help()
     _user_command = shlex.split(command)
     command = ["rosa"]
     command.extend(_user_command)
     json_output = {}
     auto_answer_yes = {}
+    auto_update = {}
     for cmd in command[1:]:
         if cmd.startswith("--"):
             continue
 
         json_output = allowed_commands.get(cmd, json_output.get(cmd, {}))
         add_json_output = json_output.get("json_output") is True
         if add_json_output:
             command.append("-ojson")
 
         auto_answer_yes = allowed_commands.get(cmd, auto_answer_yes.get(cmd, {}))
-        add_auto_answer_yes = json_output.get("auto_answer_yes") is True
+        add_auto_answer_yes = auto_answer_yes.get("auto_answer_yes") is True
         if add_auto_answer_yes:
             command.append("--yes")
 
-        if add_json_output or add_auto_answer_yes:
+        auto_update = allowed_commands.get(cmd, auto_update.get(cmd, {}))
+        add_auto_update = auto_update.get("auto_mode") is True
+        if add_auto_update:
+            command.append("--mode auto")
+
+        if add_json_output or add_auto_answer_yes or add_auto_update:
             break
 
     LOGGER.info(f"Executing command: {' '.join(command)}")
     res = subprocess.run(command, capture_output=True, check=True, text=True)
     return parse_json_response(response=res.stdout)
```

### Comparing `rosa_python_client-1.0.3/PKG-INFO` & `rosa_python_client-1.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosa-python-client
-Version: 1.0.3
+Version: 1.0.5
 Summary: Wrapper for rosa cli
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

