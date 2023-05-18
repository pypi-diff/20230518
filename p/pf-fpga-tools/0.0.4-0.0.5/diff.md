# Comparing `tmp/pf_fpga_tools-0.0.4.tar.gz` & `tmp/pf_fpga_tools-0.0.5.tar.gz`

## Comparing `pf_fpga_tools-0.0.4.tar` & `pf_fpga_tools-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/.flake8
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/__about__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/__init__.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/exceptions.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/utils.py
--rwxr-xr-x   0        0        0      916 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfBuildCore/__main__.py
--rw-r--r--   0        0        0    14660 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfBuildCore/pfBuildCore.py
--rwxr-xr-x   0        0        0      940 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfCloneCoreTemplate/__main__.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfCloneCoreTemplate/pfCloneCoreTemplate.py
--rwxr-xr-x   0        0        0      925 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfConvertImage/__main__.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfConvertImage/pfConvertImage.py
--rwxr-xr-x   0        0        0      922 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfInstallCore/__main__.py
--rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfInstallCore/pfInstallCore.py
--rwxr-xr-x   0        0        0      937 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfReverseBitstream/__main__.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfReverseBitstream/pfReverseBitstream.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/LICENSE
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/README.md
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/.flake8
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/__about__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/__init__.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/exceptions.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/utils.py
+-rwxr-xr-x   0        0        0      916 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfBuildCore/__main__.py
+-rw-r--r--   0        0        0    14696 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfBuildCore/pfBuildCore.py
+-rwxr-xr-x   0        0        0      940 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfCloneCoreTemplate/__main__.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfCloneCoreTemplate/pfCloneCoreTemplate.py
+-rwxr-xr-x   0        0        0      925 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfConvertImage/__main__.py
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfConvertImage/pfConvertImage.py
+-rwxr-xr-x   0        0        0      922 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfInstallCore/__main__.py
+-rw-r--r--   0        0        0     7282 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfInstallCore/pfInstallCore.py
+-rwxr-xr-x   0        0        0      922 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfQuartusEdit/__main__.py
+-rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfQuartusEdit/pfQuartusEdit.py
+-rwxr-xr-x   0        0        0      937 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfReverseBitstream/__main__.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfReverseBitstream/pfReverseBitstream.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/README.md
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/PKG-INFO
```

### Comparing `pf_fpga_tools-0.0.4/pffpgatools/utils.py` & `pf_fpga_tools-0.0.5/pfFPGATools/utils.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.4/pffpgatools/pfBuildCore/__main__.py` & `pf_fpga_tools-0.0.5/pfFPGATools/pfBuildCore/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import sys
 import traceback
 
 from .pfBuildCore import pfBuildCore
-from pffpgatools.exceptions import ArgumentError
+from pfFPGATools.exceptions import ArgumentError
 
 # -- This enables more debugging information for exceptions.
 _debug_on: bool = False
 
 
 def main():
     global _debug_on
```

### Comparing `pf_fpga_tools-0.0.4/pffpgatools/pfBuildCore/pfBuildCore.py` & `pf_fpga_tools-0.0.5/pfFPGATools/pfBuildCore/pfBuildCore.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import os
 import sys
 import getopt
 import shutil
 import traceback
 
-from pffpgatools.__about__ import __version__
-from pffpgatools.utils import Utils
+from pfFPGATools.__about__ import __version__
+from pfFPGATools.utils import Utils
 
 from datetime import date
 from pathlib import Path
 from typing import List
 from typing import Dict
 
 try:
@@ -25,23 +25,27 @@
 # -- Classes
 class pfBuildCore:
     """A tool to build an analog pocket core"""
 
     def __init__(self, args):
         """Constructor based on command line arguments."""
 
+        self.short_name: str = None
+
         try:
             # -- Gather the arguments
-            opts, arguments = getopt.getopt(args, 'hv', ['help', 'version', 'corefilename', 'bitstreamfile', 'debug'])
+            opts, arguments = getopt.getopt(args, 'hv', ['debug', 'help', 'version', 'corefilename', 'bitstreamfile', 'debug'])
 
             print_core_filename: bool = False
             print_bitstream_file: bool = False
 
             for o, a in opts:
-                if o in ('-h', '--help'):
+                if o in ('--debug'):
+                    continue
+                elif o in ('-h', '--help'):
                     pfBuildCore.printUsage()
                     sys.exit(0)
                 elif o in ('-v', '--version'):
                     pfBuildCore.printVersion()
                     sys.exit(0)
                 elif o in ('--corefilename'):
                     print_core_filename = True
@@ -95,14 +99,24 @@
 
         param: str = section.get(param_name, None)
         if param is None:
             raise RuntimeError('Can\'t find parameter %s in sectior %s config file.' % (param_name, section_name))
 
         return param
 
+    def getShortName(self) -> str:
+        if self.short_name is None:
+            self.short_name = self.getConfigParam('Platform', 'short_name')
+
+            for c in self.short_name:
+                if (c.isalnum() is False) or c.isupper():
+                    raise RuntimeError('Platform short name should be lower-case and can only contain a-z, 0-9 or _.')
+
+        return self.short_name
+
     def generateDefinitionFiles(self, cores_folder, platforms_folder) -> None:
         output_filename = os.path.join(cores_folder, 'audio.json')
         with open(output_filename, 'w') as out_file:
             out_file.write('{\n')
             out_file.write('  "audio": {\n')
             out_file.write('    "magic": "APF_VER_1"\n')
             out_file.write('  }\n')
@@ -159,15 +173,15 @@
             out_file.write('        "rotation": %d,\n' % (self.getConfigParam('Video', 'rotation')))
             out_file.write('        "mirror": %d\n' % (self.getConfigParam('Video', 'mirror')))
             out_file.write('      }\n')
             out_file.write('    ]\n')
             out_file.write('  }\n')
             out_file.write('}\n')
 
-        output_filename = os.path.join(platforms_folder, '%s.json' % (self.getConfigParam('Platform', 'short_name')))
+        output_filename = os.path.join(platforms_folder, '%s.json' % (self.getShortName()))
         with open(output_filename, 'w') as out_file:
             out_file.write('{\n')
             out_file.write('  "platform": {\n')
             out_file.write('    "category": "%s",\n' % (self.getConfigParam('Platform', 'category')))
             out_file.write('    "name": "%s",\n' % (self.getConfigParam('Platform', 'name')))
             out_file.write('    "year": %s,\n' % (self.today.split('-')[0]))
             out_file.write('    "manufacturer": "%s"\n' % (self.getConfigParam('Author', 'name')))
@@ -176,16 +190,16 @@
 
         output_filename = os.path.join(cores_folder, 'core.json')
         with open(output_filename, 'w') as out_file:
             out_file.write('{\n')
             out_file.write('  "core": {\n')
             out_file.write('    "magic": "APF_VER_1",\n')
             out_file.write('    "metadata": {\n')
-            out_file.write('      "platform_ids": ["%s"],\n' % (self.getConfigParam('Platform', 'short_name')))
-            out_file.write('      "shortname": "%s",\n' % (self.getConfigParam('Platform', 'short_name')))
+            out_file.write('      "platform_ids": ["%s"],\n' % (self.getShortName()))
+            out_file.write('      "shortname": "%s",\n' % (self.getShortName()))
             out_file.write('      "description": "%s",\n' % (self.getConfigParam('Platform', 'description')))
             out_file.write('      "author": "%s",\n' % (self.getConfigParam('Author', 'name')))
             out_file.write('      "url": "%s",\n' % (self.getConfigParam('Author', 'url')))
             out_file.write('      "version": "%s",\n' % (self.getConfigParam('Build', 'version')))
             out_file.write('      "date_release": "%s"\n' % (self.today))
             out_file.write('    },\n')
             out_file.write('    "framework": {\n')
@@ -201,39 +215,41 @@
             out_file.write('        "cartridge_adapter": -1\n')
             out_file.write('      }\n')
             out_file.write('    },\n')
             out_file.write('    "cores": [\n')
             out_file.write('      {\n')
             out_file.write('        "name": "default",\n')
             out_file.write('        "id": 0,\n')
-            out_file.write('        "filename": "%s.rbf_r"\n' % (self.getConfigParam('Platform', 'short_name')))
+            out_file.write('        "filename": "%s.rbf_r"\n' % (self.getShortName()))
             out_file.write('      }\n')
             out_file.write('    ]\n')
             out_file.write('  }\n')
             out_file.write('}\n')
 
     def convertImages(self, cores_folder, platforms_image_folder, dep_file) -> None:
         convert_image_command = 'pfConvertImage'
 
         src_image_file = os.path.join(self.config_file_folder, self.getConfigParam('Platform', 'image'))
-        dest_bin_file = os.path.join(platforms_image_folder, '%s.bin' % (self.getConfigParam('Platform', 'short_name')))
+        dest_bin_file = os.path.join(platforms_image_folder, '%s.bin' % (self.getShortName()))
         Utils.shellCommand([convert_image_command, src_image_file, dest_bin_file])
         self.addDependency(dep_file, src_image_file)
 
         src_image_file = os.path.join(self.config_file_folder, self.getConfigParam('Author', 'icon'))
         dest_bin_file = os.path.join(cores_folder, 'icon.bin')
         Utils.shellCommand([convert_image_command, src_image_file, dest_bin_file])
         self.addDependency(dep_file, src_image_file)
 
     def outputFilename(self):
         return os.path.join(self.destination_folder, self.packagedFilename())
 
     def packageCore(self):
         deps = []
-        packaged_filename = os.path.join('..', self.packagedFilename())
+        packaged_filename = os.path.abspath(os.path.join(self.destination_folder, self.packagedFilename()))
+        if os.path.exists(packaged_filename):
+            os.remove(packaged_filename)
 
         arguments: List[str] = ['zip', '-r', packaged_filename]
         for p in Path(self.core_folder).rglob('*'):
             if os.path.isdir(p):
                 continue
 
             arguments.append(str(p.relative_to(self.core_folder)))
@@ -247,40 +263,44 @@
             dep_file.write('%s: %s' % (output_filename.replace(' ', '\\ '), self.config_filename))
 
         dep_file.write(' \\\n %s' % (dep))
 
         self.dependency_count += 1
 
     def fullPlatformName(self) -> str:
-        return '%s.%s' % (self.getConfigParam('Author', 'name'), self.getConfigParam('Platform', 'short_name'))
+        return '%s.%s' % (self.getConfigParam('Author', 'name'), self.getShortName())
 
     def packagedFilename(self) -> str:
         return '%s-%s-%s.zip' % (self.fullPlatformName(), self.getConfigParam('Build', 'version'), self.today)
 
     def bitstreamFile(self) -> str:
         return os.path.expandvars(self.getConfigParam('Bitstream', 'source'))
 
     def main(self) -> None:
-        os.makedirs(self.core_folder, exist_ok=True)
+        # -- We delete the core build folder in case stale files are in there (for example after changing the core config file)
+        if os.path.exists(self.core_folder):
+            shutil.rmtree(self.core_folder)
+
+        os.makedirs(self.core_folder)
 
         full_platform_name = self.fullPlatformName()
         cores_folder = os.path.join(self.core_folder, 'Cores', full_platform_name)
         os.makedirs(cores_folder, exist_ok=True)
 
         platforms_folder = os.path.join(self.core_folder, 'Platforms')
         os.makedirs(platforms_folder, exist_ok=True)
 
         platforms_image_folder = os.path.join(platforms_folder, '_images')
         os.makedirs(platforms_image_folder, exist_ok=True)
 
-        dependency_filename = os.path.join(self.core_folder, 'deps.d')
+        dependency_filename = os.path.join(self.destination_folder, 'deps.d')
         with open(dependency_filename, 'w') as dep_file:
-            print('Building bitstream file...')
+            print('Reversing bitstream file...')
             bitstream_source = self.bitstreamFile()
-            bitstream_dest = os.path.join(cores_folder, '%s.rbf_r' % (self.getConfigParam('Platform', 'short_name')))
+            bitstream_dest = os.path.join(cores_folder, '%s.rbf_r' % self.getShortName())
             Utils.shellCommand(['pfReverseBitstream', bitstream_source, bitstream_dest])
 
             self.addDependency(dep_file, bitstream_source)
 
             print('Generating definitions files...')
             self.generateDefinitionFiles(cores_folder, platforms_folder)
 
@@ -314,36 +334,7 @@
         print('   --version/-v       - Display the app\'s version.')
         print('   --debug            - Enable extra debugging information.')
         print('')
 
     @classmethod
     def printVersion(cls) -> None:
         print('🛠️  pfBuildCore v' + __version__ + ' 🛠️')
-
-
-def main():
-    _debug_on = False
-
-    try:
-        if '--debug' in sys.argv:
-            print('Enabling debugging information.')
-            _debug_on = True
-
-        # -- Remove the first argument (which is the script filename)
-        build = pfBuildCore(sys.argv[1:])
-
-        if build is not None:
-            build.main()
-    except Exception as e:
-        if _debug_on is True:
-            print(traceback.format_exc())
-        else:
-            print(e)
-
-        sys.exit(1)
-    except KeyboardInterrupt:
-        print('Execution interrupted by user.')
-        sys.exit(1)
-
-
-if __name__ == '__main__':
-    main()
```

### Comparing `pf_fpga_tools-0.0.4/pffpgatools/pfCloneCoreTemplate/__main__.py` & `pf_fpga_tools-0.0.5/pfFPGATools/pfCloneCoreTemplate/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import sys
 import traceback
 
 from .pfCloneCoreTemplate import pfCloneCoreTemplate
-from pffpgatools.exceptions import ArgumentError
+from pfFPGATools.exceptions import ArgumentError
 
 # -- This enables more debugging information for exceptions.
 _debug_on: bool = False
 
 
 def main():
     global _debug_on
```

### Comparing `pf_fpga_tools-0.0.4/pffpgatools/pfCloneCoreTemplate/pfCloneCoreTemplate.py` & `pf_fpga_tools-0.0.5/pfFPGATools/pfCloneCoreTemplate/pfCloneCoreTemplate.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,35 +3,37 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
 import sys
 import getopt
 import shutil
 
-from pffpgatools.__about__ import __version__
-from pffpgatools.utils import Utils
-from pffpgatools.exceptions import ArgumentError
+from pfFPGATools.__about__ import __version__
+from pfFPGATools.utils import Utils
+from pfFPGATools.exceptions import ArgumentError
 
 
 # -- Classes
 class pfCloneCoreTemplate:
     """A tool to clone the Github core template."""
 
     def __init__(self, args):
         """Constructor based on command line arguments."""
 
         try:
             self.branch_name = None
             self.tag_name = None
 
             # -- Gather the arguments
-            opts, arguments = getopt.getopt(args, 'hvb:t:', ['help', 'version', 'branch=', 'tag='])
+            opts, arguments = getopt.getopt(args, 'hvb:t:', ['debug', 'help', 'version', 'branch=', 'tag='])
 
             for o, a in opts:
-                if o in ('-h', '--help'):
+                if o in ('--debug'):
+                    continue
+                elif o in ('-h', '--help'):
                     pfCloneCoreTemplate.printUsage()
                     sys.exit(0)
                 elif o in ('-v', '--version'):
                     pfCloneCoreTemplate.printVersion()
                     sys.exit(0)
                 elif o in ('-b', '--branch'):
                     if self.tag_name is not None:
@@ -54,60 +56,46 @@
             print('Unknown option or argument. Maybe start with `pfCloneCoreTemplate --help?')
             sys.exit(0)
 
     def main(self) -> None:
         if Utils.commandExists('git') is False:
             raise RuntimeError('You must have git installed on your machine to continue.')
 
-        repo_folder = os.path.join(self.destination_folder, 'pf-core-template')
+        repo_folder = os.path.join(self.destination_folder, 'pfCoreTemplate')
         if os.path.exists(repo_folder):
             shutil.rmtree(repo_folder)
 
         print('Cloning core template in \'' + repo_folder + '\'.')
 
         command_line = ['git', 'clone', '--depth', '1']
 
         if self.branch_name is not None:
             command_line.append('--branch')
             command_line.append(self.branch_name)
         elif self.tag_name is not None:
             command_line.append('--branch')
             command_line.append(self.tag_name)
 
-        command_line.append('https://github.com/DidierMalenfant/pf-core-template.git')
+        command_line.append('https://github.com/DidierMalenfant/pfCoreTemplate.git')
 
         Utils.shellCommand(command_line, from_dir=self.destination_folder, silent_mode=True)
 
+        git_folder = os.path.join(repo_folder, '.git')
+        if os.path.exists(git_folder):
+            shutil.rmtree(git_folder)
+
     @classmethod
     def printUsage(cls) -> None:
         pfCloneCoreTemplate.printVersion()
         print('')
         print('usage: pfCloneCoreTemplate <options> destination_folder')
         print('')
         print('The following options are supported:')
         print('')
         print('   --help/-h          - Show a help message.')
         print('   --version/-v       - Display the app\'s version.')
+        print('   --debug            - Enable extra debugging information.')
         print('')
 
     @classmethod
     def printVersion(cls) -> None:
         print('🛠️  pfCloneCoreTemplate v' + __version__ + ' 🛠️')
-
-
-def main():
-    try:
-        # -- Remove the first argument (which is the script filename)
-        build = pfCloneCoreTemplate(sys.argv[1:])
-
-        if build is not None:
-            build.main()
-    except Exception as e:
-        print(e)
-        sys.exit(1)
-    except KeyboardInterrupt:
-        print('Execution interrupted by user.')
-        sys.exit(1)
-
-
-if __name__ == '__main__':
-    main()
```

### Comparing `pf_fpga_tools-0.0.4/pffpgatools/pfConvertImage/__main__.py` & `pf_fpga_tools-0.0.5/pfFPGATools/pfConvertImage/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import sys
 import traceback
 
 from .pfConvertImage import pfConvertImage
-from pffpgatools.exceptions import ArgumentError
+from pfFPGATools.exceptions import ArgumentError
 
 # -- This enables more debugging information for exceptions.
 _debug_on: bool = False
 
 
 def main():
     global _debug_on
```

### Comparing `pf_fpga_tools-0.0.4/pffpgatools/pfConvertImage/pfConvertImage.py` & `pf_fpga_tools-0.0.5/pfFPGATools/pfConvertImage/pfConvertImage.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,33 +3,35 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
 import sys
 import getopt
 import traceback
 
-from pffpgatools.__about__ import __version__
-from pffpgatools.utils import Utils
+from pfFPGATools.__about__ import __version__
+from pfFPGATools.utils import Utils
 
 from PIL import Image
 
 
 # -- Classes
 class pfConvertImage:
     """A tool to install a zipped up core file onto a given volume (SD card or Pocket in USB access mode)."""
 
     def __init__(self, args):
         """Constructor based on command line arguments."""
 
         try:
             # -- Gather the arguments
-            opts, arguments = getopt.getopt(args, 'hv', ['help', 'version', 'debug'])
+            opts, arguments = getopt.getopt(args, 'hv', ['debug', 'help', 'version', 'debug'])
 
             for o, a in opts:
-                if o in ('-h', '--help'):
+                if o in ('--debug'):
+                    continue
+                elif o in ('-h', '--help'):
                     pfConvertImage.printUsage()
                     sys.exit(0)
                 elif o in ('-v', '--version'):
                     pfConvertImage.printVersion()
                     sys.exit(0)
                 elif o in ('--debug'):
                     # -- We ignore this argument because it was already dealt with in the calling main() code.
@@ -96,36 +98,7 @@
         print('   --version/-v       - Display the app\'s version.')
         print('   --debug            - Enable extra debugging information.')
         print('')
 
     @classmethod
     def printVersion(cls) -> None:
         print('🛠️  pfConvertImage v' + __version__ + ' 🛠️')
-
-
-def main():
-    _debug_on = False
-
-    try:
-        if '--debug' in sys.argv:
-            print('Enabling debugging information.')
-            _debug_on = True
-
-        # -- Remove the first argument (which is the script filename)
-        build = pfConvertImage(sys.argv[1:])
-
-        if build is not None:
-            build.main()
-    except Exception as e:
-        if _debug_on is True:
-            print(traceback.format_exc())
-        else:
-            print(e)
-
-        sys.exit(1)
-    except KeyboardInterrupt:
-        print('Execution interrupted by user.')
-        sys.exit(1)
-
-
-if __name__ == '__main__':
-    main()
```

### Comparing `pf_fpga_tools-0.0.4/pffpgatools/pfInstallCore/__main__.py` & `pf_fpga_tools-0.0.5/pfFPGATools/pfInstallCore/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import sys
 import traceback
 
 from .pfInstallCore import pfInstallCore
-from pffpgatools.exceptions import ArgumentError
+from pfFPGATools.exceptions import ArgumentError
 
 # -- This enables more debugging information for exceptions.
 _debug_on: bool = False
 
 
 def main():
     global _debug_on
```

### Comparing `pf_fpga_tools-0.0.4/pffpgatools/pfReverseBitstream/__main__.py` & `pf_fpga_tools-0.0.5/pfFPGATools/pfReverseBitstream/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import sys
 import traceback
 
 from .pfReverseBitstream import pfReverseBitstream
-from pffpgatools.exceptions import ArgumentError
+from pfFPGATools.exceptions import ArgumentError
 
 # -- This enables more debugging information for exceptions.
 _debug_on: bool = False
 
 
 def main():
     global _debug_on
```

### Comparing `pf_fpga_tools-0.0.4/pffpgatools/pfReverseBitstream/pfReverseBitstream.py` & `pf_fpga_tools-0.0.5/pfFPGATools/pfReverseBitstream/pfReverseBitstream.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
 import sys
 import getopt
 
-from pffpgatools.__about__ import __version__
+from pfFPGATools.__about__ import __version__
 
 
 # -- Classes
 class pfReverseBitstream:
     """A tool to reverse the bitstream of an rbf file for an Analog Pocket core."""
 
     def __init__(self, args):
         """Constructor based on command line arguments."""
 
         try:
             # -- Gather the arguments
-            opts, arguments = getopt.getopt(args, 'hv', ['help', 'version'])
+            opts, arguments = getopt.getopt(args, 'hv', ['debug', 'help', 'version'])
 
             for o, a in opts:
-                if o in ('-h', '--help'):
+                if o in ('--debug'):
+                    continue
+                elif o in ('-h', '--help'):
                     pfReverseBitstream.printUsage()
                     sys.exit(0)
                 elif o in ('-v', '--version'):
                     pfReverseBitstream.printVersion()
                     sys.exit(0)
 
             nb_of_arguments: int = len(arguments)
@@ -69,31 +71,13 @@
         print('')
         print('usage: pfReverseBitstream <options> src_filename dest_filename')
         print('')
         print('The following options are supported:')
         print('')
         print('   --help/-h          - Show a help message.')
         print('   --version/-v       - Display the app\'s version.')
+        print('   --debug            - Enable extra debugging information.')
         print('')
 
     @classmethod
     def printVersion(cls) -> None:
         print('🛠️  pfReverseBitstream v' + __version__ + ' 🛠️')
-
-
-def main():
-    try:
-        # -- Remove the first argument (which is the script filename)
-        build = pfReverseBitstream(sys.argv[1:])
-
-        if build is not None:
-            build.main()
-    except Exception as e:
-        print(e)
-        sys.exit(1)
-    except KeyboardInterrupt:
-        print('Execution interrupted by user.')
-        sys.exit(1)
-
-
-if __name__ == '__main__':
-    main()
```

### Comparing `pf_fpga_tools-0.0.4/LICENSE` & `pf_fpga_tools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.4/README.md` & `pf_fpga_tools-0.0.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# pf-fpga-tools
+# pfFPGATools
 
-[![GPL-v3.0](https://img.shields.io/github/license/DidierMalenfant/pf-fpga-tools)](https://spdx.org/licenses/GPL-3.0-or-later.html) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pf-fpga-tools.svg)](https://python.org) [![PyPI - Version](https://img.shields.io/pypi/v/pf-fpga-tools.svg)](https://pypi.org/project/pf-fpga-tools)
+[![GPL-v3.0](https://img.shields.io/github/license/DidierMalenfant/pfFPGATools)](https://spdx.org/licenses/GPL-3.0-or-later.html) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pfFPGATools.svg)](https://python.org) [![PyPI - Version](https://img.shields.io/pypi/v/pfFPGATools.svg)](https://pypi.org/project/pfFPGATools)
 
 A set of tools for building and installing [**openFPGA**](https://www.analogue.co/developer) cores for the [**Analog Pocket**](https://www.analogue.co/pocket).
 
 Copyright (c) 2023-present Didier Malenfant.
 
 openFPGA is a registered trademark of [**Analogue**](https://analogue.co).
 
 -----
 
 ### Installation
 
-**pf-fpga-tools** requires at least [Python](https://python.org) 3.7. Make sure you have a [supported version](http://didier.malenfant.net/blog/nerdy/2022/08/17/installing-python.html) of **Python** before proceeding.
+**pfFPGATools** requires at least [Python](https://python.org) 3.7. Make sure you have a [supported version](http://didier.malenfant.net/blog/nerdy/2022/08/17/installing-python.html) of **Python** before proceeding.
 
-You can then install **pf-fpga-tools** by typing the following in a terminal window:
+You can then install **pfFPGATools** by typing the following in a terminal window:
 ```console
 pip install pf-fpga-tools
 ```
 
 ### Installation (macOS)
 
 Also install the following tool dependencies via [brew](https://brew.sh):
@@ -31,24 +31,26 @@
 Also install the following tool dependencies:
 ```
 sudo apt install imagemagick
 ```
 
 ### Usage
 
-**pf-fpga-tools** provides the follow commands commands, sometimes with one or two extra arguments:
+**pfFPGATools** provides the follow commands commands, sometimes with one or two extra arguments:
 
 - `pfBuildCore` - Build a core according to a `toml` config file.
 
 - `pfInstallCore` - Install a zipped up core file onto a given volume.
 
 - `pfConvertImage` - Convert an image for to the binary format used by the **Analog Pocket** for its cores and platform lists.
 
 - `pfReverseBitstream` - Converts an `rbf` bitstream file into an `rbf_r` reversed bitstream.
 
 - `pfCloneCoreTemplate` - Clone the core dev template from Github.
 
+- `pfQuartusEdit` - Edit Quartus project files.
+
 You can use the `--help` argument to get some usage info for each command.
 
 ### License
 
-**pf-fpga-tools** is distributed under the terms of the [GPLv3.0](https://spdx.org/licenses/GPL-3.0-or-later.html) or later license.
+**pfFPGATools** is distributed under the terms of the [GPLv3.0](https://spdx.org/licenses/GPL-3.0-or-later.html) or later license.
```

### Comparing `pf_fpga_tools-0.0.4/pyproject.toml` & `pf_fpga_tools-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -24,34 +24,35 @@
 ]
 dependencies = ['Pillow',
                 'tomli >= 1.1.0 ; python_version < "3.11"']
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://didier.malenfant.net/ProjectFreedom/"
-Documentation = "https://github.com/DidierMalenfant/pf-fpga-tools#readme"
-"Bug Tracker" = "https://github.com/DidierMalenfant/pf-fpga-tools/issues"
-"Source Code" = "https://github.com/DidierMalenfant/pf-fpga-tools"
+Documentation = "https://github.com/DidierMalenfant/pfFPGATools#readme"
+"Bug Tracker" = "https://github.com/DidierMalenfant/pfFPGATools/issues"
+"Source Code" = "https://github.com/DidierMalenfant/pfFPGATools"
 
 [tool.hatch.version]
-path = "pffpgatools/__about__.py"
+path = "pfFPGATools/__about__.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
   "/.github",
 ]
 
 [tool.hatch.build.targets.wheel]
-packages = ["pffpgatools"]
+packages = ["pfFPGATools"]
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-cov",
 ]
 
 [project.scripts]
-pfBuildCore = "pffpgatools.pfBuildCore.__main__:main"
-pfConvertImage = "pffpgatools.pfConvertImage.__main__:main"
-pfInstallCore = "pffpgatools.pfInstallCore.__main__:main"
-pfReverseBitstream = "pffpgatools.pfReverseBitstream.__main__:main"
-pfCloneCoreTemplate = "pffpgatools.pfCloneCoreTemplate.__main__:main"
+pfBuildCore = "pfFPGATools.pfBuildCore.__main__:main"
+pfConvertImage = "pfFPGATools.pfConvertImage.__main__:main"
+pfInstallCore = "pfFPGATools.pfInstallCore.__main__:main"
+pfReverseBitstream = "pfFPGATools.pfReverseBitstream.__main__:main"
+pfCloneCoreTemplate = "pfFPGATools.pfCloneCoreTemplate.__main__:main"
+pfQuartusEdit = "pfFPGATools.pfQuartusEdit.__main__:main"
```

### Comparing `pf_fpga_tools-0.0.4/PKG-INFO` & `pf_fpga_tools-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pf-fpga-tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: A collection of tools for openFPGA projects
 Project-URL: Homepage, https://didier.malenfant.net/ProjectFreedom/
-Project-URL: Documentation, https://github.com/DidierMalenfant/pf-fpga-tools#readme
-Project-URL: Bug Tracker, https://github.com/DidierMalenfant/pf-fpga-tools/issues
-Project-URL: Source Code, https://github.com/DidierMalenfant/pf-fpga-tools
+Project-URL: Documentation, https://github.com/DidierMalenfant/pfFPGATools#readme
+Project-URL: Bug Tracker, https://github.com/DidierMalenfant/pfFPGATools/issues
+Project-URL: Source Code, https://github.com/DidierMalenfant/pfFPGATools
 Author-email: Didier Malenfant <coding@malenfant.net>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Keywords: analoguepocket,fpga,openFPGA
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -19,31 +19,31 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: pillow
 Requires-Dist: tomli>=1.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
-# pf-fpga-tools
+# pfFPGATools
 
-[![GPL-v3.0](https://img.shields.io/github/license/DidierMalenfant/pf-fpga-tools)](https://spdx.org/licenses/GPL-3.0-or-later.html) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pf-fpga-tools.svg)](https://python.org) [![PyPI - Version](https://img.shields.io/pypi/v/pf-fpga-tools.svg)](https://pypi.org/project/pf-fpga-tools)
+[![GPL-v3.0](https://img.shields.io/github/license/DidierMalenfant/pfFPGATools)](https://spdx.org/licenses/GPL-3.0-or-later.html) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pfFPGATools.svg)](https://python.org) [![PyPI - Version](https://img.shields.io/pypi/v/pfFPGATools.svg)](https://pypi.org/project/pfFPGATools)
 
 A set of tools for building and installing [**openFPGA**](https://www.analogue.co/developer) cores for the [**Analog Pocket**](https://www.analogue.co/pocket).
 
 Copyright (c) 2023-present Didier Malenfant.
 
 openFPGA is a registered trademark of [**Analogue**](https://analogue.co).
 
 -----
 
 ### Installation
 
-**pf-fpga-tools** requires at least [Python](https://python.org) 3.7. Make sure you have a [supported version](http://didier.malenfant.net/blog/nerdy/2022/08/17/installing-python.html) of **Python** before proceeding.
+**pfFPGATools** requires at least [Python](https://python.org) 3.7. Make sure you have a [supported version](http://didier.malenfant.net/blog/nerdy/2022/08/17/installing-python.html) of **Python** before proceeding.
 
-You can then install **pf-fpga-tools** by typing the following in a terminal window:
+You can then install **pfFPGATools** by typing the following in a terminal window:
 ```console
 pip install pf-fpga-tools
 ```
 
 ### Installation (macOS)
 
 Also install the following tool dependencies via [brew](https://brew.sh):
@@ -56,24 +56,26 @@
 Also install the following tool dependencies:
 ```
 sudo apt install imagemagick
 ```
 
 ### Usage
 
-**pf-fpga-tools** provides the follow commands commands, sometimes with one or two extra arguments:
+**pfFPGATools** provides the follow commands commands, sometimes with one or two extra arguments:
 
 - `pfBuildCore` - Build a core according to a `toml` config file.
 
 - `pfInstallCore` - Install a zipped up core file onto a given volume.
 
 - `pfConvertImage` - Convert an image for to the binary format used by the **Analog Pocket** for its cores and platform lists.
 
 - `pfReverseBitstream` - Converts an `rbf` bitstream file into an `rbf_r` reversed bitstream.
 
 - `pfCloneCoreTemplate` - Clone the core dev template from Github.
 
+- `pfQuartusEdit` - Edit Quartus project files.
+
 You can use the `--help` argument to get some usage info for each command.
 
 ### License
 
-**pf-fpga-tools** is distributed under the terms of the [GPLv3.0](https://spdx.org/licenses/GPL-3.0-or-later.html) or later license.
+**pfFPGATools** is distributed under the terms of the [GPLv3.0](https://spdx.org/licenses/GPL-3.0-or-later.html) or later license.
```

