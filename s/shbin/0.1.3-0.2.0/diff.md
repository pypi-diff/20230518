# Comparing `tmp/shbin-0.1.3.tar.gz` & `tmp/shbin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shbin-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "shbin-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `shbin-0.1.3.tar` & `shbin-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4901 2023-05-16 20:03:37.038733 shbin-0.1.3/README.md
--rw-r--r--   0        0        0     1081 2023-05-16 20:03:37.038733 shbin-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     7827 2023-05-16 20:03:37.038733 shbin-0.1.3/shbin.py
--rw-r--r--   0        0        0     5742 1970-01-01 00:00:00.000000 shbin-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     5318 2023-05-18 19:25:15.761602 shbin-0.2.0/README.md
+-rw-r--r--   0        0        0     1081 2023-05-18 19:25:15.761602 shbin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8075 2023-05-18 19:25:15.761602 shbin-0.2.0/shbin.py
+-rw-r--r--   0        0        0     6159 1970-01-01 00:00:00.000000 shbin-0.2.0/PKG-INFO
```

### Comparing `shbin-0.1.3/README.md` & `shbin-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,69 @@
 ![](https://github.com/Shiphero/shbin/actions/workflows/pytest.yml/badge.svg)
 ![](https://github.com/Shiphero/shbin/actions/workflows/black.yml/badge.svg)
 
 `shbin` turns a Github repo into a pastebin. 
 
-It's a tiny command-line tool we've built at [Shiphero](http://shiphero.com) that lets you easily upload code snippets, notebooks, images, or any other file to a Github repository that acts as your internal pastebin, and returns the URL to share it with your team. If possible, this URL is automatically copied to the clipboard. 
+It's a tiny command-line tool we've built at
+[Shiphero](http://shiphero.com) that lets you easily upload code
+snippets, notebooks, images, or any other file to a Github repository
+that acts as your internal pastebin, and returns the URL to share it
+with your team. If possible, this URL is automatically copied to the
+clipboard. 
 
 # Why? 
 
-You want to share code snippets, images, notebooks, etc. with your team, probably privately. Gist is great, but it has some limitations:
+You want to share code snippets, images, notebooks, etc. with your team,
+probably privately. Gist is great, but it has some limitations:
 
-- The content may be secret but it is not private: if you have the url you have the access (and to err is human). 
-- The ownership of the shared content is in the user's namespace, not the organization's.  What happens if the user leaves the organization? 
-- You can't find a secret content shared by a teammate if the URL is lost. Only the person who created it can find it, and even that isn't easy if the content doesn't have a good name and description. 
-- Content organization is difficult: you can upload multiple files to a gist, but you can't create folders.
-- The default gist interface does not allow you to "paste" an image (you can paste it as part of a comment, but not as part of the gist content itself). Sharing screenshots is a common use case on computers. 
-
-Using a full repository has all the advantages of Gist (rich content rendering like markdown or ipynb, every change is a git commit, etc.) without these limitations. 
-
-The only downside of a plain repository is that it is not as easy as "paste" the content, 
-even if the edition is done from the Github's interface. But `shbin` solves that. 
+- The content may be secret but it is not private: if you have the url
+  you have the access (and to err is human). 
+- The ownership of the shared content is in the user's namespace, not
+  the organization's.  What happens if the user leaves the organization? 
+- You can't find some secret content shared by a teammate if the URL is
+  lost. Only the person who created it can find it, and even that isn't
+  easy if the content doesn't have a good name and description. 
+- Content organization is difficult: you can upload multiple files to
+  a gist, but you can't create folders.
+- The default gist interface does not allow you to "paste" an image (you
+  can paste it as part of a comment, but not as part of the gist content
+  itself). Sharing screenshots is a common use case on computers. 
+
+Using a full repository has all the advantages of Gist (rich content
+rendering like markdown or ipynb, every change is a git commit, etc.)
+without these limitations. 
+
+The only downside of a plain repository is that it is not as easy as
+"paste" the content, even when  editing through the Github interface.
+But `shbin` solves that. 
 
 # Usage
 
 ```console
-# upload or upgrade a file
+# upload or update a file
 $ shbin demo.py
 
 # upload with a commit description
 $ shbin demo.py -m "my cool demo script"         
 
-# upload any content in clipboard, discovering its format. e.g. an screenshot. 
-# the name will be random but the extension will be based on the format detected.
+# Upload any content in clipboard, discovering its format. e.g.
+# a screenshot. The name will be random but the extension will be
+# based on the format detected.
 $ shbin -x          
 
-# upload the content in the clipboard but giving it a name
+# upload the content in the clipboard with a given filename
 $ shbin -x -f my_snippet.md 
 
+# upload from stdin
+$ echo "some content" | shbin -
+
 # download a given file (inside the namespace)
 $ shbin dl my_snippet.md     
 
-# upgrade the content of a file that already exists
+# update the content of a file that already exists
 $ shbin my_snippet.md
 
 # from clipboard with a given name to a directory in your user directory
 $ shbin -x -f the_coolest_thing.py -d coolest_things/python
 
 # upload several files in a directory
 $ shbin *.ipynb *.csv -d notebooks/project -m "my new work"   
@@ -52,15 +72,17 @@
 $ shbin demo.py -p
 
 $ shbin -h   # show full options
 ```
 
 # How it works
 
-It uses [Github API](https://docs.github.com/en/rest/repos/contents?apiVersion=2022-11-28#create-or-update-file-contents) to create or update files in the given repo. So there is not need to have the target repository fully cloned.  
+It uses [Github API](https://docs.github.com/en/rest/repos/contents?apiVersion=2022-11-28#create-or-update-file-contents)
+to create or update files in the given repo. So there is no need to
+have the target repository fully cloned locally.  
 
 
 # Install
 
 The recommended way is to use [pipx](https://pypa.github.io/pipx/)
 
 ```console
@@ -76,15 +98,17 @@
 To install the latest development version from the repository:
 
 ```console
 pip install --user https://github.com/Shiphero/shbin/archive/refs/heads/main.zip
 ```
 
 ## OSX
-It can be issues with [python-magic](https://github.com/ahupp/python-magic#osx) install
+shbin depends on 
+[python-magic](https://github.com/ahupp/python-magic#osx). This can be
+installed as follows.
 
 - When using Homebrew: 
 
 ```console
 brew install libmagic
 ```
 
@@ -92,28 +116,43 @@
 
 ```console
 port install file
 ```
 
 # Setup
 
-Create a [new fine-grained personal token](https://github.com/settings/personal-access-tokens/new) on Github for your "pastebin" repository (under your user or your organization ownership), with read and write permissions on "contents: 
+Create a [new fine-grained personal token](https://github.com/settings/personal-access-tokens/new)
+on Github restricted to your "pastebin" repository (under your user or
+your organization's ownership), with read and write permissions on
+"Contents". 
 
 ![image](https://user-images.githubusercontent.com/2355719/238758491-9d15e7e6-e4b7-43c8-a321-b65c968fc7e0.png)
 
 - Then set the environment variables in your preferred place:
     
   ```
   export SHBIN_GITHUB_TOKEN="<your personal token>"
   export SHBIN_REPO="<user_or_org>/<repo>"   # example "Shiphero/pastebin"   
    ```
 
-- By default `shbin` assigns a top-level folder to separate the content uploaded by each user. This can be changed using the `SHBIN_NAMESPACE` environment variable or the `--namespace` argument from the command line. For example: 
+- By default `shbin` assigns a top-level folder to separate the content
+  uploaded by each user. This can be changed using the `SHBIN_NAMESPACE`
+  environment variable or the `--namespace` argument from the command
+  line. For example: 
 
-  -  `export SHBIN_NAMESPACE=""`        # no namespace
-  -  `export SHBIN_NAMESPACE="pastebin_folder"`  # the full pastebin is inside pastebin_folder/" 
+  - `export SHBIN_NAMESPACE=""`        # no namespace
+  - `export SHBIN_NAMESPACE="pastebin_folder"`  # the full pastebin is inside pastebin_folder/" 
   - `export SHBIN_NAMESPACE="pastebin_folder/{user}"`   # mix of both: each user has its own subfolder inside `pastebin_folder/` 
 
-- [optional] To interact with the clipboard, we use the library `pyclip`. This may require some additional system dependencies depending your operating system. See [these notes](https://github.com/spyoungtech/pyclip#platform-specific-notesissues).
+- [optional] To interact with the clipboard, we use the library `pyclip`.
+  This may require some additional system dependencies
+  depending your operating system. See [these notes](https://github.com/spyoungtech/pyclip#platform-specific-notesissues).
+
+  If you want to disable the automatic copying of the URL to the clipboard 
+  you can set the environment variable `SHBIN_COPY_URL=false` (or "0" or "no"). 
+  
+  This is useful in some Linux distributions that use Wayland as the call via `wl-copy`
+  that `pyclip` uses in such environment can be slow. 
+
 
 
-PRs are welcome! 
+PRs are welcome!
```

### Comparing `shbin-0.1.3/pyproject.toml` & `shbin-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shbin-0.1.3/shbin.py` & `shbin-0.2.0/shbin.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from docopt import DocoptExit, docopt
 from github import Github, GithubException
 from rich import print
 
 usage = """
 
 Usage:
-  shbin (<path>... | -x ) [-f <file-name>] [-n] [-m <message>] [-d <target-dir>] 
+  shbin (<path>... | -x | -) [-f <file-name>] [-n] [-m <message>] [-d <target-dir>] 
         [--namespace=<namespace>] [--url-link-to-pages]
   shbin dl <url_or_path>
   shbin (-h | --help)
   
 
 Options:
   -h --help                                         Show this screen.
@@ -31,15 +31,15 @@
   -m <message>, --message=<message>                 Commit message
   -d <target-dir>, --target-dir=<target-dir>        Optional (sub)directory to upload file/s. 
   --namespace=<namespace>                           Base namespace to upload. Default to
                                                     SHBIN_NAMESPACE envvar or "{user}/". 
   -p, --url-link-to-pages                           Reformat the url to link to Github pages. 
 """
 
-__version__ = "0.1.3"
+__version__ = "0.2.0"
 
 
 class FakePath:
     """
     A wrapper on a PurePath object (ie it doesn’t actually access a filesystem)
     with an explicity content in bytes.
     """
@@ -135,19 +135,22 @@
     if namespace is None:
         namespace = os.environ.get("SHBIN_NAMESPACE", "{user}")
     namespace = namespace.format(user=user).rstrip("/")
 
     if args["dl"]:
         return download(args["<url_or_path>"], repo, user)
 
-    elif args["--from-clipboard"]:
-        try:
-            content = pyclip.paste()
-        except pyclip.ClipboardSetupException as e:
-            raise DocoptExit(str(e))
+    elif args["--from-clipboard"] or args["<path>"] == ["-"]:
+        if args["--from-clipboard"]:
+            try:
+                content = pyclip.paste()
+            except pyclip.ClipboardSetupException as e:
+                raise DocoptExit(str(e))
+        else:
+            content = sys.stdin.buffer.read()
 
         if args["--file-name"] and not args["--target-dir"]:
             file_name = f'{args["--file-name"]}'
         elif args["--target-dir"]:
             directory = pathlib.PurePath(args["--target-dir"])
             extension = get_extension(content)
             # TODO try autodectect extension via pygment if .txt was guessed.
@@ -179,16 +182,17 @@
         url = result["content"].html_url.rpartition("/")[0] if len(files) > 1 else result["content"].html_url
         if args["--url-link-to-pages"]:
             content = url.partition(f"{repo.default_branch}/")[-1]
             url = f"https://{repo.owner.login.lower()}.github.io/{repo.name}/{content}"
 
         emoji = "🔗"
         try:
-            pyclip.copy(str(url))
-            emoji += "📋"
+            if os.environ.get("SHBIN_COPY_URL", "").strip().lower() not in ("0", "false", "no"):
+                pyclip.copy(str(url))
+                emoji += "📋"
         except pyclip.ClipboardSetupException:
             pass
         print(f"{emoji} {url}")
 
 
 def create_or_update(repo, path, namespace, message, force_new):
     file_content = path.read_bytes()
```

### Comparing `shbin-0.1.3/PKG-INFO` & `shbin-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shbin
-Version: 0.1.3
+Version: 0.2.0
 Summary: Turns a Github repo into a pastebin.
 Author-email: Alvar Maciel <alvar.maciel@shiphero.com>, Martín Gaitán <marting@shiphero.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -22,51 +22,71 @@
 Provides-Extra: dev
 
 ![](https://github.com/Shiphero/shbin/actions/workflows/pytest.yml/badge.svg)
 ![](https://github.com/Shiphero/shbin/actions/workflows/black.yml/badge.svg)
 
 `shbin` turns a Github repo into a pastebin. 
 
-It's a tiny command-line tool we've built at [Shiphero](http://shiphero.com) that lets you easily upload code snippets, notebooks, images, or any other file to a Github repository that acts as your internal pastebin, and returns the URL to share it with your team. If possible, this URL is automatically copied to the clipboard. 
+It's a tiny command-line tool we've built at
+[Shiphero](http://shiphero.com) that lets you easily upload code
+snippets, notebooks, images, or any other file to a Github repository
+that acts as your internal pastebin, and returns the URL to share it
+with your team. If possible, this URL is automatically copied to the
+clipboard. 
 
 # Why? 
 
-You want to share code snippets, images, notebooks, etc. with your team, probably privately. Gist is great, but it has some limitations:
+You want to share code snippets, images, notebooks, etc. with your team,
+probably privately. Gist is great, but it has some limitations:
 
-- The content may be secret but it is not private: if you have the url you have the access (and to err is human). 
-- The ownership of the shared content is in the user's namespace, not the organization's.  What happens if the user leaves the organization? 
-- You can't find a secret content shared by a teammate if the URL is lost. Only the person who created it can find it, and even that isn't easy if the content doesn't have a good name and description. 
-- Content organization is difficult: you can upload multiple files to a gist, but you can't create folders.
-- The default gist interface does not allow you to "paste" an image (you can paste it as part of a comment, but not as part of the gist content itself). Sharing screenshots is a common use case on computers. 
-
-Using a full repository has all the advantages of Gist (rich content rendering like markdown or ipynb, every change is a git commit, etc.) without these limitations. 
-
-The only downside of a plain repository is that it is not as easy as "paste" the content, 
-even if the edition is done from the Github's interface. But `shbin` solves that. 
+- The content may be secret but it is not private: if you have the url
+  you have the access (and to err is human). 
+- The ownership of the shared content is in the user's namespace, not
+  the organization's.  What happens if the user leaves the organization? 
+- You can't find some secret content shared by a teammate if the URL is
+  lost. Only the person who created it can find it, and even that isn't
+  easy if the content doesn't have a good name and description. 
+- Content organization is difficult: you can upload multiple files to
+  a gist, but you can't create folders.
+- The default gist interface does not allow you to "paste" an image (you
+  can paste it as part of a comment, but not as part of the gist content
+  itself). Sharing screenshots is a common use case on computers. 
+
+Using a full repository has all the advantages of Gist (rich content
+rendering like markdown or ipynb, every change is a git commit, etc.)
+without these limitations. 
+
+The only downside of a plain repository is that it is not as easy as
+"paste" the content, even when  editing through the Github interface.
+But `shbin` solves that. 
 
 # Usage
 
 ```console
-# upload or upgrade a file
+# upload or update a file
 $ shbin demo.py
 
 # upload with a commit description
 $ shbin demo.py -m "my cool demo script"         
 
-# upload any content in clipboard, discovering its format. e.g. an screenshot. 
-# the name will be random but the extension will be based on the format detected.
+# Upload any content in clipboard, discovering its format. e.g.
+# a screenshot. The name will be random but the extension will be
+# based on the format detected.
 $ shbin -x          
 
-# upload the content in the clipboard but giving it a name
+# upload the content in the clipboard with a given filename
 $ shbin -x -f my_snippet.md 
 
+# upload from stdin
+$ echo "some content" | shbin -
+
 # download a given file (inside the namespace)
 $ shbin dl my_snippet.md     
 
-# upgrade the content of a file that already exists
+# update the content of a file that already exists
 $ shbin my_snippet.md
 
 # from clipboard with a given name to a directory in your user directory
 $ shbin -x -f the_coolest_thing.py -d coolest_things/python
 
 # upload several files in a directory
 $ shbin *.ipynb *.csv -d notebooks/project -m "my new work"   
@@ -75,15 +95,17 @@
 $ shbin demo.py -p
 
 $ shbin -h   # show full options
 ```
 
 # How it works
 
-It uses [Github API](https://docs.github.com/en/rest/repos/contents?apiVersion=2022-11-28#create-or-update-file-contents) to create or update files in the given repo. So there is not need to have the target repository fully cloned.  
+It uses [Github API](https://docs.github.com/en/rest/repos/contents?apiVersion=2022-11-28#create-or-update-file-contents)
+to create or update files in the given repo. So there is no need to
+have the target repository fully cloned locally.  
 
 
 # Install
 
 The recommended way is to use [pipx](https://pypa.github.io/pipx/)
 
 ```console
@@ -99,15 +121,17 @@
 To install the latest development version from the repository:
 
 ```console
 pip install --user https://github.com/Shiphero/shbin/archive/refs/heads/main.zip
 ```
 
 ## OSX
-It can be issues with [python-magic](https://github.com/ahupp/python-magic#osx) install
+shbin depends on 
+[python-magic](https://github.com/ahupp/python-magic#osx). This can be
+installed as follows.
 
 - When using Homebrew: 
 
 ```console
 brew install libmagic
 ```
 
@@ -115,28 +139,44 @@
 
 ```console
 port install file
 ```
 
 # Setup
 
-Create a [new fine-grained personal token](https://github.com/settings/personal-access-tokens/new) on Github for your "pastebin" repository (under your user or your organization ownership), with read and write permissions on "contents: 
+Create a [new fine-grained personal token](https://github.com/settings/personal-access-tokens/new)
+on Github restricted to your "pastebin" repository (under your user or
+your organization's ownership), with read and write permissions on
+"Contents". 
 
 ![image](https://user-images.githubusercontent.com/2355719/238758491-9d15e7e6-e4b7-43c8-a321-b65c968fc7e0.png)
 
 - Then set the environment variables in your preferred place:
     
   ```
   export SHBIN_GITHUB_TOKEN="<your personal token>"
   export SHBIN_REPO="<user_or_org>/<repo>"   # example "Shiphero/pastebin"   
    ```
 
-- By default `shbin` assigns a top-level folder to separate the content uploaded by each user. This can be changed using the `SHBIN_NAMESPACE` environment variable or the `--namespace` argument from the command line. For example: 
+- By default `shbin` assigns a top-level folder to separate the content
+  uploaded by each user. This can be changed using the `SHBIN_NAMESPACE`
+  environment variable or the `--namespace` argument from the command
+  line. For example: 
 
-  -  `export SHBIN_NAMESPACE=""`        # no namespace
-  -  `export SHBIN_NAMESPACE="pastebin_folder"`  # the full pastebin is inside pastebin_folder/" 
+  - `export SHBIN_NAMESPACE=""`        # no namespace
+  - `export SHBIN_NAMESPACE="pastebin_folder"`  # the full pastebin is inside pastebin_folder/" 
   - `export SHBIN_NAMESPACE="pastebin_folder/{user}"`   # mix of both: each user has its own subfolder inside `pastebin_folder/` 
 
-- [optional] To interact with the clipboard, we use the library `pyclip`. This may require some additional system dependencies depending your operating system. See [these notes](https://github.com/spyoungtech/pyclip#platform-specific-notesissues).
+- [optional] To interact with the clipboard, we use the library `pyclip`.
+  This may require some additional system dependencies
+  depending your operating system. See [these notes](https://github.com/spyoungtech/pyclip#platform-specific-notesissues).
+
+  If you want to disable the automatic copying of the URL to the clipboard 
+  you can set the environment variable `SHBIN_COPY_URL=false` (or "0" or "no"). 
+  
+  This is useful in some Linux distributions that use Wayland as the call via `wl-copy`
+  that `pyclip` uses in such environment can be slow. 
+
 
 
 PRs are welcome! 
+
```

