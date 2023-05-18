# Comparing `tmp/makejinja-1.1.5b4.tar.gz` & `tmp/makejinja-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makejinja-1.1.5b4.tar", max compression
+gzip compressed data, was "makejinja-2.0.0b1.tar", max compression
```

## Comparing `makejinja-1.1.5b4.tar` & `makejinja-2.0.0b1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-05-09 09:39:35.952606 makejinja-1.1.5b4/LICENSE
--rw-r--r--   0        0        0    16958 2023-05-09 09:39:35.952606 makejinja-1.1.5b4/README.md
--rw-r--r--   0        0        0      101 2023-05-09 09:39:35.952606 makejinja-1.1.5b4/makejinja/__init__.py
--rw-r--r--   0        0        0       48 2023-05-09 09:39:35.952606 makejinja-1.1.5b4/makejinja/__main__.py
--rw-r--r--   0        0        0     5805 2023-05-09 09:39:35.952606 makejinja-1.1.5b4/makejinja/app.py
--rw-r--r--   0        0        0     1291 2023-05-09 09:39:35.952606 makejinja-1.1.5b4/makejinja/cli.py
--rw-r--r--   0        0        0    12184 2023-05-09 09:39:35.956606 makejinja-1.1.5b4/makejinja/config.py
--rw-r--r--   0        0        0     1060 2023-05-09 09:39:35.956606 makejinja-1.1.5b4/makejinja/loader.py
--rw-r--r--   0        0        0        0 2023-05-09 09:39:35.956606 makejinja-1.1.5b4/makejinja/py.typed
--rw-r--r--   0        0        0      813 2023-05-09 09:41:19.506295 makejinja-1.1.5b4/pyproject.toml
--rw-r--r--   0        0        0    18182 1970-01-01 00:00:00.000000 makejinja-1.1.5b4/setup.py
--rw-r--r--   0        0        0    17820 1970-01-01 00:00:00.000000 makejinja-1.1.5b4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-18 19:42:03.032560 makejinja-2.0.0b1/LICENSE
+-rw-r--r--   0        0        0    16708 2023-05-18 19:42:03.032560 makejinja-2.0.0b1/README.md
+-rw-r--r--   0        0        0      101 2023-05-18 19:42:03.032560 makejinja-2.0.0b1/makejinja/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-18 19:42:03.032560 makejinja-2.0.0b1/makejinja/__main__.py
+-rw-r--r--   0        0        0     6783 2023-05-18 19:42:03.032560 makejinja-2.0.0b1/makejinja/app.py
+-rw-r--r--   0        0        0     1187 2023-05-18 19:42:03.032560 makejinja-2.0.0b1/makejinja/cli.py
+-rw-r--r--   0        0        0    12243 2023-05-18 19:42:03.032560 makejinja-2.0.0b1/makejinja/config.py
+-rw-r--r--   0        0        0     1060 2023-05-18 19:42:03.032560 makejinja-2.0.0b1/makejinja/loader.py
+-rw-r--r--   0        0        0        0 2023-05-18 19:42:03.032560 makejinja-2.0.0b1/makejinja/py.typed
+-rw-r--r--   0        0        0      813 2023-05-18 19:43:55.469251 makejinja-2.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0    17929 1970-01-01 00:00:00.000000 makejinja-2.0.0b1/setup.py
+-rw-r--r--   0        0        0    17570 1970-01-01 00:00:00.000000 makejinja-2.0.0b1/PKG-INFO
```

### Comparing `makejinja-1.1.5b4/LICENSE` & `makejinja-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `makejinja-1.1.5b4/README.md` & `makejinja-2.0.0b1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -69,44 +69,42 @@
  makejinja can be used to automatically generate files from Jinja templates.
  Instead of passing CLI options, you can also write them to a file called .makejinja.toml in your working directory.
  Note: In this file, options may be named differently. Please refer to the file makejinja/config.py to see their actual
  names. You will also find an example here: makejinja/tests/data/.makejinja.toml.
 
 ╭─ Input/Output ───────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ *  --input                DIRECTORY  Path to a folder containing template files. It is passed to Jinja's             │
-│                                      FileSystemLoader when creating the environment.                                 │
+│                                      FileSystemLoader when creating the environment. Note: This option may be passed │
+│                                      multiple times to pass a list of values. If a template exists in multiple       │
+│                                      inputs, the last value with be used.                                            │
 │                                      [required]                                                                      │
 │ *  --output               DIRECTORY  Path to a folder where the rendered templates are stored. makejinja preserves   │
 │                                      the relative paths in the process, meaning that you can even use it on nested   │
 │                                      directories.                                                                    │
 │                                      [required]                                                                      │
 │    --input-pattern        TEXT       Glob pattern to search for files in input_folder. Accepts all pattern supported │
 │                                      by fnmatch. If a file is matched by this pattern and does not end with the      │
 │                                      specified jinja-suffix, it is copied over to the output_folder. Note: Do not    │
 │                                      add a special suffix used by your template files here, instead use the          │
 │                                      jinja-suffix option.                                                            │
 │                                      [default: **/*]                                                                 │
+│    --exclude-pattern      TEXT       Glob patterns pattern to exclude files matched. Applied against files           │
+│                                      discovered by the input glob. Multiple can be provided.                         │
 │    --jinja-suffix         TEXT       File ending of Jinja template files. All files with this suffix in input_folder │
 │                                      matched by pattern are passed to the Jinja renderer. Note: Should be provided   │
 │                                      with the leading dot.                                                           │
 │                                      [default: .jinja]                                                               │
-│    --copy-tree                       If your input_folder containes additional files besides Jinja templates, you    │
-│                                      may want to copy them to output_folder as well. This operation maintains the    │
-│                                      metadata of all files and folders, meaning that tools like rsync will treat     │
-│                                      them exactly like the original ones. Note: Even if set to no-copy-tree, files   │
-│                                      that are matched by your provided pattern within input_folder are still copied  │
-│                                      over. In both cases, a file's metadata is untouched. The main difference is     │
-│                                      that with copy-tree, folders keep their metadata while matched files are copied │
-│                                      to newly-created subfolders that differ in their metadata.                      │
 │    --keep-jinja-suffix               Decide whether the specified jinja-suffix is removed from the file after        │
 │                                      rendering.                                                                      │
 │    --keep-empty                      Some Jinja template files may be empty after rendering (e.g., if they only      │
 │                                      contain macros that are imported by other templates). By default, we do not     │
 │                                      copy such empty files. If there is a need to have them available anyway, you    │
 │                                      can adjust that.                                                                │
+│    --copy-metadata                   Copy the file metadata (e.g., created/modified/permissions) from the input file │
+│                                      using shutil.copystat                                                           │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Jinja Environment ──────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --data           PATH       Load variables from yaml/yml/toml files for use in your Jinja templates. The defintions  │
 │                             are passed to Jinja's render function. Can either be a file or a folder containg files.  │
 │                             Note: This option may be passed multiple times to pass a list of values. If multiple     │
 │                             files are supplied, beware that previous declarations will be overwritten by newer ones. │
 │ --loader         TEXT       Use custom Python code to adjust the used Jinja environment to your needs. The specified │
```

### Comparing `makejinja-1.1.5b4/makejinja/app.py` & `makejinja-2.0.0b1/makejinja/app.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,37 +25,67 @@
 def makejinja(config: Config):
     """makejinja can be used to automatically generate files from [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/templates/)."""
 
     for path in config.import_paths:
         sys.path.append(str(path.resolve()))
 
     data = load_data(config)
+
+    if config.output.is_dir():
+        print(f"Remove output '{config.output}'")
+        shutil.rmtree(config.output)
+
+    config.output.mkdir()
+
     env = init_jinja_env(config)
 
     for loader in config.loaders:
         process_loader(loader, env, data)
 
-    if config.output.is_dir():
-        print(f"Remove '{config.output}' from previous run")
-        shutil.rmtree(config.output)
+    rendered_files: set[Path] = set()
+    rendered_folders: dict[Path, Path] = {}
+
+    for input_dir in config.inputs:
+        for input_path in sorted(input_dir.glob(config.input_pattern)):
+            relative_path = input_path.relative_to(input_dir)
+            output_path = generate_output_path(config, relative_path)
+
+            if (
+                input_path.is_file()
+                and output_path not in rendered_files
+                and not any(input_path.match(x) for x in config.exclude_patterns)
+            ):
+                render_path(input_path, relative_path, output_path, config, env, data)
+                rendered_files.add(output_path)
+
+            elif input_path.is_dir() and output_path not in rendered_folders:
+                print(f"Create folder '{input_path}' -> '{output_path}'")
+                output_path.mkdir()
+                rendered_folders[output_path] = input_path
+
+    # The metadata has to be copied after all files are rendered
+    # Otherwise the mtime will be updated
+    if config.copy_metadata:
+        for output_path, input_path in rendered_folders.items():
+            print(f"Copy metadata '{input_path}' -> '{output_path}'")
+            shutil.copystat(input_path, output_path)
 
-    if config.copy_tree:
-        print(f"Copy file tree '{config.input}' -> '{config.output}'")
-        shutil.copytree(config.input, config.output)
-
-    config.output.mkdir(parents=True, exist_ok=True)
-
-    for input in config.input.glob(config.input_pattern):
-        if not input.is_dir():
-            render_file(input, config, env, data)
+
+def generate_output_path(config: Config, relative_path: Path) -> Path:
+    output_file = config.output / relative_path
+
+    if relative_path.suffix == config.jinja_suffix and not config.keep_jinja_suffix:
+        output_file = output_file.with_suffix("")
+
+    return output_file
 
 
 def init_jinja_env(config: Config) -> Environment:
     return Environment(
-        loader=FileSystemLoader(config.input),
+        loader=FileSystemLoader(config.inputs),
         extensions=config.extensions,
         block_start_string=config.delimiter.block_start,
         block_end_string=config.delimiter.block_end,
         variable_start_string=config.delimiter.variable_start,
         variable_end_string=config.delimiter.variable_end,
         comment_start_string=config.delimiter.comment_start,
         comment_end_string=config.delimiter.comment_end,
@@ -155,36 +185,34 @@
     if hasattr(loader, "policies"):
         env.policies.update(loader.policies())
 
     if hasattr(loader, "data"):
         data.update(loader.data())
 
 
-def render_file(input: Path, config: Config, env: Environment, data: dict[str, t.Any]):
-    relative_path = input.relative_to(config.input)
-    output = config.output / relative_path
-    output.parent.mkdir(parents=True, exist_ok=True)
-
-    if relative_path.suffix == config.jinja_suffix:
+def render_path(
+    input: Path,
+    relative_path: Path,
+    output: Path,
+    config: Config,
+    env: Environment,
+    data: dict[str, t.Any],
+) -> None:
+    if input.suffix == config.jinja_suffix:
         template = env.get_template(str(relative_path))
-
-        # Remove the copied file if the tree has been duplicated
-        if config.copy_tree:
-            output.unlink()
-
-        if not config.keep_jinja_suffix:
-            output = output.with_suffix("")
-
         rendered = template.render(data)
 
         # Write the rendered template if it has content
         # Prevents empty macro definitions
         if rendered.strip() == "" and not config.keep_empty:
-            print(f"Skip '{input}'")
+            print(f"Skip empty '{input}'")
         else:
-            print(f"Render '{input}' -> '{output}'")
-            with output.open("w") as f:
-                f.write(rendered)
+            print(f"Render file '{input}' -> '{output}'")
+            with output.open("w") as fp:
+                fp.write(rendered)
+
+            if config.copy_metadata:
+                shutil.copystat(input, output)
 
-    elif not config.copy_tree:
-        print(f"Copy '{input}' -> '{output}'")
+    else:
+        print(f"Copy file '{input}' -> '{output}'")
         shutil.copy2(input, output)
```

### Comparing `makejinja-1.1.5b4/makejinja/cli.py` & `makejinja-2.0.0b1/makejinja/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from pathlib import Path
-from typing import Type, cast
 
 import rich_click as click
 import typed_settings as ts
-from typed_settings.types import AttrsInstance
 
 from makejinja.config import OPTION_GROUPS, Config
 
 from .app import makejinja
 
 __all__ = ["makejinja_cli"]
 
@@ -16,15 +14,15 @@
 
 _loader = ts.default_loaders(
     appname="makejinja", config_files=(Path(".makejinja.toml"),)
 )
 
 
 @click.command("makejinja")
-@ts.click_options(cast(Type[AttrsInstance], Config), _loader)
+@ts.click_options(Config, _loader)
 def makejinja_cli(config: Config):
     """makejinja can be used to automatically generate files from [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/templates/).
 
     Instead of passing CLI options, you can also write them to a file called `.makejinja.toml` in your working directory.
     **Note**: In this file, options may be named differently.
     Please refer to the file [`makejinja/config.py`](https://github.com/mirkolenz/makejinja/blob/main/makejinja/config.py) to see their actual names.
     You will also find an example here: [`makejinja/tests/data/.makejinja.toml`](https://github.com/mirkolenz/makejinja/blob/main/tests/data/.makejinja.toml).
```

### Comparing `makejinja-1.1.5b4/makejinja/config.py` & `makejinja-2.0.0b1/makejinja/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,19 +142,25 @@
             The default is `False`, which causes a single newline, if present, to be stripped from the end of the template.
         """,
     )
 
 
 @ts.settings(frozen=True)
 class Config:
-    input: Path = ts.option(
-        click={"type": click.Path(exists=True, file_okay=False, path_type=Path)},
+    inputs: list[Path] = ts.option(
+        click={
+            "type": click.Path(exists=True, file_okay=False, path_type=Path),
+            "param_decls": "--input",
+            "required": True,
+        },
         help="""
             Path to a folder containing template files.
             It is passed to Jinja's [FileSystemLoader](https://jinja.palletsprojects.com/en/3.1.x/api/#jinja2.FileSystemLoader) when creating the environment.
+            **Note:** This option may be passed multiple times to pass a list of values.
+            If a template exists in multiple inputs, the last value with be used.
         """,
     )
     output: Path = ts.option(
         click={"type": click.Path(file_okay=False, writable=True, path_type=Path)},
         help="""
             Path to a folder where the rendered templates are stored.
             makejinja preserves the relative paths in the process, meaning that you can even use it on nested directories.
@@ -165,14 +171,22 @@
         help="""
             Glob pattern to search for files in `input_folder`.
             Accepts all pattern supported by [`fnmatch`](https://docs.python.org/3/library/fnmatch.html#module-fnmatch).
             If a file is matched by this pattern and does not end with the specified `jinja-suffix`, it is copied over to the `output_folder`.
             **Note:** Do not add a special suffix used by your template files here, instead use the `jinja-suffix` option.
         """,
     )
+    exclude_patterns: list[str] = ts.option(
+        factory=list,
+        click={"param_decls": "--exclude-pattern"},
+        help="""
+            Glob patterns pattern to exclude files matched. Applied against files discovered by the input glob.
+            Multiple can be provided.
+        """,
+    )
     jinja_suffix: str = ts.option(
         default=".jinja",
         help="""
             File ending of Jinja template files.
             All files with this suffix in `input_folder` matched by `pattern` are passed to the Jinja renderer.
             **Note:** Should be provided *with* the leading dot.
         """,
@@ -180,34 +194,30 @@
     keep_jinja_suffix: bool = ts.option(
         default=False,
         click={"param_decls": "--keep-jinja-suffix"},
         help="""
             Decide whether the specified `jinja-suffix` is removed from the file after rendering.
         """,
     )
-    copy_tree: bool = ts.option(
-        default=False,
-        click={"param_decls": "--copy-tree"},
-        help="""
-            If your `input_folder` containes additional files besides Jinja templates, you may want to copy them to `output_folder` as well.
-            This operation maintains the metadata of all files and folders, meaning that tools like `rsync` will treat them exactly like the original ones.
-            **Note:** Even if set to `no-copy-tree`, files that are matched by your provided `pattern` within `input_folder` are still copied over.
-            In both cases, a file's metadata is untouched.
-            The main difference is that with `copy-tree`, folders keep their metadata while matched files are copied to newly-created subfolders that differ in their metadata.
-        """,
-    )
     keep_empty: bool = ts.option(
         default=False,
         click={"param_decls": "--keep-empty"},
         help="""
             Some Jinja template files may be empty after rendering (e.g., if they only contain macros that are imported by other templates).
             By default, we do not copy such empty files.
             If there is a need to have them available anyway, you can adjust that.
         """,
     )
+    copy_metadata: bool = ts.option(
+        default=False,
+        click={"param_decls": "--copy-metadata"},
+        help="""
+            Copy the file metadata (e.g., created/modified/permissions) from the input file using `shutil.copystat`
+        """,
+    )
     data: list[Path] = ts.option(
         factory=list,
         click={
             "type": click.Path(exists=True, path_type=Path),
             "param_decls": "--data",
         },
         help="""
@@ -265,18 +275,19 @@
     "makejinja": [
         {
             "name": "Input/Output",
             "options": [
                 "--input",
                 "--output",
                 "--input-pattern",
+                "--exclude-pattern",
                 "--jinja-suffix",
-                "--copy-tree",
                 "--keep-jinja-suffix",
                 "--keep-empty",
+                "--copy-metadata",
             ],
         },
         {
             "name": "Jinja Environment",
             "options": [
                 "--data",
                 "--loader",
```

### Comparing `makejinja-1.1.5b4/makejinja/loader.py` & `makejinja-2.0.0b1/makejinja/loader.py`

 * *Files identical despite different names*

### Comparing `makejinja-1.1.5b4/pyproject.toml` & `makejinja-2.0.0b1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "makejinja"
-version = "1.1.5b4"
+version = "2.0.0b1"
 description = "Automatically generate files based on Jinja templates. Use it to easily generate complex Home Assistant dashboards!"
 authors = ["Mirko Lenz <mirko@mirkolenz.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mirkolenz/makejinja"
 
 [tool.poetry.scripts]
 makejinja = "makejinja.cli:makejinja_cli"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 jinja2 = "^3.1.2"
 pyyaml = "^6.0"
 rich-click = "^1.6.1"
-typed-settings = "^23.0.0"
+typed-settings = "^23.0.1"
 tomli = { version = "^2.0.1", python = "<3.11" }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 
 [tool.pytest.ini_options]
```

### Comparing `makejinja-1.1.5b4/setup.py` & `makejinja-2.0.0b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['jinja2>=3.1.2,<4.0.0',
  'pyyaml>=6.0,<7.0',
  'rich-click>=1.6.1,<2.0.0',
- 'typed-settings>=23.0.0,<24.0.0']
+ 'typed-settings>=23.0.1,<24.0.0']
 
 extras_require = \
 {':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['makejinja = makejinja.cli:makejinja_cli']}
 
 setup_kwargs = {
     'name': 'makejinja',
-    'version': '1.1.5b4',
+    'version': '2.0.0b1',
     'description': 'Automatically generate files based on Jinja templates. Use it to easily generate complex Home Assistant dashboards!',
-    'long_description': '# makejinja\n\nmakejinja can be used to automatically generate files from [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/templates/).\nThis allows you to load variables from external files or create repeating patterns via loops.\nIt is conceptually similar to [gomplate](https://github.com/hairyhenderson/gomplate), but is built on Python and Jinja instead of Go.\nA use case for this tool is generating config files for [Home Assistant](https://www.home-assistant.io/):\nUsing the same language that the built-in templates use, you can greatly simplify your configuration.\n\n## Home Assistant Example\n\n[A concrete example for Home Assistant can be found in the tests directory.](./tests/data)\n\n## Features\n\n- Recursively convert nested directories containing template files. One can even specify a pattern to specify relevant files in a folder.\n- Load data files containing variables to use in your Jinja templates from YAML, TOML, and Python files.\n- Use custom functions in your Jinja templates by loading custom filters and/or globals.\n- Easily load bundled as well as custom Jinja extensions.\n- Tailor the whitespace behavior to your needs.\n- Use custom delimiters for Jinja blocks/comments/variables.\n- Modify _all_ init options for the Jinja environment.\n- Write custom **Python loaders** that implement a subset of our fully typed [abstract loader class](./makejinja/loader.py)\n\n## Installation\n\nWe support multiple installation methods: pip, nix, and docker.\n\n### PIP\n\nmakejinja is available via `pip` and can be installed via\n\n`pip install makejinja`\n\nBeware that depending on other packages installed on your system via pip, there may be incompatibilities.\nThus, we advise leveraging [`pipx`](https://github.com/pypa/pipx) instead:\n\n`pipx install makejinja`\n\nYou can then directly invoke the app as follows:\n\n`makejinja --input ./data/input --output ./data/output`\n\n### Nix\n\nIf you use the `nix` package manager, you can add this repository as an input to your flake and use `makejinja.packages.${system}.default`.\nYou can also run it directly\n\n`nix run github:mirkolenz/makejinja -- --input ./data/input --output ./data/output`\n\n### Docker\n\nWe automatically publish an image at `ghcr.io/mirkolenz/makejinja`.\nTo use it, mount a folder to the container and pass the options as the command.\n\n`docker run --rm -v $(pwd)/data:/data ghcr.io/mirkolenz/makejinja:latest --input /data/input --output /data/output`\n\n## Usage\n\nIn its default configuration, makejinja searches the input folder recursively for files ending in `.jinja`.\nAlso, we copy all contents (except raw template files) of the input folder to the output folder and remove the `.jinja` ending during the render process.\nTo get an overview of the remaining options, we advise you to run `makejinja --help`:\n\n<!-- echo -e "\\n```txt\\n$(COLUMNS=120 poetry run makejinja --help)\\n```" >> README.md -->\n\n```txt\n\n Usage: makejinja [OPTIONS]\n\n makejinja can be used to automatically generate files from Jinja templates.\n Instead of passing CLI options, you can also write them to a file called .makejinja.toml in your working directory.\n Note: In this file, options may be named differently. Please refer to the file makejinja/config.py to see their actual\n names. You will also find an example here: makejinja/tests/data/.makejinja.toml.\n\n╭─ Input/Output ───────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ *  --input                DIRECTORY  Path to a folder containing template files. It is passed to Jinja\'s             │\n│                                      FileSystemLoader when creating the environment.                                 │\n│                                      [required]                                                                      │\n│ *  --output               DIRECTORY  Path to a folder where the rendered templates are stored. makejinja preserves   │\n│                                      the relative paths in the process, meaning that you can even use it on nested   │\n│                                      directories.                                                                    │\n│                                      [required]                                                                      │\n│    --input-pattern        TEXT       Glob pattern to search for files in input_folder. Accepts all pattern supported │\n│                                      by fnmatch. If a file is matched by this pattern and does not end with the      │\n│                                      specified jinja-suffix, it is copied over to the output_folder. Note: Do not    │\n│                                      add a special suffix used by your template files here, instead use the          │\n│                                      jinja-suffix option.                                                            │\n│                                      [default: **/*]                                                                 │\n│    --jinja-suffix         TEXT       File ending of Jinja template files. All files with this suffix in input_folder │\n│                                      matched by pattern are passed to the Jinja renderer. Note: Should be provided   │\n│                                      with the leading dot.                                                           │\n│                                      [default: .jinja]                                                               │\n│    --copy-tree                       If your input_folder containes additional files besides Jinja templates, you    │\n│                                      may want to copy them to output_folder as well. This operation maintains the    │\n│                                      metadata of all files and folders, meaning that tools like rsync will treat     │\n│                                      them exactly like the original ones. Note: Even if set to no-copy-tree, files   │\n│                                      that are matched by your provided pattern within input_folder are still copied  │\n│                                      over. In both cases, a file\'s metadata is untouched. The main difference is     │\n│                                      that with copy-tree, folders keep their metadata while matched files are copied │\n│                                      to newly-created subfolders that differ in their metadata.                      │\n│    --keep-jinja-suffix               Decide whether the specified jinja-suffix is removed from the file after        │\n│                                      rendering.                                                                      │\n│    --keep-empty                      Some Jinja template files may be empty after rendering (e.g., if they only      │\n│                                      contain macros that are imported by other templates). By default, we do not     │\n│                                      copy such empty files. If there is a need to have them available anyway, you    │\n│                                      can adjust that.                                                                │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Jinja Environment ──────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --data           PATH       Load variables from yaml/yml/toml files for use in your Jinja templates. The defintions  │\n│                             are passed to Jinja\'s render function. Can either be a file or a folder containg files.  │\n│                             Note: This option may be passed multiple times to pass a list of values. If multiple     │\n│                             files are supplied, beware that previous declarations will be overwritten by newer ones. │\n│ --loader         TEXT       Use custom Python code to adjust the used Jinja environment to your needs. The specified │\n│                             Python file should export a class containing a subset of the following functions:        │\n│                             filters, globals, data, and extensions. In addition, you may add an __init__ function    │\n│                             that recives two positional arguments: the created Jinja environment and the data parsed │\n│                             from the files supplied to makejinja\'s data option. This allows you to apply aribtrary   │\n│                             logic to makejinja. An import path can be specified either in dotted notation            │\n│                             (your.custom.Loader) or with a colon as object delimiter (your.custom:Loader). Note:     │\n│                             This option may be passed multiple times to pass a list of values.                       │\n│ --import-path    DIRECTORY  In order to load custom loaders or Jinja extensions, the PYTHONPATH variable needs to be │\n│                             patched. By default, makejinja will look for modules in your current directory, but you  │\n│                             may change that.                                                                         │\n│                             [default: .]                                                                             │\n│ --extension      TEXT       List of Jinja extensions to use as strings of import paths. An overview of the built-in  │\n│                             ones can be found on the project website. Note: This option may be passed multiple times │\n│                             to pass a list of values.                                                                │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Jinja Whitespace ───────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --lstrip-blocks/--no-lstrip-blocks          If this is set to True, leading spaces and tabs are stripped from the    │\n│                                             start of a line to a block.                                              │\n│                                             [default: lstrip-blocks]                                                 │\n│ --trim-blocks/--no-trim-blocks              If this is set to True, the first newline after a block is removed       │\n│                                             (block, not variable tag!).                                              │\n│                                             [default: trim-blocks]                                                   │\n│ --keep-trailing-newline                     Preserve the trailing newline when rendering templates. The default is   │\n│                                             False, which causes a single newline, if present, to be stripped from    │\n│                                             the end of the template.                                                 │\n│ --newline-sequence                    TEXT  The sequence that starts a newline. The default is tailored for          │\n│                                             UNIX-like systems (Linux/macOS).                                         │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Jinja Delimiters ───────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --delimiter-block-start       TEXT  The string marking the beginning of a block.                                     │\n│                                     [default: {%]                                                                    │\n│ --delimiter-block-end         TEXT  The string marking the end of a block.                                           │\n│                                     [default: %}]                                                                    │\n│ --delimiter-comment-start     TEXT  The string marking the beginning of a comment.                                   │\n│                                     [default: {#]                                                                    │\n│ --delimiter-comment-end       TEXT  The string marking the end of a comment.                                         │\n│                                     [default: #}]                                                                    │\n│ --delimiter-variable-start    TEXT  The string marking the beginning of a print statement.                           │\n│                                     [default: {{]                                                                    │\n│ --delimiter-variable-end      TEXT  The string marking the end of a print statement.                                 │\n│                                     [default: }}]                                                                    │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Jinja Prefixes ─────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --prefix-line-statement    TEXT  If given and a string, this will be used as prefix for line based statements.       │\n│ --prefix-line-comment      TEXT  If given and a string, this will be used as prefix for line based comments.         │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --help      Show this message and exit.                                                                              │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n```\n',
+    'long_description': '# makejinja\n\nmakejinja can be used to automatically generate files from [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/templates/).\nThis allows you to load variables from external files or create repeating patterns via loops.\nIt is conceptually similar to [gomplate](https://github.com/hairyhenderson/gomplate), but is built on Python and Jinja instead of Go.\nA use case for this tool is generating config files for [Home Assistant](https://www.home-assistant.io/):\nUsing the same language that the built-in templates use, you can greatly simplify your configuration.\n\n## Home Assistant Example\n\n[A concrete example for Home Assistant can be found in the tests directory.](./tests/data)\n\n## Features\n\n- Recursively convert nested directories containing template files. One can even specify a pattern to specify relevant files in a folder.\n- Load data files containing variables to use in your Jinja templates from YAML, TOML, and Python files.\n- Use custom functions in your Jinja templates by loading custom filters and/or globals.\n- Easily load bundled as well as custom Jinja extensions.\n- Tailor the whitespace behavior to your needs.\n- Use custom delimiters for Jinja blocks/comments/variables.\n- Modify _all_ init options for the Jinja environment.\n- Write custom **Python loaders** that implement a subset of our fully typed [abstract loader class](./makejinja/loader.py)\n\n## Installation\n\nWe support multiple installation methods: pip, nix, and docker.\n\n### PIP\n\nmakejinja is available via `pip` and can be installed via\n\n`pip install makejinja`\n\nBeware that depending on other packages installed on your system via pip, there may be incompatibilities.\nThus, we advise leveraging [`pipx`](https://github.com/pypa/pipx) instead:\n\n`pipx install makejinja`\n\nYou can then directly invoke the app as follows:\n\n`makejinja --input ./data/input --output ./data/output`\n\n### Nix\n\nIf you use the `nix` package manager, you can add this repository as an input to your flake and use `makejinja.packages.${system}.default`.\nYou can also run it directly\n\n`nix run github:mirkolenz/makejinja -- --input ./data/input --output ./data/output`\n\n### Docker\n\nWe automatically publish an image at `ghcr.io/mirkolenz/makejinja`.\nTo use it, mount a folder to the container and pass the options as the command.\n\n`docker run --rm -v $(pwd)/data:/data ghcr.io/mirkolenz/makejinja:latest --input /data/input --output /data/output`\n\n## Usage\n\nIn its default configuration, makejinja searches the input folder recursively for files ending in `.jinja`.\nAlso, we copy all contents (except raw template files) of the input folder to the output folder and remove the `.jinja` ending during the render process.\nTo get an overview of the remaining options, we advise you to run `makejinja --help`:\n\n<!-- echo -e "\\n```txt\\n$(COLUMNS=120 poetry run makejinja --help)\\n```" >> README.md -->\n\n```txt\n\n Usage: makejinja [OPTIONS]\n\n makejinja can be used to automatically generate files from Jinja templates.\n Instead of passing CLI options, you can also write them to a file called .makejinja.toml in your working directory.\n Note: In this file, options may be named differently. Please refer to the file makejinja/config.py to see their actual\n names. You will also find an example here: makejinja/tests/data/.makejinja.toml.\n\n╭─ Input/Output ───────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ *  --input                DIRECTORY  Path to a folder containing template files. It is passed to Jinja\'s             │\n│                                      FileSystemLoader when creating the environment. Note: This option may be passed │\n│                                      multiple times to pass a list of values. If a template exists in multiple       │\n│                                      inputs, the last value with be used.                                            │\n│                                      [required]                                                                      │\n│ *  --output               DIRECTORY  Path to a folder where the rendered templates are stored. makejinja preserves   │\n│                                      the relative paths in the process, meaning that you can even use it on nested   │\n│                                      directories.                                                                    │\n│                                      [required]                                                                      │\n│    --input-pattern        TEXT       Glob pattern to search for files in input_folder. Accepts all pattern supported │\n│                                      by fnmatch. If a file is matched by this pattern and does not end with the      │\n│                                      specified jinja-suffix, it is copied over to the output_folder. Note: Do not    │\n│                                      add a special suffix used by your template files here, instead use the          │\n│                                      jinja-suffix option.                                                            │\n│                                      [default: **/*]                                                                 │\n│    --exclude-pattern      TEXT       Glob patterns pattern to exclude files matched. Applied against files           │\n│                                      discovered by the input glob. Multiple can be provided.                         │\n│    --jinja-suffix         TEXT       File ending of Jinja template files. All files with this suffix in input_folder │\n│                                      matched by pattern are passed to the Jinja renderer. Note: Should be provided   │\n│                                      with the leading dot.                                                           │\n│                                      [default: .jinja]                                                               │\n│    --keep-jinja-suffix               Decide whether the specified jinja-suffix is removed from the file after        │\n│                                      rendering.                                                                      │\n│    --keep-empty                      Some Jinja template files may be empty after rendering (e.g., if they only      │\n│                                      contain macros that are imported by other templates). By default, we do not     │\n│                                      copy such empty files. If there is a need to have them available anyway, you    │\n│                                      can adjust that.                                                                │\n│    --copy-metadata                   Copy the file metadata (e.g., created/modified/permissions) from the input file │\n│                                      using shutil.copystat                                                           │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Jinja Environment ──────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --data           PATH       Load variables from yaml/yml/toml files for use in your Jinja templates. The defintions  │\n│                             are passed to Jinja\'s render function. Can either be a file or a folder containg files.  │\n│                             Note: This option may be passed multiple times to pass a list of values. If multiple     │\n│                             files are supplied, beware that previous declarations will be overwritten by newer ones. │\n│ --loader         TEXT       Use custom Python code to adjust the used Jinja environment to your needs. The specified │\n│                             Python file should export a class containing a subset of the following functions:        │\n│                             filters, globals, data, and extensions. In addition, you may add an __init__ function    │\n│                             that recives two positional arguments: the created Jinja environment and the data parsed │\n│                             from the files supplied to makejinja\'s data option. This allows you to apply aribtrary   │\n│                             logic to makejinja. An import path can be specified either in dotted notation            │\n│                             (your.custom.Loader) or with a colon as object delimiter (your.custom:Loader). Note:     │\n│                             This option may be passed multiple times to pass a list of values.                       │\n│ --import-path    DIRECTORY  In order to load custom loaders or Jinja extensions, the PYTHONPATH variable needs to be │\n│                             patched. By default, makejinja will look for modules in your current directory, but you  │\n│                             may change that.                                                                         │\n│                             [default: .]                                                                             │\n│ --extension      TEXT       List of Jinja extensions to use as strings of import paths. An overview of the built-in  │\n│                             ones can be found on the project website. Note: This option may be passed multiple times │\n│                             to pass a list of values.                                                                │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Jinja Whitespace ───────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --lstrip-blocks/--no-lstrip-blocks          If this is set to True, leading spaces and tabs are stripped from the    │\n│                                             start of a line to a block.                                              │\n│                                             [default: lstrip-blocks]                                                 │\n│ --trim-blocks/--no-trim-blocks              If this is set to True, the first newline after a block is removed       │\n│                                             (block, not variable tag!).                                              │\n│                                             [default: trim-blocks]                                                   │\n│ --keep-trailing-newline                     Preserve the trailing newline when rendering templates. The default is   │\n│                                             False, which causes a single newline, if present, to be stripped from    │\n│                                             the end of the template.                                                 │\n│ --newline-sequence                    TEXT  The sequence that starts a newline. The default is tailored for          │\n│                                             UNIX-like systems (Linux/macOS).                                         │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Jinja Delimiters ───────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --delimiter-block-start       TEXT  The string marking the beginning of a block.                                     │\n│                                     [default: {%]                                                                    │\n│ --delimiter-block-end         TEXT  The string marking the end of a block.                                           │\n│                                     [default: %}]                                                                    │\n│ --delimiter-comment-start     TEXT  The string marking the beginning of a comment.                                   │\n│                                     [default: {#]                                                                    │\n│ --delimiter-comment-end       TEXT  The string marking the end of a comment.                                         │\n│                                     [default: #}]                                                                    │\n│ --delimiter-variable-start    TEXT  The string marking the beginning of a print statement.                           │\n│                                     [default: {{]                                                                    │\n│ --delimiter-variable-end      TEXT  The string marking the end of a print statement.                                 │\n│                                     [default: }}]                                                                    │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Jinja Prefixes ─────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --prefix-line-statement    TEXT  If given and a string, this will be used as prefix for line based statements.       │\n│ --prefix-line-comment      TEXT  If given and a string, this will be used as prefix for line based comments.         │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --help      Show this message and exit.                                                                              │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n```\n',
     'author': 'Mirko Lenz',
     'author_email': 'mirko@mirkolenz.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mirkolenz/makejinja',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `makejinja-1.1.5b4/PKG-INFO` & `makejinja-2.0.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: makejinja
-Version: 1.1.5b4
+Version: 2.0.0b1
 Summary: Automatically generate files based on Jinja templates. Use it to easily generate complex Home Assistant dashboards!
 Home-page: https://github.com/mirkolenz/makejinja
 License: MIT
 Author: Mirko Lenz
 Author-email: mirko@mirkolenz.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
-Requires-Dist: typed-settings (>=23.0.0,<24.0.0)
+Requires-Dist: typed-settings (>=23.0.1,<24.0.0)
 Project-URL: Repository, https://github.com/mirkolenz/makejinja
 Description-Content-Type: text/markdown
 
 # makejinja
 
 makejinja can be used to automatically generate files from [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/templates/).
 This allows you to load variables from external files or create repeating patterns via loops.
@@ -90,44 +90,42 @@
  makejinja can be used to automatically generate files from Jinja templates.
  Instead of passing CLI options, you can also write them to a file called .makejinja.toml in your working directory.
  Note: In this file, options may be named differently. Please refer to the file makejinja/config.py to see their actual
  names. You will also find an example here: makejinja/tests/data/.makejinja.toml.
 
 ╭─ Input/Output ───────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ *  --input                DIRECTORY  Path to a folder containing template files. It is passed to Jinja's             │
-│                                      FileSystemLoader when creating the environment.                                 │
+│                                      FileSystemLoader when creating the environment. Note: This option may be passed │
+│                                      multiple times to pass a list of values. If a template exists in multiple       │
+│                                      inputs, the last value with be used.                                            │
 │                                      [required]                                                                      │
 │ *  --output               DIRECTORY  Path to a folder where the rendered templates are stored. makejinja preserves   │
 │                                      the relative paths in the process, meaning that you can even use it on nested   │
 │                                      directories.                                                                    │
 │                                      [required]                                                                      │
 │    --input-pattern        TEXT       Glob pattern to search for files in input_folder. Accepts all pattern supported │
 │                                      by fnmatch. If a file is matched by this pattern and does not end with the      │
 │                                      specified jinja-suffix, it is copied over to the output_folder. Note: Do not    │
 │                                      add a special suffix used by your template files here, instead use the          │
 │                                      jinja-suffix option.                                                            │
 │                                      [default: **/*]                                                                 │
+│    --exclude-pattern      TEXT       Glob patterns pattern to exclude files matched. Applied against files           │
+│                                      discovered by the input glob. Multiple can be provided.                         │
 │    --jinja-suffix         TEXT       File ending of Jinja template files. All files with this suffix in input_folder │
 │                                      matched by pattern are passed to the Jinja renderer. Note: Should be provided   │
 │                                      with the leading dot.                                                           │
 │                                      [default: .jinja]                                                               │
-│    --copy-tree                       If your input_folder containes additional files besides Jinja templates, you    │
-│                                      may want to copy them to output_folder as well. This operation maintains the    │
-│                                      metadata of all files and folders, meaning that tools like rsync will treat     │
-│                                      them exactly like the original ones. Note: Even if set to no-copy-tree, files   │
-│                                      that are matched by your provided pattern within input_folder are still copied  │
-│                                      over. In both cases, a file's metadata is untouched. The main difference is     │
-│                                      that with copy-tree, folders keep their metadata while matched files are copied │
-│                                      to newly-created subfolders that differ in their metadata.                      │
 │    --keep-jinja-suffix               Decide whether the specified jinja-suffix is removed from the file after        │
 │                                      rendering.                                                                      │
 │    --keep-empty                      Some Jinja template files may be empty after rendering (e.g., if they only      │
 │                                      contain macros that are imported by other templates). By default, we do not     │
 │                                      copy such empty files. If there is a need to have them available anyway, you    │
 │                                      can adjust that.                                                                │
+│    --copy-metadata                   Copy the file metadata (e.g., created/modified/permissions) from the input file │
+│                                      using shutil.copystat                                                           │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Jinja Environment ──────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --data           PATH       Load variables from yaml/yml/toml files for use in your Jinja templates. The defintions  │
 │                             are passed to Jinja's render function. Can either be a file or a folder containg files.  │
 │                             Note: This option may be passed multiple times to pass a list of values. If multiple     │
 │                             files are supplied, beware that previous declarations will be overwritten by newer ones. │
 │ --loader         TEXT       Use custom Python code to adjust the used Jinja environment to your needs. The specified │
```

