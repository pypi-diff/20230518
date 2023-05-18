# Comparing `tmp/xmlable-1.0.1.tar.gz` & `tmp/xmlable-1.1.0.tar.gz`

## Comparing `xmlable-1.0.1.tar` & `xmlable-1.1.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 xmlable-1.0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/basic_config/config.xsd
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/basic_config/config_xml_example.xml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/basic_config/config_xml_template.xml
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/basic_config/main.py
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/complex/config.xsd
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/complex/config_xml_example.xml
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/complex/config_xml_template.xml
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/complex/main.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/invalid/main.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/maps/config.xsd
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/maps/config_xml_example.xml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/maps/config_xml_template.xml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/maps/main.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/namespaces/config.xsd
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/namespaces/config_xml_example.xml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/namespaces/config_xml_template.xml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/namespaces/main.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/userdefined/config.xsd
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/userdefined/config_xml_example.xml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/userdefined/config_xml_template.xml
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/userdefined/main.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/_errors.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/_io.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/_lxml_helpers.py
--rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/_manual.py
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/_user.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/_utils.py
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/_xmlify.py
--rw-r--r--   0        0        0    23007 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/_xobject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/py.typed
--rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 xmlable-1.0.1/tests/test_basic.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 xmlable-1.0.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 xmlable-1.0.1/LICENSE
--rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 xmlable-1.0.1/README.md
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 xmlable-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 xmlable-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 xmlable-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/basic_config/config.xsd
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/basic_config/config_xml_example.xml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/basic_config/config_xml_template.xml
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/basic_config/main.py
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/complex/config.xsd
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/complex/config_xml_example.xml
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/complex/config_xml_template.xml
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/complex/main.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/invalid/main.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/maps/config.xsd
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/maps/config_xml_example.xml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/maps/config_xml_template.xml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/maps/main.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/namespaces/config.xsd
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/namespaces/config_xml_example.xml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/namespaces/config_xml_template.xml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/namespaces/main.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/userdefined/config.xsd
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/userdefined/config_xml_example.xml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/userdefined/config_xml_template.xml
+-rw-r--r--   0        0        0     5383 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/userdefined/main.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/_errors.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/_io.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/_lxml_helpers.py
+-rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/_manual.py
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/_user.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/_utils.py
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/_xmlify.py
+-rw-r--r--   0        0        0    23209 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/_xobject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/py.typed
+-rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 xmlable-1.1.0/tests/test_basic.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 xmlable-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 xmlable-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 xmlable-1.1.0/README.md
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 xmlable-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xmlable-1.1.0/PKG-INFO
```

### Comparing `xmlable-1.0.1/.github/workflows/ci.yml` & `xmlable-1.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/examples/basic_config/config.xsd` & `xmlable-1.1.0/examples/basic_config/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/examples/basic_config/main.py` & `xmlable-1.1.0/examples/basic_config/main.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/examples/complex/config.xsd` & `xmlable-1.1.0/examples/complex/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/examples/complex/config_xml_example.xml` & `xmlable-1.1.0/examples/complex/config_xml_example.xml`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/examples/complex/config_xml_template.xml` & `xmlable-1.1.0/examples/complex/config_xml_template.xml`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/examples/complex/main.py` & `xmlable-1.1.0/examples/complex/main.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/examples/maps/config.xsd` & `xmlable-1.1.0/examples/maps/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/examples/maps/config_xml_example.xml` & `xmlable-1.1.0/examples/maps/config_xml_example.xml`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/examples/maps/config_xml_template.xml` & `xmlable-1.1.0/examples/maps/config_xml_template.xml`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/examples/maps/main.py` & `xmlable-1.1.0/examples/maps/main.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/examples/namespaces/config.xsd` & `xmlable-1.1.0/examples/namespaces/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/examples/namespaces/main.py` & `xmlable-1.1.0/examples/namespaces/main.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/examples/userdefined/config.xsd` & `xmlable-1.1.0/examples/userdefined/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/examples/userdefined/main.py` & `xmlable-1.1.0/examples/userdefined/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,18 +105,21 @@
         # if so we should use this prefix for type
         if (prefix := firstkey(add_ns, XMLURL)) is not None:
             restrict = Element(
                 f"{XMLSchema}restriction",
                 base=f"{prefix}:string",
             )
         else:
+            new_ns = "xs"
+            while new_ns in add_ns:
+                new_ns += "s"
             restrict = Element(
                 f"{XMLSchema}restriction",
-                base="xs:string",
-                nsmap={"xs": XMLURL},
+                base=f"{new_ns}:string",
+                nsmap={new_ns: XMLURL},
             )
 
         return with_child(
             Element(f"{XMLSchema}simpleType", name="PGConnection"),
             with_child(
                 restrict,
                 Element(f"{XMLSchema}pattern", value=CONN_PATTERN),
```

### Comparing `xmlable-1.0.1/src/xmlable/_errors.py` & `xmlable-1.1.0/src/xmlable/_errors.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/src/xmlable/_io.py` & `xmlable-1.1.0/src/xmlable/_io.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/src/xmlable/_lxml_helpers.py` & `xmlable-1.1.0/src/xmlable/_lxml_helpers.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/src/xmlable/_manual.py` & `xmlable-1.1.0/src/xmlable/_manual.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,17 +69,20 @@
                 for d in deps:
                     if d not in visited:
                         toposort(d, visited, dec_order)
                 dec_order.append(curr)
 
             toposort(cls, visited, dec_order)
 
-            # Create forward declarations
+            # Create forward declarations, potentially adding to namespaces
             decs: list[_Element] = [dec.xsd_forward(namespaces) for dec in dec_order]  # type: ignore[attr-defined]
 
+            # generate main element (can add to namespaces)
+            main_element = cls_xobject.xsd_out(id, add_ns=namespaces)
+
             return ElementTree(
                 with_children(
                     Element(
                         f"{XMLSchema}schema",
                         id=id,
                         elementFormDefault="qualified",
                         nsmap=namespaces,
@@ -89,15 +92,15 @@
                             f"{XMLSchema}import",
                             namespace=ns,
                             schemaLocation=sloc,
                         )
                         for ns, sloc in imports.items()
                     ]
                     + decs
-                    + [cls_xobject.xsd_out(id, add_ns=namespaces)],
+                    + [main_element],
                 )
             )
 
         def xml(schema_name: str = cls_name) -> _ElementTree:
             return ElementTree(cls_xobject.xml_temp(schema_name))
 
         def xml_value(self, id: str = cls_name) -> _ElementTree:
```

### Comparing `xmlable-1.0.1/src/xmlable/_user.py` & `xmlable-1.1.0/src/xmlable/_user.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/src/xmlable/_utils.py` & `xmlable-1.1.0/src/xmlable/_utils.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/src/xmlable/_xmlify.py` & `xmlable-1.1.0/src/xmlable/_xmlify.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/src/xmlable/_xobject.py` & `xmlable-1.1.0/src/xmlable/_xobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,20 +81,25 @@
             return Element(
                 f"{XMLSchema}element",
                 name=name,
                 type=f"{prefix}:{self.type_str}",
                 attrib=attribs,
             )
         else:
+            # add new namespace, resolve conflicts with extra 's'
+            new_ns = "xs"
+            while new_ns in add_ns:
+                new_ns += "s"
+            add_ns[new_ns] = XMLURL
             return Element(
                 f"{XMLSchema}element",
                 name=name,
-                type=f"xs:{self.type_str}",
+                type=f"{new_ns}:{self.type_str}",
                 attrib=attribs,
-                nsmap={"xs": XMLURL},
+                nsmap={new_ns: XMLURL},
             )
 
     def xml_temp(self, name: str) -> _Element:
         return with_text(Element(name), f"Fill me with an {self.type_str}")
 
     def xml_out(self, name: str, val: Any, ctx: XErrorCtx) -> _Element:
         if not self.validate_fn(val):
```

### Comparing `xmlable-1.0.1/tests/test_basic.py` & `xmlable-1.1.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/LICENSE` & `xmlable-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.1/README.md` & `xmlable-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 write_file("config_xml_example.xml", original.xml_value())
 
 read_config: Config = parse_file(Config, "config_xml_example.xml")
 
 assert read_config == original
 ```
 
-See more in [examples](examples/)
+See more in [examples](https://github.com/OliverKillane/xmlable/tree/master/examples)
 
 ## Capabilities
 
 ### Types
 
 Currently supports the types:
 
@@ -88,15 +88,15 @@
     def xsd_forward(add_ns: dict[str, str]) -> _Element:
         pass
 
     def xsd_dependencies() -> set[type]:
         return {MyClass}
 ```
 
-See the [user define example](examples/userdefined) for implementation.
+See the [user define example](https://github.com/OliverKillane/xmlable/tree/master/examples/userdefined) for implementation.
 
 ## Limitations
 
 ### Unions of Generic Types
 
 Generating xsd works, parsing works, however generating an xml template can fail
 if they type is not determinable at runtime.
```

### Comparing `xmlable-1.0.1/pyproject.toml` & `xmlable-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xmlable"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
   { name="Oliver Killane", email="oliverkillane.business@gmail.com" },
 ]
-description = "A tool for generating xsd and xml config from python data classes"
+description = "A decorator for generating xsd, xml and parsers from dataclasses"
 readme = "README.md"
 license = { file = "LICENSE"}
 keywords = ["xml", "xmlschema", "xsd", "lxml"]
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `xmlable-1.0.1/PKG-INFO` & `xmlable-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: xmlable
-Version: 1.0.1
-Summary: A tool for generating xsd and xml config from python data classes
+Version: 1.1.0
+Summary: A decorator for generating xsd, xml and parsers from dataclasses
 Project-URL: Homepage, https://github.com/OliverKillane/xmlable
 Project-URL: Bug Tracker, https://github.com/OliverKillane/xmlable/issues
 Project-URL: Source, https://github.com/OliverKillane/xmlable
 Author-email: Oliver Killane <oliverkillane.business@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Oliver Killane
@@ -68,15 +68,15 @@
 write_file("config_xml_example.xml", original.xml_value())
 
 read_config: Config = parse_file(Config, "config_xml_example.xml")
 
 assert read_config == original
 ```
 
-See more in [examples](examples/)
+See more in [examples](https://github.com/OliverKillane/xmlable/tree/master/examples)
 
 ## Capabilities
 
 ### Types
 
 Currently supports the types:
 
@@ -132,15 +132,15 @@
     def xsd_forward(add_ns: dict[str, str]) -> _Element:
         pass
 
     def xsd_dependencies() -> set[type]:
         return {MyClass}
 ```
 
-See the [user define example](examples/userdefined) for implementation.
+See the [user define example](https://github.com/OliverKillane/xmlable/tree/master/examples/userdefined) for implementation.
 
 ## Limitations
 
 ### Unions of Generic Types
 
 Generating xsd works, parsing works, however generating an xml template can fail
 if they type is not determinable at runtime.
```

