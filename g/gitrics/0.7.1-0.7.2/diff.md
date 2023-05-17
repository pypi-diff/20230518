# Comparing `tmp/gitrics-0.7.1.tar.gz` & `tmp/gitrics-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitrics-0.7.1.tar", last modified: Mon Feb 21 18:10:30 2022, max compression
+gzip compressed data, was "gitrics-0.7.2.tar", last modified: Wed May 17 22:48:53 2023, max compression
```

## Comparing `gitrics-0.7.1.tar` & `gitrics-0.7.2.tar`

### file list

```diff
@@ -1,48 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-21 18:10:30.642743 gitrics-0.7.1/
--rw-rw-rw-   0 root         (0) root         (0)       42 2022-02-21 18:10:21.000000 gitrics-0.7.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      422 2022-02-21 18:10:30.642743 gitrics-0.7.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      159 2022-02-21 18:10:21.000000 gitrics-0.7.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2022-02-21 18:10:21.000000 gitrics-0.7.1/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-21 18:10:30.633742 gitrics-0.7.1/gitrics/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-21 18:10:30.640743 gitrics-0.7.1/gitrics/bin/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/bin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3638 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/bin/generate_dependency_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     1725 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/bin/generate_group_blockers.py
--rw-rw-rw-   0 root         (0) root         (0)     1778 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/bin/generate_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/bin/generate_user_activity.py
--rw-rw-rw-   0 root         (0) root         (0)     2446 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/bin/generate_user_color.py
--rw-rw-rw-   0 root         (0) root         (0)     5383 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/bin/generate_user_connection.py
--rw-rw-rw-   0 root         (0) root         (0)    16263 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/bin/generate_user_contribution.py
--rw-rw-rw-   0 root         (0) root         (0)     1615 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/bin/generate_user_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3107 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/bin/generate_user_data_coverage.py
--rw-rw-rw-   0 root         (0) root         (0)     3133 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/bin/generate_user_languages.py
--rw-rw-rw-   0 root         (0) root         (0)     4041 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/bin/generate_user_profile.py
--rw-rw-rw-   0 root         (0) root         (0)     6252 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/bin/generate_user_project_membership.py
--rw-rw-rw-   0 root         (0) root         (0)     3167 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/bin/generate_user_topics.py
--rw-rw-rw-   0 root         (0) root         (0)     5095 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/bin/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2446 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     2804 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/epic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-21 18:10:30.641743 gitrics-0.7.1/gitrics/group/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/group/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1841 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/group/group.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/group/users.py
--rw-rw-rw-   0 root         (0) root         (0)     1324 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/issue.py
--rw-rw-rw-   0 root         (0) root         (0)    11907 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/itemset.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/project.py
--rw-rw-rw-   0 root         (0) root         (0)     9768 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/set.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-21 18:10:30.641743 gitrics-0.7.1/gitrics/user/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/user/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1046 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/user/user.py
--rw-rw-rw-   0 root         (0) root         (0)     2036 2022-02-21 18:10:21.000000 gitrics-0.7.1/gitrics/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-21 18:10:30.635742 gitrics-0.7.1/gitrics.egg-info/
--rw-r--r--   0 root         (0) root         (0)      422 2022-02-21 18:10:30.000000 gitrics-0.7.1/gitrics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1093 2022-02-21 18:10:30.000000 gitrics-0.7.1/gitrics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-21 18:10:30.000000 gitrics-0.7.1/gitrics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      892 2022-02-21 18:10:30.000000 gitrics-0.7.1/gitrics.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-02-21 18:10:30.000000 gitrics-0.7.1/gitrics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-02-21 18:10:30.000000 gitrics-0.7.1/gitrics.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2022-02-21 18:10:21.000000 gitrics-0.7.1/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)       41 2022-02-21 18:10:21.000000 gitrics-0.7.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-02-21 18:10:30.642743 gitrics-0.7.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1821 2022-02-21 18:10:21.000000 gitrics-0.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:48:53.024736 gitrics-0.7.2/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-05-17 22:48:45.000000 gitrics-0.7.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      386 2023-05-17 22:48:53.024736 gitrics-0.7.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      159 2023-05-17 22:48:45.000000 gitrics-0.7.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-17 22:48:45.000000 gitrics-0.7.2/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:48:53.023736 gitrics-0.7.2/gitrics/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 22:48:45.000000 gitrics-0.7.2/gitrics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:48:53.024736 gitrics-0.7.2/gitrics/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 22:48:45.000000 gitrics-0.7.2/gitrics/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24306 2023-05-17 22:48:45.000000 gitrics-0.7.2/gitrics/cli/gitrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2500 2023-05-17 22:48:45.000000 gitrics-0.7.2/gitrics/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:48:53.024736 gitrics-0.7.2/gitrics/project/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 22:48:45.000000 gitrics-0.7.2/gitrics/project/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7609 2023-05-17 22:48:45.000000 gitrics-0.7.2/gitrics/project/enrichment.py
+-rw-rw-rw-   0 root         (0) root         (0)    26279 2023-05-17 22:48:45.000000 gitrics-0.7.2/gitrics/user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1718 2023-05-17 22:48:45.000000 gitrics-0.7.2/gitrics/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:48:53.023736 gitrics-0.7.2/gitrics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      386 2023-05-17 22:48:52.000000 gitrics-0.7.2/gitrics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2023-05-17 22:48:53.000000 gitrics-0.7.2/gitrics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 22:48:52.000000 gitrics-0.7.2/gitrics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-17 22:48:52.000000 gitrics-0.7.2/gitrics.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-05-17 22:48:52.000000 gitrics-0.7.2/gitrics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-17 22:48:52.000000 gitrics-0.7.2/gitrics.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-17 22:48:45.000000 gitrics-0.7.2/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-05-17 22:48:45.000000 gitrics-0.7.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 22:48:53.024736 gitrics-0.7.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      832 2023-05-17 22:48:45.000000 gitrics-0.7.2/setup.py
```

### Comparing `gitrics-0.7.1/gitrics/utilities.py` & `gitrics-0.7.2/gitrics/utilities.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,20 +45,7 @@
     """
 
     # convert time
     dt_end = datetime.datetime.strptime(date_end, "%Y-%m-%d")
     dt_start = datetime.datetime.strptime(date_start, "%Y-%m-%d") if date_start and date_end and date_start != date_end else dt_end - datetime.timedelta(3)
 
     return (dt_start, dt_end)
-
-def parse_multi_parameters(value):
-    """
-    Parse a string of comma-delimetered values into a native python list.
-
-    Args:
-        value (string): comma-delimetered value
-
-    Returns:
-        A list of strings where each is a discrete value in the set.
-    """
-
-    return value.split(",") if value else list()
```

