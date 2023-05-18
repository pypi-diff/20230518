# Comparing `tmp/deploymentutils-0.7.0.tar.gz` & `tmp/deploymentutils-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deploymentutils-0.7.0.tar", last modified: Thu May  5 14:19:06 2022, max compression
+gzip compressed data, was "deploymentutils-0.8.0.tar", last modified: Thu May 18 16:39:25 2023, max compression
```

## Comparing `deploymentutils-0.7.0.tar` & `deploymentutils-0.8.0.tar`

### file list

```diff
@@ -1,23 +1,47 @@
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-05-05 14:19:06.325864 deploymentutils-0.7.0/
--rw-r--r--   0 ck2       (1000) ck2       (1000)    34470 2020-05-23 15:55:46.000000 deploymentutils-0.7.0/LICENSE
--rw-r--r--   0 ck2       (1000) ck2       (1000)       25 2021-02-04 12:18:53.000000 deploymentutils-0.7.0/MANIFEST.in
--rw-r--r--   0 ck2       (1000) ck2       (1000)     3968 2022-05-05 14:19:06.325864 deploymentutils-0.7.0/PKG-INFO
--rw-r--r--   0 ck2       (1000) ck2       (1000)     3443 2022-05-05 14:12:29.000000 deploymentutils-0.7.0/README.md
--rw-r--r--   0 ck2       (1000) ck2       (1000)      114 2021-08-03 11:46:12.000000 deploymentutils-0.7.0/requirements.txt
--rw-r--r--   0 ck2       (1000) ck2       (1000)       38 2022-05-05 14:19:06.325864 deploymentutils-0.7.0/setup.cfg
--rw-r--r--   0 ck2       (1000) ck2       (1000)     1412 2021-10-12 10:30:48.000000 deploymentutils-0.7.0/setup.py
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-05-05 14:19:06.317864 deploymentutils-0.7.0/src/
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-05-05 14:19:06.321864 deploymentutils-0.7.0/src/deploymentutils/
--rw-r--r--   0 ck2       (1000) ck2       (1000)       79 2022-01-15 19:00:03.000000 deploymentutils-0.7.0/src/deploymentutils/__init__.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)    32378 2022-03-07 22:40:43.000000 deploymentutils-0.7.0/src/deploymentutils/core.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)       22 2022-02-05 13:43:49.000000 deploymentutils-0.7.0/src/deploymentutils/release.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)      807 2021-10-12 14:33:14.000000 deploymentutils-0.7.0/src/deploymentutils/script.py
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-05-05 14:19:06.325864 deploymentutils-0.7.0/src/deploymentutils.egg-info/
--rw-r--r--   0 ck2       (1000) ck2       (1000)     3968 2022-05-05 14:19:05.000000 deploymentutils-0.7.0/src/deploymentutils.egg-info/PKG-INFO
--rw-r--r--   0 ck2       (1000) ck2       (1000)      454 2022-05-05 14:19:05.000000 deploymentutils-0.7.0/src/deploymentutils.egg-info/SOURCES.txt
--rw-r--r--   0 ck2       (1000) ck2       (1000)        1 2022-05-05 14:19:05.000000 deploymentutils-0.7.0/src/deploymentutils.egg-info/dependency_links.txt
--rw-r--r--   0 ck2       (1000) ck2       (1000)       64 2022-05-05 14:19:05.000000 deploymentutils-0.7.0/src/deploymentutils.egg-info/entry_points.txt
--rw-r--r--   0 ck2       (1000) ck2       (1000)      114 2022-05-05 14:19:05.000000 deploymentutils-0.7.0/src/deploymentutils.egg-info/requires.txt
--rw-r--r--   0 ck2       (1000) ck2       (1000)       16 2022-05-05 14:19:05.000000 deploymentutils-0.7.0/src/deploymentutils.egg-info/top_level.txt
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-05-05 14:19:06.325864 deploymentutils-0.7.0/test/
--rw-r--r--   0 ck2       (1000) ck2       (1000)    17100 2022-03-07 22:45:00.000000 deploymentutils-0.7.0/test/test_core.py
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-05-18 16:39:25.844558 deploymentutils-0.8.0/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      590 2022-03-04 15:48:52.000000 deploymentutils-0.8.0/.drone.yml
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     1814 2020-05-23 15:55:46.000000 deploymentutils-0.8.0/.gitignore
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    34470 2020-05-23 15:55:46.000000 deploymentutils-0.8.0/LICENSE
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       25 2021-02-04 12:18:53.000000 deploymentutils-0.8.0/MANIFEST.in
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     3948 2023-05-18 16:39:25.844558 deploymentutils-0.8.0/PKG-INFO
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     3443 2022-05-05 14:12:29.000000 deploymentutils-0.8.0/README.md
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      155 2023-05-18 16:36:08.000000 deploymentutils-0.8.0/requirements.txt
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       38 2023-05-18 16:39:25.844558 deploymentutils-0.8.0/setup.cfg
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     1412 2021-10-12 10:30:48.000000 deploymentutils-0.8.0/setup.py
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-05-18 16:39:25.812558 deploymentutils-0.8.0/src/
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-05-18 16:39:25.832558 deploymentutils-0.8.0/src/deploymentutils/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       79 2022-01-15 19:00:03.000000 deploymentutils-0.8.0/src/deploymentutils/__init__.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    35120 2023-05-18 14:11:31.000000 deploymentutils-0.8.0/src/deploymentutils/core.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       22 2022-05-09 13:46:54.000000 deploymentutils-0.8.0/src/deploymentutils/release.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     1131 2023-05-18 14:17:55.000000 deploymentutils-0.8.0/src/deploymentutils/script.py
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-05-18 16:39:25.836558 deploymentutils-0.8.0/src/deploymentutils.egg-info/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     3948 2023-05-18 16:39:25.000000 deploymentutils-0.8.0/src/deploymentutils.egg-info/PKG-INFO
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      858 2023-05-18 16:39:25.000000 deploymentutils-0.8.0/src/deploymentutils.egg-info/SOURCES.txt
+-rw-r--r--   0 ck2       (1000) ck2       (1000)        1 2023-05-18 16:39:25.000000 deploymentutils-0.8.0/src/deploymentutils.egg-info/dependency_links.txt
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       64 2023-05-18 16:39:25.000000 deploymentutils-0.8.0/src/deploymentutils.egg-info/entry_points.txt
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      155 2023-05-18 16:39:25.000000 deploymentutils-0.8.0/src/deploymentutils.egg-info/requires.txt
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       16 2023-05-18 16:39:25.000000 deploymentutils-0.8.0/src/deploymentutils.egg-info/top_level.txt
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-05-18 16:39:25.840558 deploymentutils-0.8.0/test/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)        0 2020-06-05 08:37:15.000000 deploymentutils-0.8.0/test/__init__.py
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-05-18 16:39:25.816558 deploymentutils-0.8.0/test/_test_data/
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-05-18 16:39:25.816558 deploymentutils-0.8.0/test/_test_data/data1/
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-05-18 16:39:25.840558 deploymentutils-0.8.0/test/_test_data/data1/dir/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)        0 2021-07-08 15:52:32.000000 deploymentutils-0.8.0/test/_test_data/data1/dir/file1.txt
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-05-18 16:39:25.816558 deploymentutils-0.8.0/test/_test_data/data2/
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-05-18 16:39:25.840558 deploymentutils-0.8.0/test/_test_data/data2/dir/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)        0 2021-07-08 15:52:32.000000 deploymentutils-0.8.0/test/_test_data/data2/dir/file1.txt
+-rw-r--r--   0 ck2       (1000) ck2       (1000)        0 2021-07-08 15:52:32.000000 deploymentutils-0.8.0/test/_test_data/data2/dir/file2.txt
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-05-18 16:39:25.840558 deploymentutils-0.8.0/test/_test_data/data2/dir/subdir/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)        0 2021-07-08 15:52:32.000000 deploymentutils-0.8.0/test/_test_data/data2/dir/subdir/file3.txt
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-05-18 16:39:25.816558 deploymentutils-0.8.0/test/_test_data/data3/
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-05-18 16:39:25.840558 deploymentutils-0.8.0/test/_test_data/data3/dir/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)        0 2021-07-08 15:52:32.000000 deploymentutils-0.8.0/test/_test_data/data3/dir/file1.txt
+-rw-r--r--   0 ck2       (1000) ck2       (1000)        0 2021-07-08 15:52:32.000000 deploymentutils-0.8.0/test/_test_data/data3/dir/file4.txt
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-05-18 16:39:25.844558 deploymentutils-0.8.0/test/_test_json_data/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      125 2021-08-03 11:22:11.000000 deploymentutils-0.8.0/test/_test_json_data/data1.json
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      122 2021-08-03 11:26:04.000000 deploymentutils-0.8.0/test/_test_json_data/data2.yml
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-05-18 16:39:25.844558 deploymentutils-0.8.0/test/_test_templates/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      154 2020-05-24 14:24:12.000000 deploymentutils-0.8.0/test/_test_templates/template_1.txt
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      795 2023-05-18 12:18:18.000000 deploymentutils-0.8.0/test/test_config.ini
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     1012 2023-05-18 14:01:36.000000 deploymentutils-0.8.0/test/test_config.toml
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    22518 2023-05-18 14:09:58.000000 deploymentutils-0.8.0/test/test_core.py
```

### Comparing `deploymentutils-0.7.0/LICENSE` & `deploymentutils-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deploymentutils-0.7.0/PKG-INFO` & `deploymentutils-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: deploymentutils
-Version: 0.7.0
+Version: 0.8.0
 Summary: Small python package to facilitate deployment of some personal projects.
 Author: Carsten Knoll
 Author-email: carsten.knoll@posteo.de
 License: GNU General Public License v3
 Keywords: ssh,remote execution
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://cloud.drone.io/api/badges/cknoll/deploymentutils/status.svg)](https://cloud.drone.io/cknoll/deploymentutils)
@@ -103,9 +102,7 @@
 
 ## Known Issues
 
 - If a command started by `c.run("some_command")` is reading input, then the calling python process waits 'forever', i.e. until interrupted manually.
     - possible solution fragment: https://stackoverflow.com/questions/35751295/python-subprocess-check-to-see-if-the-executed-script-is-asking-for-user-input
 
 
-
-
```

### Comparing `deploymentutils-0.7.0/README.md` & `deploymentutils-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `deploymentutils-0.7.0/setup.py` & `deploymentutils-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `deploymentutils-0.7.0/src/deploymentutils/core.py` & `deploymentutils-0.8.0/src/deploymentutils/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -299,15 +299,15 @@
     ):
         """
 
         :param cmd:             the command to execute, preferably as a list like it is expected by subprocess
         :param use_dir:         boolean flag whether or not to use self.dir
         :param use_venv:        boolean flag whether or not to use self.venv_path
         :param hide:            see docs of invoke {"out", "err", True, False}
-        :param warn:            see docs of invoke and handling of "smart" bewlow
+        :param warn:            see docs of invoke and handling of "smart" below
         :param printonly:       flag for debugging
         :param target_spec:     str; default: "remote"
         :return:
         """
 
         # full_command_list will be a list of lists
         if isinstance(cmd, list):
@@ -717,15 +717,15 @@
     :param devmode:     Flag that triggers development mode (default: False).
                         If True variables which end with "__DEVMODE" will replace variables without such appendix
 
     :param start_dir:   (optional) start directory
 
     :return:    config object from decoupl module
     """
-    assert fname.endswith(".ini")
+    assert fname.endswith(".ini") or fname.endswith(".toml")
 
     path0, fname = os.path.split(fname)
 
     if path0 != "":
         assert start_dir is None
         assert limit is None
         path0 = os.path.abspath(path0)
@@ -751,37 +751,86 @@
             break
         path_list.insert(0, "..")
     else:
         msg = f"Could not find {fname} in current directory nor in {limit} parent dirs."
         raise FileNotFoundError(msg)
 
     # this is kept local to keep the dependency optional
-    from decouple import Config, RepositoryIni, Csv
 
-    config = Config(RepositoryIni(path))
+    if fname.endswith(".ini"):
+        from decouple import Config, RepositoryIni, Csv
+        config = Config(RepositoryIni(path))
+        config.settings_dict = config.repository.parser.__dict__["_sections"]["settings"]
+        config.Csv = Csv
+    elif fname.endswith(".toml"):
+        config = TOMLConfig(path)
 
     if devmode:
-        relevant_dict = config.repository.parser.__dict__["_sections"]["settings"]
-        for key, value in relevant_dict.items():
+        for key, value in config.settings_dict.items():
             # it seems that keys are converted to lowercase automatically
-            if key.endswith("__devmode"):
+            if "__" in key:
+                suffix = key.split("__")[-1]
+            else:
+                suffix = None
+            if suffix in ("devmode", "DEVMODE"):
 
                 # use the value specified for the development-mode for the actual variable (if it exists)
-                main_key = key.replace("__devmode", "")
-                if main_key in relevant_dict:
-                    relevant_dict[main_key] = value
+                main_key = key.replace(f"__{suffix}", "")
+                if main_key in config.settings_dict:
+                    config.settings_dict[main_key] = value
 
     # enable convenient access to Csv parser and actual path of the file
-    config.Csv = Csv
     config.path = os.path.abspath(path)
 
     os.chdir(old_dir)
     return config
 
 
+# based on decouple.Config
+class TOMLConfig(object):
+    """
+    Handle .toml file format used by Foreman.
+    """
+
+    def __init__(self, fpath):
+        try:
+            # this will be part of standard library for python >= 3.11
+            import tomllib
+        except ModuleNotFoundError:
+            import tomli as tomllib
+
+        with open(fpath, "rb") as fp:
+            complete_dict = tomllib.load(fp)
+            self.settings_dict = complete_dict["settings"]
+
+    @staticmethod
+    def _cast_do_nothing(value):
+        return value
+
+    def get(self, key, ignore_undefined=False, default=None):
+        """
+        Return the value for option or default if defined.
+        """
+
+        try:
+            value = self.settings_dict[key]
+        except KeyError:
+            if not ignore_undefined:
+                raise
+            value = default
+
+        return value
+
+    def __call__(self, *args, **kwargs):
+        """
+        Convenient shortcut to get.
+        """
+        return self.get(*args, **kwargs)
+
+
 def set_repo_tag(
     ref_path: str = None, message: str = None, repo_path: str = None, ask=True
 ) -> None:
     """
     Set a git tag to the current or specified repo (default: `deploy/<datetime>`)
 
     :param ref_path:    name of the tag; default: `deploy/<datetime>`
@@ -849,100 +898,139 @@
     else:
         print(bred(f"{url}: unexpected status code: {r.status_code}."))
         return 2
 
 
 def remove_secrets_from_config(path, new_path=None):
     """
-    Parse the ini file at `path` and create a copy where every non-comment line containing `pass` or `key`
+    Parse the ini/toml file at `path` and create a copy where every non-comment line containing `pass` or `key`
     has a dummy value.
 
+    NOTE: This function has no support for multiline assignments (allowed by toml)
+
     Use case: When developing deployment software with deployment tools, one often wants to share the
     general configuration but not the secrets. This function serves to automate this process.
 
     The dummy value is either generated or read from an actual variable name with the pattern
     `<secret-varname>-example`.  E.g. `my_pass-example = toFoh9pu`
 
     :param path:        path of the original file
     :param new_path:    (optional) path of new file to create
 
     :return:            `new_path`
     """
-    assert path.endswith(".ini")
+    if path.endswith(".ini"):
+        fname_suffix = ".ini"
+
+        # for ini-format: strings should not be quoted
+        quote_func = lambda x: x
 
-    config = configparser.ConfigParser()
-    config.optionxform = str  # preserve case when parsing the keys (non-default)
-    config.read(path)
+        config = configparser.ConfigParser()
+        config.optionxform = str  # preserve case when parsing the keys (non-default)
+        config.read(path)
+        keys = config["settings"].keys()
+        config.settings_dict = config["settings"]
+
+    elif path.endswith(".toml"):
+        fname_suffix = ".toml"
+        # for tomk-format: strings should be quoted
+        quote_func = repr
+        config = TOMLConfig(path)
+        keys = config.settings_dict.keys()
+    else:
+        msg = f"Unexpected file type (neither .ini nor .toml): of {path}"
+        raise TypeError(msg)
+
+    check_nested_dicts(config.settings_dict, level=0)
+
+    with open(path) as fp:
+        fulltext_lines = fp.readlines()
 
-    with open(path) as inifile:
-        fulltext_lines = inifile.readlines()
-    keys = config["settings"].keys()
+    critical_keys = []
+    for k in keys:
+        if contains_critical_token(k) and not k.endswith("__EXAMPLE"):
+            critical_keys.append(k)
 
-    critical_keys = [k for k in keys if (("pass" in k.lower()) or ("key" in k.lower())) and not k.endswith("__EXAMPLE")]
     keys_with_example_values = [k.replace("__EXAMPLE", "") for k in keys if k.endswith("__EXAMPLE")]
 
     critical_keys_with_example_values = set(critical_keys).intersection(keys_with_example_values)
     critical_keys = list(set(critical_keys) - set(keys_with_example_values))
 
     action_keys = critical_keys + keys_with_example_values
     result_lines = []
 
     for line in fulltext_lines:
 
         line = line.lstrip(" ")
         line_parts = line.split("=")
         for ak in action_keys:
-            # if line[:len(ck)] == ck:
-            if ak in line_parts[0]:
+            key_str = line_parts[0].strip()
+
+            if ak == key_str or key_str.replace(ak, "").startswith("__"):
                 # action-key found, no need to search further in this line
                 break
         else:
             # this else-branch is triggered if the inner for loop got no break
             # no critical key in this line
             # -> use this line and proceed to next one
             result_lines.append(line)
             continue
 
-        assert ak in line_parts[0]
+        assert ak in key_str
         if line.startswith("#"):
             # ignore this line (this might omit useful comments, but safety first!)
             continue
 
         if ak in critical_keys:
             n = 10
             xx = secrets.token_urlsafe(2 * n)
-            new_line = f"{ak} = {xx[:n]}--example-secret--{xx[n:]}\n"
+            new_line = f'{ak} = "{xx[:n]}--example-secret--{xx[n:]}"\n'
             result_lines.append(new_line)
         else:
             assert ak in keys_with_example_values
             if line.startswith(f"{ak}__EXAMPLE"):
                 # do not add the example-key-value-line to the output
                 # but only the real key with the example value
                 continue
-            example_value = config["settings"][f"{ak}__EXAMPLE"]
-            new_line = f"{ak} = {example_value}\n"
+            example_value = config.settings_dict[f"{ak}__EXAMPLE"]
+            new_line = f"{ak} = {quote_func(example_value)}\n"
             result_lines.append(new_line)
             # replacement_lines.append((ak, new_line))
 
     if new_path is None:
         if "production" in path:
             new_path = path.replace("production", "example")
         else:
-            new_path = path.replace(".ini", "-example.ini")
+            new_path = path.replace(fname_suffix, f"-example{fname_suffix}")
     else:
         if new_path == path:
             raise ValueError("new_path must be different from original path")
 
     with open(new_path, "w") as inifile:
         inifile.writelines(result_lines)
 
     print("The values for the following keys were replaced: ", ", ".join(critical_keys))
     print("File written", new_path)
     return new_path
 
+def contains_critical_token(keystr):
+    kl = keystr.lower()
+    return (("pass" in kl) or ("key" in kl) or ("secret" in kl))
+
+def check_nested_dicts(some_dict, level):
+    for key, value in some_dict.items():
+        if isinstance(value, dict):
+            if contains_critical_token(key):
+                msg = f"{key} is not allowed as name of a table (cannot remove secrets)"
+                raise ValueError(msg)
+            else:
+                check_nested_dicts(value, level+1)
+        elif level > 0 and contains_critical_token(key):
+            msg = f"{key} is not allowed as name of a table entry (cannot remove secrets)"
+            raise ValueError(msg)
 
 # noinspection PyShadowingBuiltins
 def get_deployment_date(fpath: str, format="%Y-%m-%d %H:%M:%S") -> str:
     """
     Find out the modification date of a file and return it
 
     :param fpath:
```

### Comparing `deploymentutils-0.7.0/src/deploymentutils.egg-info/PKG-INFO` & `deploymentutils-0.8.0/src/deploymentutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: deploymentutils
-Version: 0.7.0
+Version: 0.8.0
 Summary: Small python package to facilitate deployment of some personal projects.
 Author: Carsten Knoll
 Author-email: carsten.knoll@posteo.de
 License: GNU General Public License v3
 Keywords: ssh,remote execution
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://cloud.drone.io/api/badges/cknoll/deploymentutils/status.svg)](https://cloud.drone.io/cknoll/deploymentutils)
@@ -103,9 +102,7 @@
 
 ## Known Issues
 
 - If a command started by `c.run("some_command")` is reading input, then the calling python process waits 'forever', i.e. until interrupted manually.
     - possible solution fragment: https://stackoverflow.com/questions/35751295/python-subprocess-check-to-see-if-the-executed-script-is-asking-for-user-input
 
 
-
-
```

### Comparing `deploymentutils-0.7.0/test/test_core.py` & `deploymentutils-0.8.0/test/test_core.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,24 +20,32 @@
 These tests only cover a fraction of the actual features. Some tests require access to a remote machine.
 
 
 run tests locally with:
 `export NOREMOTE=True; python -m unittest`
 or
 `export NOREMOTE=True; rednose`
+`export NOREMOTE=True; pytest -s`
+
+to run with remote access, unlock the ssh key and use e.g
+`pytest -s`
+
+
+
 """
 
 DIR_OF_THIS_FILE = os.path.dirname(os.path.abspath(sys.modules.get(__name__).__file__))
 
 TEMPLATEDIR = os.path.join(DIR_OF_THIS_FILE, "_test_templates")
 TESTDATADIR = os.path.join(DIR_OF_THIS_FILE, "_test_data")
 TESTJSONDATADIR = os.path.join(DIR_OF_THIS_FILE, "_test_json_data")
 
 # noinspection PyPep8Naming
 CONFIG_FNAME = "test_config.ini"
+CONFIG_FNAME_TOML = "test_config.toml"
 
 
 class NoRemote(Exception):
     pass
 
 
 # because uberspace offers many pip_commands:
@@ -77,22 +85,24 @@
     try:
         sys.stdout, sys.stderr = new_out, new_err
         yield sys.stdout, sys.stderr
     finally:
         sys.stdout, sys.stderr = old_out, old_err
 
 
-class TC1(unittest.TestCase):
+class LocalFileDeletingTestCase(unittest.TestCase):
     def setUp(self):
         self.local_files_to_delete = []
 
     def tearDown(self):
         for path in self.local_files_to_delete:
             os.unlink(path)
 
+
+class TC1(LocalFileDeletingTestCase):
     def test_get_dir_of_this_file(self):
         test_path = get_dir_of_this_file()
 
         expected_path = "test"
         self.assertTrue(test_path.endswith(expected_path))
 
     def test_render_remplate(self):
@@ -262,18 +272,18 @@
         self.assertRaises(
             FileNotFoundError,
             du.get_nearest_config,
             fname=target_name,
             start_dir=DIR_OF_THIS_FILE,
             limit=1,
         )
+        self.local_files_to_delete.append(target_path)
 
         config2 = du.get_nearest_config(target_name, start_dir=DIR_OF_THIS_FILE, limit=2)
         self.assertEqual(config2("testvalue1"), "OK")
-        os.remove(target_path)
 
         abspath = "/does/not/exist.ini"
 
         self.assertRaises(FileNotFoundError, du.get_nearest_config, fname=abspath, start_dir=None)
 
         abspath = os.path.join(DIR_OF_THIS_FILE, "test_config.ini")
         config3 = du.get_nearest_config(abspath)
@@ -332,16 +342,18 @@
         self.local_files_to_delete.append(new_path)
         public_config = du.get_nearest_config(new_path)
 
         self.assertEqual(secret_config("testvalue5"), public_config("testvalue5"))
 
         self.assertNotEqual(secret_config("test_pass1"), public_config("test_pass1"))
         self.assertNotEqual(secret_config("test_key1"), public_config("test_key1"))
+        self.assertNotEqual(secret_config("test_secret1"), public_config("test_secret1"))
         self.assertIn("--example-secret--", public_config("test_pass1"))
         self.assertIn("--example-secret--", public_config("test_key1"))
+        self.assertIn("--example-secret--", public_config("test_secret1"))
 
         example_value1 = secret_config("testvalue1__EXAMPLE")
         example_value2 = secret_config("testvalue2__EXAMPLE")
         self.assertRaises(decouple.UndefinedValueError, public_config, "testvalue1__EXAMPLE")
         self.assertRaises(decouple.UndefinedValueError, public_config, "testvalue2__EXAMPLE")
 
         self.assertEqual(example_value1, public_config("testvalue1"))
@@ -362,14 +374,125 @@
         self.assertTrue(dt < 1.0)
 
         dep_date = du.get_deployment_date("__not_existing_file__")
         self.assertEqual(dep_date, "<not available>")
 
 
 
+class TC1b(LocalFileDeletingTestCase):
+    def test_get_nearest_config_toml(self):
+
+        # explicitly passing start_dir seems only necessary in unittests
+
+        config = du.get_nearest_config(CONFIG_FNAME_TOML, start_dir=DIR_OF_THIS_FILE)
+
+        self.assertEqual(config("testvalue1"), "OK")
+        self.assertEqual(config("testvalue2"), "Very OK")
+        self.assertEqual(config("testvalue3"), "Robust=OK")
+        self.assertEqual(config("testvalue4"), '"Quoted String"')
+        self.assertEqual(config("testvalue5"), "Spaces are acceptable")
+        self.assertEqual(config("testvalue_number"), 1234.567)
+
+        # arrays are a special feature of TOML; no need for CSV
+        self.assertEqual(
+            config("testvalue_array"), ["string1", "string2", "some more words"]
+        )
+        # tables are a special feature of TOML; -> result in a dict
+
+        tab = config("table1")
+        self.assertEqual(tab["testvalue8"], "value inside a TOML table")
+        self.assertEqual(tab["testvalue9"], True)
+        self.assertEqual(tab["testvalue10"], False)
+
+        self.assertEqual(config("testvalue_empty_str"), "")
+        self.assertEqual(config("testvalue6"), "production_option")
+        self.assertEqual(config("testvalue6__DEVMODE"), "development_option")
+        self.assertEqual(config("testvalueX__DEVMODE"), "does not exist for production")
+
+        self.assertRaises(KeyError, config, "testvalueX")
+
+        config_dev = du.get_nearest_config(CONFIG_FNAME_TOML, devmode=True, start_dir=DIR_OF_THIS_FILE)
+        self.assertEqual(config_dev("testvalue6"), "development_option")
+
+        # now make a copy of the config file and place it in a parent dir
+
+        target_name = CONFIG_FNAME_TOML.replace(".toml", "_toml.ini")
+        target_path = os.path.join(DIR_OF_THIS_FILE, "..", "..", target_name)
+        self.assertRaises(FileNotFoundError, du.get_nearest_config, fname=target_name)
+
+        source_path = os.path.join(DIR_OF_THIS_FILE, CONFIG_FNAME)
+
+        shutil.copy2(source_path, target_path)
+        self.assertRaises(
+            FileNotFoundError,
+            du.get_nearest_config,
+            fname=target_name,
+            start_dir=DIR_OF_THIS_FILE,
+            limit=1,
+        )
+        self.local_files_to_delete.append(target_path)
+
+        config2 = du.get_nearest_config(target_name, start_dir=DIR_OF_THIS_FILE, limit=2)
+        self.assertEqual(config2("testvalue1"), "OK")
+
+        abspath = "/does/not/exist.ini"
+
+        self.assertRaises(FileNotFoundError, du.get_nearest_config, fname=abspath, start_dir=None)
+
+        abspath = os.path.join(DIR_OF_THIS_FILE, "test_config.toml")
+        config3 = du.get_nearest_config(abspath)
+        self.assertEqual(config3("testvalue1"), "OK")
+
+    def test_remove_secrets_from_config_toml(self):
+
+        # explicitly passing start_dir seems only necessary in unittests
+        secret_config = du.get_nearest_config(CONFIG_FNAME_TOML, start_dir=DIR_OF_THIS_FILE)
+
+        new_path = du.remove_secrets_from_config(secret_config.path)
+        self.local_files_to_delete.append(new_path)
+        public_config = du.get_nearest_config(new_path)
+
+        self.assertEqual(secret_config("testvalue5"), public_config("testvalue5"))
+
+        self.assertNotEqual(secret_config("test_pass1"), public_config("test_pass1"))
+        self.assertNotEqual(secret_config("test_key1"), public_config("test_key1"))
+        self.assertNotEqual(secret_config("test_secret1"), public_config("test_secret1"))
+        self.assertIn("--example-secret--", public_config("test_pass1"))
+        self.assertIn("--example-secret--", public_config("test_key1"))
+        self.assertIn("--example-secret--", public_config("test_secret1"))
+
+        example_value1 = secret_config("testvalue1__EXAMPLE")
+        example_value2 = secret_config("testvalue2__EXAMPLE")
+        self.assertRaises(KeyError, public_config, "testvalue1__EXAMPLE")
+        self.assertRaises(KeyError, public_config, "testvalue2__EXAMPLE")
+
+        self.assertEqual(example_value1, public_config("testvalue1"))
+        self.assertEqual(example_value2, public_config("testvalue2"))
+        self.assertEqual(public_config("testvalue7"), "string conatining testvalue1")
+
+        self.assertEqual(public_config("test_key2"), secret_config("test_key2__EXAMPLE"))
+
+        # check tables:
+        with open(CONFIG_FNAME_TOML) as fp:
+            full_text = fp.read()
+
+        # introduce a secret value inside a table
+        bad_full_text = full_text.replace("# XXX secret-test", 'testvalue11_key = "secret inside table"')
+
+        with open(new_path, "w") as fp:
+            fp.write(bad_full_text)
+        self.assertRaises(ValueError, du.remove_secrets_from_config, new_path)
+
+        # introduce a secret value indicator as table name
+        bad_full_text = full_text.replace("[settings.table1]", '[settings.secret_table1]')
+
+        with open(new_path, "w") as fp:
+            fp.write(bad_full_text)
+        self.assertRaises(ValueError, du.remove_secrets_from_config, new_path)
+
 
 @unittest.skipUnless(remote_server is not None, "no remote server specified")
 class TC2(unittest.TestCase):
     def setUp(self):
         self.c = du.StateConnection(remote_server, user=remote_user, target="remote")
         pass
```

