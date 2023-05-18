# Comparing `tmp/southwark-0.8.2.tar.gz` & `tmp/southwark-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "southwark-0.8.2.tar", last modified: Tue May 10 16:00:16 2022, max compression
+gzip compressed data, was "southwark-0.9.0.tar", last modified: Thu May 18 15:27:22 2023, max compression
```

## Comparing `southwark-0.8.2.tar` & `southwark-0.9.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0 runner    (1001) docker     (121)     7015 2022-05-10 16:00:16.529017 southwark-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4853 2022-05-10 16:00:16.529017 southwark-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     5319 2022-05-10 16:00:16.529017 southwark-0.8.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-05-10 16:00:16.521016 southwark-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-05-10 16:00:16.529017 southwark-0.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2431 2022-05-10 15:59:41.070463 southwark-0.8.2/southwark/click.py
--rw-r--r--   0 runner    (1001) docker     (121)     3240 2022-05-10 15:59:41.070463 southwark-0.8.2/southwark/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     6342 2022-05-10 15:59:41.070463 southwark-0.8.2/southwark/log.py
--rw-r--r--   0 runner    (1001) docker     (121)    11028 2022-05-10 15:59:41.070463 southwark-0.8.2/southwark/targit.py
--rw-r--r--   0 runner    (1001) docker     (121)    11700 2022-05-10 15:59:41.070463 southwark-0.8.2/southwark/repo.py
--rw-r--r--   0 runner    (1001) docker     (121)    13229 2022-05-10 15:59:41.070463 southwark-0.8.2/southwark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-10 15:59:41.070463 southwark-0.8.2/southwark/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     5321 2023-05-18 15:27:22.466680 southwark-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-05-18 15:27:22.458680 southwark-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-05-18 15:27:22.466680 southwark-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7068 2023-05-18 15:27:22.470680 southwark-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4907 2023-05-18 15:27:22.466680 southwark-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 15:26:40.198293 southwark-0.9.0/southwark/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     2431 2023-05-18 15:26:40.198293 southwark-0.9.0/southwark/click.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11755 2023-05-18 15:26:40.198293 southwark-0.9.0/southwark/repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3256 2023-05-18 15:26:40.198293 southwark-0.9.0/southwark/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6342 2023-05-18 15:26:40.198293 southwark-0.9.0/southwark/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11002 2023-05-18 15:26:40.198293 southwark-0.9.0/southwark/targit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13281 2023-05-18 15:26:40.198293 southwark-0.9.0/southwark/__init__.py
```

### Comparing `southwark-0.8.2/PKG-INFO` & `southwark-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: southwark
-Version: 0.8.2
+Version: 0.9.0
 Summary: Extensions to the Dulwich Git library.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: dulwich,git,vcs
 Home-page: https://github.com/repo-helper/southwark
 Project-URL: Issue Tracker, https://github.com/repo-helper/southwark/issues
 Project-URL: Source Code, https://github.com/repo-helper/southwark
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Requires-Dist: click>=7.1.2
@@ -98,16 +99,16 @@
 	:target: https://github.com/repo-helper/southwark/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/repo-helper/southwark/workflows/mypy/badge.svg
 	:target: https://github.com/repo-helper/southwark/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/repo-helper/southwark/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/repo-helper/southwark/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/southwark/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/southwark/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/repo-helper/southwark/master?logo=coveralls
 	:target: https://coveralls.io/github/repo-helper/southwark?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/southwark?logo=codefactor
@@ -141,23 +142,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/southwark
 	:target: https://github.com/repo-helper/southwark/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/southwark
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/southwark/v0.8.2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/southwark/v0.9.0
 	:target: https://github.com/repo-helper/southwark/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/southwark
 	:target: https://github.com/repo-helper/southwark/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/Southwark
 	:target: https://pypi.org/project/Southwark/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `southwark-0.8.2/pyproject.toml` & `southwark-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "Southwark"
-version = "0.8.2"
+version = "0.9.0"
 description = "Extensions to the Dulwich Git library."
 readme = "README.rst"
 keywords = [ "dulwich", "git", "vcs",]
 dynamic = []
 dependencies = [
     "click>=7.1.2",
     "consolekit>=0.1.2",
@@ -22,14 +22,15 @@
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -57,15 +58,15 @@
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Version Control :: Git",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 package = "southwark"
 
 [tool.mkrecipe]
 conda-channels = [ "conda-forge", "domdfcoding",]
@@ -150,15 +151,15 @@
     "__new__",
     "__getnewargs__",
     "__abstractmethods__",
     "__hash__",
 ]
 
 [tool.mypy]
-python_version = "3.6"
+python_version = "3.8"
 namespace_packages = true
 check_untyped_defs = true
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
```

### Comparing `southwark-0.8.2/README.rst` & `southwark-0.9.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -57,16 +57,16 @@
 	:target: https://github.com/repo-helper/southwark/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/repo-helper/southwark/workflows/mypy/badge.svg
 	:target: https://github.com/repo-helper/southwark/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/repo-helper/southwark/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/repo-helper/southwark/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/southwark/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/southwark/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/repo-helper/southwark/master?logo=coveralls
 	:target: https://coveralls.io/github/repo-helper/southwark?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/southwark?logo=codefactor
@@ -100,23 +100,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/southwark
 	:target: https://github.com/repo-helper/southwark/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/southwark
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/southwark/v0.8.2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/southwark/v0.9.0
 	:target: https://github.com/repo-helper/southwark/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/southwark
 	:target: https://github.com/repo-helper/southwark/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/Southwark
 	:target: https://pypi.org/project/Southwark/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `southwark-0.8.2/LICENSE` & `southwark-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `southwark-0.8.2/southwark/click.py` & `southwark-0.9.0/southwark/click.py`

 * *Files identical despite different names*

### Comparing `southwark-0.8.2/southwark/config.py` & `southwark-0.9.0/southwark/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,29 +47,29 @@
 
 # 3rd party
 from dulwich.config import ConfigFile
 
 __all__ = ["set_remote_ssh", "set_remote_http", "get_remotes"]
 
 
-def set_remote_ssh(config: ConfigFile, domain: str, username: str, repo: str, name: str = "origin"):
+def set_remote_ssh(config: ConfigFile, domain: str, username: str, repo: str, name: str = "origin") -> None:
 	"""
 	Set the remote url for the repository, using SSH.
 
 	:param config:
 	:param domain:
 	:param username:
 	:param repo:
 	:param name: The name of the remote to set.
 	"""
 
 	config.set(("remote", name), "url", f"git@{domain}:{username}/{repo}.git".encode("UTF-8"))
 
 
-def set_remote_http(config: ConfigFile, domain: str, username: str, repo: str, name: str = "origin"):
+def set_remote_http(config: ConfigFile, domain: str, username: str, repo: str, name: str = "origin") -> None:
 	"""
 	Set the remote url for the repository, using HTTP.
 
 	:param config:
 	:param domain:
 	:param username:
 	:param repo:
```

### Comparing `southwark-0.8.2/southwark/log.py` & `southwark-0.9.0/southwark/log.py`

 * *Files identical despite different names*

### Comparing `southwark-0.8.2/southwark/targit.py` & `southwark-0.9.0/southwark/targit.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,29 +157,29 @@
 	:raises FileNotFoundError: If the file is opened in read or append mode, but it does not exist.
 	:raises FileExistsError: If the file is opened in write mode, but it already exists.
 	:raises ValueError: If an unknown value for ``mode`` is given.
 	"""  # noqa: D400
 
 	__mode: Modes
 	__repo: Repo
-	__lock: Optional[FileLock]  # type: ignore[valid-type]
+	__lock: Optional[FileLock]
 
 	def __init__(self, filename: PathLike, mode: Modes = 'r'):
 		self.filename = PathPlus(filename)
 		self.__closed: bool = True
 
 		self.__tmpdir: TemporaryPathPlus = TemporaryPathPlus()
 		self.__tmpdir_p = self.__tmpdir.name
 		atexit.register(self.__exit_handler)
 
 		if mode in {'w', 'a'}:
 			lock_file = str(self.filename.with_suffix(self.filename.suffix + ".lock"))
 			self.__lock = FileLock(lock_file, timeout=1)
 			try:
-				self.__lock.acquire()  # type: ignore[attr-defined]
+				self.__lock.acquire()
 			except Timeout:
 				raise OSError(f"Unable to acquire a lock for the file '{self.filename!s}'")
 		else:
 			self.__lock = None
 
 		if mode in {'r', 'a'}:
 			if not self.exists():
@@ -274,15 +274,15 @@
 		current_status = status(self.__tmpdir_p)
 
 		for file in (*current_status.unstaged, *current_status.untracked):
 			self.__repo.stage(str(file))
 
 		return status(self.__tmpdir_p).staged
 
-	def __do_commit(self, message: str):
+	def __do_commit(self, message: str) -> None:
 		if self.closed:
 			raise OSError("IO operation on closed TarGit file.")
 		elif self.__mode not in {'w', 'a'}:
 			raise OSError("Cannot write to TarGit file opened in read-only mode.")
 
 		login = getpass.getuser()
 		username = f"{login} <{login}@{socket.gethostname()}>"
@@ -300,23 +300,23 @@
 	def exists(self) -> bool:
 		"""
 		Returns whether the :class:`~.TarGit` archive exists.
 		"""
 
 		return self.filename.is_file()
 
-	def close(self):
+	def close(self) -> None:
 		"""
 		Closes the :class:`~.TarGit` archive.
 		"""
 
 		self.__exit_handler()
 		atexit.unregister(self.__exit_handler)
 
-	def __exit_handler(self):
+	def __exit_handler(self) -> None:
 		if self.__tmpdir is not None:
 			self.__tmpdir.cleanup()
 		if self.__lock is not None:
 			self.__lock.release()
 		self.__closed = True
 
 	@property
@@ -344,15 +344,15 @@
 		representing the given filename relative to the archive root.
 
 		:param filename:
 		"""  # noqa: D400
 
 		return self.__tmpdir_p / filename
 
-	def __del__(self):
+	def __del__(self) -> None:
 		self.close()
 
 	def __repr__(self) -> str:
 		"""
 		Returns a string representation of the :class:`~.TarGit`.
 		"""
```

### Comparing `southwark-0.8.2/southwark/repo.py` & `southwark-0.9.0/southwark/repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,21 +41,21 @@
 #  |  License for the specific language governing permissions and limitations
 #  |  under the License.
 #
 
 # stdlib
 import os
 from itertools import chain
-from typing import Any, Dict, Iterator, Optional, Type, TypeVar, Union, cast
+from typing import Any, Dict, Iterator, Optional, Set, Type, TypeVar, Union, cast
 
 # 3rd party
 import click
 import dulwich.index
 import dulwich.refs
-from domdf_python_tools.compat import PYPY, PYPY36
+from domdf_python_tools.compat import PYPY36
 from domdf_python_tools.paths import PathPlus
 from domdf_python_tools.typing import PathLike
 from dulwich import repo
 from dulwich.config import StackedConfig
 from dulwich.objects import Commit, Tree, TreeEntry
 
 __all__ = ["get_user_identity", "Repo", "_R"]
@@ -227,26 +227,26 @@
 		"""
 		Create a new repository.
 
 		:param path: Path in which to create the repository.
 		:param mkdir: Whether to create the directory if it doesn't exist.
 		"""
 
-		return super().init(path, mkdir)
+		return super().init(path, mkdir=mkdir)
 
 	@classmethod
 	def init_bare(cls: Type[_R], path: PathLike, mkdir: bool = False) -> _R:
 		"""
 		Create a new bare repository.
 
 		:param path: Path in which to create the repository.
 		:param mkdir:
 		"""
 
-		return super().init_bare(path, mkdir)
+		return super().init_bare(path, mkdir=mkdir)
 
 	def list_remotes(self) -> Dict[str, str]:
 		"""
 		Returns a mapping of remote names to remote URLs, for the repo's current remotes.
 
 		.. versionadded:: 0.7.0
 		"""
@@ -256,15 +256,15 @@
 
 		for key in list(config.keys()):
 			if key[0] == b"remote":
 				remotes[key[1].decode("UTF-8")] = config.get(key, "url").decode("UTF-8")
 
 		return remotes
 
-	def reset_to(self, sha: Union[str, bytes]):
+	def reset_to(self, sha: Union[str, bytes]) -> None:
 		"""
 		Reset the state of the repository to the given commit sha.
 
 		Any files added in subsequent commits will be removed,
 		any deleted will be restored,
 		and any modified will be reverted.
 
@@ -349,15 +349,15 @@
 
 					if dulwich.refs.check_ref_format(refname.encode("UTF-8")):
 						allkeys.add(refname.encode("UTF-8"))
 
 			allkeys.update(self.get_packed_refs())
 			return allkeys
 
-		def subkeys(self, base):
+		def subkeys(self, base) -> Set[str]:
 			subkeys = set()
 
 			path = self.refpath(base).decode("UTF-8")
 			base = base.decode("UTF-8")
 
 			for root, unused_dirs, files in os.walk(path):
 				dir = root[len(path):]  # noqa: A001  # pylint: disable=redefined-builtin
@@ -376,15 +376,15 @@
 
 			for key in self.get_packed_refs():
 				if key.startswith(base):
 					subkeys.add(key[len(base):].strip('/'))
 
 			return subkeys
 
-		def as_dict(self, base=None):
+		def as_dict(self, base=None) -> Dict:  # todo: KT, VT
 			ret = {}
 			keys = self.keys(base)
 
 			if base is None:
 				base = b""
 			else:
 				base = base.rstrip(b"/")
```

### Comparing `southwark-0.8.2/southwark/__init__.py` & `southwark-0.9.0/southwark/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 # this package
 from southwark.repo import Repo
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.8.2"
+__version__: str = "0.9.0"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = [
 		"get_tags",
 		"check_git_status",
 		"assert_clean",
 		"get_untracked_paths",
@@ -453,15 +453,15 @@
 def open_repo_closing(path_or_repo: _DR) -> ContextManager[_DR]: ...
 
 
 @overload
 def open_repo_closing(path_or_repo: Union[str, os.PathLike]) -> ContextManager[Repo]: ...
 
 
-def open_repo_closing(path_or_repo):
+def open_repo_closing(path_or_repo) -> ContextManager:  # noqa: MAN001
 	"""
 	Returns a context manager which will return :class:`dulwich.repo.Repo` objects unchanged,
 	but will create a new :class:`dulwich.repo.Repo` when a filesystem path is given.
 
 	.. versionadded:: 0.7.0
 
 	:param path_or_repo: Either a :class:`dulwich.repo.Repo` object or the path of a repository.
@@ -470,15 +470,15 @@
 	if isinstance(path_or_repo, dulwich.repo.BaseRepo):
 		return nullcontext(path_or_repo)
 
 	return closing(Repo(path_or_repo))
 
 
 @contextmanager
-def windows_clone_helper():
+def windows_clone_helper() -> Iterator[None]:
 	"""
 	Contextmanager to aid cloning on Windows during tests.
 
 	.. versionadded:: 0.8.0
 
 	.. attention:: This function is intended only for use in tests.
```

