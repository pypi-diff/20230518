# Comparing `tmp/dan-build-0.2.0.tar.gz` & `tmp/dan-build-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dan-build-0.2.0.tar", last modified: Tue May 16 12:28:02 2023, max compression
+gzip compressed data, was "dan-build-0.2.1.tar", last modified: Thu May 18 18:41:29 2023, max compression
```

## Comparing `dan-build-0.2.0.tar` & `dan-build-0.2.1.tar`

### file list

```diff
@@ -1,88 +1,97 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.467818 dan-build-0.2.0/
--rw-rw-rw-   0        0        0     1092 2023-05-13 13:14:52.000000 dan-build-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     3629 2023-05-16 12:28:02.467818 dan-build-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1828 2023-05-13 16:18:25.000000 dan-build-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.340174 dan-build-0.2.0/completion/
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.355119 dan-build-0.2.0/completion/bash/
--rw-rw-rw-   0        0        0      654 2023-05-13 16:11:33.000000 dan-build-0.2.0/completion/bash/dan.sh
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.368085 dan-build-0.2.0/dan/
--rw-rw-rw-   0        0        0      365 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/__init__.py
--rw-rw-rw-   0        0        0       65 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/__main__.py
--rw-rw-rw-   0        0        0    11767 2023-05-13 16:18:25.000000 dan-build-0.2.0/dan/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.371077 dan-build-0.2.0/dan/cmake/
--rw-rw-rw-   0        0        0       51 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cmake/__init__.py
--rw-rw-rw-   0        0        0     1886 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cmake/configure_file.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.375067 dan-build-0.2.0/dan/conan/
--rw-rw-rw-   0        0        0       34 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/conan/__init__.py
--rw-rw-rw-   0        0        0     3117 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/conan/requirements.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.414959 dan-build-0.2.0/dan/core/
--rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/__init__.py
--rw-rw-rw-   0        0        0      933 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/aiofiles.py
--rw-rw-rw-   0        0        0     9952 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/asyncio.py
--rw-rw-rw-   0        0        0     3029 2023-05-14 09:30:30.000000 dan-build-0.2.0/dan/core/cache.py
--rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/detect.py
--rw-rw-rw-   0        0        0      100 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/errors.py
--rw-rw-rw-   0        0        0     1951 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/find.py
--rw-rw-rw-   0        0        0     1053 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/functools.py
--rw-rw-rw-   0        0        0     1063 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/generator.py
--rw-rw-rw-   0        0        0     5669 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/core/include.py
--rw-rw-rw-   0        0        0     4670 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/core/makefile.py
--rw-rw-rw-   0        0        0    14158 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/osinfo.py
--rw-rw-rw-   0        0        0      814 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/pathlib.py
--rw-rw-rw-   0        0        0     1100 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/pm.py
--rw-rw-rw-   0        0        0      602 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/register.py
--rw-rw-rw-   0        0        0     4461 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/core/requirements.py
--rw-rw-rw-   0        0        0     5733 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/runners.py
--rw-rw-rw-   0        0        0     2322 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/settings.py
--rw-rw-rw-   0        0        0    15715 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/core/target.py
--rw-rw-rw-   0        0        0     4634 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/test.py
--rw-rw-rw-   0        0        0     1672 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/utils.py
--rw-rw-rw-   0        0        0     4203 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/core/version.py
--rw-rw-rw-   0        0        0     3407 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/win.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.424932 dan-build-0.2.0/dan/cxx/
--rw-rw-rw-   0        0        0     2678 2023-05-13 16:18:25.000000 dan-build-0.2.0/dan/cxx/__init__.py
--rw-rw-rw-   0        0        0     1395 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cxx/compile_commands.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.428922 dan-build-0.2.0/dan/cxx/data/
--rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cxx/data/__init__.py
--rwxrwxrwx   0        0        0       29 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cxx/data/detect.cmd
--rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cxx/data/empty.c
--rw-rw-rw-   0        0        0    21030 2023-05-13 16:18:25.000000 dan-build-0.2.0/dan/cxx/detect.py
--rw-rw-rw-   0        0        0     5974 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cxx/msvc_toolchain.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.431914 dan-build-0.2.0/dan/cxx/support/
--rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cxx/support/__init__.py
--rw-rw-rw-   0        0        0     3524 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cxx/support/qt.py
--rw-rw-rw-   0        0        0    17115 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/cxx/targets.py
--rw-rw-rw-   0        0        0     7231 2023-05-14 12:16:57.000000 dan-build-0.2.0/dan/cxx/toolchain.py
--rw-rw-rw-   0        0        0     6509 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cxx/unix_toolchain.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.437901 dan-build-0.2.0/dan/io/
--rw-rw-rw-   0        0        0       35 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/io/__init__.py
--rw-rw-rw-   0        0        0     8536 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/io/package.py
--rw-rw-rw-   0        0        0     1662 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/io/repositories.py
--rw-rw-rw-   0        0        0     1679 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/jinja.py
--rw-rw-rw-   0        0        0     4023 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/logging.py
--rw-rw-rw-   0        0        0    15674 2023-05-13 23:45:04.000000 dan-build-0.2.0/dan/make.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.441889 dan-build-0.2.0/dan/pkgconfig/
--rw-rw-rw-   0        0        0       71 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/pkgconfig/__init__.py
--rw-rw-rw-   0        0        0     9318 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/pkgconfig/package.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.444880 dan-build-0.2.0/dan/pkgconfig/templates/
--rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/pkgconfig/templates/__init__.py
--rw-rw-rw-   0        0        0      429 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/pkgconfig/templates/pkg.pc.jinja2
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.449866 dan-build-0.2.0/dan/smc/
--rw-rw-rw-   0        0        0       56 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/smc/__init__.py
--rw-rw-rw-   0        0        0     1833 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/smc/git.py
--rw-rw-rw-   0        0        0     1033 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/smc/tar.py
--rw-rw-rw-   0        0        0       37 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/testing.py
--rw-rw-rw-   0        0        0     6360 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/vscode.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.461834 dan-build-0.2.0/dan_build.egg-info/
--rw-rw-rw-   0        0        0     3629 2023-05-16 12:28:02.000000 dan-build-0.2.0/dan_build.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1511 2023-05-16 12:28:02.000000 dan-build-0.2.0/dan_build.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 12:28:02.000000 dan-build-0.2.0/dan_build.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-16 12:28:02.000000 dan-build-0.2.0/dan_build.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      102 2023-05-16 12:28:02.000000 dan-build-0.2.0/dan_build.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-16 12:28:02.000000 dan-build-0.2.0/dan_build.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1313 2023-05-16 12:21:25.000000 dan-build-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 12:28:02.468815 dan-build-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.465823 dan-build-0.2.0/tests/
--rw-rw-rw-   0        0        0     3114 2023-05-13 15:47:33.000000 dan-build-0.2.0/tests/test_cxx_libraries.py
--rw-rw-rw-   0        0        0     2950 2023-05-13 15:47:33.000000 dan-build-0.2.0/tests/test_cxx_simple.py
--rw-rw-rw-   0        0        0     2268 2023-05-13 13:04:49.000000 dan-build-0.2.0/tests/test_cxx_smc_catch2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-18 18:41:19.000000 dan-build-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-05-18 18:41:29.241839 dan-build-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-18 18:41:19.000000 dan-build-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.233839 dan-build-0.2.1/completion/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.233839 dan-build-0.2.1/completion/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-18 18:41:19.000000 dan-build-0.2.1/completion/bash/dan-io.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-18 18:41:19.000000 dan-build-0.2.1/completion/bash/dan.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.233839 dan-build-0.2.1/completion/zsh/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-18 18:41:19.000000 dan-build-0.2.1/completion/zsh/dan-io.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-18 18:41:19.000000 dan-build-0.2.1/completion/zsh/dan.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.233839 dan-build-0.2.1/dan/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.237839 dan-build-0.2.1/dan/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cli/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cli/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cli/vscode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.237839 dan-build-0.2.1/dan/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cmake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cmake/configure_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.237839 dan-build-0.2.1/dan/conan/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/conan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/conan/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.237839 dan-build-0.2.1/dan/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/aiofiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/osinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/win.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/dan/cxx/
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/compile_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/dan/cxx/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/data/detect.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/data/empty.c
+-rw-r--r--   0 runner    (1001) docker     (123)    21030 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/msvc_toolchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/dan/cxx/support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/support/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/unix_toolchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/dan/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/io/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/io/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/make.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/dan/pkgconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/pkgconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/pkgconfig/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/dan/pkgconfig/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/pkgconfig/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/pkgconfig/templates/pkg.pc.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/dan/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/src/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/src/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/src/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/dan_build.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-05-18 18:41:29.000000 dan-build-0.2.1/dan_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-18 18:41:29.000000 dan-build-0.2.1/dan_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:41:29.000000 dan-build-0.2.1/dan_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-18 18:41:29.000000 dan-build-0.2.1/dan_build.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-18 18:41:29.000000 dan-build-0.2.1/dan_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-18 18:41:29.000000 dan-build-0.2.1/dan_build.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-18 18:41:19.000000 dan-build-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 18:41:29.241839 dan-build-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-18 18:41:19.000000 dan-build-0.2.1/tests/test_cxx_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-18 18:41:19.000000 dan-build-0.2.1/tests/test_cxx_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-18 18:41:19.000000 dan-build-0.2.1/tests/test_cxx_smc_catch2.py
```

### Comparing `dan-build-0.2.0/LICENSE` & `dan-build-0.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Sylvain Garcia
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Sylvain Garcia
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `dan-build-0.2.0/completion/bash/dan.sh` & `dan-build-0.2.1/completion/bash/dan.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/cli.py` & `dan-build-0.2.1/dan/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,24 @@
-import inspect
 import os
 import sys
 
 from dan.core.find import find_file
 from dan.core.pathlib import Path
-import click
+from dan.cli import click
 
 import logging
 import asyncio
 from dan.core.cache import Cache
 from dan.cxx.targets import Executable
 
 
 from dan.make import ConfigCache, InstallMode, Make
-from dan.vscode import Code
+from dan.cli.vscode import Code
 
 
-class AsyncContext(click.Context):
-    def invoke(__self, __callback, *args, **kwargs):
-        ret = super().invoke(__callback, *args, **kwargs)
-        if inspect.isawaitable(ret):
-            loop = asyncio.get_event_loop()
-            if loop.is_running():
-                return ret  # must be awaited
-            return loop.run_until_complete(ret)
-        else:
-            return ret
-
-
-click.BaseCommand.context_class = AsyncContext
-
-
-_logger = logging.getLogger('cli')
-
 _minimal_options = [
     click.option('--build-path', '-B', 'path', help='Path where dan has been initialized.',
                  type=click.Path(resolve_path=True, path_type=Path), required=True, default='build', envvar='DAN_BUILD_PATH'),
 
 ]
 
 _common_opts = [
@@ -87,14 +69,15 @@
         return self._make
 
 
 pass_context = click.make_pass_decorator(CommandsContext)
 
 
 @click.group()
+@click.version_option(package_name='dan-build')
 @click.option('--quiet', '-q', is_flag=True,
               help='Dont print informations (errors only)')
 @click.option('--verbose', '-v', is_flag=True,
               help='Pring debug informations')
 @click.option('--jobs', '-j',
               help='Maximum jobs', default=None, type=int)
 @click.pass_context
@@ -124,16 +107,16 @@
 async def configure(verbose: bool, toolchain: str, settings: tuple[str], options: tuple[str], build_path: Path, source_path: Path):
     """Configure dan project"""
     logging.getLogger().setLevel(logging.DEBUG if verbose else logging.INFO)
     config = ConfigCache(build_path / Make._config_name, )
     config.data.source_path = config.data.source_path if hasattr(
         config, 'source_path') else str(source_path)
     config.data.build_path = str(build_path)
-    _logger.info(f'source path: {config.data.source_path}')
-    _logger.info(f'build path: {config.data.build_path}')
+    click.logger.info(f'source path: {config.data.source_path}')
+    click.logger.info(f'build path: {config.data.build_path}')
     config.data.toolchain = toolchain or config.data.toolchain or click.prompt('Toolchain', type=_toolchain_choice, default='default')
     await config.save()
     Cache.ignore(config)
     del config
 
     if len(settings) or len(options):
         make = Make(build_path, None, verbose, False)
@@ -194,20 +177,20 @@
                  for mf in f.readlines()]
     to_be_removed = '\n'.join([f" - {f}" for f in files])
     yes = yes or click.confirm(
         f'Following files will be removed:\n {to_be_removed}\nProceed ?')
     if yes:
         def rm_empty(dir: Path):
             if dir.is_empty:
-                _logger.debug(f'removing empty directory: {dir}')
+                click.logger.debug(f'removing empty directory: {dir}')
                 os.rmdir(dir)
                 rm_empty(dir.parent)
 
         for f in files:
-            _logger.debug(f'removing: {f}')
+            click.logger.debug(f'removing: {f}')
             os.remove(f)
             rm_empty(f.parent)
 
         os.remove(manifest)
         rm_empty(manifest.parent)
 
 @cli.group()
@@ -240,15 +223,19 @@
 @pass_context
 async def tests(ctx: CommandsContext, **kwargs):
     """List tests"""
     kwargs['quiet'] = True
     ctx(**kwargs)
     await ctx.make.initialize()
     for t in ctx.make.tests:
-        click.echo(t.fullname)
+        if len(t) > 1:
+            for c in t.cases:
+                click.echo(f'{t.fullname}:{c.name}')
+        else:
+            click.echo(t.fullname)
 
 @ls.command()
 @common_opts
 @pass_context
 async def options(ctx: CommandsContext, **kwargs):
     """List tests"""
     kwargs['quiet'] = True
@@ -328,14 +315,31 @@
             'output': str(target.output),
             'executable': isinstance(target, Executable),
             'type': type(target).__name__
         })
     import json
     click.echo(json.dumps(out))
 
+@code.command()
+@common_opts
+@pass_context
+async def get_tests(ctx: CommandsContext, **kwargs):
+    kwargs['quiet'] = True
+    ctx(**kwargs)
+    await ctx.make.initialize()
+    from dan.core.include import context
+    import json
+    out = list()
+    for t in context.root.all_tests:
+        out.append(t.fullname)
+        if len(t) > 1:
+            for c in t.cases:
+                out.append(f'{t.fullname}:{c.name}')
+    click.echo(json.dumps(out))
+
 
 @code.command()
 @common_opts
 @click.option('--pretty', is_flag=True)
 @pass_context
 async def get_test_suites(ctx: CommandsContext, pretty, **kwargs):
     kwargs['quiet'] = True
@@ -380,17 +384,17 @@
 
 
 def main():
     import sys
     try:
         cli(auto_envvar_prefix='DAN')
     except Exception as err:
-        _logger.error(str(err))
+        click.logger.error(str(err))
         _ex_type, _ex, tb = sys.exc_info()
         import traceback
-        _logger.debug(' '.join(traceback.format_tb(tb)))
+        click.logger.debug(' '.join(traceback.format_tb(tb)))
         try:
             # wait asyncio loop to terminate
             asyncio.get_running_loop().run_until_complete()
         except Exception:
             pass
         return -1
```

### Comparing `dan-build-0.2.0/dan/cmake/configure_file.py` & `dan-build-0.2.1/dan/cmake/configure_file.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/conan/requirements.py` & `dan-build-0.2.1/dan/conan/requirements.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/core/aiofiles.py` & `dan-build-0.2.1/dan/core/aiofiles.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/core/asyncio.py` & `dan-build-0.2.1/dan/core/asyncio.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/core/cache.py` & `dan-build-0.2.1/dan/core/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         self.__dirty = False
         self.__caches[self.name] = self
     
     def _dump(self):
         if self.dataclass == dict:
             return json.dumps(self.data, indent=self.indent)
         else:
-            return self.data.to_json()
+            return self.data.to_json(indent=self.indent)
 
     
     @property
     def path(self):
         return self.__path
     
     @property
@@ -61,16 +61,16 @@
     @property
     def dirty(self):
         if not self.__dirty:
             self.__state = self._dump()
             self.__dirty = self.__initial_state != self.__state
         return self.__dirty
     
-    async def save(self):
-        if self.path and self.dirty:
+    async def save(self, force=False):
+        if self.path and (self.dirty or force):
             if self.__state:
                 self.path.parent.mkdir(exist_ok=True, parents=True)
                 async with aiofiles.open(self.path, 'w') as f:
                     await f.write(self.__state)
 
     @classmethod
     async def save_all(cls):
```

### Comparing `dan-build-0.2.0/dan/core/find.py` & `dan-build-0.2.1/dan/core/find.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/core/functools.py` & `dan-build-0.2.1/dan/core/functools.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/core/generator.py` & `dan-build-0.2.1/dan/core/generator.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/core/include.py` & `dan-build-0.2.1/dan/core/include.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/core/makefile.py` & `dan-build-0.2.1/dan/core/makefile.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/core/osinfo.py` & `dan-build-0.2.1/dan/core/osinfo.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/core/pathlib.py` & `dan-build-0.2.1/dan/core/pathlib.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/core/pm.py` & `dan-build-0.2.1/dan/core/pm.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/core/register.py` & `dan-build-0.2.1/dan/core/register.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/core/requirements.py` & `dan-build-0.2.1/dan/core/requirements.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,49 @@
 from dan.core import asyncio
 from dan.core.pm import re_match
 from dan.core.settings import InstallMode, InstallSettings
 
 from dan.core.version import Version, VersionSpec
 from dan.logging import Logging
 
+def parse_package(name: str) -> tuple[str, str, str]:
+    """Parse package name
+    
+    :returns: package, library, repository"""
+    match re_match(name):
+        # full specification <pkg>:<lib>@<repo>
+        case r'(.+?):(.+?)@(.+)' as m:
+            package = m[1]
+            library = m[2]
+            repository = m[3]
+        # repo specification <lib>@<repo>
+        case r'(.+?)@(.+)' as m:
+            package = None
+            library = m[1]
+            repository = m[2]
+        # package specification <pkg>:<lib>
+        case r'(.+?):(.+)' as m:
+            package = m[1]
+            library = m[2]
+            repository = None
+        # no specification, automatic resolution in default repository
+        case _:
+            package = None
+            library = name
+            repository = None
+    
+    return package, library, repository
+
 
 class RequiredPackage(Logging):
     def __init__(self, name: str, version_spec: VersionSpec = None):
         self.version_spec = version_spec
         super().__init__(name)
         self.target : 'Target' = None
-
-        match re_match(name):
-            case r'(.+?)@(.+)' as m:
-                self.name = m[1]
-                self.provider = m[2]
-            case _:
-                self.name = name
-                self.provider = None
+        self.package, self.name, self.repository = parse_package(name)
 
     def is_compatible(self, t: 'Target'):
         if self.version_spec is not None:
             version_ok = self.version_spec.is_compatible(t.version)
         else:
             version_ok = True
         return t.name == self.name and version_ok
@@ -104,17 +125,17 @@
                 if makefile.requirements:
                     # install requirement from dan-requires.py
                     t = makefile.requirements.find(req.name)
                     if not t:
                         raise RuntimeError(f'Unresolved requirement {req}, it should have been defined in {makefile.requirements.__file__}')
                     logger.debug('%s using requirements\' target %s', req, t.fullname)
                 else:
-                    t = Package(req.name, req.version_spec, repository=req.provider, makefile=makefile)
+                    t = Package(req.name, req.version_spec, package=req.package, repository=req.repository, makefile=makefile)
                     logger.debug('%s: adding package %s', req, t.fullname)
-                unresolved.append(req)                
+                unresolved.append(req)
                 group.create_task(t.install(deps_settings, InstallMode.dev))
 
 
 
     if install:
         for req in unresolved:
             pkg = find_package(req.name, req.version_spec, search_paths=pkgs_search_paths, makefile=makefile)
```

### Comparing `dan-build-0.2.0/dan/core/runners.py` & `dan-build-0.2.1/dan/core/runners.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/core/settings.py` & `dan-build-0.2.1/dan/core/settings.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/core/target.py` & `dan-build-0.2.1/dan/core/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,43 +212,38 @@
         return iter(self.__items)
 
 
 class Target(Logging, MakefileRegister, internal=True):
     name: str = None
     fullname: str = None
     description: str = None,
-    version: str = None
     default: bool = True
     installed: bool = False
     output: Path = None
     options: dict[str, Any] = dict()
 
     dependencies: set[TargetDependencyLike] = set()
     preload_dependencies: set[TargetDependencyLike] = set()
 
     def __init__(self,
                  name: str = None,
                  parent: 'Target' = None,
                  version: str = None,
                  default: bool = None,
                  makefile=None) -> None:
-        if isinstance(self.version, str):
-            self.version = Version(self.version)
+        
         self.parent = parent
         self.__cache: dict = None
 
         if name is not None:
             self.name = name
 
         if self.name is None:
             self.name = self.__class__.__name__
 
-        if version is not None:
-            self.version = version
-
         if default is not None:
             self.default = default
 
         if parent is not None:
             self.makefile = parent.makefile
             self.fullname = f'{parent.fullname}.{self.name}'
 
@@ -260,16 +255,19 @@
 
 
         if self.fullname is None:
             self.fullname = f'{self.makefile.fullname}.{self.name}'
 
         self.options = Options(self, self.options)
 
-        if self.version is None:
-            self.version = self.makefile.version
+        if version is not None:
+            self._version = version
+
+        if not hasattr(self, '_version'):
+            self._version = self.makefile.version
 
         if self.description is None:
             self.description = self.makefile.description
 
         self.other_generated_files: set[Path] = set()
         self.dependencies = Dependencies(self, self.dependencies)
         self.preload_dependencies = Dependencies(
@@ -287,14 +285,27 @@
 
     
     @property
     def output(self):
         if self._output is None:
             return None
         return self.build_path / self._output
+    
+    @property
+    def version(self):
+        version = self._version
+        if isinstance(version, Option):
+            version = version.value
+        if isinstance(version, str):
+            version = Version(version)
+        return version
+
+    @version.setter
+    def version(self, value):
+        self._version = value
 
     @output.setter
     def output(self, path):
         path = Path(path)
         if path.is_absolute() and self.build_path in path.parents:
             raise RuntimeError(f'output must not be an absolute path within build directory')
         self._output = path
```

### Comparing `dan-build-0.2.0/dan/core/test.py` & `dan-build-0.2.1/dan/core/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 class AsyncExecutable(Logging):
     async def execute(self, *args, **kwargs): ...
 
 
 class Case:
-    def __init__(self, name, *args, expected_result=0, expected_output=None, file=None, lineno=None, strip_output=True, normalize_newlines=True):
+    def __init__(self, name, *args, expected_result: int = 0, expected_output: str = None, file=None, lineno=None, strip_output=True, normalize_newlines=True):
         self.name = name
         self.args = args
         self.expected_result = expected_result
         self.file = file
         self.lineno = lineno
         self.expected_output = expected_output
         self.strip_output = strip_output
@@ -95,30 +95,35 @@
                 msg += '\nstdout: ' + out
             if err:
                 msg += '\nstderr: ' + err
             raise RuntimeError(msg)
 
         if caze.expected_output is not None:
 
+            if callable(caze.expected_output):
+                expected_output = caze.expected_output(caze)
+            else:
+                expected_output = caze.expected_output
+
             if caze.strip_output:
                 out = out.strip()
 
             if caze.normalize_newlines:
                 out = out.replace(os.linesep, '\n')
 
-            if isinstance(caze.expected_output, re.Pattern):
-                if not caze.expected_output.match(out):
+            if isinstance(expected_output, re.Pattern):
+                if not expected_output.match(out):
                     out = out.strip()
                     err = err.strip()
-                    msg = f'Test \'{name}\' failed (output: {out}, expected: {caze.expected_output}) !'
+                    msg = f'Test \'{name}\' failed (output: {out}, expected: {expected_output}) !'
                     raise RuntimeError(msg)
-            elif out != caze.expected_output:
+            elif out != expected_output:
                 out = out.strip()
                 err = err.strip()
-                msg = f'Test \'{name}\' failed (output: {out}, expected: {caze.expected_output.strip()}) !'
+                msg = f'Test \'{name}\' failed (output: {out}, expected: {expected_output.strip()}) !'
                 raise RuntimeError(msg)
 
     async def run_test(self):
         try:
             async with asyncio.TaskGroup(f'running {self.name} tests') as tests:
                 for caze in self.cases:
                     tests.create_task(self._run_test(caze))
```

### Comparing `dan-build-0.2.0/dan/core/utils.py` & `dan-build-0.2.1/dan/core/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,20 @@
 def unique(*seqs):
     seen = set()
     full = list()
     for seq in seqs:
         full.extend(seq)
     return [x for x in full if not (x in seen or seen.add(x))]
 
+
+def chunks(lst, chunk_size):
+    for ii in range(0, len(lst), chunk_size):
+        yield lst[ii:ii + chunk_size]
+
+
 class _ClassPropertyDescriptor(object):
 
     def __init__(self, fget, fset=None):
         self.fget = fget
         self.fset = fset
 
     def __get__(self, obj, klass=None):
```

### Comparing `dan-build-0.2.0/dan/core/version.py` & `dan-build-0.2.1/dan/core/version.py`

 * *Files 22% similar despite different names*

```diff
@@ -42,14 +42,29 @@
     def __eq__(self, other):
         if isinstance(other, str):
             other = Version(other)
         elif not isinstance(other, Version):
             return False
         if self.major != other.major:
             return False
+        if self.minor != other.minor:
+            return False
+        if self.patch != other.patch:
+            return False
+        if self.build != other.build:
+            return False
+        return True
+    
+    def is_compatible(self, other):
+        if isinstance(other, str):
+            other = Version(other)
+        elif not isinstance(other, Version):
+            return False
+        if self.major != other.major:
+            return False
         if self.minor and other.minor and self.minor != other.minor:
             return False
         if self.patch and other.patch and self.patch != other.patch:
             return False
         if self.build and other.build and self.build != other.build:
             return False
         return True
@@ -60,23 +75,28 @@
         elif not isinstance(other, Version):
             return False
         for mine, their in zip(self._parts, other._parts):
             if mine > their:
                 return True
             if mine < their:
                 return False
-        return False
+        return True
 
 
     def __ge__(self, other: 'Version'):
         if isinstance(other, str):
             other = Version(other)
         elif not isinstance(other, Version):
             return False
-        return self.__eq__(other) or self.__gt__(other)
+        for mine, their in zip(self._parts, other._parts):
+            if mine >= their:
+                return True
+            if mine < their:
+                return False
+        return False
     
     def __lt__(self, other: 'Version'):
         if isinstance(other, str):
             other = Version(other)
         elif not isinstance(other, Version):
             return False
         for mine, their in zip(self._parts, other._parts):
@@ -88,28 +108,39 @@
 
     
     def __le__(self, other: 'Version'):
         if isinstance(other, str):
             other = Version(other)
         elif not isinstance(other, Version):
             return False
-        return self.__eq__(other) or self.__le__(other)
+        for mine, their in zip(self._parts, other._parts):
+            if mine < their:
+                return True
+            if mine > their:
+                return False
+        return True
 
     def __str__(self) -> str:
         res = str(self.major)
         if self.minor is not None:
             res += f'.{self.minor}'
             if self.patch is not None:
                 res += f'.{self.patch}'
                 if self.build is not None:
                     res += f'.{self.build}'
         return res
     
     def __repr__(self) -> str:
         return f'Version[{self}]'
+    
+    def __hash__(self) -> int:
+        h = 0
+        for part in self._parts:
+            h ^= hash(part)
+        return h
 
 
 class VersionSpec:
 
     @staticmethod
     def parse(data: str) -> tuple[str|None, 'VersionSpec']:
         m = re.match(r'(.+?)?\s+?([><]=?|=)\s+([\d\.]+)', data)
@@ -123,16 +154,18 @@
 
     def __init__(self, version: Version, op: str) -> None:
         self.version = version
         self.op = op
         
     def is_compatible(self, version: Version):
         match self.op:
-            case '==' | '=':
+            case '==':
                 return version == self.version
+            case '=':
+                return version.is_compatible(self.version)
             case '>':
                 return version > self.version
             case '>=':
                 return version >= self.version
             case '<':
                 return version < self.version
             case '<=':
```

### Comparing `dan-build-0.2.0/dan/core/win.py` & `dan-build-0.2.1/dan/core/win.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/cxx/__init__.py` & `dan-build-0.2.1/dan/cxx/__init__.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/cxx/compile_commands.py` & `dan-build-0.2.1/dan/cxx/compile_commands.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/cxx/detect.py` & `dan-build-0.2.1/dan/cxx/detect.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/cxx/msvc_toolchain.py` & `dan-build-0.2.1/dan/cxx/msvc_toolchain.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/cxx/support/qt.py` & `dan-build-0.2.1/dan/cxx/support/qt.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/cxx/targets.py` & `dan-build-0.2.1/dan/cxx/targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from enum import Enum
 from functools import cached_property
 
 from dan.core.pathlib import Path
 from dan.core import aiofiles, cache
 from dan.core.settings import InstallMode, InstallSettings
 from dan.core.target import Target
-from dan.core.utils import unique
+from dan.core.utils import chunks, unique
 from dan.core.runners import async_run
 from dan.core import asyncio
 
 
 class CXXObject(Target, internal=True):
     def __init__(self, source:Path, parent: 'CXXTarget') -> None:
         super().__init__(source.stem, parent=parent, default=False)
@@ -424,16 +424,21 @@
                             header.relative_to(public_include_dir)
                         tasks.append(do_install(header, dest))
 
             for obj in self.objs:
                 for dbg_file in self.toolchain.debug_files(obj.output):
                     tasks.append(do_install(dbg_file, settings.libraries_destination / dbg_file.name))
 
-        return await asyncio.gather(super().install(settings, mode), *tasks)
+        tasks.insert(0, super().install(settings, mode))
 
+        result = list()
+        for tchunk in chunks(tasks, 100):
+            result.append(await asyncio.gather(*tchunk))
+
+        return result
 
 class Module(CXXObjectsTarget, internal=True):
     def __init__(self, name: str, sources: list[str], *args, **kwargs):
         super().__init__(name, sources, *args, **kwargs)
 
     @property
     def cxx_flags(self):
```

### Comparing `dan-build-0.2.0/dan/cxx/toolchain.py` & `dan-build-0.2.1/dan/cxx/toolchain.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/cxx/unix_toolchain.py` & `dan-build-0.2.1/dan/cxx/unix_toolchain.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/jinja.py` & `dan-build-0.2.1/dan/jinja.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/logging.py` & `dan-build-0.2.1/dan/logging.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import tqdm
-import logging
+from logging import *
 from termcolor import colored
 
 
 def merge(lhs, rhs):
     if type(lhs) != type(rhs):
         raise RuntimeError(f'cannot merge {type(lhs)} with {rhs}')
     if type(lhs) == dict:
@@ -22,15 +22,15 @@
         self.fn = fn
         self.args = args
 
     def __call__(self, *args, **kwds):
         return self.fn(*args, *self.args, **kwds)
 
 
-class ColoredFormatter(logging.Formatter):
+class ColoredFormatter(Formatter):
 
     COLORS = {
         'WARNING': bind_back(colored, 'yellow'),
         'INFO': bind_back(colored, 'green'),
         'DEBUG': bind_back(colored, 'cyan'),
         'CRITICAL': bind_back(colored, 'yellow'),
         'ERROR': bind_back(colored, 'red')
@@ -67,62 +67,62 @@
         return super().format(record)
 
 
 _color_formatter = ColoredFormatter()
 _no_color_formatter = ColoredFormatter(use_color=False)
 
 
-class TqdmHandler(logging.Handler):
+class TqdmHandler(Handler):
     def emit(self, record):
         tqdm.tqdm.write(self.format(record))
 
 
-def setup_logger(logger: logging.Logger):
+def setup_logger(logger: Logger):
     if not logger.hasHandlers():
         console = TqdmHandler()
         console.setFormatter(_color_formatter)
         logger.addHandler(console)
     else:
         for handler in logger.handlers:
             handler.setFormatter(_color_formatter if isinstance(
-                handler, logging.StreamHandler) else _no_color_formatter)
+                handler, StreamHandler) else _no_color_formatter)
 
 
-class ColoredLogger(logging.Logger):
+class ColoredLogger(Logger):
 
     def __init__(self, name):
         super().__init__(name)
         self.propagate = False
         setup_logger(self)
 
 
-logging.setLoggerClass(ColoredLogger)
+setLoggerClass(ColoredLogger)
 
 
 class Logging:
     def __init__(self, name: str = None) -> None:
         if name is None:
             name = self.__class__.__name__
         if name.startswith('root.'):
             name = name.removeprefix('root.')
-        self._logger = logging.getLogger(name)
+        self._logger = getLogger(name)
         self.debug = self._logger.debug
         self.info = self._logger.info
         self.warning = self._logger.warning
         self.error = self._logger.error
 
 
 def _get_makefile_logger():
     from dan.core.include import context
     if not hasattr(context.current, '_logger'):
-        makefile_logger = logging.getLogger(context.current.name)
+        makefile_logger = getLogger(context.current.name)
         setup_logger(makefile_logger)
         setattr(context.current, '_logger', makefile_logger)
     else:
-        makefile_logger: logging.Logger = getattr(
+        makefile_logger: Logger = getattr(
             context.current, '_logger')
     return makefile_logger
 
 
 def debug(*args, **kwds):
     return _get_makefile_logger().debug(*args, **kwds)
```

### Comparing `dan-build-0.2.0/dan/make.py` & `dan-build-0.2.1/dan/make.py`

 * *Files 6% similar despite different names*

```diff
@@ -169,26 +169,27 @@
 
     @functools.cached_property
     def tests(self) -> list[Test]:
         from dan.core.include import context
         items = list()
         if self.required_targets and len(self.required_targets) > 0:
             for required in self.required_targets:
+                test_name, *test_case = required.split(':')
+                test_case = test_case[0] if len(test_case) else None
+
                 for test in context.root.all_tests:
-                    if len(test) > 1 and required.startswith(test.fullname):
-                        case_name = required.removeprefix(test.fullname + '.')
-                        cases = list()
-                        for case in test.cases:
-                            if fnmatch.fnmatch(case.name, case_name):
-                                cases.append(case)
-                        test.cases = cases
-                        items.append(test)
-                        continue
                     
-                    if required.startswith(test.fullname) or fnmatch.fnmatch(test.fullname, f'*{required}*'):
+                    if fnmatch.fnmatch(test.fullname, f'*{test_name}*'):
+                        if len(test) > 1 and test_case is not None:
+                            cases = list()
+                            for case in test.cases:
+                                if fnmatch.fnmatch(case.name, test_case):
+                                    cases.append(case)
+                            test.cases = cases
+                        
                         items.append(test)
         else:
             for test in context.root.all_tests:
                 items.append(test)
         return items
 
     @property
@@ -214,32 +215,32 @@
             target._init_sources()
             if source.name in target.sources:
                 return target
 
 
     @classmethod
     def _parse_str_value(cls, name, value: str, orig: type, tp: type = None):
-        if issubclass(orig, str):
-            return value
-        elif issubclass(orig, Enum):
+        if issubclass(orig, Enum):
             names = [n.lower()
                         for n in orig._member_names_]
             value = value.lower()
             if value in names:
                 return orig(names.index(value))
             else:
                 raise RuntimeError(f'{name} should be one of {names}')
         elif issubclass(orig, (set, list)):
             assert tp is not None
             result = list()
             for sub in value.split(';'):
                 result.append(cls._parse_str_value(name, sub, tp))
             return orig(result)
         else:
-            raise TypeError(f'unhandled type {orig}')
+            if tp is not None:
+                raise TypeError(f'unhandled type {orig}[{tp}]')
+            return orig(value)
 
     
     @classmethod
     def _apply_inputs(self, inputs: list[str], get_item: t.Callable[[str], tuple[t.Any, t.Any, t.Any]], info: t.Callable[[t.Any], t.Any]):
         for input in inputs:
             m = re.match(r'(.+?)([+-])?="?(.+)"?', input)
             if m:
@@ -251,14 +252,15 @@
                 if orig is None:
                     orig = type(input)
                 if hasattr(orig, '__annotations__') and sname in orig.__annotations__:
                     tp = orig.__annotations__[sname]
                     orig = t.get_origin(tp)
                     if orig is None:
                         orig = tp
+                        tp = None
                     else:
                         args = t.get_args(tp)
                         if args:
                             tp = args[0]
                 else:
                     tp = None
                 in_value = self._parse_str_value(name, value, orig, tp)
```

### Comparing `dan-build-0.2.0/dan/pkgconfig/package.py` & `dan-build-0.2.1/dan/pkgconfig/package.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/smc/git.py` & `dan-build-0.2.1/dan/src/git.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/dan/vscode.py` & `dan-build-0.2.1/dan/cli/vscode.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         from dan.core.include import context, MakeFile
         from dan.core.test import Test, Case
         from dan.cxx import Executable
 
         def make_inner_test_info(test: Test, case: Case):
             basename = test.basename(case)
             out, err = test.outs(case)
-            ident = f'{test.fullname}.{case.name}' if case .name is not None else test.fullname
+            ident = f'{test.fullname}:{case.name}' if case.name is not None else test.fullname
             info = {
                 'type': 'test',
                 'id': ident,
                 'label': basename,
                 'debuggable': False,
                 'target': test.executable.fullname,
                 'out': str(out),
```

### Comparing `dan-build-0.2.0/tests/test_cxx_libraries.py` & `dan-build-0.2.1/tests/test_cxx_libraries.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/tests/test_cxx_simple.py` & `dan-build-0.2.1/tests/test_cxx_simple.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.0/tests/test_cxx_smc_catch2.py` & `dan-build-0.2.1/tests/test_cxx_smc_catch2.py`

 * *Files identical despite different names*

