# Comparing `tmp/algokit_client_generator-0.1.0b1-py3-none-any.whl.zip` & `tmp/algokit_client_generator-0.1.0b2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,16 @@
-Zip file size: 12319 bytes, number of entries: 11
+Zip file size: 13241 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       91 b- defN 80-Jan-01 00:00 algokit_client_generator/__init__.py
--rw-r--r--  2.0 unx     1130 b- defN 80-Jan-01 00:00 algokit_client_generator/cli.py
+-rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 algokit_client_generator/__main__.py
+-rw-r--r--  2.0 unx     1783 b- defN 80-Jan-01 00:00 algokit_client_generator/cli.py
 -rw-r--r--  2.0 unx     3122 b- defN 80-Jan-01 00:00 algokit_client_generator/document.py
 -rw-r--r--  2.0 unx    22444 b- defN 80-Jan-01 00:00 algokit_client_generator/generator.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_client_generator/py.typed
 -rw-r--r--  2.0 unx     5986 b- defN 80-Jan-01 00:00 algokit_client_generator/spec.py
 -rw-r--r--  2.0 unx     3847 b- defN 80-Jan-01 00:00 algokit_client_generator/utils.py
--rw-r--r--  2.0 unx      810 b- defN 80-Jan-01 00:00 algokit_client_generator/writer.py
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b1.dist-info/LICENSE
--rw-r--r--  2.0 unx      635 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1005 b- defN 16-Jan-01 00:00 algokit_client_generator-0.1.0b1.dist-info/RECORD
-11 files, 40234 bytes uncompressed, 10587 bytes compressed:  73.7%
+-rw-r--r--  2.0 unx      890 b- defN 80-Jan-01 00:00 algokit_client_generator/writer.py
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      635 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       78 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1297 b- defN 16-Jan-01 00:00 algokit_client_generator-0.1.0b2.dist-info/RECORD
+14 files, 41391 bytes uncompressed, 11025 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -1,34 +1,43 @@
 Filename: algokit_client_generator/__init__.py
 Comment: 
 
+Filename: algokit_client_generator/__main__.py
+Comment: 
+
 Filename: algokit_client_generator/cli.py
 Comment: 
 
 Filename: algokit_client_generator/document.py
 Comment: 
 
 Filename: algokit_client_generator/generator.py
 Comment: 
 
+Filename: algokit_client_generator/py.typed
+Comment: 
+
 Filename: algokit_client_generator/spec.py
 Comment: 
 
 Filename: algokit_client_generator/utils.py
 Comment: 
 
 Filename: algokit_client_generator/writer.py
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b1.dist-info/LICENSE
+Filename: algokit_client_generator-0.1.0b2.dist-info/LICENSE
+Comment: 
+
+Filename: algokit_client_generator-0.1.0b2.dist-info/METADATA
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b1.dist-info/METADATA
+Filename: algokit_client_generator-0.1.0b2.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b1.dist-info/WHEEL
+Filename: algokit_client_generator-0.1.0b2.dist-info/entry_points.txt
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b1.dist-info/RECORD
+Filename: algokit_client_generator-0.1.0b2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_client_generator/cli.py

```diff
@@ -1,37 +1,46 @@
 import sys
 from pathlib import Path
 
 from algokit_client_generator.generator import GenerationSettings
 from algokit_client_generator.writer import generate_client
 
+DEFAULT_CLIENT = "client_generated.py"
+
 
 def walk_dir(path: Path, output_name: str, settings: GenerationSettings) -> None:
     for child in path.iterdir():
         if child.is_dir():
             walk_dir(child, output_name, settings)
         elif child.name.lower() == "application.json":
             generate_client(child, child.parent / output_name, settings)
 
 
 def main() -> None:
     # TODO: proper CLI parsing
-    args = dict(enumerate(sys.argv))
-    input_path = Path(args.get(1, ".")).absolute()
-    output = args.get(2, "client_generated.py")
-
     settings = GenerationSettings(max_line_length=120)
 
-    if not input_path.exists():
-        raise Exception(f"{input_path} not found")
-
-    if input_path.is_dir():
-        walk_dir(input_path, output, settings)
-    else:
-        output_path = Path(output)
-        if not output_path.is_absolute():
-            output_path = input_path.parent / output
+    if "--scan" in sys.argv:
+        walk_dir(Path(".").absolute(), DEFAULT_CLIENT, settings)
+    elif len(sys.argv) > 1:
+        input_path = Path(sys.argv[1]).absolute()
+        if not input_path.exists():
+            print(f"{input_path} not found", file=sys.stderr)
+            return
+        elif input_path.is_dir():
+            print(f"{input_path} is not a file", file=sys.stderr)
+            return
+        if len(sys.argv) > 2:
+            output_path = Path(sys.argv[2])
+        else:
+            output_path = input_path.parent / DEFAULT_CLIENT
         generate_client(input_path, output_path, settings)
-
-
-if __name__ == "__main__":
-    main()
+    else:
+        print("usage: algokit-client-generator --scan")
+        print("       Scans current directory recursively and outputs a typed client for each application.json found")
+        print()
+        print("usage: algokit-client-generator path/to/application.json")
+        print(f"       Outputs a typed client to path/to/{DEFAULT_CLIENT}")
+        print()
+        print("usage: algokit-client-generator path/to/application.json my_client.py")
+        print("       Outputs a typed client to my_client.py")
+        return
```

## algokit_client_generator/writer.py

```diff
@@ -10,12 +10,13 @@
     app_spec = ApplicationSpecification.from_json(input_path.read_text())
 
     context = GenerateContext(app_spec)
     if settings:
         context.settings = settings
     output = render(generate(context), context.settings)
     output_path.write_text(output)
+    print(f"Output typed client for {app_spec.contract.name} to {output_path}")
 
 
 def render(parts: DocumentParts, settings: GenerationSettings) -> str:
     context = RenderContext(indent_inc=settings.indent)
     return "".join(convert_part(parts, context))
```

## Comparing `algokit_client_generator-0.1.0b1.dist-info/LICENSE` & `algokit_client_generator-0.1.0b2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_client_generator-0.1.0b1.dist-info/METADATA` & `algokit_client_generator-0.1.0b2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-client-generator
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: Algorand typed client Generator
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_client_generator-0.1.0b1.dist-info/RECORD` & `algokit_client_generator-0.1.0b2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 algokit_client_generator/__init__.py,sha256=ikLxrMdPVjpmrVYDdHbunvzUwiXqrCdvp8Qi5x0gC0c,91
-algokit_client_generator/cli.py,sha256=OFNbJNWhSDP-xqE54RwJDOgxE0sx5FqoatHkfq8Htlc,1130
+algokit_client_generator/__main__.py,sha256=MlkUdDAWa2XH1QDdjvayVR_WaZEGkA9voNutHzWEfFo,54
+algokit_client_generator/cli.py,sha256=F7dcZtmliFiDCZEU5hc2ya9BPxoi7fKx49Azx0tqOrc,1783
 algokit_client_generator/document.py,sha256=-IIw0wXqZ9NesrGGbTXANcQQrggAX-DBcegTq9gOJ3s,3122
 algokit_client_generator/generator.py,sha256=meXSfSB6fzX9kYRu7FFyHcRQcC0AorRieeX2EAgViag,22444
+algokit_client_generator/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 algokit_client_generator/spec.py,sha256=LcPiMhvnnscvnACk_YGzweEnzQ7V7kQyDvQ94Uo9Nlo,5986
 algokit_client_generator/utils.py,sha256=iILQJ-KNSPigkH6Hn8-lJUAMf2dU4cvDKsHFuF9vw5M,3847
-algokit_client_generator/writer.py,sha256=6K1hA28OkxruJ8kGdN9H0tLJh_Ivw-wEV2yvjM_eydc,810
-algokit_client_generator-0.1.0b1.dist-info/LICENSE,sha256=fkgfhUgPPyK1aS4tK9QOFRl5fWtuFEtkKx4zPQNT1bQ,1076
-algokit_client_generator-0.1.0b1.dist-info/METADATA,sha256=-laIOfzBOnCP9wyeVStb1eC8ldXRGQ-gip9ye7CPmlQ,635
-algokit_client_generator-0.1.0b1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-algokit_client_generator-0.1.0b1.dist-info/RECORD,,
+algokit_client_generator/writer.py,sha256=MF46CQ8q1nW-K66RcKcXYE1uArrNRKHWF-uKQT8eziU,890
+algokit_client_generator-0.1.0b2.dist-info/LICENSE,sha256=fkgfhUgPPyK1aS4tK9QOFRl5fWtuFEtkKx4zPQNT1bQ,1076
+algokit_client_generator-0.1.0b2.dist-info/METADATA,sha256=P0r-6hVmEFjp2etgM18L5TWl22ysvtfdZ2Vlp1N9E5g,635
+algokit_client_generator-0.1.0b2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+algokit_client_generator-0.1.0b2.dist-info/entry_points.txt,sha256=Z4YZmQEtOuvNIRYqH_aAJeJymkTBWrOnZW3HLaT7qBc,78
+algokit_client_generator-0.1.0b2.dist-info/RECORD,,
```

