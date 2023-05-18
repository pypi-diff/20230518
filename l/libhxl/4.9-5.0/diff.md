# Comparing `tmp/libhxl-4.9.tar.gz` & `tmp/libhxl-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libhxl-4.9.tar", last modified: Fri Jun 29 14:07:55 2018, max compression
+gzip compressed data, was "libhxl-5.0.tar", last modified: Thu May 18 15:26:11 2023, max compression
```

## Comparing `libhxl-4.9.tar` & `libhxl-5.0.tar`

### file list

```diff
@@ -1,25 +1,33 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-06-29 14:07:55.000000 libhxl-4.9/
--rw-rw-r--   0 david     (1000) david     (1000)       28 2018-05-31 15:34:50.000000 libhxl-4.9/MANIFEST.in
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-06-29 14:07:55.000000 libhxl-4.9/hxl/
--rw-rw-r--   0 david     (1000) david     (1000)    61324 2018-06-05 23:32:24.000000 libhxl-4.9/hxl/validation.py
--rw-rw-r--   0 david     (1000) david     (1000)    30621 2018-06-29 14:04:15.000000 libhxl-4.9/hxl/io.py
--rw-rw-r--   0 david     (1000) david     (1000)    89899 2018-06-29 14:04:15.000000 libhxl-4.9/hxl/filters.py
--rw-rw-r--   0 david     (1000) david     (1000)     7365 2018-06-14 18:00:10.000000 libhxl-4.9/hxl/datatypes.py
--rw-rw-r--   0 david     (1000) david     (1000)    39332 2018-06-29 14:04:15.000000 libhxl-4.9/hxl/model.py
--rw-rw-r--   0 david     (1000) david     (1000)     6242 2018-05-02 15:51:22.000000 libhxl-4.9/hxl/converters.py
--rw-rw-r--   0 david     (1000) david     (1000)     1983 2018-05-31 13:01:57.000000 libhxl-4.9/hxl/hxl-default-schema.json
--rw-rw-r--   0 david     (1000) david     (1000)     4561 2018-03-29 19:42:28.000000 libhxl-4.9/hxl/geo.py
--rw-rw-r--   0 david     (1000) david     (1000)     2899 2018-06-29 14:04:15.000000 libhxl-4.9/hxl/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    27370 2018-05-02 15:51:22.000000 libhxl-4.9/hxl/scripts.py
--rw-rw-r--   0 david     (1000) david     (1000)     7410 2018-05-02 15:51:22.000000 libhxl-4.9/README.md
--rw-rw-r--   0 david     (1000) david     (1000)      267 2018-06-29 14:07:55.000000 libhxl-4.9/PKG-INFO
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-06-29 14:07:55.000000 libhxl-4.9/libhxl.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)      467 2018-06-29 14:07:55.000000 libhxl-4.9/libhxl.egg-info/entry_points.txt
--rw-rw-r--   0 david     (1000) david     (1000)      398 2018-06-29 14:07:55.000000 libhxl-4.9/libhxl.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)      267 2018-06-29 14:07:55.000000 libhxl-4.9/libhxl.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)        4 2018-06-29 14:07:55.000000 libhxl-4.9/libhxl.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)       47 2015-10-13 15:28:48.000000 libhxl-4.9/libhxl.egg-info/pbr.json
--rw-rw-r--   0 david     (1000) david     (1000)       70 2018-06-29 14:07:55.000000 libhxl-4.9/libhxl.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2018-06-29 14:07:55.000000 libhxl-4.9/libhxl.egg-info/dependency_links.txt
--rwxrwxr-x   0 david     (1000) david     (1000)     1380 2018-06-29 14:04:15.000000 libhxl-4.9/setup.py
--rw-rw-r--   0 david     (1000) david     (1000)       38 2018-06-29 14:07:55.000000 libhxl-4.9/setup.cfg
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-18 15:26:11.104760 libhxl-5.0/
+-rw-rw-r--   0 david     (1001) david     (1001)     1210 2022-10-28 23:20:29.000000 libhxl-5.0/LICENSE.md
+-rw-rw-r--   0 david     (1001) david     (1001)       28 2022-10-28 23:20:29.000000 libhxl-5.0/MANIFEST.in
+-rw-rw-r--   0 david     (1001) david     (1001)     6393 2023-05-18 15:26:11.104760 libhxl-5.0/PKG-INFO
+-rw-rw-r--   0 david     (1001) david     (1001)     6000 2022-10-28 23:20:29.000000 libhxl-5.0/README.md
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-18 15:26:11.100760 libhxl-5.0/hxl/
+-rw-rw-r--   0 david     (1001) david     (1001)     3639 2023-05-18 15:24:53.000000 libhxl-5.0/hxl/__init__.py
+-rw-rw-r--   0 david     (1001) david     (1001)     6595 2022-10-28 23:20:29.000000 libhxl-5.0/hxl/converters.py
+-rw-rw-r--   0 david     (1001) david     (1001)    13116 2022-10-28 23:20:29.000000 libhxl-5.0/hxl/datatypes.py
+-rw-rw-r--   0 david     (1001) david     (1001)   105695 2023-03-10 15:48:58.000000 libhxl-5.0/hxl/filters.py
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-18 15:26:11.104760 libhxl-5.0/hxl/formulas/
+-rw-rw-r--   0 david     (1001) david     (1001)        0 2022-10-28 23:20:29.000000 libhxl-5.0/hxl/formulas/__init__.py
+-rw-rw-r--   0 david     (1001) david     (1001)      703 2022-11-25 16:01:58.000000 libhxl-5.0/hxl/formulas/eval.py
+-rw-rw-r--   0 david     (1001) david     (1001)    12797 2022-11-25 16:01:58.000000 libhxl-5.0/hxl/formulas/functions.py
+-rw-rw-r--   0 david     (1001) david     (1001)     1010 2022-11-25 16:01:58.000000 libhxl-5.0/hxl/formulas/lexer.py
+-rw-rw-r--   0 david     (1001) david     (1001)     1820 2022-11-25 16:01:58.000000 libhxl-5.0/hxl/formulas/parser.py
+-rw-rw-r--   0 david     (1001) david     (1001)     3919 2022-10-28 23:20:50.000000 libhxl-5.0/hxl/formulas/parsetab.py
+-rw-rw-r--   0 david     (1001) david     (1001)     5788 2022-10-28 23:20:29.000000 libhxl-5.0/hxl/geo.py
+-rw-rw-r--   0 david     (1001) david     (1001)     1983 2022-10-28 23:20:29.000000 libhxl-5.0/hxl/hxl-default-schema.json
+-rw-rw-r--   0 david     (1001) david     (1001)    67144 2023-05-18 15:23:18.000000 libhxl-5.0/hxl/input.py
+-rw-rw-r--   0 david     (1001) david     (1001)    51976 2023-03-10 15:35:47.000000 libhxl-5.0/hxl/model.py
+-rw-rw-r--   0 david     (1001) david     (1001)    79626 2023-05-18 15:23:18.000000 libhxl-5.0/hxl/scripts.py
+-rw-rw-r--   0 david     (1001) david     (1001)      605 2022-11-25 16:01:58.000000 libhxl-5.0/hxl/util.py
+-rw-rw-r--   0 david     (1001) david     (1001)    62582 2022-10-28 23:20:29.000000 libhxl-5.0/hxl/validation.py
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-18 15:26:11.104760 libhxl-5.0/libhxl.egg-info/
+-rw-rw-r--   0 david     (1001) david     (1001)     6393 2023-05-18 15:26:11.000000 libhxl-5.0/libhxl.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1001) david     (1001)      541 2023-05-18 15:26:11.000000 libhxl-5.0/libhxl.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1001) david     (1001)        1 2023-05-18 15:26:11.000000 libhxl-5.0/libhxl.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1001) david     (1001)      663 2023-05-18 15:26:11.000000 libhxl-5.0/libhxl.egg-info/entry_points.txt
+-rw-rw-r--   0 david     (1001) david     (1001)      153 2023-05-18 15:26:11.000000 libhxl-5.0/libhxl.egg-info/requires.txt
+-rw-rw-r--   0 david     (1001) david     (1001)        4 2023-05-18 15:26:11.000000 libhxl-5.0/libhxl.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1001) david     (1001)       38 2023-05-18 15:26:11.104760 libhxl-5.0/setup.cfg
+-rwxrwxr-x   0 david     (1001) david     (1001)     2134 2023-05-18 15:24:53.000000 libhxl-5.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `libhxl-4.9/hxl/validation.py` & `libhxl-5.0/hxl/validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """Validation code for the Humanitarian Exchange Language (HXL) v1.0
 David Megginson
 Started October 2014
 
 License: Public Domain
 Documentation: https://github.com/HXLStandard/libhxl-python/wiki
 
-A \L{Schema} is the top-level class for validating a HXL dataset. The
+A Schema is the top-level class for validating a HXL dataset. The
 easiest way to create a schema is via the hxl.schema() method. The
 validate() function validates a dataset. Here is a simple validation
 example:
 
     def callback(e):
         print("Validation error:", e.message)
 
     source = hxl.data(data_url)
     if not hxl.schema(schema_url, callback=callback).validate(source):
         print('Validation failed')
 
-Each schema contains one or more \L{SchemaRule} objects.
+Each schema contains one or more SchemaRule objects.
 
 Each schema rule contains one or more objects implementing
-\L{AbstractRuleTest}. To add a new test, create a class extending
+AbstractRuleTest. To add a new test, create a class extending
 AbstractRuleTest, override the methods you need (validate_cell() is
 the most common), then add code to Schema.parse() method to parse and
 create your new test from the HXL schema.
 
 Validation tests go through the following workflow:
 
 - needs_scan() to check if the test needs multiple passes
 - start()
-- scan_row(\L{hxl.model.Row}) for each row in the dataset (only if needs_scan() returned True)
-- scan_cell(value, \L{hxl.model.Row}, L\{hxl.model.Column}) for each non-empty cell in each row (only if needs_scan() returned True)
+- scan_row(hxl.model.Row) for each row in the dataset (only if needs_scan() returned True)
+- scan_cell(value, hxl.model.Row, hxl.model.Column) for each non-empty cell in each row (only if needs_scan() returned True)
 - end_scan() (only if needs_scan() returned True)
-- validate_dataset(\L{hxl.model.Dataset})
-- validate_row(\L{hxl.model.Row}) for each row (row-level validations only)
-- validate_cell(value, \L{hxl.model.Row}, \L{hxl.model.Column}) for each cell in each row
+- validate_dataset(hxl.model.Dataset)
+- validate_row(hxl.model.Row) for each row (row-level validations only)
+- validate_cell(value, hxl.model.Row, hxl.model.Column) for each cell in each row
 - end()
 
 Any failure means that the entire test, rule, and schema fail
 validation, though error reporting will continue to the end.
 """
 
 import hxl
@@ -47,44 +47,46 @@
 logger = logging.getLogger(__name__)
 
 
 class HXLValidationException(hxl.HXLException):
     """Data structure to hold a HXL validation error.
 
     Normally, this exception isn't thrown, but is passed as a
-    parameter to callbacks via \L{Schema}, \L{SchemaRule}, and classes
-    extending \L{AbstractRuleTest}.
+    parameter to callbacks via Schema, SchemaRule, and classes
+    extending AbstractRuleTest.
     """
 
     SCOPES = ('dataset', 'column', 'row', 'cell',)
     """Allowed values for the error scope"""
 
-    def __init__(self, message, rule=None, value=None, row=None, column=None, suggested_value=None, scope='cell'):
+    def __init__(self, message, rule=None, value=None, row=None, column=None, suggested_value=None, scope='cell', is_external=False):
         """Construct a new validation error report.
         @param message: the text message for the error
         @param rule: the rule associated with the error (it may have a more-general descriptive message)
         @param value: the value that triggered the error, if available
-        @param row: the \L{hxl.model.Row} object associated with the error, if any
-        @param column: the \L{hxl.model.Column} object associated with the error, if any
+        @param row: the hxl.model.Row object associated with the error, if any
+        @param column: the hxl.model.Column object associated with the error, if any
         @param suggested_value: the suggested replacement value, if known
         @param scope: the error scope (dataset, column, row, or cell)
+        @param is_external: if True, the error is external to the data itself
         """
         super().__init__(message)
         
         self.rule = rule
         self.value = value
         self.row = row
         self.column = column
         self.suggested_value = suggested_value
+        self.is_external = is_external
 
         scope = hxl.datatypes.normalise_string(scope)
         if scope in HXLValidationException.SCOPES:
             self.scope = scope
         else:
-            raise HXLException("Unrecognised validation-error scope: {}".format(scope))
+            raise hxl.HXLException("Unrecognised validation-error scope: {}".format(scope))
 
     def __str__(self):
         """Get a string rendition of this error."""
         s = '<HXLValidationException '
         if self.message:
             s += self.message + ' '
         if self.rule:
@@ -93,22 +95,23 @@
                     s += '{}={} '.format(str(self.rule.tag_pattern), str(self.value))
                 else:
                     s += '{} '.format(str(self.rule.tag_pattern))
             if self.message:
                 s += '- {}'.format(self.message)
         return s
 
+
 #
 # Individual tests within a Schema Rule
 #
 
 class AbstractRuleTest(object):
     """Base class for a single test inside a validation rule.
 
-    Workflow (triggered by \L{SchemaRule}):
+    Workflow (triggered by SchemaRule):
 
     - needs_scan()
     - start()
     - scan_row() for each row (only if needs_scan() returned True)
     - scan_cell() for each non-empty matching cell (only if needs_scan() returned True)
     - end_scan() (only if needs_scan() returned True)
     - validate_dataset()
@@ -144,15 +147,15 @@
         """Setup code to run before validating each dataset.
         This code should not report errors, since it hasn't seen the data yet.
         """
         return True
 
     def end(self):
         """Code to run after validating each dataset.
-        Will report errors via the test's \I{callback}, if available.
+        Will report errors via the test's callback, if available.
         @returns: True if there are no new validation errors
         """
         return True
 
     def scan_row(self, row, indices=None, tag_pattern=None):
         """Scan a row of the dataset to collect information.
 
@@ -191,62 +194,63 @@
         """
         return
 
     def validate_dataset(self, dataset, indices=None, tag_pattern=None):
 
         """Apply test at the dataset level
         Called before validate_row() or validate_value()
-        Will report errors via the test's \I{callback}, if available.
+        Will report errors via the test's callback, if available.
         @param dataset: a hxl.model.Dataset object to validate
         @param indices: optional pre-compiled indices for columns matching tag_pattern
         @returns: True if there are no new validation errors.
         """
         return True
 
     def validate_row(self, row, indices=None, tag_pattern=None):
         """Apply test at the row level
         Called for each row before validate_cell() calls.
-        Will report errors via the test's \I{callback}, if available.
+        Will report errors via the test's callback, if available.
         @param row: a hxl.model.Row object to validate
         @param indices: optional pre-compiled indices for columns matching tag_pattern
         @returns: True if there are no new validation errors.
         """
         return True
 
     def validate_cell(self, value, row, column):
         """Apply test at the cell level
         Called for each matching non-empty value.
-        Will also report errors via the test's \I{callback}, if available.
+        Will also report errors via the test's callback, if available.
         @param value: the non-empty value to validate
         @param row: a hxl.model.Row object for location
         @param column: a hxl.model.Column object for location
         @returns: True if there are no new validation errors.
         """
         return True
 
     def get_indices(self, indices, tag_pattern, columns):
         """Get a set of column indices by hook or by crook, based on what we have"""
         if indices is not None:
             return indices
         elif tag_pattern is not None:
             tag_pattern = hxl.model.TagPattern.parse(tag_pattern)
-            return get_column_indices(tag_pattern, columns)
+            return hxl.model.get_column_indices([tag_pattern], columns)
         else:
-            raise HXLException("Internal error: rule test requires a tag pattern or a list of indices")
+            raise hxl.HXLException("Internal error: rule test requires a tag pattern or a list of indices")
 
     def report_error(self, message, row=None, column=None, value=None, suggested_value=None, scope='cell'):
         """Report an error from this test, if there is a callback function available."""
         if self.callback:
             self.callback(HXLValidationException(
                 message,
                 value=value,
                 row=row,
                 column=column,
                 suggested_value=suggested_value,
-                scope=scope
+                scope=scope,
+                is_external=False
             ))
         return False # for convenience
 
 
 class RequiredTest(AbstractRuleTest):
     """Test min/max occurrence
     HXL schema: #valid_required
@@ -317,15 +321,15 @@
 
         return status
 
     
 class DatatypeTest(AbstractRuleTest):
     """Test for a specified datatype
     HXL schema: #valid_datatype-consistent
-    See also \L{ConsistentDatatypeTest}, which infers the most-common datatype.
+    See also ConsistentDatatypeTest, which infers the most-common datatype.
     """
 
     # allowed datatypes
     DATATYPES = ('text', 'number', 'url', 'email', 'phone', 'date',)
 
     def __init__(self, datatype):
         """Constructor
@@ -390,26 +394,33 @@
             self.min_value = None
         if max_value is not None:
             self.max_value = hxl.datatypes.normalise_string(max_value)
         else:
             self.max_value = None
 
         # precompile numbers and dates for efficiency
-        self.min_num = None
-        self.max_num = None
-        self.min_date = None
-        self.max_date = None
-        if hxl.datatypes.is_number(min_value):
+        try:
             self.min_num = hxl.datatypes.normalise_number(min_value)
-        if hxl.datatypes.is_number(max_value):
+        except ValueError:
+            self.min_num = None
+
+        try:
             self.max_num = hxl.datatypes.normalise_number(max_value)
-        if hxl.datatypes.is_date(min_value):
+        except ValueError:
+            self.max_num = None
+
+        try:
             self.min_date = hxl.datatypes.normalise_date(min_value)
-        if hxl.datatypes.is_date(max_value):
+        except ValueError:
+            self.min_date = None
+
+        try:
             self.max_date = hxl.datatypes.normalise_date(max_value)
+        except ValueError:
+            self.max_date = None
 
     def validate_cell(self, value, row, column):
         """Test that a value is >= min_value and/or <= max_value
         Includes special handling for numbers and dates.
         """
         def report(message):
             return self.report_error(
@@ -655,14 +666,15 @@
         """
         super().__init__()
         self.tag_patterns = hxl.model.TagPattern.parse_list(tag_patterns)
 
     def start(self):
         """Build an empty correlation map"""
         self.correlation_map = dict()
+        self.correlation_indices = None
 
     def end(self):
         """All the error reporting happens here.
         We don't know the most-common correlations for each key until the end.
         Use the most-common value for each correlation key as the suggested
         value for the others.
         """
@@ -692,18 +704,23 @@
 
     def validate_row(self, row, indices=None, tag_pattern=None):
         """Row validation always succeeds
         We use this method to capture the correlation keys,
         so that we can report on them in the end() method.
         """
 
+        # will cache, so that we don't repeat the calculation
         indices = self.get_indices(indices, tag_pattern, row.columns)
 
+        # calculate the correlation-column indices only once as well
+        if self.correlation_indices is None:
+            self.correlation_indices = hxl.model.get_column_indices(self.tag_patterns, row.columns)
+
         # Make the correlation key
-        key = row.key(self.tag_patterns)
+        key = row.key(indices=self.correlation_indices)
 
         # Record the locations
         # key -> value -> location
         for i in indices:
             tagspec = row.columns[i].get_display_tag(sort_attributes=True)
             if i < len(row.values) and not hxl.datatypes.is_empty(row.values[i]):
                 value = row.values[i]
@@ -930,15 +947,18 @@
             # now calculate the standard deviation of the remaining values
             self.mean_values[tagspec] = sum(values) / len(values)
             self.standard_deviations[tagspec] = math.sqrt(
                 sum(map(lambda n: (n-self.mean_values[tagspec])*(n-self.mean_values[tagspec]), values)) / len(values)
             )
 
             # calculate the coefficient of variance, which we'll use as a cutoff
-            self.variation_coefficients[tagspec] = self.standard_deviations[tagspec] / self.mean_values[tagspec]
+            if self.mean_values[tagspec]:
+                self.variation_coefficients[tagspec] = self.standard_deviations[tagspec] / self.mean_values[tagspec]
+            else:
+                self.variation_coefficients[tagspec] = 0
 
         # free some memory
         del self.values
 
     def validate_cell(self, value, row, column):
         tagspec = column.get_display_tag(sort_attributes=True) # FIXME
 
@@ -970,15 +990,15 @@
 
 class SchemaRule(object):
     """A single rule within a schema.
     A rule contains one or more tests, together with some common metadata
     (a tag pattern, severity level, and description). If any test fails, then
     the whole rule fails.
 
-    Workflow (triggered by \L{Schema.validate}:
+    Workflow (triggered by Schema.validate:
 
     - needs_scan()
     - start()
     - scan_row() for each row (if needs_scan() returned True)
     - scan_cell() for each maching non-empty cell (if needs_scan() returned True)
     - end_scan() (if needs_scan() returned True)
     - validate_dataset()
@@ -1001,22 +1021,22 @@
         self.callback = callback
 
         # make sure the severity level is valid
         severity = hxl.datatypes.normalise_string(severity)
         if severity in SchemaRule.SEVERITY:
             self.severity = severity
         else:
-            raise HXLException("Unsupported rule severity level: {}".format(severity))
+            raise hxl.HXLException("Unsupported rule severity level: {}".format(severity))
 
         # Additional internal variables
         self.tests = []
-        """List of \L{AbstractRuleTest} objects to apply as part of this rule"""
+        """List of AbstractRuleTest objects to apply as part of this rule"""
 
-        self.loading_errors = []
-        """Errors setting up the rule, to be reported once during each run."""
+        self.external_errors = []
+        """Errors external to the dataset itself (e.g. missing taxonomies)"""
 
         self.saved_indices = None
         """List of saved column indices matching tag_pattern"""
 
     def needs_scan(self):
         """Check if any test in this rule requires a pre-scan of the dataset.
         @returns: True if at least one test's needs_scan() method returns True
@@ -1060,15 +1080,15 @@
         """Pre-scan a row and its individual cells.
         This method does not report errors or return a status.
         Will be invoked only if needs_scan() returned True
         Calls both scan_row() and scan_cell() for each test.
         @param row the Row to scan
         """
         if self.saved_indices is None:
-            self.saved_indices = get_column_indices(self.tag_pattern, row.columns)
+            self.saved_indices = hxl.model.get_column_indices([self.tag_pattern], row.columns)
 
         # scan each row, then each matching cell in the row
         for test in self.tests:
             if not test.needs_scan(): # don't invoke unless the test asked for it
                 continue
             test.scan_row(row, self.saved_indices)
             for i in self.saved_indices: # validate individual cells
@@ -1082,19 +1102,18 @@
                 test.end_scan()
                     
     def validate_dataset(self, dataset, indices=None, tag_pattern=None):
         """Test whether the columns are present to satisfy this rule."""
         
         status = True
         if self.saved_indices is None:
-            self.saved_indices = get_column_indices(self.tag_pattern, dataset.columns)
+            self.saved_indices = hxl.model.get_column_indices([self.tag_pattern], dataset.columns)
 
-        # Report any loading errors
-        for error in self.loading_errors:
-            status = False
+        # Report any external errors
+        for error in self.external_errors:
             if self.callback:
                 self.callback(error)
 
         # run each of the tests
         for test in self.tests:
             if not test.validate_dataset(dataset, indices=self.saved_indices):
                 status = False
@@ -1107,15 +1126,15 @@
         @param row the Row to validate
         @return True if all matching values in the row are valid
         """
 
         # individual rules may change to False
         status = True
         if self.saved_indices is None:
-            self.saved_indices = get_column_indices(self.tag_pattern, row.columns)
+            self.saved_indices = hxl.model.get_column_indices([self.tag_pattern], row.columns)
 
         # run each test on the complete row, then on individual cells
         for test in self.tests:
             if not test.validate_row(row, self.saved_indices):
                 status = False
             for i in self.saved_indices: # validate individual cells
                 if i < len(row.values) and not hxl.datatypes.is_empty(row.values[i]):
@@ -1144,25 +1163,25 @@
     Add new rules with
 
         schema.rules.append(rule)
     """
 
     def __init__(self, callback=None):
         """Constructor
-        @param callback: a callback function to receive \L{HXLValidationException} objects as error reports
+        @param callback: a callback function to receive HXLValidationException objects as error reports
         """
         self.rules = []
         """Rules making up this schema"""
         
         self.callback = callback
         """Callback function to receive error reports"""
 
     def validate(self, source):
         """Execute the main validation workflow.
-        @param source: the \L{hxl.model.Dataset} to validate
+        @param source: the hxl.model.Dataset to validate
         """
         status = True # all is well at the beginning
         needs_scan = False # assume we don't need a pre-scan
 
         # do we need a cached, in-memory dataset?
         for rule in self.rules:
             if rule.needs_scan():
@@ -1226,15 +1245,15 @@
         """End pre-scan, for rules that require it."""
         for rule in self.rules:
             if rule.needs_scan():
                 rule.end_scan()
 
     def validate_dataset(self, dataset):
         """Validate just at the dataset level
-        @param dataset: the \L{hxl.model.Dataset} object to validate
+        @param dataset: the hxl.model.Dataset object to validate
         """
         status = True
         for rule in self.rules:
             if not rule.validate_dataset(dataset):
                 status = False
         return status
 
@@ -1266,15 +1285,15 @@
         """
 
         # Catch special cases
 
         if source is None:
             # Use the built-in default schema and recurse
             path = os.path.join(os.path.dirname(__file__), 'hxl-default-schema.json');
-            with hxl.data(path, True) as source:
+            with hxl.data(path, hxl.InputOptions(allow_local=True)) as source:
                 return Schema.parse(source, callback)
 
         if isinstance(source, Schema):
             # Already a schema; set the callback and return it
             source.callback = callback
             return source
 
@@ -1388,43 +1407,33 @@
                         target_tag = row.get('#valid_value+target_tag', default=tag_pattern)
                         try:
                             # read the values from an external dataset
                             source = hxl.data(url)
                             allowed_values = source.get_value_set(row.get('#valid_value+target_tag'))
                             if len(allowed_values) > 0:
                                 rule.tests.append(EnumerationTest(allowed_values, case_sensitive))
-                        except Exception as error:
-                            rule.loading_errors.append(HXLValidationException(
-                                'Error loading allowed values from {}: {}'.format(url, str(error)),
+                        except BaseException as error:
+                            # don't add the test to the rule
+                            # do add an error about loading the values
+                            rule.external_errors.append(HXLValidationException(
+                                'Error loading allowed values from {}: {}'.format(url, error.args[0]),
                                 scope='dataset',
-                                rule=rule
+                                rule=rule,
+                                is_external=True
                             ))
 
 
                     schema.rules.append(rule)
 
         return schema
 
 #
 # Internal helper functions
 #
 
-def get_column_indices(tag_pattern, columns):
-    """Return a list of column indices matching tag_pattern
-    @param tag_pattern: the hxl.model.TagPattern to test
-    @param columns: a sequence of hxl.model.Column objects to test
-    @returns: a possibly-empty sequence of integer indices into columns
-    """
-    indices = []
-    for i, column in enumerate(columns):
-        if tag_pattern.match(column):
-            indices.append(i)
-    return indices
-
-
 def find_closest_match(s, allowed_values):
     """Find the closest match for a value from a list.
     This is not super efficient right now; look at
     https://en.wikipedia.org/wiki/Edit_distance for better algorithms.
     Uses a cutoff of len(s)/3 for candidate matches, and if two matches have the same 
     edit distance, prefers the one with the longer common prefix.
     @param s: the misspelled string to check
@@ -1497,60 +1506,67 @@
     """Convenience function for validating HXL data.
     The is_valid parameter in the report will be a True/False value for the result.
 
     If you want to do anything tricky, you can pass pre-cooked hxl.data() parameters in, e.g.
 
     result = hxl.validate(hxl.data('foo.csv', allow_local=True), hxl.data('schema.csv', allow_local=True))
 
-    @param data: the data to validate (a URL or anything else accepted by \L{hxl.data})
+    @param data: the data to validate (a URL or anything else accepted by hxl.data)
     @param schema: the schema to validate against (anything accepted by L{hxl.data}), or None (default) to use the built-in schema.
     @returns: a JSON validation report as documented at https://github.com/HXLStandard/hxl-proxy/wiki/Validation-reports
     """
 
     issue_map = dict()
+    external_issue_map = dict()
 
     def add_issue(issue):
         hash = make_rule_hash(issue.rule)
-        issue_map.setdefault(hash, []).append(issue)
+        if issue.is_external:
+            external_issue_map.setdefault(hash, []).append(issue)
+        else:
+            issue_map.setdefault(hash, []).append(issue)
 
     status = hxl.schema(schema, callback=add_issue).validate(hxl.data(data))
 
     schema_url = None
     data_url = None
     if hxl.datatypes.is_string(schema):
         schema_url = schema
     if hxl.datatypes.is_string(data):
         data_url = data
 
-    return make_json_report(status, issue_map, schema_url=schema_url, data_url=data_url)
+    return make_json_report(status, issue_map, external_issue_map, schema_url=schema_url, data_url=data_url)
 
 
 #
 # Local functions
 #
 
-def make_json_report(status, issue_map, schema_url=None, data_url=None):
+def make_json_report(status, issue_map, external_issue_map, schema_url=None, data_url=None):
     """Generate a JSON error report from a dict of errors
     @param status: the validation status (boolean)
-    @param issue_map: a dict of lists of \L{HXLValidationException} objects grouped by rule hash
+    @param issue_map: a dict of lists of HXLValidationException objects grouped by rule hash
+    @param external_issue_map: a dict of lists of HXLValidationException objects grouped by rule hash
     @param data_url: the original URL of the data, if available
     @param schema_url: the original URL of the schema, if available
     """
 
     json_report = {
         "validator": "libhxl-python",
         "timestamp": datetime.datetime.now().isoformat(),
         "is_valid": status,
         "stats": {
             "info": 0,
             "warning": 0,
             "error": 0,
-            "total": 0
+            "external": 0,
+            "total": 0,
         },
         "issues": [],
+        "external_issues": [],
     }
 
     if schema_url is not None:
         json_report['schema_url'] = schema_url
         
     if data_url is not None:
         json_report['data_url'] = data_url
@@ -1558,49 +1574,62 @@
     # add the issue objects
     for rule_id, locations in issue_map.items():
         json_issue = make_json_issue(rule_id, locations)
         json_report['stats']['total'] += len(json_issue['locations'])
         json_report['stats'][locations[0].rule.severity] += len(json_issue['locations'])
         json_report['issues'].append(json_issue)
 
+    # add the external issue objects
+    for rule_id, locations in external_issue_map.items():
+        json_issue = make_json_issue(rule_id, locations, is_external=True)
+        json_report['stats']['total'] += 1
+        json_report['stats']['external'] += 1
+        json_report['external_issues'].append(json_issue)
+
     return json_report
 
-def make_json_issue(rule_id, locations):
+def make_json_issue(rule_id, locations, is_external=False):
     """Create an issue (with list of locations) for a JSON validation report
     @param rule_id: the hash for the rule (used to group locations)
-    @param locations: a list of \L{HXLValidation"""
+    @param locations: a list of HXLValidation
+    """
 
     # grab first location as a model
     model = locations[0]
 
     # get a custom description first, then the generic message as a fallback
     description = model.rule.description
     if not description:
         description = model.message
 
-    # get all unique locations
-    location_keys = set()
-    json_locations = []
-    for location in locations:
-        location_key = (location.row.row_number, location.column.column_number, location.value, location.suggested_value,)
-        if not location_key in location_keys:
-            json_locations.append(make_json_location(location))
-            location_keys.add(location_key)
-
     # make the issue
     json_issue = {
         "rule_id": rule_id,
         "tag_pattern": str(model.rule.tag_pattern),
         "description": description,
         "severity": model.rule.severity,
-        "location_count": len(locations),
         "scope": model.scope,
-        "locations": json_locations
     }
 
+    # get all unique locations
+    if is_external:
+        json_issue["description"] = model.message
+    else:
+        location_keys = set()
+        json_locations = []
+        for location in locations:
+            row_number = location.row.row_number if location.row else None
+            column_number = location.column.column_number if location.column else None
+            location_key = (row_number, column_number, location.value, location.suggested_value,)
+            if not location_key in location_keys:
+                json_locations.append(make_json_location(location))
+                location_keys.add(location_key)
+        json_issue["location_count"] = len(locations)
+        json_issue["locations"] = json_locations
+
     return json_issue
 
 def make_json_location(location):
     """Create a single location for a JSON validation report"""
     json_location = {}
 
     # is there a row object?
```

### Comparing `libhxl-4.9/hxl/filters.py` & `libhxl-5.0/hxl/filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,17 +33,18 @@
 @organization: UNOCHA
 @license: Public Domain
 @date: Started October 2014
 @see: U{hxlstandard.org}
 
 """
 
-import hxl
-import abc, copy, dateutil.parser, json, jsonpath_rw, logging, re, six, sys
+import hxl, hxl.formulas.eval as feval
+import abc, copy, dateutil.parser, itertools, json, jsonpath_ng.ext, logging, re, six, sys
 
+from hxl.util import logup
 
 logger = logging.getLogger(__name__)
 
 
 class HXLFilterException(hxl.HXLException):
     """Base class for HXL filter exceptions.
 
@@ -70,15 +71,15 @@
     subclass L{AbstractStreamingFilter} or L{AbstractCachingFilter},
     both of which are child classes of this one; however, there may be
     some special applications where you need to subclass
     I{AbstractBaseFilter} directly (see L{AppendFilter} for an
     example).
 
     Subclassing works like this::
-    
+
       class MyFilter(hxl.filters.AbstractBaseFilter):
 
           def __init__(self, source):
               super(AbstractBaseFilter, self).__init__(source)
 
           def filter_columns(self):
               return [Column.parse('#org'), Column.parse('#adm1')]
@@ -175,15 +176,15 @@
         """Create an instance of the filter from a dict.
         Child classes must override this method.
         @param spec: the JSON-like spec to read
         @returns: a new filter object
         """
         raise NotImplementedError("No static _load method implemented.")
 
-    
+
 class AbstractStreamingFilter(AbstractBaseFilter):
     """Abstract base class for streaming filters.
 
     A streaming filter processes one row at a time.  It can skip rows,
     but it never reorders them.  As a result, a streaming filter is
     I{much} more efficient than a L{caching
     filter<AbstractCachingFilter>}, since it needs to hold only one
@@ -232,15 +233,15 @@
         """Filter a single row of data.
 
         By default, this method returns the row's values,
         unchanged. Subclasses can use it to replace, add or suppress
         rows on the fly, without having to keep a copy of the entire
         dataset in memory.
 
-        @param row: the original L{hxl.model.Row} object.  
+        @param row: the original L{hxl.model.Row} object.
         @returns: A list of string values (I{not} a Row object) or
         C{None} to skip the row.
         @see: L{AbstractBaseFilter.filter_columns}
 
         """
         return row.values
 
@@ -260,15 +261,15 @@
             self.source_iter = iter(self.outer.source) # iterator for the source data
             self.row_number = -1
 
         def __iter__(self):
             return self
 
         def __next__(self):
-            """Return the next filtered row of data.  
+            """Return the next filtered row of data.
 
             Uses the L{AbstractStreamingFilter.filter_row} method. The
             returned row is always a new object, so that if the client
             changes it, it won't change the version visible upstream
             in the filter chain.
 
             @returns: a L{hxl.model.Row} object
@@ -343,24 +344,24 @@
         """Test if the input is cached.
         @returns: always C{True} for caching filters
         """
         return True
 
     def filter_rows(self):
         """Filter all of the data together.
-        
+
         This method returns raw lists and strings, not objects from
         the L{hxl.model} module; for example, it could return the
         following for a three-row dataset::
 
           [['UNICEF', '20'], ['UNHCR', '15'], ['OXFAM', '25']]
 
         The I{AbstractCachingFilter} class will construct the
         appropriate objects around the data.
-        
+
         @returns: a list of lists of strings, one list for each row.
         @see: L{AbstractBaseFilter.filter_columns}
         """
         return self.source.values
 
     def __iter__(self):
         return AbstractCachingFilter._Iterator(self)
@@ -391,15 +392,15 @@
             if self.values_iter is None:
                 if self.outer._saved_rows is None:
                     # filter rows only once, when requested
                     self.outer._saved_rows = self.outer.filter_rows()
                 self.values_iter = iter(self.outer._saved_rows)
             self.row_number += 1
             return hxl.model.Row(self.outer.columns, next(self.values_iter), self.row_number)
-        
+
 
 #
 # Utility classes
 #
 class Aggregator(object):
     """Class for aggregating a single value vertically through a dataset
 .
@@ -425,55 +426,100 @@
             raise HXLFilterException('Pattern missing for {} aggregator'.format(type))
         if not column:
             column = '{type}#meta+{type}'.format(type=self.type)
         self.column = hxl.model.Column.parse_spec(column)
 
         self.total = 0
         """Total number of rows used."""
+
         self.value = None
         """Resulting aggregation value."""
 
+        self.normalised = None
+        """Normalised value to use for internal comparison"""
+
+        self.values = set()
+        """Unique values seen (for concat)"""
+
     def evaluate_row(self, row):
         """Evaluate a single row of HXL data against this aggregator.
         @param row: the input row to read
         @exception HXLFilterException: for an unrecognised aggregator type
         """
 
+        #
+        # Shortcut: just counting rows
+        #
         if self.type == 'count':
-            if self.value is None: self.value = 0
+            if self.value is None:
+                self.value = 0
             self.value += 1
             return
 
+        #
+        # Aggregating values
+        #
         value = row.get(self.pattern)
-        if value is not '' and value is not None:
-            try:
-                # try to force to a number for aggregation
-                n = float(value)
-                self.total += 1
-                if self.type == 'sum':
-                    if not self.value: self.value = 0
-                    self.value += n
-                elif self.type == 'average':
-                    if not self.value: self.value = 0
-                    self.value = ((self.value * (self.total - 1)) + n) / self.total
-                elif self.type == 'min':
-                    if self.value is None or self.value > n:
-                        self.value = n
-                elif self.type == 'max':
-                    if self.value is None or self.value < n:
-                        self.value = n
-                else:
-                    raise HXLFilterException("Bad aggregator type for count filter: {}".format(type))
-            except:
-                logger.error("Cannot use %s as a numeric value for aggregation; skipping.", value)
 
-    TAG_PATTERN = '#?{token}(?:\s*[+-]{token})*'.format(token=hxl.datatypes.TOKEN_PATTERN)
+        # Skip empty values
+        if hxl.datatypes.is_empty(value):
+            return
+
+        # Numbers only for sum and average
+        datatype = hxl.datatypes.typeof(value, self.pattern)
+        if self.type in ['sum', 'average'] and datatype != 'number':
+            logup("Cannot use as a numeric value for aggregation; skipping.", {"value": value}, level='info')
+            logger.warning("Cannot use %s as a numeric value for aggregation; skipping.", value)
+            return
+
+        normalised = hxl.datatypes.normalise(value, self.pattern)
+        self.total += 1
+
+        # aggregate as appropriate
+        # note that we track a separate normalised value for strings and dates
+        if self.type == 'sum':
+            if self.value is None:
+                self.value = 0
+            self.value += normalised
+        elif self.type == 'average':
+            if self.value is None:
+                self.value = 0
+            self.value = ((self.value * (self.total - 1)) + normalised) / self.total
+        elif self.type == 'min':
+            def gt(a, b):
+                try:
+                    return a > b
+                except TypeError:
+                    return str(a) > str(b)
+            if self.normalised is None or gt(self.normalised, normalised):
+                self.value = value
+                self.normalised = normalised
+        elif self.type == 'max':
+            def lt(a, b):
+                try:
+                    return a < b
+                except TypeError:
+                    return str(a) < str(b)
+            if self.normalised is None or lt(self.normalised, normalised):
+                self.value = value
+                self.normalised = normalised
+        elif self.type == 'concat':
+            if not hxl.datatypes.is_empty(value):
+                value = hxl.datatypes.normalise_space(value)
+                if value not in self.values:
+                    # regenerate the list if it's a new value
+                    self.values.add(value)
+                    self.value = "|".join(sorted(self.values))
+        else:
+            raise HXLFilterException("Bad aggregator type for count filter: {}".format(type))
+
+    TAG_PATTERN = r'#?{token}(?:\s*[+-]{token})*'.format(token=hxl.datatypes.TOKEN_PATTERN)
     """Regular expression for a tag pattern"""
-    
-    COL_PATTERN = '#{token}(?:\s*\+{token})*'.format(token=hxl.datatypes.TOKEN_PATTERN)
+
+    COL_PATTERN = r'#{token}(?:\s*\+{token})*'.format(token=hxl.datatypes.TOKEN_PATTERN)
     """Regular expression for an output column pattern"""
 
     AGGREGATOR_PATTERN = r'^\s*({token})\(({tag})?\)(?:\s*as\s+([^#]*)({col}))?$'.format(
         token = hxl.datatypes.TOKEN_PATTERN,
         tag = TAG_PATTERN,
         col = COL_PATTERN
     )
@@ -601,32 +647,35 @@
         """
         values = copy.copy(row.values)
         if self.before:
             return self._subst(row, self.const_values) + values
         else:
             return values + self._subst(row, self.const_values)
 
-    _SUBST_PATTERN = '{{(#' + hxl.datatypes.TOKEN_PATTERN + '(?:[+-]' + hxl.datatypes.TOKEN_PATTERN + ')*)}}';
+    _SUBST_PATTERN = r'{{(.+?)}}' # non-greedy expression
     """Regular expression to parse a substitution pattern in the fixed contents for the new cell"""
 
     def _subst(self, row, const_values):
         """Execute pattern substitutions for fixed values for the new columns.
         Substitutions are tag patterns inside double braces. Example: "X-{{#country+code}}"
         @param row: the row to search for matches to any patterns.
         @param const_values: the constant values to scan for patterns
         @returns: the constant values (only) with substitutions executed
         """
         def do_sub(match_object):
-            return row.get(match_object.group(1))
+            # FIXME don't want to reparse the formula for every row
+            # Need to pre-parse and pre-chunk the replacement string
+            result = feval.eval(row, match_object.group(1))
+            return str(result)
         values = []
         for value in const_values:
             values.append(re.sub(AddColumnsFilter._SUBST_PATTERN, do_sub, value))
         return values
 
-    SPEC_PATTERN = r'^\s*(?:([^#]*)#)?({token}(?:\s*\+{token})*)=(.*)\s*$'.format(token=hxl.datatypes.TOKEN_PATTERN)
+    SPEC_PATTERN = r'^\s*(?:([^#]*?)#)?({token}(?:\s*\+{token})*)=(.*)\s*$'.format(token=hxl.datatypes.TOKEN_PATTERN)
     """Pattern for a string specification for a new column"""
 
     @staticmethod
     def parse_spec(spec):
         """Parse a new-column specification.
 
         The format is I{<header text>}B{#}I{<tag and
@@ -663,15 +712,15 @@
 
 
 class AppendFilter(AbstractBaseFilter):
 
     """Composable filter class to concatenate two datasets.
 
     Usage::
-    
+
         filter = AppendFilter(hxl.data(url), hxl.data(url2))
 
     This filter concatenates a second dataset to the end of the first
     one. It supports the L{hxl.model.Dataset.append} convenience
     method, and the L{hxl.scripts.hxlappend} command-line script.
 
     The filter preserves the order of the columns in the first
@@ -738,15 +787,15 @@
         super(AppendFilter, self).__init__(source)
 
         # parameters
         if is_sourcey(append_sources):
             append_sources = [append_sources]
         self.append_sources = [hxl.data(src) for src in append_sources] # so that we can take a plain URL
         """The sources to append to this source"""
-        self.add_columns = add_columns
+        self.add_extra_columns = add_columns
         """If true, always add new columns instead of replacing existing ones"""
         self.queries = self._setup_queries(queries)
         """The row queries to limit where we choose append candidates"""
 
         # internal properties
         self._column_positions = []
         """Cache of column positions, to avoid rescanning on every pass"""
@@ -772,15 +821,15 @@
                     if column == original_column:
                         # yes, there is one; clear it, so it's not reused
                         self._column_positions[i][j] = k
                         columns_in[k] = None
                         break
                 if self._column_positions[i].get(j) is None:
                     # no -- we need to add a new column
-                    if self.add_columns:
+                    if self.add_extra_columns:
                         self._column_positions[i][j] = len(columns_out)
                         columns_out.append(copy.deepcopy(column))
                     else:
                         self._column_positions[i][j] = None
 
         # make an empty template for each row
         self._template_row = [''] * len(columns_out)
@@ -795,15 +844,15 @@
 
     class _Iterator:
         """Custom iterator to return the contents of all sources, in sequence."""
 
         def __init__(self, outer):
             """@param outer: reference to outer object"""
             self.outer = outer
-            
+
             self._iterator = iter(outer.source)
             self._column_map = {i: i for i in range(len(self.outer.source.columns))}
             self._is_source = True
 
             self._sources = list(self.outer.append_sources)
             self._column_positions = list(self.outer._column_positions)
 
@@ -839,23 +888,41 @@
                         self._sources = self._sources[1:]
                         self._column_positions = self._column_positions[1:]
                         self._is_source = False
                     else:
                         self._iterator = None
 
             raise StopIteration()
-        
+
+    @staticmethod
+    def parse_external_source_list(input):
+        append_sources = []
+        with hxl.data(input) as source:
+            for row in source:
+                append_source = row.get('#x_source')
+                if append_source:
+                    append_sources.append(append_source)
+        return append_sources
+
     @staticmethod
     def _load(source, spec):
         """Create an AppendFilter from a dict spec.
         @param spec: the string specification
         """
+
+        if spec.get('filter') == 'append_external_list':
+            append_sources = AppendFilter.parse_external_source_list(
+                hxl.data(req_arg(spec, 'source_list_url'))
+            )
+        else:
+            append_sources = req_arg(spec, 'append_sources')
+
         return AppendFilter(
             source=source,
-            append_sources=req_arg(spec, 'append_sources'),
+            append_sources=append_sources,
             add_columns=opt_arg(spec, 'add_columns', True),
             queries=opt_arg(spec, 'queries', [])
         )
 
 
 class CacheFilter(AbstractBaseFilter):
     """Composable filter to cache HXL data in memory.
@@ -974,15 +1041,15 @@
         example, it is impossible to guess whether "9/6/15" refers to
         6 September 2016 or 9 June 2016 (hence the need for ISO dates)
         -- but it will do its best.
       - B{number}: attempt to normalise numbers to standard computer
         format (remove commas or spaces between thousands, and use "."
         as the decimal separator).
       - B{latlon}: attempt to normalise latitude and longitude values.
-      
+
     For each type of cleaning, you specify one or more L{tag
     patterns<hxl.model.TagPattern>} to which the cleaning applies (you
     may use string representations instead of creating the objects),
     or use C{True} to apply the cleaning to the whole row. You may
     also include L{hxl.model.RowQuery} objects to apply the cleaning
     tasks only to specific rows. You can also specify a format for
     normalised dates or numbers, and choose to purge any dates,
@@ -1035,56 +1102,90 @@
         self.date_format = date_format
         self.number = hxl.model.TagPattern.parse_list(number)
         self.number_format = number_format
         self.latlon = hxl.model.TagPattern.parse_list(latlon)
         self.purge = purge
         self.queries = self._setup_queries(queries)
 
+        # We need to prescan for dates
+        if date:
+            self.source = self.source.cache();
+            self.date_dayfirst = self._guess_dayfirst()
+
     def filter_row(self, row):
         """@returns: cleaned row data"""
         if hxl.model.RowQuery.match_list(row, self.queries):
             # if there are no queries, or row matches at least one
             columns = self.columns
             values = copy.copy(row.values)
             for i in range(min(len(values), len(columns))):
                 values[i] = self._clean_value(values[i], columns[i])
             return values
         else:
             # otherwise, leave as-is
             return row.values
 
+    def _guess_dayfirst(self):
+        """Guess whether the default should be DD-MM-YYYY or MM-DD-YYYY
+        @returns: true if we should default to dayfirst format
+        """
+        ddmm_count = 0
+        mmdd_count = 0
+
+        # prescan columns to speed things up
+        indices = []
+        for i, column in enumerate(self.source.columns):
+            if hxl.TagPattern.match_list(column, self.date):
+                indices.append(i)
+
+        # if there are any matching columns, then prescan values
+        if indices:
+            for row in self.source:
+                for i in indices:
+                    value = row.values[i]
+                    if value:
+                        result = re.match(r'^[^\d]*(\d\d?)[^\d]+(\d\d?)[^\d].*$', hxl.datatypes.normalise_string(value))
+                        if result:
+                            if int(result.group(1)) > 12:
+                                ddmm_count += 1
+                            elif int(result.group(2)) > 12:
+                                mmdd_count += 1
+
+        return (ddmm_count >= mmdd_count)
+
+
     def _clean_value(self, value, column):
         """Clean a single value, using the column def for guidance.
         @returns: a single cleaned value
         """
         value = str(value)
 
         # Whitespace (-w)
         if self._match_patterns(self.whitespace, column):
-            value = re.sub('^\s+', '', value)
-            value = re.sub('\s+$', '', value)
-            value = re.sub('\s+', ' ', value)
+            value = re.sub(r'^\s+', '', value)
+            value = re.sub(r'\s+$', '', value)
+            value = re.sub(r'\s+', ' ', value)
 
         # Uppercase (-u)
         if self._match_patterns(self.upper, column):
             value = value.upper()
 
         # Lowercase (-l)
         if self._match_patterns(self.lower, column):
             value = value.lower()
 
         # Date
         if self._match_patterns(self.date, column):
             if value:
-                if hxl.datatypes.is_date(value):
+                try:
+                    value = hxl.datatypes.normalise_date(value, self.date_dayfirst)
                     if self.date_format is not None:
                         value = dateutil.parser.parse(value).strftime(self.date_format)
-                    else:
-                        value = hxl.datatypes.normalise_date(value)
-                else:
+                except ValueError:
+                    logup("Cannot use as a date", {"value": value}, level='info')
                     logger.warning('Cannot parse %s as a date', str(value))
                     if self.purge:
                         value = ''
 
         # Number
         if self._match_patterns(self.number, column):
 
@@ -1100,50 +1201,54 @@
                 except:
                     return None
 
                 # fixme - get much smarter about numbers
             if value:
                 n = try_number(value)
                 if n is None:
-                    s = re.sub('[^\de.]+', '', value)
+                    s = re.sub(r'[^\de.]+', '', value)
                     n = try_number(s) # OK, try again
                 if n is not None:
                     value = n
                 else:
-                    logger.warning('Cannot parse {} as a number', str(value))
+                    logup('Cannot parse as a number', {"value": value}, level='info')
+                    logger.warning('Cannot parse %s as a number', str(value))
                     if self.purge:
                         value = ''
 
         # Latlon
         if self._match_patterns(self.latlon, column):
             if 'lat' in column.attributes:
                 lat = hxl.geo.parse_lat(value)
                 if lat is not None:
                     value = format(lat, '0.4f')
                 else:
+                    logup('Cannot parse as a latitude', {"value": value}, level='info')
                     logger.warning('Cannot parse %s as a latitude', str(value))
                     if self.purge:
                         value = ''
             elif 'lon' in column.attributes:
                 lon = hxl.geo.parse_lon(value)
                 if lon is not None:
                     value = format(lon, '0.4f')
                 else:
+                    logup('Cannot parse as a longitude', {"value": value}, level='info')
                     logger.warning('Cannot parse %s as a longitude', str(value))
                     if self.purge:
                         value = ''
             elif 'coord' in column. attributes:
                 coord = hxl.geo.parse_coord(value)
                 if coord is not None:
                     value = '{:.4f},{:.4f}'.format(coord[0], coord[1])
                 else:
+                    logup('Cannot parse as geographical coordinates', {"value": value}, level='info')
                     logger.warning('Cannot parse %s as geographical coordinates', str(value))
                     if self.purge:
                         value = ''
-        
+
         return value
 
     def _match_patterns(self, patterns, column):
         """Test if a column matches a list of patterns.
         @param patterns: a list of tag patterns to match
         @param column: the column definition to test
         @returns: C{True} if the column matches at least one pattern in the list
@@ -1163,29 +1268,30 @@
         """
         return CleanDataFilter(
             source=source,
             whitespace=opt_arg(spec,'whitespace', []),
             upper=opt_arg(spec, 'upper', []),
             lower=opt_arg(spec, 'lower', []),
             date=opt_arg(spec, 'date', []),
-            date_format=opt_arg(spec, 'date_format', '%Y-%m-%d'),
+            date_format=opt_arg(spec, 'date_format', None),
             number=opt_arg(spec, 'number', []),
             number_format=opt_arg(spec, 'number_format', None),
             latlon=opt_arg(spec, 'latlon', []),
             purge=opt_arg(spec, 'purge', False),
             queries=opt_arg(spec, 'queries', [])
         )
 
 
 class ColumnFilter(AbstractStreamingFilter):
     """Composable filter class to remove columns from a HXL dataset.
 
-    This filter supports removing columns based on either a whitelist
-    or a blacklist of L{tag patterns<hxl.model.TagPattern>}. It
-    supports the L{hxl.model.Dataset.with_columns} and
+    This filter supports removing columns based on either an include
+    list or an exclude list of L{tag
+    patterns<hxl.model.TagPattern>}. It supports the
+    L{hxl.model.Dataset.with_columns} and
     L{hxl.model.Dataset.without_columns} convenience methods and the
     L{hxl.scripts.hxlcut} command-line script.
 
     Remove all columns matching the pattern "#contact+email" from the
     dataset::
 
       filter = ColumnFilter(hxl.data(url), exclude_tags='contact+email')
@@ -1200,21 +1306,22 @@
       filter = ColumnFilter(hxl.data(url), include_tags=['org', 'sector', 'activity'])
 
       # or
 
       filter = hxl.data(url).with_columns(['org', 'sector', 'activity'])
 
     @see: L{RowFilter}
+
     """
 
     def __init__(self, source, include_tags=[], exclude_tags=[], skip_untagged=False):
         """Construct a column filter.
         @param source: a L{hxl.model.Dataset}
-        @param include_tags: a whitelist of L{tag patterns<hxl.model.TagPattern>} objects to include
-        @param exclude_tags: a blacklist of tag patterns objects to exclude
+        @param include_tags: an include list of L{tag patterns<hxl.model.TagPattern>} objects to include
+        @param exclude_tags: an exclude list of tag patterns objects to exclude
         @param skip_untagged: True if all columns without HXL hashtags should be removed
         """
         super(ColumnFilter, self).__init__(source)
         self.include_tags = hxl.model.TagPattern.parse_list(include_tags)
         self.exclude_tags = hxl.model.TagPattern.parse_list(exclude_tags)
         self.skip_untagged = skip_untagged
         self.indices = [] # saved indices for columns to include
@@ -1236,63 +1343,66 @@
             try:
                 values.append(row.values[i])
             except IndexError:
                 pass # don't add anything
         return values
 
     def _test_column(self, column):
-        """Test whether a  column should be included in the output.
-        If there is a whitelist, it must be in the whitelist; if there is a blacklist, it must not be in the blacklist.
+        """Test whether a column should be included in the output.  If there
+        is an include list, it must be in that list; if there is an
+        exclude list, it must not be in that list.
+
         @param column: the L{hxl.model.Column} to test
         @returns: True if the column should be included
+
         """
         if self.include_tags:
-            # whitelist
+            # exclude list
             for pattern in self.include_tags:
                 if pattern.match(column):
                     # succeed as soon as we match an included pattern
                     return True
-            # fail if there was a whitelist and we didn't match
+            # fail if there was an exclude list and we didn't match
             return False
 
         if self.exclude_tags or self.skip_untagged:
             # skip untagged columns?
             if self.skip_untagged and not column.tag:
                 return False
-            # blacklist
+            # exclude list
             for pattern in self.exclude_tags:
                 if pattern.match(column):
                     # fail as soon as we match an excluded pattern
                     return False
 
-        # not a whitelist, and no reason to exclude
+        # not an include list, and no reason to exclude
         return True
 
     @staticmethod
     def _load(source, spec):
         """Create a filter object from a JSON-like spec.
         Note that there are two JSON filter definitions for this class: "with_columns" and "without_columns".
         @param spec: the specification
         @returns: a L{ColumnFilter} object
         """
         if spec.get('filter') == 'with_columns':
             return ColumnFilter(
                 source=source,
-                include_tags=req_arg(spec, 'whitelist')
+                include_tags=req_arg(spec, 'includes')
             )
         else:
             return ColumnFilter(
                 source=source,
-                exclude_tags=req_arg(spec, 'blacklist'),
+                exclude_tags=req_arg(spec, 'excludes'),
                 skip_untagged=opt_arg(spec, 'skip_untagged')
             )
 
 
 class CountFilter(AbstractCachingFilter):
-    """Composable filter class to aggregate rows in a HXL dataset.
+    """Composable filter class to aggregate rows in a HXL dataset (like a pivot table)
 
     This class supports the L{hxl.model.Dataset.count} convenience
     method and the L{hxl.scripts.hxlcount} command-line script.
 
     This is a L{caching filter<AbstractCachingFilter>} that performs
     aggregate actions such as counting, summing, and averaging across
     multiple rows of data. For example, it can reduce a dataset to a
@@ -1346,28 +1456,28 @@
                 columns.append(copy.deepcopy(column))
             else:
                 columns.append(hxl.Column())
 
         # Add generated columns
         for aggregator in self.aggregators:
             columns.append(aggregator.column)
-            
+
         return columns
 
     def filter_rows(self):
         """@returns: the filtered row values"""
 
         raw_data = []
 
         # each item is a sequence containing a tuple of key values and an _Aggregator object
         for aggregate in self._aggregate_data():
             raw_data.append(
-                list(aggregate[0]) + [hxl.datatypes.normalise_number(aggregator.value) if aggregator.value is not None else '' for aggregator in aggregate[1]]
+                list(aggregate[0]) + [aggregator.value if aggregator.value is not None else '' for aggregator in aggregate[1]]
             )
-            
+
         return raw_data
 
     def _aggregate_data(self):
         """Read the entire source dataset and produce saved aggregate data.
         @returns: the aggregated values as raw data
         """
         aggregators = {}
@@ -1377,15 +1487,15 @@
             # will always match if there are no queries
             if hxl.model.RowQuery.match_list(row, self.queries):
                 # get the values in the order we need them
                 values = [hxl.datatypes.normalise_space(row.get(pattern, default='')) for pattern in self.patterns]
                 # make a dict key for the aggregator
                 key = tuple(values)
                 if not key in aggregators:
-                    aggregators[key] = [copy.copy(aggregator) for aggregator in self.aggregators]
+                    aggregators[key] = [copy.deepcopy(aggregator) for aggregator in self.aggregators]
                 for aggregator in aggregators[key]:
                     aggregator.evaluate_row(row)
 
         # sort the aggregators by their keys
         return sorted(aggregators.items())
 
     @staticmethod
@@ -1451,15 +1561,130 @@
         """
         return DeduplicationFilter(
             source = source,
             patterns=opt_arg(spec, 'patterns', []),
             queries=opt_arg(spec, 'queries', [])
         )
 
-        
+
+class ExpandListsFilter(AbstractBaseFilter):
+    """Expand in-cell lists by duplicating data rows.
+    """
+
+    def __init__(self, source, patterns=None, separator="|", correlate=False, queries=[]):
+        super().__init__(source)
+        self.separator = str(separator)
+        self.scan_columns(patterns)
+        self.correlate = correlate
+        self.queries = self._setup_queries(queries)
+        """The row queries to limit where we expand lists"""
+
+    def filter_columns(self):
+        """ Remove the +list attribute from targeted columns """
+        columns = list(self.source.columns)
+        for index in self.column_indices:
+            column = copy.deepcopy(columns[index])
+            column.remove_attribute('list')
+            columns[index] = column
+        return columns
+
+    def scan_columns(self, patterns):
+        """ Save the indices of the columns containing lists """
+        self.column_indices = []
+        if patterns:
+            patterns = hxl.model.TagPattern.parse_list(patterns)
+            for i, column in enumerate(self.source.columns):
+                if hxl.model.TagPattern.match_list(column, patterns):
+                    self.column_indices.append(i)
+        else:
+            for i, column in enumerate(self.source.columns):
+                if column.has_attribute("list"):
+                    self.column_indices.append(i)
+
+    def __iter__(self):
+
+        # Special case: no columns to expand
+        if len(self.column_indices) == 0:
+            for row in self.source:
+                yield row
+            return
+
+
+        # Regular case
+
+        min_length = max(self.column_indices) + 1
+
+        for row in self.source:
+
+            # If there are queries, the row must match one of them
+            if not hxl.model.RowQuery.match_list(row, self.queries):
+                yield row
+                continue
+
+            # parse the lists
+            value_lists = []
+            for index in self.column_indices:
+                if index < len(row.values):
+                    values = str(row.values[index]).split(self.separator)
+                    value_lists.append(list(map(hxl.datatypes.normalise_space, values)))
+                else:
+                    value_lists.append([""])
+
+            if (self.correlate):
+                # correlate the lists
+
+                nrows = max([len(item) for item in value_lists])
+
+                for i in range(0, nrows):
+                    values = copy.deepcopy(row.values)
+                    for j, v in enumerate(value_lists):
+                        index = self.column_indices[j]
+                        if len(v) <= i:
+                            values[index] = ""
+                        else:
+                            values[index] = v[i]
+                    yield hxl.model.Row(self.columns, values)
+
+            else:
+                # generate the cartesian product of all the lists
+
+                # generate the cartesian product of the values
+                row_value_list = list(itertools.product(*value_lists))
+
+                # yield all of the resulting rows
+                for row_values in row_value_list:
+                    values = copy.deepcopy(row.values)
+
+                    # make sure the value list is long enough
+                    if len(values) < min_length:
+                        values += [""] * (min_length - len(values))
+
+                    # replace the list values
+                    for i, value in enumerate(row_values):
+                        values[self.column_indices[i]] = value
+
+                    # yield a new row
+                    yield hxl.model.Row(self.columns, values)
+
+
+    @staticmethod
+    def _load(source, spec):
+        """New instance from a JSON-style dictionary.
+        @param source: the upstream data source
+        @param spec: the JSON-style specification
+        """
+        return ExpandListsFilter(
+            source=source,
+            patterns=opt_arg(spec, 'patterns'),
+            separator=opt_arg(spec, 'separator'),
+            correlate=opt_arg(spec, 'correlate'),
+            queries=opt_arg(spec, 'queries')
+        )
+
+
 class ExplodeFilter(AbstractBaseFilter):
     """Explode a wide (series) dataset into a long version.
 
     Every set of identically-tagged columns that contain the +label
     attribute in their hashtag will get their own row, with the header
     text and the value side by side.  For example,
 
@@ -1475,14 +1700,15 @@
     Cameroon,2014,150
     Cameroon,2015,120
 
     (You can use the RenameFilter to change the names and hashtags of
     the generated columns.)
 
     @see: hxl.model.Dataset.explode
+    @see: hxl.filters.ImplodeFilter
     """
 
     def __init__(self, source, header_attribute='header', value_attribute='value'):
         """
         Constructor
         @param source: the upstream source dataset
         @param header_attribute: the attribute to add to the hashtag for the column with the former header (default: 'header')
@@ -1565,14 +1791,172 @@
         return ExplodeFilter(
             source=source,
             header_attribute=opt_arg(spec, 'header_attribute', 'header'),
             value_attribute=opt_arg(spec, 'value_attribute', 'value')
         )
 
 
+class ImplodeFilter(AbstractBaseFilter):
+    """Implode a long (series) dataset into a wide version.
+
+    The first column matching the pattern will be used as headers. For example, with the tag pattern #date+year,
+
+    Country,Header,Value
+    #country,#date+year,#affected
+    Cameroon,2015,100
+    Cameroon,2014,150
+    Cameroon,2015,120
+
+    will be converted to
+
+    Country,2015,2014,2013
+    #country,#affected+label,#affected+label,#affected+label
+    Cameroon,100,150,120
+
+    @see: hxl.model.Dataset.implode
+    @see: hxl.filters.ExplodeFilter
+    """
+
+    def __init__(self, source, label_pattern, value_pattern):
+        """ Constructor
+        @param source: the upstream source dataset
+        @param pattern: the tag pattern to use for the labels
+        @param output_tagspec: the tagspec to use for the repeated, wide columns
+        """
+        super(ImplodeFilter, self).__init__(source)
+        self.label_pattern = label_pattern
+        self.value_pattern = value_pattern
+
+        self.processed = False
+        self.label_index = -1
+        self.value_index = -1
+        self.labels = set()
+        self.rows = dict()
+        self.new_columns = None
+        self.source_iterator = None
+
+    def filter_columns(self):
+        """@returns: the new (exploded) column headers"""
+        if self.new_columns is None:
+            self.process()
+            # add existing columns (excluding label and value columns)
+            self.new_columns = []
+            for i, column in enumerate(self.source.columns):
+                if i != self.label_index and i != self.value_index:
+                    self.new_columns.append(column)
+
+            # add extra columns for new, "wide" data
+            model = self.source.columns[self.value_index]
+            for label in sorted(self.labels):
+                attributes = set(model.attributes)
+                attributes.add("label")
+                column = hxl.model.Column(tag=model.tag, attributes=attributes, header=label)
+                self.new_columns.append(column)
+
+        return self.new_columns
+
+    def __iter__(self):
+        """Custom iterator to produce exploded rows."""
+        self.process()
+        for key in self.rows:
+            values = list(key)
+            # extra, wide values
+            for label in sorted(self.labels):
+                values.append(self.rows[key].get(label, ""))
+            yield hxl.model.Row(self.columns, values)
+
+    def process(self):
+        # check if we've already done all this
+        if self.processed:
+            return
+
+        # determine the indices of the label and value columns
+        # if either is missing, just pass on the source data normally (with logged errors)
+        lpattern = hxl.model.TagPattern.parse(self.label_pattern)
+        vpattern = hxl.model.TagPattern.parse(self.value_pattern)
+        for i, column in enumerate(self.source.columns):
+            if lpattern.match(column):
+                if self.label_index == -1:
+                    self.label_index = i
+                else:
+                    logup('[Implode filter] multiple columns match label pattern; using first match', {
+                        "pattern": self.label_pattern,
+                        "tag": self.source.columns[self.label_index].display_tag,
+                        "header": self.source.columns[self.label_index].header
+                    }, level='info')
+                    logger.warning(
+                        "[Implode filter] multiple columns match label pattern %s; using first match %s (%s)",
+                        self.label_pattern,
+                        self.source.columns[self.label_index].display_tag,
+                        self.source.columns[self.label_index].header
+                    )
+            if vpattern.match(column):
+                if self.value_index == -1:
+                    self.value_index = i
+                else:
+                    logup('[Implode filter] multiple columns match value pattern; using first match', {
+                        "pattern": self.label_pattern
+                    }, level='info')
+                    logger.warning(
+                        "[Implode filter] multiple columns match value pattern %s; using first match",
+                        self.value_pattern
+                    )
+
+        if self.label_index == -1:
+            raise HXLFilterException("No matching label column for {}".format(self.label_pattern))
+
+        if self.value_index == -1:
+            raise HXLFilterException("No matching value column for {}".format(self.value_pattern))
+
+        # iterate through the dataset
+        for row in self.source:
+
+            values = list(row.values)
+
+            # get the "wide" label and value
+            label = ""
+            if self.label_index < len(values):
+                label = values[self.label_index]
+
+            self.labels.add(label)
+
+            value = ""
+            if self.value_index < len(values):
+                value = values[self.value_index]
+
+            # make a key tuple, excluding the label and value columns
+            values = []
+            for i, value in enumerate(row.values):
+                if i != self.label_index and i != self.value_index:
+                    values.append(value)
+            key = tuple(values)
+
+            # check to see if we already have data for that key
+            if key not in self.rows:
+                self.rows[key] = {}
+            if label in self.rows[key]:
+                logup('Multiple values in implode filter; using first match', {"value": label, "value_used": self.rows[key][label]}, level='info')
+                logger.error("Multiple values for %s in implode filter; using %s", label, self.rows[key][label])
+            else:
+                self.rows[key][label] = value
+
+    @staticmethod
+    def _load(source, spec):
+        """Create an implode filter from a dict spec.
+        @param source: the upstream source
+        @param spec: the JSON-like filter specification
+        @returns: an L{ImplodeFilter} object
+        """
+        return ImplodeFilter(
+            source=source,
+            label_pattern=req_arg(spec, 'label_pattern'),
+            value_pattern=req_arg(spec, 'value_pattern')
+        )
+
+
 class MergeDataFilter(AbstractStreamingFilter):
     """Composable filter class to merge values from two HXL datasets.
 
     Merges the values for the *last* matching row in the merge
     dataset. Can use patterns to match multiple cells for merging
     (using all candidate columns when there are muliple columns
     matching the same hashtag pattern). Can overwrite existing columns
@@ -1627,27 +2011,27 @@
         """Indices for mapping columns from merge source to output dataset
         [source_index, output_index, overwrite_ok]
         """
         self._merge_values = None
         """Dictionary of values from merge source, indexed by key."""
 
     def filter_columns(self):
-        """Filter the columns to add newly-merged ones.  
+        """Filter the columns to add newly-merged ones.
         Note: this is called only once, the first time someone
         accesses the Dataset.columns property, then the result is saved for future use.
         As a side effect, builds the _merge_indices specs for generating the merged data.
         @see hxl.filters.AbstractBaseFilter.filter_columns
         """
 
         new_columns = list(self.source.columns)
         """The new column list to return."""
-        
+
         merge_column_index = len(self.source.columns)
         """Target index for merging into the output dataset"""
-            
+
         # Check every pattern
         for pattern in self.merge_tags:
 
             # Check the pattern against every column
             for index, column in enumerate(self.merge_source.columns):
 
                 seen_replacement = False
@@ -1707,15 +2091,15 @@
 
     def _read_merge(self):
         """Read the second (merging) dataset into memory.
         Stores only the values necessary for the merge.
         Uses *last* matching row for each key (top to bottom).
         @returns: a map of merge values
         """
-        
+
         self.columns # make sure we've created the _merge_indices map
 
         merge_values = {}
         """Map of keys to merge values from the merge source."""
 
         for row in self.merge_source:
             if hxl.model.RowQuery.match_list(row, self.queries):
@@ -1783,37 +2167,41 @@
     def filter_row(self, row):
         """@returns: a deep copy of the row's values"""
         return copy.copy(row.values)
 
     def _rename_column(self, column):
         """@returns: a copy of the column object, with a new name if needed"""
         for spec in self.rename:
-            if spec[0].match(column):
+            norm = hxl.datatypes.normalise_string
+            if spec[0].match(column) and (not spec[2] or norm(spec[2]) == norm(column.header)):
                 new_column = copy.deepcopy(spec[1])
                 if new_column.header is None:
                     new_column.header = column.header
                 return new_column
         return copy.deepcopy(column)
 
-    RENAME_PATTERN = r'^\s*#?({token}(?:\s*[+-]{token})*):(?:([^#]*)#)?({token}(?:\s*[+]{token})*)\s*$'.format(token=hxl.datatypes.TOKEN_PATTERN)
+    RENAME_PATTERN = r'^\s*(?:([^#]*)#)?({token}(?:\s*[+-]{token})*)\s*:\s*(?:([^#]*)#)?({token}(?:\s*[+]{token})*)\s*$'.format(
+        token=hxl.datatypes.TOKEN_PATTERN
+    )
     """Regular expression for parsing a rename pattern"""
 
     @staticmethod
     def parse_rename(s):
         """Parse a rename specification from the parameters.
         @param s: the specification to parse
         @returns: a tuple with the old pattern to match and new column spec
         @exception HXLFilterException: if the spec is not parseable
         """
         if isinstance(s, six.string_types):
             result = re.match(RenameFilter.RENAME_PATTERN, s)
             if result:
-                pattern = hxl.model.TagPattern.parse(result.group(1))
-                column = hxl.model.Column.parse('#' + result.group(3), header=result.group(2), use_exception=True)
-                return (pattern, column)
+                header = result.group(1)
+                pattern = hxl.model.TagPattern.parse(result.group(2))
+                column = hxl.model.Column.parse('#' + result.group(4), header=result.group(3), use_exception=True)
+                return (pattern, column, header)
             else:
                 raise HXLFilterException("Bad rename expression: " + s)
         else:
             return s
 
     @staticmethod
     def _load(source, spec):
@@ -1823,72 +2211,75 @@
         @returns: a L{RenameFilter} object
         """
         return RenameFilter(
             source=source,
             rename=req_arg(spec, 'specs')
         )
 
-    
+
 class JSONPathFilter(AbstractStreamingFilter):
     """Extract values from a JSON string expression using JSONPath
     See http://goessner.net/articles/JsonPath/
     Optionally restrict to specific columns and/or rows
     """
 
-    def __init__(self, source, path, patterns=None, queries=[]):
+    def __init__(self, source, path, patterns=None, queries=[], use_json=True):
         """Constructor
         @param source: the upstream data source
         @param path: a JSONPath expression for extracting data
         @param patterns: a tag pattern or list of patterns for the columns to use (default to all)
         @param queries: a predicate or list of predicates for the rows to consider.
+        @param use_json: if True, serialise multiple values as JSON (default); otherwise, separate with " | "
         """
         super().__init__(source)
-        self.path = jsonpath_rw.parse(path)
+        self.path = jsonpath_ng.ext.parse(path)
         self.patterns = hxl.model.TagPattern.parse_list(patterns)
         self.queries = self._setup_queries(queries)
+        self.use_json = use_json
         self._indices = None
 
     def filter_row(self, row):
         if self._indices is None:
             self._indices = self._get_indices(self.patterns)
 
         values = list(row.values)
 
         if hxl.model.RowQuery.match_list(row, self.queries):
-        
+
             for i in self._indices:
                 try:
                     expr = json.loads(values[i])
                     results = [match.value for match in self.path.find(expr)]
                     if len(results) == 0:
                         values[i] = ''
                     elif len(results) == 1:
-                        values[i] = hxl.datatypes.flatten(results[0])
+                        values[i] = hxl.datatypes.flatten(results[0], self.use_json)
                     else:
-                        values[i] = hxl.datatypes.flatten(results)
-                except ValueError as e:
+                        values[i] = hxl.datatypes.flatten(results, self.use_json)
+                except (ValueError, TypeError,) as e:
+                    logup('Skipping invalid JSON expression', {"expression": str(values[i])}, level='info')
                     logger.warning("Skipping invalid JSON expression '%s'", values[i])
 
         return values
-    
+
     @staticmethod
     def _load(source, spec):
         """Create a JSONPath filter from a dict spec.
         @param source: the upstream data source
         @param spec: the JSON-like filter specification
         @returns: a L{RenameFilter} object
         """
         return JSONPathFilter(
             source=source,
             path=req_arg(spec, 'path'),
             patterns=opt_arg(spec, 'patterns'),
             queries=opt_arg(spec, 'queries')
         )
 
-    
+
 class FillDataFilter(AbstractStreamingFilter):
     """Fill empty cells in a dataset.
     By default, fill all empty cells with the closest non-empty value in a previous row.
     Optionally restrict to specific columns and/or rows.
     """
 
     def __init__(self, source, patterns=None, queries=[]):
@@ -1903,23 +2294,25 @@
         self._saved = {}
         self._indices = None
 
     def filter_row(self, row):
         """@returns: row values with some empty values possibly filled in"""
         values = list(row.values)
 
-        # Fill if there are no row queries, or this row matches one
+        # Guessing at empty cells (column-wise only)
         if self._indices is None:
             self._indices = self._get_indices(self.patterns)
         for i in self._indices:
+            if i >= len(values):
+                values += [''] * (i - len(values) + 1) # make sure list is long enough
             if values[i]:
                 self._saved[i] = values[i]
             elif (not self.queries) or (hxl.model.RowQuery.match_list(row, self.queries)):
                 values[i] = self._saved[i] if self._saved.get(i) else ''
-                    
+
         return values
 
     @staticmethod
     def _load(source, spec):
         """Create a fill-data filter from a dict spec.
         @param source: the upstream data source
         @param spec: the JSON-like filter specification
@@ -1927,15 +2320,15 @@
         """
         return FillDataFilter(
             source=source,
             patterns=opt_arg(spec, 'patterns'),
             queries=opt_arg(spec, 'queries'),
         )
 
-    
+
 class ReplaceDataFilter(AbstractStreamingFilter):
     """
     Composable filter class to replace values in a HXL dataset.
 
     This is the class supporting the hxlreplace console script.
 
     Usage:
@@ -1954,27 +2347,47 @@
         @param queries: optional list of filter queries for rows where replacements should be applied.
         """
         super(ReplaceDataFilter, self).__init__(source)
         self.replacements = replacements
         if isinstance(self.replacements, ReplaceDataFilter.Replacement):
             self.replacements = [self.replacements]
         self.queries = self._setup_queries(queries)
+        self.indices = self._setup_indices(self.replacements, self.columns)
+
 
     def filter_row(self, row):
         """@returns: the row values with replacements"""
         if hxl.model.RowQuery.match_list(row, self.queries):
+            replaced = set()
             values = copy.copy(row.values)
-            for index, value in enumerate(values):
-                for replacement in self.replacements:
-                    value = replacement.sub(row.columns[index], value)
-                    values[index] = value
+            for i, replacement in enumerate(self.replacements):
+                indices = self.indices[i]
+                for index in indices:
+                    if index not in replaced and index < len(values):
+                        new_value = replacement.sub(values[index])
+                        if new_value is not False:
+                            replaced.add(index)
+                            values[index] = new_value
             return values
         else:
             return row.values
 
+
+    def _setup_indices(self, replacements, columns):
+        """ Return a list of matching column indices for each replacement """
+        result = []
+        for replacement in replacements:
+            indices = []
+            for i, column in enumerate(columns):
+                if replacement.matches(column):
+                    indices.append(i)
+            result.append(indices)
+        return result
+
+
     class Replacement:
         """Replacement specification."""
 
         def __init__(self, original, replacement, patterns=None, is_regex=False):
             """
             @param original: a string (case- and space-insensitive) or regular expression (sensitive) to replace
             @param replacement: the replacement string or regular expression substitution
@@ -1990,29 +2403,36 @@
                 self.patterns = hxl.model.TagPattern.parse_list(patterns)
             else:
                 self.patterns = None
             self.is_regex = is_regex
             if not self.is_regex:
                 self.original = hxl.datatypes.normalise_string(self.original)
 
-        def sub(self, column, value):
+        def matches(self, column):
+            """ Return true if the replacement applies to the column provided """
+            if self.patterns:
+                return hxl.model.TagPattern.match_list(column, self.patterns)
+            else:
+                return True
+
+        def sub(self, value):
             """
             Substitute inside the value, if appropriate.
-            @param column: the column definition
             @param value: the cell value
-            @returns: the value, possibly changed
+            @returns: the new value if changed; False otherwise
             """
-            if self.patterns and not hxl.model.TagPattern.match_list(column, self.patterns):
-                return value
-            elif self.is_regex:
-                return re.sub(self.original, self.replacement, str(value))
+            
+            if self.is_regex:
+                result = re.subn(self.original, self.replacement, str(value))
+                if result[1] > 0:
+                    return result[0]
             elif self.original == hxl.datatypes.normalise_string(value):
                 return self.replacement
-            else:
-                return value
+
+            return False
 
         @staticmethod
         def parse_map(source):
             """Parse a substitution map."""
             replacements = []
             for row in source:
                 if row.get('#x_pattern'):
@@ -2051,23 +2471,23 @@
 
         return ReplaceDataFilter(
             source=source,
             replacements=replacements,
             queries=opt_arg(spec, 'queries', [])
         )
 
-        
+
 class RowCountFilter(AbstractStreamingFilter):
     """
     Composable filter class to count lines (and nothing else)
 
     The output is identical to the input; the line count is
     stored in the filter itself.  As a result, there is no corresponding
     command-line utility.
-    
+
     Usage:
 
     <pre>
     counter = hxl.data(url).row_counter();
     // process the filter
     print("{} lines".format(counter.row_count);
     </pre>
@@ -2078,27 +2498,27 @@
         self.row_count = 0
         self.queries = self._setup_queries(queries)
 
     def filter_row(self, row):
         if hxl.model.RowQuery.match_list(row, self.queries):
             self.row_count += 1
         return row.values
-    
+
 
 class RowFilter(AbstractStreamingFilter):
     """
     Composable filter class to select rows from a HXL dataset.
 
     Usage:
 
     <pre>
-    # whitelist
+    # include list
     hxl.data(url).with_rows('org=OXFAM')
 
-    # blacklist
+    # exclude list
     hxl.data(url).without_rows('org=OXFAM')
     </pre>
     """
 
     def __init__(self, source, queries=[], reverse=False, mask=[]):
         """
         Constructor
@@ -2127,27 +2547,27 @@
             if not hxl.model.RowQuery.match_list(row, self.queries, self.reverse):
                 return None
         return row.values
 
     @staticmethod
     def _load(source, spec):
         """Construct a row filter from a dict spec."""
-        
+
         reverse = False
         if spec.get('filter') == 'without_rows':
             reverse = True
 
         return RowFilter(
             source=source,
             queries=req_arg(spec, 'queries'),
             reverse=reverse,
             mask=opt_arg(spec, 'mask', [])
         )
 
-    
+
 class SortFilter(AbstractCachingFilter):
     """
     Composable filter class to sort a HXL dataset.
 
     This is the class supporting the hxlsort command-line utility.
 
     Usage:
@@ -2201,15 +2621,16 @@
 
         if indices:
             for index in indices:
                 key.append(SortFilter._make_sort_value(self.columns[index].tag, values[index]))
         else:
             # Sort everything, left to right
             for index, value in enumerate(values):
-                key.append(SortFilter._make_sort_value(self.columns[index].tag, value))
+                if index < len(self.columns):
+                    key.append(SortFilter._make_sort_value(self.columns[index].tag, value))
 
         # convert the key to a tuple for sorting
         return tuple(key)
 
     @staticmethod
     def _make_sort_value(tag, value):
         """
@@ -2217,47 +2638,50 @@
 
         The sort value is is a tuple of a numeric value (possibly inf)
         and the original string value. This will ensure that numeric
         values sort properly, and string values sort after them.
         """
         norm = hxl.datatypes.normalise_string(value)
         if tag == '#date':
-            if hxl.datatypes.is_date(norm):
+            try:
                 return (float('inf'), hxl.datatypes.normalise_date(norm))
-            else:
+            except ValueError:
                 return (float('inf'), norm)
         else:
             try:
                 return (float(norm), norm)
             except:
                 return (float('inf'), norm)
 
     @staticmethod
     def _load(source, spec):
         """Create a sort filter from a dict spec."""
         return SortFilter(
             source = source,
-            tags=opt_arg(spec, 'keys', []),
+            tags=opt_arg(spec, 'tags', []),
             reverse=opt_arg(spec, 'reverse', False)
         )
 
 
 #
 # Compile a filter chain
 #
 
 LOAD_MAP = {
     'add_columns': AddColumnsFilter._load,
     'append': AppendFilter._load,
+    'append_external_list': AppendFilter._load,
     'cache': CacheFilter._load,
     'clean_data': CleanDataFilter._load,
     'count': CountFilter._load,
     'dedup': DeduplicationFilter._load,
+    'expand_lists': ExpandListsFilter._load,
     'explode': ExplodeFilter._load,
     'fill_data': FillDataFilter._load,
+    'implode': ImplodeFilter._load,
     'jsonpath': JSONPathFilter._load,
     'merge_data': MergeDataFilter._load,
     'rename_columns': RenameFilter._load,
     'replace_data': ReplaceDataFilter._load,
     'replace_data_map': ReplaceDataFilter._load,
     'sort': SortFilter._load,
     'with_columns': ColumnFilter._load,
@@ -2326,20 +2750,20 @@
         type = req_arg(spec, 'filter')
         loader = LOAD_MAP.get(type)
         if not loader:
             raise HXLFilterException("Unknown filter type {}".format(type))
 
         # Create the filter
         source = loader(source, spec)
-        
+
     return source
 
 
 def list_product(lists, head=[]):
-    """Generate the cartesian product of a list of lists 
+    """Generate the cartesian product of a list of lists
     The elements of the result will be all possible combinations of the elements of
     the input lists.
     @param lists: a list of lists
     @return: the cross-product of the lists
     """
     if lists:
         result = []
@@ -2349,15 +2773,15 @@
         return result
     else:
         return [head]
 
 
 def is_sourcey(arg):
     """Convoluted method to try to distinguish a single HXL data source from a list of sources.
-    Trying to recognise all the source types supported by hxl.io.make_input
+    Trying to recognise all the source types supported by hxl.input.make_input
     @param arg: the thing to test (we want to know if it's a single source or lists of sources)
     @returns: True if we think it's a single source; False otherwise.
     """
 
     # Not a list
     if ((not hasattr(arg, '__len__')) or
         isinstance(arg, dict) or
```

### Comparing `libhxl-4.9/hxl/model.py` & `libhxl-5.0/hxl/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,81 @@
-"""
-Data model for the Humanitarian Exchange Language (HXL) v1.0
-David Megginson
-Started October 2014
+"""Main data-model classes for the Humanitarian Exchange Language (HXL).
+
+This module defines the basic classes for working with HXL data. Other
+modules have classes derived from these (e.g. in
+[hxl.filters](filters.html) or [hxl.input](io.html)). The core class is
+[Dataset](#hxl.model.Dataset), which defines the operations available
+on a HXL dataset, including convenience methods for chaining filters.
+
+Typical usage:
+
+    source = hxl.data("https://example.org/data.csv")
+    # returns a hxl.model.Dataset object
+
+    result = source.with_lines("#country+name=Kenya").sort()
+    # a filtered/sorted view of the data
+
+
+This code is released into the Public Domain and comes with NO WARRANTY.
 
-License: Public Domain
-Documentation: https://github.com/HXLStandard/libhxl-python/wiki
 """
 
-import abc, copy, csv, dateutil, json, logging, operator, re, six
+import abc, copy, csv, dateutil, hashlib, json, logging, operator, re, six
 
 import hxl
 
+from hxl.util import logup
+
 logger = logging.getLogger(__name__)
 
 
+# Cut off for fuzzy detection of a hashtag row
+# At least this percentage of cells must parse as HXL hashtags
+FUZZY_HASHTAG_PERCENTAGE = 0.5
+
+
 class TagPattern(object):
     """Pattern for matching a HXL hashtag and attributes
-    #tag matches #tag with any attributes
-    #tag+foo matches #tag with foo among its attributes
-    #tag-foo matches #tag with foo *not* among its attributes
-    #tag+foo-bar matches #tag with foo but not bar
+
+    - the pattern "#*" matches any hashtag/attribute combination
+    - the pattern "#*+foo" matches any hashtag with the foo attribute
+    - the pattern "#tag" matches #tag with any attributes
+    - the pattern "#tag+foo" matches #tag with foo among its attributes
+    - the pattern "#tag-foo" matches #tag with foo *not* among its attributes
+    - the pattern "#tag+foo-bar" matches #tag with foo but not bar
+    - the pattern "#tag+foo+bar!" matches #tag with exactly the attributes foo and bar, but *no others*
+
+    The normal way to create a tag pattern is using the
+    [parse()](#hxl.model.TagPattern.parse) method rather than the
+    constructor:
+
+        pattern = hxl.model.TagPattern.parse("#affected+f-children")
+
+    Args:
+        tag: the basic hashtag (without attributes)
+        include_attributes: a list of attributes that must be present
+        exclude_attributes: a list of attributes that must not be present
+        is_absolute: if True, no attributes are allowed except those in _include_attributes_
+
     """
 
-    # Regular expression to match a HXL tag pattern (including '-' to exclude attributes)
+
     PATTERN = r'^\s*#?({token}|\*)((?:\s*[+-]{token})*)\s*(!)?\s*$'.format(token=hxl.datatypes.TOKEN_PATTERN)
+    """Constant: regular expression to match a HXL tag pattern.
+    """
 
     def __init__(self, tag, include_attributes=[], exclude_attributes=[], is_absolute=False):
-        """Like a column, but has a whitelist and a blacklist.
-        @param tag: the basic hashtag (without attributes)
-        @param include_attributes: a list of attributes that must be present
-        @param exclude_attributes: a list of attributes that must not be present
-        """
         self.tag = tag
-        """HXL hashtag, or "#*" for a wildcard"""
 
         self.include_attributes = set(include_attributes)
         """Set of all attributes that must be present"""
-        
+
         self.exclude_attributes = set(exclude_attributes)
         """Set of all attributes that must not be present"""
-        
+
         self.is_absolute = is_absolute
         """True if this pattern is absolute (no extra attributes allowed)"""
 
     def is_wildcard(self):
         return self.tag == '#*'
 
     def match(self, column):
@@ -109,15 +141,28 @@
                 s += '-' + attribute
         return s
 
     __str__ = __repr__
 
     @staticmethod
     def parse(s):
-        """Parse a single tag pattern, like #tag+foo-bar."""
+        """Parse a single tag-pattern string.
+
+            pattern = TagPattern.parse("#affected+f-children")
+
+        The [parse_list()](#hxl.model.TagPattern.parse_list) method
+        will call this method to parse multiple patterns at once.
+
+        Args:
+            s: the tag-pattern string to parse
+
+        Returns:
+            A TagPattern object
+
+        """
 
         if not s:
             # edge case: null value
             raise hxl.HXLException('Attempt to parse empty tag pattern')
         elif isinstance(s, TagPattern):
             # edge case: already parsed
             return s
@@ -146,33 +191,56 @@
                 is_absolute=is_absolute
             )
         else:
             raise hxl.HXLException('Malformed tag: ' + s)
 
     @staticmethod
     def parse_list(specs):
-        """
-        Normalise a list of tag specs.
-        Split if a comma-separated string.
-        Convert every element to a TagPattern
-        @param specs the raw input
-        @return normalised list of tag patterns
+        """Parse a list of tag-pattern strings.
+
+        If _specs_ is a list of already-parsed TagPattern objects, do
+        nothing. If it's a list of strings, apply
+        [parse()](#hxl.model.TagPattern.parse) to each one. If it's a
+        single string with multiple patterns separated by commas,
+        split the string, then parse the patterns.
+
+            patterns = TagPattern.parse_list("#affected+f,#inneed+f")
+            # or
+            patterns = TagPattern.parse_list("#affected+f", "#inneed+f")
+
+        Args:
+            specs: the raw input (a list of strings, or a single string with commas separating the patterns)
+
+        Returns:
+            A list of TagPattern objects.
+
         """
         if not specs:
             return []
         if isinstance(specs, six.string_types):
             specs = specs.split(',')
         return [TagPattern.parse(spec) for spec in specs]
 
     @staticmethod
     def match_list(column, patterns):
         """Test if a column matches any of the patterns in a list.
-        @param column: the column to test
-        @param patterns: a list of zero or more patterns.
-        @returns: True if there is a match
+
+        This is convenient to use together with [parse_list()](hxl.model.TagPattern.parse_list):
+
+            patterns = TagPattern.parse_list(["#affected+f", "#inneed+f"])
+            if TagPattern.match_list(column, patterns):
+                print("The column matched one of the patterns")
+
+        Args:
+            column: the column to test
+            patterns: a list of zero or more patterns.
+
+        Returns:
+            True if there is a match
+
         """
         for pattern in patterns:
             if pattern.match(column):
                 return True
         return False
 
 
@@ -215,14 +283,60 @@
     def columns(self):
         """Get the column definitions for the dataset.
         @returns: a list of Column objects.
         """
         raise RuntimeException("child class must implement columns property method")
 
     @property
+    def columns_hash(self):
+        """Generate a hash across all of the columns in the dataset.
+
+        This function helps detect whether two HXL documents are of
+        the same type, even if they contain different data (e.g. the
+        HXL API output for the same humanitarian dataset in two
+        different months or two different countries).
+
+        It takes into account text headers, hashtags, the order of
+        attributes, and the order of columns. Whitespace is
+        normalised, and null values are treated as empty strings. The
+        MD5 hash digest is generated from a UTF-8 encoded version of
+        each header.
+
+        @returns: a 32-character hex-formatted MD5 hash string
+
+        """
+        return hxl.Column.hash_list(self.columns)
+
+    @property
+    def data_hash(self):
+        """Generate a hash for the entire dataset.
+
+        This function allows checking if two HXL datasets are
+        functionally identical. It takes into account text headers,
+        hashtags, the order of attributes, and the order of
+        columns. Whitespace is normalised, and null values are treated
+        as empty strings. The MD5 hash digest is generated from a
+        UTF-8 encoded version of each header and data cell.
+
+        @returns: a 32-character hex-formatted MD5 hash string
+        """
+        md5 = hashlib.md5()
+        # text header row
+        for column in self.columns:
+            md5.update(hxl.datatypes.normalise_space(column.header).encode('utf-8'))
+        # hashtag row
+        for column in self.columns:
+            md5.update(hxl.datatypes.normalise_space(column.display_tag).encode('utf-8'))
+        # data rows
+        for row in self:
+            for value in row:
+                md5.update(hxl.datatypes.normalise_space(value).encode('utf-8'))
+        return md5.hexdigest()
+
+    @property
     def headers(self):
         """Return a list of header strings (for a spreadsheet row).
         """
         return [column.header if column else '' for column in self.columns]
 
     @property
     def tags(self):
@@ -274,57 +388,72 @@
             if normalise:
                 new_values = [hxl.datatypes.normalise(s) for s in new_values]
             else:
                 new_values = [hxl.datatypes.normalise_space(s) for s in new_values]
             value_set.update(new_values)
         return value_set
 
+
+    def get_column_indices(self, tag_patterns, columns):
+        """Get a list of indices that match the tag patterns provided
+        @param tag_patterns: a list of tag patterns or a string version of the list
+        @param columns: a list of columns
+        @returns: a (possibly-empty) list of 0-based indices
+        """
+        patterns = TagPattern.parse_list(tag_patterns)
+        indices = []
+        for i, column in enumerate(columns):
+            for pattern in patterns:
+                if pattern.match(column):
+                    indices.push(i)
+        return indices
+
     #
     # Aggregates
     #
 
     def _get_minmax(self, pattern, op):
         """Calculate the extreme min/max value for a tag pattern
         Will iterate through the dataset, and use values from multiple matching columns.
         Uses numbers, dates, or strings for comparison, based on the first non-empty value found.
         @param pattern: the L{hxl.model.TagPattern} to match
         @param op: operator_lt or operator_gt
-        @returns: the minimum value according to the '<' operator, or None if no values found
+        @returns: the extreme value according to operator supplied, or None if no values found
         """
         pattern = TagPattern.parse(pattern)
-        target_value = None
-        type = None
+        result_raw = None # what's actually in the dataset
+        result_normalised = None # normalised version for comparison
+
+        # Look at every row
         for row in self:
-            for value in row.get_all(pattern):
-                value = hxl.datatypes.normalise_string(value)
+            # Look at every matching value in every row
+            for i, value in enumerate(row.get_all(pattern)):
+                # ignore empty values
                 if hxl.datatypes.is_empty(value):
-                    continue # don't care about empty cells
-                if pattern.tag == '#date' or type == 'date':
-                    if re.match(r'^\d\d\d\d$', value):
-                        # special case for year
-                        type = 'date'
-                    else:
-                        if hxl.datatypes.is_date(value):
-                            value = hxl.datatypes.normalise_date(value)
-                            type = 'date'
-                if type is None or type == 'number':
+                    continue
+
+                # make a normalised value for comparison
+                normalised = hxl.datatypes.normalise(value, row.columns[i])
+
+                # first non-empty value is always a match
+                if result_normalised is None:
+                    result_raw = value
+                    result_normalised = normalised
+                else:
+                    # try comparing the normalised types first, then strings on failure
                     try:
-                        value = float(value)
-                        type = 'number'
-                    except ValueError:
-                        if type == 'number': # not a number
-                            value = None
-                if type is None:
-                    type = 'string'
-                    value = str(value)
-                if value is not None:
-                    if target_value is None or op(value, target_value):
-                        target_value = value
-        return target_value
-        
+                        if op(normalised, result_normalised):
+                            result_raw = value
+                            result_normalised = normalised
+                    except TypeError:
+                        if op(str(normalised), str(result_normalised)):
+                            result_raw = value
+                            result_normalised = normalised
+
+        return result_raw
 
     def min(self, pattern):
         """Calculate the minimum value for a tag pattern
         Will iterate through the dataset, and use values from multiple matching columns.
         Uses numbers, dates, or strings for comparison, based on the first non-empty value found.
         @param pattern: the L{hxl.model.TagPattern} to match
         @returns: the minimum value according to the '<' operator, or None if no values found
@@ -360,37 +489,57 @@
         return hxl.filters.from_recipe(self, recipe)
 
     #
     # Filters
     #
 
     def append(self, append_sources, add_columns=True, queries=[]):
-        """Append a second dataset."""
+        """Append additional datasets.
+        @param append_sources: a list of sources to append
+        @param add_columns: if True (default), include any extra columns in the append sources
+        @param queries: a list of row queries to select rows for inclusion from the append sources.
+        @returns: a new HXL source for chaining
+        """
+        import hxl.filters
+        return hxl.filters.AppendFilter(self, append_sources, add_columns=add_columns, queries=queries)
+
+    def append_external_list(self, source_list_url, add_columns=True, queries=[]):
+        """Append additional datasets from an external list
+        @param source_list_url: URL of a HXL dataset containing a list of sources to append.
+        @param add_columns: if True (default), include any extra columns in the append sources.
+        @param queries: a list of row queries to select rows for inclusion from the append sources.
+        @returns: a new HXL source for chaining
+        """
         import hxl.filters
+        logup('Loading append list', {"list": source_list_url}, level='debug')
+        logger.debug("Loading append list from %s...", source_list_url)
+        append_sources = hxl.filters.AppendFilter.parse_external_source_list(source_list_url)
+        logup('Done loading', {"list": source_list_url}, level='debug')
+        logger.debug("Done loading")
         return hxl.filters.AppendFilter(self, append_sources, add_columns=add_columns, queries=queries)
 
     def cache(self):
         """Add a caching filter to the dataset."""
         import hxl.filters
         return hxl.filters.CacheFilter(self)
 
     def dedup(self, patterns=[], queries=[]):
         """Deduplicate a dataset."""
         import hxl.filters
         return hxl.filters.DeduplicationFilter(self, patterns=patterns, queries=queries)
 
-    def with_columns(self, whitelist):
+    def with_columns(self, includes):
         """Select matching columns."""
         import hxl.filters
-        return hxl.filters.ColumnFilter(self, include_tags=whitelist)
+        return hxl.filters.ColumnFilter(self, include_tags=includes)
 
-    def without_columns(self, blacklist=None, skip_untagged=False):
+    def without_columns(self, excludes=None, skip_untagged=False):
         """Select non-matching columns."""
         import hxl.filters
-        return hxl.filters.ColumnFilter(self, exclude_tags=blacklist, skip_untagged=skip_untagged)
+        return hxl.filters.ColumnFilter(self, exclude_tags=excludes, skip_untagged=skip_untagged)
 
     def with_rows(self, queries, mask=[]):
         """Select matching rows.
         @param queries: a predicate or list of predicates for rows to include
         @param mask: a predicate or list of predicates for rows to test (default: [] to test all)
         @return: a filtered version of the source
         """
@@ -458,42 +607,69 @@
             lower=lower,
             date=date, date_format=date_format,
             number=number, number_format=number_format,
             latlon=latlon,
             purge=purge,
             queries=queries
         )
-    
+
     def merge_data(self, merge_source, keys, tags, replace=False, overwrite=False, queries=[]):
-        """Merges values from a second dataset."""
+        """Merges values from a second dataset.
+        @param merge_source: the second HXL data source
+        @param keys: a single tagspec or list of tagspecs for the shared keys
+        @param tags: the tags to copy over from the second dataset
+        @param replace: if True, replace existing columns when present
+        @param overwrite: if True, overwrite individual values in existing columns when available
+        @param queries: optional row queries to control the merge
+        """
         import hxl.filters
         return hxl.filters.MergeDataFilter(self, merge_source, keys, tags, replace, overwrite, queries=queries)
 
+    def expand_lists(self, patterns=None, separator="|", correlate=False, queries=[]):
+        """Expand lists by repeating rows.
+        By default, applies to every column with a +list attribute, and uses "|" as the separator.
+        @param patterns: a single tag pattern or list of tag patterns for columns to expand
+        @param separator: the list-item separator
+        """
+        import hxl.filters
+        return hxl.filters.ExpandListsFilter(self, patterns=patterns, separator=separator, correlate=correlate, queries=queries)
+
     def explode(self, header_attribute='header', value_attribute='value'):
         """Explodes a wide dataset into a long datasets.
         @param header_attribute: the attribute to add to the hashtag of the column with the former header (default 'header')
         @param value_attribute: the attribute to add to the hashtag of the column with the former value (default 'value')
         @return: filtered dataset.
         @see hxl.filters.ExplodeFilter
         """
-        
+
         import hxl.filters
         return hxl.filters.ExplodeFilter(self, header_attribute, value_attribute)
 
-    def jsonpath(self, path, patterns=[], queries=[]):
+    def implode(self, label_pattern, value_pattern):
+        """Implodes a long dataset into a wide dataset
+        @param label_pattern: the tag pattern to match the label column
+        @param value_pattern: the tag pattern to match the
+        @return: filtered dataset.
+        @see hxl.filters.ImplodeFilter
+        """
+        import hxl.filters
+        return hxl.filters.ImplodeFilter(self, label_pattern=label_pattern, value_pattern=value_pattern)
+
+    def jsonpath(self, path, patterns=[], queries=[], use_json=True):
         """Parse the value as a JSON expression and extract data from it.
         See http://goessner.net/articles/JsonPath/
         @param path: a JSONPath expression for extracting data
         @param patterns: a tag pattern or list of patterns for the columns to use (default to all)
         @param queries: a predicate or list of predicates for the rows to consider.
+        @param use_json: if True, serialise multiple results as JSON lists.
         @returns: filtered dataset
         @see: hxl.filters.JSONPathFilter
         """
         import hxl.filters
-        return hxl.filters.JSONPathFilter(self, path, patterns=patterns, queries=queries)
+        return hxl.filters.JSONPathFilter(self, path, patterns=patterns, queries=queries, use_json=use_json)
 
     def fill_data(self, patterns=[], queries=[]):
         """Fills empty cells in a column using the last non-empty value.
         @param patterns: a tag pattern or list of patterns for the columns to fill (default to all)
         @param queries: a predicate or list of predicates for rows to fill (leave any blank that don't match).
         @return filtered dataset
         @see hxl.filters.FillFilter
@@ -552,15 +728,15 @@
                     yield ",\n" + json.dumps(raw)
         yield "\n]\n"
 
 
 class Column(object):
     """
     The definition of a logical column in the HXL data.
-    """ 
+    """
 
     # Regular expression to match a HXL tag
     PATTERN = r'^\s*(#{token})((?:\s*\+{token})*)\s*$'.format(token=hxl.datatypes.TOKEN_PATTERN)
 
     # To tighten debugging (may reconsider later -- not really a question of memory efficiency here)
     __slots__ = ['tag', 'attributes', 'attribute_list', 'header', 'column_number']
 
@@ -582,15 +758,15 @@
 
     @property
     def display_tag(self):
         """Default display version of a HXL hashtag.
         Attributes are not sorted.
         """
         return self.get_display_tag(sort_attributes=False)
-    
+
     def get_display_tag(self, sort_attributes=False):
         """
         Generate a display version of the column hashtag
         @param sort_attributes: if True, sort attributes; otherwise, preserve the original order
         @return the reassembled HXL hashtag string, including language code
         """
         if self.tag:
@@ -638,55 +814,140 @@
 
     def __repr__(self):
         return self.display_tag
 
     __str__ = __repr__
 
     @staticmethod
-    def parse(raw_string, header=None, use_exception=False, column_number=None):
+    def hash_list(columns):
+        """Generate a hash across all of the columns in the dataset.
+
+        This function helps detect whether two HXL documents are of
+        the same type, even if they contain different data (e.g. the
+        HXL API output for the same humanitarian dataset in two
+        different months or two different countries).
+
+        It takes into account text headers, hashtags, the order of
+        attributes, and the order of columns. Whitespace is
+        normalised, and null values are treated as empty strings. The
+        MD5 hash digest is generated from a UTF-8 encoded version of
+        each header.
+
+        @returns: a 32-character hex-formatted MD5 hash string
+
         """
-        Attempt to parse a full hashtag specification.
+        md5 = hashlib.md5()
+        for column in columns:
+            md5.update(hxl.datatypes.normalise_space(column.header).encode('utf-8'))
+        for column in columns:
+            md5.update(hxl.datatypes.normalise_space(column.display_tag).encode('utf-8'))
+        return md5.hexdigest()
+
+    @staticmethod
+    def parse(raw_string, header=None, use_exception=False, column_number=None):
+        """ Attempt to parse a full hashtag specification.
+        @param raw_string: the string representation of the tagspec
+        @param header: the text header to include
+        @param use_exception: if True, throw an exception for a malformed tagspec
+        @returns: None if the string is empty, False if it's malformed (and use_exception is False), or a Column object otherwise
         """
+
         # Already parsed?
         if isinstance(raw_string, Column):
             return raw_string
-        
+
+        # Empty string?
+        if hxl.datatypes.is_empty(raw_string):
+            return None
+
         # Pattern for a single tag
         result = re.match(Column.PATTERN, raw_string)
         if result:
             tag = result.group(1)
             attribute_string = result.group(2)
             if attribute_string:
                 attributes = re.split(r'\s*\+', attribute_string.strip().strip('+'))
             else:
                 attributes = []
             return Column(tag=tag, attributes=attributes, header=header, column_number=column_number)
         else:
             if use_exception:
                 raise hxl.HXLException("Malformed tag expression: " + raw_string)
             else:
-                return None
+                logup('Not a HXL hashtag spec', {"string": raw_string}, level='debug')
+                logger.debug("Not a HXL hashtag spec: %s", raw_string)
+                return False
 
     @staticmethod
     def parse_spec(raw_string, default_header=None, use_exception=False, column_number=None):
         """Attempt to parse a single-string header/hashtag spec"""
         # Already parsed?
         if isinstance(raw_string, Column):
             return raw_string
-        
+
         matches = re.match(r'^(.*)(#.*)$', raw_string)
         if matches:
             header = matches.group(1) if matches.group(1) else default_header
             return Column.parse(matches.group(2), header=header, column_number=column_number)
         else:
             return Column.parse('#' + raw_string, header=default_header, column_number=column_number)
 
+    @staticmethod
+    def parse_list(raw_row, previous_row=None):
+        """Try parsing a raw data row as a HXL hashtag row.
+
+        Args:
+            raw_row (list): a raw row from a ``hxl.input.AbstractInput`` object
+            previous_row (list): the previous raw row, for extracting headers
+
+        Returns:
+            list: a list of hxl.model.Column objects if successfully parsed; None otherwise.
+
+        """
+        # how many values we've seen
+        nonEmptyCount = 0
+
+        # the logical column number
+        hashtags_found = 0
+
+        columns = []
+        failed_hashtags = []
+
+        for source_column_number, raw_string in enumerate(raw_row):
+            if previous_row and source_column_number < len(previous_row):
+                header = previous_row[source_column_number]
+            else:
+                header = None
+            if not hxl.datatypes.is_empty(raw_string):
+                raw_string = hxl.datatypes.normalise_string(raw_string)
+                nonEmptyCount += 1
+                column = hxl.model.Column.parse(raw_string, header=header, column_number=source_column_number)
+                if column:
+                    columns.append(column)
+                    hashtags_found += 1
+                    continue
+                elif column is False:
+                    failed_hashtags.append(raw_string)
+
+            columns.append(hxl.model.Column(header=header, column_number=source_column_number))
+
+        # Have we seen at least FUZZY_HASHTAG_PERCENTAGE?
+        if (nonEmptyCount > 0) and ((hashtags_found/float(nonEmptyCount)) >= FUZZY_HASHTAG_PERCENTAGE):
+            if len(failed_hashtags) > 0:
+                logup('Skipping column(s) with malformed hashtag specs', {"hastags": ', '.join(failed_hashtags)}, level='error')
+                logger.error('Skipping column(s) with malformed hashtag specs: %s', ', '.join(failed_hashtags))
+            return columns
+        else:
+            return None
+
+
 class Row(object):
-    """
-    An iterable row of values in a HXL dataset.
+    """ An iterable row of values in a HXL dataset.
+
+    If a value is part of a merged area, and not in the top left position, it will be a MergedCell object.
     """
 
     # Predefine the slots for efficiency (may reconsider later)
     __slots__ = ['columns', 'values', 'row_number', 'source_row_number']
 
     def __init__(self, columns, values=[], row_number=None, source_row_number=None):
         """
@@ -721,15 +982,15 @@
         @return The value found, or the default value provided. If parsed=True, the return value will be a list (default: False)
         """
 
         # FIXME - move externally, use for get_all as well, and support numbers and dates
         def parse(column, value):
             if parsed:
                 if column.has_attribute('list'):
-                    return re.split("\s*,\s*", value)
+                    return re.split(r'\s*,\s*', value)
                 else:
                     return [value]
             return value
 
         if type(tag) is TagPattern:
             pattern = tag
         else:
@@ -771,35 +1032,38 @@
             if pattern.match(column):
                 value = self.values[i]
                 if default is not None and not value:
                     value = default
                 result.append(value)
         return result
 
-    def key(self, patterns=None):
+    def key(self, patterns=None, indices=None):
         """Generate a unique key tuple for the row, based on a list of tag patterns
         @param patterns: a list of L{TagPattern} objects, or a parseable string
         @returns: the key as a tuple (might be empty)
         """
-        if patterns:
-            patterns = TagPattern.parse_list(patterns)
-
-        def in_key(col):
-            if not patterns:
-                return True
-            for pattern in patterns:
-                if pattern.match(col):
-                    return True
-            return False
 
         key = []
-        for i, value in enumerate(self.values):
-            if i < len(self.columns) and in_key(self.columns[i]):
+
+        # if the user doesn't provide indices, get indices from the pattern
+        if not indices and patterns:
+            indices = get_column_indices(patterns, self.columns)
+
+        if indices:
+            # if we have indices, use them to build the key
+            for i in indices:
+                if i < len(self.values):
+                    key.append(hxl.datatypes.normalise(self.values[i], self.columns[i]))
+        else:
+            # if there are still no indices, use the whole row for the key
+            for i, value in enumerate(self.values):
                 key.append(hxl.datatypes.normalise(value, self.columns[i]))
-        return tuple(key)
+
+        return tuple(key) # make it into a tuple so that it's hashable
+
 
     @property
     def dictionary(self):
         """Return the row as a Python dict.
         The keys will be HXL hashtags and attributes, normalised per HXL 1.1.
         If two or more columns have the same hashtags and attributes, only the first will be included.
         @return: The row as a Python dictionary.
@@ -841,32 +1105,39 @@
         @param value: the value to compare against
         @param is_aggregate: if True, the value is a special placeholder like "min" or "max" that needs to be calculated
         """
         self.pattern = TagPattern.parse(pattern)
         self.op = op
         self.value = value
 
+        # if the value is a formula, extract it
+        self.formula = None
+        result = re.match(r'^{{(.+)}}$', hxl.datatypes.normalise_space(value))
+        if result:
+            self.formula = result.group(1)
+
         self.is_aggregate=is_aggregate
         self.needs_aggregate = False
         """Need to calculate an aggregate value"""
-        
+
         if is_aggregate:
             self.needs_aggregate = True
 
         # calculate later
         self.date_value = None
         self.number_value = None
         self._saved_indices = None
 
     def calc_aggregate(self, dataset):
         """Calculate the aggregate value that we need for the row query
         Substitute the special values "min" and "max" with aggregates.
         @param dataset: the HXL dataset to use (must be cached)
         """
         if not self.needs_aggregate:
+            logup('no aggregate calculation needed', level='warning')
             logger.warning("no aggregate calculation needed")
             return # no need to calculate
         if not dataset.is_cached:
             raise HXLException("need a cached dataset for calculating an aggregate value")
         if self.value == 'min':
             self.value = dataset.min(self.pattern)
             self.op = operator.eq
@@ -878,44 +1149,67 @@
             self.op = operator.ne
         elif self.value == 'not max':
             self.value = dataset.max(self.pattern)
             self.op = operator.ne
         else:
             raise HXLException("Unrecognised aggregate: {}".format(value))
         self.needs_aggregate = False
-                               
+
     def match_row(self, row):
         """Check if a key-value pair appears in a HXL row"""
 
         # fail if we need an aggregate and haven't calculated it
         if self.needs_aggregate and not self.aggregate_is_calculated:
             raise HXLException("must call calc_aggregate before matching an 'is min' or 'is max' condition")
 
         # initialise is this is the first time matching for the row query
-        if self._saved_indices is None:
-            if self.pattern.tag == '#date' and hxl.datatypes.is_date(self.value):
-                self.date_value = hxl.datatypes.normalise_date(self.value)
-            elif hxl.datatypes.is_number(self.value):
-                self.number_value = hxl.datatypes.normalise_number(self.value)
+        if self._saved_indices is None or self.formula:
+
+            # if it's a row formula, evaluate first
+            if self.formula:
+                value = hxl.formulas.eval.eval(row, self.formula)
+            else:
+                value = self.value
+
+            if self.pattern.tag == '#date':
+                try:
+                    self.date_value = hxl.datatypes.normalise_date(value)
+                except ValueError:
+                    self.date_value = None
+
+            try:
+                self.number_value = hxl.datatypes.normalise_number(value)
+            except ValueError:
+                self.number_value = None
+
+            self.string_value = hxl.datatypes.normalise_string(value)
 
         # try all the matching column values
         indices = self._get_saved_indices(row.columns)
         for i in indices:
             if i < len(row.values) and self.match_value(row.values[i], self.op):
                 return True
         return False
 
+
     def match_value(self, value, op):
         """Try matching as dates, then as numbers, then as simple strings"""
-        if self.date_value is not None and hxl.datatypes.is_date(value):
-            return op(hxl.datatypes.normalise_date(value), self.date_value)
-        elif self.number_value is not None and hxl.datatypes.is_number(value):
-            return op(hxl.datatypes.normalise_number(value), self.number_value)
-        else:
-            return self.op(hxl.datatypes.normalise_string(value), hxl.datatypes.normalise_string(self.value))
+        if self.date_value is not None:
+            try:
+                return op(hxl.datatypes.normalise_date(value), self.date_value)
+            except ValueError:
+                pass
+
+        if self.number_value is not None:
+            try:
+                return op(hxl.datatypes.normalise_number(value), self.number_value)
+            except:
+                pass
+
+        return self.op(hxl.datatypes.normalise_string(value), self.string_value)
 
     def _get_saved_indices(self, columns):
         """Cache the column tests, so that we run them only once."""
         # FIXME - assuming that the columns never change
         self._saved_indices = []
         for i in range(len(columns)):
             if self.pattern.match(columns[i]):
@@ -990,27 +1284,45 @@
             return not hxl.datatypes.is_number(s)
         elif condition == 'date':
             return (hxl.datatypes.is_date(s))
         elif condition == 'not date':
             return (hxl.datatypes.is_date(s) is False)
         else:
             raise hxl.HXLException('Unknown is condition: {}'.format(condition))
-    
+
 
     # Constant map of comparison operators
     OPERATOR_MAP = {
         '=': operator.eq,
         '!=': operator.ne,
         '<': operator.lt,
         '<=': operator.le,
         '>': operator.gt,
         '>=': operator.ge,
     }
 
 
+# Static functions
+
+def get_column_indices(tag_patterns, columns):
+    """Get a list of column indices that match the tag patterns provided
+    @param tag_patterns: a list of tag patterns or a string version of the list
+    @param columns: a list of columns
+    @returns: a (possibly-empty) list of 0-based indices
+    """
+    tag_patterns = TagPattern.parse_list(tag_patterns)
+    columns = [Column.parse(column) for column in columns]
+    indices = []
+    for i, column in enumerate(columns):
+        for pattern in tag_patterns:
+            if pattern.match(column):
+                indices.append(i)
+    return indices
+
+
 # Extra static initialisation
 RowQuery.OPERATOR_MAP['~'] = RowQuery.operator_re
 RowQuery.OPERATOR_MAP['!~'] = RowQuery.operator_nre
 RowQuery.OPERATOR_MAP['is'] = RowQuery.operator_is
 
 
 # end
```

### Comparing `libhxl-4.9/hxl/converters.py` & `libhxl-5.0/hxl/converters.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,69 @@
 """Data-conversion classes
 
 This module holds classes for converting to HXL from other formats, or
-from HXL to other formats. Current, the only class is L{Tagger} (for
-adding tags to non-HXL tabular data on the fly), but we will add more
-converters soon, especially for formats like GeoJSON.
-
-@author: David Megginson
-@organization: UNOCHA
-@license: Public Domain
-@date: Started April 2015
-@see: U{http://hxlstandard.org}
+from HXL to other formats. Current, the only class is ``Tagger`` (for
+adding tags to non-HXL tabular data on the fly), but we may add more
+converters, especially for formats like GeoJSON.
+
+Author:
+    David Megginson
+
+License:
+    Public Domain
+
 """
 
 import hxl
 import logging, re
 
 
 logger = logging.getLogger(__name__)
 
 
-class Tagger(hxl.io.AbstractInput):
-    """Add HXL hashtags to a CSV-like input stream.
-
-    Usage::
-    
-      input = open('data.csv', 'r')
-      specs = [('Cluster', '#sector'), ('Organi', '#org'), ('province', '#adm1+es')]
-      tagger = Tagger(input, specs)
+class Tagger(hxl.input.AbstractInput):
+    """Add HXL hashtags to a non-HXL datasource on the fly.
 
-    The tagger object acts as a L{hxl.io.AbstractInput} source, which you can
-    use with the L{hxl.data} function like this::
-
-      source = hxl.data(Tagger(input, specs)).with_rows('org=unicef').sort()
+    Example:
+    ```
+    input = hxl.input.make_input(url_or_filename)
+    specs = [('Cluster', '#sector'), ('Organi', '#org'), ('province', '#adm1+es')]
+    dataset = hxl.converters.Tagger(input, specs)
+    ```
+
+    The more-common way to invoke the tagger is through the
+    ``hxl.input.tagger()`` function:
+
+    ```
+    dataset = hxl.input.tagger(url_or_filename, specs)
+    ```
 
     """
 
     def __init__(self, input, specs=[], default_tag=None, match_all=False):
         """Construct a new Tagger object.
 
         The input spec is a list of tuples, where the first item is a
         substring to match (case-/space-/punctuation-insensitive), and
-        the second item is the HXL tag spec to use. Example::
-
-          [('Cluster', '#sector'), ('Organi', '#org'), ('province', '#adm1+es')]
+        the second item is the HXL tag spec to use.
 
-        @param input: an input stream of some kind
-        @param specs: the input specs, as described above (default: [])
-        @param match_all: if True, require that the full header string match; otherwise, match substrings (default: False)
-        @param default_tag: default tagspec to use for any column without a match
+        Example:
+        ```
+        spec = [
+            ['Cluster', '#sector'],
+            ['Organisation', '#org'],
+            ['Province', '#adm1+es']
+        ]
+        ```
+
+        Args:
+            input (hxl.input.AbstractInput): an input source that can yield rows of values (see ``hxl.input.make_input``).
+            specs (dict): the input specs, as described above (default: [])
+             match_all (bool): if True, require that the full header string match; otherwise, match substrings (default: False)
+            default_tag (str): default tagspec to use for any column without a match
         """
         if isinstance(specs, dict):
             # convert to list of tuples if needed
             specs = [(key, specs[key]) for key in specs]
         self.specs = [(hxl.datatypes.normalise_string(spec[0]), spec[1]) for spec in specs]
         self.default_tag = default_tag
         self.match_all = match_all
@@ -76,15 +88,15 @@
 
     def _add_tags(self):
         """Look for headers in the first 25 rows of data.
         @return: True if headers were found matching the tagging specs; False otherwise.
         """
         for n in range(0, 25):
             raw_row = next(self.input)
-            if not raw_row:
+            if raw_row is None:
                 break
             self._cache.append(raw_row)
             tag_row = self._try_tag_row(raw_row)
             if tag_row:
                 self._cache.append(tag_row)
                 return True
         return False
@@ -133,41 +145,58 @@
         return self
 
     _SPEC_PATTERN = r'^(.+)(#{token}([+]{token})*)$'.format(token=hxl.datatypes.TOKEN_PATTERN)
     """Regular-expression pattern for matching a tagging specification as a string"""
 
     @staticmethod
     def parse_spec(s):
-        """Try parsing a tagger spec (used only by the command-line tools)
-        Uses Tagger._SPEC_PATTERN
-        @param s: the string representing a tagging specification
-        @return: the parsed specification
-        @exception HXLFilterException: if there is an error parsing the spec
+        """Parse a JSON-like tagger spec
+
+        The string is in the format "HEADER TEXT#hashtag+attributes"
+
+        Example:
+        ```
+        spec = hxl.converters.Tagger.parse_spec("Organisation name#org+name")
+        ```
+
+        Used only by the command-line tools.
+
+        Args:
+            s (str): the string representing a tagging specification
+
+        Returns:
+            hxl.model.Column: the parsed specification as a column object (header, hashtags, and attributes)
+
+        Raises:
+            hxl.filters.HXLFilterException: if there is an error parsing the spec
+
         """
         result = re.match(Tagger._SPEC_PATTERN, s)
         if result:
             return (result.group(1), hxl.model.Column.parse(result.group(2), use_exception=True).display_tag)
         else:
             raise HXLFilterException("Bad tagging spec: " + s)
 
     @staticmethod
     def _load(input, spec):
         """Create a tagger from a dict spec.
-        Example spec:
+
+        Example:
+        ```
         {
-          "match_all": False,
+          "match_all": false,
           "default_tag": "#affected+label",
           "specs": [
-            ('district', '#adm1+name',),
-            ('p-code', '#adm1+code+v_pcode',),
-            ('organi', '#org+name',),
+            ["district", "#adm1+name"],
+            ["p-code", "#adm1+code+v_pcode"],
+            ["organi", "#org+name"]
           ]
         }
-        @param spec: the dictionary specification
-        @return: a Tagger object
+        ```
+
         """
         return Tagger(
             input=input,
             specs=spec.get('specs', []),
             default_tag=spec.get('default_tag', None),
             match_all=spec.get('match_all', False)
         )
```

### Comparing `libhxl-4.9/hxl/hxl-default-schema.json` & `libhxl-5.0/hxl/hxl-default-schema.json`

 * *Files identical despite different names*

### Comparing `libhxl-4.9/hxl/__init__.py` & `libhxl-5.0/hxl/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,121 @@
-"""Support library for the Humanitarian Exchange Language (HXL), version 1.0.
+"""Support library for the Humanitarian Exchange Language (HXL), version 1.1.
 
 This library provides support for parsing, validating, cleaning, and
-transforming humanitarian datasets that follow the HXL standard. Its
-use will be familiar to developers who have worked with libraries like
-U{JQuery<https://jquery.com>}.  Here's an example::
-
-  import hxl
-  data = hxl.data('data.xlsx', True).with_rows('org=UNICEF').without_columns('contact').count('country')
+transforming humanitarian datasets that follow the [HXL
+standard](https://hxlstandard.org). Its use will be familiar to
+developers who have worked with libraries like
+[JQuery](https://jquery.com).
+
+### Example
+
+```
+import hxl
+data = hxl.data('data.xlsx', True).with_rows('org=UNICEF').without_columns('contact').count('country')
+```
 
 This two-line script performs the following actions:
 
-  1. Load and parse the spreadsheet C{data.xlsx} (the library can also
-     load from any URL, and understands how to read Google
-     spreadsheets or U{CKAN<http://ckan.org>} resources).
+  1. Load and parse the spreadsheet ``data.xlsx`` (the library can
+     also load from any URL, and understands how to read Google
+     spreadsheets or [CKAN](http://ckan.org) resources).
 
   2. Filter out all rows where the value "UNICEF" doesn't appear under
-     the C{#org} (organisation) hashtag.
+     the ``#org`` (organisation) hashtag.
 
   3. Strip out personally-identifiable information by removing all
-     columns with the C{#contact} hashtag (e.g. C{#contact+name},
-     C{#contact+phone}, C{#contact+email}).
+     columns with the ``#contact`` hashtag (e.g. ``#contact+name`` or
+     ``#contact+phone`` or ``#contact+email``).
 
   4. Produce a report showing the number of times each unique
-     C{#country} appears in the resulting sheet (e.g. to count the number
-     of activities being conducted by UNICEF in each country).
+     ``#country`` appears in the resulting sheet (e.g. to count the
+     number of activities being conducted by UNICEF in each country).
+
+### Command-line scripts
+
+The various filters are also available
+as command-line scripts, so you could perform the same actions as
+above in a shell script like this:
+
+```
+$ cat data.xlsx | hxlselect -q 'org=UNICEF' | hxlcut -x contact | hxlcount -t country
+```
+
+For more information about scripts, see the documentation for
+`hxl.scripts`, or invoke any script with the ``-h`` option.
+
+### Imports
+
+Several identifiers are imported into this top-level package for
+typing convenience, including `hxl.model.TagPattern`,
+`hxl.model.Dataset`, `hxl.model.Column`, `hxl.model.Row`,
+`hxl.model.RowQuery`, `hxl.input.data`, `hxl.input.tagger`,
+`hxl.input.HXLParseException`, `hxl.input.write_hxl`,
+`hxl.input.make_input`, `hxl.input.InputOptions`,
+`hxl.input.from_spec`, `hxl.validation.schema`,
+`hxl.validation.validate`, and
+`hxl.validation.HXLValidationException`.
+
+### Next steps
+
+To get started, read the documentation for the `hxl.input.data` function and
+the `hxl.model.Dataset` class. 
+
+### About this module
+
+**Author:** David Megginson
+
+**Organisation:** UN OCHA
+
+**License:** Public Domain
+
+**Started:** Started August 2014
+
+**GitHub:** https://github.com/HXLStandard/libhxl-python
+
+**PyPi:** https://pypi.org/project/libhxl/
 
-To get started, read the documentation for the L{hxl.data} function
-and the L{hxl.model.Dataset} class. The various filters are also
-available as command-line scripts, so you could perform the same
-actions as above in a shell script like this::
-
-  $ cat data.xlsx | hxlselect -q 'org=UNICEF' | hxlcut -x contact | hxlcount -t country
-
-@author: David Megginson
-@organization: UNOCHA
-@license: Public Domain
-@date: Started August 2014
-@see: U{http://hxlstandard.org} for the HXL data standard
-@see: U{https://proxy.hxlstandard.org} for web-based deployment of this library
 """
 
 import sys
 
 if sys.version_info < (3,):
     raise RuntimeError("libhxl requires Python 3 or higher")
 
-__version__="4.9"
+__version__="5.0"
 """Module version number
 see https://www.python.org/dev/peps/pep-0396/
 """
 
 # Flatten out common items for easier access
 
 class HXLException(Exception):
     """Base class for all HXL-related exceptions."""
 
     def __init__(self, message, data={}):
         """Create a new HXL exception.
 
-        @param message: error message for the exception
-        @param data: dict of properties associated with the exception (default {})
+        Args:
+            message (str): error message for the exception
+            data (dict): properties associated with the exception (default {})
         """
         super(Exception, self).__init__(message)
 
         self.message = message
         """The human-readable error message."""
 
         self.data = data
         """Additional properties related to the error."""
 
     def __str__(self):
-        return "<HXLException: " + str(self.message) + ">"
+        return "<{}: {}>".format(type(self).__name__, str(self.message))
 
 import hxl.geo
 import hxl.datatypes
 from hxl.model import TagPattern, Dataset, Column, Row, RowQuery
-from hxl.io import data, tagger, HXLParseException, write_hxl, make_input, from_spec
+from hxl.input import data, info, tagger, HXLParseException, write_hxl, make_input, InputOptions, from_spec
 from hxl.validation import schema, validate, HXLValidationException
 
 # end
```

