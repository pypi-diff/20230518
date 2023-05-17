# Comparing `tmp/ai-commit-gen-0.2.tar.gz` & `tmp/ai-commit-gen-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-commit-gen-0.2.tar", last modified: Wed May 17 22:08:23 2023, max compression
+gzip compressed data, was "ai-commit-gen-0.3.tar", last modified: Wed May 17 22:19:55 2023, max compression
```

## Comparing `ai-commit-gen-0.2.tar` & `ai-commit-gen-0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 sameer    (1000) sameer    (1000)        0 2023-05-17 22:08:23.560664 ai-commit-gen-0.2/
--rw-r--r--   0 sameer    (1000) sameer    (1000)     2045 2023-05-17 22:08:23.556664 ai-commit-gen-0.2/PKG-INFO
--rw-r--r--   0 sameer    (1000) sameer    (1000)     1867 2023-05-17 22:00:35.000000 ai-commit-gen-0.2/README.md
--rwxr-xr-x   0 sameer    (1000) sameer    (1000)     4618 2023-05-17 21:53:33.000000 ai-commit-gen-0.2/ai-commit.py
-drwxr-xr-x   0 sameer    (1000) sameer    (1000)        0 2023-05-17 22:08:23.556664 ai-commit-gen-0.2/ai_commit_gen.egg-info/
--rw-r--r--   0 sameer    (1000) sameer    (1000)     2045 2023-05-17 22:08:23.000000 ai-commit-gen-0.2/ai_commit_gen.egg-info/PKG-INFO
--rw-r--r--   0 sameer    (1000) sameer    (1000)      215 2023-05-17 22:08:23.000000 ai-commit-gen-0.2/ai_commit_gen.egg-info/SOURCES.txt
--rw-r--r--   0 sameer    (1000) sameer    (1000)        1 2023-05-17 22:08:23.000000 ai-commit-gen-0.2/ai_commit_gen.egg-info/dependency_links.txt
--rw-r--r--   0 sameer    (1000) sameer    (1000)       24 2023-05-17 22:08:23.000000 ai-commit-gen-0.2/ai_commit_gen.egg-info/requires.txt
--rw-r--r--   0 sameer    (1000) sameer    (1000)        1 2023-05-17 22:08:23.000000 ai-commit-gen-0.2/ai_commit_gen.egg-info/top_level.txt
--rw-r--r--   0 sameer    (1000) sameer    (1000)       38 2023-05-17 22:08:23.560664 ai-commit-gen-0.2/setup.cfg
--rw-r--r--   0 sameer    (1000) sameer    (1000)      541 2023-05-17 22:07:46.000000 ai-commit-gen-0.2/setup.py
+drwxr-xr-x   0 sameer    (1000) sameer    (1000)        0 2023-05-17 22:19:55.160680 ai-commit-gen-0.3/
+-rw-r--r--   0 sameer    (1000) sameer    (1000)     2045 2023-05-17 22:19:55.156679 ai-commit-gen-0.3/PKG-INFO
+-rw-r--r--   0 sameer    (1000) sameer    (1000)     1867 2023-05-17 22:00:35.000000 ai-commit-gen-0.3/README.md
+drwxr-xr-x   0 sameer    (1000) sameer    (1000)        0 2023-05-17 22:19:55.156679 ai-commit-gen-0.3/ai_commit_gen.egg-info/
+-rw-r--r--   0 sameer    (1000) sameer    (1000)     2045 2023-05-17 22:19:55.000000 ai-commit-gen-0.3/ai_commit_gen.egg-info/PKG-INFO
+-rw-r--r--   0 sameer    (1000) sameer    (1000)      259 2023-05-17 22:19:55.000000 ai-commit-gen-0.3/ai_commit_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 sameer    (1000) sameer    (1000)        1 2023-05-17 22:19:55.000000 ai-commit-gen-0.3/ai_commit_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 sameer    (1000) sameer    (1000)       53 2023-05-17 22:19:55.000000 ai-commit-gen-0.3/ai_commit_gen.egg-info/entry_points.txt
+-rw-r--r--   0 sameer    (1000) sameer    (1000)       24 2023-05-17 22:19:55.000000 ai-commit-gen-0.3/ai_commit_gen.egg-info/requires.txt
+-rw-r--r--   0 sameer    (1000) sameer    (1000)        1 2023-05-17 22:19:55.000000 ai-commit-gen-0.3/ai_commit_gen.egg-info/top_level.txt
+-rwxr-xr-x   0 sameer    (1000) sameer    (1000)     4618 2023-05-17 21:53:33.000000 ai-commit-gen-0.3/ai_commit_gen.py
+-rw-r--r--   0 sameer    (1000) sameer    (1000)       38 2023-05-17 22:19:55.160680 ai-commit-gen-0.3/setup.cfg
+-rw-r--r--   0 sameer    (1000) sameer    (1000)      659 2023-05-17 22:19:06.000000 ai-commit-gen-0.3/setup.py
```

### Comparing `ai-commit-gen-0.2/PKG-INFO` & `ai-commit-gen-0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-commit-gen
-Version: 0.2
+Version: 0.3
 Summary: A binary to generate commit messages or commits using generative models.
 Description-Content-Type: text/markdown
 
 # Ai-Commit-Gen
 
 Ai-Commit-Gen is a Python binary that leverages OpenAI's language models to generate meaningful commit messages. There's approximately a thousand such binaries out there, but none that fit into all of my workflows, so here's the 1001st.
```

### Comparing `ai-commit-gen-0.2/README.md` & `ai-commit-gen-0.3/README.md`

 * *Files identical despite different names*

### Comparing `ai-commit-gen-0.2/ai-commit.py` & `ai-commit-gen-0.3/ai_commit_gen.py`

 * *Files identical despite different names*

### Comparing `ai-commit-gen-0.2/ai_commit_gen.egg-info/PKG-INFO` & `ai-commit-gen-0.3/ai_commit_gen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-commit-gen
-Version: 0.2
+Version: 0.3
 Summary: A binary to generate commit messages or commits using generative models.
 Description-Content-Type: text/markdown
 
 # Ai-Commit-Gen
 
 Ai-Commit-Gen is a Python binary that leverages OpenAI's language models to generate meaningful commit messages. There's approximately a thousand such binaries out there, but none that fit into all of my workflows, so here's the 1001st.
```

