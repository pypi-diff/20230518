# Comparing `tmp/ai-commit-gen-0.3.tar.gz` & `tmp/ai-commit-gen-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-commit-gen-0.3.tar", last modified: Wed May 17 22:19:55 2023, max compression
+gzip compressed data, was "ai-commit-gen-0.4.tar", last modified: Wed May 17 22:25:36 2023, max compression
```

## Comparing `ai-commit-gen-0.3.tar` & `ai-commit-gen-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sameer    (1000) sameer    (1000)        0 2023-05-17 22:19:55.160680 ai-commit-gen-0.3/
--rw-r--r--   0 sameer    (1000) sameer    (1000)     2045 2023-05-17 22:19:55.156679 ai-commit-gen-0.3/PKG-INFO
--rw-r--r--   0 sameer    (1000) sameer    (1000)     1867 2023-05-17 22:00:35.000000 ai-commit-gen-0.3/README.md
-drwxr-xr-x   0 sameer    (1000) sameer    (1000)        0 2023-05-17 22:19:55.156679 ai-commit-gen-0.3/ai_commit_gen.egg-info/
--rw-r--r--   0 sameer    (1000) sameer    (1000)     2045 2023-05-17 22:19:55.000000 ai-commit-gen-0.3/ai_commit_gen.egg-info/PKG-INFO
--rw-r--r--   0 sameer    (1000) sameer    (1000)      259 2023-05-17 22:19:55.000000 ai-commit-gen-0.3/ai_commit_gen.egg-info/SOURCES.txt
--rw-r--r--   0 sameer    (1000) sameer    (1000)        1 2023-05-17 22:19:55.000000 ai-commit-gen-0.3/ai_commit_gen.egg-info/dependency_links.txt
--rw-r--r--   0 sameer    (1000) sameer    (1000)       53 2023-05-17 22:19:55.000000 ai-commit-gen-0.3/ai_commit_gen.egg-info/entry_points.txt
--rw-r--r--   0 sameer    (1000) sameer    (1000)       24 2023-05-17 22:19:55.000000 ai-commit-gen-0.3/ai_commit_gen.egg-info/requires.txt
--rw-r--r--   0 sameer    (1000) sameer    (1000)        1 2023-05-17 22:19:55.000000 ai-commit-gen-0.3/ai_commit_gen.egg-info/top_level.txt
--rwxr-xr-x   0 sameer    (1000) sameer    (1000)     4618 2023-05-17 21:53:33.000000 ai-commit-gen-0.3/ai_commit_gen.py
--rw-r--r--   0 sameer    (1000) sameer    (1000)       38 2023-05-17 22:19:55.160680 ai-commit-gen-0.3/setup.cfg
--rw-r--r--   0 sameer    (1000) sameer    (1000)      659 2023-05-17 22:19:06.000000 ai-commit-gen-0.3/setup.py
+drwxr-xr-x   0 sameer    (1000) sameer    (1000)        0 2023-05-17 22:25:36.084687 ai-commit-gen-0.4/
+-rw-r--r--   0 sameer    (1000) sameer    (1000)     2045 2023-05-17 22:25:36.084687 ai-commit-gen-0.4/PKG-INFO
+-rw-r--r--   0 sameer    (1000) sameer    (1000)     1867 2023-05-17 22:00:35.000000 ai-commit-gen-0.4/README.md
+drwxr-xr-x   0 sameer    (1000) sameer    (1000)        0 2023-05-17 22:25:36.080687 ai-commit-gen-0.4/ai_commit_gen.egg-info/
+-rw-r--r--   0 sameer    (1000) sameer    (1000)     2045 2023-05-17 22:25:36.000000 ai-commit-gen-0.4/ai_commit_gen.egg-info/PKG-INFO
+-rw-r--r--   0 sameer    (1000) sameer    (1000)      259 2023-05-17 22:25:36.000000 ai-commit-gen-0.4/ai_commit_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 sameer    (1000) sameer    (1000)        1 2023-05-17 22:25:36.000000 ai-commit-gen-0.4/ai_commit_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 sameer    (1000) sameer    (1000)       53 2023-05-17 22:25:36.000000 ai-commit-gen-0.4/ai_commit_gen.egg-info/entry_points.txt
+-rw-r--r--   0 sameer    (1000) sameer    (1000)       24 2023-05-17 22:25:36.000000 ai-commit-gen-0.4/ai_commit_gen.egg-info/requires.txt
+-rw-r--r--   0 sameer    (1000) sameer    (1000)        1 2023-05-17 22:25:36.000000 ai-commit-gen-0.4/ai_commit_gen.egg-info/top_level.txt
+-rwxr-xr-x   0 sameer    (1000) sameer    (1000)     4657 2023-05-17 22:22:51.000000 ai-commit-gen-0.4/ai_commit_gen.py
+-rw-r--r--   0 sameer    (1000) sameer    (1000)       38 2023-05-17 22:25:36.084687 ai-commit-gen-0.4/setup.cfg
+-rw-r--r--   0 sameer    (1000) sameer    (1000)      659 2023-05-17 22:24:56.000000 ai-commit-gen-0.4/setup.py
```

### Comparing `ai-commit-gen-0.3/PKG-INFO` & `ai-commit-gen-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-commit-gen
-Version: 0.3
+Version: 0.4
 Summary: A binary to generate commit messages or commits using generative models.
 Description-Content-Type: text/markdown
 
 # Ai-Commit-Gen
 
 Ai-Commit-Gen is a Python binary that leverages OpenAI's language models to generate meaningful commit messages. There's approximately a thousand such binaries out there, but none that fit into all of my workflows, so here's the 1001st.
```

### Comparing `ai-commit-gen-0.3/README.md` & `ai-commit-gen-0.4/README.md`

 * *Files identical despite different names*

### Comparing `ai-commit-gen-0.3/ai_commit_gen.egg-info/PKG-INFO` & `ai-commit-gen-0.4/ai_commit_gen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-commit-gen
-Version: 0.3
+Version: 0.4
 Summary: A binary to generate commit messages or commits using generative models.
 Description-Content-Type: text/markdown
 
 # Ai-Commit-Gen
 
 Ai-Commit-Gen is a Python binary that leverages OpenAI's language models to generate meaningful commit messages. There's approximately a thousand such binaries out there, but none that fit into all of my workflows, so here's the 1001st.
```

### Comparing `ai-commit-gen-0.3/ai_commit_gen.py` & `ai-commit-gen-0.4/ai_commit_gen.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,32 +6,34 @@
 import argparse
 import openai
 import keyring
 import logging
 import subprocess
 import getpass
 
+
 def get_root_dir_name():
     """
     Returns the name of the root git directory.
     """
     try:
         root_dir = subprocess.check_output(["git", "rev-parse", "--show-toplevel"])
         return f"Repository root dir: {os.path.basename(root_dir.strip())}\n\n"
     except subprocess.CalledProcessError:
         return ""
 
+
 def get_last_commits(num_commits=3):
     """
     Returns the commit messages of the last num_commits commits made in this git repository.
     """
     try:
         commit_messages = subprocess.check_output(
             ["git", "log", "-n", str(num_commits), "--pretty=format:%B"],
-            stderr=subprocess.DEVNULL
+            stderr=subprocess.DEVNULL,
         )
         return f"Recent commits:\n{commit_messages.decode()}\n\n"
     except subprocess.CalledProcessError:
         return ""
 
 
 def get_character_limit(model):
@@ -42,24 +44,28 @@
         return 25000
     elif model == "gpt-4-32k":
         return 120000
     else:
         print(f"Invalid model: {model}")
         sys.exit(1)
 
+
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-p", "--prompt", help="Specify the prompt for the OpenAI model"
     )
     parser.add_argument(
         "-c", "--commit", action="store_true", help="Make the git commit directly"
     )
     parser.add_argument(
-        "-e", "--include_extra_context", action="store_true", help="Experimental, include extra context in the prompt to the AI model."
+        "-e",
+        "--include_extra_context",
+        action="store_true",
+        help="Experimental, include extra context in the prompt to the AI model.",
     )
     parser.add_argument(
         "-m", "--model", default="gpt-3.5-turbo", help="Specify the model to be used"
     )
     parser.add_argument(
         "-d", "--debug", action="store_true", help="Enable debug logging"
     )
@@ -67,22 +73,22 @@
 
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     # Get the OpenAI API key from the environment variables or keyring.
     api_key = os.getenv("OPENAI_KEY")
     if api_key is None:
-        api_key = keyring.get_password("autocommit", "openai_key")
+        api_key = keyring.get_password("ai_commit_gen", "openai_key")
         if api_key is None:
             store_in_keyring = input(
                 "No OpenAI API key found. Would you like to store one in the keyring? (y/n) "
             )
-            if store_in_keyring.lower() == 'y':
+            if store_in_keyring.lower() == "y":
                 api_key = getpass.getpass("Enter your OpenAI API key: ")
-                keyring.set_password("autocommit", "openai_key", api_key)
+                keyring.set_password("ai_commit_gen", "openai_key", api_key)
             else:
                 print("No OpenAI API key provided. Exiting.")
                 sys.exit(1)
     openai.api_key = api_key
 
     messages = [
         {"role": "system", "content": "You are a helpful assistant."},
@@ -103,15 +109,15 @@
         extra_context = f"{get_root_dir_name()}{get_last_commits()}"
 
     # Create prompt.
     prompt = (
         args.prompt
         if args.prompt
         else (
-        f"""As your response, please provide a concise git commit message for the changes described below.
+            f"""As your response, please provide a concise git commit message for the changes described below.
 
 The first paragraph of your response should be a single short line less than 50 characters. 
 
 Add more paragraphs that describe the changes in more detail only if necessary. Prefer to use bullet lists instead of long paragraphs.
 
 {extra_context}
 Output of "git diff --staged": 
@@ -137,14 +143,14 @@
     logging.debug(f"Query took {end_time - start_time:.2f} seconds")
 
     response_content = response["choices"][0]["message"]["content"]
 
     # If the commit flag was passed, make the commit.
     if args.commit:
         commit_message = [("-m " + p) for p in response_content.split("\n\n")]
-        subprocess.run(['git', 'commit'] + commit_message, check=True)
+        subprocess.run(["git", "commit"] + commit_message, check=True)
     else:
         print(response_content)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ai-commit-gen-0.3/setup.py` & `ai-commit-gen-0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read in the README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="ai-commit-gen",
-    version="0.3",
+    version="0.4",
     packages=find_packages(),
     scripts=["ai_commit_gen.py"],
     install_requires=[
         "openai",
         "keyring",
         "argparse",
     ],
```

