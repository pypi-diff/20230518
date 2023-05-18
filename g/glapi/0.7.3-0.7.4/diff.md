# Comparing `tmp/glapi-0.7.3.tar.gz` & `tmp/glapi-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glapi-0.7.3.tar", last modified: Wed Apr 19 23:28:32 2023, max compression
+gzip compressed data, was "glapi-0.7.4.tar", last modified: Thu May 18 18:47:24 2023, max compression
```

## Comparing `glapi-0.7.3.tar` & `glapi-0.7.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 23:28:32.398032 glapi-0.7.3/
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-04-19 23:28:22.000000 glapi-0.7.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      307 2023-04-19 23:28:32.397032 glapi-0.7.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-04-19 23:28:22.000000 glapi-0.7.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-19 23:28:22.000000 glapi-0.7.3/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 23:28:32.396031 glapi-0.7.3/glapi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 23:28:22.000000 glapi-0.7.3/glapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      731 2023-04-19 23:28:22.000000 glapi-0.7.3/glapi/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     3655 2023-04-19 23:28:22.000000 glapi-0.7.3/glapi/connection.py
--rw-rw-rw-   0 root         (0) root         (0)     5925 2023-04-19 23:28:22.000000 glapi-0.7.3/glapi/epic.py
--rw-rw-rw-   0 root         (0) root         (0)     4800 2023-04-19 23:28:22.000000 glapi-0.7.3/glapi/group.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2023-04-19 23:28:22.000000 glapi-0.7.3/glapi/issue.py
--rw-rw-rw-   0 root         (0) root         (0)     4459 2023-04-19 23:28:22.000000 glapi-0.7.3/glapi/project.py
--rw-rw-rw-   0 root         (0) root         (0)     6845 2023-04-19 23:28:22.000000 glapi-0.7.3/glapi/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 23:28:32.397032 glapi-0.7.3/glapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      307 2023-04-19 23:28:32.000000 glapi-0.7.3/glapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      357 2023-04-19 23:28:32.000000 glapi-0.7.3/glapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 23:28:32.000000 glapi-0.7.3/glapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-04-19 23:28:32.000000 glapi-0.7.3/glapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-19 23:28:32.000000 glapi-0.7.3/glapi.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-19 23:28:22.000000 glapi-0.7.3/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-04-19 23:28:22.000000 glapi-0.7.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 23:28:32.398032 glapi-0.7.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      698 2023-04-19 23:28:22.000000 glapi-0.7.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:47:23.998247 glapi-0.7.4/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-05-18 18:47:16.000000 glapi-0.7.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      307 2023-05-18 18:47:23.998247 glapi-0.7.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-05-18 18:47:16.000000 glapi-0.7.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-18 18:47:16.000000 glapi-0.7.4/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:47:23.997331 glapi-0.7.4/glapi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-18 18:47:16.000000 glapi-0.7.4/glapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      731 2023-05-18 18:47:16.000000 glapi-0.7.4/glapi/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     3655 2023-05-18 18:47:16.000000 glapi-0.7.4/glapi/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     5925 2023-05-18 18:47:16.000000 glapi-0.7.4/glapi/epic.py
+-rw-rw-rw-   0 root         (0) root         (0)     4745 2023-05-18 18:47:16.000000 glapi-0.7.4/glapi/group.py
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2023-05-18 18:47:16.000000 glapi-0.7.4/glapi/issue.py
+-rw-rw-rw-   0 root         (0) root         (0)     5175 2023-05-18 18:47:16.000000 glapi-0.7.4/glapi/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2023-05-18 18:47:16.000000 glapi-0.7.4/glapi/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:47:23.998247 glapi-0.7.4/glapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      307 2023-05-18 18:47:23.000000 glapi-0.7.4/glapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      357 2023-05-18 18:47:23.000000 glapi-0.7.4/glapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 18:47:23.000000 glapi-0.7.4/glapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-05-18 18:47:23.000000 glapi-0.7.4/glapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-18 18:47:23.000000 glapi-0.7.4/glapi.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-18 18:47:16.000000 glapi-0.7.4/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-05-18 18:47:16.000000 glapi-0.7.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 18:47:23.998247 glapi-0.7.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      698 2023-05-18 18:47:16.000000 glapi-0.7.4/setup.py
```

### Comparing `glapi-0.7.3/glapi/configuration.py` & `glapi-0.7.4/glapi/configuration.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.3/glapi/connection.py` & `glapi-0.7.4/glapi/connection.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.3/glapi/epic.py` & `glapi-0.7.4/glapi/epic.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.3/glapi/group.py` & `glapi-0.7.4/glapi/project.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,142 +1,138 @@
 from glapi import configuration
 from glapi.connection import GitlabConnection
+from glapi.issue import GitlabIssue
 
-class GitlabGroup:
+class GitlabProject:
     """
-    GitlabGroup is a Gitlab Group.
+    GitlabProject is a Gitlab Project.
     """
 
-    def __init__(self, id: str = None, group: dict = None, token :str = configuration.GITLAB_TOKEN, version: str = configuration.GITLAB_API_VERSION):
+    def __init__(self, id: str = None, project: dict = None, connection: GitlabConnection = None, event_actions: list = None, get_members: bool = False, get_events: bool = False, token :str = configuration.GITLAB_TOKEN, version: str = configuration.GITLAB_API_VERSION):
         """
         Args:
+            connection (GitlabConnection): glapi connection
+            event_actions (list): strings of Gitlab User contribution types https://docs.gitlab.com/ee/user/index.html#user-contribution-events
+            get_events (bool): TRUE if should pull events
+            get_members (bool): TRUE if should pull user membership
             id (string): GitLab Project id
-            group (dictionary): GitLab Group
+            project (dictionary): GitLab Project
             token (string): GitLab personal access or deploy token
             version (string): GitLab API version as base url
         """
-        self.connection = GitlabConnection(
-            token=token,
-            version=version
-        )
-        self.group = group if group else (self.connection.query("groups/%s" % id)["data"] if id and token and version else None)
-        self.id = self.group["id"] if self.group else None
+        self.connection = connection if connection else GitlabConnection(token=token, version=version)
+        self.gitlab_type = "project"
+        self.project = project if project else (self.connection.query("projects/%s" % id)["data"] if id and token and version else None)
+        self.id = self.project["id"] if self.project else None
+        self.events = self.extract_events(actions=event_actions) if get_events else None
+        self.membership = self.extract_members() if get_members else None
 
-    def extract_epics(self, date_start: str = None, date_end: str = None, group_users: list = None, get_issues: bool = False, get_notes: bool = False, get_participants: bool = False) -> list:
+    def extract_events(self, actions: list, date_start: str = None, date_end: str = None) -> dict:
         """
-        Extract group-specific epic data.
+        Extract project-specific event data.
 
         Args:
+            actions (list): enums where each represent an event action type https://docs.gitlab.com/ee/user/index.html#user-contribution-events
             date_end (string): iso 8601 date value
             date_start (string): iso 8601 date value
-            get_issues (boolean): TRUE if issues should be pulled
-            get_notes (boolean): TRUE if notes should be pulled
-            get_participants (boolean): TRUE if participants should be pulled
-            group_users (list): classes of GitlabUser
 
         Returns:
-            A list of GitlabEpic classes where each represents a GtiLab Epic.
+            A dictionary where keys are event action types and corresponding values are lists of dictionaries where each represents a GitLab Event.
         """
 
-        result = None
-        params = dict()
+        result = list()
 
-        # check params
-        if date_end: params["created_before"] = date_end
-        if date_start: params["created_after"] = date_start
-
-        # check connection params
+        # check for connection ready
         if self.id and self.connection.token and self.connection.version:
 
-            # query api
-            result = self.connection.paginate(
-                endpoint="groups/%s/epics" % self.id,
-                params=params
-            )
+            # loop through actions
+            for action in actions:
 
-        return result
+                # check params
+                if date_start or date_end or actions: params = dict()
+                if date_end: params["created_before"] = date_end
+                if date_start: params["created_after"] = date_start
 
-    def extract_issues(self, scope: str = "all", date_start: str = None, date_end: str = None, get_notes: bool = False, get_links: bool = False, get_participants: bool = False) -> list:
-        """
-        Extract group-specific epic data.
+                # update for action
+                params["action"] = action
 
-        Args:
-            date_end (string): iso 8601 date value
-            date_start (string): iso 8601 date value
-            get_links (boolean): TRUE if links should be pulled
-            get_notes (boolean): TRUE if notes should be pulled
-            get_participants (boolean): TRUE if participants should be pulled
-            scope (enum): all | assigned_to_me | created_by_me
+                # get events
+                result += self.connection.paginate(
+                    endpoint="projects/%s/events" % self.id,
+                    params=params
+                )
+
+        return result if result else None
+
+    def extract_languages(self) -> list:
+        """
+        Extract project-specific language data.
 
         Returns:
-            A list of GitlabIssue classes where each represents a GtiLab Issue.
+            A dictionary of key/value pairs where each key is a coding language and corresponding value is a float representing the coverage of the language in the project.
         """
 
         result = None
 
-        # check params
-        if date_start or date_end or scope: params = dict()
-        if date_end: params["created_before"] = date_end
-        if date_start: params["created_after"] = date_start
-        if scope: params["scope"] = scope
-
         # check connection params
         if self.id and self.connection.token and self.connection.version:
 
             # query api
             result = self.connection.paginate(
-                endpoint="groups/%s/issues" % self.id,
-                params=params
+                endpoint="projects/%s/languages" % self.id
             )
 
         return result
 
-    def extract_projects(self, date_start: str = None, date_end: str = None) -> list:
+    def extract_issues(self, labels: str = None, scope: str = "all", date_start: str = None, date_end: str = None) -> list:
         """
-        Extract group-specific project data.
+        Extract group-specific epic data.
 
         Args:
             date_end (string): iso 8601 date value
             date_start (string): iso 8601 date value
+            labels (string): comma-delimitered list of labels | all | any
+            scope (enum): all | assigned_to_me | created_by_me
 
         Returns:
-            A list of GitlabProject classes where each represents a GtiLab Project.
+            A list of GitlabIssue classes where each represents a GtiLab Issue.
         """
 
         result = None
-        params = dict()
 
         # check params
-        if date_start or date_end: params = dict()
+        if date_start or date_end or scope: params = dict()
         if date_end: params["created_before"] = date_end
         if date_start: params["created_after"] = date_start
+        if labels: params["labels"] = labels
+        if scope: params["scope"] = scope
 
         # check connection params
         if self.id and self.connection.token and self.connection.version:
 
             # query api
             result = self.connection.paginate(
-                endpoint="groups/%s/projects" % self.id,
+                endpoint="projects/%s/issues" % self.id,
                 params=params
             )
 
         return result
 
-    def extract_users(self) -> list:
+    def extract_members(self) -> list:
         """
-        Extract group-specific user data.
+        Extract project-specific member data.
 
         Returns:
-            A list of GitlabUser classes where each represents a GtiLab User.
+            A list of dictionaries where each represents a GtiLab User.
         """
 
         result = None
 
         # check connection params
         if self.id and self.connection.token and self.connection.version:
 
             # query api
             result = self.connection.paginate(
-                endpoint="groups/%s/members" % self.id
+                endpoint="projects/%s/members" % self.id
             )
 
         return result
```

### Comparing `glapi-0.7.3/glapi/issue.py` & `glapi-0.7.4/glapi/issue.py`

 * *Files identical despite different names*

### Comparing `glapi-0.7.3/glapi/user.py` & `glapi-0.7.4/glapi/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,33 +86,35 @@
                 result = self.connection.paginate(
                     endpoint="users/%s/events" % self.id,
                     params=params
                 )
 
         return result if result else None
 
-    def extract_issues(self, scope: str, date_start: str = None, date_end: str = None) -> list:
+    def extract_issues(self, labels: str = None, scope: str = "all", date_start: str = None, date_end: str = None) -> list:
         """
-        Extract user-specific issue data.
+        Extract group-specific epic data.
 
         Args:
             date_end (string): iso 8601 date value
             date_start (string): iso 8601 date value
-            scope (enum): "assigned_to_me" | "created_by_me"
+            labels (string): comma-delimitered list of labels | all | any
+            scope (enum): all | assigned_to_me | created_by_me
 
         Returns:
-            A list of dictionaries where each represents a GtiLab Issue.
+            A list of GitlabIssue classes where each represents a GtiLab Issue.
         """
 
         result = None
-        params = dict()
 
         # check params
+        if date_start or date_end or scope: params = dict()
         if date_end: params["created_before"] = date_end
         if date_start: params["created_after"] = date_start
+        if labels: params["labels"] = labels
         if scope: params["scope"] = scope
 
         # check connection params
         if self.id and self.connection.token and self.connection.version:
 
             # query api for issues
             result = self.connection.paginate(
```

### Comparing `glapi-0.7.3/setup.py` & `glapi-0.7.4/setup.py`

 * *Files identical despite different names*

