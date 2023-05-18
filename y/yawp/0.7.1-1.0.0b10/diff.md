# Comparing `tmp/yawp-0.7.1.tar.gz` & `tmp/yawp-1.0.0b10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yawp-0.7.1.tar", last modified: Sat Jun 25 19:00:51 2022, max compression
+gzip compressed data, was "yawp-1.0.0b10.tar", last modified: Thu May 18 16:14:55 2023, max compression
```

## Comparing `yawp-0.7.1.tar` & `yawp-1.0.0b10.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     9635 2022-06-25 18:53:03.193255 yawp-0.7.1/README.md
--rwxr-xr-x   0        0        0      769 2022-06-07 07:43:28.190425 yawp-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    26731 2022-06-25 18:52:30.493042 yawp-0.7.1/yawp/__init__.py
--rw-r--r--   0        0        0    46768 2022-06-25 18:52:56.041209 yawp-0.7.1/yawp/__main__.py
--rw-r--r--   0        0        0    79131 2022-06-25 18:58:05.419207 yawp-0.7.1/yawp/docs/yawp.pdf
--rw-r--r--   0        0        0    10371 1970-01-01 00:00:00.000000 yawp-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    13951 2023-05-18 15:02:43.510753 yawp-1.0.0b10/README.md
+-rwxr-xr-x   0        0        0      807 2023-01-23 10:24:56.324823 yawp-1.0.0b10/pyproject.toml
+-rwxr-xr-x   0        0        0    32580 2023-05-18 15:02:41.402757 yawp-1.0.0b10/yawp/__init__.py
+-rwxr-xr-x   0        0        0    98271 2023-05-18 14:39:13.246607 yawp-1.0.0b10/yawp/__main__.py
+-rw-r--r--   0        0        0   232685 2023-05-03 07:29:14.608193 yawp-1.0.0b10/yawp/docs/.test.pdf
+-rw-r--r--   0        0        0   125254 2023-05-12 12:19:25.432197 yawp-1.0.0b10/yawp/docs/.yawp.pdf
+-rw-r--r--   0        0        0   125697 2023-05-18 16:12:47.720089 yawp-1.0.0b10/yawp/docs/yawp.pdf
+-rw-r--r--   0        0        0    14727 1970-01-01 00:00:00.000000 yawp-1.0.0b10/PKG-INFO
```

### Comparing `yawp-0.7.1/pyproject.toml` & `yawp-1.0.0b10/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "yawp"
 authors = [{name = "Carlo Alessandro Verre", email = "carlo.alessandro.verre@gmail.com"}]
@@ -13,14 +12,15 @@
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: POSIX :: Linux"]
 requires-python = ">=3.6"
+dependencies = ["PySimpleGui","pdfrw"]
 dynamic = ["version", "description"]
 
 [project.urls]
 Home = "https://pypi.org/project/yawp"
 
 [project.scripts]
 yawp = "yawp.__main__:main"
```

### Comparing `yawp-0.7.1/yawp/__init__.py` & `yawp-1.0.0b10/yawp/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,283 +1,232 @@
-#!/usr/bin/python3
+#!/usr/bin/env python3
 
-'''Yet Another Word Processor, an automatic word processor for text files, with PDF export
+'''Yet Another Word Processor, a word processor for text files, with PDF export
 
-                       I sound my barbaric yawp over the roofs of the world
-                       
-                                                               Walt Whitman
-
-The  name  "yawp"  here  means  Yet  Another Word Processor, and yawp is an
-automatic  (batch,  not  interactive)  word processor for plain text files,
-with  PDF  export.  If  you  really need all the features of a full-fledged
-WYSIWYG  word  processor as LibreOffice Writer, yawp is not for you. But if
-you  just  want to create a simple quick-and-dirty no-frills document, with
-yawp you can:
-
-    • edit a text file by your favorite editor
-    • run yawp in order to:
-        • backup read format and rewrite the text file
-        • export the text file into a PDF file
-        • view the PDF file for check or print
-    • possibly go back to the editor and update the text file, or finish
-
-                                           ┌───────┐
-                                           │backup │
-                                           │       │
-                                           │ file  │
-                                           └─────┬─┘    ┌─────────┐
-                                             △   │      │messages │
-                                             │   │undo  └─────────┘
-                                       backup│   │           △
-                                             │   ▽           │
- ┌───────────┐                           ┌───┴───────┐       │
- │           │         ┌───────┐  read   │           │ show  │
- │           │  edit   │ text  ├────────▷│           ├───────┘    ┌───────┐
- │  editor   ├────────▷│       │         │   yawp    │            │ PDF   │
- │           │         │ file  │◁────────┤           ├───────────▷│       │
- │           │         └───────┘ rewrite │           │ export     │ file  │
- └───────────┘                           └───────────┘            └───┬───┘
-       △                                                              │
-       │                          check                               │
-       └──────────────────────────────────────────────────────────────┘
+"YAWP" here means Yet Another Word Processor, and YAWP is a pure-Python Linux-only
+word  processor  for plain text files, with PDF export. If you really need all the
+features  of  a  full-fledged  WYSIWYG  word processor (with italic bold fonts etc
+etc)  as LibreOffice Writer, YAWP is not for you. But if you just want to create a
+draft or a simple quick-and-dirty no-frills document, give YAWP a try.
 
 Main features are:
 
-    • yawp  processes  in place a single text file, hereinafter referred to
-      simply as "the file"
-    • yawp  before  processing  creates  a  timestamped backup of the file,
-      allowing undo operation
-    • yawp  processing  is  driven by the text in the file and by arguments
-      only, not by commands or tags embedded in text
-    • yawp justifies text at left and right in:
+    • YAWP has a GUI interface, but can be used as a CLI command too
+    • YAWP  processes  in  place a single plain text file, hereinafter referred to
+      simply as the "text file"
+    • YAWP  before  rewriting the text file creates a timestamped backup, allowing
+      Undo operation
+    • YAWP justifies text at left and right in:
         • unindented paragraphs
         • dot-marked indented paragraphs (as this one)
-    • yawp  accepts  unjustified  pictures  (as  schemas,  tables  and code
-      examples) freely intermixed with text
-    • yawp  adopts  an  ad  hoc  policy  for  Python  files, formatting the
-      docstrings but not the Python code
-    • yawp  performs  automatic  multi-level  renumbering  of  chapters and
-      inserts an automatic contents chapter in the file
-    • yawp performs automatic renumbering of figure captions and inserts an
-      automatic figures chapter in the file
-    • yawp  recognizes  relevant  subjects  (quoted  by '"') and inserts an
-      automatic index chapter in the file
-    • yawp cuts the file in pages, by inserting 2-lines page headers
-    • yawp  also has some limited graphic features, you can sketch pictures
-      with  segments (by '`') and arrowheads (by '^'), yawp redraws them by
-      suitable graphic characters (as in Figure above)
-    • yawp  exports  the  resulting  lines in PDF format, with control over
-      character  size  and page layout, and lets you view the generated PDF
-      file for check or print
-    • yawp  corrects  errors  made  by  CUPS-PDF  about  font size and page
-      margins, you can use default corrections or redefine them by yawp.cfg
-    • yawp is "stable", namely if after a yawp execution you run yawp again
-      on  the  same  file with the same arguments, the file content doesn't
-      change
-
-Believe it or not, everything has been kept as simple as possible. 
-
-As  an  example, the Yawp Manual has been created as yawp.pdf from yawp.txt
-by typing:
-
-    │ $ yawp -v -w 80 -J -E 'Yawp 0.7.1 Manual' -X yawp.txt
-
-In order to install yawp, type:
-
-    │ $ sudo apt-get -y update
-    │ $ sudo apt-get -y install printer-driver-cups-pdf
-
-If you don't have pip, type:
-
-    │ $ sudo apt-get -y install python3-pip
-
-If you type at terminal:
-
-    │ $ pip3 install --upgrade yawp
-
-this command will:
-
-    • install current version of yawp if not present
-    • upgrade yawp to the current version if already installed
-
-If you see a message like this:
-
-    │ WARNING: The script yawp is installed in ... which is not on PATH.
-
-don't worry, a reboot should fix the problem.
-
-In  order  to use yawp, you need to know how it works. For any detail, view
-the yawp-generated Yawp Manual by typing:
+    • YAWP  justification  is driven by the text in the text file and by arguments
+      only, not by commands or tags embedded in text
+    • YAWP  accepts  unjustified  pictures  (as schemas, tables and code examples)
+      freely intermixed with text
+    • YAWP  performs  automatic multi-level renumbering of chapters and inserts an
+      automatic Contents chapter in the text file
+    • YAWP  recognizes  relevant subjects (quoted by '"') and inserts an automatic
+      Index chapter in the text file
+    • YAWP  performs  automatic  multi-level  renumbering  of  figure captions and
+      inserts an automatic Figures chapter in the text file
+    • YAWP  cuts  the  text  file  in  pages, by inserting two-lines page headers,
+      allowing  page  numbering  control  and  insertion of initial Roman-numbered
+      pages
+    • YAWP also has some graphic features, you can sketch pictures with horizontal
+      and vertical segments (by '`') and arrowheads (by '^'), YAWP redraws them by
+      suitable Unicode graphic characters
+    • YAWP  exports  the text file in PDF format, with control over character size
+      and  page  layout,  and  lets  you  browse  the generated PDF file, allowing
+      preview and printing
+    • YAWP keeps a distinct argument set for each text file
+    • YAWP  in GUI mode saves the last processed text file and restores it at next
+      invocation
+    • YAWP in GUI mode saves a list of the 20 most recent processed text files and
+      allows to select one at next invocation
+    • YAWP  tries  to  correct  errors  made  by CUPS-PDF about font size and page
+      margins,  you  can  use default corrections or redefine them by a correction
+      file
+    • YAWP  writes  messages  about  processing on terminal and into a timestamped
+      session log file
+    • YAWP  locks the text file to  be processed in order to avoid interference by
+      other concurrent YAWP executions
+    • YAWP  is  stable,  if  after a YAWP execution you run YAWP again on the same
+      file with the same arguments, the text file content does not change
+    • believe  or  not,  YAWP   has   been  kept as simple as possible, about 3000
+      lines of Python code  (plus 3000 lines of this YAWP User Manual)
+
+In  order to install YAWP, we assume that your Linux belongs to the Debian family.
+Type at terminal:
+
+    │ $ sudo apt-get update
+    │ $ sudo apt-get purge printer-driver-cups-pdf
+    │ $ sudo apt-get install printer-driver-cups-pdf idle python3-pip
+    │ $ pip3 install yawp
+
+Imagine your user name is 'xxxx'. If you see a message like this:
+
+    WARNING: The script yawp is installed in '/home/xxxx/.local/bin'
+    which is not on PATH
+
+you can fix the problem by typing:
+
+    │ $ echo 'PATH=$PATH:/home/xxxx/.local/bin' >> /home/xxxx/.bashrc
+
+Now you can close the terminal, open another one, and call YAWP. Syntax is:
+
+    │ $ yawp -h # show a help message and exit
+    │ $ yawp -V # show program's version number and exit
+    │ $ yawp -H [-Y pdf_browser] # browse the PDF YAWP User Manual and exit
+    │ $ yawp -M e [-y text_editor] text_file # run YAWP in CLI Edit mode
+    │ $ yawp -M f [...arguments...] text_file # run YAWP in CLI Format mode
+    │ $ yawp -M n [...arguments...] text_file # run YAWP in CLI Noformat mode
+    │ $ yawp -M u [...arguments...] text_file # run YAWP in CLI Undo mode
+    │ $ yawp text_file # run YAWP in GUI mode, explicit text file, no arguments
+    │ $ yawp # run YAWP in GUI mode, text file from previous session, no arguments
+
+This is the GUI Main window:
+
+ ┌───┬───────────────────────────────────────────────────────────────────┬───┬───┐
+ │   │                              YAWP - Main                          │ _ │ x │
+ ├───┴───────────────────────────────────────────────────────────────────┴───┴───┤
+ │ -v --verbose         □                                                        │
+ │ -y --text-editor    [idle............] -g --graphics        □                 │
+ │ -w --chars-per-line [0...............] -l --just-left-only  □                 │
+ │ -c --contents-title [contents........] -i --index-title    [index...........] │
+ │ -f --figures-title  [figures.........] -F --caption-prefix [figure..........] │
+ │ -p --page-headers    ◎ n=no  ○ f=fullpage  ○ p=picture  ○ c=chapter           │
+ │ -e --even-left      [%n/%N...........] -E --even-right     [%F %Y-%m-%d.....] │
+ │ -o --odd-left       [%c..............] -O --odd-right      [%n/%N...........] │
+ │ -n --page-offset    [0...............] -a --all-pages-E-e   □                 │
+ │ -X --export-pdf      □                                                        │
+ │ -Y --pdf-browser    [xdg-open........] -P --file-pdf       [%P%f.pdf........] │
+ │ -W --char-width     [0...............] -A --char-aspect    [3/5.............] │
+ │ -S --paper-size     [A4..............] -Z --landscape       □                 │
+ │ -L --left-margin    [2cm.............] -R --right-margin   [2cm.............] │
+ │ -T --top-margin     [2cm.............] -B --bottom-margin  [2cm.............] │
+ │ -C --correct-sizes   ○ n=no  ◎ d=default  ○ f=file    -K --fake-margins □     │
+ │ text_file           [.......................................................] │
+ │ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐ │
+ │ │   New    │ │   Open   │ │  Recent  │ │  Saveas  │ │   Help   │ │   Exit   │ │
+ │ └──────────┘ └──────────┘ └──────────┘ └──────────┘ └──────────┘ └──────────┘ │
+ │ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐ │
+ │ │   Edit   │ │  Format  │ │ Noformat │ │   Undo   │ │   Log    │ │  Correct │ │
+ │ └──────────┘ └──────────┘ └──────────┘ └──────────┘ └──────────┘ └──────────┘ │
+ └───────────────────────────────────────────────────────────────────────────────┘
+
+These are the buttons in GUI Main window:
+
+    • 4 buttons dedicated to the selection of the text file:
+        • New button: create a new empty text file
+        • Open button: browse the file system to select the text file
+        • Recent button: browse the list of recent files to select the text file
+        • Saveas button: clone current text file into a new target text file
+    • Help button: browse the YAWP Manual through the PDF browser defined by -Y
+    • Exit button: save current text file with its arguments and finish
+    • 4 buttons dedicated to the processing of the text file:
+        • Edit button: edit the text file through the text editor defined by -y
+        • Format button: process the text file by formatting it
+        • Noformat button: process the text file without formatting it
+        • Undo button: restore the text file to its previous content
+    • Log button: browse the log file through the text editor defined by -y
+    • Correct button: manage the correction file (Edit Reset or Undo)
 
-    │ $ yawp -H
 '''
 
-__version__ = '0.7.1'
-
-__all__ = []
+__version__ = '1.0.0b10'
 
 #----- imports -----
 
 from fnmatch import fnmatchcase
 from glob import glob
-from os import chdir, lstat, popen
-from os.path import join as joinpath, split as splitpath, abspath, expanduser, splitext, exists, isfile, isdir
+from os import chdir, lstat, popen, sep as path_sep
+from os.path import split as splitpath, abspath, expanduser, normpath, splitext, exists, isfile, isdir, basename, dirname
 from subprocess import run, PIPE
 from sys import exit, stdout, stderr
-from time import localtime
+from time import localtime, sleep
 import readline
 
-#----- path & file functions -----
-
-def longpath(path='.'):
-    return abspath(expanduser(path))
-
-def shortpath(path='.'):
-    path, home = longpath(path), longpath('~')
-    return '~' + path[len(home):] if path.startswith(home) else path
-
-def splitpath4(pathfile):
-    '''return (long, short, file, ext), where:
-
-    • long is the long path to file, without ending slash
-    • short is the short path to file, without ending slash
-    • file is the file name, without extension
-    • ext is the file extension, without initial dot
-
-    >>> splitpath4('~/yyy/aaa.bbb.ccc')
-    ('/home/xxxx/yyy', '~/yyy', 'aaa.bbb', 'ccc')
-    >>> splitpath4('/home/xxxx/yyy/aaa.bbb.ccc')
-    ('/home/xxxx/yyy', '~/yyy', 'aaa.bbb', 'ccc')
-'''
-    long, filext = splitpath(longpath(pathfile))
-    short = shortpath(long)
-    fil, ext = splitext(filext)
-    return long, short, fil, ext[1:]
-
-def listfiles(pattern):
-    "return a list of absolute paths to pattern-matching files ('**' in path is allowed)"
-    return [file for file in glob(longpath(pattern), recursive=True) if isfile(file)]
-
-def getfile(pattern):
-    "return unique pattern-matching file, or '' if not found or ambiguous"
-    files = listfiles(pattern)
-    return files[0] if len(files) == 1 else ''
-
-def lastfile(pattern):
-    "return the newest path_file among matching path_files, or '' if not found"
-    files = listfiles(pattern)
-    return max((lstat(file).st_mtime, file) for file in files)[1] if files else ''
-
-def localfile(pathfile):
-    'return absolute path of a package relative pathfile'
-    return joinpath(splitpath(__file__)[0], pathfile)
-
-def listdirs(pattern):
-    "return a list of absolute paths to pattern-matching dirs ('**' in path is allowed)"
-    return [path for path in glob(longpath(pattern), recursive=True) if isdir(path)]
-
-def getdir(pattern):
-    "return unique pattern-matching dir, or '' if not found or ambiguous"
-    dirs = listdirs(pattern)
-    return dirs[0] if len(dirs) == 1 else ''
-
-def chdir2(pattern='~'):
-    '''like os.chdir(), but it accepts '~' '.' '..' '?' '*' '**' etc'''
-    paths = listdirs(pattern)
-    if not paths:
-        print(f'cd: path {pattern!r} not found', file=stderr)
-    elif len(paths) > 1:
-        print(f'cd: path {pattern!r} is ambiguous', file=stderr)
-    else:
-        chdir(paths[0])
-
-def newbackfile(file, YmdHMS=None):
-    'create a timestamped filename for backup of file'
-    path, ext = splitext(longpath(file))
-    return f'{path}-%04d.%02d.%02d-%02d.%02d.%02d{ext}' % (YmdHMS or localtime())[:6]
-
-def oldbackfile(file):
-    "return filename of the newest timestamped backup of file, or '' if not found"
-    path, ext = splitext(longpath(file))
-    return lastfile(f'{path}-????.??.??-??.??.??{ext}')
-
 #----- string functions -----
 
 def hold(string, charpattern, default=''):
-    'hold charpattern-matching chars in shrunk string and replace not matching chars with default'
+    'hold charpattern-matching chars in string and replace not matching chars with default'
     return ''.join(char if fnmatchcase(char, charpattern) else default for char in string)
 
 def take(string, charset, default=''):
-    'take chars in shrunk string found in charset and replace not found chars with default'
+    'take chars in string found in charset and replace not found chars with default'
     return ''.join(char if char in charset else default for char in string)
 
 def drop(string, charset, default=''):
-    'drop chars in shrunk string found in charset and replace not found chars with default'
+    'drop chars in string found in charset and replace not found chars with default'
     return ''.join(default if char in charset else char for char in string)
 
 def chars(charpattern):
     'return a sorted string of all charpattern-matching characters'
     kernel = charpattern[1:-1]
     a, z = ord(min(kernel)), ord(max(kernel)) + 1
     return ''.join(chr(j) for j in range(a, z) if fnmatchcase(chr(j), charpattern))
 
-def upperin(string):
-    'there is an uppercase letter in string?'
-    return string != string.lower()
-
-def lowerin(string):
-    'there is a lowercase letter in string?'
-    return string != string.upper()
-
-def letterin(string):
-    'there is a letter in string?'
-    return string != string.lower() or string != string.upper()
-
-def digitin(string):
-    'there is a digit in string?'
-    return any('0' <= char <= '9' for char in string)
-
-def specialin(string):
-    'there is a special (not alphanumeric) character in string?'
-    return any(char == char.lower() == char.upper() and not '0' <= char <= '9' for char in string)
-
-def split(string, separator=None):
-    'return [] if not string else string.split(separator)'
-    return [] if not string else string.split(separator)
+def ispattern(string):
+    'is string a fnmatch pattern?'
+    return bool(take(string, '?*['))
+
+def split_lines(string):
+    "split_lines('aaa\nbbb\n') -> ['aaa', 'bbb'], split_lines('') -> []"
+    string = string.rstrip()
+    return [] if not string else [line.rstrip() for line in string.split('\n')]
 
 def replace(string, *oldsnews):
     'replace(string, a, b, c, d, ...) == string.replace(a, b).replace(c, d)...'
     for j in range(0, len(oldsnews), 2):
         string = string.replace(oldsnews[j], oldsnews[j+1])
     return string
 
-def change(string, olds, news, char='%'):
-    'replace char + x with y for x, y in zip(olds, news)'
+def evalchar(string, olds, news, char='%'):
+    '''for old, new in zip(olds, news): string = string.replace(char + old, new)
+on error raise ValueError('%x')'''
     trans = {old: new for old, new in zip(olds, news)}
     trans[char] = char # char + char --> char
     value = ''
     skip = False
-    for j, charj in enumerate(string):
+    j = 0
+    while j < len(string):
+        charj = string[j]
         if charj == char:
             try:
                 value += trans[string[j+1]]
             except (KeyError, IndexError):
                 raise ValueError(string[j:j+2])
             else:
-                skip = True
-        elif skip:
-            skip = False
+                j += 1
         else:
             value += charj
+        j += 1
     return value
 
 def shrink(string, joinby=' ', splitby=None):
     'eliminate from string all leading, multiple and trailing blanks'
     return joinby.join(string.split(splitby))
 
+def adjust(string, length, align='!'):
+    "adjust string, align: '<'=left, '!'=center, '>'=right"
+    return (string.ljust(length) if align == '<' else
+            string.rjust(length) if align == '>' else
+            string.center(length))
+
+def frame(lines, align='!'):
+    "frame around lines, align: '<'=left, '!'=center, '>'=right"
+    if isinstance(lines, str):
+        lines = lines.split('\n')
+    length = max(len(line) for line in lines)
+    updown = (length + 2) * '─'
+    result = [f'┌{updown}┐']
+    for line in lines:
+        result.append(f'│ {adjust(line, length, align)} │')
+    return '\n'.join(result + [f'└{updown}┘'])
+
 def expand(string, width):
     "insert blanks into string until len(string) == width, on error return ''"
     string = shrink(string)
     if len(string) == width:
         return string
     if ' ' not in string[1:] or len(string) > width:
         raise ValueError(f'Impossible to right-justify: {string!r}')
@@ -285,15 +234,15 @@
     jchar = 0
     while True:
         if chars[jchar] != ' ' and chars[jchar + 1] == ' ':
             chars.insert(jchar + 1, ' ')
             if len(chars) == width:
                 return ''.join(chars)
         jchar = jchar + 1 if jchar < len(chars) - 2 else 0
-        
+
 def findchar(string, pattern):
     'return index of first pattern-matching char found in string, or -1 if not found'
     for j, char in enumerate(string):
         if fnmatchcase(char, pattern):
             return j
     else:
         return -1
@@ -303,68 +252,70 @@
     for j, char in retroenum(string):
         if fnmatchcase(char, pattern):
             return j
     else:
         return -1
 
 def prevchar(char):
-    "return chr(ord(char) - 1)"
+    """>>> prevchar('b')
+'a'
+"""
     return chr(ord(char) - 1)
 
 def nextchar(char):
-    "return chr(ord(char) + 1)"
+    """>>> nextchar('a')
+'b'
+"""
     return chr(ord(char) + 1)
 
-def chrs(jj):
-    "return ''.join(chr(j) for j in jj)"
-    return ''.join(chr(j) for j in jj)
+def chrs(list):
+    """>>> chrs([97, 98, 99])
+'abc'
+"""
+    return ''.join(chr(j) for j in list)
 
 def ords(string):
-    'return [ord(char) for char in string]'
+    """>>> ords('abc')
+[97, 98, 99]
+"""
     return [ord(char) for char in string]
 
-def uppunqshr(string, quotes='"'):
-    '''uppercase unquoted chars in shrunk string
+def unqupper(string, quotes='"'):
+    '''uppercase unquoted chars in string
 '''
     result = ''; quote = ''
-    for char in ' '.join(string.split()): # ... in shrink(string):
+    for char in string:
         if quote:
             result += char
             if char == quote:
                 quote = ''
         else:
             result += char.upper()
             if char in quotes:
                 quote = char
     return result
-            
-def lowunqshr(string, quotes='"'):
-    '''lowercase unquoted chars in shrunk string
->>> print(lowunqshr("""aAa 'bBb' cCc "dDd" eEe"""))
-aaa 'bBb' ccc "dDd" eee
-'''
+
+def unqlower(string, quotes='"'):
+    '''lowercase unquoted chars in string'''
     result = ''; quote = ''
-    for char in ' '.join(string.split()): # ... in shrink(string):
+    for char in string:
         if quote:
             result += char
             if char == quote:
                 quote = ''
         else:
             result += char.lower()
             if char in quotes:
                 quote = char
     return result
-            
-def titunqshr(string, quotes='"'):
-    '''titlecase unquoted chars in shrunk string
->>> print(titunqshr("""aAa 'bBb' cCc "dDd" eEe"""))
-Aaa 'bBb' Ccc "dDd" Eee
-'''
+
+def unqtitle(string, quotes='"'):
+    '''titlecase unquoted chars in string'''
     result = ''; quote = ''; first = True
-    for char in ' '.join(string.split()): # ... in shrink(string):
+    for char in string:
         if quote:
             result += char
             first = True
             if char == quote:
                 quote = ''
         elif char.isalpha():
             result += char.upper() if first else char.lower()
@@ -391,29 +342,30 @@
 >>> print(plural(3, 'mouse'))
 3 mouses
 >>> print(plural(3, 'mouse', 'mice'))
 3 mice
 '''
     return f'1 {sing}' if num == 1 else f'{num} {plur}' if plur else f'{num} {sing}s'
 
-def edit(item, width=0, ndig=None):
-    'convert item to str, justifying numbers at right and anything else at left'
+def edit(item, width=0, ndig=None, right=False):
     if isinstance(item, int):
         return str(item).rjust(width)
     elif isinstance(item, float):
         string = str(item if ndig is None else round(item, ndig))
         return (string[:-2] if string.endswith('.0') else string).rjust(width)
+    elif right:
+        return str(item).rjust(width)
     else:
         return str(item).ljust(width)
 
 def table(head, body, ndig=None):
     '''
 >>> for line in table(('n', 'n2', 'n3'),
-	[(n, n * n, n ** 3) for n in range(11)]):
-	print(f'    {line}')
+    [(n, n * n, n ** 3) for n in range(11)]):
+    print(f'    {line}')
 
     ┌──┬───┬────┐
     │N │ N2│ N3 │
     ├──┼───┼────┤
     │ 0│  0│   0│
     │ 1│  1│   1│
     │ 2│  4│   8│
@@ -424,28 +376,141 @@
     │ 7│ 49│ 343│
     │ 8│ 64│ 512│
     │ 9│ 81│ 729│
     │10│100│1000│
     └──┴───┴────┘
 '''
     head = [name.upper() for name in head]
-    wids = [len(name) for name in head]
+    widths = [len(name) for name in head]
     lenhead = len(head)
+    result = []
     for jrow, row in enumerate(body):
         row = tuple(row[:lenhead]) + (lenhead - len(row)) * ('',)
         for jcol, item in enumerate(row):
-            wids[jcol] = max(wids[jcol], len(edit(item, 0, ndig)))
+            widths[jcol] = max(widths[jcol], len(edit(item, 0, ndig)))
         body[jrow] = row
-    yield('┌' + '┬'.join(wid * '─' for wid in wids) + '┐')
-    yield('│' + '│'.join(name.center(wid) for name, wid in zip(head, wids)) + '│')
-    yield('├' + '┼'.join(wid * '─' for wid in wids) + '┤')
+    result.append('┌' + '┬'.join(width * '─' for width in widths) + '┐')
+    result.append('│' + '│'.join(name.center(width) for name, width in zip(head, widths)) + '│')
+    result.append('├' + '┼'.join(width * '─' for width in widths) + '┤')
     for row in body:
-        yield('│' + '│'.join(edit(item, wid, ndig) for item, wid in zip(row, wids)) + '│')
-    yield('└' + '┴'.join(wid * '─' for wid in wids) + '┘')
-    
+        result.append('│' + '│'.join(edit(item, width, ndig) for item, width in zip(row, widths)) + '│')
+    result.append('└' + '┴'.join(width * '─' for width in widths) + '┘')
+    return result
+
+def int2roman(number):
+    '''
+>>> int2roman(0)
+''
+>>> int2roman(3999)
+'mmmcmxcix'
+'''
+    if number not in range(4000):
+        raise ValueError
+    m, c, x, i = [int(digit) for digit in f'{number:04}']
+    return (['','m','mm','mmm'][m] +
+            ['','c','cc','ccc','cd','d','dc','dcc','dccc','cm'][c] +
+            ['','x','xx','xxx','xl','l','lx','lxx','lxxx','xc'][x] +
+            ['','i','ii','iii','iv','v','vi','vii','viii','ix'][i])
+
+#----- path & file functions -----
+
+def join_path(*paths):
+    '''
+>>> join_path('/a/b/', '/c/d.e')
+'/a/b/c/d.e'
+>>> join_path('/a/b', 'c/d.e')
+'/a/b/c/d.e'
+''' 
+    return normpath(path_sep.join(paths))
+
+def long_path(path='.'):
+    path = (path or '').strip()
+    return '' if not path else abspath(expanduser(path))
+
+def short_path(path='.'):
+    path, home = long_path(path), long_path('~')
+    return '' if not path else '~' + path[len(home):] if path.startswith(home) else path
+
+def get_files(pattern):
+    "return a list of absolute paths to pattern-matching files ('**' in path is allowed)"
+    return [file for file in glob(long_path(pattern), recursive=True) if isfile(file)]
+
+def get_file(pattern):
+    "return unique pattern-matching file, or '' if not found or ambiguous"
+    files = get_files(pattern)
+    return files[0] if len(files) == 1 else ''
+
+def get_lines(file):
+    "like lines in open(file).readlines(), but normalized"
+    return [line.rstrip().replace('\t','    ') for line in open(file)]
+
+def max_file(pattern):
+    "return the max path_file among matching path_files, or raise FileNotFoundError if not found"
+    files = get_files(pattern)
+    if files:
+        return max(files)
+    else:
+        raise FileNotFoundError
+
+def last_file(pattern):
+    "return the newest path_file among matching path_files, or raise FileNotFoundError if not found"
+    files = get_files(pattern)
+    if files:
+        return max((lstat(file).st_mtime, file) for file in files)[1]
+    else:
+        raise FileNotFoundError
+
+def get_PpfFeYmdHMS(file):
+    '''return (P, p, f, F, e, Y, m, d, H, M, S), where:
+    • P is long path to file, without final '/'
+    • p is short path to file, without final '/'
+    • f is file name, with no extension
+    • F is file name, with no extension, spaced and titlecased
+    • e is file extension, starting with '.'
+    • Y is 4-digit current year
+    • m, d, H, M, S are 2-digit current month, day, hour, minute, second'''
+    P, f_e = splitpath(long_path(file))
+    p = short_path(P)
+    f, e = splitext(f_e)
+    F = hold(f, '[a-zA-Z0-9]', ' ').title()
+    return (P, p, f, F, e) + get_YmdHMS()
+
+def new_file(pattern, char='%'):
+    'return not existing expanded pathfile, initialize file as empty'
+    while True:
+        file = long_path(evalchar(pattern, 'YmdHMS', get_YmdHMS(), char=char))
+        if char in pattern and isfile(file):
+            sleep(0.1)
+        else:
+            open(file, 'w').write('')
+            return file
+        
+def local_file(pathfile):
+    'return absolute path of a package relative pathfile'
+    return normpath(f'{dirname(__file__)}/{pathfile}')
+
+def get_dirs(pattern):
+    "return a list of absolute paths to pattern-matching dirs ('**' in path is allowed)"
+    return [path for path in glob(long_path(pattern), recursive=True) if isdir(path)]
+
+def get_dir(pattern):
+    "return unique pattern-matching dir, or '' if not found or ambiguous"
+    dirs = get_dirs(pattern)
+    return dirs[0] if len(dirs) == 1 else ''
+
+def chdir2(pattern='~'):
+    '''like os.chdir(), but it accepts '~' '.' '..' '?' '*' '**' etc'''
+    paths = get_dirs(pattern)
+    if not paths:
+        print(f'cd: path {pattern!r} not found', file=stderr)
+    elif len(paths) > 1:
+        print(f'cd: path {pattern!r} is ambiguous', file=stderr)
+    else:
+        chdir(paths[0])
+
 #----- sequence functions -----
 
 def retroenum(sequence):
     'like enumerate(sequence), but backwards from last to first item'
     for j in range(len(sequence) - 1, -1, -1):
         yield j, sequence[j]
 
@@ -461,294 +526,362 @@
     'return index of last item found in sequence, or -1 if not found'
     for j, itemj in retroenum(sequence):
         if itemj == item:
             return j
     else:
         return -1
 
-def get(sequence, index, default=None):
-    'return sequence[index] if 0 <= index < len(sequence) else default'
-    return sequence[index] if 0 <= index < len(sequence) else default
+def index(sequence, item):
+    'return index of first item found in sequence, or raise ValueError if not found'
+    for j, itemj in enumerate(sequence):
+        if itemj == item:
+            return j
+    else:
+        raise ValueError('item not found')
+
+def rindex(sequence, item):
+    'return index of last item found in sequence, or raise ValueError if not found'
+    for j, itemj in retroenum(sequence):
+        if itemj == item:
+            return j
+    else:
+        raise ValueError('item not found')
 
-def unique(sequence):
-    'return copy of sequence with no duplicate items'
+def get(xx, j, default=None):
+    'return xx[j] if 0 <= j < len(xx) else default'
+    return xx[j] if 0 <= j < len(xx) else default
+
+def unique(xx):
+    'return copy of list xx with no duplicates'
     olds = set()
     result = []
-    for item in sequence:
-        if item not in olds:
-            olds.add(item)
-            result.append(item)
+    for x in xx:
+        if x not in olds:
+            olds.add(x)
+            result.append(x)
     return result
 
 #----- shell functions -----
 
-def shell(command, mode='p', file=stdout):
-    '''
-minimal shell, stderr is not piped
-if 'C' in mode: print command
-if 'p' in mode: pipe stdout and return stdout as a list of lines
-if 'P' in mode: pipe stdout, print stdout on file and return stdout as a list of lines
-if 'p' not in mode and 'P' not in mode: stdout is not piped, return []
-'''
-    if 'C' in mode:
-        print(f'{shortpath()} --> {command}', file=file)
-    command, out = command.strip(), []
-    if command == 'cd':
-        chdir2()
-    elif command.startswith('cd '):
-        chdir2(command[3:].strip())
-    else:
-        result = run(command, shell=True, text=True, stdout=PIPE if 'p' in mode.lower() else None)
-        out = [line.rstrip() for line in (result.stdout or '').split('\n') if line.rstrip()]
-        if 'P' in mode:
-            for line in out:
-                print(line, file=file)
-    return out
+def shell(command, echo=False):
+    if echo:
+        print('--> ' + command)
+    nocomment = command.split('#')[0].strip()
+    if nocomment == 'exit' or nocomment.startswith('exit '):
+        raise SystemExit
+    elif nocomment == 'cd' or nocomment.startswith('cd '):
+        where = nocomment[3:].strip() or '~'
+        paths = glob(long_path(where))
+        if not paths:
+            print(f'cd: {where!r}: No such file or directory', file=stderr)
+        elif len(paths) > 1:
+            print(f'cd: too many arguments', file=stderr)
+        else:
+            chdir(paths[0])
+        return []
+    else:
+        result = run(command.strip(), shell=True, text=True, capture_output=True)
+        for line in split_lines(result.stderr):
+            print(line, file=stderr)
+        return split_lines(result.stdout)
 
-def term(mode='P', file=stdout):
-    '''
-minimal terminal, type 'exit' to exit, '#'-comments not allowed"
-'''
-    print(70 * '<')
+def term():
+    print(frame('term - minimalistic terminal'))
     while True:
-        command = input(f'{shortpath()} --> ')
-        if command.split('#')[0].strip() == 'exit':
-            break
-        shell(command, mode=mode, file=file)
-    print(70 * '>')
+        try:
+            command = input(f"{abspath('.')} $ ")
+            try:
+                for line in shell(command):
+                    print(line)
+            except SystemExit:
+                break
+        except KeyboardInterrupt:
+            print('^C')
+    print(frame("term - terminated by 'exit'"))
+
+def command_exists(command):
+    return bool(shell(f'which {command}'))
 
 #----- metric functions -----
 
 in2in = lambda In: float(In) # inch converters
 in2pt = lambda In: In * 72.0
 pt2in = lambda pt: pt / 72.0
 in2cm = lambda In: In * 2.54
 cm2in = lambda cm: cm / 2.54
 in2mm = lambda In: In * 25.4
 mm2in = lambda mm: mm / 25.4
 
-def in2str(inch, units='pt in mm cm', ndig=3):
+def inch2str(inch, digits):
     'convert float inch into a multi-unit human-readable string'
-    return ' = '.join(str(round({'pt': in2pt, 'in': in2in, 'mm': in2mm, 'cm': in2cm}[unit](inch), ndig)) + unit for unit in units.split())
-    
-def str2in(string):
-    '''convert '{float}{suffix}' into an inch float value
-on error raise ValueError or KeyError
-suffix can be: 'pt' = point, 'in' = inch, 'mm' = millimeter or 'cm' = centimeter
-only zero value (as '0', '0.0'...) can lack the suffix
-'''
-    if tryfunc(float, (string,), 1.0) == 0.0:
+    in2xx = {'pt': in2pt, 'in': in2in, 'mm': in2mm, 'cm': in2cm}
+    return ' = '.join(f"{in2xx[unit](inch):.{digits}f}{unit}" for unit in ['pt','in','mm','cm'])
+
+def str2inch(string):
+    "convert '{float}{suffix}' into an inch float value"
+    string = replace(string,' ','',',','.')
+    try:
+        assert float(string) == 0.0
         return 0.0
-    else:
-        return {'pt': pt2in, 'in': in2in, 'mm': mm2in, 'cm': cm2in}[string[-2:]](float(string[:-2]))
-      
+    except:
+        xx2in = {'pt': pt2in, 'in': in2in, 'mm': mm2in, 'cm': cm2in}
+        try:
+            value = xx2in[string[-2:]](float(string[:-2]))
+            assert value >= 0.0
+            return value
+        except:
+            raise ValueError
+
 def str2inxin(string):
-    '''convert '{float}x{float}{suffix}' into two inch float values
-on error raise ValueError or KeyError
-suffix can be: 'pt' = point, 'in' = inch, 'mm' = millimeter or 'cm' = centimeter
-'''
-    left, right = string.split('x')
-    return str2in(left + right[-2:]), str2in(right)
+    "convert '{float}x{float}{suffix}' into two inch float values"
+    try:
+        a, b = string.split('x')
+        x, y = str2inch(a + b[-2:]), str2inch(b)
+        return (x, y)
+    except:
+        raise ValueError
 
 def ratio(string):
-    '''convert '{float}/{float}' or '{float}' into a float value
-on error raise ValueError or ZeroDivisionError
+    '''convert '{float}/{float}' or '{float}' into a float
+float value(s) must be positive
 '''
-    if '/' in string:
-        over, under = string.split('/')
-        return float(over) / float(under)
-    else:
-        return float(string)
-    
+    string = replace(string,' ','',',','.')
+    try:
+        r = float(string)
+        assert r > 0
+        return r
+    except (ValueError, AssertionError):
+        try:
+            a, b = string.split('/')
+            a, b = float(a), float(b)
+            assert a > 0 < b
+            return a / b
+        except (ValueError, AssertionError):
+            raise ValueError
+
 #----- numeric functions -----
 
-def frange(start, stop, step, first=True, last=False):
+def frange(start, stop=None, step=1.0, first=True, last=False):
     """float range
 >>> list(frange(0, 1, 1/3, last=True))
 [0.0, 0.3333333333333333, 0.6666666666666666, 1.0]
 >>> list(frange(1, 0, -1/3, last=True))
 [1.0, 0.6666666666666667, 0.33333333333333337, 0.0]"""
+    if stop is None:
+        start, stop = 0.0, start
     start, stop, step = float(start), float(stop), float(step)
     if first:
         yield start
     for j in range(1, round((stop - start) / step)):
         yield start + j * step
     if last:
         yield stop
 
-def linterpol(xyxy, x=None):
-    '''linear interpolation (by least squares if len(xyxy) > 2)
-xyxy = [(x, y), (x, y),...], len(xyxy) = n
-if x is None: return (a, b, err) such that:
-    . y = a * x + b is the interpolating line
-    . err = sqrt(sum((a * x + b - y) ** 2) / n)
-else: return a * x + b
-'''
+def difs(xx):
+    return [xj - xx[j-1] if j else xj for j, xj in enumerate(xx)]
+            
+def sums(xx):
+    yy = xx[:]
+    for j in range(1, len(yy)):
+        yy[j] += yy[j - 1]
+    return yy
+
+def broken_line(xyxy, x):
+    '''linear interpolation by broken line
+xyxy = [(x0, y0), (x1, y1), (x2, y2),...]
+0.0 <= x0 < x1 < x2 ...
+0.0 <= y0 < y1 < y2 ...'''
+    n = len(xyxy)
+    if n == 0: # straight line by [(0.0, 0.0), (1.0, 1.0)]
+        return  x
+    elif n == 1: # straight line by [(0.0, 0.0), (x0, y0)]
+        x0, y0 = xyxy[0]
+        return (y0 / x0) * x
+    elif n == 2: # straight line by [(x0, y0), (x1, y1)]
+        x0, y0 = xyxy[0]
+        x1, y1 = xyxy[1]
+        d = x1 - x0
+        a = (y1 - y0) / d
+        b = (y0 * x1 - y1 * x0) / d
+        return a * x + b
+    else: # broken line by [(x0, y0), (x1, y1), (x2, y2),...]
+        for j, (x0, y0) in enumerate(xyxy):
+            x1, y1 = xyxy[j + 1]
+            if j >= n - 2 or x <= x1:
+                return y0 + (x - x0) * (y1 - y0) / (x1 - x0)
+
+def least_squares_line(xyxy, x):
+    '''linear interpolation by least-squares straight line
+xyxy = [(x0, y0), (x1, y1), (x2, y2),...]
+for j > 0: x[j] > x[j - 1] and y[j] > y[j -1 ]'''
     n = len(xyxy)
     if n == 0: # straight line by [(0.0, 0.0), (1.0, 1.0)]
-        value =  (1.0, 0.0, 0.0) if x is None else x
+        return  x
     elif n == 1: # straight line by [(0.0, 0.0), (x0, y0)]
         x0, y0 = xyxy[0]
-        value =  (y0 / x0, 0.0, 0.0) if x is None else (y0 / x0) * x
+        return (y0 / x0) * x
     elif n == 2: # straight line by [(x0, y0), (x1, y1)]
         x0, y0 = xyxy[0]
         x1, y1 = xyxy[1]
         d = x1 - x0
         a = (y1 - y0) / d
         b = (y0 * x1 - y1 * x0) / d
-        value =  (a, b, 0.0) if x is None else a * x + b
-    else: # n > 2, least squares straight line by [(x0, y0), (x1, y1), (x2, y2), ...]
+        return a * x + b
+    else: # least-squares straight line by [(x0, y0), (x1, y1), (x2, y2),...]
         sx = sum(x for x, y in xyxy)
         sx2 = sum(x * x for x, y in xyxy)
         sy = sum(y for x, y in xyxy)
         sxy = sum(x * y for x, y in xyxy)
         d = n * sx2 - sx * sx
         a = (n * sxy - sx * sy) / d
         b = (sx2 * sy - sx * sxy) / d
-        err = (sum((a * x + b - y) ** 2 for x, y in xyxy) / n) ** 0.5
-        value =  (a, b, err) if x is None else a * x + b
-    return value
+        return a * x + b
 
 def moving_means(xx, n=7):
     """return [yy[j] = sum(xx[j+1-n:j+1]) / n]
 >>> moving_means(list(range(10)))
 [0.0, 0.5, 1.0, 1.5, 2.0, 2.5, 3.0, 4.0, 5.0, 6.0]
 >>> moving_means(list(range(10)), 3)
 [0.0, 0.5, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0]
 """
     return [sum(xx[max(0, j + 1 - n): j + 1]) / min(n, j + 1) for j in range(len(xx))]
 
-#----- messages -----
-
-def inform(message):
-    'print an information message and continue'
-    print(message, file=stderr)
-
-def warning(message, jline=-1, line=''):
-    'print a warning message and continue'
-    if jline > -1:
-        print(f'LINE {jline+1}: {line}', file=stderr)
-    print(f'WARNING: {message}', file=stderr)
-
-def error(message, jline=None, line=''):
-    'print an error message and exit'
-    if jline is not None:
-        print(f'LINE {jline+1}: {line.rstrip()}', file=stderr)
-    exit(f'ERROR: {message}')
-
 #----- other functions -----
 
-def tryfunc(func, args, default=None):
-    'try: return func(*args); except: return default'
+def now():
+    "return 'YYYY-mm-dd HH:MM:SS'"
+    Y, m, d, H, M, S = localtime()[:6]
+    return f'{Y:04d}-{m:02d}-{d:02d} {H:02d}:{M:02d}:{S:02d}'
+
+def today():
+    "return 'YYYY-mm-dd'"
+    Y, m, d = localtime()[:3]
+    return f'{Y:04d}-{m:02d}-{d:02d}'
+
+def get_YmdHMS():
+    "return ('YYYY','mm','dd','HH','MM','SS')"
+    Y, m, d, H, M, S = localtime()[:6]
+    return tuple(f'{Y:04d} {m:02d} {d:02d} {H:02d} {M:02d} {S:02d}'.split())
+    
+def get_Ymd():
+    "return ('YYYY','mm','dd')"
+    Y, m, d = localtime()[:3]
+    return tuple(f'{Y:04d} {m:02d} {d:02d}'.split())
+    
+def try_func(func, args, on_error=None):
+    'try: return func(*args); except: return on_error'
     try:
         return func(*args)
     except:
-        return default
+        return on_error
+
+def try_func1(func, arg, on_error=None):
+    'try: return func(arg); except: return on_error'
+    try:
+        return func(arg)
+    except:
+        return on_error
 
 def idem(x):
     'return x'
     return x
 
 def dump(object, undertoo=False):
     items = sorted((key, value) for key, value in object.__dict__.items() if undertoo or not key.startswith('_'))
     length = max((len(key) for key, value in items), default=0)
     for key, value in items:
-        value = (in2str if isinstance(value, float) else str)(value)
-        print(f'    {edit(key, length)} = {value}')
+        value = (inch2str if isinstance(value, float) else str)(value)
+        print(f'    {edit(key, length)}\t = {value!r}')
 
-def show(names, *vars):
+def show(names):
     '''
->>> a, b, c = 'xyz'; show('a, b, c', a, b, c)
+>>> a, b, c = 'xyz'; show('a, b, c')
 a = 'x'
 b = 'y'
 c = 'z'
 '''
     names = [name.strip() for name in names.split(',')]
-    assert len(names) == len(vars), f'show(): {len(names)} names but {len(vars)} vars'
-    for name, var in zip(names, vars):
+    for name in names:
+        var = eval(name)
         if isinstance(var, tuple):
             if not var:
                 print(name, '= ()')
             else:
                 print(name, '= (')
                 for j, v in enumerate(var):
-                    print(f'    {v!r},{")"*(j==len(var)-1)}')
+                    print(f'    {v!r},')
+                print('    )')
         elif isinstance(var, list):
             if not var:
                 print(name, '= []')
             else:
                 print(name, '= [')
                 for j, v in enumerate(var):
-                    print(f'    {v!r},{"]"*(j==len(var)-1)}')
+                    print(f'    {v!r},')
+                print('    ]')
         elif isinstance(var, dict):
             if not var:
                 print(name, '= {}')
             else:
                 print(name, '= {')
                 for j, (k, v) in enumerate(sorted(var.items())):
-                    print(f'    {k!r}: {v!r},{"}"*(j==len(var)-1)}')
+                    print(f'    {k!r}: {v!r},')
+                print('    }')
         elif isinstance(var, (set, frozenset)):
             if not var:
                 print(name, '= set()')
             else:
                 print(name, '= {')
                 for j, v in enumerate(sorted(var)):
-                    print(f'    {v!r},{"}"*(j==len(var)-1)}')
+                    print(f'    {v!r},')
+                print('    }')
         else:
             print(f'{name} = {var!r}')
 
-#----- classes -----
+#----- dict subclasses -----
 
 class ListDict(dict):
     'dictionary of lists'
 
+    def __getitem__(listdict, key):
+        return listdict.get(key, [])
+
     def append(listdict, key, value):
         if key not in listdict:
             listdict[key] = []
         listdict[key].append(value)
 
-    def __getitem__(listdict, key):
-        return listdict.get(key, [])
-
 class SetDict(dict):
     'dictionary of sets'
 
+    def __getitem__(setdict, key):
+        return setdict.get(key, set())
+
     def add(setdict, key, value):
         if key not in setdict:
             setdict[key] = set()
         setdict[key].add(value)
 
-    def __getitem__(setdict, key):
-        return setdict.get(key, set())
-
-#----- yawp-specific functions -----
-
-def chapter_level(prefix):
-    status = 0; level = 0
-    for char in prefix:
-        if status == 0:
-            if char.isdecimal():
-                status = 1
-            else:
-                return 0
-        else: # status == 1
-            if char.isdecimal():
-                pass
-            elif char == '.':
-                level += 1
-                status = 0
-            else:
-                return 0
-    return level if status == 0 else 0
-
-def figure_level(prefix):
-    if fnmatchcase(prefix, '[a-z].'):
-        return 1
-    elif not fnmatchcase(prefix, '*[a-z].'):
-        return 0
-    else:
-        chaplevel = chapter_level(prefix[:-2])
-        return 0 if chaplevel == 0 else chaplevel + 1
+#----- PySimpleGUI-related functions -----
 
+def get_radio(window, start, chars):
+    ntrue = 0
+    for j, charj in enumerate(chars):
+        if window[start + j].get():
+            ntrue += 1
+            char = charj
+    if ntrue != 1:
+        raise ValueError
+    return char
+
+def put_radio(window, start, chars, char):
+    ntrue = 0
+    for j, charj in enumerate(chars):
+        if charj == char:
+            ntrue += 1
+            window[start + j].update(True)
+        else:
+            window[start + j].update(False)
+    if ntrue != 1:
+        raise ValueError
+ 
 #----- end -----
-
-
```

