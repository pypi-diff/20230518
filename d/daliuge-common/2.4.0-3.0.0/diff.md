# Comparing `tmp/daliuge-common-2.4.0.tar.gz` & `tmp/daliuge-common-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daliuge-common-2.4.0.tar", last modified: Sat Mar 11 06:01:19 2023, max compression
+gzip compressed data, was "daliuge-common-3.0.0.tar", last modified: Thu May 18 12:49:51 2023, max compression
```

## Comparing `daliuge-common-2.4.0.tar` & `daliuge-common-3.0.0.tar`

### file list

```diff
@@ -1,41 +1,35 @@
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:19.863368 daliuge-common-2.4.0/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      340 2023-03-11 06:01:19.863368 daliuge-common-2.4.0/PKG-INFO
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      654 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/README.md
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     1888 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/build_common.sh
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:19.859368 daliuge-common-2.4.0/daliuge_common.egg-info/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      340 2023-03-11 06:01:19.000000 daliuge-common-2.4.0/daliuge_common.egg-info/PKG-INFO
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      893 2023-03-11 06:01:19.000000 daliuge-common-2.4.0/daliuge_common.egg-info/SOURCES.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        1 2023-03-11 06:01:19.000000 daliuge-common-2.4.0/daliuge_common.egg-info/dependency_links.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       45 2023-03-11 06:01:19.000000 daliuge-common-2.4.0/daliuge_common.egg-info/entry_points.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       29 2023-03-11 06:01:19.000000 daliuge-common-2.4.0/daliuge_common.egg-info/requires.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        4 2023-03-11 06:01:19.000000 daliuge-common-2.4.0/daliuge_common.egg-info/top_level.txt
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:19.859368 daliuge-common-2.4.0/dlg/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1275 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/dlg/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9571 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/dlg/clients.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:19.859368 daliuge-common-2.4.0/dlg/common/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9055 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/dlg/common/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1109 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/dlg/common/deployment_methods.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1451 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/dlg/common/k8s_utils.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6305 2023-02-01 12:39:07.000000 daliuge-common-2.4.0/dlg/common/network.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1987 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/dlg/common/osutils.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:19.859368 daliuge-common-2.4.0/dlg/common/reproducibility/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        0 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/dlg/common/reproducibility/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4420 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/dlg/common/reproducibility/constants.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7505 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/dlg/common/reproducibility/reprodata_compare.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    32970 2023-01-20 05:49:49.000000 daliuge-common-2.4.0/dlg/common/reproducibility/reproducibility.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9084 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/dlg/common/reproducibility/reproducibility_fields.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5843 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/dlg/common/streams.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5123 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/dlg/common/tool.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      199 2023-03-11 06:01:19.000000 daliuge-common-2.4.0/dlg/common/version.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1850 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/dlg/constants.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4834 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/dlg/exceptions.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6972 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/dlg/restutils.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2210 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/dlg/version_helper.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:19.863368 daliuge-common-2.4.0/docker/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      585 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/docker/Dockerfile
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1957 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/docker/Dockerfile.casa
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      620 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/docker/Dockerfile.dev
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1423 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/docker/Dockerfile.devcuda
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      632 2022-11-30 13:05:02.000000 daliuge-common-2.4.0/docker/Dockerfile.ray
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       38 2023-03-11 06:01:19.863368 daliuge-common-2.4.0/setup.cfg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2454 2023-03-11 05:57:46.000000 daliuge-common-2.4.0/setup.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.340462 daliuge-common-3.0.0/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      321 2023-05-18 12:49:51.340462 daliuge-common-3.0.0/PKG-INFO
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      654 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/README.md
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.340462 daliuge-common-3.0.0/daliuge_common.egg-info/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      321 2023-05-18 12:49:51.000000 daliuge-common-3.0.0/daliuge_common.egg-info/PKG-INFO
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      779 2023-05-18 12:49:51.000000 daliuge-common-3.0.0/daliuge_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        1 2023-05-18 12:49:51.000000 daliuge-common-3.0.0/daliuge_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       44 2023-05-18 12:49:51.000000 daliuge-common-3.0.0/daliuge_common.egg-info/entry_points.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       29 2023-05-18 12:49:51.000000 daliuge-common-3.0.0/daliuge_common.egg-info/requires.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        4 2023-05-18 12:49:51.000000 daliuge-common-3.0.0/daliuge_common.egg-info/top_level.txt
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.340462 daliuge-common-3.0.0/dlg/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1275 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9571 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/clients.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.340462 daliuge-common-3.0.0/dlg/common/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8417 2023-05-18 12:40:21.000000 daliuge-common-3.0.0/dlg/common/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1109 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/common/deployment_methods.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1451 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/common/k8s_utils.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6305 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/common/network.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1987 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/common/osutils.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.340462 daliuge-common-3.0.0/dlg/common/reproducibility/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/common/reproducibility/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4420 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/common/reproducibility/constants.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7505 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/common/reproducibility/reprodata_compare.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    33879 2023-05-18 12:40:21.000000 daliuge-common-3.0.0/dlg/common/reproducibility/reproducibility.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8979 2023-05-18 12:40:21.000000 daliuge-common-3.0.0/dlg/common/reproducibility/reproducibility_fields.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5843 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/common/streams.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5123 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/common/tool.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      199 2023-05-18 12:49:51.000000 daliuge-common-3.0.0/dlg/common/version.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1850 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/constants.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4834 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/exceptions.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7029 2023-05-18 12:40:21.000000 daliuge-common-3.0.0/dlg/restutils.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16698 2023-05-18 12:40:21.000000 daliuge-common-3.0.0/dlg/utils.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2210 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/version_helper.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       38 2023-05-18 12:49:51.340462 daliuge-common-3.0.0/setup.cfg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2454 2023-05-18 12:43:13.000000 daliuge-common-3.0.0/setup.py
```

### Comparing `daliuge-common-2.4.0/README.md` & `daliuge-common-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `daliuge-common-2.4.0/dlg/__init__.py` & `daliuge-common-3.0.0/dlg/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-2.4.0/dlg/clients.py` & `daliuge-common-3.0.0/dlg/clients.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-2.4.0/dlg/common/__init__.py` & `daliuge-common-3.0.0/dlg/common/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,106 +15,39 @@
 #    Lesser General Public License for more details.
 #
 #    You should have received a copy of the GNU Lesser General Public
 #    License along with this library; if not, write to the Free Software
 #    Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 #    MA 02111-1307  USA
 #
+from enum import Enum
+from dataclasses import dataclass, field, asdict
+import logging
+
 """Common utilities used by daliuge packages"""
 from .osutils import terminate_or_kill, wait_or_kill
 from .network import check_port, connect_to, portIsClosed, portIsOpen, write_to
 from .streams import ZlibCompressedStream, JSONStream
 
+logger = logging.getLogger(__name__)
 
-class Categories:
-    START = "Start"
-    END = "End"
-
-    MEMORY = "Memory"
-    SHMEM = "SharedMemory"
-    FILE = "File"
-    NGAS = "NGAS"
-    NULL = "null"
-    JSON = "json"
-    S3 = "S3"
-    PLASMA = "Plasma"
-    PLASMAFLIGHT = "PlasmaFlight"
-    PARSET = "ParameterSet"
-    ENVIRONMENTVARS = "EnvironmentVariables"
-
-    MKN = "MKN"
-    SCATTER = "Scatter"
-    GATHER = "Gather"
-    GROUP_BY = "GroupBy"
-    LOOP = "Loop"
-    VARIABLES = "Variables"
-
-    BRANCH = "Branch"
-    DATA = "Data"
-    COMPONENT = "Component"
-    PYTHON_APP = "PythonApp"
-    BASH_SHELL_APP = "BashShellApp"
-    MPI = "Mpi"
-    DYNLIB_APP = "DynlibApp"
-    DOCKER = "Docker"
-    DYNLIB_PROC_APP = "DynlibProcApp"
-    SERVICE = "Service"
-
-    COMMENT = "Comment"
-    DESCRIPTION = "Description"
-
-
-STORAGE_TYPES = {
-    Categories.MEMORY,
-    Categories.SHMEM,
-    Categories.FILE,
-    Categories.NGAS,
-    Categories.NULL,
-    Categories.END,
-    Categories.JSON,
-    Categories.PLASMA,
-    Categories.PLASMAFLIGHT,
-    Categories.PARSET,
-    Categories.ENVIRONMENTVARS,
-    Categories.S3,
-}
-APP_DROP_TYPES = [
-    Categories.COMPONENT,
-    Categories.PYTHON_APP,
-    Categories.BRANCH,
-    Categories.BASH_SHELL_APP,
-    Categories.MPI,
-    Categories.DYNLIB_APP,
-    Categories.DOCKER,
-    Categories.DYNLIB_PROC_APP,
-    Categories.SERVICE,
-]
-
-
-class DropType:
-    # this gives the mapping to fields containing class paths
-    DATA = "data" # TODO: need to drop this one
-    DATACLASS = "dataclass"
-    APPCLASS = "appclass"
-    SOCKET = "socket"
-    APP = "app"  # TODO: need to drop this one
-    SERVICE_APP = "serviceapp"  # App drop that runs continously
-    CONTAINER = "container"  # Drop that contains other drops
 
-class CategoryType:
+class CategoryType(str, Enum):
     DATA = "Data"
     APPLICATION = "Application"
+    CONSTRUCT = "Construct"
     GROUP = "Group"
     UNKNOWN = "Unknown"
     SERVICE = "Service"
     CONTAINER = "Container"
     SOCKET = "Socket"
     CONTROL = "Control"
     OTHER = "Other"
 
+
 def b2s(b, enc="utf8"):
     "Converts bytes into a string"
     return b.decode(enc)
 
 
 class dropdict(dict):
     """
@@ -135,38 +68,55 @@
 
     Users of this class are, for example, the graph_loader module which deals
     with JSON -> DROP representation transformations, and the different
     repositories where graph templates are expected to be found by the
     DROPManager.
     """
 
-    def _addSomething(self, other, key, IdText=None):
+    def __init__(self, init_dict=None):
+        if init_dict is None:
+            init_dict = {
+                "oid": None,
+                "categoryType": "Unknown",
+            }
+
+        self.update(init_dict)
+        if "oid" not in self:
+            self.update({"oid": None})
+        return super().__init_subclass__()
+
+    def _addSomething(self, other, key, name=None):
         if key not in self:
             self[key] = []
         if other["oid"] not in self[key]:
-            append = {other["oid"]: IdText} if IdText else other["oid"]
+            # TODO: Returning just the other drop OID instead of the named
+            #       port list is not a good solution. Required for the dask
+            #       tests.
+            append = {other["oid"]: name} if name else other["oid"]
+            # if name is None:
+            # raise ValueError
             self[key].append(append)
 
-    def addConsumer(self, other, IdText=None):
-        self._addSomething(other, "consumers", IdText=IdText)
+    def addConsumer(self, other, name=None):
+        self._addSomething(other, "consumers", name=name)
 
-    def addStreamingConsumer(self, other, IdText=None):
-        self._addSomething(other, "streamingConsumers", IdText=IdText)
+    def addStreamingConsumer(self, other, name=None):
+        self._addSomething(other, "streamingConsumers", name=name)
 
-    def addInput(self, other, IdText=None):
-        self._addSomething(other, "inputs", IdText=IdText)
+    def addInput(self, other, name=None):
+        self._addSomething(other, "inputs", name=name)
 
-    def addStreamingInput(self, other, IdText=None):
-        self._addSomething(other, "streamingInputs", IdText=IdText)
+    def addStreamingInput(self, other, name=None):
+        self._addSomething(other, "streamingInputs", name=name)
 
-    def addOutput(self, other, IdText=None):
-        self._addSomething(other, "outputs", IdText=IdText)
+    def addOutput(self, other, name=None):
+        self._addSomething(other, "outputs", name=name)
 
-    def addProducer(self, other, IdText=None):
-        self._addSomething(other, "producers", IdText=IdText)
+    def addProducer(self, other, name=None):
+        self._addSomething(other, "producers", name=name)
 
 
 def _sanitize_links(links):
     """
     Links can now be dictionaries, but we only need
     the key.
     """
@@ -189,36 +139,45 @@
     """
 
     # We find all the nonroots first, which are easy to spot.
     # The rest are the roots
     all_oids = set()
     nonroots = set()
     for dropspec in pg_spec:
-
         # Assumed to be reprodata / other non-drop elements
         #
         # TODO (rtobar): Note that this should be a temporary measure.
         # In principle the pg_spec given here should be a graph, which (until
         # recently) consisted on drop specifications only. The fact that repro
         # data is now appended at the end of some graphs highlights the need for
         # a more formal specification of graphs and other pieces of data that we
         # move through the system.
         if "oid" not in dropspec:
             continue
 
         oid = dropspec["oid"]
         all_oids.add(oid)
-
-        if dropspec["type"] in (DropType.APP, DropType.SOCKET):
-            if dropspec.get("inputs", None) or dropspec.get("streamingInputs", None):
+        ctype = (
+            dropspec["categoryType"]
+            if "categoryType" in dropspec
+            else dropspec["type"]
+        )
+        if ctype in (
+            CategoryType.APPLICATION,
+            CategoryType.SOCKET,
+            "app",
+        ):
+            if dropspec.get("inputs", None) or dropspec.get(
+                "streamingInputs", None
+            ):
                 nonroots.add(oid)
             if dropspec.get("outputs", None):
                 do = _sanitize_links(dropspec["outputs"])
                 nonroots |= set(do)
-        elif dropspec["type"] == DropType.DATA:
+        elif ctype == CategoryType.DATA:
             if dropspec.get("producers", None):
                 nonroots.add(oid)
             if dropspec.get("consumers", None):
                 dc = _sanitize_links(dropspec["consumers"])
                 nonroots |= set(dc)
             if dropspec.get("streamingConsumers", None):
                 dsc = _sanitize_links(dropspec["streamingConsumers"])
@@ -234,36 +193,40 @@
     """
 
     # We find all the nonleaves first, which are easy to spot.
     # The rest are the leaves
     all_oids = set()
     nonleaves = set()
     for dropspec in pg_spec:
-
         oid = dropspec["oid"]
         all_oids.add(oid)
+        ctype = (
+            dropspec["categoryType"]
+            if "categoryType" in dropspec
+            else dropspec["type"]
+        )
 
-        if dropspec["type"] == DropType.APP:
+        if ctype in [CategoryType.APPLICATION, "app"]:
             if dropspec.get("outputs", None):
                 nonleaves.add(oid)
             if dropspec.get("streamingInputs", None):
                 dsi = _sanitize_links(dropspec["streamingInputs"])
                 nonleaves |= set(dsi)
             if dropspec.get("inputs", None):
                 di = _sanitize_links(dropspec["inputs"])
                 nonleaves |= set(di)
-        if dropspec["type"] == DropType.SERVICE_APP:
+        if ctype in [CategoryType.SERVICE, "socket"]:
             nonleaves.add(oid)  # services are never leaves
             if dropspec.get("streamingInputs", None):
                 dsi = _sanitize_links(dropspec["streamingInputs"])
                 nonleaves |= set(dsi)
             if dropspec.get("inputs", None):
                 di = _sanitize_links(dropspec["inputs"])
                 nonleaves |= set(di)
-        elif dropspec["type"] == DropType.DATA:
+        elif ctype in [CategoryType.DATA, "data"]:
             if dropspec.get("producers", None):
                 dp = _sanitize_links(dropspec["producers"])
                 nonleaves |= set(dp)
             if dropspec.get("consumers", None) or dropspec.get(
                 "streamingConsumers", None
             ):
                 nonleaves.add(oid)
```

### Comparing `daliuge-common-2.4.0/dlg/common/deployment_methods.py` & `daliuge-common-3.0.0/dlg/common/deployment_methods.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-2.4.0/dlg/common/k8s_utils.py` & `daliuge-common-3.0.0/dlg/common/k8s_utils.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-2.4.0/dlg/common/network.py` & `daliuge-common-3.0.0/dlg/common/network.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-2.4.0/dlg/common/osutils.py` & `daliuge-common-3.0.0/dlg/common/osutils.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-2.4.0/dlg/common/reproducibility/constants.py` & `daliuge-common-3.0.0/dlg/common/reproducibility/constants.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-2.4.0/dlg/common/reproducibility/reprodata_compare.py` & `daliuge-common-3.0.0/dlg/common/reproducibility/reprodata_compare.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-2.4.0/dlg/common/reproducibility/reproducibility.py` & `daliuge-common-3.0.0/dlg/common/reproducibility/reproducibility.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 arranged top-to-bottom as logical to physical to runtime.
 """
 import collections
 import logging
 
 from merklelib import MerkleTree
 
-from dlg.common import STORAGE_TYPES
 from dlg.common.reproducibility.constants import (
     ReproducibilityFlags,
     REPRO_DEFAULT,
     PROTOCOL_VERSION,
     HashingAlg,
     rmode_supported,
     rflag_caster,
@@ -90,46 +89,59 @@
     :return: A dictionary containing accumulated reproducibility data for a given drop.
     """
     if not rmode_supported(level):
         raise NotImplementedError(
             f"Reproducibility level {level.name} not yet supported"
         )
     category = drop.get("category", "")
+    # category = drop.get("categoryType", "")
 
     # Cheeky way to get field list into dicts. map(dict, drop...) makes a copy
-    fields = {e.pop("name"): e["value"] for e in map(dict, drop.get("fields", {}))}
-    app_fields = {e.pop("name"): e["value"] for e in map(dict, drop.get("applicationArgs", {}))}
+    fields = {
+        e.pop("name"): e["value"] for e in map(dict, drop.get("fields", {}))
+    }
+    app_fields = {
+        e.pop("name"): e["value"]
+        for e in map(dict, drop.get("applicationArgs", {}))
+    }
     fields.update(app_fields)
     lg_fields = lg_block_fields(category, level, app_fields.keys())
     data = extract_fields(fields, lg_fields)
     return data
 
 
 def accumulate_pgt_unroll_drop_data(drop: dict):
     """
     Accumulates relevant reproducibility fields for a single drop at the physical template level.
     :param drop:
     :return: A dictionary containing accumulated reproducibility data for a given drop.
     """
     if drop.get("reprodata") is None:
-        drop["reprodata"] = {"rmode": str(REPRO_DEFAULT.value), "lg_blockhash": None}
+        drop["reprodata"] = {
+            "rmode": str(REPRO_DEFAULT.value),
+            REPRO_DEFAULT.name: {
+                "rmode": str(REPRO_DEFAULT.value),
+                "lg_blockhash": None,
+            },
+        }
     if drop["reprodata"].get("rmode") is None:
         level = REPRO_DEFAULT
-        drop["reprodata"]["rmode"] = str(level.value)
+        drop["reprodata"]["rmode"] = str(level.level)
+        drop["reprodata"][level.name] = {}
     else:
         level = rflag_caster(drop["reprodata"]["rmode"])
     if not rmode_supported(level):
         logger.warning(
             "Requested reproducibility mode %s not yet implemented", str(level)
         )
         level = REPRO_DEFAULT
         drop["reprodata"]["rmode"] = str(level.value)
-    if drop.get("type") is None:
-        return {}
-    drop_type = drop["type"]
+    # if drop.get("categoryType") is None:
+    #     return {}
+    drop_type = drop["categoryType"]
     candidate_rmodes = []
     if level == ReproducibilityFlags.ALL:
         candidate_rmodes.extend(ALL_RMODES)
     else:
         candidate_rmodes.append(level)
     data = {}
     for rmode in candidate_rmodes:
@@ -141,15 +153,18 @@
 def accumulate_pgt_partition_drop_data(drop: dict):
     """
     Is as combination of unroll drop data
     :param drop:
     :return:
     """
     if drop.get("reprodata") is None:
-        drop["reprodata"] = {"rmode": str(REPRO_DEFAULT.value), "lg_blockhash": None}
+        drop["reprodata"] = {
+            "rmode": str(REPRO_DEFAULT.value),
+            "lg_blockhash": None,
+        }
     if drop["reprodata"].get("rmode") is None:
         level = REPRO_DEFAULT
         drop["reprodata"]["rmode"] = str(level.value)
     else:
         level = rflag_caster(drop["reprodata"]["rmode"])
     if not rmode_supported(level):
         logger.warning(
@@ -340,30 +355,33 @@
 #  ------ Graph-Wide Functionality ------
 
 
 def accumulate_meta_data():
     """
     WARNING: Relies on naming convention in hashlib.
     """
-    data = {"repro_protocol": PROTOCOL_VERSION, "HashingAlg": str(HashingAlg)}
+    data = {
+        "repro_protocol": PROTOCOL_VERSION,
+        "HashingAlg": HashingAlg.__name__,
+    }
     return data
 
 
 def build_lg_block_data(drop: dict, rmode):
     """
     Builds the logical graph reprodata entry for a processed drop description
     :param drop: The drop description
     :return:
     """
     block_data = [drop["reprodata"][rmode.name]["lgt_data"]["merkleroot"]]
     if "merkleroot" in drop["reprodata"][rmode.name]["lg_data"]:
         lg_hash = drop["reprodata"][rmode.name]["lg_data"]["merkleroot"]
         block_data.append(lg_hash)
     for parenthash in sorted(
-            drop["reprodata"][rmode.name]["lg_parenthashes"].values()
+        drop["reprodata"][rmode.name]["lg_parenthashes"].values()
     ):
         block_data.append(parenthash)
     mtree = MerkleTree(block_data, common_hash)
     drop["reprodata"][rmode.name]["lg_blockhash"] = mtree.merkle_root
 
 
 def build_pgt_block_data(drop: dict, rmode):
@@ -377,15 +395,15 @@
         if "merkleroot" in drop["reprodata"][rmode.name]["pgt_data"]:
             block_data.append(
                 drop["reprodata"][rmode.name]["pgt_data"]["merkleroot"]
             )
     if "lg_blockhash" in drop["reprodata"][rmode.name]:
         block_data.append(drop["reprodata"][rmode.name]["lg_blockhash"])
     for parenthash in sorted(
-            drop["reprodata"][rmode.name]["pgt_parenthashes"].values()
+        drop["reprodata"][rmode.name]["pgt_parenthashes"].values()
     ):
         block_data.append(parenthash)
     mtree = MerkleTree(block_data, common_hash)
     drop["reprodata"][rmode.name]["pgt_blockhash"] = mtree.merkle_root
 
 
 def build_pg_block_data(drop: dict, rmode):
@@ -396,15 +414,15 @@
     """
     block_data = [
         drop["reprodata"][rmode.name]["pg_data"]["merkleroot"],
         drop["reprodata"][rmode.name]["pgt_blockhash"],
         drop["reprodata"][rmode.name]["lg_blockhash"],
     ]
     for parenthash in sorted(
-            drop["reprodata"][rmode.name]["pg_parenthashes"].values()
+        drop["reprodata"][rmode.name]["pg_parenthashes"].values()
     ):
         block_data.append(parenthash)
     mtree = MerkleTree(block_data, common_hash)
     drop["reprodata"][rmode.name]["pg_blockhash"] = mtree.merkle_root
 
 
 def build_rg_block_data(drop: dict, rmode):
@@ -418,15 +436,15 @@
             "merkleroot"
         ],
         drop["reprodata"][rmode.name]["pg_blockhash"],
         drop["reprodata"][rmode.name]["pgt_blockhash"],
         drop["reprodata"][rmode.name]["lg_blockhash"],
     ]
     for parenthash in sorted(
-            drop["reprodata"][rmode.name]["rg_parenthashes"].values()
+        drop["reprodata"][rmode.name]["rg_parenthashes"].values()
     ):
         block_data.append(parenthash)
     mtree = MerkleTree(block_data, common_hash)
     drop["reprodata"][rmode.name]["rg_blockhash"] = mtree.merkle_root
 
 
 def lg_build_blockdag(logical_graph: dict, level):
@@ -476,18 +494,22 @@
         if rmode == ReproducibilityFlags.ALL:
             rmode = level  # Only building one layer at a time.
         for neighbour in neighbourset[did]:
             dropset[neighbour][1] -= 1
             parenthash = {}
             if rmode != ReproducibilityFlags.NOTHING:
                 if rmode == ReproducibilityFlags.REPRODUCE:
+                    if "categoryType" in dropset[did][0]:
+                        dtype = dropset[did][0]["categoryType"].lower()
+                    elif "categoryType" in dropset[did][0]:
+                        dtype = dropset[did][0]["categoryType"].lower()
                     if (
-                            dropset[did][0]["category"] in STORAGE_TYPES
-                            and (dropset[did][1] == 0 or dropset[did][2] == 0)
-                            and (did in roots or did in leaves)
+                        dtype == "data"
+                        and (dropset[did][1] == 0 or dropset[did][2] == 0)
+                        and (did in roots or did in leaves)
                     ):
                         # Add my new hash to the parent-hash list
                         if did not in parenthash:
                             parenthash[did] = dropset[did][0]["reprodata"][
                                 level.name
                             ]["lg_blockhash"]
                         # parenthash.append(dropset[did][0]['reprodata']['lg_blockhash'])
@@ -495,15 +517,17 @@
                         # Add my parenthashes to the parent-hash list
                         parenthash.update(
                             dropset[did][0]["reprodata"][level.name][
                                 "lg_parenthashes"
                             ]
                         )
                         # parenthash.extend(dropset[did][0]['reprodata']['lg_parenthashes'])
-                if rmode != ReproducibilityFlags.REPRODUCE:  # Non-compressing behaviour
+                if (
+                    rmode != ReproducibilityFlags.REPRODUCE
+                ):  # Non-compressing behaviour
                     parenthash[did] = dropset[did][0]["reprodata"][level.name][
                         "lg_blockhash"
                     ]
                     # parenthash.append(dropset[did][0]['reprodata']['lg_blockhash'])
                 #  Add our new hash to the parent-hash list
                 # We deal with duplicates later
                 dropset[neighbour][0]["reprodata"][level.name][
@@ -565,15 +589,15 @@
             for dest in drop["outputs"]:
                 if isinstance(dest, dict):
                     dest = next(iter(dest))
                 dropset[dest][1] += 1
                 dropset[did][2] += 1
                 neighbourset[did].append(dest)
         if (
-                "consumers" in drop
+            "consumers" in drop
         ):  # There may be some bizarre scenario when a drop has both
             for dest in drop["consumers"]:
                 if isinstance(dest, dict):
                     dest = next(iter(dest))
                 dropset[dest][1] += 1
                 dropset[did][2] += 1
                 neighbourset[did].append(
@@ -594,21 +618,30 @@
             rmode = level
         for neighbour in neighbourset[did]:
             dropset[neighbour][1] -= 1
             parenthash = {}
             if rmode != ReproducibilityFlags.NOTHING:
                 if rmode == ReproducibilityFlags.REPRODUCE:
                     # WARNING: Hack! may break later, proceed with caution
-                    category = dropset[did][0]["reprodata"][rmode.name]["lgt_data"][
-                        "category"
-                    ]
                     if (
-                            category in STORAGE_TYPES
-                            and (dropset[did][1] == 0 or dropset[did][2] == 0)
-                            and (did in roots or did in leaves)
+                        "categoryType"
+                        in dropset[did][0]["reprodata"][rmode.name]["pgt_data"]
+                    ):
+                        ctype = dropset[did][0]["reprodata"][rmode.name][
+                            "pgt_data"
+                        ]["categoryType"]
+                    else:
+                        ctype = dropset[did][0]["reprodata"][rmode.name][
+                            "lgt_data"
+                        ]["categoryType"]
+
+                    if (
+                        ctype.lower() == "data"
+                        and (dropset[did][1] == 0 or dropset[did][2] == 0)
+                        and (did in roots or did in leaves)
                     ):
                         # Add my new hash to the parent-hash list
                         if did not in parenthash:
                             parenthash[did] = dropset[did][0]["reprodata"][
                                 level.name
                             ][blockstr + "_blockhash"]
                         # parenthash.append(dropset[did][0]['reprodata'] \
@@ -617,20 +650,20 @@
                         # Add my parenthashes to the parent-hash list
                         parenthash.update(
                             dropset[did][0]["reprodata"][level.name][parentstr]
                         )
                 if rmode != ReproducibilityFlags.REPRODUCE:
                     parenthash[did] = dropset[did][0]["reprodata"][level.name][
                         blockstr + "_blockhash"
-                        ]
+                    ]
                 # Add our new hash to the parent-hash list if on the critical path
                 if rmode == ReproducibilityFlags.RERUN:
                     if "iid" in dropset[did][0].keys():
                         if (
-                                dropset[did][0]["iid"] == "0/0"
+                            dropset[did][0]["iid"] == "0/0"
                         ):  # TODO: This is probably wrong
                             dropset[neighbour][0]["reprodata"][level.name][
                                 parentstr
                             ].update(parenthash)
                     else:
                         dropset[neighbour][0]["reprodata"][level.name][
                             parentstr
@@ -644,15 +677,15 @@
 
     if len(visited) != len(dropset):
         logger.warning("Not a DAG")
 
     for i, leaf in enumerate(leaves):
         leaves[i] = dropset[leaf][0]["reprodata"][level.name][
             blockstr + "_blockhash"
-            ]
+        ]
     return leaves, visited
 
     # logger.info("BlockDAG Generated at" + abstraction + " level")
 
 
 def agglomerate_leaves(leaves: list):
     """
@@ -674,15 +707,18 @@
     """
     rmode = rflag_caster(rmode)
     if not rmode_supported(rmode):
         logger.warning(
             "Requested reproducibility mode %s not yet implemented", str(rmode)
         )
         rmode = REPRO_DEFAULT
-    reprodata = {"rmode": str(rmode.value), "meta_data": accumulate_meta_data()}
+    reprodata = {
+        "rmode": str(rmode.value),
+        "meta_data": accumulate_meta_data(),
+    }
     meta_tree = MerkleTree(reprodata.items(), common_hash)
     reprodata["merkleroot"] = meta_tree.merkle_root
     for drop in logical_graph_template.get("nodeDataArray", []):
         init_lgt_repro_drop_data(drop, rmode)
     logical_graph_template["reprodata"] = reprodata
     logger.info("Reproducibility data finished at LGT level")
     return logical_graph_template
@@ -710,17 +746,17 @@
         candidate_rmodes.extend(ALL_RMODES)
     else:
         candidate_rmodes.append(level)
     for rmode in candidate_rmodes:
         if rmode.name not in logical_graph["reprodata"]:
             logical_graph["reprodata"][rmode.name] = {}
         leaves, _ = lg_build_blockdag(logical_graph, rmode)
-        logical_graph["reprodata"][rmode.name]["signature"] = agglomerate_leaves(
-            leaves
-        )
+        logical_graph["reprodata"][rmode.name][
+            "signature"
+        ] = agglomerate_leaves(leaves)
     logger.info("Reproducibility data finished at LG level")
     return logical_graph
 
 
 def init_pgt_unroll_repro_data(physical_graph_template: list):
     """
     Handles adding reproducibility data at the physical graph template level.
```

### Comparing `daliuge-common-2.4.0/dlg/common/reproducibility/reproducibility_fields.py` & `daliuge-common-3.0.0/dlg/common/reproducibility/reproducibility_fields.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,26 +23,29 @@
 This module defines the fields each drop takes for each reproducibility standard defined.
 Consider this module partially documentation, partially code.
 Data generated by instanced drops at runtime are defined with that drop's implementation.
 """
 
 from enum import Enum
 
-from dlg.common import Categories
 from dlg.common.reproducibility.constants import ReproducibilityFlags
+import logging
+
+logger = logging.getLogger("__name__")
 
 
 class FieldOps(Enum):
     """
     Defines the operations possible on drop data for provenance collection.
     """
 
     STORE = 0
     COUNT = 1
     REMOVE_FIRST = 2  # Removes the first char of an assumed string
+    DO_NOT_STORE = None
 
 
 def extract_fields(drop: dict, fields: dict):
     """
     Attempts to extract fields with the names in fields from the drop description.
     If not found, the key will not be present in the returned dictionary.
     """
@@ -79,116 +82,121 @@
         del data["inputPorts"]
         del data["outputPorts"]
         del data["inputLocalPorts"]
         del data["outputLocalPorts"]
     return data
 
 
-def lg_block_fields(category_type: str, rmode: ReproducibilityFlags, custom_fields=None):
+def lg_block_fields(
+    category_type: str, rmode: ReproducibilityFlags, custom_fields=None
+):
     """
     Collects dict of fields and operations for all drop types at the lg layer for
     the supplied reproducibility standard.
     :param category: The broad type of drop
     :param rmode: The reproducibility level in question
     :param custom_fields: Additional application args (used in custom components)
     :return: Dictionary of <str, FieldOp> pairs
     """
     data = {}
     if rmode in (
-            ReproducibilityFlags.NOTHING,
-            ReproducibilityFlags.RERUN,
-            ReproducibilityFlags.REPRODUCE,
-            ReproducibilityFlags.REPLICATE_SCI,
+        ReproducibilityFlags.NOTHING,
+        ReproducibilityFlags.RERUN,
+        ReproducibilityFlags.REPRODUCE,
+        ReproducibilityFlags.REPLICATE_SCI,
     ):
         return data
     # Drop category considerations - Just try to get everything we can, will be filtered later
     data["execution_time"] = FieldOps.STORE
     data["num_cpus"] = FieldOps.STORE
     data["inputApplicationName"] = FieldOps.STORE
     data["inputApplicationType"] = FieldOps.STORE
     data["data_volume"] = FieldOps.STORE
 
     # Drop type considerations
-    if category_type == Categories.START:
+    if category_type == "Start":
         pass
-    elif category_type == Categories.END:
+    elif category_type == "End":
         pass
-    elif category_type == Categories.MEMORY:
+    elif category_type == "Memory":
         pass
-    elif category_type == Categories.SHMEM:
+    elif category_type == "ShMem":
         pass
-    elif category_type == Categories.FILE:
+    elif category_type == "File":
         data["check_filepath_exists"] = FieldOps.STORE
         if rmode in (
-                ReproducibilityFlags.RECOMPUTE,
-                ReproducibilityFlags.REPLICATE_COMP,
+            ReproducibilityFlags.RECOMPUTE,
+            ReproducibilityFlags.REPLICATE_COMP,
         ):
             data["filepath"] = FieldOps.STORE
             data["dirname"] = FieldOps.STORE
-    elif category_type == Categories.NULL:
+    elif category_type == "null":
         pass
-    elif category_type == Categories.JSON:
+    elif category_type == "json":
         pass
-    elif category_type == Categories.NGAS:
+    elif category_type == "NGAS":
         pass
-    elif category_type == Categories.S3:
+    elif category_type == "S3":
         pass
-    elif category_type == Categories.PLASMA:
+    elif category_type == "Plasma":
         data["plasma_path"] = FieldOps.STORE
         data["object_id"] = FieldOps.STORE
-    elif category_type == Categories.PLASMAFLIGHT:
+    elif category_type == "PlasmaFlight":
         data["plasma_path"] = FieldOps.STORE
         data["object_id"] = FieldOps.STORE
         data["flight_path"] = FieldOps.STORE
-    elif category_type == Categories.PARSET:
+    elif category_type == "ParameterSet":
         pass
-    elif category_type == Categories.ENVIRONMENTVARS:
+    elif category_type == "EnvironmentVariables":
         pass
-    elif category_type == Categories.MKN:
+    elif category_type == "MKN":
         data["m"] = FieldOps.STORE
         data["k"] = FieldOps.STORE
         data["n"] = FieldOps.STORE
-    elif category_type == Categories.SCATTER:
+    elif category_type == "Scatter":
         data["num_of_copies"] = FieldOps.STORE
         data["scatter_axis"] = FieldOps.STORE
-    elif category_type == Categories.GATHER:
+    elif category_type == "Gather":
         data["num_of_inputs"] = FieldOps.STORE
         data["gather_axis"] = FieldOps.STORE
-    elif category_type == Categories.LOOP:
+    elif category_type == "Loop":
         data["num_of_iter"] = FieldOps.STORE
-    elif category_type == Categories.GROUP_BY:
+    elif category_type == "GroupBy":
         data["group_key"] = FieldOps.STORE
         data["group_axis"] = FieldOps.STORE
-    elif category_type == Categories.VARIABLES:
+    elif category_type == "Variables":
         pass
-    elif category_type == Categories.BRANCH:
-        data["appclass"] = FieldOps.STORE
-    elif category_type == Categories.PYTHON_APP:
-        data["appclass"] = FieldOps.STORE
-    elif category_type == Categories.COMPONENT:
-        data["appclass"] = FieldOps.STORE
-    elif category_type == Categories.BASH_SHELL_APP:
+    elif category_type == "Branch":
+        data["dropclass"] = FieldOps.STORE
+    elif category_type == "PythonApp":
+        data["dropclass"] = FieldOps.STORE
+    elif category_type == "Component":
+        data["dropclass"] = FieldOps.STORE
+    elif category_type == "BashShellApp":
         data["Arg01"] = FieldOps.STORE
-    elif category_type == Categories.MPI:
+    elif category_type == "Mpi":
         data["num_of_procs"] = FieldOps.STORE
-    elif category_type == Categories.DOCKER:
+    elif category_type == "Docker":
         data["image"] = FieldOps.STORE
         data["command"] = FieldOps.STORE
         data["user"] = FieldOps.STORE
         data["ensureUserAndSwitch"] = FieldOps.STORE
         data["removeContainer"] = FieldOps.STORE
         data["additionalBindings"] = FieldOps.STORE
-    elif category_type == Categories.DYNLIB_APP:
+    elif category_type == "DynlibApp":
         data["libpath"] = FieldOps.STORE
-    elif category_type == Categories.DYNLIB_PROC_APP:
+    elif category_type == "DynlibProcApp":
         data["libpath"] = FieldOps.STORE
     if custom_fields is not None and rmode in (
-            ReproducibilityFlags.RECOMPUTE, ReproducibilityFlags.REPLICATE_COMP):
+        ReproducibilityFlags.RECOMPUTE,
+        ReproducibilityFlags.REPLICATE_COMP,
+    ):
         for name in custom_fields:
             data[name] = FieldOps.STORE
+
     return data
 
 
 def pgt_unroll_block_fields(category_type, rmode: ReproducibilityFlags):
     """
     Collects dict of fields and operations for all drop types at the pgt unroll layer for
     the supplied reproducibility standard.
@@ -196,46 +204,55 @@
     :param rmode: The reproducibility level in question
     :return: Dictionary of <str, FieldOp> pairs
     """
     data = {}
     if rmode == ReproducibilityFlags.NOTHING:
         return data
     if rmode != ReproducibilityFlags.NOTHING:
-        data["type"] = FieldOps.STORE
+        data["categoryType"] = FieldOps.STORE
     if rmode != ReproducibilityFlags.REPRODUCE:
-        if category_type != "data":
+        if category_type.lower() != "data":
             data["dt"] = FieldOps.STORE
-    if category_type == "data":
+    if category_type.lower() == "data":
         data["storage"] = FieldOps.STORE
-    if rmode in (ReproducibilityFlags.RECOMPUTE, ReproducibilityFlags.REPLICATE_COMP):
+    if rmode in (
+        ReproducibilityFlags.RECOMPUTE,
+        ReproducibilityFlags.REPLICATE_COMP,
+    ):
         data["rank"] = FieldOps.STORE
 
     return data
 
 
 def pgt_partition_block_fields(rmode: ReproducibilityFlags):
     """
     Collects dict of fields and operations for all drop types at the pgt partition layer for
     the supplied reproducibility standard.
     :param rmode: The reproducibility level in question
     :return: Dictionary of <str, FieldOp> pairs
     """
     data = {}
-    if rmode in (ReproducibilityFlags.RECOMPUTE, ReproducibilityFlags.REPLICATE_COMP):
+    if rmode in (
+        ReproducibilityFlags.RECOMPUTE,
+        ReproducibilityFlags.REPLICATE_COMP,
+    ):
         data["node"] = FieldOps.REMOVE_FIRST
         data["island"] = FieldOps.REMOVE_FIRST
     return data
 
 
 def pg_block_fields(rmode: ReproducibilityFlags):
     """
     Collects dict of fields and operations for all drop types at the pg layer for
     the supplied reproducibility standard.
     :param rmode: The reproducibility level in question
     :return: Dictionary of <str, FieldOp> pairs
     """
     # These two happen to have the same data.
     data = {}
-    if rmode in (ReproducibilityFlags.RECOMPUTE, ReproducibilityFlags.REPLICATE_COMP):
+    if rmode in (
+        ReproducibilityFlags.RECOMPUTE,
+        ReproducibilityFlags.REPLICATE_COMP,
+    ):
         data["node"] = FieldOps.STORE
         data["island"] = FieldOps.STORE
     return data
```

### Comparing `daliuge-common-2.4.0/dlg/common/streams.py` & `daliuge-common-3.0.0/dlg/common/streams.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-2.4.0/dlg/common/tool.py` & `daliuge-common-3.0.0/dlg/common/tool.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-2.4.0/dlg/constants.py` & `daliuge-common-3.0.0/dlg/constants.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-2.4.0/dlg/exceptions.py` & `daliuge-common-3.0.0/dlg/exceptions.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-2.4.0/dlg/restutils.py` & `daliuge-common-3.0.0/dlg/restutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,16 @@
 ):
     daemon_threads = True
     allow_reuse_address = True
 
 
 class LoggingWSGIRequestHandler(wsgiref.simple_server.WSGIRequestHandler):
     def log_message(self, fmt, *args):
-        logger.debug(fmt, *args)
+        pass
+        # logger.debug(fmt, *args)
 
 
 class RestServerWSGIServer:
     def __init__(self, wsgi_app, listen="localhost", port=8080):
         self.wsgi_app = wsgi_app
         self.listen = listen
         self.port = port
@@ -139,15 +140,17 @@
     def _get_json(self, url):
         ret = self._GET(url)
         return json.load(ret) if ret else None
 
     def _post_form(self, url, content=None):
         if content is not None:
             content = urllib.parse.urlencode(content)
-        ret = self._POST(url, content, content_type="application/x-www-form-urlencoded")
+        ret = self._POST(
+            url, content, content_type="application/x-www-form-urlencoded"
+        )
         return json.load(ret) if ret else None
 
     def _post_json(self, url, content, compress=False):
         if not isinstance(content, (str, bytes)):
             content = common.JSONStream(content)
         ret = self._POST(
             url, content, content_type="application/json", compress=compress
@@ -173,18 +176,19 @@
         return stream
 
     def _DELETE(self, url):
         stream, _ = self._request(url, "DELETE")
         return stream
 
     def _request(self, url, method, content=None, headers={}):
-
         # Do the HTTP stuff...
         url = self.url_prefix + url
-        logger.debug("Sending %s request to %s:%d%s", method, self.host, self.port, url)
+        logger.debug(
+            "Sending %s request to %s:%d%s", method, self.host, self.port, url
+        )
 
         if not common.portIsOpen(self.host, self.port, self.timeout):
             raise RestClientException(
                 "Cannot connect to %s:%d after %.2f [s]"
                 % (self.host, self.port, self.timeout)
             )
 
@@ -194,15 +198,14 @@
 
         self._conn = http.client.HTTPConnection(self.host, self.port)
         self._conn.request(method, url, content, headers)
         self._resp = self._conn.getresponse()
 
         # Server errors are encoded in the body as json content
         if self._resp.status != http.HTTPStatus.OK:
-
             msg = "Error on remote %s@%s:%s%s (status %d): " % (
                 method,
                 self.host,
                 self.port,
                 url,
                 self._resp.status,
             )
```

### Comparing `daliuge-common-2.4.0/dlg/version_helper.py` & `daliuge-common-3.0.0/dlg/version_helper.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-2.4.0/setup.py` & `daliuge-common-3.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 # Version information
 # We do like numpy: we have a major/minor/patch hand-written version written
 # here. If we find the git commit (either via "git" command execution or in a
 # dlg/version.py file) we append it to the VERSION later.
 # The RELEASE flag allows us to create development versions properly supported
 # by setuptools/pkg_resources or "final" versions.
-MAJOR = 2
-MINOR = 4
+MAJOR = 3
+MINOR = 0
 PATCH = 0
 VERSION = (MAJOR, MINOR, PATCH)
 VERSION_FILE = "dlg/common/version.py"
 RELEASE = True
 
 
 def do_versioning():
```

