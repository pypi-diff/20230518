# Comparing `tmp/eons-2.5.7.tar.gz` & `tmp/eons-2.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.5.7.tar", last modified: Mon Apr 24 07:47:50 2023, max compression
+gzip compressed data, was "eons-2.5.8.tar", last modified: Thu May 18 21:54:04 2023, max compression
```

## Comparing `eons-2.5.7.tar` & `eons-2.5.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:47:50.671429 eons-2.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-24 07:47:50.671429 eons-2.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19582 2023-04-24 07:47:31.000000 eons-2.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:47:50.663429 eons-2.5.7/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:47:50.667429 eons-2.5.7/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 07:47:40.000000 eons-2.5.7/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    84500 2023-04-24 07:47:40.000000 eons-2.5.7/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:47:50.667429 eons-2.5.7/pkg/eons/method/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-24 07:47:19.000000 eons-2.5.7/pkg/eons/method/External.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 07:47:40.000000 eons-2.5.7/pkg/eons/method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:47:50.671429 eons-2.5.7/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 07:47:40.000000 eons-2.5.7/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-24 07:47:19.000000 eons-2.5.7/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-24 07:47:19.000000 eons-2.5.7/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 07:47:19.000000 eons-2.5.7/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-24 07:47:19.000000 eons-2.5.7/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-24 07:47:19.000000 eons-2.5.7/pkg/eons/resolve/resolve_install_with_pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:47:50.667429 eons-2.5.7/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-24 07:47:50.000000 eons-2.5.7/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-24 07:47:50.000000 eons-2.5.7/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 07:47:50.000000 eons-2.5.7/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-24 07:47:50.000000 eons-2.5.7/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 07:47:50.000000 eons-2.5.7/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 07:47:40.000000 eons-2.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-24 07:47:50.671429 eons-2.5.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:54:04.988934 eons-2.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-05-18 21:54:04.988934 eons-2.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19582 2023-05-18 21:53:48.000000 eons-2.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:54:04.984934 eons-2.5.8/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:54:04.984934 eons-2.5.8/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-18 21:53:56.000000 eons-2.5.8/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87237 2023-05-18 21:53:56.000000 eons-2.5.8/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:54:04.984934 eons-2.5.8/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-18 21:53:41.000000 eons-2.5.8/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:53:56.000000 eons-2.5.8/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:54:04.988934 eons-2.5.8/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:53:56.000000 eons-2.5.8/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-18 21:53:41.000000 eons-2.5.8/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-18 21:53:41.000000 eons-2.5.8/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-18 21:53:41.000000 eons-2.5.8/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-18 21:53:41.000000 eons-2.5.8/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-18 21:53:41.000000 eons-2.5.8/pkg/eons/resolve/resolve_install_with_pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:54:04.984934 eons-2.5.8/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-05-18 21:54:04.000000 eons-2.5.8/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-18 21:54:04.000000 eons-2.5.8/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:54:04.000000 eons-2.5.8/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-18 21:54:04.000000 eons-2.5.8/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-18 21:54:04.000000 eons-2.5.8/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 21:53:56.000000 eons-2.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 21:54:04.988934 eons-2.5.8/setup.cfg
```

### Comparing `eons-2.5.7/PKG-INFO` & `eons-2.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.5.7
+Version: 2.5.8
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.5.7/README.md` & `eons-2.5.8/README.md`

 * *Files identical despite different names*

### Comparing `eons-2.5.7/pkg/eons/eons.py` & `eons-2.5.8/pkg/eons/eons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import logging
 import os
-import shutil
-from copy import deepcopy
-import builtins
 import sys
 import pkgutil
 import importlib.machinery
 import importlib.util
 import types
-import traceback
+import builtins
+import argparse
+import requests
 import jsonpickle
+import yaml
 from pathlib import Path
+from tqdm import tqdm
+from zipfile import ZipFile
+from distutils.dir_util import mkpath
+import operator
+import traceback
+from copy import deepcopy
+import shutil
 from subprocess import Popen
 from subprocess import PIPE
 from subprocess import STDOUT
 import inspect
-import ctypes
-import operator
 import re
-import argparse
-import requests
-import yaml
-from tqdm import tqdm
-from zipfile import ZipFile
-from distutils.dir_util import mkpath
 
 ######## START CONTENT ########
 def INVALID_NAME():
 	return "INVALID_NAME"
 
 class ActualType(type):
 	def __repr__(self):
@@ -281,15 +280,15 @@
 			if (styles is None):
 				styles = []
 			#\x1b may also work.
 			compiledCode = f"\033[{cls.saturationCode[saturation]}{cls.foregroundCodes[foreground]}"
 			if (background != 'none'):
 				compiledCode += f";{cls.backgroundCodes[background]}"
 			if (styles):
-				compiledCode += ';' + ';'.join([str(cls.styleCodes[s]) for s in styles])
+				compiledCode += ';' + ';'.join([str(cls.styleCodes[s]) for s in list(styles)])
 			compiledCode += 'm'
 			return compiledCode
 
 		resetStyle = "\033[0m"
 
 
 	# Add a logging level
@@ -319,14 +318,212 @@
 		setattr(logging, levelName, value)
 		setattr(logging.getLogger(), methodName, logForLevel)
 		setattr(logging, methodName, logToRoot)
 
 
 jsonpickle.handlers.registry.register(util.DotDict, util.DotDictPickler)
 
+
+# A DataContainer allows Data to be stored and worked with.
+# This class is intended to be derived from and added to.
+# Each DataContainer is comprised of multiple Data (see Datum.py for more).
+# NOTE: DataContainers are, themselves Data. Thus, you can nest your child classes however you would like.
+class DataContainer(Datum):
+
+	def __init__(this, name=INVALID_NAME()):
+		super().__init__(name)
+
+		# The data *this contains.
+		this.data = []
+
+
+	# RETURNS: an empty, invalid Datum.
+	def InvalidDatum(this):
+		ret = Datum()
+		ret.Invalidate()
+		return ret
+
+
+	# Sort things! Requires by be a valid attribute of all Data.
+	def SortData(this, by):
+		this.data.sort(key=operator.attrgetter(by))
+
+
+	# Adds a Datum to *this
+	def AddDatum(this, datum):
+		this.data.append(datum)
+
+
+	# RETURNS: a Datum with datumAttribute equal to match, an invalid Datum if none found.
+	def GetDatumBy(this, datumAttribute, match):
+		for d in this.data:
+			try: # within for loop 'cause maybe there's an issue with only 1 Datum and the rest are fine.
+				if (str(util.GetAttr(d, datumAttribute)) == str(match)):
+					return d
+			except Exception as e:
+				logging.error(f"{this.name} - {e.message}")
+				continue
+		return this.InvalidDatum()
+
+
+	# RETURNS: a Datum of the given name, an invalid Datum if none found.
+	def GetDatum(this, name):
+		return this.GetDatumBy('name', name)
+
+
+	# Removes all Data in toRem from *this.
+	# RETURNS: the Data removed
+	def RemoveData(this, toRem):
+		# logging.debug(f"Removing {toRem}")
+		this.data = [d for d in this.data if d not in toRem]
+		return toRem
+
+
+	# Removes all Data which match toRem along the given attribute
+	def RemoveDataBy(this, datumAttribute, toRem):
+		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) in list(map(str, toRem))]
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data in *this except toKeep.
+	# RETURNS: the Data removed
+	def KeepOnlyData(this, toKeep):
+		toRem = [d for d in this.data if d not in toKeep]
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data except those that match toKeep along the given attribute
+	# RETURNS: the Data removed
+	def KeepOnlyDataBy(this, datumAttribute, toKeep):
+		# logging.debug(f"Keeping only class with a {datumAttribute} of {toKeep}")
+		# toRem = []
+		# for d in this.class:
+		#	 shouldRem = False
+		#	 for k in toKeep:
+		#		 if (str(util.GetAttr(d, datumAttribute)) == str(k)):
+		#			 logging.debug(f"found {k} in {d.__dict__}")
+		#			 shouldRem = True
+		#			 break
+		#	 if (shouldRem):
+		#		 toRem.append(d)
+		#	 else:
+		#		 logging.debug(f"{k} not found in {d.__dict__}")
+		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) not in list(map(str, toKeep))]
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data with the name "INVALID NAME"
+	# RETURNS: the removed Data
+	def RemoveAllUnlabeledData(this):
+		toRem = []
+		for d in this.data:
+			if (d.name =="INVALID NAME"):
+				toRem.append(d)
+		return this.RemoveData(toRem)
+
+
+	# Removes all invalid Data
+	# RETURNS: the removed Data
+	def RemoveAllInvalidData(this):
+		toRem = []
+		for d in this.data:
+			if (not d.IsValid()):
+				toRem.append(d)
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data that have an attribute value relative to target.
+	# The given relation can be things like operator.le (i.e. <=)
+	#   See https://docs.python.org/3/library/operator.html for more info.
+	# If ignoreNames is specified, any Data of those names will be ignored.
+	# RETURNS: the Data removed
+	def RemoveDataRelativeToTarget(this, datumAttribute, relation, target, ignoreNames = []):
+		try:
+			toRem = []
+			for d in this.data:
+				if (ignoreNames and d.name in ignoreNames):
+					continue
+				if (relation(util.GetAttr(d, datumAttribute), target)):
+					toRem.append(d)
+			return this.RemoveData(toRem)
+		except Exception as e:
+			logging.error(f"{this.name} - {e.message}")
+			return []
+
+
+	# Removes any Data that have the same datumAttribute as a previous Datum, keeping only the first.
+	# RETURNS: The Data removed
+	def RemoveDuplicateDataOf(this, datumAttribute):
+		toRem = [] # list of Data
+		alreadyProcessed = [] # list of strings, not whatever datumAttribute is.
+		for d1 in this.data:
+			skip = False
+			for dp in alreadyProcessed:
+				if (str(util.GetAttr(d1, datumAttribute)) == dp):
+					skip = True
+					break
+			if (skip):
+				continue
+			for d2 in this.data:
+				if (d1 is not d2 and str(util.GetAttr(d1, datumAttribute)) == str(util.GetAttr(d2, datumAttribute))):
+					logging.info(f"Removing duplicate Datum {d2} with unique id {util.GetAttr(d2, datumAttribute)}")
+					toRem.append(d2)
+					alreadyProcessed.append(str(util.GetAttr(d1, datumAttribute)))
+		return this.RemoveData(toRem)
+
+
+	# Adds all Data from otherDataContainer to *this.
+	# If there are duplicate Data identified by the attribute preventDuplicatesOf, they are removed.
+	# RETURNS: the Data removed, if any.
+	def ImportDataFrom(this, otherDataContainer, preventDuplicatesOf=None):
+		this.data.extend(otherDataContainer.data);
+		if (preventDuplicatesOf is not None):
+			return this.RemoveDuplicateDataOf(preventDuplicatesOf)
+		return []
+
+
+
+# FunctorTracker is a global singleton which keeps a record of all functors that are currently in the call stack.
+# Functors should add and remove themselves from this list when they are called.
+class FunctorTracker:
+	def __init__(this):
+		# Singletons man...
+		if "instance" not in FunctorTracker.__dict__:
+			logging.debug(f"Creating new FunctorTracker: {this}")
+			FunctorTracker.instance = this
+		else:
+			return None
+
+		this.functors = [None]
+
+	@staticmethod
+	def Instance():
+		if "instance" not in FunctorTracker.__dict__:
+			FunctorTracker()
+		return FunctorTracker.instance
+
+	@staticmethod
+	def Push(functor):
+		FunctorTracker.Instance().functors.append(functor)
+
+	# Remove the last instance of the functor from the list.
+	@staticmethod
+	def Pop(functor):
+		tracker = FunctorTracker.Instance()
+		tracker.functors.reverse()
+		try:
+			tracker.functors.remove(functor)
+		except:
+			pass
+		tracker.functors.reverse()
+
+	@staticmethod
+	def GetCount():
+		return len(FunctorTracker.Instance().functors)
+
 # Don't import Method or Executor, even though they are required: it will cause a circular dependency.
 # Instead, pretend there's a forward declaration here and don't think too hard about it ;)
 ################################################################################
 
 # Functor is a base class for any function-oriented class structure or operation.
 # This class derives from Datum, primarily, to give it a name but also to allow it to be stored and manipulated, should you so desire.
 # Functors will automatically Fetch any ...Args specified.
@@ -334,14 +531,18 @@
 # When Executing a Functor, you can say 'next=[...]', in which case multiple Functors will be Executed in sequence. This is necessary for the method propagation machinary to work.
 # When invoking a sequence of Functors, only the result of the last Functor to be Executed or the first Functor to fail will be returned.
 class Functor(Datum):
 
 	def __init__(this, name=INVALID_NAME()):
 		super().__init__(name)
 
+		# Which method to call when executing *this through __call__.
+		this.callMethod = 'Function'
+		this.rollbackMethod = 'Rollback'
+
 		this.initialized = False
 
 		# All necessary args that *this cannot function without.
 		this.requiredKWArgs = []
 
 		# Static arguments are Fetched when *this is first called and never again.
 		# All static arguments are required.
@@ -468,14 +669,24 @@
 		pass
 
 
 	# Override this with any logic you'd like to run at the bottom of __call__
 	def AfterFunction(this):
 		pass
 
+
+	# Override this with any logic you'd like to run at the top of __call__
+	def BeforeRollback(this):
+		pass
+
+
+	# Override this with any logic you'd like to run at the bottom of __call__
+	def AfterRollback(this):
+		pass
+
 	# Create a list of methods / member functions which will search different places for a variable.
 	# See the end of the file for examples of these methods.
 	def PopulateFetchLocations(this):
 		try:
 			for loc in this.fetchFrom:
 				this.fetchLocations.update({loc:getattr(this,f"fetch_location_{loc}")})
 		except:
@@ -853,59 +1064,65 @@
 				logging.error(f"ERROR: {e}")
 				util.LogStack()
 
 
 	# Make functor.
 	# Don't worry about this; logic is abstracted to Function
 	def __call__(this, *args, **kwargs) :
-		logging.debug(f"<---- {this.name} ---->")
+		logging.debug(f"{this.name} ({args}, {kwargs}) {{")
+		FunctorTracker.Push(this)
+
 		ret = None
 		nextRet = None
+		
 		try:
 			this.WarmUp(*args, **kwargs)
 			logging.debug(f"{this.name}({this.args}, {this.kwargs})")
 
-			this.BeforeFunction()
-			ret = this.Function()
+			getattr(this, f"Before{this.callMethod}")()
+			ret = getattr(this, this.callMethod)()
 
-			if (this.DidFunctionSucceed()):
+			if (getattr(this, f"Did{this.callMethod}Succeed")()):
 					this.result = 1
 					# logging.info(f"{this.name} successful!")
 					nextRet = this.CallNext()
 			elif (this.enableRollback):
 				logging.warning(f"{this.name} failed. Attempting Rollback...")
-				this.Rollback()
-				if (this.DidRollbackSucceed()):
+				ret = getattr(this, this.rollbackMethod)()
+				if (getattr(this, f"Did{this.rollbackMethod}Succeed")()):
 					this.result = 2
 					# logging.info(f"Rollback succeeded. All is well.")
 					nextRet = this.CallNext()
 				else:
 					this.result = 3
-					logging.error(f"Rollback FAILED! SYSTEM STATE UNKNOWN!!!")
+					logging.error(f"ROLLBACK FAILED! SYSTEM STATE UNKNOWN!!!")
 			else:
 				this.result = 4
 				logging.error(f"{this.name} failed.")
 
-			this.AfterFunction()
+			getattr(this, f"After{this.callMethod}")()
 
 		except Exception as e:
 			if (this.raiseExceptions):
 				raise e
 			else:
 				logging.error(f"ERROR: {e}")
 				util.LogStack()
 
 		if (this.raiseExceptions and this.result > 2):
 			raise FunctorError(f"{this.name} failed with result {this.result}")
 
-		logging.debug(f">---- {this.name} complete ----<")
 		if (nextRet is not None):
-			return nextRet
-		else:
-			return ret
+			ret = nextRet
+
+		logging.debug(f"return {ret}")
+		FunctorTracker.Pop(this)
+		logging.debug(f"}} ({this.name})")
+
+		return ret
 
 
 	# Adapter for @recoverable.
 	# See Recoverable.py for details
 	def GetExecutor(this):
 		return this.executor
 
@@ -983,686 +1200,14 @@
 		envVar = os.getenv(varName.upper())
 		if (envVar is not None):
 			return envVar, True
 		return default, False
 
 	######## END: Fetch Locations ########
 
-
-def METHOD_PENDING_POPULATION(obj, *args, **kwargs):
-	raise MethodPendingPopulation("METHOD PENDING POPULATION")
-
-# Use the @method() decorator to turn any class function into an eons Method Functor.
-# Methods are Functors which can be implicitly transferred between classes (see Functor.PopulateMethods)
-# Using Methods also gives us full control over the execution of your code; meaning, we can change how Python interprets what you wrote!
-# All Methods will be stored in the method member of your Functor. However, you shouldn't need to access that.
-#
-# If you would like to specify a custom implementation, set the 'impl' kwarg (e.g. @method(impl='MyMethodImplementation'))
-# Beside 'impl', all key-word arguments provided to the @method() decorator will be set as member variables of the created Method.
-# For example, to set whether or not the Method should be propagated, you can use @method(propagate=True).
-# This means, you can create a custom means of interpreting your code with your own feature set and still use this @method decorator.
-# Perhaps you'd like something along the lines of: @method(impl='MakeAwesome', awesomeness=10000).
-# NOTE: in order for impl to work, the implementation class must already be Registered (or this must be called from an appropriate @recoverable function).
-def method(impl='Method', **kwargs):
-
-	# Class decorator with __set_name__, as described here: https://stackoverflow.com/questions/2366713/can-a-decorator-of-an-instance-method-access-the-class
-	class MethodDecorator:
-		def __init__(this, function):
-			this.function = function
-
-		# Apparently, this is called when the decorated function is constructed.
-		def __set_name__(this, cls, functionName):
-			logging.debug(f"Constructing new method for {this.function} in {cls}")
-
-			# Create and configure a new Method
-
-			method = SelfRegistering(impl)
-			method.Constructor(this.function, cls)
-			for key, value in kwargs.items():
-				setattr(method, key, value)
-
-			# Store the new method in the class
-			if (not hasattr(cls, 'classMethods') or not isinstance(cls.classMethods, dict)):
-				cls.classMethods = {}
-			cls.classMethods[functionName] = method
-
-			# Self-destruct by replacing the decorated function.
-			# We rely on Functor.PopulateMethods to re-establish the method as callable.
-			# It seems like this just outright removes the methods. There may be an issue with using __get__ this way.
-			# Regardless deleting the method is okay as long as we add it back before anyone notices.
-			setattr(cls, functionName, METHOD_PENDING_POPULATION.__get__(cls))
-
-	return MethodDecorator
-
-class Method(Functor):
-
-	def __init__(this, name=INVALID_NAME()):
-		super().__init__(name)
-
-		# Methods do not fetch from the environment by default.
-		this.fetchFrom.remove('environment')
-
-		# Whether or not *this should be combined with other Methods of the same name.
-		this.inheritMethods = True
-
-		# Where should inherited methods be inserted?
-		# First here means "before *this".
-		# If False, inherited code will be run after *this.
-		this.inheritedMethodsFirst = True # otherwise ...Last
-
-		# Propagation allows for Functors called after that which defines *this to also call *this.
-		# This system allows for partial, implicit inheritance.
-		# By default, Methods will not be propagated. Use @propagate to enable propagation.
-		this.propagate = False
-
-		# We don't care about these checks right now.
-		# Plus, we can't exactly wrap 2 functions even if we wanted to Rollback.
-		this.functionSucceeded = True
-		this.rollbackSucceeded = True
-		this.enableRollback = False
-
-		# The source code of the function we're implementing.
-		this.source = ""
-
-		# The instance of the class to which *this belongs.
-		# i.e. the object that called *this, aka 'owner', 'caller', etc.
-		this.object = None
-
-		this.original = util.DotDict()
-		this.original.cls = None
-		this.original.function = None
-
-
-	# Make *this execute the code in this.source
-	def UpdateSource(this):
-		wrappedFunctionName = f'_eons_method_{this.name}'
-		completeSource = f'''\
-def {wrappedFunctionName}(this):
-{this.source}
-'''
-		if (this.executor and this.executor.verbosity > 3):
-			logging.debug(f"Source for {this.name} is:\n{completeSource}")
-		code = compile(completeSource, '', 'exec')
-		exec(code)
-		exec(f'this.Function = {wrappedFunctionName}.__get__(this, this.__class__)')
-
-
-
-	# Parse arguments and update the source code
-	# TODO: Implement full python parser to avoid bad string replacement (e.g. "def func(self):... self.selfImprovement" => "... this.object.this.object.Improvement").
-	def PopulateFrom(this, function):
-		this.source = ':'.join(inspect.getsource(function).split(':')[1:]) #Remove the first function definition
-
-		args = inspect.signature(function, follow_wrapped=False).parameters
-		thisSymbol = next(iter(args))
-		#del args[thisSymbol] # ??? 'mappingproxy' object does not support item deletion
-		this.source = this.source.replace(thisSymbol, 'this.object')
-
-		first = True
-		for arg in args.values(): #args.values[1:] also doesn't work.
-			if (first):
-				first = False
-				continue
-
-			replaceWith = arg.name
-
-			if (arg.kind == inspect.Parameter.VAR_POSITIONAL):
-				replaceWith = 'this.args'
-
-			elif (arg.kind == inspect.Parameter.VAR_KEYWORD):
-				replaceWith = 'this.kwargs'
-
-			else:
-				if (arg.default != inspect.Parameter.empty):
-					this.optionalKWArgs[arg.name] = arg.default
-				else:
-					this.requiredKWArgs.append(arg.name)
-				replaceWith = f'this.{arg.name}'
-
-				if (arg.kind in [inspect.Parameter.POSITIONAL_OR_KEYWORD, inspect.Parameter.POSITIONAL_ONLY]):
-					this.argMapping.append(arg.name)
-
-			this.source = this.source.replace(arg.name, replaceWith)
-
-
-	# When properly constructing a Method, rely only on the function *this should implement.
-	# The class and all other properties are irrelevant. However, they are provided and intended for debugging only.
-	def Constructor(this, function, cls):
-		this.name = function.__name__
-		this.original.cls = cls
-		this.original.function = function
-
-		this.PopulateFrom(function)
-		
-		# UpdateSource is called by Functor.PopulateMethods()
-		# this.UpdateSource()
-
-
-	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
-	def PopulatePrecursor(this):
-		if (not this.object):
-			raise MissingArgumentError(f"Call {this.name} from a class instance: {this.original.cls.__name__}.{this.name}(...). Maybe Functor.PopulateMethods() hasn't been called yet?")
-
-		this.executor = this.object.executor
-
-		if ('precursor' in this.kwargs):
-			this.precursor = this.kwargs.pop('precursor')
-		else:
-			this.precursor = None
-
-
-	# Next is set by Functor.PopulateMethods.
-	# We  definitely don't want to Fetch 'next'.
-	def PopulateNext(this):
-		pass
-
-
-	# Method.next should be a list of other Methods, as opposed to the standard string; so, instead of Executor.Execute..., we can directly invoke whatever is next.
-	# We skip all validation here.
-	# We also don't pass any args that were given in the initial function call. Those can all be Fetched from 'precursor'.
-	def CallNext(this):
-		if (not this.next):
-			return None
-
-		for next in this.next:
-			next(precursor=this)
-
-
-# The standard Functor extends Functor to add a set of standard members and methods.
-# This is similar to the standard library in C and C++
-# You must inherit from *this if you would like to use the functionality *this provides. The methods defined will not be propagated.
-class StandardFunctor(Functor):
-	def __init__(this, name="Standard Functor"):
-		super().__init__(name)
-
-	# Override this and do whatever!
-	# This is purposefully vague.
-	def Function(this):
-		pass
-
-
-	# Undo any changes made by UserFunction.
-	# Please override this too!
-	def Rollback(this):
-		pass
-
-
-	# Override this to check results of operation and report on status.
-	# Override this to perform whatever success checks are necessary.
-	def DidFunctionSucceed(this):
-		return this.functionSucceeded
-
-
-	# RETURN whether or not the Rollback was successful.
-	# Override this to perform whatever success checks are necessary.
-	def DidRollbackSucceed(this):
-		return this.rollbackSucceeded
-
-
-	######## START: UTILITIES ########
-
-	# RETURNS: an opened file object for writing.
-	# Creates the path if it does not exist.
-	@method()
-	def CreateFile(this, file, mode="w+"):
-		Path(os.path.dirname(os.path.abspath(file))).mkdir(parents=True, exist_ok=True)
-		return open(file, mode)
-
-	# Copy a file or folder from source to destination.
-	# This really shouldn't be so hard...
-	# root allows us to interpret '/' as something other than the top of the filesystem.
-	@method()
-	def Copy(this, source, destination, root='/'):
-		if (source.startswith('/')):
-			source = str(Path(root).joinpath(source[1:]).resolve())
-		else:
-			source = str(Path(source).resolve())
-		
-		destination = str(Path(destination).resolve())
-		
-		Path(destination).parent.mkdir(parents=True, exist_ok=True)
-
-		if (os.path.isfile(source)):
-			logging.debug(f"Copying file {source} to {destination}")
-			try:
-				shutil.copy(source, destination)
-			except shutil.Error as exc:
-				errors = exc.args[0]
-				for error in errors:
-					src, dst, msg = error
-					logging.debug(f"{msg}")
-		elif (os.path.isdir(source)):
-			logging.debug(f"Copying directory {source} to {destination}")
-			try:
-				shutil.copytree(source, destination)
-			except shutil.Error as exc:
-				errors = exc.args[0]
-				for error in errors:
-					src, dst, msg = error
-					logging.debug(f"{msg}")
-		else:
-			logging.error(f"Could not find source to copy: {source}")
-
-	# Delete a file or folder
-	@method()
-	def Delete(this, target):
-		if (not os.path.exists(target)):
-			logging.debug(f"Unable to delete nonexistent target: {target}")
-			return
-		if (os.path.isfile(target)):
-			logging.debug(f"Deleting file {target}")
-			os.remove(target)
-		elif (os.path.isdir(target)):
-			logging.debug(f"Deleting directory {target}")
-			try:
-				shutil.rmtree(target)
-			except shutil.Error as exc:
-				errors = exc.args[0]
-				for error in errors:
-					src, dst, msg = error
-					logging.debug(f"{msg}")
-
-	# Run whatever.
-	# DANGEROUS!!!!!
-	# RETURN: Return value and, optionally, the output as a list of lines.
-	@method()
-	def RunCommand(this, command, saveout=False, raiseExceptions=True):
-		logging.debug(f"================ Running command: {command} ================")
-		process = Popen(command, stdout=PIPE, stderr=STDOUT, shell=True)
-		output = []
-		while process.poll() is None:
-			line = process.stdout.readline().decode('utf8')[:-1]
-			if (saveout):
-				output.append(line)
-			if (line):
-				logging.debug(f"| {line}")  # [:-1] to strip excessive new lines.
-
-		message = f"Command returned {process.returncode}: {command}"
-		logging.debug(message)
-		if (raiseExceptions and process.returncode is not None and process.returncode):
-			raise CommandUnsuccessful(message)
-		
-		logging.debug(f"================ Completed command: {command} ================")
-		if (saveout):
-			return process.returncode, output
-		
-		return process.returncode
-	######## END: UTILITIES ########
-
-
-# ExecutorTracker is a global singleton which keeps a record of all Executors that have been launched.
-# This can be abused quite a bit, so please try to restrict usage of this to only:
-# * Ease of use global functions
-#
-# Thanks! 
-class ExecutorTracker:
-	def __init__(this):
-		# Singletons man...
-		if "instance" not in ExecutorTracker.__dict__:
-			logging.debug(f"Creating new ExecutorTracker: {this}")
-			ExecutorTracker.instance = this
-		else:
-			return None
-
-		this.executors = [None]
-
-	@staticmethod
-	def Instance():
-		if "instance" not in ExecutorTracker.__dict__:
-			ExecutorTracker()
-		return ExecutorTracker.instance
-
-	@staticmethod
-	def Push(executor):
-		ExecutorTracker.Instance().executors.append(executor)
-
-		# Adding the executor to our list here increases its reference count.
-		# Executors are supposed to remove themselves from this list when they are deleted.
-		# A python object cannot be deleted if it has references.
-		# Thus, we forcibly decrease the reference count and rely on Exectuor's self-reporting to avoid accessing deallocated memory.
-		# This appears to cause segfaults on some systems, so we'll just live with the fact that Executors will never be destroyed.
-		# If you want your executor to stop being tracked, do it yourself. :(
-		#
-		# ctypes.pythonapi.Py_DecRef(ctypes.py_object(executor))
-
-		logging.debug(f"Now tracking Executor: {executor}")
-
-	@staticmethod
-	def Pop(executor):
-		try:
-			ExecutorTracker.Instance().executors.remove(executor)
-			logging.debug(f"No longer tracking Executor: {executor}")
-		except:
-			pass
-
-	@staticmethod
-	def GetLatest():
-		return ExecutorTracker.Instance().executors[-1]
-
-
-# Global Fetch() function.
-# Uses the latest registered Executor
-def Fetch(varName, default=None, fetchFrom=None, start=True, attempted=None):
-    return ExecutorTracker.GetLatest().Fetch(varName, default, fetchFrom, start, attempted)
-
-# Ease-of-use wrapper for the global Fetch()
-def f(varName, default=None, fetchFrom=None, start=True, attempted=None):
-    Fetch(varName, default, fetchFrom, start, attempted)
-
-# A DataContainer allows Data to be stored and worked with.
-# This class is intended to be derived from and added to.
-# Each DataContainer is comprised of multiple Data (see Datum.py for more).
-# NOTE: DataContainers are, themselves Data. Thus, you can nest your child classes however you would like.
-class DataContainer(Datum):
-
-	def __init__(this, name=INVALID_NAME()):
-		super().__init__(name)
-
-		# The data *this contains.
-		this.data = []
-
-
-	# RETURNS: an empty, invalid Datum.
-	def InvalidDatum(this):
-		ret = Datum()
-		ret.Invalidate()
-		return ret
-
-
-	# Sort things! Requires by be a valid attribute of all Data.
-	def SortData(this, by):
-		this.data.sort(key=operator.attrgetter(by))
-
-
-	# Adds a Datum to *this
-	def AddDatum(this, datum):
-		this.data.append(datum)
-
-
-	# RETURNS: a Datum with datumAttribute equal to match, an invalid Datum if none found.
-	def GetDatumBy(this, datumAttribute, match):
-		for d in this.data:
-			try: # within for loop 'cause maybe there's an issue with only 1 Datum and the rest are fine.
-				if (str(util.GetAttr(d, datumAttribute)) == str(match)):
-					return d
-			except Exception as e:
-				logging.error(f"{this.name} - {e.message}")
-				continue
-		return this.InvalidDatum()
-
-
-	# RETURNS: a Datum of the given name, an invalid Datum if none found.
-	def GetDatum(this, name):
-		return this.GetDatumBy('name', name)
-
-
-	# Removes all Data in toRem from *this.
-	# RETURNS: the Data removed
-	def RemoveData(this, toRem):
-		# logging.debug(f"Removing {toRem}")
-		this.data = [d for d in this.data if d not in toRem]
-		return toRem
-
-
-	# Removes all Data which match toRem along the given attribute
-	def RemoveDataBy(this, datumAttribute, toRem):
-		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) in list(map(str, toRem))]
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data in *this except toKeep.
-	# RETURNS: the Data removed
-	def KeepOnlyData(this, toKeep):
-		toRem = [d for d in this.data if d not in toKeep]
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data except those that match toKeep along the given attribute
-	# RETURNS: the Data removed
-	def KeepOnlyDataBy(this, datumAttribute, toKeep):
-		# logging.debug(f"Keeping only class with a {datumAttribute} of {toKeep}")
-		# toRem = []
-		# for d in this.class:
-		#	 shouldRem = False
-		#	 for k in toKeep:
-		#		 if (str(util.GetAttr(d, datumAttribute)) == str(k)):
-		#			 logging.debug(f"found {k} in {d.__dict__}")
-		#			 shouldRem = True
-		#			 break
-		#	 if (shouldRem):
-		#		 toRem.append(d)
-		#	 else:
-		#		 logging.debug(f"{k} not found in {d.__dict__}")
-		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) not in list(map(str, toKeep))]
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data with the name "INVALID NAME"
-	# RETURNS: the removed Data
-	def RemoveAllUnlabeledData(this):
-		toRem = []
-		for d in this.data:
-			if (d.name =="INVALID NAME"):
-				toRem.append(d)
-		return this.RemoveData(toRem)
-
-
-	# Removes all invalid Data
-	# RETURNS: the removed Data
-	def RemoveAllInvalidData(this):
-		toRem = []
-		for d in this.data:
-			if (not d.IsValid()):
-				toRem.append(d)
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data that have an attribute value relative to target.
-	# The given relation can be things like operator.le (i.e. <=)
-	#   See https://docs.python.org/3/library/operator.html for more info.
-	# If ignoreNames is specified, any Data of those names will be ignored.
-	# RETURNS: the Data removed
-	def RemoveDataRelativeToTarget(this, datumAttribute, relation, target, ignoreNames = []):
-		try:
-			toRem = []
-			for d in this.data:
-				if (ignoreNames and d.name in ignoreNames):
-					continue
-				if (relation(util.GetAttr(d, datumAttribute), target)):
-					toRem.append(d)
-			return this.RemoveData(toRem)
-		except Exception as e:
-			logging.error(f"{this.name} - {e.message}")
-			return []
-
-
-	# Removes any Data that have the same datumAttribute as a previous Datum, keeping only the first.
-	# RETURNS: The Data removed
-	def RemoveDuplicateDataOf(this, datumAttribute):
-		toRem = [] # list of Data
-		alreadyProcessed = [] # list of strings, not whatever datumAttribute is.
-		for d1 in this.data:
-			skip = False
-			for dp in alreadyProcessed:
-				if (str(util.GetAttr(d1, datumAttribute)) == dp):
-					skip = True
-					break
-			if (skip):
-				continue
-			for d2 in this.data:
-				if (d1 is not d2 and str(util.GetAttr(d1, datumAttribute)) == str(util.GetAttr(d2, datumAttribute))):
-					logging.info(f"Removing duplicate Datum {d2} with unique id {util.GetAttr(d2, datumAttribute)}")
-					toRem.append(d2)
-					alreadyProcessed.append(str(util.GetAttr(d1, datumAttribute)))
-		return this.RemoveData(toRem)
-
-
-	# Adds all Data from otherDataContainer to *this.
-	# If there are duplicate Data identified by the attribute preventDuplicatesOf, they are removed.
-	# RETURNS: the Data removed, if any.
-	def ImportDataFrom(this, otherDataContainer, preventDuplicatesOf=None):
-		this.data.extend(otherDataContainer.data);
-		if (preventDuplicatesOf is not None):
-			return this.RemoveDuplicateDataOf(preventDuplicatesOf)
-		return []
-
-
-
-# Use an ErrorStringParser for each "parsers" in order to avoid having to override the GetObjectFromError method and create a new class for every error you want to handle.
-# ErrorStringParsers enable ErrorResolutions to be created on a per-functionality, rather than per-error basis, reducing the total amount of duplicate code.
-# Each error has a different string. In order to get the object of the error, we have to know where the object starts and ends.
-# NOTE: this assumes only 1 object per string. Maybe fancier parsing logic can be added in the future.
-#
-# startPosition is always positive
-# endPosition is always negative
-class ErrorStringParser:
-
-	def __init__(this, applicableError, startPosition, endPosition):
-		this.applicableError = applicableError
-		this.startPosition = startPosition
-		this.endPosition = endPosition
-
-	def Parse(this, errorString):
-		end = this.endPosition
-		if (not end):
-			end = len(errorString)
-		return errorString[this.startPosition:end]
-
-
-# ErrorResolution is a Functor which can be executed when an Exception is raised.
-# The goal of this class is to do some kind of work that will fix the problem on the second try of whatever generated the error.
-class ErrorResolution(StandardFunctor):
-
-	def __init__(this, name=INVALID_NAME()):
-		super().__init__(name)
-
-		# What errors, as ErrorStringParser objects, is *this prepared to handle?
-		this.parsers = []
-
-		this.error = None
-		this.errorType = ""
-		this.errorString = ""
-		this.errorObject = ""
-		this.errorResolutionStack = {}
-
-		# Provided directly from the recoverable decorator.
-		this.optionalKWArgs["obj"] = None
-		this.optionalKWArgs["function"] = None
-
-		# We do want to know whether or not we should attempt to run whatever failed again.
-		# So, let's store that in functionSucceeded. Meaning if this.functionSucceeded, try the original method again.
-		# No rollback, by default and definitely don't throw Exceptions.
-		this.enableRollback = False
-		this.functionSucceeded = True
-		this.raiseExceptions = False
-
-		this.errorShouldBeResolved = False
-
-
-
-	# Put your logic here!
-	def Resolve(this):
-		# You get the following members:
-		# this.error (an Exception)
-		# this.errorString (a string cast of the Exception)
-		# this.errorType (a string)
-		# this.errorObjet (a string or whatever you return from GetObjectFromError())
-
-		# You get the following guarantees:
-		# *this has not been called on this particular error before.
-		# the error given is applicable to *this per this.parsers
-
-		###############################################
-		# Please throw errors if something goes wrong #
-		# Otherwise, set this.errorShouldBeResolved   #
-		###############################################
-		
-		pass
-
-
-
-	# Helper method for creating ErrorStringParsers
-	# To use this, simply take an example output and replace the object you want to extract with "OBJECT"
-	def ApplyTo(this, error, exampleString):
-		match = re.search('OBJECT', exampleString)
-		this.parsers.append(ErrorStringParser(error, match.start(), match.end() - len(exampleString)))
-
-
-	# Get the type of this.error as a string.
-	def GetErrorType(this):
-		return type(this.error).__name__
-
-
-	# Get an actionable object from the error.
-	# For example, if the error is 'ModuleNotFoundError', what is the module?
-	def GetObjectFromError(this):
-		for parser in this.parsers:
-			if (parser.applicableError != this.errorType):
-				continue
-
-			this.errorObject = parser.Parse(this.errorString)
-			return
-
-		raise ErrorResolutionError(f"{this.name} cannot parse error object from ({this.errorType}): {str(this.error)}.")
-
-
-	# Determine if this resolution method is applicable.
-	def CanProcess(this):
-		return this.GetErrorType() in [parser.applicableError for parser in this.parsers]
-
-
-	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
-	def ParseInitialArgs(this):
-		super().ParseInitialArgs()
-		if ('error' in this.kwargs):
-			this.error = this.kwargs.pop('error')
-			# Just assume the error is an actual Exception object.
-		else:
-			raise ErrorResolutionError(f"{this.name} was not given an error to resolve.")
-
-		this.errorString = str(this.error)
-		this.errorType = this.GetErrorType()
-
-		# Internal member to avoid processing duplicates
-		this.errorResolutionStack = this.executor.errorResolutionStack
-
-
-	# Error resolution is unchained.
-	def PopulateNext(this):
-		this.next = []
-
-
-	# Override of Functor method.
-	# We'll keep calling this until an error is raised.
-	def Function(this):
-		this.functionSucceeded = True
-		this.errorShouldBeResolved = True
-		
-		if (not this.CanProcess()):
-			this.errorShouldBeResolved = False
-			return this.errorResolutionStack, this.errorShouldBeResolved
-
-		if (not this.errorString in this.errorResolutionStack.keys()):
-			this.errorResolutionStack.update({this.errorString:[]})
-		
-		if (this.name in this.errorResolutionStack[this.errorString]):
-			raise FailedErrorResolution(f"{this.name} already tried and failed to resolve {this.errorType}: {this.errorString}.")
-
-		this.GetObjectFromError()
-
-		try:
-			this.Resolve()
-		except Exception as e:
-			logging.error(f"Error resolution with {this.name} failed: {e}")
-			util.LogStack()
-			this.functionSucceeded = False
-		
-		this.errorResolutionStack[this.errorString].append(this.name)
-		return this.errorResolutionStack, this.errorShouldBeResolved
-
 #from .Executor import Executor # don't import this, it'll be circular!
 
 # @recoverable
 # Decorating another function with this method will engage the error recovery system provided by *this.
 # To use this, you must define a GetExecutor() method in your class and decorate the functions you want to recover from.
 # For more info, see Executor.ResolveError and the README.md
 def recoverable(function):
@@ -1735,14 +1280,64 @@
 		return ret
 
 	#  We failed to resolve the error. Die
 	sys.tracebacklimit = 0 # traceback is NOT helpful here.
 	raise FailedErrorResolution(f"Tried and failed to resolve: {error} STACK: {executor.errorResolutionStack}. See earlier logs (in debug) for traceback.")
 
 
+# ExecutorTracker is a global singleton which keeps a record of all Executors that have been launched.
+# This can be abused quite a bit, so please try to restrict usage of this to only:
+# * Ease of use global functions
+#
+# Thanks! 
+class ExecutorTracker:
+	def __init__(this):
+		# Singletons man...
+		if "instance" not in ExecutorTracker.__dict__:
+			logging.debug(f"Creating new ExecutorTracker: {this}")
+			ExecutorTracker.instance = this
+		else:
+			return None
+
+		this.executors = [None]
+
+	@staticmethod
+	def Instance():
+		if "instance" not in ExecutorTracker.__dict__:
+			ExecutorTracker()
+		return ExecutorTracker.instance
+
+	@staticmethod
+	def Push(executor):
+		ExecutorTracker.Instance().executors.append(executor)
+
+		# Adding the executor to our list here increases its reference count.
+		# Executors are supposed to remove themselves from this list when they are deleted.
+		# A python object cannot be deleted if it has references.
+		# Thus, we forcibly decrease the reference count and rely on Exectuor's self-reporting to avoid accessing deallocated memory.
+		# This appears to cause segfaults on some systems, so we'll just live with the fact that Executors will never be destroyed.
+		# If you want your executor to stop being tracked, do it yourself. :(
+		#
+		# ctypes.pythonapi.Py_DecRef(ctypes.py_object(executor))
+
+		logging.debug(f"Now tracking Executor: {executor}")
+
+	@staticmethod
+	def Pop(executor):
+		try:
+			ExecutorTracker.Instance().executors.remove(executor)
+			logging.debug(f"No longer tracking Executor: {executor}")
+		except:
+			pass
+
+	@staticmethod
+	def GetLatest():
+		return ExecutorTracker.Instance().executors[-1]
+
+
 # Executor: a base class for user interfaces.
 # An Executor is a functor and can be executed as such.
 # For example
 #	class MyExecutor(Executor):
 #		def __init__(this):
 #			super().__init__()
 #	. . .
@@ -1752,15 +1347,14 @@
 class Executor(DataContainer, Functor):
 
 	def __init__(this, name=INVALID_NAME(), descriptionStr="Eons python framework. Extend as thou wilt."):
 		this.SetupLogging()
 
 		super().__init__(name)
 
-		# Error resolution configuration.
 		this.resolveErrors = True
 		this.errorRecursionDepth = 0
 		this.errorResolutionStack = {}
 		this.resolveErrorsWith = [ # order matters: FIFO (first is first).
 			'find_by_fetch',
 			'install_from_repo_with_default_package_type',
 			'install_from_repo',
@@ -1880,29 +1474,39 @@
 			util.AddLoggingLevel('recovery', logging.ERROR+1)
 		except:
 			# Could already be setup.
 			pass
 
 		class CustomFormatter(logging.Formatter):
 
-			preFormat = util.console.GetColorCode('white', 'dark') + '%(asctime)s'
-			format = ' [%(levelname)4s] %(message)s '
+			preFormat = util.console.GetColorCode('white', 'dark') + '%(asctime)s '
+			levelName = '[%(levelname)8s] '
+			indentation = util.console.GetColorCode('blue', 'dark', styles=['faint']) + '__INDENTATION__' + util.console.GetColorCode('white', 'dark', styles=['none'])
+			message = '%(message)s '
 			postFormat = util.console.GetColorCode('white', 'dark') + '(%(filename)s:%(lineno)s)' + util.console.resetStyle
 
 			formats = {
-				logging.DEBUG: preFormat + util.console.GetColorCode('cyan', 'dark') + format + postFormat,
-				logging.INFO: preFormat + util.console.GetColorCode('white', 'light') + format + postFormat,
-				logging.WARNING: preFormat + util.console.GetColorCode('yellow', 'light') + format + postFormat,
-				logging.ERROR: preFormat + util.console.GetColorCode('red', 'dark') + format + postFormat,
-				logging.RECOVERY: preFormat + util.console.GetColorCode('green', 'light') + format + postFormat,
-				logging.CRITICAL: preFormat + util.console.GetColorCode('red', 'light', styles=['bold']) + format + postFormat
+				logging.DEBUG: preFormat + levelName + indentation + util.console.GetColorCode('cyan', 'dark') + message + postFormat,
+				logging.INFO: preFormat + levelName + indentation + util.console.GetColorCode('white', 'light') + message + postFormat,
+				logging.WARNING: preFormat + levelName + indentation + util.console.GetColorCode('yellow', 'light') + message + postFormat,
+				logging.ERROR: preFormat + levelName + indentation + util.console.GetColorCode('red', 'dark') + message + postFormat,
+				logging.RECOVERY: preFormat + levelName + indentation + util.console.GetColorCode('green', 'light') + message + postFormat,
+				logging.CRITICAL: preFormat + levelName + indentation + util.console.GetColorCode('red', 'light', styles=['bold']) + message + postFormat
 			}
 
 			def format(this, record):
 				log_fmt = this.formats.get(record.levelno)
+				if (hasattr(logging.getLogger(), 'tab_logs') and getattr(logging.getLogger(), 'tab_logs')):
+					tabWidth = 4
+					if (hasattr(logging.getLogger(), 'tab_width')):
+						tabWidth = getattr(logging.getLogger(), 'tab_width')
+					tabWidth = int(tabWidth) - 1
+					log_fmt = log_fmt.replace('__INDENTATION__', f"|{' ' * tabWidth}" * (FunctorTracker.GetCount() - 1)) # -1 because we're already in a Functor.
+				else:
+					log_fmt = log_fmt.replace('__INDENTATION__', ' ')
 				formatter = logging.Formatter(log_fmt, datefmt = '%H:%M:%S')
 				return formatter.format(record)
 
 		# Skip setting up logging if it's already been done.
 		if (hasattr(logging.getLogger(), 'setupBy')):
 			return
 
@@ -2044,17 +1648,19 @@
 			this.repo[key] = this.Fetch(f"repo_{key}", default=default)
 
 
 	# How do we get the verbosity level and what do we do with it?
 	# This method should set log levels, etc.
 	def SetVerbosity(this, fetch=True):
 
+		fetchFrom = ['args', 'config', 'environment']
+
 		if (fetch):
 			# Take the highest of -v vs --verbosity
-			verbosity = this.EvaluateToType(this.Fetch('verbosity', 0, ['args', 'config', 'environment']))
+			verbosity = this.EvaluateToType(this.Fetch('verbosity', 0, fetchFrom))
 			if (verbosity > this.verbosity):
 				logging.debug(f"Setting verbosity to {verbosity}") # debug statements will be available when using external systems, like pytest.
 				this.verbosity = verbosity
 
 		if (this.verbosity == 0):
 			logging.getLogger().handlers[0].setLevel(logging.CRITICAL)
 			logging.getLogger().setLevel(logging.CRITICAL)
@@ -2064,14 +1670,22 @@
 		elif (this.verbosity == 2):
 			logging.getLogger().handlers[0].setLevel(logging.INFO)
 			logging.getLogger().setLevel(logging.INFO)
 		elif(this.verbosity >= 3):
 			logging.getLogger().handlers[0].setLevel(logging.DEBUG)
 			logging.getLogger().setLevel(logging.DEBUG)
 
+		if (fetch):
+			tabLogs, foundTabLogs = this.Fetch('tab_logs', False, fetchFrom, start=False)
+			tabLogs = this.EvaluateToType(tabLogs)
+			if (tabLogs or (this.verbosity >= 3 and not foundTabLogs)):
+				setattr(logging.getLogger(), 'tab_logs', True)
+				tabWidth = this.Fetch('logging_tab_width', 2, fetchFrom)
+				setattr(logging.getLogger(), 'tab_width', int(tabWidth))
+
 
 	# Do the argparse thing.
 	# Extra arguments are converted from --this-format to this_format, without preceding dashes. For example, --repo-url ... becomes repo_url ...
 	# NOTE: YOU CANNOT USE @recoverable METHODS HERE!
 	def ParseArgs(this):
 		this.parsedArgs, extraArgs = this.argparser.parse_known_args()
 
@@ -2404,7 +2018,470 @@
 		for key, val in this.extraArgs.items():
 			if (key == varName):
 				return val, True
 		return default, False
 
 	######## END: Fetch Locations ########
 
+
+def METHOD_PENDING_POPULATION(obj, *args, **kwargs):
+	raise MethodPendingPopulation("METHOD PENDING POPULATION")
+
+# Use the @method() decorator to turn any class function into an eons Method Functor.
+# Methods are Functors which can be implicitly transferred between classes (see Functor.PopulateMethods)
+# Using Methods also gives us full control over the execution of your code; meaning, we can change how Python interprets what you wrote!
+# All Methods will be stored in the method member of your Functor. However, you shouldn't need to access that.
+#
+# If you would like to specify a custom implementation, set the 'impl' kwarg (e.g. @method(impl='MyMethodImplementation'))
+# Beside 'impl', all key-word arguments provided to the @method() decorator will be set as member variables of the created Method.
+# For example, to set whether or not the Method should be propagated, you can use @method(propagate=True).
+# This means, you can create a custom means of interpreting your code with your own feature set and still use this @method decorator.
+# Perhaps you'd like something along the lines of: @method(impl='MakeAwesome', awesomeness=10000).
+# NOTE: in order for impl to work, the implementation class must already be Registered (or this must be called from an appropriate @recoverable function).
+def method(impl='Method', **kwargs):
+
+	# Class decorator with __set_name__, as described here: https://stackoverflow.com/questions/2366713/can-a-decorator-of-an-instance-method-access-the-class
+	class MethodDecorator:
+		def __init__(this, function):
+			this.function = function
+
+		# Apparently, this is called when the decorated function is constructed.
+		def __set_name__(this, cls, functionName):
+			logging.debug(f"Constructing new method for {this.function} in {cls}")
+
+			# Create and configure a new Method
+
+			method = SelfRegistering(impl)
+			method.Constructor(this.function, cls)
+			for key, value in kwargs.items():
+				setattr(method, key, value)
+
+			# Store the new method in the class
+			if (not hasattr(cls, 'classMethods') or not isinstance(cls.classMethods, dict)):
+				cls.classMethods = {}
+			cls.classMethods[functionName] = method
+
+			# Self-destruct by replacing the decorated function.
+			# We rely on Functor.PopulateMethods to re-establish the method as callable.
+			# It seems like this just outright removes the methods. There may be an issue with using __get__ this way.
+			# Regardless deleting the method is okay as long as we add it back before anyone notices.
+			setattr(cls, functionName, METHOD_PENDING_POPULATION.__get__(cls))
+
+	return MethodDecorator
+
+class Method(Functor):
+
+	def __init__(this, name=INVALID_NAME()):
+		super().__init__(name)
+
+		# Methods do not fetch from the environment by default.
+		this.fetchFrom.remove('environment')
+
+		# Whether or not *this should be combined with other Methods of the same name.
+		this.inheritMethods = True
+
+		# Where should inherited methods be inserted?
+		# First here means "before *this".
+		# If False, inherited code will be run after *this.
+		this.inheritedMethodsFirst = True # otherwise ...Last
+
+		# Propagation allows for Functors called after that which defines *this to also call *this.
+		# This system allows for partial, implicit inheritance.
+		# By default, Methods will not be propagated. Use @propagate to enable propagation.
+		this.propagate = False
+
+		# We don't care about these checks right now.
+		# Plus, we can't exactly wrap 2 functions even if we wanted to Rollback.
+		this.functionSucceeded = True
+		this.rollbackSucceeded = True
+		this.enableRollback = False
+
+		# The source code of the function we're implementing.
+		this.source = ""
+
+		# The instance of the class to which *this belongs.
+		# i.e. the object that called *this, aka 'owner', 'caller', etc.
+		this.object = None
+
+		this.original = util.DotDict()
+		this.original.cls = None
+		this.original.function = None
+
+
+	# Make *this execute the code in this.source
+	def UpdateSource(this):
+		wrappedFunctionName = f'_eons_method_{this.name}'
+		completeSource = f'''\
+def {wrappedFunctionName}(this):
+{this.source}
+'''
+		if (this.executor and this.executor.verbosity > 3):
+			logging.debug(f"Source for {this.name} is:\n{completeSource}")
+		code = compile(completeSource, '', 'exec')
+		exec(code)
+		exec(f'this.Function = {wrappedFunctionName}.__get__(this, this.__class__)')
+
+
+
+	# Parse arguments and update the source code
+	# TODO: Implement full python parser to avoid bad string replacement (e.g. "def func(self):... self.selfImprovement" => "... this.object.this.object.Improvement").
+	def PopulateFrom(this, function):
+		this.source = ':'.join(inspect.getsource(function).split(':')[1:]) #Remove the first function definition
+
+		args = inspect.signature(function, follow_wrapped=False).parameters
+		thisSymbol = next(iter(args))
+		#del args[thisSymbol] # ??? 'mappingproxy' object does not support item deletion
+		this.source = this.source.replace(thisSymbol, 'this.object')
+
+		first = True
+		for arg in args.values(): #args.values[1:] also doesn't work.
+			if (first):
+				first = False
+				continue
+
+			replaceWith = arg.name
+
+			if (arg.kind == inspect.Parameter.VAR_POSITIONAL):
+				replaceWith = 'this.args'
+
+			elif (arg.kind == inspect.Parameter.VAR_KEYWORD):
+				replaceWith = 'this.kwargs'
+
+			else:
+				if (arg.default != inspect.Parameter.empty):
+					this.optionalKWArgs[arg.name] = arg.default
+				else:
+					this.requiredKWArgs.append(arg.name)
+				replaceWith = f'this.{arg.name}'
+
+				if (arg.kind in [inspect.Parameter.POSITIONAL_OR_KEYWORD, inspect.Parameter.POSITIONAL_ONLY]):
+					this.argMapping.append(arg.name)
+
+			this.source = this.source.replace(arg.name, replaceWith)
+
+
+	# When properly constructing a Method, rely only on the function *this should implement.
+	# The class and all other properties are irrelevant. However, they are provided and intended for debugging only.
+	def Constructor(this, function, cls):
+		this.name = function.__name__
+		this.original.cls = cls
+		this.original.function = function
+
+		this.PopulateFrom(function)
+		
+		# UpdateSource is called by Functor.PopulateMethods()
+		# this.UpdateSource()
+
+
+	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
+	def PopulatePrecursor(this):
+		if (not this.object):
+			raise MissingArgumentError(f"Call {this.name} from a class instance: {this.original.cls.__name__}.{this.name}(...). Maybe Functor.PopulateMethods() hasn't been called yet?")
+
+		this.executor = this.object.executor
+
+		if ('precursor' in this.kwargs):
+			this.precursor = this.kwargs.pop('precursor')
+		else:
+			this.precursor = None
+
+
+	# Next is set by Functor.PopulateMethods.
+	# We  definitely don't want to Fetch 'next'.
+	def PopulateNext(this):
+		pass
+
+
+	# Method.next should be a list of other Methods, as opposed to the standard string; so, instead of Executor.Execute..., we can directly invoke whatever is next.
+	# We skip all validation here.
+	# We also don't pass any args that were given in the initial function call. Those can all be Fetched from 'precursor'.
+	def CallNext(this):
+		if (not this.next):
+			return None
+
+		for next in this.next:
+			next(precursor=this)
+
+
+# The standard Functor extends Functor to add a set of standard members and methods.
+# This is similar to the standard library in C and C++
+# You must inherit from *this if you would like to use the functionality *this provides. The methods defined will not be propagated.
+class StandardFunctor(Functor):
+	def __init__(this, name="Standard Functor"):
+		super().__init__(name)
+
+	# Override this and do whatever!
+	# This is purposefully vague.
+	def Function(this):
+		pass
+
+
+	# Undo any changes made by UserFunction.
+	# Please override this too!
+	def Rollback(this):
+		pass
+
+
+	# Override this to check results of operation and report on status.
+	# Override this to perform whatever success checks are necessary.
+	def DidFunctionSucceed(this):
+		return this.functionSucceeded
+
+
+	# RETURN whether or not the Rollback was successful.
+	# Override this to perform whatever success checks are necessary.
+	def DidRollbackSucceed(this):
+		return this.rollbackSucceeded
+
+
+	######## START: UTILITIES ########
+
+	# RETURNS: an opened file object for writing.
+	# Creates the path if it does not exist.
+	@method()
+	def CreateFile(this, file, mode="w+"):
+		Path(os.path.dirname(os.path.abspath(file))).mkdir(parents=True, exist_ok=True)
+		return open(file, mode)
+
+	# Copy a file or folder from source to destination.
+	# This really shouldn't be so hard...
+	# root allows us to interpret '/' as something other than the top of the filesystem.
+	@method()
+	def Copy(this, source, destination, root='/'):
+		if (source.startswith('/')):
+			source = str(Path(root).joinpath(source[1:]).resolve())
+		else:
+			source = str(Path(source).resolve())
+		
+		destination = str(Path(destination).resolve())
+		
+		Path(destination).parent.mkdir(parents=True, exist_ok=True)
+
+		if (os.path.isfile(source)):
+			logging.debug(f"Copying file {source} to {destination}")
+			try:
+				shutil.copy(source, destination)
+			except shutil.Error as exc:
+				errors = exc.args[0]
+				for error in errors:
+					src, dst, msg = error
+					logging.debug(f"{msg}")
+		elif (os.path.isdir(source)):
+			logging.debug(f"Copying directory {source} to {destination}")
+			try:
+				shutil.copytree(source, destination)
+			except shutil.Error as exc:
+				errors = exc.args[0]
+				for error in errors:
+					src, dst, msg = error
+					logging.debug(f"{msg}")
+		else:
+			logging.error(f"Could not find source to copy: {source}")
+
+	# Delete a file or folder
+	@method()
+	def Delete(this, target):
+		if (not os.path.exists(target)):
+			logging.debug(f"Unable to delete nonexistent target: {target}")
+			return
+		if (os.path.isfile(target)):
+			logging.debug(f"Deleting file {target}")
+			os.remove(target)
+		elif (os.path.isdir(target)):
+			logging.debug(f"Deleting directory {target}")
+			try:
+				shutil.rmtree(target)
+			except shutil.Error as exc:
+				errors = exc.args[0]
+				for error in errors:
+					src, dst, msg = error
+					logging.debug(f"{msg}")
+
+	# Run whatever.
+	# DANGEROUS!!!!!
+	# RETURN: Return value and, optionally, the output as a list of lines.
+	@method()
+	def RunCommand(this, command, saveout=False, raiseExceptions=True):
+		logging.debug(f"================ Running command: {command} ================")
+		process = Popen(command, stdout=PIPE, stderr=STDOUT, shell=True)
+		output = []
+		while process.poll() is None:
+			line = process.stdout.readline().decode('utf8')[:-1]
+			if (saveout):
+				output.append(line)
+			if (line):
+				logging.debug(f"| {line}")  # [:-1] to strip excessive new lines.
+
+		message = f"Command returned {process.returncode}: {command}"
+		logging.debug(message)
+		if (raiseExceptions and process.returncode is not None and process.returncode):
+			raise CommandUnsuccessful(message)
+		
+		logging.debug(f"================ Completed command: {command} ================")
+		if (saveout):
+			return process.returncode, output
+		
+		return process.returncode
+	######## END: UTILITIES ########
+
+
+# Global Fetch() function.
+# Uses the latest registered Executor
+def Fetch(varName, default=None, fetchFrom=None, start=True, attempted=None):
+    return ExecutorTracker.GetLatest().Fetch(varName, default, fetchFrom, start, attempted)
+
+# Ease-of-use wrapper for the global Fetch()
+def f(varName, default=None, fetchFrom=None, start=True, attempted=None):
+    Fetch(varName, default, fetchFrom, start, attempted)
+
+# Use an ErrorStringParser for each "parsers" in order to avoid having to override the GetObjectFromError method and create a new class for every error you want to handle.
+# ErrorStringParsers enable ErrorResolutions to be created on a per-functionality, rather than per-error basis, reducing the total amount of duplicate code.
+# Each error has a different string. In order to get the object of the error, we have to know where the object starts and ends.
+# NOTE: this assumes only 1 object per string. Maybe fancier parsing logic can be added in the future.
+#
+# startPosition is always positive
+# endPosition is always negative
+class ErrorStringParser:
+
+	def __init__(this, applicableError, startPosition, endPosition):
+		this.applicableError = applicableError
+		this.startPosition = startPosition
+		this.endPosition = endPosition
+
+	def Parse(this, errorString):
+		end = this.endPosition
+		if (not end):
+			end = len(errorString)
+		return errorString[this.startPosition:end]
+
+
+# ErrorResolution is a Functor which can be executed when an Exception is raised.
+# The goal of this class is to do some kind of work that will fix the problem on the second try of whatever generated the error.
+class ErrorResolution(StandardFunctor):
+
+	def __init__(this, name=INVALID_NAME()):
+		super().__init__(name)
+
+		# What errors, as ErrorStringParser objects, is *this prepared to handle?
+		this.parsers = []
+
+		this.error = None
+		this.errorType = ""
+		this.errorString = ""
+		this.errorObject = ""
+		this.errorResolutionStack = {}
+
+		# Provided directly from the recoverable decorator.
+		this.optionalKWArgs["obj"] = None
+		this.optionalKWArgs["function"] = None
+
+		# We do want to know whether or not we should attempt to run whatever failed again.
+		# So, let's store that in functionSucceeded. Meaning if this.functionSucceeded, try the original method again.
+		# No rollback, by default and definitely don't throw Exceptions.
+		this.enableRollback = False
+		this.functionSucceeded = True
+		this.raiseExceptions = False
+
+		this.errorShouldBeResolved = False
+
+
+
+	# Put your logic here!
+	def Resolve(this):
+		# You get the following members:
+		# this.error (an Exception)
+		# this.errorString (a string cast of the Exception)
+		# this.errorType (a string)
+		# this.errorObjet (a string or whatever you return from GetObjectFromError())
+
+		# You get the following guarantees:
+		# *this has not been called on this particular error before.
+		# the error given is applicable to *this per this.parsers
+
+		###############################################
+		# Please throw errors if something goes wrong #
+		# Otherwise, set this.errorShouldBeResolved   #
+		###############################################
+		
+		pass
+
+
+
+	# Helper method for creating ErrorStringParsers
+	# To use this, simply take an example output and replace the object you want to extract with "OBJECT"
+	def ApplyTo(this, error, exampleString):
+		match = re.search('OBJECT', exampleString)
+		this.parsers.append(ErrorStringParser(error, match.start(), match.end() - len(exampleString)))
+
+
+	# Get the type of this.error as a string.
+	def GetErrorType(this):
+		return type(this.error).__name__
+
+
+	# Get an actionable object from the error.
+	# For example, if the error is 'ModuleNotFoundError', what is the module?
+	def GetObjectFromError(this):
+		for parser in this.parsers:
+			if (parser.applicableError != this.errorType):
+				continue
+
+			this.errorObject = parser.Parse(this.errorString)
+			return
+
+		raise ErrorResolutionError(f"{this.name} cannot parse error object from ({this.errorType}): {str(this.error)}.")
+
+
+	# Determine if this resolution method is applicable.
+	def CanProcess(this):
+		return this.GetErrorType() in [parser.applicableError for parser in this.parsers]
+
+
+	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
+	def ParseInitialArgs(this):
+		super().ParseInitialArgs()
+		if ('error' in this.kwargs):
+			this.error = this.kwargs.pop('error')
+			# Just assume the error is an actual Exception object.
+		else:
+			raise ErrorResolutionError(f"{this.name} was not given an error to resolve.")
+
+		this.errorString = str(this.error)
+		this.errorType = this.GetErrorType()
+
+		# Internal member to avoid processing duplicates
+		this.errorResolutionStack = this.executor.errorResolutionStack
+
+
+	# Error resolution is unchained.
+	def PopulateNext(this):
+		this.next = []
+
+
+	# Override of Functor method.
+	# We'll keep calling this until an error is raised.
+	def Function(this):
+		this.functionSucceeded = True
+		this.errorShouldBeResolved = True
+		
+		if (not this.CanProcess()):
+			this.errorShouldBeResolved = False
+			return this.errorResolutionStack, this.errorShouldBeResolved
+
+		if (not this.errorString in this.errorResolutionStack.keys()):
+			this.errorResolutionStack.update({this.errorString:[]})
+		
+		if (this.name in this.errorResolutionStack[this.errorString]):
+			raise FailedErrorResolution(f"{this.name} already tried and failed to resolve {this.errorType}: {this.errorString}.")
+
+		this.GetObjectFromError()
+
+		try:
+			this.Resolve()
+		except Exception as e:
+			logging.error(f"Error resolution with {this.name} failed: {e}")
+			util.LogStack()
+			this.functionSucceeded = False
+		
+		this.errorResolutionStack[this.errorString].append(this.name)
+		return this.errorResolutionStack, this.errorShouldBeResolved
+
```

### Comparing `eons-2.5.7/pkg/eons/method/External.py` & `eons-2.5.8/pkg/eons/method/External.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.7/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-2.5.8/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.7/pkg/eons/resolve/resolve_import_module.py` & `eons-2.5.8/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.7/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-2.5.8/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.7/pkg/eons.egg-info/PKG-INFO` & `eons-2.5.8/pkg/eons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.5.7
+Version: 2.5.8
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.5.7/pkg/eons.egg-info/SOURCES.txt` & `eons-2.5.8/pkg/eons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eons-2.5.7/setup.cfg` & `eons-2.5.8/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 2.5.7
+version = 2.5.8
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -18,18 +18,18 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	pyyaml
-	requests
 	jsonpickle
+	requests
 	tqdm
+	pyyaml
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

