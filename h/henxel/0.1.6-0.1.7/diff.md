# Comparing `tmp/henxel-0.1.6.tar.gz` & `tmp/henxel-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henxel-0.1.6.tar", last modified: Mon Mar 13 10:36:41 2023, max compression
+gzip compressed data, was "henxel-0.1.7.tar", last modified: Sat Mar 18 09:21:05 2023, max compression
```

## Comparing `henxel-0.1.6.tar` & `henxel-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-03-13 10:36:41.375196 henxel-0.1.6/
--rw-r--r--   0 samuel    (1000) samuel    (1000)    34801 2023-02-23 18:22:17.000000 henxel-0.1.6/LICENSE
--rw-r--r--   0 samuel    (1000) samuel    (1000)       50 2022-12-03 19:30:56.000000 henxel-0.1.6/MANIFEST.in
--rw-r--r--   0 samuel    (1000) samuel    (1000)     5051 2023-03-13 10:36:41.375196 henxel-0.1.6/PKG-INFO
--rw-r--r--   0 samuel    (1000) samuel    (1000)     4406 2023-03-13 09:44:43.000000 henxel-0.1.6/README.md
--rw-r--r--   0 samuel    (1000) samuel    (1000)       98 2023-03-13 09:40:40.000000 henxel-0.1.6/pyproject.toml
--rw-r--r--   0 samuel    (1000) samuel    (1000)      765 2023-03-13 10:36:41.375196 henxel-0.1.6/setup.cfg
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-03-13 10:36:41.367192 henxel-0.1.6/src/
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-03-13 10:36:41.375196 henxel-0.1.6/src/henxel/
--rw-r--r--   0 samuel    (1000) samuel    (1000)    91422 2023-03-13 10:34:13.000000 henxel-0.1.6/src/henxel/__init__.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     6358 2023-02-23 18:21:27.000000 henxel-0.1.6/src/henxel/changefont.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      359 2022-12-03 19:17:18.000000 henxel-0.1.6/src/henxel/editor.png
--rw-r--r--   0 samuel    (1000) samuel    (1000)     7218 2023-02-17 17:42:15.000000 henxel-0.1.6/src/henxel/fdialog.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     6190 2023-03-13 09:38:09.000000 henxel-0.1.6/src/henxel/help.txt
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-03-13 10:36:41.375196 henxel-0.1.6/src/henxel.egg-info/
--rw-r--r--   0 samuel    (1000) samuel    (1000)     5051 2023-03-13 10:36:41.000000 henxel-0.1.6/src/henxel.egg-info/PKG-INFO
--rw-r--r--   0 samuel    (1000) samuel    (1000)      302 2023-03-13 10:36:41.000000 henxel-0.1.6/src/henxel.egg-info/SOURCES.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)        1 2023-03-13 10:36:41.000000 henxel-0.1.6/src/henxel.egg-info/dependency_links.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)        7 2023-03-13 10:36:41.000000 henxel-0.1.6/src/henxel.egg-info/top_level.txt
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-03-18 09:21:05.883043 henxel-0.1.7/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    34801 2023-02-23 18:22:17.000000 henxel-0.1.7/LICENSE
+-rw-r--r--   0 samuel    (1000) samuel    (1000)       50 2022-12-03 19:30:56.000000 henxel-0.1.7/MANIFEST.in
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     5051 2023-03-18 09:21:05.883043 henxel-0.1.7/PKG-INFO
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     4406 2023-03-13 09:44:43.000000 henxel-0.1.7/README.md
+-rw-r--r--   0 samuel    (1000) samuel    (1000)       98 2023-03-13 09:40:40.000000 henxel-0.1.7/pyproject.toml
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      765 2023-03-18 09:21:05.883043 henxel-0.1.7/setup.cfg
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-03-18 09:21:05.863042 henxel-0.1.7/src/
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-03-18 09:21:05.879042 henxel-0.1.7/src/henxel/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    92239 2023-03-18 09:15:34.000000 henxel-0.1.7/src/henxel/__init__.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     6358 2023-02-23 18:21:27.000000 henxel-0.1.7/src/henxel/changefont.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      359 2022-12-03 19:17:18.000000 henxel-0.1.7/src/henxel/editor.png
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     7218 2023-03-17 08:57:46.000000 henxel-0.1.7/src/henxel/fdialog.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     7110 2023-03-18 09:14:12.000000 henxel-0.1.7/src/henxel/help.txt
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-03-18 09:21:05.883043 henxel-0.1.7/src/henxel.egg-info/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     5051 2023-03-18 09:21:05.000000 henxel-0.1.7/src/henxel.egg-info/PKG-INFO
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      302 2023-03-18 09:21:05.000000 henxel-0.1.7/src/henxel.egg-info/SOURCES.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)        1 2023-03-18 09:21:05.000000 henxel-0.1.7/src/henxel.egg-info/dependency_links.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)        7 2023-03-18 09:21:05.000000 henxel-0.1.7/src/henxel.egg-info/top_level.txt
```

### Comparing `henxel-0.1.6/LICENSE` & `henxel-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `henxel-0.1.6/PKG-INFO` & `henxel-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henxel
-Version: 0.1.6
+Version: 0.1.7
 Summary: GUI-editor for Python development.
 Home-page: https://github.com/SamuelKos/henxel
 Author: SamuelKos
 Author-email: koskinens371@gmail.com
 Project-URL: Bug Tracker, https://github.com/SamuelKos/henxel/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `henxel-0.1.6/README.md` & `henxel-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `henxel-0.1.6/setup.cfg` & `henxel-0.1.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = henxel
-version = 0.1.6
+version = 0.1.7
 author = SamuelKos
 author_email = koskinens371@gmail.com
 description = GUI-editor for Python development.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/SamuelKos/henxel
 project_urls =
```

### Comparing `henxel-0.1.6/src/henxel/__init__.py` & `henxel-0.1.7/src/henxel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 # for executing edited file in the same env than this editor, which is nice:
 # It means you have your installed dependencies available. By self.run()
 import subprocess
 
 ############ Imports End
 ############ Class Tab Begin
-
+					
 class Tab:
 	'''	Represents a tab-page of an Editor-instance
 	'''
 	
 	def __init__(self, **entries):
 		self.active = True
 		self.filepath = None
@@ -99,15 +99,14 @@
 ############ Constants Begin
 CONFPATH = 'editor.cnf'
 ICONPATH = 'editor.png'
 HELPPATH = 'help.txt'
 VERSION = importlib.metadata.version(__name__)
 
 
-
 TAB_WIDTH = 4
 TAB_WIDTH_CHAR = ' '
 
 SLIDER_MINSIZE = 66
 
 
 GOODFONTS = [
@@ -416,27 +415,14 @@
 			self.btn_git.config(font=self.menufont)
 			
 			self.ln_widget.config(font=self.font, foreground=self.fgcolor, background=self.bgcolor, selectbackground=self.bgcolor, selectforeground=self.fgcolor, inactiveselectbackground=self.bgcolor, state='disabled')
 
 		
 		self.helptxt = f'{self.helptxt}\n\nHenxel v. {self.version}'
 		
-		# set cursor pos:
-		line = self.tabs[self.tabindex].position
-		self.contents.focus_set()
-		
-		try:
-			self.contents.mark_set('insert', line)
-			self.ensure_idx_visibility(line)
-			
-		except tkinter.TclError:
-			self.contents.mark_set('insert', '1.0')
-			self.tabs[self.tabindex].position = '1.0'
-			self.contents.see('1.0')
-			
 		
 		# Widgets are configured
 		###############################
 		#
 		# Syntax-highlight Begin #################
 		
 		self.keywords = [
@@ -500,15 +486,14 @@
 		
 		red = r'#c01c28'
 		cyan = r'#2aa1b3'
 		magenta = r'#a347ba'
 		green = r'#26a269'
 		orange = r'#e95b38'
 		gray = r'#508490'
-		#blue = r'#68c4e0'
 		
 		self.tagnames = [
 				'keywords',
 				'numbers',
 				'bools',
 				'strings',
 				'comments',
@@ -517,14 +502,15 @@
 				'selfs'
 				]
 		
 		self.boldfont = self.font.copy()
 		self.boldfont.config(weight='bold')
 		
 		self.contents.tag_config('keywords', font=self.boldfont, foreground='deep sky blue')
+		#self.contents.tag_config('tests', font=self.boldfont, foreground='khaki3')
 		self.contents.tag_config('numbers', font=self.boldfont, foreground=red)
 		self.contents.tag_config('comments', font=self.boldfont, foreground=gray)
 		self.contents.tag_config('breaks', font=self.boldfont, foreground=orange)
 		self.contents.tag_config('calls', font=self.boldfont, foreground=cyan)
 		
 		self.contents.tag_config('bools', foreground=magenta)
 		self.contents.tag_config('strings', foreground=green)
@@ -566,14 +552,28 @@
 		else:
 			self.contents.grid_configure(row=1, column=0, columnspan=4, sticky='nswe')
 			self.ln_widget.grid_remove()
 			
 		self.scrollbar.grid_configure(row=1,column=4, sticky='nse')
 		
 		
+		# set cursor pos:
+		line = self.tabs[self.tabindex].position
+		self.contents.focus_set()
+		
+		try:
+			self.contents.mark_set('insert', line)
+			self.ensure_idx_visibility(line)
+			
+		except tkinter.TclError:
+			self.contents.mark_set('insert', '1.0')
+			self.tabs[self.tabindex].position = '1.0'
+			self.contents.see('1.0')
+			
+			
 		self.update_idletasks()
 		self.viewsync()
 		self.__class__.alive = True
 		self.update_title()
 		
 		############################# init End ##########################
 		
@@ -588,112 +588,35 @@
 		return 'break'
 	
 		
 	def skip_bindlevel(self, event=None):
 		return 'continue'
 		
 	
-	def check_indent_depth(self, contents):
-		'''Contents is contents of py-file as string.'''
-		
-		words = [
-				'def ',
-				'if ',
-				'for ',
-				'while ',
-				'class '
-				]
-				
-		tmp = contents.splitlines()
-		
-		for word in words:
-			
-			for i in range(len(tmp)):
-				line = tmp[i]
-				if word in line:
-					
-					# Trying to check if at the beginning of new block:
-					if line.strip()[-1] == ':':
-						# Offset is num of empty lines between this line and next
-						# non empty line
-						nextline = None
-						
-						for offset in range(1, len(tmp)-i):
-							nextline = tmp[i+offset]
-							if nextline.strip() == '': continue
-							else: break
-							
-							
-						if not nextline:
-							continue
-						
-						
-						# Now should have next non empty line,
-						# so start parsing it:
-						flag_space = False
-						indent_0 = 0
-						indent_1 = 0
-		
-						for char in line:
-							if char in [' ', '\t']: indent_0 += 1
-							else: break
-		
-						for char in nextline:
-							# Check if indent done with spaces:
-							if char == ' ':
-								flag_space = True
-		
-							if char in [' ', '\t']: indent_1 += 1
-							else: break
-						
-						
-						indent = indent_1 - indent_0
-						#print(indent)
-						tests = [
-								( indent <= 0 ),
-								( not flag_space and indent > 1 )
-								]
-						
-						if any(tests):
-							#print('indent err')
-							#skipping
-							continue
-						
-						
-						# All is good, do nothing:
-						if not flag_space:
-							return False, 0
-							
-						# Found one block with spaced indentation,
-						# assuming it is used in whole file.
-						else:
-							if indent != self.ind_depth:
-								return True, indent
-							
-							else:
-								return False, 0
-					
-		return False, 0
-	
-	
 	def ensure_idx_visibility(self, index):
+		''' There seems to be inconsistency when contents of view of Text-widget is refreshed.
+			At least it is mystery to me. To test: search something common like: self.
+			Then start going backwards with ctrl-p until in place where multiple matches are
+			in same time visible in center of screen. Now try repeatedly multiple ctrl-n and ctrl-p
+			and notice the inconsistency yourself.
+		'''
 		
-		start = self.contents.bbox('%s - 2lines' % index)
-		end = self.contents.bbox('%s + 2lines' % index)
+		s = self.contents.bbox('%s - 2lines' % index)
+		e = self.contents.bbox('%s + 2lines' % index)
 		
 		tests = [
-				( not start ),
-				( not end ),
-				( start and start[1] < 0 )
+				( not s ),
+				( not e ),
+				( s and s[1] < 0 )
 				]
-		
+				
 		if any(tests):
-			self.contents.see('%s + 2lines' % index)
-			self.update_idletasks()
 			self.contents.see('%s - 2lines' % index)
+			self.update_idletasks()
+			self.contents.see('%s + 2lines' % index)
 			
 		
 	def quit_me(self):
 	
 		self.save(forced=True)
 		self.save_config()
 		
@@ -1314,29 +1237,33 @@
 			tmp = self.tabs[self.tabindex].contents
 			
 			
 		linenum = int(start_idx.split('.')[0])
 		flag_err = False
 		#print(self.token_err)
 		
+		
 		try:
 			with io.BytesIO( tmp.encode('utf-8') ) as fo:
 			
 				tokens = tokenize.tokenize( fo.readline )
 			
 				# Remove old tags:
 				for tag in self.tagnames:
 					self.contents.tag_remove( tag, start_idx, end_idx )
 					
 				# Retag:
 				for token in tokens:
 					#print(token)
+					
+					# token.line contains line as string which contains token.
+					
 					if token.type == tokenize.NAME or \
 						( token.type in [ tokenize.NUMBER, tokenize.STRING, tokenize.COMMENT] ) or \
-						( token.type == tokenize.OP and token.string == '(' ):
+						( token.exact_type == tokenize.LPAR ):
 						
 						# initiate indexes with correct linenum
 						s0, s1 = map(str, [ token.start[0] + linenum - 1, token.start[1] ] )
 						e0, e1 = map(str, [ token.end[0] + linenum - 1, token.end[1] ] )
 						idx_start = s0 + '.' + s1
 						idx_end = e0 + '.' + e1
 						
@@ -1351,27 +1278,33 @@
 							
 								if token.string == 'self':
 									self.contents.tag_add('selfs', idx_start, idx_end)
 								
 								elif token.string in self.bools:
 									self.contents.tag_add('bools', idx_start, idx_end)
 									
+##								elif token.string in self.tests:
+##									self.contents.tag_add('tests', idx_start, idx_end)
+								
 								elif token.string in self.breaks:
 									self.contents.tag_add('breaks', idx_start, idx_end)
-									
+								
 								else:
 									self.contents.tag_add('keywords', idx_start, idx_end)
 								
 						
 						# calls
-						elif token.type == tokenize.OP:
+						elif token.exact_type == tokenize.LPAR:
 							# Need to know if last char before ( was not empty.
-							# This check likely takes some time. Faster way would require
-							# info about position of ( in the string tmp.
-							if self.contents.get( '%s - 1c' % idx_start, idx_start ).strip():
+							# Previously used test was:
+							#if self.contents.get( '%s - 1c' % idx_start, idx_start ).strip():
+							
+							# token.line contains line as string which contains token.
+							prev_char_idx = token.start[1]-1
+							if prev_char_idx > -1 and token.line[prev_char_idx].isalnum():
 								self.contents.tag_add('calls', last_idx_start, last_idx_end)
 								
 						elif token.type == tokenize.STRING:
 							self.contents.tag_add('strings', idx_start, idx_end)
 							
 						elif token.type == tokenize.COMMENT:
 							self.contents.tag_add('comments', idx_start, idx_end)
@@ -1682,15 +1615,15 @@
 					tmp = f.read()
 					self.tabs[self.tabindex].oldcontents = tmp
 					
 					if '.py' in filepath.suffix:
 						indentation_is_alien, indent_depth = self.check_indent_depth(tmp)
 						
 						if indentation_is_alien:
-							# Assuming user wants TABWIDTH, change it without notice:
+							# Assuming user wants self.ind_depth, change it without notice:
 							tmp = self.tabs[self.tabindex].oldcontents.splitlines(True)
 							tmp[:] = [self.tabify(line, width=indent_depth) for line in tmp]
 							tmp = ''.join(tmp)
 							self.tabs[self.tabindex].contents = tmp
 							
 						else:
 							self.tabs[self.tabindex].contents = self.tabs[self.tabindex].oldcontents
@@ -2215,28 +2148,30 @@
 		
 		try:
 			mod = importlib.import_module(target)
 			is_module = True
 			filepath = inspect.getsourcefile(mod)
 			
 			if not filepath:
+				# for example: readline
 				self.bell()
+				print('Could not inspect:', target, '\nimport and use help()')
 				return 'break'
 			
 			try:
 				with open(filepath, 'r', encoding='utf-8') as f:
 					fcontents = f.read()
 					self.new_tab()
 					
 					# just in case:
 					if '.py' in filepath:
 						indentation_is_alien, indent_depth = self.check_indent_depth(fcontents)
 						
 						if indentation_is_alien:
-							# Assuming user wants TABWIDTH, change it without notice:
+							# Assuming user wants self.ind_depth, change it without notice:
 							tmp = fcontents.splitlines(True)
 							tmp[:] = [self.tabify(line, width=indent_depth) for line in tmp]
 							tmp = ''.join(tmp)
 							self.tabs[self.tabindex].contents = tmp
 							
 						else:
 							self.tabs[self.tabindex].contents = fcontents
@@ -2291,15 +2226,15 @@
 				
 				self.new_tab()
 				
 				# just in case:
 				indentation_is_alien, indent_depth = self.check_indent_depth(t)
 				
 				if indentation_is_alien:
-					# Assuming user wants TABWIDTH, change it without notice:
+					# Assuming user wants self.ind_depth, change it without notice:
 					tmp = t.splitlines(True)
 					tmp[:] = [self.tabify(line, width=indent_depth) for line in tmp]
 					tmp = ''.join(tmp)
 					self.tabs[self.tabindex].contents = tmp
 					
 				else:
 					self.tabs[self.tabindex].contents = t
@@ -2342,33 +2277,42 @@
 	
 		try:
 			startline = self.contents.index(tkinter.SEL_FIRST).split(sep='.')[0]
 			endline = self.contents.index(tkinter.SEL_LAST).split(sep='.')[0]
 			
 			start = '%s.0' % startline
 			end = '%s.0 lineend' % endline
+			tmp = self.contents.get(start, end)
 			
-			# Check indent (tabify) and rstrip:
-			tmp = self.contents.get(start, end).splitlines()
-			tmp[:] = [self.tabify(line) for line in tmp]
+			indentation_is_alien, indent_depth = self.check_indent_depth(tmp)
+			
+			tmp = tmp.splitlines()
+			
+			if indentation_is_alien:
+				# Assuming user wants self.ind_depth, change it without notice:
+				tmp[:] = [self.tabify(line, width=indent_depth) for line in tmp]
+							
+			else:
+				tmp[:] = [self.tabify(line) for line in tmp]
+			
+						
 			tmp = ''.join(tmp)
-	
-
+			
 			self.contents.delete(start, end)
 			self.contents.insert(start, tmp)
 			
 			
 			self.update_tokens(start=start, end=end)
 						
 															
 			self.contents.edit_separator()
 			return "break"
 		
 		except tkinter.TclError as e:
-			print(e)
+			#print(e)
 			return "break"
 	
 	
 	def tabify(self, line, width=None):
 		
 		if width:
 			ind_width = width
@@ -2476,15 +2420,15 @@
 				tmp = f.read()
 				self.tabs[self.tabindex].oldcontents = tmp
 				
 				if '.py' in filename.suffix:
 					indentation_is_alien, indent_depth = self.check_indent_depth(tmp)
 					
 					if indentation_is_alien:
-						# Assuming user wants TABWIDTH, change it without notice:
+						# Assuming user wants self.ind_depth, change it without notice:
 						tmp = self.tabs[self.tabindex].oldcontents.splitlines(True)
 						tmp[:] = [self.tabify(line, width=indent_depth) for line in tmp]
 						tmp = ''.join(tmp)
 						self.tabs[self.tabindex].contents = tmp
 						
 					else:
 						self.tabs[self.tabindex].contents = self.tabs[self.tabindex].oldcontents
@@ -2903,15 +2847,98 @@
 		self.btn_save.config(state='disabled')
 		
 		self.bind("<Button-3>", self.do_nothing)
 		self.bind("<Escape>", self.stop_help)
 			
 ########## Gotoline and Help End
 ########## Indent and Comment Begin
-
+	
+	def check_indent_depth(self, contents):
+		'''Contents is contents of py-file as string.'''
+		
+		words = [
+				'def ',
+				'if ',
+				'for ',
+				'while ',
+				'class '
+				]
+				
+		tmp = contents.splitlines()
+		
+		for word in words:
+			
+			for i in range(len(tmp)):
+				line = tmp[i]
+				if word in line:
+					
+					# Trying to check if at the beginning of new block:
+					if line.strip()[-1] == ':':
+						# Offset is num of empty lines between this line and next
+						# non empty line
+						nextline = None
+						
+						for offset in range(1, len(tmp)-i):
+							nextline = tmp[i+offset]
+							if nextline.strip() == '': continue
+							else: break
+							
+							
+						if not nextline:
+							continue
+						
+						
+						# Now should have next non empty line,
+						# so start parsing it:
+						flag_space = False
+						indent_0 = 0
+						indent_1 = 0
+		
+						for char in line:
+							if char in [' ', '\t']: indent_0 += 1
+							else: break
+		
+						for char in nextline:
+							# Check if indent done with spaces:
+							if char == ' ':
+								flag_space = True
+		
+							if char in [' ', '\t']: indent_1 += 1
+							else: break
+						
+						
+						indent = indent_1 - indent_0
+						#print(indent)
+						tests = [
+								( indent <= 0 ),
+								( not flag_space and indent > 1 )
+								]
+						
+						if any(tests):
+							#print('indent err')
+							#skipping
+							continue
+						
+						
+						# All is good, do nothing:
+						if not flag_space:
+							return False, 0
+							
+						# Found one block with spaced indentation,
+						# assuming it is used in whole file.
+						else:
+							if indent != self.ind_depth:
+								return True, indent
+							
+							else:
+								return False, 0
+					
+		return False, 0
+	
+	
 	def indent(self, event=None):
 		if self.state != 'normal':
 			self.bell()
 			
 		try:
 			startline = int(self.contents.index(tkinter.SEL_FIRST).split(sep='.')[0])
 			endline = int(self.contents.index(tkinter.SEL_LAST).split(sep='.')[0])
@@ -3249,26 +3276,15 @@
 		self.btn_open.config(state='normal')
 		self.btn_save.config(state='normal')
 		self.bind("<Button-3>", lambda event: self.raise_popup(event))
 		self.contents.tag_remove('focus', '1.0', tkinter.END)
 			
 		# Leave tags on, if replace_all, Esc clears.
 		if self.state == 'replace_all':
-			self.contents.tag_remove('match', '1.0', tkinter.END)
-			wordlen = len(self.new_word)
-			pos = '1.0'
-
-			while True:
-				pos = self.contents.search(self.new_word, pos, stopindex=tkinter.END)
-				if not pos: break
-
-				lastpos = "%s + %dc" % (pos, wordlen)
-				self.contents.tag_add('match', pos, lastpos)
-				pos = "%s + %dc" % (pos, wordlen+1)
-
+		
 			self.bind("<Escape>", self.clear_search_tags)
 			
 		else:
 			self.contents.tag_remove('match', '1.0', tkinter.END)
 			self.bind("<Escape>", self.do_nothing)
 			
 		
@@ -3428,25 +3444,27 @@
 			self.stop_search()
 
 	
 	def do_replace_all(self, event=None):
 		
 		self.contents.config(state='normal')
 		wordlen = len(self.old_word)
+		wordlen2 = len(self.new_word)
 		pos = '1.0'
 		
 		while True:
 			pos = self.contents.search(self.old_word, pos, tkinter.END)
 			if not pos: break
 			
 			lastpos = "%s + %dc" % ( pos, wordlen )
+			lastpos2 = "%s + %dc" % ( pos, wordlen2 )
 			
-			#self.contents.tag_add( 'match', pos, lastpos )
 			self.contents.delete( pos, lastpos )
 			self.contents.insert( pos, self.new_word )
+			self.contents.tag_add( 'match', pos, lastpos2 )
 				
 			pos = "%s + %dc" % (pos, wordlen+1)
 			
 		# show lastpos but dont put cursor on it
 		line = lastpos
 		self.ensure_idx_visibility(line)
```

### Comparing `henxel-0.1.6/src/henxel/changefont.py` & `henxel-0.1.7/src/henxel/changefont.py`

 * *Files identical despite different names*

### Comparing `henxel-0.1.6/src/henxel/fdialog.py` & `henxel-0.1.7/src/henxel/fdialog.py`

 * *Files identical despite different names*

### Comparing `henxel-0.1.6/src/henxel/help.txt` & `henxel-0.1.7/src/henxel/help.txt`

 * *Files 7% similar despite different names*

```diff
@@ -138,17 +138,40 @@
 		then indentation of this first line is wrong when pasted, compared
 		to other lines. But editor moves cursor at the start of block so
 		you can start fixing indenting that function definition line or
 		similar.
 		
 	
 	How to: change indent-depth
+		For all files:
 	  - If you started editor with: import henxel and e=henxel.Editor(),
 		then to change indent-depth in python-console:
 		e.change_indentation_width(8)
+		
+		For code-snippet:
+	  - If you copied something to your editor that has different indentation
+		than rest of the file:
+		(Note that you don't have to do anything if it is indented with normal
+		4 spaces and you have indent-depth the normal 4 )
+		1: Make sure you copied the block starting with one empty line.
+		2: Click cursor to start of empty line and paste.
+		
+  def myfunc(foo):
+	print(foo)
+	
+	return foo + 1
+
+		Then select that code and press mouse-right and select tabify, and
+		it should then be indented as you wanted and you can then continue
+		indenting the pasted code to the right place. You can try all this
+		by copying the code example above and then trying to fix it.
+		
+		(Note that you don't have to do anything if you open a file that has
+		different indentation than your setting, it is changed automatically
+		and saved with tabbed indentation after you for example close it.)
 	
 	
 	Running file
 	  - input from stdin does not work, so use test-data for that.
 	  
 	  - Editor freezes when running a program. So if you are testing
 		for possible runtime-errors, keep that in mind. You should
```

### Comparing `henxel-0.1.6/src/henxel.egg-info/PKG-INFO` & `henxel-0.1.7/src/henxel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henxel
-Version: 0.1.6
+Version: 0.1.7
 Summary: GUI-editor for Python development.
 Home-page: https://github.com/SamuelKos/henxel
 Author: SamuelKos
 Author-email: koskinens371@gmail.com
 Project-URL: Bug Tracker, https://github.com/SamuelKos/henxel/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

